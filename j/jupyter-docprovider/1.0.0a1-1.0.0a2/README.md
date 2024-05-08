# Comparing `tmp/jupyter_docprovider-1.0.0a1.tar.gz` & `tmp/jupyter_docprovider-1.0.0a2.tar.gz`

## Comparing `jupyter_docprovider-1.0.0a1.tar` & `jupyter_docprovider-1.0.0a2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/install.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/setup.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/_version.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/package.json
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/341.998da4ec9a27d6dbdb1a.js
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/422.3ab44960b241aac9f303.js
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/544.1c4f1124ffffdb64812e.js
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/722.06cb6508a379f7976e9e.js
--rw-r--r--   0        0        0     8193 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/944.80e0d65b220a1dfdc0ff.js
--rw-r--r--   0        0        0    13097 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/994.c290665e94ae9503337f.js
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/remoteEntry.6347eb8bae6b74aa4edc.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/style.js
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/babel.config.js
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/jest.config.js
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/package.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/tsconfig.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/tsconfig.test.json
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/awareness.ts
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/index.ts
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/requests.ts
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/tokens.ts
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/utils.ts
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/ydrive.ts
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/yprovider.ts
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider/src/__tests__/yprovider.spec.ts
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/README.md
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/package.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/tsconfig.json
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/executor.ts
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/filebrowser.ts
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/index.ts
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/style/index.css
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/packages/docprovider-extension/style/index.js
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/LICENSE
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/README.md
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/install.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/setup.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/_version.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/package.json
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/341.ee0b3dfba7c4aa24f62b.js
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/422.3ab44960b241aac9f303.js
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/544.8aa72b83c45d4c8bffa7.js
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/722.377e3bdce002f0b0ca9e.js
+-rw-r--r--   0        0        0     8193 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/944.80e0d65b220a1dfdc0ff.js
+-rw-r--r--   0        0        0    13097 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/994.c290665e94ae9503337f.js
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/remoteEntry.4aa297cefdfc2dc35259.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/style.js
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/babel.config.js
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/jest.config.js
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/package.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/tsconfig.json
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/tsconfig.test.json
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/src/awareness.ts
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/src/index.ts
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/src/requests.ts
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/src/tokens.ts
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/src/utils.ts
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/src/ydrive.ts
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/src/yprovider.ts
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider/src/__tests__/yprovider.spec.ts
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider-extension/README.md
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider-extension/package.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider-extension/tsconfig.json
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider-extension/src/executor.ts
+-rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider-extension/src/filebrowser.ts
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider-extension/src/index.ts
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider-extension/style/index.css
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/packages/docprovider-extension/style/index.js
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/README.md
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 jupyter_docprovider-1.0.0a2/PKG-INFO
```

### Comparing `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/package.json` & `jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9685606060606061%*

 * *Differences: {"'dependencies'": "{'@jupyter/docprovider': '^3.0.0-alpha.2', '@jupyter/ydoc': '^2.0.0', "*

 * *                   "'@jupyterlab/application': '^4.2.0', '@jupyterlab/apputils': '^4.2.0', "*

 * *                   "'@jupyterlab/docregistry': '^4.2.0', '@jupyterlab/filebrowser': '^4.2.0', "*

 * *                   "'@jupyterlab/fileeditor': '^4.2.0', '@jupyterlab/logconsole': '^4.2.0', "*

 * *                   "'@jupyterlab/notebook': '^4.2.0', '@jupyterlab/settingregistry': '^4.2.0', "*

 * *                   "'@jupyterlab/transla […]*

```diff
@@ -1,24 +1,24 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/docprovider": "^3.0.0-alpha.1",
-        "@jupyter/ydoc": "^1.1.0-a0",
-        "@jupyterlab/application": "^4.2.0-beta.0",
-        "@jupyterlab/apputils": "^4.2.0-beta.0",
-        "@jupyterlab/docregistry": "^4.2.0-beta.0",
-        "@jupyterlab/filebrowser": "^4.2.0-beta.0",
-        "@jupyterlab/fileeditor": "^4.2.0-beta.0",
-        "@jupyterlab/logconsole": "^4.2.0-beta.0",
-        "@jupyterlab/notebook": "^4.2.0-beta.0",
-        "@jupyterlab/settingregistry": "^4.2.0-beta.0",
-        "@jupyterlab/translation": "^4.2.0-beta.0",
+        "@jupyter/docprovider": "^3.0.0-alpha.2",
+        "@jupyter/ydoc": "^2.0.0",
+        "@jupyterlab/application": "^4.2.0",
+        "@jupyterlab/apputils": "^4.2.0",
+        "@jupyterlab/docregistry": "^4.2.0",
+        "@jupyterlab/filebrowser": "^4.2.0",
+        "@jupyterlab/fileeditor": "^4.2.0",
+        "@jupyterlab/logconsole": "^4.2.0",
+        "@jupyterlab/notebook": "^4.2.0",
+        "@jupyterlab/settingregistry": "^4.2.0",
+        "@jupyterlab/translation": "^4.2.0",
         "@lumino/commands": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Collaborative Shared Models",
     "devDependencies": {
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-collaboration",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6347eb8bae6b74aa4edc.js",
+            "load": "static/remoteEntry.4aa297cefdfc2dc35259.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "@jupyterlab/filebrowser-extension:defaultFileBrowser",
             "@jupyterlab/notebook-extension:cell-executor"
         ],
         "extension": true,
@@ -119,9 +119,9 @@
     "typedoc": {
         "displayName": "@jupyter/docprovider-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.1"
+    "version": "3.0.0-alpha.2"
 }
```

### Comparing `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/341.998da4ec9a27d6dbdb1a.js` & `jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/341.ee0b3dfba7c4aa24f62b.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -42,17 +42,17 @@
                         t = i.xv();
                     i.zd(t, o.CHAT), i.Qj(t, JSON.stringify(s)), this.ws.send(i.Fo(t))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            var h = t(655),
-                d = t(824),
-                _ = t(440),
+            var h = t(702),
+                d = t(861),
+                _ = t(923),
                 l = t(262);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, _.showErrorMessage)(this._trans.__("Document session error"), e.reason, [_.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
```

### Comparing `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/422.3ab44960b241aac9f303.js` & `jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/422.3ab44960b241aac9f303.js`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/544.1c4f1124ffffdb64812e.js` & `jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/544.8aa72b83c45d4c8bffa7.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 "use strict";
 (self.webpackChunk_jupyter_docprovider_extension = self.webpackChunk_jupyter_docprovider_extension || []).push([
     [544], {
         544: (e, o, t) => {
             t.r(o), t.d(o, {
                 default: () => _
             });
-            var r, n = t(371),
-                i = t(440),
-                a = t(943),
-                s = t(716),
-                l = t(312),
-                c = t(506),
-                d = t(500),
-                u = t(844),
-                v = t(667),
-                p = t(835);
+            var r, n = t(626),
+                i = t(923),
+                a = t(670),
+                s = t(441),
+                l = t(557),
+                c = t(291),
+                d = t(825),
+                u = t(265),
+                v = t(697),
+                p = t(438);
             ! function(e) {
                 e.openPath = "filebrowser:open-path"
             }(r || (r = {}));
             const g = {
                     id: "@jupyter/docprovider-extension:drive",
                     description: "The default collaborative drive provider",
                     provides: p.ICollaborativeDrive,
@@ -139,16 +139,16 @@
                             path: l.browser,
                             dontShowBrowser: !0
                         })) : (await e.model.restore(e.id), await e.model.refresh()), e.removeClass(a), (null == i ? void 0 : i.isEmpty("main")) && o.execute("launcher:create")
                     };
                     t.routed.connect(s)
                 }
             }(b || (b = {}));
-            var f = t(655),
-                k = t(824);
+            var f = t(702),
+                k = t(861);
             async function x({
                 cell: e,
                 notebook: o,
                 notebookConfig: t,
                 onCellExecuted: r,
                 onCellExecutionScheduled: n,
                 sessionContext: i,
```

### Comparing `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/722.06cb6508a379f7976e9e.js` & `jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/722.377e3bdce002f0b0ca9e.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -42,17 +42,17 @@
                         t = i.xv();
                     i.zd(t, o.CHAT), i.Qj(t, JSON.stringify(s)), this.ws.send(i.Fo(t))
                 }
                 _onUserChanged(e) {
                     this._awareness.setLocalStateField("user", e.identity)
                 }
             }
-            var h = t(655),
-                d = t(824),
-                _ = t(440),
+            var h = t(702),
+                d = t(861),
+                _ = t(923),
                 l = t(262);
             class p {
                 constructor(e) {
                     this._onConnectionClosed = e => {
                         1003 === e.code && (console.error("Document provider closed:", e.reason), (0, _.showErrorMessage)(this._trans.__("Document session error"), e.reason, [_.Dialog.okButton()]), this._sharedModel.dispose())
                     }, this._onSync = e => {
                         var s;
```

### Comparing `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/944.80e0d65b220a1dfdc0ff.js` & `jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/944.80e0d65b220a1dfdc0ff.js`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/994.c290665e94ae9503337f.js` & `jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/994.c290665e94ae9503337f.js`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/remoteEntry.6347eb8bae6b74aa4edc.js` & `jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/remoteEntry.4aa297cefdfc2dc35259.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, o, a, n, i, l, u, f, s, d, p, c, h, v, b, y, g, m, j, w = {
+    var e, r, t, o, a, n, i, l, u, d, f, s, c, p, h, v, b, y, g, m, j, w = {
             496: (e, r, t) => {
                 var o = {
-                        "./index": () => Promise.all([t.e(393), t.e(544)]).then((() => () => t(544))),
-                        "./extension": () => Promise.all([t.e(393), t.e(544)]).then((() => () => t(544))),
+                        "./index": () => Promise.all([t.e(74), t.e(544)]).then((() => () => t(544))),
+                        "./extension": () => Promise.all([t.e(74), t.e(544)]).then((() => () => t(544))),
                         "./style": () => t.e(944).then((() => () => t(944)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -43,63 +43,63 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        206: "346950b0376f11c0b868",
-        341: "998da4ec9a27d6dbdb1a",
-        393: "39aa8f8542ebf94ba223",
+        74: "1aed62da05965a23df58",
+        206: "849ac6f72ee27b29de19",
+        341: "ee0b3dfba7c4aa24f62b",
         422: "3ab44960b241aac9f303",
-        544: "1c4f1124ffffdb64812e",
-        652: "282f02247000ea4106c5",
-        722: "06cb6508a379f7976e9e",
+        544: "8aa72b83c45d4c8bffa7",
+        652: "54e538f1662afe1004a8",
+        722: "377e3bdce002f0b0ca9e",
         944: "80e0d65b220a1dfdc0ff",
         994: "c290665e94ae9503337f"
     } [e] + ".js?v=" + {
-        206: "346950b0376f11c0b868",
-        341: "998da4ec9a27d6dbdb1a",
-        393: "39aa8f8542ebf94ba223",
+        74: "1aed62da05965a23df58",
+        206: "849ac6f72ee27b29de19",
+        341: "ee0b3dfba7c4aa24f62b",
         422: "3ab44960b241aac9f303",
-        544: "1c4f1124ffffdb64812e",
-        652: "282f02247000ea4106c5",
-        722: "06cb6508a379f7976e9e",
+        544: "8aa72b83c45d4c8bffa7",
+        652: "54e538f1662afe1004a8",
+        722: "377e3bdce002f0b0ca9e",
         944: "80e0d65b220a1dfdc0ff",
         994: "c290665e94ae9503337f"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyter/docprovider-extension:", S.l = (t, o, a, n) => {
         if (e[t]) e[t].push(o);
         else {
             var i, l;
             if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        i = s;
+                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
+                    var f = u[d];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [o];
-            var d = (r, o) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var s = (r, o) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(o))), r) return r(o)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -121,15 +121,15 @@
                         (!l || !l.loaded && (!o != !l.eager ? o : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyter/docprovider-extension", "3.0.0-alpha.1", (() => Promise.all([S.e(393), S.e(544)]).then((() => () => S(544))))), l("@jupyter/docprovider", "3.0.0-alpha.1", (() => Promise.all([S.e(422), S.e(652), S.e(393), S.e(341)]).then((() => () => S(341))))), l("y-websocket", "1.5.4", (() => Promise.all([S.e(422), S.e(994), S.e(206)]).then((() => () => S(994)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyter/docprovider-extension", "3.0.0-alpha.2", (() => Promise.all([S.e(74), S.e(544)]).then((() => () => S(544))))), l("@jupyter/docprovider", "3.0.0-alpha.2", (() => Promise.all([S.e(422), S.e(652), S.e(74), S.e(341)]).then((() => () => S(341))))), l("y-websocket", "1.5.4", (() => Promise.all([S.e(422), S.e(994), S.e(206)]).then((() => () => S(994)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -179,84 +179,84 @@
     }, n = (e, r) => {
         if (0 in e) {
             r = t(r);
             var o = e[0],
                 a = o < 0;
             a && (o = -o - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > o && !a : "" == d != a);
-                if ("u" == s) {
-                    if (!u || "u" != d) return !1
+                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == s ? l > o && !a : "" == s != a);
+                if ("u" == f) {
+                    if (!u || "u" != s) return !1
                 } else if (u)
-                    if (d == s)
+                    if (s == f)
                         if (l <= o) {
-                            if (f != e[l]) return !1
+                            if (d != e[l]) return !1
                         } else {
-                            if (a ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (a ? d > e[l] : d < e[l]) return !1;
+                            d != e[l] && (u = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != s && "n" != s) {
                     if (a || l <= o) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= o || s < d != a) return !1;
+                    if (l <= o || f < s != a) return !1;
                     u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? n(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? n(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, u = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(o) + ")", f = (e, r, t, o) => {
+    }, u = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(o) + ")", d = (e, r, t, o) => {
         var a = l(e, t);
-        return n(o, a) || d(u(e, t, a, o)), p(e[t][a])
-    }, s = (e, r, t) => {
+        return n(o, a) || s(u(e, t, a, o)), c(e[t][a])
+    }, f = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !n(t, r) || e && !o(e, r) ? e : r), 0)) && a[r]
-    }, d = e => {
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, o, a) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, o, a) {
         var n = S.I(r);
         return n && n.then ? n.then(e.bind(e, r, S.S[r], t, o, a)) : e(r, S.S[r], t, o, a)
-    })(((e, r, t, o) => (i(e, t), f(r, 0, t, o)))), v = c(((e, r, t, o, a) => r && S.o(r, t) ? f(r, 0, t, o) : a())), b = c(((e, r, t, o, a) => {
-        var n = r && S.o(r, t) && s(r, t, o);
-        return n ? p(n) : a()
+    })(((e, r, t, o) => (i(e, t), d(r, 0, t, o)))), v = p(((e, r, t, o, a) => r && S.o(r, t) ? d(r, 0, t, o) : a())), b = p(((e, r, t, o, a) => {
+        var n = r && S.o(r, t) && f(r, t, o);
+        return n ? c(n) : a()
     })), y = {}, g = {
-        440: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
-        655: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
-        824: () => h("default", "@jupyterlab/services", [1, 7, 1, 8]),
-        312: () => h("default", "@jupyterlab/logconsole", [1, 4, 1, 8]),
-        371: () => h("default", "@jupyterlab/application", [1, 4, 1, 8]),
-        500: () => h("default", "@jupyterlab/settingregistry", [1, 4, 1, 8]),
-        506: () => h("default", "@jupyterlab/notebook", [1, 4, 1, 8]),
-        667: () => h("default", "@jupyter/ydoc", [1, 1, 1, 1]),
-        716: () => h("default", "@jupyterlab/fileeditor", [1, 4, 1, 8]),
-        835: () => v("default", "@jupyter/docprovider", [1, 3, 0, 0, , "alpha", 1], (() => Promise.all([S.e(422), S.e(652), S.e(722)]).then((() => () => S(341))))),
-        844: () => h("default", "@jupyterlab/translation", [1, 4, 1, 8]),
-        943: () => h("default", "@jupyterlab/filebrowser", [1, 4, 1, 8]),
+        702: () => h("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
+        861: () => h("default", "@jupyterlab/services", [1, 7, 2, 0]),
+        923: () => h("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
+        265: () => h("default", "@jupyterlab/translation", [1, 4, 2, 0]),
+        291: () => h("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
+        438: () => v("default", "@jupyter/docprovider", [1, 3, 0, 0, , "alpha", 2], (() => Promise.all([S.e(422), S.e(652), S.e(722)]).then((() => () => S(341))))),
+        441: () => h("default", "@jupyterlab/fileeditor", [1, 4, 2, 0]),
+        557: () => h("default", "@jupyterlab/logconsole", [1, 4, 2, 0]),
+        626: () => h("default", "@jupyterlab/application", [1, 4, 2, 0]),
+        670: () => h("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
+        697: () => h("default", "@jupyter/ydoc", [1, 2, 0, 1]),
+        825: () => h("default", "@jupyterlab/settingregistry", [1, 4, 2, 0]),
         262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
         560: () => b("default", "y-websocket", [1, 1, 3, 15], (() => Promise.all([S.e(994), S.e(206)]).then((() => () => S(994))))),
         602: () => h("default", "@lumino/signaling", [1, 2, 0, 0]),
         206: () => h("default", "yjs", [1, 13, 5, 40])
     }, m = {
+        74: [702, 861, 923],
         206: [206],
-        393: [440, 655, 824],
-        544: [312, 371, 500, 506, 667, 716, 835, 844, 943],
+        544: [265, 291, 438, 441, 557, 626, 670, 697, 825],
         652: [262, 560, 602]
     }, j = {}, S.f.consumes = (e, r) => {
         S.o(m, e) && m[e].forEach((e => {
             if (S.o(y, e)) return r.push(y[e]);
             if (!j[e]) {
                 var t = r => {
                     y[e] = 0, S.m[e] = t => {
@@ -281,15 +281,15 @@
         var e = {
             552: 0
         };
         S.f.j = (r, t) => {
             var o = S.o(e, r) ? e[r] : void 0;
             if (0 !== o)
                 if (o) t.push(o[2]);
-                else if (/^(206|393|652)$/.test(r)) e[r] = 0;
+                else if (/^(206|652|74)$/.test(r)) e[r] = 0;
             else {
                 var a = new Promise(((t, a) => o = e[r] = [t, a]));
                 t.push(o[2] = a);
                 var n = S.p + S.u(r),
                     i = new Error;
                 S.l(n, (t => {
                     if (S.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
```

### Comparing `jupyter_docprovider-1.0.0a1/jupyter_docprovider/labextension/static/third-party-licenses.json` & `jupyter_docprovider-1.0.0a2/jupyter_docprovider/labextension/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '3.0.0-alpha.2'}, 1: {'versionInfo': '3.0.0-alpha.2'}}"}*

```diff
@@ -1,20 +1,20 @@
 {
     "packages": [
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/collaboration",
-            "versionInfo": "3.0.0-alpha.1"
+            "versionInfo": "3.0.0-alpha.2"
         },
         {
             "extractedText": "",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter/docprovider",
-            "versionInfo": "3.0.0-alpha.1"
+            "versionInfo": "3.0.0-alpha.2"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
             "versionInfo": "6.11.0"
         },
```

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider/jest.config.js` & `jupyter_docprovider-1.0.0a2/packages/docprovider/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider/package.json` & `jupyter_docprovider-1.0.0a2/packages/docprovider/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.970679012345679%*

 * *Differences: {"'dependencies'": "{'@jupyter/ydoc': '^2.0.0'}", "'version'": "'3.0.0-alpha.2'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/ydoc": "^1.1.0-a0",
+        "@jupyter/ydoc": "^2.0.0",
         "@jupyterlab/coreutils": "^6.0.5",
         "@jupyterlab/services": "^7.0.5",
         "@lumino/coreutils": "^2.1.0",
         "@lumino/disposable": "^2.1.0",
         "@lumino/signaling": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
@@ -61,9 +61,9 @@
     ],
     "typedoc": {
         "displayName": "@jupyter/docprovider",
         "entryPoint": "./src/index.ts",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.1"
+    "version": "3.0.0-alpha.2"
 }
```

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider/src/awareness.ts` & `jupyter_docprovider-1.0.0a2/packages/docprovider/src/awareness.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider/src/requests.ts` & `jupyter_docprovider-1.0.0a2/packages/docprovider/src/requests.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider/src/tokens.ts` & `jupyter_docprovider-1.0.0a2/packages/docprovider/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider/src/ydrive.ts` & `jupyter_docprovider-1.0.0a2/packages/docprovider/src/ydrive.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider/src/yprovider.ts` & `jupyter_docprovider-1.0.0a2/packages/docprovider/src/yprovider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider-extension/package.json` & `jupyter_docprovider-1.0.0a2/packages/docprovider-extension/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9689393939393939%*

 * *Differences: {"'dependencies'": "{'@jupyter/docprovider': '^3.0.0-alpha.2', '@jupyter/ydoc': '^2.0.0', "*

 * *                   "'@jupyterlab/application': '^4.2.0', '@jupyterlab/apputils': '^4.2.0', "*

 * *                   "'@jupyterlab/docregistry': '^4.2.0', '@jupyterlab/filebrowser': '^4.2.0', "*

 * *                   "'@jupyterlab/fileeditor': '^4.2.0', '@jupyterlab/logconsole': '^4.2.0', "*

 * *                   "'@jupyterlab/notebook': '^4.2.0', '@jupyterlab/settingregistry': '^4.2.0', "*

 * *                   "'@jupyterlab/transla […]*

```diff
@@ -1,24 +1,24 @@
 {
     "author": "Project Jupyter",
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-collaboration/issues"
     },
     "dependencies": {
-        "@jupyter/docprovider": "^3.0.0-alpha.1",
-        "@jupyter/ydoc": "^1.1.0-a0",
-        "@jupyterlab/application": "^4.2.0-beta.0",
-        "@jupyterlab/apputils": "^4.2.0-beta.0",
-        "@jupyterlab/docregistry": "^4.2.0-beta.0",
-        "@jupyterlab/filebrowser": "^4.2.0-beta.0",
-        "@jupyterlab/fileeditor": "^4.2.0-beta.0",
-        "@jupyterlab/logconsole": "^4.2.0-beta.0",
-        "@jupyterlab/notebook": "^4.2.0-beta.0",
-        "@jupyterlab/settingregistry": "^4.2.0-beta.0",
-        "@jupyterlab/translation": "^4.2.0-beta.0",
+        "@jupyter/docprovider": "^3.0.0-alpha.2",
+        "@jupyter/ydoc": "^2.0.0",
+        "@jupyterlab/application": "^4.2.0",
+        "@jupyterlab/apputils": "^4.2.0",
+        "@jupyterlab/docregistry": "^4.2.0",
+        "@jupyterlab/filebrowser": "^4.2.0",
+        "@jupyterlab/fileeditor": "^4.2.0",
+        "@jupyterlab/logconsole": "^4.2.0",
+        "@jupyterlab/notebook": "^4.2.0",
+        "@jupyterlab/settingregistry": "^4.2.0",
+        "@jupyterlab/translation": "^4.2.0",
         "@lumino/commands": "^2.1.0",
         "y-protocols": "^1.0.5",
         "y-websocket": "^1.3.15",
         "yjs": "^13.5.40"
     },
     "description": "JupyterLab - Collaborative Shared Models",
     "devDependencies": {
@@ -114,9 +114,9 @@
     "typedoc": {
         "displayName": "@jupyter/docprovider-extension",
         "entryPoint": "./src/index.ts",
         "readmeFile": "./README.md",
         "tsconfig": "./tsconfig.json"
     },
     "types": "lib/index.d.ts",
-    "version": "3.0.0-alpha.1"
+    "version": "3.0.0-alpha.2"
 }
```

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/executor.ts` & `jupyter_docprovider-1.0.0a2/packages/docprovider-extension/src/executor.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/filebrowser.ts` & `jupyter_docprovider-1.0.0a2/packages/docprovider-extension/src/filebrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/packages/docprovider-extension/src/index.ts` & `jupyter_docprovider-1.0.0a2/packages/docprovider-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/.gitignore` & `jupyter_docprovider-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/LICENSE` & `jupyter_docprovider-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/pyproject.toml` & `jupyter_docprovider-1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_docprovider-1.0.0a1/PKG-INFO` & `jupyter_docprovider-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter-docprovider
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: JupyterLab/Jupyter Notebook 7+ extension integrating collaborative shared models.
 Project-URL: Documentation, https://jupyterlab-realtime-collaboration.readthedocs.io/
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-collaboration
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
         This project is licensed under the terms of the Modified BSD License
```


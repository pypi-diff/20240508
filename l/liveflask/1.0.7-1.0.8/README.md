# Comparing `tmp/liveflask-1.0.7.tar.gz` & `tmp/liveflask-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveflask-1.0.7.tar", last modified: Sat May  4 23:27:59 2024, max compression
+gzip compressed data, was "liveflask-1.0.8.tar", last modified: Wed May  8 11:47:20 2024, max compression
```

## Comparing `liveflask-1.0.7.tar` & `liveflask-1.0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.459731 liveflask-1.0.7/
--rw-rw-rw-   0        0        0     1368 2024-05-04 23:27:59.458729 liveflask-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.411729 liveflask-1.0.7/liveflask/
--rw-rw-rw-   0        0        0     6302 2024-05-04 23:25:43.000000 liveflask-1.0.7/liveflask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.419730 liveflask-1.0.7/liveflask/attributes/
--rw-rw-rw-   0        0        0     2023 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.420729 liveflask-1.0.7/liveflask/attributes/__pycache__/
--rw-rw-rw-   0        0        0     3650 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.422729 liveflask-1.0.7/liveflask/static/
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.433731 liveflask-1.0.7/liveflask/static/liveflask/
--rw-rw-rw-   0        0        0     1566 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/action.js
--rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/constants.js
--rw-rw-rw-   0        0        0      245 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/events.js
--rw-rw-rw-   0        0        0      872 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/liveflask.js
--rw-rw-rw-   0        0        0     2191 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/model.js
--rw-rw-rw-   0        0        0     1660 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/polling.js
--rw-rw-rw-   0        0        0     8475 2024-05-04 23:27:21.000000 liveflask-1.0.7/liveflask/static/liveflask/utils.js
--rw-rw-rw-   0        0        0    73154 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/lodash.min.js
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.436729 liveflask-1.0.7/liveflask/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/templates/liveflask-head.html
--rw-rw-rw-   0        0        0      348 2024-05-04 23:19:29.000000 liveflask-1.0.7/liveflask/templates/liveflask-scripts.html
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.446729 liveflask-1.0.7/liveflask/traits/
--rw-rw-rw-   0        0        0      205 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/Bootable.py
--rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.456728 liveflask-1.0.7/liveflask/traits/__pycache__/
--rw-rw-rw-   0        0        0      867 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
--rw-rw-rw-   0        0        0      198 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3292 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
--rw-rw-rw-   0        0        0     4272 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/has_props.cpython-311.pyc
--rw-rw-rw-   0        0        0     2835 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
--rw-rw-rw-   0        0        0     4776 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
--rw-rw-rw-   0        0        0     2042 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/has_actions.py
--rw-rw-rw-   0        0        0     2488 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/has_props.py
--rw-rw-rw-   0        0        0     2486 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/has_renders.py
--rw-rw-rw-   0        0        0     4106 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/has_snapshots.py
--rw-rw-rw-   0        0        0     2032 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.417729 liveflask-1.0.7/liveflask.egg-info/
--rw-rw-rw-   0        0        0     1368 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1204 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 23:27:59.459731 liveflask-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1222 2024-05-04 23:27:46.000000 liveflask-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.747722 liveflask-1.0.8/
+-rw-rw-rw-   0        0        0     1368 2024-05-08 11:47:20.745721 liveflask-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.686721 liveflask-1.0.8/liveflask/
+-rw-rw-rw-   0        0        0     6302 2024-05-04 23:25:43.000000 liveflask-1.0.8/liveflask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.696721 liveflask-1.0.8/liveflask/attributes/
+-rw-rw-rw-   0        0        0     2023 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.698721 liveflask-1.0.8/liveflask/attributes/__pycache__/
+-rw-rw-rw-   0        0        0     3650 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.700723 liveflask-1.0.8/liveflask/static/
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.714723 liveflask-1.0.8/liveflask/static/liveflask/
+-rw-rw-rw-   0        0        0     1566 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/static/liveflask/action.js
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/static/liveflask/constants.js
+-rw-rw-rw-   0        0        0      245 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/static/liveflask/events.js
+-rw-rw-rw-   0        0        0      872 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/static/liveflask/liveflask.js
+-rw-rw-rw-   0        0        0     2191 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/static/liveflask/model.js
+-rw-rw-rw-   0        0        0     1660 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/static/liveflask/polling.js
+-rw-rw-rw-   0        0        0     9170 2024-05-08 11:46:18.000000 liveflask-1.0.8/liveflask/static/liveflask/utils.js
+-rw-rw-rw-   0        0        0    73154 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/static/lodash.min.js
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.718721 liveflask-1.0.8/liveflask/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/templates/liveflask-head.html
+-rw-rw-rw-   0        0        0      348 2024-05-04 23:19:29.000000 liveflask-1.0.8/liveflask/templates/liveflask-scripts.html
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.729721 liveflask-1.0.8/liveflask/traits/
+-rw-rw-rw-   0        0        0      205 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/Bootable.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.742724 liveflask-1.0.8/liveflask/traits/__pycache__/
+-rw-rw-rw-   0        0        0      867 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
+-rw-rw-rw-   0        0        0      198 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3292 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4272 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/__pycache__/has_props.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2835 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4776 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2042 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/has_actions.py
+-rw-rw-rw-   0        0        0     2488 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/has_props.py
+-rw-rw-rw-   0        0        0     2486 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/has_renders.py
+-rw-rw-rw-   0        0        0     4106 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/traits/has_snapshots.py
+-rw-rw-rw-   0        0        0     2032 2024-05-01 21:07:09.000000 liveflask-1.0.8/liveflask/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:47:20.695724 liveflask-1.0.8/liveflask.egg-info/
+-rw-rw-rw-   0        0        0     1368 2024-05-08 11:47:20.000000 liveflask-1.0.8/liveflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1204 2024-05-08 11:47:20.000000 liveflask-1.0.8/liveflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 11:47:20.000000 liveflask-1.0.8/liveflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-08 11:47:20.000000 liveflask-1.0.8/liveflask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 11:47:20.000000 liveflask-1.0.8/liveflask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 11:47:20.747722 liveflask-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1222 2024-05-08 11:46:40.000000 liveflask-1.0.8/setup.py
```

### Comparing `liveflask-1.0.7/PKG-INFO` & `liveflask-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.7
+Version: 1.0.8
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.7/liveflask/__init__.py` & `liveflask-1.0.8/liveflask/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/attributes/__init__.py` & `liveflask-1.0.8/liveflask/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/attributes/__pycache__/__init__.cpython-311.pyc` & `liveflask-1.0.8/liveflask/attributes/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/static/liveflask/action.js` & `liveflask-1.0.8/liveflask/static/liveflask/action.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/static/liveflask/liveflask.js` & `liveflask-1.0.8/liveflask/static/liveflask/liveflask.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/static/liveflask/model.js` & `liveflask-1.0.8/liveflask/static/liveflask/model.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/static/liveflask/polling.js` & `liveflask-1.0.8/liveflask/static/liveflask/polling.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/static/liveflask/utils.js` & `liveflask-1.0.8/liveflask/static/liveflask/utils.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -135,14 +135,30 @@
             "Content-Type": "application/json",
             "X-CSRF-Token": csrfToken
         },
         body: JSON.stringify({
             snapshot: snapshot,
             ...add_to_payload
         })
+    }).then(response => {
+        if (!response.ok) {
+            if (response.status === 400) {
+                return response.text().then(text => {
+                    if (text.includes("The CSRF token has expired.")) {
+                        // Handle CSRF token expiration here
+                        onpageexpired();
+                    } else {
+                        throw new Error(text);
+                    }
+                });
+            } else {
+                throw new Error('Network response was not ok.');
+            }
+        }
+        return response;
     }).then(i => i.json()).then(response => {
         let {
             html,
             snapshot
         } = response
         el.__liveflask = snapshot
         el.__liveflask['children'] = children
@@ -224,14 +240,19 @@
     }).then(el => {
 
 
     })
 }
 
 
+function onpageexpired() {
+    alert("The CSRF token has expired. Please refresh the page.")
+}
+
+
 function update_dom(el, html) {
     let class_name = el.__liveflask['class']
     html = `<div data-component="${class_name}" id="${el.id}">${html}</div>`
     morphdom(el, html, {
         onBeforeElUpdated: function(fromEl, toEl) {
             // spec - https://dom.spec.whatwg.org/#concept-node-equals
             if (fromEl.isEqualNode(toEl)) {
```

### Comparing `liveflask-1.0.7/liveflask/static/lodash.min.js` & `liveflask-1.0.8/liveflask/static/lodash.min.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/traits/__pycache__/Bootable.cpython-311.pyc` & `liveflask-1.0.8/liveflask/traits/__pycache__/Bootable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/traits/__pycache__/has_actions.cpython-311.pyc` & `liveflask-1.0.8/liveflask/traits/__pycache__/has_actions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/traits/__pycache__/has_props.cpython-311.pyc` & `liveflask-1.0.8/liveflask/traits/__pycache__/has_props.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/traits/__pycache__/has_renders.cpython-311.pyc` & `liveflask-1.0.8/liveflask/traits/__pycache__/has_renders.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc` & `liveflask-1.0.8/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/traits/has_actions.py` & `liveflask-1.0.8/liveflask/traits/has_actions.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/traits/has_props.py` & `liveflask-1.0.8/liveflask/traits/has_props.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/traits/has_renders.py` & `liveflask-1.0.8/liveflask/traits/has_renders.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/traits/has_snapshots.py` & `liveflask-1.0.8/liveflask/traits/has_snapshots.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask/utils.py` & `liveflask-1.0.8/liveflask/utils.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/liveflask.egg-info/PKG-INFO` & `liveflask-1.0.8/liveflask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.7
+Version: 1.0.8
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.7/liveflask.egg-info/SOURCES.txt` & `liveflask-1.0.8/liveflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.7/setup.py` & `liveflask-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="liveflask",
-    version="1.0.7",
+    version="1.0.8",
     author="Jarriq Rolle",
     author_email="jrolle@baysidetechgroup.com",
     description="Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/liveflask",
     packages=['liveflask'],
```


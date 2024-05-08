# Comparing `tmp/liveflask-1.0.9rc1.tar.gz` & `tmp/liveflask-1.0.9rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveflask-1.0.9rc1.tar", last modified: Wed May  8 13:30:04 2024, max compression
+gzip compressed data, was "liveflask-1.0.9rc2.tar", last modified: Wed May  8 15:09:19 2024, max compression
```

## Comparing `liveflask-1.0.9rc1.tar` & `liveflask-1.0.9rc2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.876981 liveflask-1.0.9rc1/
--rw-rw-rw-   0        0        0     1294 2024-05-08 13:30:04.875981 liveflask-1.0.9rc1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.825153 liveflask-1.0.9rc1/liveflask/
--rw-rw-rw-   0        0        0     6326 2024-05-08 13:26:44.000000 liveflask-1.0.9rc1/liveflask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.833392 liveflask-1.0.9rc1/liveflask/attributes/
--rw-rw-rw-   0        0        0     2023 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.835395 liveflask-1.0.9rc1/liveflask/attributes/__pycache__/
--rw-rw-rw-   0        0        0     3654 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.837916 liveflask-1.0.9rc1/liveflask/static/
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.849865 liveflask-1.0.9rc1/liveflask/static/liveflask/
--rw-rw-rw-   0        0        0     1566 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/static/liveflask/action.js
--rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/static/liveflask/constants.js
--rw-rw-rw-   0        0        0      245 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/static/liveflask/events.js
--rw-rw-rw-   0        0        0     1328 2024-05-08 13:29:26.000000 liveflask-1.0.9rc1/liveflask/static/liveflask/init.js
--rw-rw-rw-   0        0        0      894 2024-05-08 13:26:44.000000 liveflask-1.0.9rc1/liveflask/static/liveflask/liveflask.js
--rw-rw-rw-   0        0        0     2191 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/static/liveflask/model.js
--rw-rw-rw-   0        0        0     1660 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/static/liveflask/polling.js
--rw-rw-rw-   0        0        0     9170 2024-05-08 13:26:44.000000 liveflask-1.0.9rc1/liveflask/static/liveflask/utils.js
--rw-rw-rw-   0        0        0    73154 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/static/lodash.min.js
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.852865 liveflask-1.0.9rc1/liveflask/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/templates/liveflask-head.html
--rw-rw-rw-   0        0        0      348 2024-05-08 13:26:44.000000 liveflask-1.0.9rc1/liveflask/templates/liveflask-scripts.html
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.862956 liveflask-1.0.9rc1/liveflask/traits/
--rw-rw-rw-   0        0        0      205 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/Bootable.py
--rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.874983 liveflask-1.0.9rc1/liveflask/traits/__pycache__/
--rw-rw-rw-   0        0        0      871 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
--rw-rw-rw-   0        0        0      202 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3296 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
--rw-rw-rw-   0        0        0     4276 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/__pycache__/has_props.cpython-311.pyc
--rw-rw-rw-   0        0        0     2839 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
--rw-rw-rw-   0        0        0     4780 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
--rw-rw-rw-   0        0        0     2042 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/has_actions.py
--rw-rw-rw-   0        0        0     2488 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/has_props.py
--rw-rw-rw-   0        0        0     2486 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/has_renders.py
--rw-rw-rw-   0        0        0     4106 2024-05-01 20:13:57.000000 liveflask-1.0.9rc1/liveflask/traits/has_snapshots.py
--rw-rw-rw-   0        0        0     2032 2024-05-01 19:41:30.000000 liveflask-1.0.9rc1/liveflask/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:30:04.832391 liveflask-1.0.9rc1/liveflask.egg-info/
--rw-rw-rw-   0        0        0     1294 2024-05-08 13:30:04.000000 liveflask-1.0.9rc1/liveflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2024-05-08 13:30:04.000000 liveflask-1.0.9rc1/liveflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:30:04.000000 liveflask-1.0.9rc1/liveflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-08 13:30:04.000000 liveflask-1.0.9rc1/liveflask.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 13:30:04.000000 liveflask-1.0.9rc1/liveflask.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 13:30:04.876981 liveflask-1.0.9rc1/setup.cfg
--rw-rw-rw-   0        0        0     1225 2024-05-08 13:29:56.000000 liveflask-1.0.9rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.196335 liveflask-1.0.9rc2/
+-rw-rw-rw-   0        0        0     1294 2024-05-08 15:09:19.195335 liveflask-1.0.9rc2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.137650 liveflask-1.0.9rc2/liveflask/
+-rw-rw-rw-   0        0        0     6326 2024-05-08 13:26:44.000000 liveflask-1.0.9rc2/liveflask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.147657 liveflask-1.0.9rc2/liveflask/attributes/
+-rw-rw-rw-   0        0        0     2023 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.148656 liveflask-1.0.9rc2/liveflask/attributes/__pycache__/
+-rw-rw-rw-   0        0        0     3654 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.150655 liveflask-1.0.9rc2/liveflask/static/
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.165687 liveflask-1.0.9rc2/liveflask/static/liveflask/
+-rw-rw-rw-   0        0        0     1924 2024-05-08 15:04:13.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/action.js
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/constants.js
+-rw-rw-rw-   0        0        0      245 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/events.js
+-rw-rw-rw-   0        0        0     1328 2024-05-08 13:29:26.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/init.js
+-rw-rw-rw-   0        0        0      894 2024-05-08 13:26:44.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/liveflask.js
+-rw-rw-rw-   0        0        0     2191 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/model.js
+-rw-rw-rw-   0        0        0     1660 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/polling.js
+-rw-rw-rw-   0        0        0     9170 2024-05-08 13:26:44.000000 liveflask-1.0.9rc2/liveflask/static/liveflask/utils.js
+-rw-rw-rw-   0        0        0    73154 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/static/lodash.min.js
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.168985 liveflask-1.0.9rc2/liveflask/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/templates/liveflask-head.html
+-rw-rw-rw-   0        0        0      348 2024-05-08 13:26:44.000000 liveflask-1.0.9rc2/liveflask/templates/liveflask-scripts.html
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.179297 liveflask-1.0.9rc2/liveflask/traits/
+-rw-rw-rw-   0        0        0      205 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/Bootable.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.193334 liveflask-1.0.9rc2/liveflask/traits/__pycache__/
+-rw-rw-rw-   0        0        0      871 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
+-rw-rw-rw-   0        0        0      202 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3296 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4276 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_props.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2839 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4780 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2042 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/has_actions.py
+-rw-rw-rw-   0        0        0     2488 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/has_props.py
+-rw-rw-rw-   0        0        0     2486 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/has_renders.py
+-rw-rw-rw-   0        0        0     4106 2024-05-01 20:13:57.000000 liveflask-1.0.9rc2/liveflask/traits/has_snapshots.py
+-rw-rw-rw-   0        0        0     2032 2024-05-01 19:41:30.000000 liveflask-1.0.9rc2/liveflask/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:19.145656 liveflask-1.0.9rc2/liveflask.egg-info/
+-rw-rw-rw-   0        0        0     1294 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1239 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 15:09:19.000000 liveflask-1.0.9rc2/liveflask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:09:19.196335 liveflask-1.0.9rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2024-05-08 15:09:16.000000 liveflask-1.0.9rc2/setup.py
```

### Comparing `liveflask-1.0.9rc1/PKG-INFO` & `liveflask-1.0.9rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.9rc1
+Version: 1.0.9rc2
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.9rc1/liveflask/__init__.py` & `liveflask-1.0.9rc2/liveflask/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/attributes/__init__.py` & `liveflask-1.0.9rc2/liveflask/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/attributes/__pycache__/__init__.cpython-311.pyc` & `liveflask-1.0.9rc2/liveflask/attributes/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/static/liveflask/action.js` & `liveflask-1.0.9rc2/liveflask/static/liveflask/action.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -31,18 +31,30 @@
                 try {
                     args = replace_undefined(property).match(/\(([^)]+)\)/)[1];
                     // Love this one console.log(args)
                 } catch (e) {
                     args = "__NOVAL__"
                 }
 
-                send_request(el, {
-                    'method': method,
-                    "args": args
-                }, i)
+                if (i.hasAttribute('data-action-confirm')) {
+                    if (confirm(i.getAttribute("data-action-confirm"))) {
+                        send_request(el, {
+                            'method': method,
+                            "args": args
+                        }, i)
+                    } else {
+                        return false
+                    }
+                } else {
+                    send_request(el, {
+                        'method': method,
+                        "args": args
+                    }, i)
+                }
+
             })
             i.__data_action_click_registered = true
         }
     })
 
 
 }
```

### Comparing `liveflask-1.0.9rc1/liveflask/static/liveflask/init.js` & `liveflask-1.0.9rc2/liveflask/static/liveflask/init.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/static/liveflask/liveflask.js` & `liveflask-1.0.9rc2/liveflask/static/liveflask/liveflask.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/static/liveflask/model.js` & `liveflask-1.0.9rc2/liveflask/static/liveflask/model.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/static/liveflask/polling.js` & `liveflask-1.0.9rc2/liveflask/static/liveflask/polling.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/static/liveflask/utils.js` & `liveflask-1.0.9rc2/liveflask/static/liveflask/utils.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/static/lodash.min.js` & `liveflask-1.0.9rc2/liveflask/static/lodash.min.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/traits/__pycache__/Bootable.cpython-311.pyc` & `liveflask-1.0.9rc2/liveflask/traits/__pycache__/Bootable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/traits/__pycache__/has_actions.cpython-311.pyc` & `liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_actions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/traits/__pycache__/has_props.cpython-311.pyc` & `liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_props.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/traits/__pycache__/has_renders.cpython-311.pyc` & `liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_renders.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc` & `liveflask-1.0.9rc2/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/traits/has_actions.py` & `liveflask-1.0.9rc2/liveflask/traits/has_actions.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/traits/has_props.py` & `liveflask-1.0.9rc2/liveflask/traits/has_props.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/traits/has_renders.py` & `liveflask-1.0.9rc2/liveflask/traits/has_renders.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/traits/has_snapshots.py` & `liveflask-1.0.9rc2/liveflask/traits/has_snapshots.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask/utils.py` & `liveflask-1.0.9rc2/liveflask/utils.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/liveflask.egg-info/PKG-INFO` & `liveflask-1.0.9rc2/liveflask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.9rc1
+Version: 1.0.9rc2
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.9rc1/liveflask.egg-info/SOURCES.txt` & `liveflask-1.0.9rc2/liveflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.9rc1/setup.py` & `liveflask-1.0.9rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="liveflask",
-    version="1.0.9rc1",
+    version="1.0.9rc2",
     author="Jarriq Rolle",
     author_email="jrolle@baysidetechgroup.com",
     description="Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/liveflask",
     packages=['liveflask'],
```


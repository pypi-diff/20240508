# Comparing `tmp/toga_web-0.4.3.tar.gz` & `tmp/toga_web-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toga_web-0.4.3.tar", last modified: Mon May  6 06:43:36 2024, max compression
+gzip compressed data, was "toga_web-0.4.4.tar", last modified: Wed May  8 00:58:55 2024, max compression
```

## Comparing `toga_web-0.4.3.tar` & `toga_web-0.4.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.014005 toga_web-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 06:43:01.000000 toga_web-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 06:43:01.000000 toga_web-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-06 06:43:36.010005 toga_web-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-06 06:43:01.000000 toga_web-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-06 06:43:01.000000 toga_web-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:43:36.014005 toga_web-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.006005 toga_web-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.006005 toga_web-0.4.3/src/toga_web/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/libs.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.010005 toga_web-0.4.3/src/toga_web/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/resources/toga.png
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/screens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.010005 toga_web-0.4.3/src/toga_web/static/
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/static/toga.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.010005 toga_web-0.4.3/src/toga_web/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/activityindicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/box.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/divider.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/passwordinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/widgets/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-06 06:43:01.000000 toga_web-0.4.3/src/toga_web/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:43:36.010005 toga_web-0.4.3/src/toga_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-06 06:43:36.000000 toga_web-0.4.3/src/toga_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 06:43:35.000000 toga_web-0.4.3/src/toga_web.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.436195 toga_web-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:58:26.000000 toga_web-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 00:58:26.000000 toga_web-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-08 00:58:55.432196 toga_web-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-08 00:58:26.000000 toga_web-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-08 00:58:26.000000 toga_web-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:58:55.436195 toga_web-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.428196 toga_web-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.428196 toga_web-0.4.4/src/toga_web/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/libs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.432196 toga_web-0.4.4/src/toga_web/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/resources/toga.png
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/screens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.432196 toga_web-0.4.4/src/toga_web/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/static/toga.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.432196 toga_web-0.4.4/src/toga_web/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/activityindicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/passwordinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/widgets/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-08 00:58:26.000000 toga_web-0.4.4/src/toga_web/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:58:55.432196 toga_web-0.4.4/src/toga_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-08 00:58:55.000000 toga_web-0.4.4/src/toga_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-08 00:58:55.000000 toga_web-0.4.4/src/toga_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:58:55.000000 toga_web-0.4.4/src/toga_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 00:58:55.000000 toga_web-0.4.4/src/toga_web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 00:58:55.000000 toga_web-0.4.4/src/toga_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 00:58:55.000000 toga_web-0.4.4/src/toga_web.egg-info/top_level.txt
```

### Comparing `toga_web-0.4.3/LICENSE` & `toga_web-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/PKG-INFO` & `toga_web-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-web
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Web backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-web
 ========
 
 A backend for the `Toga widget toolkit`_ on web platforms.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_web-0.4.3/README.rst` & `toga_web-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/pyproject.toml` & `toga_web-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/app.py` & `toga_web-0.4.4/src/toga_web/app.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/command.py` & `toga_web-0.4.4/src/toga_web/command.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/dialogs.py` & `toga_web-0.4.4/src/toga_web/dialogs.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/factory.py` & `toga_web-0.4.4/src/toga_web/factory.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/libs.py` & `toga_web-0.4.4/src/toga_web/libs.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/resources/toga.png` & `toga_web-0.4.4/src/toga_web/resources/toga.png`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/screens.py` & `toga_web-0.4.4/src/toga_web/screens.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/static/toga.css` & `toga_web-0.4.4/src/toga_web/static/toga.css`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/widgets/base.py` & `toga_web-0.4.4/src/toga_web/widgets/base.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/widgets/button.py` & `toga_web-0.4.4/src/toga_web/widgets/button.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/widgets/progressbar.py` & `toga_web-0.4.4/src/toga_web/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/widgets/switch.py` & `toga_web-0.4.4/src/toga_web/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/widgets/textinput.py` & `toga_web-0.4.4/src/toga_web/widgets/textinput.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web/window.py` & `toga_web-0.4.4/src/toga_web/window.py`

 * *Files identical despite different names*

### Comparing `toga_web-0.4.3/src/toga_web.egg-info/PKG-INFO` & `toga_web-0.4.4/src/toga_web.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toga-web
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Web backend for the Toga widget toolkit.
 Author-email: Russell Keith-Magee <russell@keith-magee.com>
 Maintainer-email: BeeWare Team <team@beeware.org>
 License: New BSD
 Project-URL: Homepage, https://beeware.org/project/projects/libraries/toga/
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://toga.readthedocs.io/
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: toga-core==0.4.3
+Requires-Dist: toga-core==0.4.4
 
 toga-web
 ========
 
 A backend for the `Toga widget toolkit`_ on web platforms.
 
 This package isn't much use by itself; it needs to be combined with `the core Toga library`_.
```

### Comparing `toga_web-0.4.3/src/toga_web.egg-info/SOURCES.txt` & `toga_web-0.4.4/src/toga_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/oetils-0.2.6.tar.gz` & `tmp/oetils-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oetils-0.2.6.tar", max compression
+gzip compressed data, was "oetils-0.2.7.tar", max compression
```

## Comparing `oetils-0.2.6.tar` & `oetils-0.2.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-03-17 09:22:30.972390 oetils-0.2.6/LICENSE
--rw-r--r--   0        0        0       70 2023-03-17 08:52:59.977552 oetils-0.2.6/README.md
--rw-r--r--   0        0        0       44 2024-02-11 12:55:41.228167 oetils-0.2.6/oetils/__init__.py
--rw-r--r--   0        0        0     8666 2024-03-22 09:59:09.983699 oetils-0.2.6/oetils/plotting.py
--rw-r--r--   0        0        0     1580 2024-02-12 21:01:06.631193 oetils-0.2.6/oetils/util.py
--rw-r--r--   0        0        0      718 2024-03-22 09:59:38.909232 oetils-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 oetils-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-17 09:22:30.972390 oetils-0.2.7/LICENSE
+-rw-r--r--   0        0        0       70 2023-03-17 08:52:59.977552 oetils-0.2.7/README.md
+-rw-r--r--   0        0        0       44 2024-02-11 12:55:41.228167 oetils-0.2.7/oetils/__init__.py
+-rw-r--r--   0        0        0     8625 2024-05-08 12:55:22.441881 oetils-0.2.7/oetils/plotting.py
+-rw-r--r--   0        0        0     1580 2024-02-12 21:01:06.631193 oetils-0.2.7/oetils/util.py
+-rw-r--r--   0        0        0      718 2024-05-08 12:56:24.264442 oetils-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 oetils-0.2.7/PKG-INFO
```

### Comparing `oetils-0.2.6/LICENSE` & `oetils-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oetils-0.2.6/oetils/plotting.py` & `oetils-0.2.7/oetils/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,14 @@
         })
     elif venue == 'poster':
         rc.update({
             'font.size': 14,
             'axes.labelsize': 14,
             'legend.fontsize': 14,
         })
-    if bundle:
-        rc.update(bundle)
     plt.rcParams.update(rc | rcparams)
     return W
 
 
 def savefig(fig, path, tries=20, width=None, height=None, pad=None, v=True):
     """Save figure with true size."""
     fig_ = deepcopy(fig)
```

### Comparing `oetils-0.2.6/oetils/util.py` & `oetils-0.2.7/oetils/util.py`

 * *Files identical despite different names*

### Comparing `oetils-0.2.6/pyproject.toml` & `oetils-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oetils"
-version = "0.2.6"
+version = "0.2.7"
 description = "A collection of useful functions and classes"
 authors = ["Onno Eberhard <onnoeberhard@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onnoeberhard/oetils"
 packages = [
     { include = "oetils" }
```

### Comparing `oetils-0.2.6/PKG-INFO` & `oetils-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oetils
-Version: 0.2.6
+Version: 0.2.7
 Summary: A collection of useful functions and classes
 Home-page: https://github.com/onnoeberhard/oetils
 License: MIT
 Author: Onno Eberhard
 Author-email: onnoeberhard@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


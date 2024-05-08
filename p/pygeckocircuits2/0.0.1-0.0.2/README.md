# Comparing `tmp/pygeckocircuits2-0.0.1.tar.gz` & `tmp/pygeckocircuits2-0.0.2.tar.gz`

## Comparing `pygeckocircuits2-0.0.1.tar` & `pygeckocircuits2-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.1/requirements.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.1/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.1/README.rst
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.2/pygeckocircuits2/__init__.py
+-rw-r--r--   0        0        0    28714 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.2/pygeckocircuits2/geckoCircuitsRemote.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.2/README.rst
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pygeckocircuits2-0.0.2/PKG-INFO
```

### Comparing `pygeckocircuits2-0.0.1/README.rst` & `pygeckocircuits2-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pygeckocircuits2-0.0.1/pyproject.toml` & `pygeckocircuits2-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pygeckocircuits2"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "UPB-LEA" },
 ]
 description = "Control GeckoCircuits by using python."
 readme = "README.rst"
 requires-python = "~=3.8"
 classifiers = [
@@ -26,19 +26,19 @@
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/"]
+packages = ["pygeckocircuits2/"]
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "src/*.py",
+    "pygeckocircuits2/*.py",
     "tests",
     "requirements.txt"
 ]
 
 
 
 [tool.ruff]
```

### Comparing `pygeckocircuits2-0.0.1/PKG-INFO` & `pygeckocircuits2-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pygeckocircuits2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Control GeckoCircuits by using python.
 Project-URL: Homepage, https://github.com/upb-lea/pygeckocircuits2
 Project-URL: Issues, https://github.com/upb-lea/pygeckocircuits2/issues
 Author: UPB-LEA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


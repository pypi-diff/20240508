# Comparing `tmp/unit_simple-1.0.22.tar.gz` & `tmp/unit_simple-1.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_simple-1.0.22.tar", last modified: Sun May  5 22:25:21 2024, max compression
+gzip compressed data, was "unit_simple-1.0.23.tar", last modified: Wed May  8 13:46:19 2024, max compression
```

## Comparing `unit_simple-1.0.22.tar` & `unit_simple-1.0.23.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-05 22:25:21.951172 unit_simple-1.0.22/
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     1211 2024-05-05 22:25:09.000000 unit_simple-1.0.22/LICENSE.md
--rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)     7686 2024-05-05 22:25:21.951172 unit_simple-1.0.22/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     5297 2024-05-05 21:56:47.000000 unit_simple-1.0.22/README.md
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     1129 2024-05-05 22:25:09.000000 unit_simple-1.0.22/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2024-05-05 22:25:21.951172 unit_simple-1.0.22/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-05 22:25:21.947172 unit_simple-1.0.22/src/
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-05 22:25:21.947172 unit_simple-1.0.22/src/unit_simple/
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      512 2024-05-05 20:53:32.000000 unit_simple-1.0.22/src/unit_simple/__init__.py
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)    12931 2024-05-05 20:53:32.000000 unit_simple-1.0.22/src/unit_simple/unit_simple.py
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-05 22:25:21.951172 unit_simple-1.0.22/src/unit_simple.egg-info/
--rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)     7686 2024-05-05 22:25:21.000000 unit_simple-1.0.22/src/unit_simple.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      263 2024-05-05 22:25:21.000000 unit_simple-1.0.22/src/unit_simple.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2024-05-05 22:25:21.000000 unit_simple-1.0.22/src/unit_simple.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       12 2024-05-05 22:25:21.000000 unit_simple-1.0.22/src/unit_simple.egg-info/top_level.txt
-drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-05 22:25:21.951172 unit_simple-1.0.22/test/
--rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     4401 2024-05-05 20:26:00.000000 unit_simple-1.0.22/test/test.py
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-08 13:46:19.806569 unit_simple-1.0.23/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     1211 2024-05-08 13:46:07.000000 unit_simple-1.0.23/LICENSE.md
+-rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)     7685 2024-05-08 13:46:19.806569 unit_simple-1.0.23/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     5297 2024-05-05 21:56:47.000000 unit_simple-1.0.23/README.md
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     1128 2024-05-08 13:46:07.000000 unit_simple-1.0.23/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       38 2024-05-08 13:46:19.806569 unit_simple-1.0.23/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-08 13:46:19.790568 unit_simple-1.0.23/src/
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-08 13:46:19.790568 unit_simple-1.0.23/src/unit_simple/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      512 2024-05-05 20:53:32.000000 unit_simple-1.0.23/src/unit_simple/__init__.py
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)    12931 2024-05-05 20:53:32.000000 unit_simple-1.0.23/src/unit_simple/unit_simple.py
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-08 13:46:19.806569 unit_simple-1.0.23/src/unit_simple.egg-info/
+-rw-r--r--   0 gitlab-runner   (993) gitlab-runner   (993)     7685 2024-05-08 13:46:19.000000 unit_simple-1.0.23/src/unit_simple.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)      263 2024-05-08 13:46:19.000000 unit_simple-1.0.23/src/unit_simple.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)        1 2024-05-08 13:46:19.000000 unit_simple-1.0.23/src/unit_simple.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)       12 2024-05-08 13:46:19.000000 unit_simple-1.0.23/src/unit_simple.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (993) gitlab-runner   (993)        0 2024-05-08 13:46:19.790568 unit_simple-1.0.23/test/
+-rw-rw-r--   0 gitlab-runner   (993) gitlab-runner   (993)     4401 2024-05-05 20:26:00.000000 unit_simple-1.0.23/test/test.py
```

### Comparing `unit_simple-1.0.22/LICENSE.md` & `unit_simple-1.0.23/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unit_simple-1.0.22/PKG-INFO` & `unit_simple-1.0.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unit_simple
-Version: 1.0.22
+Version: 1.0.23
 Summary: A simple measurement unit API to handle basic unit conversions.
 Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -24,28 +24,28 @@
         IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
         OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
         ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
         OTHER DEALINGS IN THE SOFTWARE.
         
         For more information, please refer to <https://unlicense.org>
         
-Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py/tree/unit_simple-1.0.22/unit_simple
-Project-URL: Documentation, http://cosmoloj.com/mkdocs/unit_simple/1.0.22
+Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py/tree/unit_simple-1.0.23/unit_simple
+Project-URL: Documentation, http://cosmoloj.com/mkdocs/unit_simple/1.0.23
 Project-URL: Specification, http://cosmoloj.com/su
 Keywords: units,converter,unit converter,measure,units of measurement
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Public Domain
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Simple Unit (Python implementation)
 
 [![Anaconda-Server Badge](https://anaconda.org/cosmoloj/unit_simple/badges/version.svg)](https://anaconda.org/cosmoloj/unit_simple)
 [![Anaconda-Server Badge](https://anaconda.org/cosmoloj/unit_simple/badges/latest_release_date.svg)](https://anaconda.org/cosmoloj/unit_simple)
```

### Comparing `unit_simple-1.0.22/README.md` & `unit_simple-1.0.23/README.md`

 * *Files identical despite different names*

### Comparing `unit_simple-1.0.22/pyproject.toml` & `unit_simple-1.0.23/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unit_simple"
-version = "1.0.22"
+version = "1.0.23"
 authors = [
   { name="Samuel Andrés", email="samuel.andres@yahoo.fr" },
 ]
 description = "A simple measurement unit API to handle basic unit conversions."
 readme = "README.md"
 license = {file = "LICENSE.md"}
-requires-python = ">=3.11"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: Public Domain",
@@ -27,10 +27,10 @@
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/SamuelAndresPascal/cosmoloj-py/tree/unit_simple-1.0.22/unit_simple"
-"Documentation" = "http://cosmoloj.com/mkdocs/unit_simple/1.0.22"
+"Homepage" = "https://github.com/SamuelAndresPascal/cosmoloj-py/tree/unit_simple-1.0.23/unit_simple"
+"Documentation" = "http://cosmoloj.com/mkdocs/unit_simple/1.0.23"
 "Specification" = "http://cosmoloj.com/su"
```

### Comparing `unit_simple-1.0.22/src/unit_simple/__init__.py` & `unit_simple-1.0.23/src/unit_simple/__init__.py`

 * *Files identical despite different names*

### Comparing `unit_simple-1.0.22/src/unit_simple/unit_simple.py` & `unit_simple-1.0.23/src/unit_simple/unit_simple.py`

 * *Files identical despite different names*

### Comparing `unit_simple-1.0.22/src/unit_simple.egg-info/PKG-INFO` & `unit_simple-1.0.23/src/unit_simple.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unit_simple
-Version: 1.0.22
+Version: 1.0.23
 Summary: A simple measurement unit API to handle basic unit conversions.
 Author-email: Samuel Andrés <samuel.andres@yahoo.fr>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -24,28 +24,28 @@
         IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
         OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
         ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
         OTHER DEALINGS IN THE SOFTWARE.
         
         For more information, please refer to <https://unlicense.org>
         
-Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py/tree/unit_simple-1.0.22/unit_simple
-Project-URL: Documentation, http://cosmoloj.com/mkdocs/unit_simple/1.0.22
+Project-URL: Homepage, https://github.com/SamuelAndresPascal/cosmoloj-py/tree/unit_simple-1.0.23/unit_simple
+Project-URL: Documentation, http://cosmoloj.com/mkdocs/unit_simple/1.0.23
 Project-URL: Specification, http://cosmoloj.com/su
 Keywords: units,converter,unit converter,measure,units of measurement
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Public Domain
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Simple Unit (Python implementation)
 
 [![Anaconda-Server Badge](https://anaconda.org/cosmoloj/unit_simple/badges/version.svg)](https://anaconda.org/cosmoloj/unit_simple)
 [![Anaconda-Server Badge](https://anaconda.org/cosmoloj/unit_simple/badges/latest_release_date.svg)](https://anaconda.org/cosmoloj/unit_simple)
```

### Comparing `unit_simple-1.0.22/test/test.py` & `unit_simple-1.0.23/test/test.py`

 * *Files identical despite different names*


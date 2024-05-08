# Comparing `tmp/ou_tm351_jl_extensions-0.2.3.tar.gz` & `tmp/ou_tm351_jl_extensions-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_tm351_jl_extensions-0.2.3.tar", max compression
+gzip compressed data, was "ou_tm351_jl_extensions-0.2.4.tar", max compression
```

## Comparing `ou_tm351_jl_extensions-0.2.3.tar` & `ou_tm351_jl_extensions-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-05-04 10:46:43.497008 ou_tm351_jl_extensions-0.2.3/LICENSE
--rw-r--r--   0        0        0     1226 2023-07-21 20:49:34.016848 ou_tm351_jl_extensions-0.2.3/README.md
--rw-r--r--   0        0        0     2388 2023-05-04 15:50:37.140962 ou_tm351_jl_extensions-0.2.3/ou_tm351_jl_extensions/__init__.py
--rw-r--r--   0        0        0      937 2024-05-07 17:05:56.103793 ou_tm351_jl_extensions-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2583 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-04 10:46:43.497008 ou_tm351_jl_extensions-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1226 2023-07-21 20:49:34.016848 ou_tm351_jl_extensions-0.2.4/README.md
+-rw-r--r--   0        0        0     2388 2023-05-04 15:50:37.140962 ou_tm351_jl_extensions-0.2.4/ou_tm351_jl_extensions/__init__.py
+-rw-r--r--   0        0        0      936 2024-05-07 19:58:55.549687 ou_tm351_jl_extensions-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.4/PKG-INFO
```

### Comparing `ou_tm351_jl_extensions-0.2.3/LICENSE` & `ou_tm351_jl_extensions-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.3/README.md` & `ou_tm351_jl_extensions-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.3/ou_tm351_jl_extensions/__init__.py` & `ou_tm351_jl_extensions-0.2.4/ou_tm351_jl_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.3/pyproject.toml` & `ou_tm351_jl_extensions-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "ou-tm351-jl-extensions"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Tony Hirst <tony.hirst@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ou_tm351_jl_extensions"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 jupyterlab = ">=4.1"
-#jupyterlab-ou-brand-extension = "^0.2.0"
+jupyterlab-ou-brand-extension = "^0.2.0"
 jupyterlab-cell-status-extension = "^0.1.3"
 jupyterlab-myst = "^2.4.0"
 jupyterlab-empinken-extension = "^0.5.0"
 jupyterlab-geojson = "^3.3.1"
 jupyterlab-skip-traceback = "^5.1.0"
 jupyterlab-git = "^0.50.0"
 jupytext = "^1.16.0"
```

### Comparing `ou_tm351_jl_extensions-0.2.3/PKG-INFO` & `ou_tm351_jl_extensions-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ou-tm351-jl-extensions
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: Tony Hirst
 Author-email: tony.hirst@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,14 +19,15 @@
 Requires-Dist: jupyterlab-empinken-extension (>=0.5.0,<0.6.0)
 Requires-Dist: jupyterlab-filesystem-access (>=0.6.0,<0.7.0)
 Requires-Dist: jupyterlab-geojson (>=3.3.1,<4.0.0)
 Requires-Dist: jupyterlab-git (>=0.50.0,<0.51.0)
 Requires-Dist: jupyterlab-language-pack-fr-fr (>=4.1.post2,<5.0)
 Requires-Dist: jupyterlab-language-pack-zh-cn (>=4.1.post2,<5.0)
 Requires-Dist: jupyterlab-myst (>=2.4.0,<3.0.0)
+Requires-Dist: jupyterlab-ou-brand-extension (>=0.2.0,<0.3.0)
 Requires-Dist: jupyterlab-skip-traceback (>=5.1.0,<6.0.0)
 Requires-Dist: jupyterlab-spellchecker (>=0.8.4,<0.9.0)
 Requires-Dist: jupytext (>=1.16.0,<2.0.0)
 Requires-Dist: stickyland (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # ou-tm351-jl-extensions
```


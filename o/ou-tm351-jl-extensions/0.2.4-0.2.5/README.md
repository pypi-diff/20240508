# Comparing `tmp/ou_tm351_jl_extensions-0.2.4.tar.gz` & `tmp/ou_tm351_jl_extensions-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_tm351_jl_extensions-0.2.4.tar", max compression
+gzip compressed data, was "ou_tm351_jl_extensions-0.2.5.tar", max compression
```

## Comparing `ou_tm351_jl_extensions-0.2.4.tar` & `ou_tm351_jl_extensions-0.2.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-05-04 10:46:43.497008 ou_tm351_jl_extensions-0.2.4/LICENSE
--rw-r--r--   0        0        0     1226 2023-07-21 20:49:34.016848 ou_tm351_jl_extensions-0.2.4/README.md
--rw-r--r--   0        0        0     2388 2023-05-04 15:50:37.140962 ou_tm351_jl_extensions-0.2.4/ou_tm351_jl_extensions/__init__.py
--rw-r--r--   0        0        0      936 2024-05-07 19:58:55.549687 ou_tm351_jl_extensions-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-04 10:46:43.497008 ou_tm351_jl_extensions-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1226 2023-07-21 20:49:34.016848 ou_tm351_jl_extensions-0.2.5/README.md
+-rw-r--r--   0        0        0     2388 2023-05-04 15:50:37.140962 ou_tm351_jl_extensions-0.2.5/ou_tm351_jl_extensions/__init__.py
+-rw-r--r--   0        0        0     1776 2024-05-08 15:07:06.765455 ou_tm351_jl_extensions-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.5/PKG-INFO
```

### Comparing `ou_tm351_jl_extensions-0.2.4/LICENSE` & `ou_tm351_jl_extensions-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.4/README.md` & `ou_tm351_jl_extensions-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.4/ou_tm351_jl_extensions/__init__.py` & `ou_tm351_jl_extensions-0.2.5/ou_tm351_jl_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.4/pyproject.toml` & `ou_tm351_jl_extensions-0.2.5/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 [tool.poetry]
 name = "ou-tm351-jl-extensions"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["Tony Hirst <tony.hirst@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ou_tm351_jl_extensions"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 jupyterlab = ">=4.1"
-jupyterlab-ou-brand-extension = "^0.2.0"
-jupyterlab-cell-status-extension = "^0.1.3"
-jupyterlab-myst = "^2.4.0"
-jupyterlab-empinken-extension = "^0.5.0"
-jupyterlab-geojson = "^3.3.1"
-jupyterlab-skip-traceback = "^5.1.0"
-jupyterlab-git = "^0.50.0"
-jupytext = "^1.16.0"
-jupyter-archive = "^3.4.0"
-jupyterlab-spellchecker = "^0.8.4"
-jupyterlab-language-pack-fr-fr = "^4.1.post2"
-jupyterlab-language-pack-zh-cn = "^4.1.post2"
-jupyter-resource-usage = "^1.0.2"
-stickyland = "^0.2.1"
-#jupyterlab-tour = "^3.1.4"
-jupyter-compare-view = "^0.2.4"
-jupyterlab-filesystem-access = "^0.6.0"
+
+# Branding and OU extensions
+jupyterlab-ou-brand-extension = "^0.2.0" # OU brand extension (faviocon.logo)
+
+# Notebook cell tools
+jupyterlab-cell-status-extension = "^0.1.3" # cell execution status; accessibility tools
+jupyterlab-empinken-extension = "^0.5.0" # cell background styling
+jupyterlab-skip-traceback = "^5.1.0" # skip trackeback / error reporting
+jupyterlab-myst = "^2.4.0" ## MyST parser and styling (markdown cells)
+jupyterlab-spellchecker = "^0.8.4" ## Spellchecker
+
+# Code support
+jupyterlab-lsp = "^5.1.0" # language server protocol
+jupyterlab-code-formatter = "^2.2.1" # Code formatter
+black = "^24.4.2" # code formatting
+isort = "^25.13.2" # code formatting
+
+# Language packs
+jupyterlab-language-pack-fr-fr = "^4.1.post2" # French
+jupyterlab-language-pack-zh-cn = "^4.1.post2" # Chinese
+
+# File browsing and handling
+jupyterlab-unfold = "^0.3.0" # tree view in files sidebar
+jupyter-archive = "^3.4.0" # archive file download
+jupyterlab-filesystem-access = "^0.6.0" # local filesystem access
+jupyterlab-git = "^0.50.0" # Git/Github tools
+jupytext = "^1.16.0" # text notebook formats
+
+# Renderers
+jupyterlab-geojson = "^3.3.1" # geojson renderer
+jupyter-compare-view = "^0.2.4" # compare images
+
+# Resource monitoring
+jupyter-resource-usage = "^1.0.2" # memorry/CPU
+
+# Misc, evaluation, etc
+#stickyland = "^0.2.1" # sticky notes - BROKEN?
+#jupyterlab-tour = "^3.1.4" # Jupyterlab tour (irritating!)
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ou_tm351_jl_extensions-0.2.4/PKG-INFO` & `ou_tm351_jl_extensions-0.2.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: ou-tm351-jl-extensions
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: Tony Hirst
 Author-email: tony.hirst@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: black (>=24.4.2,<25.0.0)
+Requires-Dist: isort (>=25.13.2,<26.0.0)
 Requires-Dist: jupyter-archive (>=3.4.0,<4.0.0)
 Requires-Dist: jupyter-compare-view (>=0.2.4,<0.3.0)
 Requires-Dist: jupyter-resource-usage (>=1.0.2,<2.0.0)
 Requires-Dist: jupyterlab (>=4.1)
 Requires-Dist: jupyterlab-cell-status-extension (>=0.1.3,<0.2.0)
+Requires-Dist: jupyterlab-code-formatter (>=2.2.1,<3.0.0)
 Requires-Dist: jupyterlab-empinken-extension (>=0.5.0,<0.6.0)
 Requires-Dist: jupyterlab-filesystem-access (>=0.6.0,<0.7.0)
 Requires-Dist: jupyterlab-geojson (>=3.3.1,<4.0.0)
 Requires-Dist: jupyterlab-git (>=0.50.0,<0.51.0)
 Requires-Dist: jupyterlab-language-pack-fr-fr (>=4.1.post2,<5.0)
 Requires-Dist: jupyterlab-language-pack-zh-cn (>=4.1.post2,<5.0)
+Requires-Dist: jupyterlab-lsp (>=5.1.0,<6.0.0)
 Requires-Dist: jupyterlab-myst (>=2.4.0,<3.0.0)
 Requires-Dist: jupyterlab-ou-brand-extension (>=0.2.0,<0.3.0)
 Requires-Dist: jupyterlab-skip-traceback (>=5.1.0,<6.0.0)
 Requires-Dist: jupyterlab-spellchecker (>=0.8.4,<0.9.0)
+Requires-Dist: jupyterlab-unfold (>=0.3.0,<0.4.0)
 Requires-Dist: jupytext (>=1.16.0,<2.0.0)
-Requires-Dist: stickyland (>=0.2.1,<0.3.0)
 Description-Content-Type: text/markdown
 
 # ou-tm351-jl-extensions
 
 Install from pypi as `ou-tm351-jl-extensions`
 
 - JupyterLab 3: v0.1.2
```


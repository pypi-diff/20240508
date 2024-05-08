# Comparing `tmp/mkdocs-print-site-plugin-2.3.6.tar.gz` & `tmp/mkdocs-print-site-plugin-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-print-site-plugin-2.3.6.tar", last modified: Mon Aug 28 07:29:52 2023, max compression
+gzip compressed data, was "mkdocs-print-site-plugin-2.4.0.tar", last modified: Wed Apr 10 11:23:59 2024, max compression
```

## Comparing `mkdocs-print-site-plugin-2.3.6.tar` & `mkdocs-print-site-plugin-2.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (999)     1064 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      132 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     3458 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2529 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/
--rw-r--r--   0 runner    (1001) docker     (999)     3477 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings1.css
--rw-r--r--   0 runner    (1001) docker     (999)     1286 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings2.css
--rw-r--r--   0 runner    (1001) docker     (999)     1444 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings3.css
--rw-r--r--   0 runner    (1001) docker     (999)     1568 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings4.css
--rw-r--r--   0 runner    (1001) docker     (999)     1675 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings5.css
--rw-r--r--   0 runner    (1001) docker     (999)     1789 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings6.css
--rw-r--r--   0 runner    (1001) docker     (999)      738 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-material.css
--rw-r--r--   0 runner    (1001) docker     (999)      949 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-mkdocs.css
--rw-r--r--   0 runner    (1001) docker     (999)     5463 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site.css
--rw-r--r--   0 runner    (1001) docker     (999)     1570 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/exclude.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (999)     4515 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/js/print-site.js
--rw-r--r--   0 runner    (1001) docker     (999)    17119 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (999)     9147 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/
--rw-r--r--   0 runner    (1001) docker     (999)      714 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/cover_page.tpl
--rw-r--r--   0 runner    (1001) docker     (999)      557 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/print_site_banner.tpl
--rw-r--r--   0 runner    (1001) docker     (999)     8832 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (999)      863 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3458 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1273 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       78 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       23 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       31 2023-08-28 07:29:52.000000 mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1458 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:52.863981 mkdocs-print-site-plugin-2.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     9196 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/tests/test_building.py
--rw-r--r--   0 runner    (1001) docker     (999)      507 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/tests/test_exclude.py
--rw-r--r--   0 runner    (1001) docker     (999)     7564 2023-08-28 07:29:14.000000 mkdocs-print-site-plugin-2.3.6/tests/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:23:59.937239 mkdocs-print-site-plugin-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-10 11:23:59.937239 mkdocs-print-site-plugin-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:23:59.933239 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:23:59.933239 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings1.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings2.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings3.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings4.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings5.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings6.css
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-material.css
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-mkdocs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:23:59.933239 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/js/print-site.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:23:59.933239 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/templates/cover_page.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/templates/print_site_banner.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:23:59.937239 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-10 11:23:59.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-10 11:23:59.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:23:59.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 11:23:59.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 11:23:59.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 11:23:59.000000 mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:23:59.937239 mkdocs-print-site-plugin-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:23:59.933239 mkdocs-print-site-plugin-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/tests/test_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/tests/test_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-10 11:23:31.000000 mkdocs-print-site-plugin-2.4.0/tests/test_urls.py
```

### Comparing `mkdocs-print-site-plugin-2.3.6/LICENSE` & `mkdocs-print-site-plugin-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/PKG-INFO` & `mkdocs-print-site-plugin-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: mkdocs-print-site-plugin
-Version: 2.3.6
+Version: 2.4.0
 Summary: MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.
 Home-page: https://github.com/timvink/mkdocs-print-site-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin print pdf
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mkdocs-material>=7.3.0
 
 [![Actions Status](https://github.com/timvink/mkdocs-print-site-plugin/workflows/pytest/badge.svg)](https://github.com/timvink/mkdocs-print-site-plugin/actions)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-print-site-plugin)
 ![PyPI](https://img.shields.io/pypi/v/mkdocs-print-site-plugin)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-print-site-plugin)
 [![codecov](https://codecov.io/gh/timvink/mkdocs-print-site-plugin/branch/master/graph/badge.svg)](https://codecov.io/gh/timvink/mkdocs-print-site-plugin)
 ![GitHub contributors](https://img.shields.io/github/contributors/timvink/mkdocs-print-site-plugin)
```

### Comparing `mkdocs-print-site-plugin-2.3.6/README.md` & `mkdocs-print-site-plugin-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings1.css` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings1.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings2.css` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings2.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings3.css` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings3.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings4.css` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings4.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings5.css` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings5.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-enum-headings6.css` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-enum-headings6.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-material.css` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-material.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site-mkdocs.css` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site-mkdocs.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/css/print-site.css` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/css/print-site.css`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/exclude.py` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/js/print-site.js` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/js/print-site.js`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/plugin.py` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 import logging
 import sys
 
 from mkdocs.plugins import BasePlugin
 from mkdocs.config import config_options
 from mkdocs.structure.files import File
 from mkdocs.structure.pages import Page
-from mkdocs.utils import write_file, copy_file, get_relative_url, warning_filter
+from mkdocs.utils import write_file, copy_file, get_relative_url
 from mkdocs.exceptions import PluginError
 
 from mkdocs_print_site_plugin.renderer import Renderer
 from mkdocs_print_site_plugin.utils import flatten_nav, get_theme_name
 from mkdocs_print_site_plugin.urls import is_external
 
 logger = logging.getLogger("mkdocs.plugins")
-logger.addFilter(warning_filter)
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
 class PrintSitePlugin(BasePlugin):
     """
     MkDocs Plugin class for combining all site pages into a single page.
@@ -354,14 +353,26 @@
         if config.get("plugins", {}).get("charts"):
             html = (
                 config.get("plugins", {})
                 .get("charts")
                 .add_javascript_variables(html, self.print_page, config)
             )
 
+        # Compatibility with mkdocs-drawio
+        # As this plugin adds renderer html for every drawio diagram
+        # referenced in your markdown files. This rendering happens
+        # in the on_post_page event, which is skipped by this plugin
+        # therefore we need to manual execute the drawio plugin renderer here. 
+        if config.get("plugins", {}).get("drawio"):
+            html = (
+                config.get("plugins", {})
+                    .get("drawio")
+                    .render_drawio_diagrams(html, self.print_page)
+            )
+
         # Compatibility with https://github.com/g-provost/lightgallery-markdown
         # This plugin insert link hrefs with double dashes, f.e.
         # <link href="//assets/css/somecss.css">
         # Details https://github.com/timvink/mkdocs-print-site-plugin/issues/68
         htmls = html.split("</head>")
         base_url = "../" if config.get("use_directory_urls") else ""
         htmls[0] = htmls[0].replace("href=\"//", f"href=\"{base_url}")
```

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/renderer.py` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/cover_page.tpl` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/templates/cover_page.tpl`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/templates/print_site_banner.tpl` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/templates/print_site_banner.tpl`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/urls.py` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin/utils.py` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/PKG-INFO` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: mkdocs-print-site-plugin
-Version: 2.3.6
+Version: 2.4.0
 Summary: MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.
 Home-page: https://github.com/timvink/mkdocs-print-site-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs plugin print pdf
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mkdocs-material>=7.3.0
 
 [![Actions Status](https://github.com/timvink/mkdocs-print-site-plugin/workflows/pytest/badge.svg)](https://github.com/timvink/mkdocs-print-site-plugin/actions)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-print-site-plugin)
 ![PyPI](https://img.shields.io/pypi/v/mkdocs-print-site-plugin)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-print-site-plugin)
 [![codecov](https://codecov.io/gh/timvink/mkdocs-print-site-plugin/branch/master/graph/badge.svg)](https://codecov.io/gh/timvink/mkdocs-print-site-plugin)
 ![GitHub contributors](https://img.shields.io/github/contributors/timvink/mkdocs-print-site-plugin)
```

### Comparing `mkdocs-print-site-plugin-2.3.6/mkdocs_print_site_plugin.egg-info/SOURCES.txt` & `mkdocs-print-site-plugin-2.4.0/mkdocs_print_site_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/setup.py` & `mkdocs-print-site-plugin-2.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,34 +5,34 @@
     long_description = ""
     for line in f:
         long_description += line
 
 
 setup(
     name="mkdocs-print-site-plugin",
-    version="2.3.6",
+    version="2.4.0",
     description="MkDocs plugin that combines all pages into one, allowing for easy export to PDF and standalone HTML.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs plugin print pdf",
     url="https://github.com/timvink/mkdocs-print-site-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
     include_package_data=True,
     license="MIT",
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     classifiers=[
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Topic :: Documentation",
         "Topic :: Text Processing",
     ],
     install_requires=["mkdocs-material>=7.3.0"],
     packages=find_packages(),
     entry_points={
```

### Comparing `mkdocs-print-site-plugin-2.3.6/tests/test_building.py` & `mkdocs-print-site-plugin-2.4.0/tests/test_building.py`

 * *Files identical despite different names*

### Comparing `mkdocs-print-site-plugin-2.3.6/tests/test_urls.py` & `mkdocs-print-site-plugin-2.4.0/tests/test_urls.py`

 * *Files identical despite different names*


# Comparing `tmp/mpl_sphinx_theme-3.8.0rc2.tar.gz` & `tmp/mpl_sphinx_theme-3.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_sphinx_theme-3.8.0rc2.tar", last modified: Wed Sep 13 22:31:47 2023, max compression
+gzip compressed data, was "mpl_sphinx_theme-3.9.0rc1.tar", last modified: Wed May  8 20:17:22 2024, max compression
```

## Comparing `mpl_sphinx_theme-3.8.0rc2.tar` & `mpl_sphinx_theme-3.9.0rc1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:31:47.743026 mpl_sphinx_theme-3.8.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-09-13 22:31:47.743026 mpl_sphinx_theme-3.8.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:31:47.743026 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:31:47.743026 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/components/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/donate_sidebar.html
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/mpl_icon_links.html
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/mpl_nav_bar.html
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:31:47.743026 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:31:47.743026 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      722 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:31:47.743026 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15406 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   127692 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/logo_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)   127493 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/logo_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 22:31:47.743026 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-09-13 22:31:47.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-09-13 22:31:47.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 22:31:47.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-09-13 22:31:47.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 22:31:47.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-13 22:31:47.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-13 22:31:47.000000 mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2023-09-13 22:31:37.000000 mpl_sphinx_theme-3.8.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-13 22:31:47.743026 mpl_sphinx_theme-3.8.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:22.005741 mpl_sphinx_theme-3.9.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-08 20:17:22.005741 mpl_sphinx_theme-3.9.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:22.001742 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:22.001742 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/components/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/donate_sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/mpl_icon_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/mpl_nav_bar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:22.005741 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:22.005741 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:22.005741 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15406 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   127692 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/logo_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   127493 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/logo_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:17:22.005741 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-08 20:17:21.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-08 20:17:21.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:17:21.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 20:17:21.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:17:21.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 20:17:21.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 20:17:21.000000 mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 20:17:13.000000 mpl_sphinx_theme-3.9.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:17:22.005741 mpl_sphinx_theme-3.9.0rc1/setup.cfg
```

### Comparing `mpl_sphinx_theme-3.8.0rc2/LICENSE.txt` & `mpl_sphinx_theme-3.9.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpl_sphinx_theme-3.8.0rc2/PKG-INFO` & `mpl_sphinx_theme-3.9.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_sphinx_theme
-Version: 3.8.0rc2
+Version: 3.9.0rc1
 Summary: Matplotlib theme for Sphinx
 Author: Matplotlib Developers
 License: BSD 3-Clause License
         
         Copyright (c) 2021-2023, Matplotlib Development Team
         
         Redistribution and use in source and binary forms, with or without
@@ -78,14 +78,28 @@
 
 To change the top navbar, edit ``mpl_sphinx_theme/mpl_nav_bar.html``
 
 To change the social icons, edit ``mpl_sphinx_theme/mpl_icon_links.html``
 
 To change the style, edit ``mpl_sphinx_theme/static/css/style.css``
 
+Overriding hard coded elements
+------------------------------
+This theme is primarily designed to be used with subprojects that are part of the main
+Matplotlib webiste (e.g., [our cheatseets](https://github.com/matplotlib/cheatsheets]
+and [list of third-party packages](https://github.com/matplotlib/mpl-third-party)).
+As such several elements are hard coded. However, the theme may also be used by
+other subprojects that need to change the hard-coded defaults.
+The following sections explain how to reset these back to their defaults by modifying
+``html_theme_options`` in ``conf.py``.
+
+Header section links
+~~~~~~~~~~~~~~~~~~~~
+Use a copy of [the default pydata-sphinx-theme navbar](https://github.com/pydata/pydata-sphinx-theme/blob/main/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/navbar-nav.html) and set the ``'navbar_center'`` key to this HTML file in ``html_theme_options``.
+
 Building
 --------
 To build the theme with a sample page, navigate into the ``doc/`` directory and run
 
 .. code-block::
 
    make html
```

### Comparing `mpl_sphinx_theme-3.8.0rc2/README.rst` & `mpl_sphinx_theme-3.9.0rc1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -32,14 +32,28 @@
 
 To change the top navbar, edit ``mpl_sphinx_theme/mpl_nav_bar.html``
 
 To change the social icons, edit ``mpl_sphinx_theme/mpl_icon_links.html``
 
 To change the style, edit ``mpl_sphinx_theme/static/css/style.css``
 
+Overriding hard coded elements
+------------------------------
+This theme is primarily designed to be used with subprojects that are part of the main
+Matplotlib webiste (e.g., [our cheatseets](https://github.com/matplotlib/cheatsheets]
+and [list of third-party packages](https://github.com/matplotlib/mpl-third-party)).
+As such several elements are hard coded. However, the theme may also be used by
+other subprojects that need to change the hard-coded defaults.
+The following sections explain how to reset these back to their defaults by modifying
+``html_theme_options`` in ``conf.py``.
+
+Header section links
+~~~~~~~~~~~~~~~~~~~~
+Use a copy of [the default pydata-sphinx-theme navbar](https://github.com/pydata/pydata-sphinx-theme/blob/main/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/navbar-nav.html) and set the ``'navbar_center'`` key to this HTML file in ``html_theme_options``.
+
 Building
 --------
 To build the theme with a sample page, navigate into the ``doc/`` directory and run
 
 .. code-block::
 
    make html
```

### Comparing `mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/__init__.py` & `mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/mpl_icon_links.html` & `mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/mpl_icon_links.html`

 * *Files identical despite different names*

### Comparing `mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/mpl_nav_bar.html` & `mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/mpl_nav_bar.html`

 * *Files identical despite different names*

### Comparing `mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/css/style.css` & `mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/images/favicon.ico` & `mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/logo_dark.svg` & `mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/logo_dark.svg`

 * *Files identical despite different names*

### Comparing `mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme/static/logo_light.svg` & `mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme/static/logo_light.svg`

 * *Files identical despite different names*

### Comparing `mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/PKG-INFO` & `mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mpl-sphinx-theme
-Version: 3.8.0rc2
+Name: mpl_sphinx_theme
+Version: 3.9.0rc1
 Summary: Matplotlib theme for Sphinx
 Author: Matplotlib Developers
 License: BSD 3-Clause License
         
         Copyright (c) 2021-2023, Matplotlib Development Team
         
         Redistribution and use in source and binary forms, with or without
@@ -78,14 +78,28 @@
 
 To change the top navbar, edit ``mpl_sphinx_theme/mpl_nav_bar.html``
 
 To change the social icons, edit ``mpl_sphinx_theme/mpl_icon_links.html``
 
 To change the style, edit ``mpl_sphinx_theme/static/css/style.css``
 
+Overriding hard coded elements
+------------------------------
+This theme is primarily designed to be used with subprojects that are part of the main
+Matplotlib webiste (e.g., [our cheatseets](https://github.com/matplotlib/cheatsheets]
+and [list of third-party packages](https://github.com/matplotlib/mpl-third-party)).
+As such several elements are hard coded. However, the theme may also be used by
+other subprojects that need to change the hard-coded defaults.
+The following sections explain how to reset these back to their defaults by modifying
+``html_theme_options`` in ``conf.py``.
+
+Header section links
+~~~~~~~~~~~~~~~~~~~~
+Use a copy of [the default pydata-sphinx-theme navbar](https://github.com/pydata/pydata-sphinx-theme/blob/main/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/components/navbar-nav.html) and set the ``'navbar_center'`` key to this HTML file in ``html_theme_options``.
+
 Building
 --------
 To build the theme with a sample page, navigate into the ``doc/`` directory and run
 
 .. code-block::
 
    make html
```

### Comparing `mpl_sphinx_theme-3.8.0rc2/mpl_sphinx_theme.egg-info/SOURCES.txt` & `mpl_sphinx_theme-3.9.0rc1/mpl_sphinx_theme.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.rst
 pyproject.toml
 mpl_sphinx_theme/__init__.py
 mpl_sphinx_theme/_version.py
 mpl_sphinx_theme/donate_sidebar.html
 mpl_sphinx_theme/mpl_icon_links.html
 mpl_sphinx_theme/mpl_nav_bar.html
-mpl_sphinx_theme/search.html
 mpl_sphinx_theme/theme.conf
 mpl_sphinx_theme.egg-info/PKG-INFO
 mpl_sphinx_theme.egg-info/SOURCES.txt
 mpl_sphinx_theme.egg-info/dependency_links.txt
 mpl_sphinx_theme.egg-info/entry_points.txt
 mpl_sphinx_theme.egg-info/not-zip-safe
 mpl_sphinx_theme.egg-info/requires.txt
```

### Comparing `mpl_sphinx_theme-3.8.0rc2/pyproject.toml` & `mpl_sphinx_theme-3.9.0rc1/pyproject.toml`

 * *Files identical despite different names*


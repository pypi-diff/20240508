# Comparing `tmp/nextstrain_sphinx_theme-2024.1.tar.gz` & `tmp/nextstrain_sphinx_theme-2024.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextstrain_sphinx_theme-2024.1.tar", last modified: Wed May  1 18:24:18 2024, max compression
+gzip compressed data, was "nextstrain_sphinx_theme-2024.2.tar", last modified: Wed May  8 17:54:14 2024, max compression
```

## Comparing `nextstrain_sphinx_theme-2024.1.tar` & `nextstrain_sphinx_theme-2024.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.278881 nextstrain_sphinx_theme-2024.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-01 18:24:18.278881 nextstrain_sphinx_theme-2024.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.270881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.274881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/css/nextstrain.css
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.274881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/js/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.274881 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    39937 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   111024 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (127)    23997 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    44598 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    29403 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)   190685 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32452 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:24:18.278881 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 18:24:18.000000 nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:24:18.278881 nextstrain_sphinx_theme-2024.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-01 18:24:07.000000 nextstrain_sphinx_theme-2024.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.148846 nextstrain_sphinx_theme-2024.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-08 17:54:14.148846 nextstrain_sphinx_theme-2024.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.144846 nextstrain_sphinx_theme-2024.2/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.140845 nextstrain_sphinx_theme-2024.2/lib/nextstrain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.140845 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.144846 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.144846 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.144846 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/css/nextstrain.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.144846 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/js/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.148846 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111024 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    23997 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44598 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    29403 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)   190685 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32452 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:54:14.148846 nextstrain_sphinx_theme-2024.2/lib/nextstrain_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-08 17:54:14.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-08 17:54:14.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:54:14.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 17:54:14.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 17:54:14.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain_sphinx_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 17:54:14.000000 nextstrain_sphinx_theme-2024.2/lib/nextstrain_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:54:14.148846 nextstrain_sphinx_theme-2024.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-08 17:54:03.000000 nextstrain_sphinx_theme-2024.2/setup.py
```

### Comparing `nextstrain_sphinx_theme-2024.1/LICENSE` & `nextstrain_sphinx_theme-2024.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/PKG-INFO` & `nextstrain_sphinx_theme-2024.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-sphinx-theme
-Version: 2024.1
+Version: 2024.2
 Summary: Nextstrain theme for Sphinx and Read The Docs
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nextstrain_sphinx_theme-2024.1/README.rst` & `nextstrain_sphinx_theme-2024.2/README.rst`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/__init__.py` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/breadcrumbs.html` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/footer.html` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/footer.html`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/layout.html` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/layout.html`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/css/nextstrain.css` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/css/nextstrain.css`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/favicon.ico` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/js/theme.js` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/bz_logo.png`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/icon.png` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/icon.png`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/sib-logo.png`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/logos/unibas-logo.svg`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg`

 * *Files identical despite different names*

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain_sphinx_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextstrain-sphinx-theme
-Version: 2024.1
+Version: 2024.2
 Summary: Nextstrain theme for Sphinx and Read The Docs
 Author: Thomas Sibley
 Author-email: tsibley@fredhutch.org
 License: MIT
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `nextstrain_sphinx_theme-2024.1/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt` & `nextstrain_sphinx_theme-2024.2/lib/nextstrain_sphinx_theme.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 lib/nextstrain/sphinx/theme/theme.conf
 lib/nextstrain/sphinx/theme/static/favicon.ico
 lib/nextstrain/sphinx/theme/static/nextstrain-logo.svg
 lib/nextstrain/sphinx/theme/static/css/nextstrain.css
 lib/nextstrain/sphinx/theme/static/js/theme.js
 lib/nextstrain/sphinx/theme/static/logos/bz_logo.png
 lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo-small.png
-lib/nextstrain/sphinx/theme/static/logos/fred-hutch-logo.png
 lib/nextstrain/sphinx/theme/static/logos/icon.png
 lib/nextstrain/sphinx/theme/static/logos/mapbox-logo-black.svg
 lib/nextstrain/sphinx/theme/static/logos/nextstrain-logo-small.png
 lib/nextstrain/sphinx/theme/static/logos/nextstrain_should_be_svg.png
 lib/nextstrain/sphinx/theme/static/logos/nih-logo-small.png
 lib/nextstrain/sphinx/theme/static/logos/nih-logo.jpg
 lib/nextstrain/sphinx/theme/static/logos/osp-logo-small.png
```

### Comparing `nextstrain_sphinx_theme-2024.1/setup.py` & `nextstrain_sphinx_theme-2024.2/setup.py`

 * *Files identical despite different names*


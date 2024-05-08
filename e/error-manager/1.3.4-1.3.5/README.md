# Comparing `tmp/error_manager-1.3.4.tar.gz` & `tmp/error_manager-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error_manager-1.3.4.tar", last modified: Tue May  7 20:02:53 2024, max compression
+gzip compressed data, was "error_manager-1.3.5.tar", last modified: Wed May  8 15:00:14 2024, max compression
```

## Comparing `error_manager-1.3.4.tar` & `error_manager-1.3.5.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.163318 error_manager-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 20:02:49.000000 error_manager-1.3.4/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:02:49.000000 error_manager-1.3.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 20:02:49.000000 error_manager-1.3.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:02:49.000000 error_manager-1.3.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-07 20:02:49.000000 error_manager-1.3.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-07 20:02:49.000000 error_manager-1.3.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    43710 2024-05-07 20:02:49.000000 error_manager-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 20:02:49.000000 error_manager-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-07 20:02:53.163318 error_manager-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-07 20:02:49.000000 error_manager-1.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.159319 error_manager-1.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.159319 error_manager-1.3.4/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/reference/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/reference/listerrors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/return_value.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-07 20:02:49.000000 error_manager-1.3.4/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 20:02:49.000000 error_manager-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-07 20:02:53.163318 error_manager-1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.155319 error_manager-1.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.163318 error_manager-1.3.4/src/error_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-07 20:02:53.000000 error_manager-1.3.4/src/error_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-07 20:02:53.000000 error_manager-1.3.4/src/error_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:02:53.000000 error_manager-1.3.4/src/error_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 20:02:53.000000 error_manager-1.3.4/src/error_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.163318 error_manager-1.3.4/src/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-07 20:02:49.000000 error_manager-1.3.4/src/errors/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:53.163318 error_manager-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:49.000000 error_manager-1.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-07 20:02:49.000000 error_manager-1.3.4/tests/test_enumerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-07 20:02:49.000000 error_manager-1.3.4/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-07 20:02:49.000000 error_manager-1.3.4/tests/test_return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.672415 error_manager-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 15:00:10.000000 error_manager-1.3.5/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-08 15:00:10.000000 error_manager-1.3.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:00:10.000000 error_manager-1.3.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-08 15:00:10.000000 error_manager-1.3.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 15:00:10.000000 error_manager-1.3.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    43710 2024-05-08 15:00:10.000000 error_manager-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 15:00:10.000000 error_manager-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-08 15:00:14.672415 error_manager-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-08 15:00:10.000000 error_manager-1.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.668414 error_manager-1.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.668414 error_manager-1.3.5/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/reference/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/reference/listerrors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/return_value.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 15:00:10.000000 error_manager-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-08 15:00:14.672415 error_manager-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.664415 error_manager-1.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.672415 error_manager-1.3.5/src/error_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-08 15:00:14.000000 error_manager-1.3.5/src/error_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 15:00:14.000000 error_manager-1.3.5/src/error_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:00:14.000000 error_manager-1.3.5/src/error_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 15:00:14.000000 error_manager-1.3.5/src/error_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.672415 error_manager-1.3.5/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.672415 error_manager-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:10.000000 error_manager-1.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-08 15:00:10.000000 error_manager-1.3.5/tests/test_enumerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-08 15:00:10.000000 error_manager-1.3.5/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-08 15:00:10.000000 error_manager-1.3.5/tests/test_return_value.py
```

### Comparing `error_manager-1.3.4/CHANGELOG.rst` & `error_manager-1.3.5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/CONTRIBUTING.rst` & `error_manager-1.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/LICENSE` & `error_manager-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/PKG-INFO` & `error_manager-1.3.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: error-manager
-Version: 1.3.4
+Version: 1.3.5
 Summary: Manage error codes, descriptions and data in a unified way throughout a project
 Home-page: https://github.com/MaartendeRuyter/errors
 Author: Maarten de Ruyter
 Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
+License: GNU
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =============
 Error Manager
 =============
 
 A lightweight implementation of a manager for error messages throughout your
```

### Comparing `error_manager-1.3.4/README.rst` & `error_manager-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/docs/Makefile` & `error_manager-1.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/docs/conf.py` & `error_manager-1.3.5/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 source_suffix = '.rst'
 master_doc = 'index'
 
 project = 'error manager'
 copyright = '2024, Maarten de Ruyter'
 author = 'Maarten de Ruyter'
-release = '1.3.4'
+release = '1.3.5'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = []
 
 templates_path = ['_templates']
```

### Comparing `error_manager-1.3.4/docs/index.rst` & `error_manager-1.3.5/docs/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -13,75 +13,73 @@
 .. list-table::
     :widths: 8 50
     :stub-columns: 1
 
     * - docs
       - |docs|
     * - tests
-      - |travis| |requires| |codecov|
+      - |travis| |codecov|
     * - package
-      - |version| |supported-versions| |commits-since|
+      - |version| |commits-since|
   
 .. |docs| image:: https://readthedocs.org/projects/errors/badge/?style=flat
     :target: https://errors.readthedocs.io/
     :alt: Documentation Status
 
 .. |travis| image:: https://api.travis-ci.com/MaartendeRuyter/errors.svg?branch=master
     :alt: Travis-CI Build Status
     :target: https://travis-ci.com/github/MaartendeRuyter/errors
 
-.. |requires| image:: https://requires.io/github/MaartendeRuyter/errors/requirements.svg?branch=master
-    :alt: Requirements Status
-    :target: https://requires.io/github/MaartendeRuyter/errors/requirements/?branch=master
-
 .. |codecov| image:: https://codecov.io/gh/MaartendeRuyter/errors/branch/master/graphs/badge.svg?branch=master
     :alt: Coverage Status
     :target: https://codecov.io/github/MaartendeRuyter/errors
 
 .. |version| image:: https://img.shields.io/pypi/v/error-manager.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/error-manager
 
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/error-manager.svg
-    :alt: Supported versions
-    :target: https://pypi.org/project/error-manager
-
 .. |commits-since| image:: https://img.shields.io/github/commits-since/MaartendeRuyter/errors/v0.1.0.svg
     :alt: Commits since latest release
     :target: https://github.com/MaartendeRuyter/errors/compare/v0.1.0...master
 
 
 
 .. end-badges
 
 
-
--------------------
-
-**error-manager main use cases**::
+error-manager main use cases
+----------------------------
+Main use case for the error-manager package is to implement a ``ListErrors`` class that can be used throughout 
+your project to define and access immutable standard error codes and descriptions ::
 
     # retrieve customer defined ErrorCode object form ``ListErrors`` class
     >>> from errors.error import ListErrors
-    >>> error = ListErrors.API_GET_RETURNED_404
-    >>> error
-    ErrorCode(code='ER_API404_00001', description='API get request returned 404', error_data=<class 'dict'>)
+    >>> ListErrors.API_GET_RETURNED_404
+    ErrorCode(
+        code='ER_API404_00001',
+        description='API get request returned 404',
+        error_data={})
     
     # add custom error data to error message when you want to persist or log the error
+    # As the errorcode are immutable the add_error_data returns a new error (immutable) error code. 
     >>> from errors.base import add_error_data
     >>> error_without_data = ListErrors.API_GET_RETURNED_404
     >>> error_with_data = add_error_data(error_without_data, {'url': 'www.bad_url.com'})
     >>> error_with_data 
-    ErrorCode(code='ER_API404_00001', description='API get request returned 404', error_data={'url': 'www.bad_url.com'})
-    
-    # This ErrorCode could be returned by the method performing the request so that
-    # the logic calling this method is aware of the failing request.
+    ErrorCode(
+        code='ER_API404_00001',
+        description='API get request returned 404',
+        error_data={'url': 'www.bad_url.com'})
     
-    # In order to use a single type as return value the error-manager package introduces a `ReturnValue` class
-    # that can hold the actual response, any possible downstream errors and the status of the return value. See 
-    # ReturnValue documentation.
+This ErrorCode could be returned by the method performing the request so that
+the logic calling this method is aware of the failing request.
+
+In order to use a single type as return value the error-manager package introduces a `ReturnValue` class
+that can hold the actual response, any possible downstream errors and the status of the return value. See 
+ReturnValue documentation.
     
 see :doc:`usage section <usage>` on how to create and
 register custom error codes for your project
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
```

### Comparing `error_manager-1.3.4/docs/make.bat` & `error_manager-1.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/docs/return_value.rst` & `error_manager-1.3.5/docs/return_value.rst`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/docs/usage.rst` & `error_manager-1.3.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/src/error_manager.egg-info/PKG-INFO` & `error_manager-1.3.5/src/error_manager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: error-manager
-Version: 1.3.4
+Version: 1.3.5
 Summary: Manage error codes, descriptions and data in a unified way throughout a project
 Home-page: https://github.com/MaartendeRuyter/errors
 Author: Maarten de Ruyter
 Author-email: "Maarten de Ruyter" <maarten@geodatagarden.com>
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
+License: GNU
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =============
 Error Manager
 =============
 
 A lightweight implementation of a manager for error messages throughout your
```

### Comparing `error_manager-1.3.4/src/error_manager.egg-info/SOURCES.txt` & `error_manager-1.3.5/src/error_manager.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .editorconfig
-.isort.cfg
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
```

### Comparing `error_manager-1.3.4/src/errors/base.py` & `error_manager-1.3.5/src/errors/base.py`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/src/errors/data_classes.py` & `error_manager-1.3.5/src/errors/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""_summary_
-"""
+"""_summary_"""
 
 from dataclasses import dataclass, field
 from typing import Any, List
 
 import errors.settings as st
 
 from .base import ErrorCode
```

### Comparing `error_manager-1.3.4/src/errors/error.py` & `error_manager-1.3.5/src/errors/error.py`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/tests/test_enumerator.py` & `error_manager-1.3.5/tests/test_enumerator.py`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/tests/test_errors.py` & `error_manager-1.3.5/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.4/tests/test_return_value.py` & `error_manager-1.3.5/tests/test_return_value.py`

 * *Files identical despite different names*


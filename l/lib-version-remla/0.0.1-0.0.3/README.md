# Comparing `tmp/lib_version_remla-0.0.1.tar.gz` & `tmp/lib_version_remla-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_remla-0.0.1.tar", last modified: Wed May  8 10:29:40 2024, max compression
+gzip compressed data, was "lib_version_remla-0.0.3.tar", last modified: Wed May  8 12:39:20 2024, max compression
```

## Comparing `lib_version_remla-0.0.1.tar` & `lib_version_remla-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 10:29:40.627223 lib_version_remla-0.0.1/
--rw-r--r--   0 jan       (1000) jan       (1000)      506 2024-05-08 10:29:40.623889 lib_version_remla-0.0.1/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)       69 2024-05-08 10:21:36.000000 lib_version_remla-0.0.1/README.md
--rw-r--r--   0 jan       (1000) jan       (1000)      920 2024-05-08 10:29:36.000000 lib_version_remla-0.0.1/pyproject.toml
--rw-r--r--   0 jan       (1000) jan       (1000)       38 2024-05-08 10:29:40.627223 lib_version_remla-0.0.1/setup.cfg
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 10:29:40.623889 lib_version_remla-0.0.1/src/
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 10:29:40.623889 lib_version_remla-0.0.1/src/lib_version_remla/
--rw-r--r--   0 jan       (1000) jan       (1000)        0 2024-05-08 10:15:16.000000 lib_version_remla-0.0.1/src/lib_version_remla/__init__.py
--rw-r--r--   0 jan       (1000) jan       (1000)        0 2024-05-08 10:15:30.000000 lib_version_remla-0.0.1/src/lib_version_remla/return_version.py
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 10:29:40.623889 lib_version_remla-0.0.1/src/lib_version_remla.egg-info/
--rw-r--r--   0 jan       (1000) jan       (1000)      506 2024-05-08 10:29:40.000000 lib_version_remla-0.0.1/src/lib_version_remla.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)      278 2024-05-08 10:29:40.000000 lib_version_remla-0.0.1/src/lib_version_remla.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) jan       (1000)        1 2024-05-08 10:29:40.000000 lib_version_remla-0.0.1/src/lib_version_remla.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) jan       (1000)       18 2024-05-08 10:29:40.000000 lib_version_remla-0.0.1/src/lib_version_remla.egg-info/top_level.txt
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:39:20.640267 lib_version_remla-0.0.3/
+-rw-r--r--   0 jan       (1000) jan       (1000)      765 2024-05-08 12:39:20.636934 lib_version_remla-0.0.3/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)      328 2024-05-08 12:32:45.000000 lib_version_remla-0.0.3/README.md
+-rw-r--r--   0 jan       (1000) jan       (1000)     1031 2024-05-08 12:39:05.000000 lib_version_remla-0.0.3/pyproject.toml
+-rw-r--r--   0 jan       (1000) jan       (1000)       38 2024-05-08 12:39:20.640267 lib_version_remla-0.0.3/setup.cfg
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:39:20.636934 lib_version_remla-0.0.3/src/
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:39:20.636934 lib_version_remla-0.0.3/src/lib_version_remla/
+-rw-r--r--   0 jan       (1000) jan       (1000)      134 2024-05-08 12:20:57.000000 lib_version_remla-0.0.3/src/lib_version_remla/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      129 2024-05-08 12:00:25.000000 lib_version_remla-0.0.3/src/lib_version_remla/return_version.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:39:20.636934 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/
+-rw-r--r--   0 jan       (1000) jan       (1000)      765 2024-05-08 12:39:20.000000 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)      278 2024-05-08 12:39:20.000000 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)        1 2024-05-08 12:39:20.000000 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)       18 2024-05-08 12:39:20.000000 lib_version_remla-0.0.3/src/lib_version_remla.egg-info/top_level.txt
```

### Comparing `lib_version_remla-0.0.1/pyproject.toml` & `lib_version_remla-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "lib_version_remla"
-version = "0.0.1"
+version = "0.0.3"
 description = "A small package which returns its own version."
 authors = ["Jan <j2000.vdm@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project]
 name = "lib_version_remla"
-version = "0.0.1"
+version = "0.0.3"
 description = "A small package which returns its own version."
 authors = [
     { name = "Jan", email="j2000.vdm@gmail.com" },
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -26,11 +26,16 @@
 requires-python = ">=3.11"
 
 [project.urls]
 Homepage = "https://github.com/remla24-team10/lib-version"
 
 [tool.poetry.dependencies]
 python = "^3.11"
+twine = ">=5.0.0"
+
+[tool.build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```


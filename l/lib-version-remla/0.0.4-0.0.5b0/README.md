# Comparing `tmp/lib_version_remla-0.0.4.tar.gz` & `tmp/lib_version_remla-0.0.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_remla-0.0.4.tar", last modified: Wed May  8 12:47:37 2024, max compression
+gzip compressed data, was "lib_version_remla-0.0.5b0.tar", max compression
```

## Comparing `lib_version_remla-0.0.4.tar` & `lib_version_remla-0.0.5b0.tar`

### file list

```diff
@@ -1,13 +1,5 @@
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:47:37.336959 lib_version_remla-0.0.4/
--rw-r--r--   0 jan       (1000) jan       (1000)      897 2024-05-08 12:47:37.333626 lib_version_remla-0.0.4/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)      459 2024-05-08 12:40:53.000000 lib_version_remla-0.0.4/README.md
--rw-r--r--   0 jan       (1000) jan       (1000)     1031 2024-05-08 12:47:26.000000 lib_version_remla-0.0.4/pyproject.toml
--rw-r--r--   0 jan       (1000) jan       (1000)       38 2024-05-08 12:47:37.336959 lib_version_remla-0.0.4/setup.cfg
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:47:37.333626 lib_version_remla-0.0.4/src/
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:47:37.333626 lib_version_remla-0.0.4/src/lib_version_remla/
--rw-r--r--   0 jan       (1000) jan       (1000)       87 2024-05-08 12:46:45.000000 lib_version_remla-0.0.4/src/lib_version_remla/return_version.py
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-08 12:47:37.333626 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/
--rw-r--r--   0 jan       (1000) jan       (1000)      897 2024-05-08 12:47:37.000000 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)      244 2024-05-08 12:47:37.000000 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) jan       (1000)        1 2024-05-08 12:47:37.000000 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) jan       (1000)       18 2024-05-08 12:47:37.000000 lib_version_remla-0.0.4/src/lib_version_remla.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1073 2024-05-08 13:25:05.200175 lib_version_remla-0.0.5b0/LICENSE
+-rw-r--r--   0        0        0      486 2024-05-08 13:25:05.200175 lib_version_remla-0.0.5b0/README.md
+-rw-r--r--   0        0        0     1154 2024-05-08 13:25:22.988188 lib_version_remla-0.0.5b0/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-08 13:25:05.204175 lib_version_remla-0.0.5b0/src/lib_version_remla/return_version.py
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 lib_version_remla-0.0.5b0/PKG-INFO
```

### Comparing `lib_version_remla-0.0.4/pyproject.toml` & `lib_version_remla-0.0.5b0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib_version_remla"
-version = "0.0.4"
+version = "0.0.5b0"
 description = "A small package which returns its own version."
 authors = ["Jan <j2000.vdm@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -33,9 +33,14 @@
 twine = ">=5.0.0"
 
 [tool.build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["poetry-core>=1.8.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = 'git'
+style = 'pep440'
```


# Comparing `tmp/xyscreens-0.0.6.tar.gz` & `tmp/xyscreens-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyscreens-0.0.6.tar", last modified: Tue Dec 13 11:53:12 2022, max compression
+gzip compressed data, was "xyscreens-0.1.0.tar", last modified: Wed May  8 14:03:58 2024, max compression
```

## Comparing `xyscreens-0.0.6.tar` & `xyscreens-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 rogier     (502) staff       (20)        0 2022-12-13 11:53:12.329982 xyscreens-0.0.6/
--rw-r--r--   0 rogier     (502) staff       (20)    11357 2022-11-18 10:04:13.000000 xyscreens-0.0.6/LICENSE
--rw-r--r--   0 rogier     (502) staff       (20)     2571 2022-12-13 11:53:12.329795 xyscreens-0.0.6/PKG-INFO
--rw-r--r--   0 rogier     (502) staff       (20)     1957 2022-12-03 14:17:53.000000 xyscreens-0.0.6/README.md
--rw-r--r--   0 rogier     (502) staff       (20)      890 2022-12-13 11:46:19.000000 xyscreens-0.0.6/pyproject.toml
--rw-r--r--   0 rogier     (502) staff       (20)       38 2022-12-13 11:53:12.330033 xyscreens-0.0.6/setup.cfg
-drwxr-xr-x   0 rogier     (502) staff       (20)        0 2022-12-13 11:53:12.328308 xyscreens-0.0.6/xyscreens/
--rw-r--r--   0 rogier     (502) staff       (20)      226 2022-12-13 11:46:27.000000 xyscreens-0.0.6/xyscreens/__init__.py
--rw-r--r--   0 rogier     (502) staff       (20)     2419 2022-12-13 11:43:25.000000 xyscreens-0.0.6/xyscreens/__main__.py
--rw-r--r--   0 rogier     (502) staff       (20)     8654 2022-12-13 11:22:55.000000 xyscreens-0.0.6/xyscreens/xyscreens.py
-drwxr-xr-x   0 rogier     (502) staff       (20)        0 2022-12-13 11:53:12.329556 xyscreens-0.0.6/xyscreens.egg-info/
--rw-r--r--   0 rogier     (502) staff       (20)     2571 2022-12-13 11:53:12.000000 xyscreens-0.0.6/xyscreens.egg-info/PKG-INFO
--rw-r--r--   0 rogier     (502) staff       (20)      263 2022-12-13 11:53:12.000000 xyscreens-0.0.6/xyscreens.egg-info/SOURCES.txt
--rw-r--r--   0 rogier     (502) staff       (20)        1 2022-12-13 11:53:12.000000 xyscreens-0.0.6/xyscreens.egg-info/dependency_links.txt
--rw-r--r--   0 rogier     (502) staff       (20)       14 2022-12-13 11:53:12.000000 xyscreens-0.0.6/xyscreens.egg-info/requires.txt
--rw-r--r--   0 rogier     (502) staff       (20)       10 2022-12-13 11:53:12.000000 xyscreens-0.0.6/xyscreens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:58.913330 xyscreens-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 14:03:54.000000 xyscreens-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-08 14:03:58.913330 xyscreens-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-08 14:03:54.000000 xyscreens-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 14:03:54.000000 xyscreens-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:03:58.913330 xyscreens-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:58.909330 xyscreens-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-05-08 14:03:54.000000 xyscreens-0.1.0/tests/test_xyscreens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:58.913330 xyscreens-0.1.0/xyscreens/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 14:03:54.000000 xyscreens-0.1.0/xyscreens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-08 14:03:54.000000 xyscreens-0.1.0/xyscreens/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:54.000000 xyscreens-0.1.0/xyscreens/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14105 2024-05-08 14:03:54.000000 xyscreens-0.1.0/xyscreens/xyscreens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:58.913330 xyscreens-0.1.0/xyscreens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-08 14:03:58.000000 xyscreens-0.1.0/xyscreens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-08 14:03:58.000000 xyscreens-0.1.0/xyscreens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:03:58.000000 xyscreens-0.1.0/xyscreens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 14:03:58.000000 xyscreens-0.1.0/xyscreens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 14:03:58.000000 xyscreens-0.1.0/xyscreens.egg-info/top_level.txt
```

### Comparing `xyscreens-0.0.6/LICENSE` & `xyscreens-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xyscreens-0.0.6/pyproject.toml` & `xyscreens-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xyscreens"
-version = "0.0.6"
+version = "0.1.0"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Library to control XY Screens projector screens and projector lifts."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "pyserial>=3.4"
+    "pyserial>=3.5",
+    "pyserial_asyncio>=6"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/rrooggiieerr/xyscreens.py"
 "Bug Tracker" = "https://github.com/rrooggiieerr/xyscreens.py/issues"
 
 [tool.black]
```


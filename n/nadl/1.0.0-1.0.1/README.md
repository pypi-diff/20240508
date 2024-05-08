# Comparing `tmp/nadl-1.0.0.tar.gz` & `tmp/nadl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.0.0.tar", last modified: Mon Apr 22 14:59:04 2024, max compression
+gzip compressed data, was "nadl-1.0.1.tar", last modified: Tue May  7 19:59:39 2024, max compression
```

## Comparing `nadl-1.0.0.tar` & `nadl-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     3973 2024-04-22 14:59:04.117178 nadl-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.0.0/readme.org
--rw-r--r--   0        0        0     1665 2024-04-22 06:25:57.457283 nadl-1.0.0/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.0.0/src/nadl/blocks.py
--rw-r--r--   0        0        0     2988 2024-04-22 06:23:20.541229 nadl-1.0.0/src/nadl/data.py
--rw-r--r--   0        0        0     3170 2024-04-22 06:27:49.753850 nadl-1.0.0/src/nadl/keys.py
--rw-r--r--   0        0        0     3696 2024-04-22 06:27:20.032703 nadl-1.0.0/src/nadl/loops.py
--rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.0.0/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.0.0/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.0.0/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.0.0/src/nadl/py.typed
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.0.0/src/nadl/transformers.py
--rw-r--r--   0        0        0     1964 2024-04-22 04:28:48.528308 nadl-1.0.0/src/nadl/utils.py
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 nadl-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2243 2024-05-07 19:59:39.708240 nadl-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.0.1/readme.org
+-rw-r--r--   0        0        0     1665 2024-05-07 19:58:50.734365 nadl-1.0.1/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.0.1/src/nadl/blocks.py
+-rw-r--r--   0        0        0     2988 2024-04-22 06:23:20.541229 nadl-1.0.1/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.0.1/src/nadl/images.py
+-rw-r--r--   0        0        0     3170 2024-04-22 06:27:49.753850 nadl-1.0.1/src/nadl/keys.py
+-rw-r--r--   0        0        0     3696 2024-04-22 06:27:20.032703 nadl-1.0.1/src/nadl/loops.py
+-rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.0.1/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.0.1/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.0.1/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.0.1/src/nadl/py.typed
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.0.1/src/nadl/transformers.py
+-rw-r--r--   0        0        0     1964 2024-04-22 04:28:48.528308 nadl-1.0.1/src/nadl/utils.py
+-rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 nadl-1.0.1/PKG-INFO
```

### Comparing `nadl-1.0.0/readme.org` & `nadl-1.0.1/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/src/nadl/__init__.py` & `nadl-1.0.1/src/nadl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 )
 from .utils import (
   classit,
   rle,
   rle_array,
 )
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 __all__ = [
   "PG",
   "SCALER",
   "DState",
   "IdxDataloader",
   "Keys",
```

### Comparing `nadl-1.0.0/src/nadl/blocks.py` & `nadl-1.0.1/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/src/nadl/data.py` & `nadl-1.0.1/src/nadl/data.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/src/nadl/keys.py` & `nadl-1.0.1/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/src/nadl/loops.py` & `nadl-1.0.1/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/src/nadl/metrics.py` & `nadl-1.0.1/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/src/nadl/nets.py` & `nadl-1.0.1/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/src/nadl/preprocessing.py` & `nadl-1.0.1/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/src/nadl/transformers.py` & `nadl-1.0.1/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/src/nadl/utils.py` & `nadl-1.0.1/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.0/PKG-INFO` & `nadl-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.0.0
+Version: 1.0.1
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
-Requires-Python: <3.13,>=3.12
+Requires-Python: >=3.11
 Requires-Dist: jax>=0.4.26
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: jaxtyping>=0.2.28
 Requires-Dist: optax>=0.2.2
 Requires-Dist: equinox>=0.11.4
+Requires-Dist: beartype>=0.18.5
+Requires-Dist: scikit-image>=0.23.2
 Requires-Dist: mkdocs-material>=9.5.18; extra == "doc"
 Requires-Dist: mkdocs>=1.5.3; extra == "doc"
 Requires-Dist: mike>=2.0.0; extra == "doc"
 Requires-Dist: mkdocstrings[python]>=0.24.3; extra == "doc"
 Provides-Extra: doc
 Description-Content-Type: text/plain
```


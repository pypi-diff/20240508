# Comparing `tmp/qdsdk-0.0.4.tar.gz` & `tmp/qdsdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdsdk-0.0.4.tar", last modified: Mon May  6 05:35:47 2024, max compression
+gzip compressed data, was "qdsdk-0.0.5.tar", last modified: Wed May  8 03:32:58 2024, max compression
```

## Comparing `qdsdk-0.0.4.tar` & `qdsdk-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 05:35:47.392915 qdsdk-0.0.4/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qdsdk-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       38 2024-04-26 02:46:25.000000 qdsdk-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6161 2024-05-06 05:35:47.392915 qdsdk-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4356 2024-03-18 09:51:27.000000 qdsdk-0.0.4/README.md
--rw-rw-rw-   0        0        0      753 2024-05-06 05:32:05.000000 qdsdk-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 05:35:47.392915 qdsdk-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 05:35:47.346014 qdsdk-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 05:35:47.377303 qdsdk-0.0.4/src/qdsdk/
--rw-rw-rw-   0        0        0      511 2024-04-26 03:23:54.000000 qdsdk-0.0.4/src/qdsdk/__init__.py
--rw-rw-rw-   0        0        0     4498 2024-04-26 03:24:50.000000 qdsdk-0.0.4/src/qdsdk/aio_api.py
--rw-rw-rw-   0        0        0    31311 2024-04-30 06:15:29.000000 qdsdk-0.0.4/src/qdsdk/api.py
--rw-rw-rw-   0        0        0     8348 2024-04-26 02:26:49.000000 qdsdk-0.0.4/src/qdsdk/client.py
--rw-rw-rw-   0        0        0      170 2024-04-25 06:56:16.000000 qdsdk-0.0.4/src/qdsdk/config.py
--rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qdsdk-0.0.4/src/qdsdk/qedata.thrift
--rw-rw-rw-   0        0        0      675 2024-04-26 02:40:38.000000 qdsdk-0.0.4/src/qdsdk/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 05:35:47.392915 qdsdk-0.0.4/src/qdsdk.egg-info/
--rw-rw-rw-   0        0        0     6161 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 03:32:58.594560 qdsdk-0.0.5/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qdsdk-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       38 2024-04-26 02:46:25.000000 qdsdk-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2384 2024-05-08 03:32:58.592574 qdsdk-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2024-05-08 03:28:53.000000 qdsdk-0.0.5/README.md
+-rw-rw-rw-   0        0        0      786 2024-05-08 03:31:45.000000 qdsdk-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:32:58.595548 qdsdk-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 03:32:58.547882 qdsdk-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 03:32:58.575157 qdsdk-0.0.5/src/qdsdk/
+-rw-rw-rw-   0        0        0      511 2024-04-26 03:23:54.000000 qdsdk-0.0.5/src/qdsdk/__init__.py
+-rw-rw-rw-   0        0        0     4498 2024-04-26 03:24:50.000000 qdsdk-0.0.5/src/qdsdk/aio_api.py
+-rw-rw-rw-   0        0        0    31311 2024-04-30 06:15:29.000000 qdsdk-0.0.5/src/qdsdk/api.py
+-rw-rw-rw-   0        0        0     8348 2024-04-26 02:26:49.000000 qdsdk-0.0.5/src/qdsdk/client.py
+-rw-rw-rw-   0        0        0      170 2024-04-25 06:56:16.000000 qdsdk-0.0.5/src/qdsdk/config.py
+-rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qdsdk-0.0.5/src/qdsdk/qedata.thrift
+-rw-rw-rw-   0        0        0      675 2024-04-26 02:40:38.000000 qdsdk-0.0.5/src/qdsdk/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:32:58.590562 qdsdk-0.0.5/src/qdsdk.egg-info/
+-rw-rw-rw-   0        0        0     2384 2024-05-08 03:32:58.000000 qdsdk-0.0.5/src/qdsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-05-08 03:32:58.000000 qdsdk-0.0.5/src/qdsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:32:58.000000 qdsdk-0.0.5/src/qdsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-08 03:32:58.000000 qdsdk-0.0.5/src/qdsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 03:32:58.000000 qdsdk-0.0.5/src/qdsdk.egg-info/top_level.txt
```

### Comparing `qdsdk-0.0.4/LICENSE` & `qdsdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.4/pyproject.toml` & `qdsdk-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qdsdk"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Fisher Yu", email="yuzs@quantdo.com.cn" },
 ]
 description = "QuantDo SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -20,11 +20,11 @@
 dependencies = [
   'msgpack_python>=0.5.6',
   'nest_asyncio>=1.5.5',
   'numpy>=1.19.2',
   'pandas>=1.3.5',
   'thriftpy2>=0.4.14',
 ]
-#[project.urls]
-#"Homepage" = "https://github.com/quantease/qesdk"
+[project.urls]
+"Homepage" = "https://doc.quantdo.com.cn/helpbook/index.html#/cn/qdsdk/0.0.1/README"
 #"Bug Tracker" = "https://github.com/quantease/qesdk/issues"
```

### Comparing `qdsdk-0.0.4/src/qdsdk/aio_api.py` & `qdsdk-0.0.5/src/qdsdk/aio_api.py`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.4/src/qdsdk/api.py` & `qdsdk-0.0.5/src/qdsdk/api.py`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.4/src/qdsdk/client.py` & `qdsdk-0.0.5/src/qdsdk/client.py`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.4/src/qdsdk/qedata.thrift` & `qdsdk-0.0.5/src/qdsdk/qedata.thrift`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.4/src/qdsdk/utils.py` & `qdsdk-0.0.5/src/qdsdk/utils.py`

 * *Files identical despite different names*


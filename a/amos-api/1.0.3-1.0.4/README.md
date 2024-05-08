# Comparing `tmp/amos_api-1.0.3.tar.gz` & `tmp/amos_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amos_api-1.0.3.tar", last modified: Wed May  8 08:21:31 2024, max compression
+gzip compressed data, was "amos_api-1.0.4.tar", last modified: Wed May  8 08:24:03 2024, max compression
```

## Comparing `amos_api-1.0.3.tar` & `amos_api-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 08:21:31.338693 amos_api-1.0.3/
--rw-rw-rw-   0        0        0        4 2024-05-08 07:51:35.000000 amos_api-1.0.3/.gitignore
--rw-rw-rw-   0        0        0       40 2024-05-08 07:40:55.000000 amos_api-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1674 2024-05-08 08:21:31.338693 amos_api-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1222 2024-05-08 06:19:41.000000 amos_api-1.0.3/README.md
--rw-rw-rw-   0        0        0       82 2024-05-08 08:07:22.000000 amos_api-1.0.3/__init__.py
--rw-rw-rw-   0        0        0       86 2024-05-08 07:53:03.000000 amos_api-1.0.3/_descr.md
--rw-rw-rw-   0        0        0      565 2024-05-08 08:21:16.000000 amos_api-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 08:21:31.338693 amos_api-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 08:21:31.333709 amos_api-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 08:21:31.337696 amos_api-1.0.3/src/amos_api.egg-info/
--rw-rw-rw-   0        0        0     1674 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 08:21:31.000000 amos_api-1.0.3/src/amos_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-08 08:07:24.000000 amos_api-1.0.3/src/amos_api.py
--rw-rw-rw-   0        0        0      571 2024-05-08 06:11:21.000000 amos_api-1.0.3/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:24:03.533630 amos_api-1.0.4/
+-rw-rw-rw-   0        0        0        4 2024-05-08 07:51:35.000000 amos_api-1.0.4/.gitignore
+-rw-rw-rw-   0        0        0       40 2024-05-08 07:40:55.000000 amos_api-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1674 2024-05-08 08:24:03.532632 amos_api-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1222 2024-05-08 06:19:41.000000 amos_api-1.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-08 07:53:03.000000 amos_api-1.0.4/_descr.md
+-rw-rw-rw-   0        0        0      565 2024-05-08 08:23:58.000000 amos_api-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 08:24:03.533630 amos_api-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 08:24:03.524619 amos_api-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 08:24:03.532632 amos_api-1.0.4/src/amos_api.egg-info/
+-rw-rw-rw-   0        0        0     1674 2024-05-08 08:24:03.000000 amos_api-1.0.4/src/amos_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-08 08:24:03.000000 amos_api-1.0.4/src/amos_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:24:03.000000 amos_api-1.0.4/src/amos_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 08:24:03.000000 amos_api-1.0.4/src/amos_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-08 08:24:03.000000 amos_api-1.0.4/src/amos_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2024-05-08 08:22:51.000000 amos_api-1.0.4/src/amos_api.py
+-rw-rw-rw-   0        0        0      571 2024-05-08 06:11:21.000000 amos_api-1.0.4/src/utils.py
```

### Comparing `amos_api-1.0.3/PKG-INFO` & `amos_api-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amos_api
-Version: 1.0.3
+Version: 1.0.4
 Summary: AMOS common api
 Author-email: "ilex.h" <390132625@qq.com>
 Project-URL: Homepage, https://github.com/aptray/python-pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
```

### Comparing `amos_api-1.0.3/README.md` & `amos_api-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `amos_api-1.0.3/pyproject.toml` & `amos_api-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "amos_api"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "ilex.h", email = "390132625@qq.com" },
 ]
 dependencies = ['pydantic']
 description = "AMOS common api"
 readme = "README.md"
 requires-python = ">=3"
```

### Comparing `amos_api-1.0.3/src/amos_api.egg-info/PKG-INFO` & `amos_api-1.0.4/src/amos_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amos_api
-Version: 1.0.3
+Version: 1.0.4
 Summary: AMOS common api
 Author-email: "ilex.h" <390132625@qq.com>
 Project-URL: Homepage, https://github.com/aptray/python-pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
```

### Comparing `amos_api-1.0.3/utils.py` & `amos_api-1.0.4/src/utils.py`

 * *Files identical despite different names*


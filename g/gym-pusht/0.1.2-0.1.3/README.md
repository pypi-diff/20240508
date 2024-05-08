# Comparing `tmp/gym_pusht-0.1.2.tar.gz` & `tmp/gym_pusht-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_pusht-0.1.2.tar", max compression
+gzip compressed data, was "gym_pusht-0.1.3.tar", max compression
```

## Comparing `gym_pusht-0.1.2.tar` & `gym_pusht-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12625 2024-04-08 10:15:07.504261 gym_pusht-0.1.2/LICENSE
--rw-r--r--   0        0        0     4267 2024-05-06 15:12:34.087834 gym_pusht-0.1.2/README.md
--rw-r--r--   0        0        0      195 2024-04-09 08:02:09.966097 gym_pusht-0.1.2/gym_pusht/__init__.py
--rw-r--r--   0        0        0       66 2024-04-09 08:02:09.966273 gym_pusht-0.1.2/gym_pusht/envs/__init__.py
--rw-r--r--   0        0        0    17716 2024-05-06 15:12:34.088271 gym_pusht-0.1.2/gym_pusht/envs/pusht.py
--rw-r--r--   0        0        0     8375 2024-04-09 08:02:09.966831 gym_pusht-0.1.2/gym_pusht/envs/pymunk_override.py
--rw-r--r--   0        0        0     1717 2024-05-07 10:02:01.691262 gym_pusht-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5382 1970-01-01 00:00:00.000000 gym_pusht-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    12625 2024-04-08 10:15:07.504261 gym_pusht-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4267 2024-05-06 15:12:34.087834 gym_pusht-0.1.3/README.md
+-rw-r--r--   0        0        0      195 2024-04-09 08:02:09.966097 gym_pusht-0.1.3/gym_pusht/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-09 08:02:09.966273 gym_pusht-0.1.3/gym_pusht/envs/__init__.py
+-rw-r--r--   0        0        0    17716 2024-05-06 15:12:34.088271 gym_pusht-0.1.3/gym_pusht/envs/pusht.py
+-rw-r--r--   0        0        0     8375 2024-04-09 08:02:09.966831 gym_pusht-0.1.3/gym_pusht/envs/pymunk_override.py
+-rw-r--r--   0        0        0     1714 2024-05-08 07:25:12.836161 gym_pusht-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 gym_pusht-0.1.3/PKG-INFO
```

### Comparing `gym_pusht-0.1.2/LICENSE` & `gym_pusht-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gym_pusht-0.1.2/README.md` & `gym_pusht-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gym_pusht-0.1.2/gym_pusht/envs/pusht.py` & `gym_pusht-0.1.3/gym_pusht/envs/pusht.py`

 * *Files identical despite different names*

### Comparing `gym_pusht-0.1.2/gym_pusht/envs/pymunk_override.py` & `gym_pusht-0.1.3/gym_pusht/envs/pymunk_override.py`

 * *Files identical despite different names*

### Comparing `gym_pusht-0.1.2/pyproject.toml` & `gym_pusht-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gym-pusht"
-version = "0.1.2"
+version = "0.1.3"
 description = "A gymnasium environment for PushT."
 authors = [
     "Rémi Cadène <re.cadene@gmail.com>",
     "Quentin Gallouédec <quentin.gallouedec@ec-lyon.fr>",
     "Alexander Soare <alexander.soare159@gmail.com>",
     "Simon Alibert <alibert.sim@gmail.com>",
 ]
@@ -19,15 +19,15 @@
 ]
 packages = [{include = "gym_pusht"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 gymnasium = ">=0.29.1"
-opencv-python = ">=4.9.0.80"
+opencv-python = ">=4.9.0"
 pygame = ">=2.5.2"
 pymunk = ">=6.6.0"
 shapely = ">=2.0.3"
 scikit-image = ">=0.22.0"
 pre-commit = {version = ">=3.7.0", optional = true}
 debugpy = {version = ">=1.8.1", optional = true}
 pytest = {version = ">=8.1.0", optional = true}
```

### Comparing `gym_pusht-0.1.2/PKG-INFO` & `gym_pusht-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-pusht
-Version: 0.1.2
+Version: 0.1.3
 Summary: A gymnasium environment for PushT.
 License: Apache-2.0
 Author: Rémi Cadène
 Author-email: re.cadene@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: debugpy (>=1.8.1) ; extra == "dev"
 Requires-Dist: gymnasium (>=0.29.1)
-Requires-Dist: opencv-python (>=4.9.0.80)
+Requires-Dist: opencv-python (>=4.9.0)
 Requires-Dist: pre-commit (>=3.7.0) ; extra == "dev"
 Requires-Dist: pygame (>=2.5.2)
 Requires-Dist: pymunk (>=6.6.0)
 Requires-Dist: pytest (>=8.1.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=5.0.0) ; extra == "test"
 Requires-Dist: scikit-image (>=0.22.0)
 Requires-Dist: shapely (>=2.0.3)
```


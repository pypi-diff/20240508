# Comparing `tmp/simple_kfp_task_stub-0.0.1.tar.gz` & `tmp/simple_kfp_task_stub-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_kfp_task_stub-0.0.1.tar", last modified: Wed May  8 07:57:54 2024, max compression
+gzip compressed data, was "simple_kfp_task_stub-0.0.2.tar", last modified: Wed May  8 08:04:33 2024, max compression
```

## Comparing `simple_kfp_task_stub-0.0.1.tar` & `simple_kfp_task_stub-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 seal01-admin   (503) staff       (20)        0 2024-05-08 07:57:54.624097 simple_kfp_task_stub-0.0.1/
--rw-r--r--   0 seal01-admin   (503) staff       (20)     1077 2024-05-08 07:53:05.000000 simple_kfp_task_stub-0.0.1/LICENSE
--rw-r--r--   0 seal01-admin   (503) staff       (20)      570 2024-05-08 07:57:54.623869 simple_kfp_task_stub-0.0.1/PKG-INFO
--rw-r--r--   0 seal01-admin   (503) staff       (20)        0 2024-05-08 07:53:05.000000 simple_kfp_task_stub-0.0.1/README.md
--rw-r--r--   0 seal01-admin   (503) staff       (20)      640 2024-05-08 07:56:59.000000 simple_kfp_task_stub-0.0.1/pyproject.toml
--rw-r--r--   0 seal01-admin   (503) staff       (20)       38 2024-05-08 07:57:54.624140 simple_kfp_task_stub-0.0.1/setup.cfg
-drwxr-xr-x   0 seal01-admin   (503) staff       (20)        0 2024-05-08 07:57:54.623124 simple_kfp_task_stub-0.0.1/simple_kfp_task/
--rw-r--r--   0 seal01-admin   (503) staff       (20)       20 2024-05-08 07:53:20.000000 simple_kfp_task_stub-0.0.1/simple_kfp_task/__init__.py
--rw-r--r--   0 seal01-admin   (503) staff       (20)      451 2024-05-08 07:55:36.000000 simple_kfp_task_stub-0.0.1/simple_kfp_task/task.py
-drwxr-xr-x   0 seal01-admin   (503) staff       (20)        0 2024-05-08 07:57:54.623705 simple_kfp_task_stub-0.0.1/simple_kfp_task_stub.egg-info/
--rw-r--r--   0 seal01-admin   (503) staff       (20)      570 2024-05-08 07:57:54.000000 simple_kfp_task_stub-0.0.1/simple_kfp_task_stub.egg-info/PKG-INFO
--rw-r--r--   0 seal01-admin   (503) staff       (20)      260 2024-05-08 07:57:54.000000 simple_kfp_task_stub-0.0.1/simple_kfp_task_stub.egg-info/SOURCES.txt
--rw-r--r--   0 seal01-admin   (503) staff       (20)        1 2024-05-08 07:57:54.000000 simple_kfp_task_stub-0.0.1/simple_kfp_task_stub.egg-info/dependency_links.txt
--rw-r--r--   0 seal01-admin   (503) staff       (20)       16 2024-05-08 07:57:54.000000 simple_kfp_task_stub-0.0.1/simple_kfp_task_stub.egg-info/top_level.txt
+drwxr-xr-x   0 seal01-admin   (503) staff       (20)        0 2024-05-08 08:04:33.323071 simple_kfp_task_stub-0.0.2/
+-rw-r--r--   0 seal01-admin   (503) staff       (20)     1077 2024-05-08 07:53:05.000000 simple_kfp_task_stub-0.0.2/LICENSE
+-rw-r--r--   0 seal01-admin   (503) staff       (20)      570 2024-05-08 08:04:33.322852 simple_kfp_task_stub-0.0.2/PKG-INFO
+-rw-r--r--   0 seal01-admin   (503) staff       (20)        0 2024-05-08 07:53:05.000000 simple_kfp_task_stub-0.0.2/README.md
+-rw-r--r--   0 seal01-admin   (503) staff       (20)      640 2024-05-08 08:03:46.000000 simple_kfp_task_stub-0.0.2/pyproject.toml
+-rw-r--r--   0 seal01-admin   (503) staff       (20)       38 2024-05-08 08:04:33.323117 simple_kfp_task_stub-0.0.2/setup.cfg
+drwxr-xr-x   0 seal01-admin   (503) staff       (20)        0 2024-05-08 08:04:33.321653 simple_kfp_task_stub-0.0.2/simple_kfp_task/
+-rw-r--r--   0 seal01-admin   (503) staff       (20)       20 2024-05-08 07:53:20.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task/__init__.py
+-rw-r--r--   0 seal01-admin   (503) staff       (20)      347 2024-05-08 08:03:19.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task/task.py
+drwxr-xr-x   0 seal01-admin   (503) staff       (20)        0 2024-05-08 08:04:33.322506 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/
+-rw-r--r--   0 seal01-admin   (503) staff       (20)      570 2024-05-08 08:04:33.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/PKG-INFO
+-rw-r--r--   0 seal01-admin   (503) staff       (20)      260 2024-05-08 08:04:33.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/SOURCES.txt
+-rw-r--r--   0 seal01-admin   (503) staff       (20)        1 2024-05-08 08:04:33.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/dependency_links.txt
+-rw-r--r--   0 seal01-admin   (503) staff       (20)       16 2024-05-08 08:04:33.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/top_level.txt
```

### Comparing `simple_kfp_task_stub-0.0.1/LICENSE` & `simple_kfp_task_stub-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_kfp_task_stub-0.0.1/PKG-INFO` & `simple_kfp_task_stub-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task-stub
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task-stub
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task-stub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_kfp_task_stub-0.0.1/pyproject.toml` & `simple_kfp_task_stub-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-kfp-task-stub"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Sebastian Alberternst", email="sebastian.alberternst@dfki.de" },
 ]
 description = "Generate a simple Kubeflow Pipeline task"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simple_kfp_task_stub-0.0.1/simple_kfp_task_stub.egg-info/PKG-INFO` & `simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task-stub
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task-stub
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task-stub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


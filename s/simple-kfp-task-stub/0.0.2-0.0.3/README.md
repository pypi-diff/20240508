# Comparing `tmp/simple_kfp_task_stub-0.0.2.tar.gz` & `tmp/simple_kfp_task_stub-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_kfp_task_stub-0.0.2.tar", last modified: Wed May  8 08:04:33 2024, max compression
+gzip compressed data, was "simple_kfp_task_stub-0.0.3.tar", last modified: Wed May  8 08:22:09 2024, max compression
```

## Comparing `simple_kfp_task_stub-0.0.2.tar` & `simple_kfp_task_stub-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 seal01-admin   (503) staff       (20)        0 2024-05-08 08:04:33.323071 simple_kfp_task_stub-0.0.2/
--rw-r--r--   0 seal01-admin   (503) staff       (20)     1077 2024-05-08 07:53:05.000000 simple_kfp_task_stub-0.0.2/LICENSE
--rw-r--r--   0 seal01-admin   (503) staff       (20)      570 2024-05-08 08:04:33.322852 simple_kfp_task_stub-0.0.2/PKG-INFO
--rw-r--r--   0 seal01-admin   (503) staff       (20)        0 2024-05-08 07:53:05.000000 simple_kfp_task_stub-0.0.2/README.md
--rw-r--r--   0 seal01-admin   (503) staff       (20)      640 2024-05-08 08:03:46.000000 simple_kfp_task_stub-0.0.2/pyproject.toml
--rw-r--r--   0 seal01-admin   (503) staff       (20)       38 2024-05-08 08:04:33.323117 simple_kfp_task_stub-0.0.2/setup.cfg
-drwxr-xr-x   0 seal01-admin   (503) staff       (20)        0 2024-05-08 08:04:33.321653 simple_kfp_task_stub-0.0.2/simple_kfp_task/
--rw-r--r--   0 seal01-admin   (503) staff       (20)       20 2024-05-08 07:53:20.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task/__init__.py
--rw-r--r--   0 seal01-admin   (503) staff       (20)      347 2024-05-08 08:03:19.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task/task.py
-drwxr-xr-x   0 seal01-admin   (503) staff       (20)        0 2024-05-08 08:04:33.322506 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/
--rw-r--r--   0 seal01-admin   (503) staff       (20)      570 2024-05-08 08:04:33.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/PKG-INFO
--rw-r--r--   0 seal01-admin   (503) staff       (20)      260 2024-05-08 08:04:33.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/SOURCES.txt
--rw-r--r--   0 seal01-admin   (503) staff       (20)        1 2024-05-08 08:04:33.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/dependency_links.txt
--rw-r--r--   0 seal01-admin   (503) staff       (20)       16 2024-05-08 08:04:33.000000 simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:22:09.335293 simple_kfp_task_stub-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-08 08:22:04.000000 simple_kfp_task_stub-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-08 08:22:09.335293 simple_kfp_task_stub-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 08:22:04.000000 simple_kfp_task_stub-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:22:09.335293 simple_kfp_task_stub-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:22:09.335293 simple_kfp_task_stub-0.0.3/simple_kfp_task/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 08:22:04.000000 simple_kfp_task_stub-0.0.3/simple_kfp_task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 08:22:04.000000 simple_kfp_task_stub-0.0.3/simple_kfp_task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:22:09.335293 simple_kfp_task_stub-0.0.3/simple_kfp_task_stub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-08 08:22:09.000000 simple_kfp_task_stub-0.0.3/simple_kfp_task_stub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 08:22:09.000000 simple_kfp_task_stub-0.0.3/simple_kfp_task_stub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:22:09.000000 simple_kfp_task_stub-0.0.3/simple_kfp_task_stub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 08:22:09.000000 simple_kfp_task_stub-0.0.3/simple_kfp_task_stub.egg-info/top_level.txt
```

### Comparing `simple_kfp_task_stub-0.0.2/LICENSE` & `simple_kfp_task_stub-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_kfp_task_stub-0.0.2/PKG-INFO` & `simple_kfp_task_stub-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task-stub
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task-stub
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task-stub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simple_kfp_task_stub-0.0.2/pyproject.toml` & `simple_kfp_task_stub-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-kfp-task-stub"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Sebastian Alberternst", email="sebastian.alberternst@dfki.de" },
 ]
 description = "Generate a simple Kubeflow Pipeline task"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/salberternst/simple-kfp-task-stub"
-Issues = "https://github.com/salberternst/simple-kfp-task-stub/issues"
+Issues = "https://github.com/salberternst/simple-kfp-task-stub/issues"
```

### Comparing `simple_kfp_task_stub-0.0.2/simple_kfp_task_stub.egg-info/PKG-INFO` & `simple_kfp_task_stub-0.0.3/simple_kfp_task_stub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-kfp-task-stub
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate a simple Kubeflow Pipeline task
 Author-email: Sebastian Alberternst <sebastian.alberternst@dfki.de>
 Project-URL: Homepage, https://github.com/salberternst/simple-kfp-task-stub
 Project-URL: Issues, https://github.com/salberternst/simple-kfp-task-stub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


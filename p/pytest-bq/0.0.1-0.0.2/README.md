# Comparing `tmp/pytest_bq-0.0.1.tar.gz` & `tmp/pytest_bq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_bq-0.0.1.tar", last modified: Wed May  8 15:26:10 2024, max compression
+gzip compressed data, was "pytest_bq-0.0.2.tar", last modified: Wed May  8 16:04:37 2024, max compression
```

## Comparing `pytest_bq-0.0.1.tar` & `pytest_bq-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:10.097766 pytest_bq-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-08 15:26:10.097766 pytest_bq-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:10.093767 pytest_bq-0.0.1/pytest_bq/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pytest_bq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pytest_bq/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:10.097766 pytest_bq-0.0.1/pytest_bq/executor/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pytest_bq/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pytest_bq/executor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:10.097766 pytest_bq-0.0.1/pytest_bq/factories/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pytest_bq/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pytest_bq/factories/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pytest_bq/factories/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pytest_bq/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/pytest_bq/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:10.097766 pytest_bq-0.0.1/pytest_bq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-08 15:26:10.000000 pytest_bq-0.0.1/pytest_bq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-08 15:26:10.000000 pytest_bq-0.0.1/pytest_bq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:26:10.000000 pytest_bq-0.0.1/pytest_bq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 15:26:10.000000 pytest_bq-0.0.1/pytest_bq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 15:26:10.000000 pytest_bq-0.0.1/pytest_bq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 15:26:10.000000 pytest_bq-0.0.1/pytest_bq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:26:10.097766 pytest_bq-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:26:10.097766 pytest_bq-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-08 15:26:04.000000 pytest_bq-0.0.1/tests/test_bq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.980794 pytest_bq-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-08 16:04:37.980794 pytest_bq-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/pytest_bq/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/pytest_bq/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/executor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/pytest_bq/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/factories/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/factories/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/pytest_bq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:04:37.980794 pytest_bq-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/tests/test_bq.py
```

### Comparing `pytest_bq-0.0.1/LICENSE` & `pytest_bq-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.1/PKG-INFO` & `pytest_bq-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-bq
-Version: 0.0.1
+Version: 0.0.2
 Summary: BigQuery fixtures and fixture factories for Pytest.
 Author-email: Sam Pegler <sam@sampegler.co.uk>
 License: Copyright (c) 2024 Sam Pegler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -51,17 +51,17 @@
 Requires-Dist: port-for
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pydocstyle; extra == "test"
 Requires-Dist: isort; extra == "test"
 
-## Pytest GCS
+## Pytest BQ
 
-This is a pytest plugin in similar vein to [pytest-postgres](https://github.com/ClearcodeHQ/pytest-postgresql) and [pytest-kafka](https://pypi.org/project/pytest-kafka/).
+This is a pytest plugin in similar vein to [pytest-postgres](https://github.com/ClearcodeHQ/pytest-postgresql) and [pytest-kafka](https://pypi.org/project/pytest-kafka/). It runs a local version of bigquery that you can use throughout your test suite. 
 
 This would have been much more painful without [Mirakuru](https://github.com/ClearcodeHQ/mirakuru)
 and [bigquery-emulator](https://github.com/goccy/bigquery-emulator); this is a simple wrapper around
 those tools.
 
 
 ### Installation
@@ -121,8 +121,9 @@
 # Run the tests.
 pytest tests/
 ```
 
 
 ### TODOs
 
-* Implement the events outputs, `-event.bucket`, `-event.list`, etc.
+* Validate `data_from_yaml` files.
+* Tools for dummy data generation.
```

### Comparing `pytest_bq-0.0.1/README.md` & `pytest_bq-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-## Pytest GCS
+## Pytest BQ
 
-This is a pytest plugin in similar vein to [pytest-postgres](https://github.com/ClearcodeHQ/pytest-postgresql) and [pytest-kafka](https://pypi.org/project/pytest-kafka/).
+This is a pytest plugin in similar vein to [pytest-postgres](https://github.com/ClearcodeHQ/pytest-postgresql) and [pytest-kafka](https://pypi.org/project/pytest-kafka/). It runs a local version of bigquery that you can use throughout your test suite. 
 
 This would have been much more painful without [Mirakuru](https://github.com/ClearcodeHQ/mirakuru)
 and [bigquery-emulator](https://github.com/goccy/bigquery-emulator); this is a simple wrapper around
 those tools.
 
 
 ### Installation
@@ -64,8 +64,9 @@
 # Run the tests.
 pytest tests/
 ```
 
 
 ### TODOs
 
-* Implement the events outputs, `-event.bucket`, `-event.list`, etc.
+* Validate `data_from_yaml` files.
+* Tools for dummy data generation.
```

### Comparing `pytest_bq-0.0.1/pyproject.toml` & `pytest_bq-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-bq"
-version = "0.0.1"
+version = "0.0.2"
 description = "BigQuery fixtures and fixture factories for Pytest."
 readme = "README.md"
 keywords = ["tests", "pytest", "fixture", "bq"]
 license = {file = "LICENSE"}
 authors = [
     {name = "Sam Pegler", email = "sam@sampegler.co.uk"}
 ]
```

### Comparing `pytest_bq-0.0.1/pytest_bq/config.py` & `pytest_bq-0.0.2/pytest_bq/config.py`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.1/pytest_bq/executor/process.py` & `pytest_bq-0.0.2/pytest_bq/executor/process.py`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.1/pytest_bq/factories/client.py` & `pytest_bq-0.0.2/pytest_bq/factories/client.py`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.1/pytest_bq/factories/proc.py` & `pytest_bq-0.0.2/pytest_bq/factories/proc.py`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.1/pytest_bq/plugin.py` & `pytest_bq-0.0.2/pytest_bq/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.1/pytest_bq.egg-info/PKG-INFO` & `pytest_bq-0.0.2/pytest_bq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-bq
-Version: 0.0.1
+Version: 0.0.2
 Summary: BigQuery fixtures and fixture factories for Pytest.
 Author-email: Sam Pegler <sam@sampegler.co.uk>
 License: Copyright (c) 2024 Sam Pegler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -51,17 +51,17 @@
 Requires-Dist: port-for
 Provides-Extra: test
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pydocstyle; extra == "test"
 Requires-Dist: isort; extra == "test"
 
-## Pytest GCS
+## Pytest BQ
 
-This is a pytest plugin in similar vein to [pytest-postgres](https://github.com/ClearcodeHQ/pytest-postgresql) and [pytest-kafka](https://pypi.org/project/pytest-kafka/).
+This is a pytest plugin in similar vein to [pytest-postgres](https://github.com/ClearcodeHQ/pytest-postgresql) and [pytest-kafka](https://pypi.org/project/pytest-kafka/). It runs a local version of bigquery that you can use throughout your test suite. 
 
 This would have been much more painful without [Mirakuru](https://github.com/ClearcodeHQ/mirakuru)
 and [bigquery-emulator](https://github.com/goccy/bigquery-emulator); this is a simple wrapper around
 those tools.
 
 
 ### Installation
@@ -121,8 +121,9 @@
 # Run the tests.
 pytest tests/
 ```
 
 
 ### TODOs
 
-* Implement the events outputs, `-event.bucket`, `-event.list`, etc.
+* Validate `data_from_yaml` files.
+* Tools for dummy data generation.
```

### Comparing `pytest_bq-0.0.1/tests/test_bq.py` & `pytest_bq-0.0.2/tests/test_bq.py`

 * *Files identical despite different names*


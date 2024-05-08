# Comparing `tmp/pytest_bq-0.0.2.tar.gz` & `tmp/pytest_bq-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_bq-0.0.2.tar", last modified: Wed May  8 16:04:37 2024, max compression
+gzip compressed data, was "pytest_bq-0.0.3.tar", last modified: Wed May  8 18:16:24 2024, max compression
```

## Comparing `pytest_bq-0.0.2.tar` & `pytest_bq-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.980794 pytest_bq-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-08 16:04:37.980794 pytest_bq-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/pytest_bq/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/pytest_bq/executor/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/executor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/pytest_bq/factories/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/factories/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/factories/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/pytest_bq/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/pytest_bq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 16:04:37.000000 pytest_bq-0.0.2/pytest_bq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:04:37.980794 pytest_bq-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:04:37.976794 pytest_bq-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-08 16:04:33.000000 pytest_bq-0.0.2/tests/test_bq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:24.001554 pytest_bq-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-08 18:16:24.001554 pytest_bq-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:23.997554 pytest_bq-0.0.3/pytest_bq/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pytest_bq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pytest_bq/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:23.997554 pytest_bq-0.0.3/pytest_bq/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pytest_bq/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pytest_bq/executor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:23.997554 pytest_bq-0.0.3/pytest_bq/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pytest_bq/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pytest_bq/factories/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pytest_bq/factories/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pytest_bq/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/pytest_bq/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:23.997554 pytest_bq-0.0.3/pytest_bq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-08 18:16:23.000000 pytest_bq-0.0.3/pytest_bq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-08 18:16:23.000000 pytest_bq-0.0.3/pytest_bq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:16:23.000000 pytest_bq-0.0.3/pytest_bq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 18:16:23.000000 pytest_bq-0.0.3/pytest_bq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 18:16:23.000000 pytest_bq-0.0.3/pytest_bq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 18:16:23.000000 pytest_bq-0.0.3/pytest_bq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:16:24.001554 pytest_bq-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:16:23.997554 pytest_bq-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-08 18:16:19.000000 pytest_bq-0.0.3/tests/test_bq.py
```

### Comparing `pytest_bq-0.0.2/LICENSE` & `pytest_bq-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.2/PKG-INFO` & `pytest_bq-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-bq
-Version: 0.0.2
+Version: 0.0.3
 Summary: BigQuery fixtures and fixture factories for Pytest.
 Author-email: Sam Pegler <sam@sampegler.co.uk>
 License: Copyright (c) 2024 Sam Pegler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `pytest_bq-0.0.2/README.md` & `pytest_bq-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.2/pyproject.toml` & `pytest_bq-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-bq"
-version = "0.0.2"
+version = "0.0.3"
 description = "BigQuery fixtures and fixture factories for Pytest."
 readme = "README.md"
 keywords = ["tests", "pytest", "fixture", "bq"]
 license = {file = "LICENSE"}
 authors = [
     {name = "Sam Pegler", email = "sam@sampegler.co.uk"}
 ]
```

### Comparing `pytest_bq-0.0.2/pytest_bq/config.py` & `pytest_bq-0.0.3/pytest_bq/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 
 class GcsConfigType(TypedDict):
     """pytest-bq config definition type."""
 
     executable: str
     port: Optional[int]
-    groc_port: Optional[int]
+    grpc_port: Optional[int]
     project_id: str
     loglevel: str
+    data_from_yaml: str
 
 
 def get_config(request: FixtureRequest) -> GcsConfigType:
     """Return a dictionary with config options."""
 
     def get_conf_option(option: str) -> Any:
         option_name = "bq_" + option
```

### Comparing `pytest_bq-0.0.2/pytest_bq/executor/process.py` & `pytest_bq-0.0.3/pytest_bq/executor/process.py`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.2/pytest_bq/factories/client.py` & `pytest_bq-0.0.3/pytest_bq/factories/client.py`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.2/pytest_bq/factories/proc.py` & `pytest_bq-0.0.3/pytest_bq/factories/proc.py`

 * *Files identical despite different names*

### Comparing `pytest_bq-0.0.2/pytest_bq/plugin.py` & `pytest_bq-0.0.3/pytest_bq/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 _HELP_HOST = "Host to run bq service on."
 _HELP_PORT = "Port to run bq service on."
 _HELP_GRPC_PORT = ""
 _HELP_LOGLEVEL = (
     "Level for bucket logging. level for logging. Options"
     " same as for logrus: trace, debug, info, warn, error, fatal, and panic"
 )
-_HELP_PROJECT_ID = ""
-_HELP_DATA_FROM_YAML = ""
+_HELP_PROJECT_ID = "Project ID to use."
+_HELP_DATA_FROM_YAML = "bigquery-emulator configuration to use."
 
 
 def pytest_addoption(parser: Parser) -> None:
     """Plugin configuration options."""
     parser.addini(
         name="bq_executable", help=_HELP_EXEC, default=which("bigquery")
     )
```

### Comparing `pytest_bq-0.0.2/pytest_bq.egg-info/PKG-INFO` & `pytest_bq-0.0.3/pytest_bq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-bq
-Version: 0.0.2
+Version: 0.0.3
 Summary: BigQuery fixtures and fixture factories for Pytest.
 Author-email: Sam Pegler <sam@sampegler.co.uk>
 License: Copyright (c) 2024 Sam Pegler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `pytest_bq-0.0.2/tests/test_bq.py` & `pytest_bq-0.0.3/tests/test_bq.py`

 * *Files identical despite different names*


# Comparing `tmp/langgraph_sdk-0.1.3.tar.gz` & `tmp/langgraph_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_sdk-0.1.3.tar", max compression
+gzip compressed data, was "langgraph_sdk-0.1.4.tar", max compression
```

## Comparing `langgraph_sdk-0.1.3.tar` & `langgraph_sdk-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       12 2024-05-08 04:47:04.090972 langgraph_sdk-0.1.3/README.md
--rw-r--r--   0        0        0       70 2024-05-08 04:47:04.091058 langgraph_sdk-0.1.3/langgraph_sdk/__init__.py
--rw-r--r--   0        0        0     9616 2024-05-08 04:47:04.091177 langgraph_sdk-0.1.3/langgraph_sdk/client.py
--rw-r--r--   0        0        0     3212 2024-05-08 04:47:04.091240 langgraph_sdk-0.1.3/langgraph_sdk/schema.py
--rw-r--r--   0        0        0     1005 2024-05-08 04:48:55.960823 langgraph_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-08 04:47:04.090972 langgraph_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0       70 2024-05-08 04:47:04.091058 langgraph_sdk-0.1.4/langgraph_sdk/__init__.py
+-rw-r--r--   0        0        0     9616 2024-05-08 04:47:04.091177 langgraph_sdk-0.1.4/langgraph_sdk/client.py
+-rw-r--r--   0        0        0     3212 2024-05-08 04:47:04.091240 langgraph_sdk-0.1.4/langgraph_sdk/schema.py
+-rw-r--r--   0        0        0     1004 2024-05-08 05:02:56.476079 langgraph_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.4/PKG-INFO
```

### Comparing `langgraph_sdk-0.1.3/langgraph_sdk/client.py` & `langgraph_sdk-0.1.4/langgraph_sdk/client.py`

 * *Files identical despite different names*

### Comparing `langgraph_sdk-0.1.3/langgraph_sdk/schema.py` & `langgraph_sdk-0.1.4/langgraph_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `langgraph_sdk-0.1.3/pyproject.toml` & `langgraph_sdk-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "langgraph-sdk"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_sdk"}]
 
 [tool.poetry.dependencies]
-python = "^3.9.0,<3.13"
+python = "^3.9.0,<4.0"
 httpx = "0.25.2"
 httpx-sse = "^0.4.0"
 orjson = "^3.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.4"
 codespell = "^2.2.0"
```

### Comparing `langgraph_sdk-0.1.3/PKG-INFO` & `langgraph_sdk-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: langgraph-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Nuno Campos
 Author-email: nuno@langchain.dev
-Requires-Python: >=3.9.0,<3.13
+Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (==0.25.2)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
 Requires-Dist: orjson (>=3.10.1,<4.0.0)
```


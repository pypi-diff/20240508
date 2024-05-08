# Comparing `tmp/llama_index_llms_anyscale-0.1.2.tar.gz` & `tmp/llama_index_llms_anyscale-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_anyscale-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_llms_anyscale-0.1.3.tar", max compression
```

## Comparing `llama_index_llms_anyscale-0.1.2.tar` & `llama_index_llms_anyscale-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0       40 2024-02-16 00:43:36.625451 llama_index_llms_anyscale-0.1.2/README.md
--rw-r--r--   0        0        0       17 2024-02-16 00:43:36.735451 llama_index_llms_anyscale-0.1.2/llama_index/llms/anyscale/BUILD
--rw-r--r--   0        0        0       76 2024-02-16 00:43:36.735451 llama_index_llms_anyscale-0.1.2/llama_index/llms/anyscale/__init__.py
--rw-r--r--   0        0        0     2721 2024-02-20 16:28:03.466443 llama_index_llms_anyscale-0.1.2/llama_index/llms/anyscale/base.py
--rw-r--r--   0        0        0     3645 2024-02-20 16:28:03.466443 llama_index_llms_anyscale-0.1.2/llama_index/llms/anyscale/utils.py
--rw-r--r--   0        0        0     1442 2024-02-20 16:46:34.509716 llama_index_llms_anyscale-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 llama_index_llms_anyscale-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-02-13 13:53:01.651916 llama_index_llms_anyscale-0.1.3/README.md
+-rw-r--r--   0        0        0       76 2024-02-13 13:53:01.652107 llama_index_llms_anyscale-0.1.3/llama_index/llms/anyscale/__init__.py
+-rw-r--r--   0        0        0     2721 2024-02-20 22:37:41.290772 llama_index_llms_anyscale-0.1.3/llama_index/llms/anyscale/base.py
+-rw-r--r--   0        0        0     3645 2024-02-20 22:37:41.290863 llama_index_llms_anyscale-0.1.3/llama_index/llms/anyscale/utils.py
+-rw-r--r--   0        0        0     1464 2024-02-21 17:33:20.656776 llama_index_llms_anyscale-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 llama_index_llms_anyscale-0.1.3/PKG-INFO
```

### Comparing `llama_index_llms_anyscale-0.1.2/llama_index/llms/anyscale/base.py` & `llama_index_llms_anyscale-0.1.3/llama_index/llms/anyscale/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_anyscale-0.1.2/llama_index/llms/anyscale/utils.py` & `llama_index_llms_anyscale-0.1.3/llama_index/llms/anyscale/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_anyscale-0.1.2/pyproject.toml` & `llama_index_llms_anyscale-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms anyscale integration"
+exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-anyscale"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12"
+python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-llms-openai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
```

### Comparing `llama_index_llms_anyscale-0.1.2/PKG-INFO` & `llama_index_llms_anyscale-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-anyscale
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index llms anyscale integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.8.1,<3.12
+Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Anyscale
```


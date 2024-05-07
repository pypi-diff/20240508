# Comparing `tmp/jsonschema_markdown-0.3.7.tar.gz` & `tmp/jsonschema_markdown-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_markdown-0.3.7.tar", max compression
+gzip compressed data, was "jsonschema_markdown-0.3.8.tar", max compression
```

## Comparing `jsonschema_markdown-0.3.7.tar` & `jsonschema_markdown-0.3.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/LICENSE
--rw-r--r--   0        0        0     3152 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/README.md
--rw-r--r--   0        0        0       81 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/converter/__init__.py
--rw-r--r--   0        0        0    15971 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/converter/markdown.py
--rw-r--r--   0        0        0     1606 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/main.py
--rw-r--r--   0        0        0     1103 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/utils.py
--rw-r--r--   0        0        0     1340 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 jsonschema_markdown-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-07 22:59:52.023644 jsonschema_markdown-0.3.8/LICENSE
+-rw-r--r--   0        0        0     3152 2024-05-07 22:59:52.023644 jsonschema_markdown-0.3.8/README.md
+-rw-r--r--   0        0        0       81 2024-05-07 22:59:52.023644 jsonschema_markdown-0.3.8/jsonschema_markdown/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:59:52.023644 jsonschema_markdown-0.3.8/jsonschema_markdown/converter/__init__.py
+-rw-r--r--   0        0        0    15971 2024-05-07 22:59:52.023644 jsonschema_markdown-0.3.8/jsonschema_markdown/converter/markdown.py
+-rw-r--r--   0        0        0     1606 2024-05-07 22:59:52.023644 jsonschema_markdown-0.3.8/jsonschema_markdown/main.py
+-rw-r--r--   0        0        0     1103 2024-05-07 22:59:52.023644 jsonschema_markdown-0.3.8/jsonschema_markdown/utils.py
+-rw-r--r--   0        0        0     1340 2024-05-07 22:59:52.023644 jsonschema_markdown-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 jsonschema_markdown-0.3.8/PKG-INFO
```

### Comparing `jsonschema_markdown-0.3.7/LICENSE` & `jsonschema_markdown-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.7/README.md` & `jsonschema_markdown-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.7/jsonschema_markdown/converter/markdown.py` & `jsonschema_markdown-0.3.8/jsonschema_markdown/converter/markdown.py`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.7/jsonschema_markdown/main.py` & `jsonschema_markdown-0.3.8/jsonschema_markdown/main.py`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.7/jsonschema_markdown/utils.py` & `jsonschema_markdown-0.3.8/jsonschema_markdown/utils.py`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.7/pyproject.toml` & `jsonschema_markdown-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "jsonschema-markdown"
 license = "MIT"
-version = "0.3.7"
+version = "0.3.8"
 description = "Export a JSON Schema document to Markdown documentation."
 authors = ["Elisiário Couto <elisiario@couto.io>"]
 repository = "https://github.com/elisiariocouto/jsonschema-markdown"
 readme = "README.md"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
```

### Comparing `jsonschema_markdown-0.3.7/PKG-INFO` & `jsonschema_markdown-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-markdown
-Version: 0.3.7
+Version: 0.3.8
 Summary: Export a JSON Schema document to Markdown documentation.
 Home-page: https://github.com/elisiariocouto/jsonschema-markdown
 License: MIT
 Keywords: jsonschema,markdown,documentation,docs,json
 Author: Elisiário Couto
 Author-email: elisiario@couto.io
 Requires-Python: >=3.9,<4.0
```


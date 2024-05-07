# Comparing `tmp/jsonschema_markdown-0.3.6.tar.gz` & `tmp/jsonschema_markdown-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_markdown-0.3.6.tar", max compression
+gzip compressed data, was "jsonschema_markdown-0.3.7.tar", max compression
```

## Comparing `jsonschema_markdown-0.3.6.tar` & `jsonschema_markdown-0.3.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/LICENSE
--rw-r--r--   0        0        0     3152 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/README.md
--rw-r--r--   0        0        0       81 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/converter/__init__.py
--rw-r--r--   0        0        0    15937 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/converter/markdown.py
--rw-r--r--   0        0        0     1606 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/main.py
--rw-r--r--   0        0        0     1103 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/jsonschema_markdown/utils.py
--rw-r--r--   0        0        0     1340 2024-04-16 00:37:34.794862 jsonschema_markdown-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 jsonschema_markdown-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/LICENSE
+-rw-r--r--   0        0        0     3152 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/README.md
+-rw-r--r--   0        0        0       81 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/converter/__init__.py
+-rw-r--r--   0        0        0    15971 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/converter/markdown.py
+-rw-r--r--   0        0        0     1606 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/main.py
+-rw-r--r--   0        0        0     1103 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/jsonschema_markdown/utils.py
+-rw-r--r--   0        0        0     1340 2024-05-07 22:46:38.578106 jsonschema_markdown-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 jsonschema_markdown-0.3.7/PKG-INFO
```

### Comparing `jsonschema_markdown-0.3.6/LICENSE` & `jsonschema_markdown-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.6/README.md` & `jsonschema_markdown-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.6/jsonschema_markdown/converter/markdown.py` & `jsonschema_markdown-0.3.7/jsonschema_markdown/converter/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,28 @@
     """
     Check if any item has a non-falsy (non-empty) value for this column.
     """
     return any(value for value in column_values)
 
 
 def _get_schema_header(
-    schema: dict, title_fallback: str, description_fallback: str, nested: bool = False
+    schema: dict, ref_key: str, description_fallback: str, nested: bool = False
 ) -> str:
     """
     Get the title and description of the schema.
 
     If nested, all headings are increased by one level.
     """
 
     prefix = "" if not nested else "#"
 
     md = ""
+    title = schema.get("title", ref_key) if not nested else ref_key
     # Add the title and description of the schema
-    md += f"{prefix}# {schema.get('title', title_fallback)}\n\n"
+    md += f"{prefix}# {title}\n\n"
     description = schema.get("description", description_fallback).strip(" \n")
     md += description if description else description_fallback
     md += "\n\n"
 
     # Add examples if present
     examples = schema.get("examples", [])
     if examples:
@@ -95,26 +96,26 @@
 
     defs = _schema.get("definitions", _schema.get("$defs", {}))
     markdown += _create_definition_table(
         _schema, defs, hide_empty_columns=hide_empty_columns
     )
 
     if defs:
-        markdown += "\n\n---\n\n# Definitions\n\n"
+        markdown += "\n---\n\n# Definitions\n\n"
         for key, definition in defs.items():
             markdown += _get_schema_header(
                 definition, key, "No description provided for this model.", nested=True
             )
             markdown += _create_definition_table(
                 definition, defs, hide_empty_columns=hide_empty_columns
             )
 
     if footer:
         # Add timestamp and a link to the project
-        markdown += "\n\n---\n\nMarkdown generated with [jsonschema-markdown](https://github.com/elisiariocouto/jsonschema-markdown)."
+        markdown += "\n---\n\nMarkdown generated with [jsonschema-markdown](https://github.com/elisiariocouto/jsonschema-markdown)."
 
     res = markdown.strip(" \n")
     res += "\n"
 
     return res
 
 
@@ -250,15 +251,15 @@
             "| " + " | ".join(["-" * len(col) for col in table_items[0]]) + " |\n"
         )
         # Generate the item rows
 
         for item in table_items:
             markdown += "| " + " | ".join(item.values()) + " |\n"
 
-    return markdown
+    return f"{markdown}\n"
 
 
 def _get_property_ref(ref, defs):
     ref = ref.split("/")[-1]
     if ref in defs:
         return (
             defs[ref].get("type", "Missing type"),
```

### Comparing `jsonschema_markdown-0.3.6/jsonschema_markdown/main.py` & `jsonschema_markdown-0.3.7/jsonschema_markdown/main.py`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.6/jsonschema_markdown/utils.py` & `jsonschema_markdown-0.3.7/jsonschema_markdown/utils.py`

 * *Files identical despite different names*

### Comparing `jsonschema_markdown-0.3.6/pyproject.toml` & `jsonschema_markdown-0.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "jsonschema-markdown"
 license = "MIT"
-version = "0.3.6"
+version = "0.3.7"
 description = "Export a JSON Schema document to Markdown documentation."
 authors = ["Elisiário Couto <elisiario@couto.io>"]
 repository = "https://github.com/elisiariocouto/jsonschema-markdown"
 readme = "README.md"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
@@ -22,18 +22,18 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.7"
 loguru = "^0.7.2"
 jsonref = "^1.1.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^24.2.0"
-ruff = "^0.3.0"
+black = "^24.4.2"
+ruff = "^0.4.3"
 pytest = "^8.0.0"
-pre-commit = "^3.6.1"
+pre-commit = "^3.7.0"
 pydantic = "^2.6.1"
 pytest-cov = "^5.0.0"
 
 [tool.poetry.scripts]
 jsonschema-markdown = "jsonschema_markdown.main:cli"
 
 [build-system]
```

### Comparing `jsonschema_markdown-0.3.6/PKG-INFO` & `jsonschema_markdown-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-markdown
-Version: 0.3.6
+Version: 0.3.7
 Summary: Export a JSON Schema document to Markdown documentation.
 Home-page: https://github.com/elisiariocouto/jsonschema-markdown
 License: MIT
 Keywords: jsonschema,markdown,documentation,docs,json
 Author: Elisiário Couto
 Author-email: elisiario@couto.io
 Requires-Python: >=3.9,<4.0
```


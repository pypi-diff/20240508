# Comparing `tmp/pydantic_glue-0.3.0.tar.gz` & `tmp/pydantic_glue-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_glue-0.3.0.tar", max compression
+gzip compressed data, was "pydantic_glue-0.4.0.tar", max compression
```

## Comparing `pydantic_glue-0.3.0.tar` & `pydantic_glue-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/LICENSE
--rw-r--r--   0        0        0     2574 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/README.md
--rw-r--r--   0        0        0       65 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/pydantic_glue/__init__.py
--rw-r--r--   0        0        0      771 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/pydantic_glue/cli.py
--rw-r--r--   0        0        0     1694 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/pydantic_glue/handler.py
--rw-r--r--   0        0        0     1591 2024-05-07 15:02:21.581716 pydantic_glue-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 pydantic_glue-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-08 19:23:29.934665 pydantic_glue-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2761 2024-05-08 19:23:29.934665 pydantic_glue-0.4.0/README.md
+-rw-r--r--   0        0        0       65 2024-05-08 19:23:29.934665 pydantic_glue-0.4.0/pydantic_glue/__init__.py
+-rw-r--r--   0        0        0     1674 2024-05-08 19:23:29.934665 pydantic_glue-0.4.0/pydantic_glue/cli.py
+-rw-r--r--   0        0        0     1694 2024-05-08 19:23:29.934665 pydantic_glue-0.4.0/pydantic_glue/handler.py
+-rw-r--r--   0        0        0     1591 2024-05-08 19:23:29.934665 pydantic_glue-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3736 1970-01-01 00:00:00.000000 pydantic_glue-0.4.0/PKG-INFO
```

### Comparing `pydantic_glue-0.3.0/LICENSE` & `pydantic_glue-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_glue-0.3.0/README.md` & `pydantic_glue-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -30,35 +30,38 @@
 This tool allows you to define a table in `pydantic`
 and generate a JSON with column types that can be used with `terraform` to create a Glue table.
 
 ## Example
 
 Take the following pydantic class
 
-```python
+```python title="example.py"
 from pydantic import BaseModel
 from typing import List
 
+
 class Bar(BaseModel):
     name: str
     age: int
 
+
 class Foo(BaseModel):
     nums: List[int]
     bars: List[Bar]
     other: str
+
 ```
 
 Running `pydantic-glue`
 
 ```bash
-pydantic-glue example.py Foo
+pydantic-glue -f example.py -c Foo
 ```
 
-you get this JSON
+you get this JSON in the terminal:
 
 ```json
 {
   "//": "Generated by pydantic-glue at 2022-05-25 12:35:55.333570. DO NOT EDIT",
   "columns": {
     "nums": "array<int>",
     "bars": "array<struct<name:string,age:int>>",
@@ -87,14 +90,20 @@
         type = columns.value
       }
     }
   }
 }
 ```
 
+Alternatively you can run CLI with `-o` flag to set output file location:
+
+```bash
+pydantic-glue -f example.py -c Foo -o example.json -l
+```
+
 ## How it works?
 
 * `pydantic` gets converted to JSON Schema
 * the JSON Schema types get mapped to Glue types recursively
 
 ## Future work
```

### Comparing `pydantic_glue-0.3.0/pydantic_glue/handler.py` & `pydantic_glue-0.4.0/pydantic_glue/handler.py`

 * *Files identical despite different names*

### Comparing `pydantic_glue-0.3.0/pyproject.toml` & `pydantic_glue-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pydantic-glue"
 keywords = ["pydantic", "glue", "athena", "types", "convert"]
-version = "0.3.0"
+version = "0.4.0"
 description = "Convert pydantic model to aws glue schema for terraform"
 authors = ["Serhii Dimchenko <svdimchenko@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/svdimchenko/pydantic-glue"
 
 [tool.poetry.urls]
```

### Comparing `pydantic_glue-0.3.0/PKG-INFO` & `pydantic_glue-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-glue
-Version: 0.3.0
+Version: 0.4.0
 Summary: Convert pydantic model to aws glue schema for terraform
 Home-page: https://github.com/svdimchenko/pydantic-glue
 License: MIT
 Keywords: pydantic,glue,athena,types,convert
 Author: Serhii Dimchenko
 Author-email: svdimchenko@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -53,35 +53,38 @@
 This tool allows you to define a table in `pydantic`
 and generate a JSON with column types that can be used with `terraform` to create a Glue table.
 
 ## Example
 
 Take the following pydantic class
 
-```python
+```python title="example.py"
 from pydantic import BaseModel
 from typing import List
 
+
 class Bar(BaseModel):
     name: str
     age: int
 
+
 class Foo(BaseModel):
     nums: List[int]
     bars: List[Bar]
     other: str
+
 ```
 
 Running `pydantic-glue`
 
 ```bash
-pydantic-glue example.py Foo
+pydantic-glue -f example.py -c Foo
 ```
 
-you get this JSON
+you get this JSON in the terminal:
 
 ```json
 {
   "//": "Generated by pydantic-glue at 2022-05-25 12:35:55.333570. DO NOT EDIT",
   "columns": {
     "nums": "array<int>",
     "bars": "array<struct<name:string,age:int>>",
@@ -110,14 +113,20 @@
         type = columns.value
       }
     }
   }
 }
 ```
 
+Alternatively you can run CLI with `-o` flag to set output file location:
+
+```bash
+pydantic-glue -f example.py -c Foo -o example.json -l
+```
+
 ## How it works?
 
 * `pydantic` gets converted to JSON Schema
 * the JSON Schema types get mapped to Glue types recursively
 
 ## Future work
```

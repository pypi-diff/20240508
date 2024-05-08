# Comparing `tmp/sqlfluff_common_conventions-0.2.0.tar.gz` & `tmp/sqlfluff_common_conventions-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff_common_conventions-0.2.0.tar", last modified: Mon Apr 29 08:12:52 2024, max compression
+gzip compressed data, was "sqlfluff_common_conventions-0.3.0.tar", last modified: Wed May  8 08:33:31 2024, max compression
```

## Comparing `sqlfluff_common_conventions-0.2.0.tar` & `sqlfluff_common_conventions-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-29 08:12:52.803366 sqlfluff_common_conventions-0.2.0/
--rw-r--r--   0 valerie.tan   (502) staff       (20)     1067 2024-04-08 03:18:16.000000 sqlfluff_common_conventions-0.2.0/LICENSE
--rw-r--r--   0 valerie.tan   (502) staff       (20)       65 2024-04-11 09:37:24.000000 sqlfluff_common_conventions-0.2.0/MANIFEST.in
--rw-r--r--   0 valerie.tan   (502) staff       (20)     3045 2024-04-29 08:12:52.802942 sqlfluff_common_conventions-0.2.0/PKG-INFO
--rw-r--r--   0 valerie.tan   (502) staff       (20)      543 2024-04-29 07:59:39.000000 sqlfluff_common_conventions-0.2.0/README.md
--rw-r--r--   0 valerie.tan   (502) staff       (20)     1506 2024-04-29 08:10:24.000000 sqlfluff_common_conventions-0.2.0/pyproject.toml
--rw-r--r--   0 valerie.tan   (502) staff       (20)       38 2024-04-29 08:12:52.803455 sqlfluff_common_conventions-0.2.0/setup.cfg
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-29 08:12:52.795451 sqlfluff_common_conventions-0.2.0/src/
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-29 08:12:52.799524 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/
--rw-r--r--   0 valerie.tan   (502) staff       (20)     3992 2024-04-29 08:05:02.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/CC01.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2557 2024-04-29 08:04:59.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/CC02.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     2319 2024-04-29 08:04:57.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/CC03.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     3410 2024-04-29 08:11:42.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/CC04.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     3304 2024-04-29 08:06:22.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/CC05.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)     1429 2024-04-29 07:42:00.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/__init__.py
--rw-r--r--   0 valerie.tan   (502) staff       (20)      244 2024-04-29 07:51:13.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/plugin_default_config.cfg
-drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-04-29 08:12:52.802499 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions.egg-info/
--rw-r--r--   0 valerie.tan   (502) staff       (20)     3045 2024-04-29 08:12:52.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions.egg-info/PKG-INFO
--rw-r--r--   0 valerie.tan   (502) staff       (20)      678 2024-04-29 08:12:52.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions.egg-info/SOURCES.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)        1 2024-04-29 08:12:52.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions.egg-info/dependency_links.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)       69 2024-04-29 08:12:52.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions.egg-info/entry_points.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)       16 2024-04-29 08:12:52.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions.egg-info/requires.txt
--rw-r--r--   0 valerie.tan   (502) staff       (20)       28 2024-04-29 08:12:52.000000 sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions.egg-info/top_level.txt
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-08 08:33:31.349658 sqlfluff_common_conventions-0.3.0/
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     1067 2024-04-08 03:18:16.000000 sqlfluff_common_conventions-0.3.0/LICENSE
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       65 2024-04-11 09:37:24.000000 sqlfluff_common_conventions-0.3.0/MANIFEST.in
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     3150 2024-05-08 08:33:31.349240 sqlfluff_common_conventions-0.3.0/PKG-INFO
+-rw-r--r--   0 valerie.tan   (502) staff       (20)      618 2024-05-08 08:31:04.000000 sqlfluff_common_conventions-0.3.0/README.md
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     1539 2024-05-08 08:33:02.000000 sqlfluff_common_conventions-0.3.0/pyproject.toml
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       38 2024-05-08 08:33:31.349873 sqlfluff_common_conventions-0.3.0/setup.cfg
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-08 08:33:31.334250 sqlfluff_common_conventions-0.3.0/src/
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-08 08:33:31.344847 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     4134 2024-05-02 09:19:06.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC01.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2699 2024-05-02 09:19:06.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC02.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2461 2024-05-02 09:19:06.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC03.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     6311 2024-05-08 02:20:21.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC04.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     6476 2024-05-08 02:11:13.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC05.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2634 2024-05-08 02:51:17.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC06.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     2613 2024-05-08 02:34:03.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/__init__.py
+-rw-r--r--   0 valerie.tan   (502) staff       (20)      470 2024-05-08 02:23:29.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/plugin_default_config.cfg
+drwxr-xr-x   0 valerie.tan   (502) staff       (20)        0 2024-05-08 08:33:31.348740 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/
+-rw-r--r--   0 valerie.tan   (502) staff       (20)     3150 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/PKG-INFO
+-rw-r--r--   0 valerie.tan   (502) staff       (20)      718 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/SOURCES.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)        1 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/dependency_links.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       69 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/entry_points.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       16 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/requires.txt
+-rw-r--r--   0 valerie.tan   (502) staff       (20)       28 2024-05-08 08:33:31.000000 sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/top_level.txt
```

### Comparing `sqlfluff_common_conventions-0.2.0/LICENSE` & `sqlfluff_common_conventions-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlfluff_common_conventions-0.2.0/PKG-INFO` & `sqlfluff_common_conventions-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlfluff_common_conventions
-Version: 0.2.0
-Summary: A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL.
+Version: 0.3.0
+Summary: A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL and Databricks SQL.
 Author-email: Valerie Tan <valerietanhx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Valerie Tan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Keywords: sqlfluff,sql,linter,formatter,bigquery
+Keywords: sqlfluff,sql,linter,formatter,bigquery,databricks
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -46,18 +46,19 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlfluff>=0.4.0
 
 # sqlfluff-common-conventions
 
-A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL.
+A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL and Databricks SQL.
 
 ## Rules
 
-As of 25 April 2024, all rules are compatible with snake, dromedary, and pascal case.
+As of 8 May 2024, all rules are compatible with snake, dromedary, and pascal case.
 
 - CC01: Start boolean columns with `is` or `has`.
 - CC02: End datetime, time, and timestamp columns with `at`.
 - CC03: End date columns with `date`.
 - CC04: Only allow a list of configurable strings to be used in identifiers.
 - CC05: Block a list of configurable strings from being used in identifiers.
+- CC06: Ensure column and table names match a given regex.
```

### Comparing `sqlfluff_common_conventions-0.2.0/README.md` & `sqlfluff_common_conventions-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # sqlfluff-common-conventions
 
-A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL.
+A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL and Databricks SQL.
 
 ## Rules
 
-As of 25 April 2024, all rules are compatible with snake, dromedary, and pascal case.
+As of 8 May 2024, all rules are compatible with snake, dromedary, and pascal case.
 
 - CC01: Start boolean columns with `is` or `has`.
 - CC02: End datetime, time, and timestamp columns with `at`.
 - CC03: End date columns with `date`.
 - CC04: Only allow a list of configurable strings to be used in identifiers.
-- CC05: Block a list of configurable strings from being used in identifiers.
+- CC05: Block a list of configurable strings from being used in identifiers.
+- CC06: Ensure column and table names match a given regex.
```

### Comparing `sqlfluff_common_conventions-0.2.0/pyproject.toml` & `sqlfluff_common_conventions-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlfluff_common_conventions"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Valerie Tan", email="valerietanhx@gmail.com" },
 ]
-description = "A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL."
+description = "A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL and Databricks SQL."
 readme = "README.md"
 license = {file = "LICENSE"}
-keywords = ["sqlfluff", "sql", "linter", "formatter", "bigquery"]
+keywords = ["sqlfluff", "sql", "linter", "formatter", "bigquery", "databricks"]
 requires-python = ">=3.8"
 dependencies = [
   'sqlfluff>=0.4.0'
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Development Status :: 3 - Alpha",
```

### Comparing `sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/CC01.py` & `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC01.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,20 @@
                 return None
 
             identifier = alias_expression.get_child("identifier").raw
             datatype = function.get_child("bracketed").get_child("data_type").raw
         else:  # column_definition
             assert segment.is_type("column_definition")
             identifier = segment.get_child("identifier").raw
-            datatype = segment.get_child("data_type").raw
+            datatype = segment.get_child("data_type")
+
+            if not datatype:  # account for views, which are parsed like tables
+                return None
+
+            datatype = datatype.raw
 
         if datatype.upper() in ["BOOL", "BOOLEAN"]:
             if self.naming_case == "snake" and not (
                 identifier.startswith("is_") or identifier.startswith("has_")
             ):
                 return LintResult(
                     anchor=context.segment,
```

### Comparing `sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/CC02.py` & `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC02.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,20 @@
                 return None
 
             identifier = alias_expression.get_child("identifier").raw
             datatype = function.get_child("bracketed").get_child("data_type").raw
         else:  # column_definition
             assert segment.is_type("column_definition")
             identifier = segment.get_child("identifier").raw
-            datatype = segment.get_child("data_type").raw
+            datatype = segment.get_child("data_type")
+
+            if not datatype:  # account for views, which are parsed like tables
+                return None
+
+            datatype = datatype.raw
 
         if datatype.upper() in ["DATETIME", "TIME", "TIMESTAMP"]:
             if self.naming_case == "snake" and not (identifier.endswith("_at")):
                 return LintResult(
                     anchor=context.segment,
                     description="Datetime, time, or timestamp column does not end with `_at`.",
                 )
```

### Comparing `sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions/CC03.py` & `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions/CC03.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,20 @@
                 return None
 
             identifier = alias_expression.get_child("identifier").raw
             datatype = function.get_child("bracketed").get_child("data_type").raw
         else:  # column_definition
             assert segment.is_type("column_definition")
             identifier = segment.get_child("identifier").raw
-            datatype = segment.get_child("data_type").raw
+            datatype = segment.get_child("data_type")
+
+            if not datatype:  # account for views, which are parsed like tables
+                return None
+
+            datatype = datatype.raw
 
         if datatype.upper() == "DATE":
             if self.naming_case == "snake" and not (identifier.endswith("_date")):
                 return LintResult(
                     anchor=context.segment,
                     description="Date column does not end with `_date`.",
                 )
```

### Comparing `sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions.egg-info/PKG-INFO` & `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlfluff_common_conventions
-Version: 0.2.0
-Summary: A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL.
+Version: 0.3.0
+Summary: A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL and Databricks SQL.
 Author-email: Valerie Tan <valerietanhx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Valerie Tan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Keywords: sqlfluff,sql,linter,formatter,bigquery
+Keywords: sqlfluff,sql,linter,formatter,bigquery,databricks
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -46,18 +46,19 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlfluff>=0.4.0
 
 # sqlfluff-common-conventions
 
-A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL.
+A plugin for rules that enforce common SQL conventions not available in SQLFluff, compatible with BigQuery SQL and Databricks SQL.
 
 ## Rules
 
-As of 25 April 2024, all rules are compatible with snake, dromedary, and pascal case.
+As of 8 May 2024, all rules are compatible with snake, dromedary, and pascal case.
 
 - CC01: Start boolean columns with `is` or `has`.
 - CC02: End datetime, time, and timestamp columns with `at`.
 - CC03: End date columns with `date`.
 - CC04: Only allow a list of configurable strings to be used in identifiers.
 - CC05: Block a list of configurable strings from being used in identifiers.
+- CC06: Ensure column and table names match a given regex.
```

### Comparing `sqlfluff_common_conventions-0.2.0/src/sqlfluff_common_conventions.egg-info/SOURCES.txt` & `sqlfluff_common_conventions-0.3.0/src/sqlfluff_common_conventions.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 src/sqlfluff_common_conventions/CC01.py
 src/sqlfluff_common_conventions/CC02.py
 src/sqlfluff_common_conventions/CC03.py
 src/sqlfluff_common_conventions/CC04.py
 src/sqlfluff_common_conventions/CC05.py
+src/sqlfluff_common_conventions/CC06.py
 src/sqlfluff_common_conventions/__init__.py
 src/sqlfluff_common_conventions/plugin_default_config.cfg
 src/sqlfluff_common_conventions.egg-info/PKG-INFO
 src/sqlfluff_common_conventions.egg-info/SOURCES.txt
 src/sqlfluff_common_conventions.egg-info/dependency_links.txt
 src/sqlfluff_common_conventions.egg-info/entry_points.txt
 src/sqlfluff_common_conventions.egg-info/requires.txt
```


# Comparing `tmp/fakesnow-0.9.8.tar.gz` & `tmp/fakesnow-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakesnow-0.9.8.tar", last modified: Fri Apr 19 06:37:41 2024, max compression
+gzip compressed data, was "fakesnow-0.9.9.tar", last modified: Wed May  1 12:15:14 2024, max compression
```

## Comparing `fakesnow-0.9.8.tar` & `fakesnow-0.9.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:37:41.287021 fakesnow-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-19 06:37:31.000000 fakesnow-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-19 06:37:41.287021 fakesnow-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-19 06:37:31.000000 fakesnow-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:37:41.279021 fakesnow-0.9.8/fakesnow/
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    29442 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/global_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/info_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    49714 2024-04-19 06:37:31.000000 fakesnow-0.9.8/fakesnow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:37:41.283021 fakesnow-0.9.8/fakesnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-19 06:37:41.000000 fakesnow-0.9.8/fakesnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-19 06:37:31.000000 fakesnow-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:37:41.287021 fakesnow-0.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:37:41.283021 fakesnow-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    67797 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_info_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    33081 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-19 06:37:31.000000 fakesnow-0.9.8/tests/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:15:14.286570 fakesnow-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-01 12:15:04.000000 fakesnow-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17846 2024-05-01 12:15:14.286570 fakesnow-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-01 12:15:04.000000 fakesnow-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:15:14.282570 fakesnow-0.9.9/fakesnow/
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29442 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/global_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    50059 2024-05-01 12:15:04.000000 fakesnow-0.9.9/fakesnow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:15:14.286570 fakesnow-0.9.9/fakesnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17846 2024-05-01 12:15:14.000000 fakesnow-0.9.9/fakesnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-01 12:15:14.000000 fakesnow-0.9.9/fakesnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:15:14.000000 fakesnow-0.9.9/fakesnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-01 12:15:14.000000 fakesnow-0.9.9/fakesnow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-01 12:15:14.000000 fakesnow-0.9.9/fakesnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 12:15:14.000000 fakesnow-0.9.9/fakesnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-01 12:15:04.000000 fakesnow-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:15:14.286570 fakesnow-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:15:14.282570 fakesnow-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-01 12:15:04.000000 fakesnow-0.9.9/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-01 12:15:04.000000 fakesnow-0.9.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 12:15:04.000000 fakesnow-0.9.9/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68082 2024-05-01 12:15:04.000000 fakesnow-0.9.9/tests/test_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-01 12:15:04.000000 fakesnow-0.9.9/tests/test_info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-01 12:15:04.000000 fakesnow-0.9.9/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-01 12:15:04.000000 fakesnow-0.9.9/tests/test_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33968 2024-05-01 12:15:04.000000 fakesnow-0.9.9/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-01 12:15:04.000000 fakesnow-0.9.9/tests/test_users.py
```

### Comparing `fakesnow-0.9.8/LICENSE` & `fakesnow-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/PKG-INFO` & `fakesnow-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.9.8
+Version: 0.9.9
 Summary: Fake Snowflake Connector for Python. Run, mock and test Snowflake DB locally.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -209,15 +209,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: duckdb~=0.10.0
 Requires-Dist: pyarrow
 Requires-Dist: snowflake-connector-python
-Requires-Dist: sqlglot~=23.3.0
+Requires-Dist: sqlglot~=23.12.2
 Provides-Extra: dev
 Requires-Dist: build~=1.0; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: snowflake-connector-python[pandas,secure-local-storage]; extra == "dev"
 Requires-Dist: pre-commit~=3.4; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: ruff~=0.3.2; extra == "dev"
```

### Comparing `fakesnow-0.9.8/README.md` & `fakesnow-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/fakesnow/__init__.py` & `fakesnow-0.9.9/fakesnow/__init__.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/fakesnow/checks.py` & `fakesnow-0.9.9/fakesnow/checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/fakesnow/cli.py` & `fakesnow-0.9.9/fakesnow/cli.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/fakesnow/expr.py` & `fakesnow-0.9.9/fakesnow/expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/fakesnow/fakes.py` & `fakesnow-0.9.9/fakesnow/fakes.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/fakesnow/global_database.py` & `fakesnow-0.9.9/fakesnow/global_database.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/fakesnow/info_schema.py` & `fakesnow-0.9.9/fakesnow/info_schema.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/fakesnow/transforms.py` & `fakesnow-0.9.9/fakesnow/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
     """
 
     if isinstance(expression, exp.Create) and (table := expression.find(exp.Table)):
         comment = None
         if props := cast(exp.Properties, expression.args.get("properties")):
             other_props = []
             for p in props.expressions:
-                if isinstance(p, exp.SchemaCommentProperty) and (isinstance(p.this, (exp.Literal, exp.Identifier))):
+                if isinstance(p, exp.SchemaCommentProperty) and (isinstance(p.this, (exp.Literal, exp.Var))):
                     comment = p.this.this
                 else:
                     other_props.append(p)
 
             new = expression.copy()
             new_props: exp.Properties = new.args["properties"]
             new_props.set("expressions", other_props)
@@ -356,18 +356,27 @@
 
     Returns:
         exp.Expression: The original expression, with any text lengths stored in the new 'text_lengths' arg.
     """
 
     if isinstance(expression, (exp.Create, exp.AlterTable)):
         text_lengths = []
-        for dt in expression.find_all(exp.DataType):
-            if dt.this in (exp.DataType.Type.VARCHAR, exp.DataType.Type.TEXT):
-                col_name = dt.parent and dt.parent.this and dt.parent.this.this
-                if dt_size := dt.find(exp.DataTypeParam):
+
+        # exp.Select is for a ctas, exp.Schema is a plain definition
+        if cols := expression.find(exp.Select, exp.Schema):
+            expressions = cols.expressions
+        else:
+            # alter table
+            expressions = expression.args.get("actions") or []
+        for e in expressions:
+            if dts := [
+                dt for dt in e.find_all(exp.DataType) if dt.this in (exp.DataType.Type.VARCHAR, exp.DataType.Type.TEXT)
+            ]:
+                col_name = e.alias if isinstance(e, exp.Alias) else e.name
+                if len(dts) == 1 and (dt_size := dts[0].find(exp.DataTypeParam)):
                     size = (
                         isinstance(dt_size.this, exp.Literal)
                         and isinstance(dt_size.this.this, str)
                         and int(dt_size.this.this)
                     )
                 else:
                     size = 16777216
```

### Comparing `fakesnow-0.9.8/fakesnow.egg-info/PKG-INFO` & `fakesnow-0.9.9/fakesnow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.9.8
+Version: 0.9.9
 Summary: Fake Snowflake Connector for Python. Run, mock and test Snowflake DB locally.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -209,15 +209,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: duckdb~=0.10.0
 Requires-Dist: pyarrow
 Requires-Dist: snowflake-connector-python
-Requires-Dist: sqlglot~=23.3.0
+Requires-Dist: sqlglot~=23.12.2
 Provides-Extra: dev
 Requires-Dist: build~=1.0; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: snowflake-connector-python[pandas,secure-local-storage]; extra == "dev"
 Requires-Dist: pre-commit~=3.4; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: ruff~=0.3.2; extra == "dev"
```

### Comparing `fakesnow-0.9.8/fakesnow.egg-info/SOURCES.txt` & `fakesnow-0.9.9/fakesnow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/pyproject.toml` & `fakesnow-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "fakesnow"
 description = "Fake Snowflake Connector for Python. Run, mock and test Snowflake DB locally."
-version = "0.9.8"
+version = "0.9.9"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 keywords = ["snowflake", "snowflakedb", "fake", "local", "mock", "testing"]
 requires-python = ">=3.9"
 dependencies = [
     "duckdb~=0.10.0",
     "pyarrow",
     "snowflake-connector-python",
-    "sqlglot~=23.3.0",
+    "sqlglot~=23.12.2",
 ]
 
 [project.urls]
 homepage = "https://github.com/tekumara/fakesnow"
 
 [project.scripts]
 fakesnow = "fakesnow.cli:main"
```

### Comparing `fakesnow-0.9.8/tests/test_checks.py` & `fakesnow-0.9.9/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/tests/test_cli.py` & `fakesnow-0.9.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/tests/test_expr.py` & `fakesnow-0.9.9/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/tests/test_fakes.py` & `fakesnow-0.9.9/tests/test_fakes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1280,14 +1280,21 @@
 
     # Assertion to sanity check that the above "in schema" filter isn't wrong, and in fact filters
     dcur.execute("show primary keys in schema db1.information_schema")
     result3 = dcur.fetchall()
     assert result3 == []
 
 
+def test_sqlglot_regression(cur: snowflake.connector.cursor.SnowflakeCursor):
+    assert cur.execute(
+        """with SOURCE_TABLE AS (SELECT '2024-01-01' AS start_date)
+            SELECT date(a.start_date) from SOURCE_TABLE AS a"""
+    ).fetchone() == (datetime.date(2024, 1, 1),)
+
+
 def test_sqlstate(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("select 'hello world'")
     # sqlstate is None on success
     assert cur.sqlstate is None
 
     with pytest.raises(snowflake.connector.errors.ProgrammingError) as _:
         cur.execute("select * from this_table_does_not_exist")
```

### Comparing `fakesnow-0.9.8/tests/test_info_schema.py` & `fakesnow-0.9.9/tests/test_info_schema.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/tests/test_patch.py` & `fakesnow-0.9.9/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/tests/test_sqlalchemy.py` & `fakesnow-0.9.9/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.8/tests/test_transforms.py` & `fakesnow-0.9.9/tests/test_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,14 +331,33 @@
 
 def test_extract_text_length() -> None:
     sql = "CREATE TABLE table1 (t1 VARCHAR, t2 VARCHAR(10), t3 TEXT(20), i1 BIGINT)"
     e = sqlglot.parse_one(sql).transform(extract_text_length)
     assert e.sql() == sql
     assert e.args["text_lengths"] == [("t1", 16777216), ("t2", 10), ("t3", 20)]
 
+    sql = "ALTER TABLE t1 ALTER COLUMN c4 SET DATA TYPE VARCHAR(50)"
+    e = sqlglot.parse_one(sql).transform(extract_text_length)
+    assert e.sql() == sql
+    assert e.args["text_lengths"] == [("c4", 50)]
+
+    # test column name is correct with alias
+    sql = """CREATE TABLE table1 AS (
+                SELECT CAST(C1 AS TEXT) AS K, CAST(C2 AS TEXT(10)) AS V
+                FROM (VALUES (1, 2)) AS T(C1, C2))"""
+    e = sqlglot.parse_one(sql).transform(extract_text_length)
+    assert e.args["text_lengths"] == [("K", 16777216), ("V", 10)]
+
+    # test ctas column name is correct for combined field
+    sql = """CREATE TABLE SOME_TABLE AS (
+                SELECT CAST(C1 AS TEXT) || '-' || CAST(C1 AS TEXT) AS K
+                FROM VALUES (1), (2) AS T (C1))"""
+    e = sqlglot.parse_one(sql).transform(extract_text_length)
+    assert e.args["text_lengths"] == [("K", 16777216)]
+
 
 def test_flatten() -> None:
     assert (
         sqlglot.parse_one(
             """
             select t.id, flat.value:fruit from
             (
```

### Comparing `fakesnow-0.9.8/tests/test_users.py` & `fakesnow-0.9.9/tests/test_users.py`

 * *Files identical despite different names*


# Comparing `tmp/databricks_labs_lsql-0.4.2.tar.gz` & `tmp/databricks_labs_lsql-0.4.3.tar.gz`

## Comparing `databricks_labs_lsql-0.4.2.tar` & `databricks_labs_lsql-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/__about__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/__main__.py
--rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/backends.py
--rw-r--r--   0        0        0    23725 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/core.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/deployment.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/databricks/labs/lsql/py.typed
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/LICENSE
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/NOTICE
--rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/README.md
--rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/databricks/labs/lsql/__about__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/databricks/labs/lsql/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/databricks/labs/lsql/__main__.py
+-rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/databricks/labs/lsql/backends.py
+-rw-r--r--   0        0        0    23851 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/databricks/labs/lsql/core.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/databricks/labs/lsql/deployment.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/databricks/labs/lsql/py.typed
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/NOTICE
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/README.md
+-rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 databricks_labs_lsql-0.4.3/PKG-INFO
```

### Comparing `databricks_labs_lsql-0.4.2/databricks/labs/lsql/backends.py` & `databricks_labs_lsql-0.4.3/databricks/labs/lsql/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
     def fetch(self, sql: str, *, catalog: str | None = None, schema: str | None = None) -> Iterator[Row]:
         logger.debug(f"[spark][fetch] {self._only_n_bytes(sql, self._debug_truncate_bytes)}")
         try:
             if catalog:
                 self._spark.sql(f"USE CATALOG {catalog}")
             if schema:
                 self._spark.sql(f"USE SCHEMA {schema}")
+            # TODO: pyspark.sql.Row is being returned instead of databricks.labs.lsql.core.Row
             return iter(self._spark.sql(sql).collect())
         except Exception as e:
             error_message = str(e)
             raise self._api_error_from_message(error_message) from None
 
     def save_table(self, full_name: str, rows: Sequence[DataclassInstance], klass: Dataclass, mode: str = "append"):
         rows = self._filter_none_rows(rows, klass)
```

### Comparing `databricks_labs_lsql-0.4.2/databricks/labs/lsql/core.py` & `databricks_labs_lsql-0.4.3/databricks/labs/lsql/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,18 @@
         """Create a new Row class with the given column names."""
         return type("Row", (Row,), {"__columns__": col_names})
 
     def as_dict(self) -> dict[str, Any]:
         """Convert the row to a dictionary with the same conventions as Databricks SDK."""
         return dict(zip(self.__columns__, self, strict=True))
 
+    # PySpark's compatibility
+    def asDict(self, recursive: bool = False) -> dict[str, Any]:
+        return self.as_dict()
+
     def __eq__(self, other):
         """Check if the rows are equal."""
         if not isinstance(other, Row):
             return False
         # compare rows as dictionaries, because the order
         # of fields in constructor is not guaranteed
         return self.as_dict() == other.as_dict()
```

### Comparing `databricks_labs_lsql-0.4.2/databricks/labs/lsql/deployment.py` & `databricks_labs_lsql-0.4.3/databricks/labs/lsql/deployment.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.2/.gitignore` & `databricks_labs_lsql-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.2/LICENSE` & `databricks_labs_lsql-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.2/NOTICE` & `databricks_labs_lsql-0.4.3/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.2/README.md` & `databricks_labs_lsql-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.2/pyproject.toml` & `databricks_labs_lsql-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_lsql-0.4.2/PKG-INFO` & `databricks_labs_lsql-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-lsql
-Version: 0.4.2
+Version: 0.4.3
 Summary: Lightweight stateless SQL execution for Databricks with minimal dependencies
 Project-URL: Documentation, https://github.com/databrickslabs/lsql#readme
 Project-URL: Issues, https://github.com/databrickslabs/lsql/issues
 Project-URL: Source, https://github.com/databrickslabs/lsql
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
```


# Comparing `tmp/pd_extras-6.0.4.tar.gz` & `tmp/pd_extras-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pd_extras-6.0.4.tar", max compression
+gzip compressed data, was "pd_extras-6.1.0.tar", max compression
```

## Comparing `pd_extras-6.0.4.tar` & `pd_extras-6.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1069 2024-05-06 13:55:39.269733 pd_extras-6.0.4/LICENSE
--rw-r--r--   0        0        0     2912 2024-05-06 13:55:39.269733 pd_extras-6.0.4/README.md
--rw-r--r--   0        0        0        0 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/check/__init__.py
--rw-r--r--   0        0        0     3245 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/check/sanitize.py
--rw-r--r--   0        0        0        0 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/extra/__init__.py
--rw-r--r--   0        0        0     3794 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/extra/flattener.py
--rw-r--r--   0        0        0     2635 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/extra/operations.py
--rw-r--r--   0        0        0        0 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/optimize/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/optimize/df_ops.py
--rw-r--r--   0        0        0        0 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/write/__init__.py
--rw-r--r--   0        0        0     1388 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/write/common.py
--rw-r--r--   0        0        0     5670 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/write/nosql_writer.py
--rw-r--r--   0        0        0     8955 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pd_extras/write/sql_writer.py
--rw-r--r--   0        0        0      729 2024-05-06 13:55:39.273733 pd_extras-6.0.4/pyproject.toml
--rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 pd_extras-6.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-08 01:34:38.591303 pd_extras-6.1.0/LICENSE
+-rw-r--r--   0        0        0     2912 2024-05-08 01:34:38.591303 pd_extras-6.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/check/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/check/sanitize.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/extra/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/extra/flattener.py
+-rw-r--r--   0        0        0     2635 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/extra/operations.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/optimize/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/optimize/df_ops.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/__init__.py
+-rw-r--r--   0        0        0     1503 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/common.py
+-rw-r--r--   0        0        0      192 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/driver.py
+-rw-r--r--   0        0        0     5670 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/nosql_writer.py
+-rw-r--r--   0        0        0     8787 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/sql_writer.py
+-rw-r--r--   0        0        0      729 2024-05-08 01:34:38.595303 pd_extras-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 pd_extras-6.1.0/PKG-INFO
```

### Comparing `pd_extras-6.0.4/LICENSE` & `pd_extras-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.4/README.md` & `pd_extras-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.4/pd_extras/check/sanitize.py` & `pd_extras-6.1.0/pd_extras/check/sanitize.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.4/pd_extras/extra/flattener.py` & `pd_extras-6.1.0/pd_extras/extra/flattener.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.4/pd_extras/extra/operations.py` & `pd_extras-6.1.0/pd_extras/extra/operations.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.4/pd_extras/optimize/df_ops.py` & `pd_extras-6.1.0/pd_extras/optimize/df_ops.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.4/pd_extras/write/common.py` & `pd_extras-6.1.0/pd_extras/write/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """Common variables for dataframe to database module"""
 
-saved_values = {
-    "sqlserver": {
+from pd_extras.write.driver import SQLDatabaseType
+
+META_INFO_QUERIES = {
+    SQLDatabaseType.SQLSERVER.value: {
         "dialect": "mssql",
         "driver": "+pymssql",
         "query": {
             "db_list": "SELECT name FROM master.sys.databases;",
             "table_list": """SELECT TABLE_NAME FROM
                 INFORMATION_SCHEMA.TABLES WHERE TABLE_TYPE = 'BASE TABLE' AND
                 TABLE_CATALOG=%s;""",
             "column_info": """SELECT * FROM
                 information_schema.columns WHERE TABLE_CATALOG='%s' AND
                 TABLE_SCHEMA = 'dbo' AND TABLE_NAME = '%s';""",
         },
     },
-    "mysql": {
+    SQLDatabaseType.MYSQL.value: {
         "dialect": "mysql",
         "driver": "+mysqldb",
         "query": {
             "db_list": "SHOW DATABASES;",
             "table_list": """SHOW TABLES FROM %s""",
             "column_info": """SELECT *
                 from information_schema.columns
                 WHERE table_schema='%s' and table_name='%s';""",
         },
     },
-    "postgresql": {
+    SQLDatabaseType.POSTGRES.value: {
         "dialect": "postgresql",
         "driver": "+psycopg2",
         "query": {
             "db_list": "select datname from pg_database;",
             "table_list": "select * from pg_catalog.pg_tables where schemaname=%s;",
             "column_info": """select * from information_schema.columns WHERE
                 table_catalog='%s' and table_name='%s';""",
```

### Comparing `pd_extras-6.0.4/pd_extras/write/nosql_writer.py` & `pd_extras-6.1.0/pd_extras/write/nosql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.4/pd_extras/write/sql_writer.py` & `pd_extras-6.1.0/pd_extras/write/sql_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,58 +11,56 @@
     Table,
     create_engine,
     text,
 )
 from sqlalchemy.orm import Session
 from sqlalchemy_utils import create_database, database_exists
 
-from pd_extras.write.common import saved_values
+from pd_extras.write.common import META_INFO_QUERIES
+from pd_extras.write.driver import SQLDatabaseType
 
 
 class SQLDatabaseWriter:
     """Database connection object for SQL databases
     Only database name `dbname` is stored.
     Rest of the credentials are used only to retrieved the connection.
     Two connections are created: one for the specific database `dbname`
     and another generic connection with no database selected.
     Be sure to call `connobj.close_connection()` after you are done.
     """
 
     def __init__(
         self,
-        dbtype: str,
+        dbtype: SQLDatabaseType,
         host: str,
         dbname: str,
         user: str,
         password: str,
         port: int,
     ):
-        if dbtype not in saved_values:
-            raise KeyError(f"{dbtype} not in {list(saved_values.keys())}")
-
-        if not dbname:
+        if not dbname or len(dbname) < 1:
             raise ValueError("`dbname` must be a valid database name")
 
-        self.__dbtype = dbtype
+        self.__dbtype = dbtype.value
         self.__dbname = dbname
         port = int(port)
 
         self.__engine = self._get_db_specific_engine(
             host=host,
             user=user,
             password=password,
             port=port,
         )
 
         if not database_exists(url=self.__engine.url):
             create_database(self.__engine.url)
 
     def _get_db_specific_engine(self, host: str, user: str, password: str, port: int):
-        dialect = saved_values[self.__dbtype]["dialect"]
-        driver = saved_values[self.__dbtype]["driver"]
+        dialect = META_INFO_QUERIES[self.__dbtype]["dialect"]
+        driver = META_INFO_QUERIES[self.__dbtype]["driver"]
 
         connection_string = (
             f"{dialect}{driver}://{user}:{password}@{host}:{port}/{self.__dbname}"
         )
 
         engine = create_engine(connection_string, future=True)
 
@@ -74,32 +72,32 @@
         :param table_name: Name of the table in database.
         :type table_name: ``str``
         :return: Pandas dataframe of table schema information.
         :rtype: ``pd.DataFrame``
         """
 
         sa_session = Session(self.__engine)
-        _saved_values: dict = saved_values[self.__dbtype]
+        _saved_values: dict = META_INFO_QUERIES[self.__dbtype]
 
         self._check_name(name=self.__dbname)
         self._check_name(name=table_name)
 
         query: str = _saved_values["query"]["column_info"] % (
             self.__dbname,
             table_name,
         )
         session = sa_session.execute(text(query))
-        cursor = session.cursor  # type: ignore
+        cursor = session.cursor
         cols = [detail[0] for detail in cursor.description]
         res = cursor.fetchall()
         res = [list(row) for row in res]
 
         info = pd.DataFrame(res, columns=cols)
         columns: list = [str(column.lower()) for column in info.columns.tolist()]
-        info.columns = columns  # type: ignore
+        info.columns = columns
 
         session.close()
 
         return info
 
     def has_table(self, table_name: str):
         """Check if the current database has table `table_name`.
@@ -124,16 +122,14 @@
         columns = info["column_name"].to_numpy()
         nullable_status = info["is_nullable"].to_numpy()
 
         columns_valid = []
         for column, status in zip(columns, nullable_status):
             if id_col == column:
                 continue
-            if column not in data.columns:
-                raise ValueError(f"{column} not in columns: {data.columns.tolist()}")
 
             if status.lower() == "no":
                 if data[column].dropna().shape[0] < data.shape[0]:
                     raise ValueError(f"`{column}` is non-nullable but has null value")
             columns_valid.append(column)
 
         data = data[columns_valid].copy()
```

### Comparing `pd_extras-6.0.4/pyproject.toml` & `pd_extras-6.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pd-extras"
-version = "6.0.4"
+version = "6.1.0"
 description = "Some utility functions on top of pandas."
 authors = ["Masum Billal <billalmasum93@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/proafxin/pd-extras"
 documentation = "https://pd-extras.readthedocs.io/en/latest/"
```

### Comparing `pd_extras-6.0.4/PKG-INFO` & `pd_extras-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pd-extras
-Version: 6.0.4
+Version: 6.1.0
 Summary: Some utility functions on top of pandas.
 Home-page: https://github.com/proafxin/pd-extras
 License: MIT
 Author: Masum Billal
 Author-email: billalmasum93@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


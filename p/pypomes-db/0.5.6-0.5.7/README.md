# Comparing `tmp/pypomes_db-0.5.6.tar.gz` & `tmp/pypomes_db-0.5.7.tar.gz`

## Comparing `pypomes_db-0.5.6.tar` & `pypomes_db-0.5.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38002 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    24057 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    21898 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    21948 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38128 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    24356 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    22234 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    22282 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.7/PKG-INFO
```

### Comparing `pypomes_db-0.5.6/src/pypomes_db/__init__.py` & `pypomes_db-0.5.7/src/pypomes_db/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .db_pomes import (
     db_setup, db_get_engines, db_get_params,
     db_assert_connection, db_connect, db_exists,
     db_select_one, db_select_all, db_update,
     db_delete, db_insert, db_bulk_insert, db_bulk_copy,
-    db_copy_lobs, db_update_lob, db_execute,
+    db_migrate_lobs, db_update_lob, db_execute,
     db_call_function, db_call_procedure,
 )
 
 __all__ = [
     # db_pomes
     "db_setup", "db_get_engines", "db_get_params",
     "db_assert_connection", "db_connect", "db_exists",
     "db_select_one", "db_select_all", "db_update",
     "db_delete", "db_insert", "db_bulk_insert", "db_bulk_copy",
-    "db_copy_lobs", "db_update_lob", "db_execute",
+    "db_migrate_lobs", "db_update_lob", "db_execute",
     "db_call_function", "db_call_procedure",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_db")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_db-0.5.6/src/pypomes_db/db_common.py` & `pypomes_db-0.5.7/src/pypomes_db/db_common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from logging import Logger
+from logging import DEBUG, Logger
 from pypomes_core import (
     APP_PREFIX,
     env_get_int, env_get_str, str_sanitize, str_get_positional
 )
 
 # the preferred way to specify database connection parameters is dynamically with 'db_setup_params'
 # specifying database connection parameters with environment variables can be done in two ways:
@@ -173,40 +173,41 @@
 
     :param query_stmt: the query command
     :param bind_vals: values associated with the query command
     :return: message indicative of empty search
     """
     result: str = str_sanitize(query_stmt)
 
-    if bind_vals:
-        for val in bind_vals:
-            if isinstance(val, str):
-                sval: str = f"'{val}'"
-            else:
-                sval: str = str(val)
-            result = result.replace("?", sval, 1)
+    for val in bind_vals or []:
+        if isinstance(val, str):
+            sval: str = f"'{val}'"
+        else:
+            sval: str = str(val)
+        result = result.replace("?", sval, 1)
 
     return result
 
 
-def _db_log(errors: list[str],
+def _db_log(logger: Logger,
             err_msg: str,
-            logger: Logger,
-            query_stmt: str,
+            level: int = DEBUG,
+            errors: list[str] = None,
+            query_stmt: str = None,
             bind_vals: tuple = None) -> None:
     """
     Log *err_msg* and add it to *errors*, or else log the executed query, whichever is applicable.
 
-    :param errors: incidental errors
-    :param err_msg: the error message
     :param logger: the logger object
-    :param query_stmt: the query statement
+    :param err_msg: the error message to log
+    :param level: log level (defaults to DEBUG)
+    :param errors: optional incidental errors
+    :param query_stmt: optional the query statement
     :param bind_vals: optional bind values for the query statement
     """
     if err_msg:
         if logger:
-            logger.error(err_msg)
+            logger.log(level, err_msg)
         if isinstance(errors, list):
             errors.append(err_msg)
-    elif logger:
-        debug_msg: str = _db_build_query_msg(query_stmt, bind_vals)
-        logger.debug(debug_msg)
+    if logger and query_stmt:
+        log_msg: str = _db_build_query_msg(query_stmt, bind_vals)
+        logger.log(level, log_msg)
```

### Comparing `pypomes_db-0.5.6/src/pypomes_db/db_pomes.py` & `pypomes_db-0.5.7/src/pypomes_db/db_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,15 +466,14 @@
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: number of tuples effectively copied
     """
     # initialize the return variable
     result: int | None = None
 
-    # no inspection DuplicatedCode
     curr_engine: str = _assert_engine(errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
         result = oracle_pomes.db_bulk_copy(errors=errors,
                                            sel_stmt=sel_stmt,
@@ -507,105 +506,105 @@
                                               target_conn=target_conn,
                                               conn=conn,
                                               logger=logger)
 
     return result
 
 
-def db_copy_lobs(errors: list[str],
-                 lob_table: str,
-                 lob_column: str,
-                 pk_columns: list[str],
-                 target_engine: str,
-                 where_clause: tuple = None,
-                 temp_file: str | Path = None,
-                 chunk_size: int = None,
-                 target_table: str = None,
-                 target_column: str = None,
-                 target_conn: Any = None,
-                 engine: str = None,
-                 conn: Any = None,
-                 logger: Logger = None) -> int:
+def db_migrate_lobs(errors: list[str],
+                    lob_table: str,
+                    lob_column: str,
+                    pk_columns: list[str],
+                    target_engine: str,
+                    where_clause: tuple = None,
+                    temp_file: str | Path = None,
+                    chunk_size: int = None,
+                    target_table: str = None,
+                    target_column: str = None,
+                    target_conn: Any = None,
+                    engine: str = None,
+                    conn: Any = None,
+                    logger: Logger = None) -> int:
     """
-    Copy large binary objects (LOBs) from one database to another database.
+    Migrate large binary objects (LOBs) from one database to another database.
 
     The destination database must be in the list of databases configured and supported by this package.
     One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
     and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
     and are of equivalent types, in both the origin and the destination database.
     If *temp_file* is not provided, a plataform-specific temporary file is used.
 
     :param errors: incidental error messages
-    :param lob_table: the column holding the LOBs
+    :param lob_table: the table holding the LOBs
     :param lob_column: the column holding the LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param target_engine: the destination database engine type
     :param where_clause: the criteria for tuple selection
     :param temp_file: temporary file to use (a file object or a valid file path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param target_table: the table to write the lob to (defaults to the source table)
     :param target_column: the column to write the lob to (defaults to the source column)
     :param target_conn: the connection to the destination database
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: number of LOBs effectively copied
+    :return: number of LOBs effectively migrated
     """
     # initialize the return variable
     result: int | None = None
 
     curr_engine: str = _assert_engine(errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_copy_lobs(errors=errors,
-                                           lob_table=lob_table,
-                                           lob_column=lob_column,
-                                           pk_columns=pk_columns,
-                                           target_engine=target_engine,
-                                           where_clause=where_clause,
-                                           temp_file=temp_file,
-                                           chunk_size=chunk_size,
-                                           target_table=target_table,
-                                           target_column=target_column,
-                                           target_conn=target_conn,
-                                           conn=conn,
-                                           logger=logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_copy_lobs(errors=errors,
-                                             lob_table=lob_table,
-                                             lob_column=lob_column,
-                                             pk_columns=pk_columns,
-                                             target_engine=target_engine,
-                                             where_clause=where_clause,
-                                             temp_file=temp_file,
-                                             chunk_size=chunk_size,
-                                             target_table=target_table,
-                                             target_column=target_column,
-                                             target_conn=target_conn,
-                                             conn=conn,
-                                             logger=logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        pass
-        result = sqlserver_pomes.db_copy_lobs(errors=errors,
+        result = oracle_pomes.db_migrate_lobs(errors=errors,
                                               lob_table=lob_table,
                                               lob_column=lob_column,
                                               pk_columns=pk_columns,
                                               target_engine=target_engine,
                                               where_clause=where_clause,
                                               temp_file=temp_file,
                                               chunk_size=chunk_size,
                                               target_table=target_table,
                                               target_column=target_column,
                                               target_conn=target_conn,
                                               conn=conn,
                                               logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_migrate_lobs(errors=errors,
+                                                lob_table=lob_table,
+                                                lob_column=lob_column,
+                                                pk_columns=pk_columns,
+                                                target_engine=target_engine,
+                                                where_clause=where_clause,
+                                                temp_file=temp_file,
+                                                chunk_size=chunk_size,
+                                                target_table=target_table,
+                                                target_column=target_column,
+                                                target_conn=target_conn,
+                                                conn=conn,
+                                                logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        pass
+        result = sqlserver_pomes.db_migrate_lobs(errors=errors,
+                                                 lob_table=lob_table,
+                                                 lob_column=lob_column,
+                                                 pk_columns=pk_columns,
+                                                 target_engine=target_engine,
+                                                 where_clause=where_clause,
+                                                 temp_file=temp_file,
+                                                 chunk_size=chunk_size,
+                                                 target_table=target_table,
+                                                 target_column=target_column,
+                                                 target_conn=target_conn,
+                                                 conn=conn,
+                                                 logger=logger)
 
     return result
 
 
 def db_update_lob(errors: list[str],
                  lob_table: str,
                  lob_column: str,
@@ -616,15 +615,15 @@
                  engine: str = None,
                  conn: Any = None,
                  logger: Logger = None) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
-    :param lob_table: the column to be update with the new LOB
+    :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
```

### Comparing `pypomes_db-0.5.6/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.5.7/src/pypomes_db/oracle_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noinspection DuplicatedCode
 from logging import Logger
 from oracledb import Connection, connect, init_oracle_client
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Any
 
 from .db_common import (
@@ -38,17 +39,17 @@
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
@@ -112,17 +113,17 @@
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
@@ -165,17 +166,17 @@
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
 def db_bulk_copy(errors: list[str],
@@ -208,15 +209,14 @@
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
-        # noinspection DuplicatedCode
         with curr_conn.cursor() as cursor:
 
             # execute the query
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
 
             # fetch rows in batches/all rows
@@ -255,62 +255,62 @@
             target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
-def db_copy_lobs(errors: list[str],
-                 lob_table: str,
-                 lob_column: str,
-                 pk_columns: list[str],
-                 target_engine: str,
-                 where_clause: tuple,
-                 temp_file: str | Path,
-                 chunk_size: int,
-                 target_table: str,
-                 target_column: str,
-                 target_conn: Any,
-                 conn: Connection,
-                 logger: Logger) -> int:
+def db_migrate_lobs(errors: list[str],
+                    lob_table: str,
+                    lob_column: str,
+                    pk_columns: list[str],
+                    target_engine: str,
+                    where_clause: tuple,
+                    temp_file: str | Path,
+                    chunk_size: int,
+                    target_table: str,
+                    target_column: str,
+                    target_conn: Any,
+                    conn: Connection,
+                    logger: Logger) -> int:
     """
-    Copy large binary objects (LOBs) from an Oracle database to another database.
+    Migrate large binary objects (LOBs) from an Oracle database to another database.
 
     The destination database must be in the list of databases configured and supported by this package.
     One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
     and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
     and are of equivalent types, in both the origin and the destination database.
     If *temp_file* is not provided, a plataform-specific temporary file is used.
 
     :param errors: incidental error messages
-    :param lob_table: the column holding the LOBs
+    :param lob_table: the table holding the LOBs
     :param lob_column: the column holding the LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param target_engine: the destination database engine type
     :param where_clause: the criteria for tuple selection
     :param temp_file: temporary file to use (a file object or a valid file path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param target_table: the table to write the lob to (defaults to the source table)
     :param target_column: the column to write the lob to (defaults to the source column)
     :param target_conn: the connection to the destination database
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: number of LOBs effectively copied
+    :return: number of LOBs effectively migrated
     """
     # initialize the return variable
-    result: int | None = None
+    result: int = 0
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     # make sure to have a target table
     if not target_table:
@@ -334,15 +334,14 @@
     sel_stmt: str = f"SELECT {pks}, {lob_column} FROM {lob_table}"
     if where_clause:
         sel_stmt += f" WHERE {where_clause}"
     blob_index: int = len(pk_columns)
 
     err_msg: str | None = None
     try:
-        # noinspection DuplicatedCode
         with curr_conn.cursor() as cursor:
 
             # execute the query
             cursor.execute(statement=sel_stmt)
 
             # fetch rows
             for row in cursor:
@@ -366,17 +365,21 @@
                                  lob_file=lob_file,
                                  chunk_size=chunk_size,
                                  pk_columns=pk_columns,
                                  pk_vals=pk_vals,
                                  engine=target_engine,
                                  conn=target_conn,
                                  logger=logger)
-
-                # register possible errors
-                errors.extend(op_errors)
+                # errors ?
+                if op_errors:
+                    # yes, register them
+                    errors.extend(op_errors)
+                else:
+                    # no, increment the LOB migration counter
+                    result += 1
 
         # commit the source and target transactions
         curr_conn.commit()
         target_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
@@ -385,18 +388,20 @@
             target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
-            query_stmt=sel_stmt)
+            errors=errors,
+            query_stmt=(f"{result} LOBs migrated, "
+                        f"from oracle at {lob_table}.{lob_column} "
+                        f"to {target_engine} at {target_table}.{target_column}"))
 
     return result
 
 
 def db_update_lob(errors: list[str],
                   lob_table: str,
                   lob_column: str,
@@ -406,15 +411,15 @@
                   chunk_size: int,
                   conn: Connection,
                   logger: Logger) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
-    :param lob_table: the column to be update with the new LOB
+    :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
@@ -460,17 +465,17 @@
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=update_stmt,
             bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
@@ -516,17 +521,17 @@
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
@@ -565,15 +570,14 @@
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
-    # noinspection DuplicatedCode
     result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     # execute the stored procedure
@@ -594,17 +598,17 @@
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=proc_name,
             bind_vals=proc_vals)
 
     return result
 
 __is_initialized: str | None = None
 
@@ -628,13 +632,13 @@
             init_oracle_client(client)
             __is_initialized = True
         except Exception as e:
             result = False
             err_msg = _db_except_msg(exception=e,
                                      engine="oracle")
         # log the results
-        _db_log(errors=errors,
+        _db_log(logger=logger,
                 err_msg=err_msg,
-                logger=logger,
+                errors=errors,
                 query_stmt="Initializing the client")
 
     return result
```

### Comparing `pypomes_db-0.5.6/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.5.7/src/pypomes_db/postgres_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noinspection DuplicatedCode
 from logging import Logger
 from pathlib import Path
 from psycopg2 import Binary, connect
 from psycopg2.extras import DictCursor, execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
 from tempfile import NamedTemporaryFile
@@ -39,17 +40,17 @@
                          password=pwd)
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(e, "postgres")
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
@@ -112,17 +113,17 @@
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
@@ -168,17 +169,17 @@
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=insert_stmt)
 
     return result
 
 
 def db_bulk_copy(errors: list[str],
                  sel_stmt: str,
@@ -210,15 +211,14 @@
 
     # make sure to have a connection
     curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
-        # noinspection DuplicatedCode
         with curr_conn.cursor() as cursor:
 
             # execute the query
             cursor.execute(statement=sel_stmt,
                            parameters=where_vals)
 
             # fetch rows in batches/all rows
@@ -257,62 +257,62 @@
             target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
-def db_copy_lobs(errors: list[str],
-                 lob_table: str,
-                 lob_column: str,
-                 pk_columns: list[str],
-                 target_engine: str,
-                 where_clause: tuple,
-                 temp_file: str | Path,
-                 chunk_size: int,
-                 target_table: str,
-                 target_column: str,
-                 target_conn: Any,
-                 conn: connection,
-                 logger: Logger) -> int:
+def db_migrate_lobs(errors: list[str],
+                    lob_table: str,
+                    lob_column: str,
+                    pk_columns: list[str],
+                    target_engine: str,
+                    where_clause: tuple,
+                    temp_file: str | Path,
+                    chunk_size: int,
+                    target_table: str,
+                    target_column: str,
+                    target_conn: Any,
+                    conn: connection,
+                    logger: Logger) -> int:
     """
-    Copy large binary objects (LOBs) from a Postgres database to another database.
+    Migrate large binary objects (LOBs) from a Postgres database to another database.
 
     The destination database must be in the list of databases configured and supported by this package.
     One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
     and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
     and are of equivalent types, in both the origin and the destination database.
     If *temp_file* is not provided, a plataform-specific temporary file is used.
 
     :param errors: incidental error messages
-    :param lob_table: the column holding the LOBs
+    :param lob_table: the table holding the LOBs
     :param lob_column: the column holding the LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param target_engine: the destination database engine type
     :param where_clause: the criteria for tuple selection
     :param temp_file: temporary file to use (a file object or a valid file path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param target_table: the table to write the lob to (defaults to the source table)
     :param target_column: the column to write the lob to (defaults to the source column)
     :param target_conn: the connection to the destination database
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: number of LOBs effectively copied
+    :return: number of LOBs effectively migrated
     """
     # initialize the return variable
-    result: int | None = None
+    result: int = 0
 
     # make sure to have a connection
     curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     # make sure to have a target table
     if not target_table:
@@ -336,15 +336,14 @@
     sel_stmt: str = f"SELECT {pks}, {lob_column} FROM {lob_table}"
     if where_clause:
         sel_stmt += f" WHERE {where_clause}"
     blob_index: int = len(pk_columns)
 
     err_msg: str | None = None
     try:
-        # noinspection DuplicatedCode
         with curr_conn.cursor(cursor_factory=DictCursor) as cursor:
 
             # execute the query
             cursor.execute(statement=sel_stmt)
 
             # fetch rows
             for row in cursor:
@@ -368,17 +367,21 @@
                                  lob_file=lob_file,
                                  chunk_size=chunk_size,
                                  pk_columns=pk_columns,
                                  pk_vals=pk_vals,
                                  engine=target_engine,
                                  conn=target_conn,
                                  logger=logger)
-
-                # register possible errors
-                errors.extend(op_errors)
+                # errors ?
+                if op_errors:
+                    # yes, register them
+                    errors.extend(op_errors)
+                else:
+                    # no, increment the LOB migration counter
+                    result += 1
 
         # commit the source and target transactions
         curr_conn.commit()
         target_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
@@ -387,18 +390,20 @@
             target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
-            query_stmt=sel_stmt)
+            errors=errors,
+            query_stmt=(f"{result} LOBs migrated, "
+                        f"from postgres at {lob_table}.{lob_column} "
+                        f"to {target_engine} at {target_table}.{target_column}"))
 
     return result
 
 
 def db_update_lob(errors: list[str],
                   lob_table: str,
                   lob_column: str,
@@ -408,15 +413,15 @@
                   chunk_size: int,
                   conn: connection,
                   logger: Logger) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
-    :param lob_table: the column to be update with the new LOB
+    :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
@@ -460,17 +465,17 @@
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=update_stmt,
             bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
@@ -516,17 +521,17 @@
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
 
@@ -572,14 +577,14 @@
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=proc_stmt,
             bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.5.6/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.5.7/src/pypomes_db/sqlserver_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noinspection DuplicatedCode
 from logging import Logger
 from pyodbc import Binary, Connection, Row, connect
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Any
 
 from .db_common import (
@@ -37,17 +38,17 @@
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
@@ -109,17 +110,17 @@
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
@@ -165,17 +166,17 @@
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
 def db_bulk_copy(errors: list[str],
@@ -208,15 +209,14 @@
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
-        # noinspection DuplicatedCode
         with curr_conn.cursor() as cursor:
 
             # execute the query
             cursor.execute(sel_stmt, where_vals)
 
             # fetch rows in batches/all rows
             result = 0
@@ -255,62 +255,62 @@
             target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
-def db_copy_lobs(errors: list[str],
-                 lob_table: str,
-                 lob_column: str,
-                 pk_columns: list[str],
-                 target_engine: str,
-                 where_clause: tuple,
-                 temp_file: str | Path,
-                 chunk_size: int,
-                 target_table: str,
-                 target_column: str,
-                 target_conn: Any,
-                 conn: Connection,
-                 logger: Logger) -> int:
+def db_migrate_lobs(errors: list[str],
+                    lob_table: str,
+                    lob_column: str,
+                    pk_columns: list[str],
+                    target_engine: str,
+                    where_clause: tuple,
+                    temp_file: str | Path,
+                    chunk_size: int,
+                    target_table: str,
+                    target_column: str,
+                    target_conn: Any,
+                    conn: Connection,
+                    logger: Logger) -> int:
     """
-    Copy large binary objects (LOBs) from a SQLServer database to another database.
+    Migrate large binary objects (LOBs) from a SQLServer database to another database.
 
     The destination database must be in the list of databases configured and supported by this package.
     One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
     and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
     and are of equivalent types, in both the origin and the destination database.
     If *temp_file* is not provided, a plataform-specific temporary file is used.
 
     :param errors: incidental error messages
-    :param lob_table: the column holding the LOBs
+    :param lob_table: the table holding the LOBs
     :param lob_column: the column holding the LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param target_engine: the destination database engine type
     :param where_clause: the criteria for tuple selection
     :param temp_file: temporary file to use (a file object or a valid file path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param target_table: the table to write the lob to (defaults to the source table)
     :param target_column: the column to write the lob to (defaults to the source column)
     :param target_conn: the connection to the destination database
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: number of LOBs effectively copied
+    :return: number of LOBs effectively migrated
     """
     # initialize the return variable
-    result: int | None = None
+    result: int = 0
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     # make sure to have a target table
     if not target_table:
@@ -334,15 +334,14 @@
     sel_stmt: str = f"SELECT {pks}, {lob_column} FROM {lob_table}"
     if where_clause:
         sel_stmt += f" WHERE {where_clause}"
     blob_index: int = len(pk_columns)
 
     err_msg: str | None = None
     try:
-        # noinspection DuplicatedCode
         with curr_conn.cursor() as cursor:
 
             # execute the query
             cursor.execute(sel_stmt)
 
             # fetch rows
             for row in cursor:
@@ -366,17 +365,21 @@
                                  lob_file=lob_file,
                                  chunk_size=chunk_size,
                                  pk_columns=pk_columns,
                                  pk_vals=pk_vals,
                                  engine=target_engine,
                                  conn=target_conn,
                                  logger=logger)
-
-                # register possible errors
-                errors.extend(op_errors)
+                # errors ?
+                if op_errors:
+                    # yes, register them
+                    errors.extend(op_errors)
+                else:
+                    # no, increment the LOB migration counter
+                    result += 1
 
         # commit the source and target transactions
         curr_conn.commit()
         target_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
@@ -385,18 +388,20 @@
             target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
-            query_stmt=sel_stmt)
+            errors=errors,
+            query_stmt=(f"{result} LOBs migrated, "
+                        f"from oracle at {lob_table}.{lob_column} "
+                        f"to {target_engine} at {target_table}.{target_column}"))
 
     return result
 
 
 def db_update_lob(errors: list[str],
                   lob_table: str,
                   lob_column: str,
@@ -406,15 +411,15 @@
                   chunk_size: int,
                   conn: Connection,
                   logger: Logger) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
-    :param lob_table: the column to be update with the new LOB
+    :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
@@ -457,17 +462,17 @@
                                  engine="oracle")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=update_stmt,
             bind_vals=pk_vals)
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
@@ -512,17 +517,17 @@
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
 def db_call_procedure(errors: list[str],
@@ -568,14 +573,14 @@
                                  engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
-    _db_log(errors=errors,
+    _db_log(logger=logger,
             err_msg=err_msg,
-            logger=logger,
+            errors=errors,
             query_stmt=proc_stmt,
             bind_vals=proc_vals)
 
     return result
```

### Comparing `pypomes_db-0.5.6/LICENSE` & `pypomes_db-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.6/pyproject.toml` & `pypomes_db-0.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.5.6"
+version = "0.5.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.5.6/PKG-INFO` & `pypomes_db-0.5.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.5.6
+Version: 0.5.7
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


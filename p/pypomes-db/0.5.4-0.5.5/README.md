# Comparing `tmp/pypomes_db-0.5.4.tar.gz` & `tmp/pypomes_db-0.5.5.tar.gz`

## Comparing `pypomes_db-0.5.4.tar` & `pypomes_db-0.5.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    29559 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    15840 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    13750 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38002 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    24057 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    21898 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    21948 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.5/PKG-INFO
```

### Comparing `pypomes_db-0.5.4/src/pypomes_db/__init__.py` & `pypomes_db-0.5.5/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.4/src/pypomes_db/db_common.py` & `pypomes_db-0.5.5/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.4/src/pypomes_db/db_pomes.py` & `pypomes_db-0.5.5/src/pypomes_db/db_pomes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from logging import Logger
+from pathlib import Path
 from typing import Any
 
 from .db_common import (
     _DB_ENGINES, _DB_CONN_DATA, _assert_engine
 )
 
 
@@ -212,15 +213,15 @@
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: tuple containing the search result, or None if there was an error, or if the search was empty
+    :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     require_min: int = 1 if require_nonempty else None
     reply: list[tuple] = db_select_all(errors=errors,
                                        sel_stmt=sel_stmt,
                                        where_vals=where_vals,
                                        require_min=require_min,
                                        require_max=1,
@@ -446,15 +447,15 @@
                  batch_size: int = None,
                  where_vals: tuple = None,
                  target_conn: Any = None,
                  engine: str = None,
                  conn: Any = None,
                  logger: Logger = None) -> int:
     """
-    Bulk copy data from a Oracle database to another database.
+    Bulk copy data from one database to another database.
 
     The destination database brand must be in the list of databases configured and supported by this package.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param insert_stmt: the insert statement to use for bulk-inserting
     :param target_engine: the destination database engine type
@@ -465,14 +466,15 @@
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: number of tuples effectively copied
     """
     # initialize the return variable
     result: int | None = None
 
+    # no inspection DuplicatedCode
     curr_engine: str = _assert_engine(errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
         result = oracle_pomes.db_bulk_copy(errors=errors,
                                            sel_stmt=sel_stmt,
@@ -505,14 +507,173 @@
                                               target_conn=target_conn,
                                               conn=conn,
                                               logger=logger)
 
     return result
 
 
+def db_copy_lobs(errors: list[str],
+                 lob_table: str,
+                 lob_column: str,
+                 pk_columns: list[str],
+                 target_engine: str,
+                 where_clause: tuple = None,
+                 temp_file: str | Path = None,
+                 chunk_size: int = None,
+                 target_table: str = None,
+                 target_column: str = None,
+                 target_conn: Any = None,
+                 engine: str = None,
+                 conn: Any = None,
+                 logger: Logger = None) -> int:
+    """
+    Copy large binary objects (LOBs) from one database to another database.
+
+    The destination database must be in the list of databases configured and supported by this package.
+    One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
+    and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
+    and are of equivalent types, in both the origin and the destination database.
+    If *temp_file* is not provided, a plataform-specific temporary file is used.
+
+    :param errors: incidental error messages
+    :param lob_table: the column holding the LOBs
+    :param lob_column: the column holding the LOB
+    :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
+    :param target_engine: the destination database engine type
+    :param where_clause: the criteria for tuple selection
+    :param temp_file: temporary file to use (a file object or a valid file path)
+    :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
+    :param target_table: the table to write the lob to (defaults to the source table)
+    :param target_column: the column to write the lob to (defaults to the source column)
+    :param target_conn: the connection to the destination database
+    :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    :return: number of LOBs effectively copied
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    curr_engine: str = _assert_engine(errors, engine)
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        result = oracle_pomes.db_copy_lobs(errors=errors,
+                                           lob_table=lob_table,
+                                           lob_column=lob_column,
+                                           pk_columns=pk_columns,
+                                           target_engine=target_engine,
+                                           where_clause=where_clause,
+                                           temp_file=temp_file,
+                                           chunk_size=chunk_size,
+                                           target_table=target_table,
+                                           target_column=target_column,
+                                           target_conn=target_conn,
+                                           conn=conn,
+                                           logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.db_copy_lobs(errors=errors,
+                                             lob_table=lob_table,
+                                             lob_column=lob_column,
+                                             pk_columns=pk_columns,
+                                             target_engine=target_engine,
+                                             where_clause=where_clause,
+                                             temp_file=temp_file,
+                                             chunk_size=chunk_size,
+                                             target_table=target_table,
+                                             target_column=target_column,
+                                             target_conn=target_conn,
+                                             conn=conn,
+                                             logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        pass
+        result = sqlserver_pomes.db_copy_lobs(errors=errors,
+                                              lob_table=lob_table,
+                                              lob_column=lob_column,
+                                              pk_columns=pk_columns,
+                                              target_engine=target_engine,
+                                              where_clause=where_clause,
+                                              temp_file=temp_file,
+                                              chunk_size=chunk_size,
+                                              target_table=target_table,
+                                              target_column=target_column,
+                                              target_conn=target_conn,
+                                              conn=conn,
+                                              logger=logger)
+
+    return result
+
+
+def db_update_lob(errors: list[str],
+                 lob_table: str,
+                 lob_column: str,
+                 pk_columns: list[str],
+                 pk_vals: tuple,
+                 lob_file: str | Path,
+                 chunk_size: int,
+                 engine: str = None,
+                 conn: Any = None,
+                 logger: Logger = None) -> None:
+    """
+    Update a large binary objects (LOB) in the given table and column.
+
+    :param errors: incidental error messages
+    :param lob_table: the column to be update with the new LOB
+    :param lob_column: the column to be updated with the new LOB
+    :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
+    :param pk_vals: values with which to locate the tuple to be updated
+    :param lob_file: file holding the LOB (a file object or a valid path)
+    :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
+    :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    :return: number of LOBs effectively copied
+    """
+    curr_engine: str = _assert_engine(errors, engine)
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        oracle_pomes.db_update_lob(errors=errors,
+                                   lob_table=lob_table,
+                                   lob_column=lob_column,
+                                   pk_columns=pk_columns,
+                                   pk_vals=pk_vals,
+                                   lob_file=lob_file,
+                                   chunk_size=chunk_size,
+                                   conn=conn,
+                                   logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        postgres_pomes.db_update_lob(errors=errors,
+                                     lob_table=lob_table,
+                                     lob_column=lob_column,
+                                     pk_columns=pk_columns,
+                                     pk_vals=pk_vals,
+                                     lob_file=lob_file,
+                                     chunk_size=chunk_size,
+                                     conn=conn,
+                                     logger=logger)
+        pass
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        sqlserver_pomes.db_update_lob(errors=errors,
+                                      lob_table=lob_table,
+                                      lob_column=lob_column,
+                                      pk_columns=pk_columns,
+                                      pk_vals=pk_vals,
+                                      lob_file=lob_file,
+                                      chunk_size=chunk_size,
+                                      conn=conn,
+                                      logger=logger)
+
+
 def db_execute(errors: list[str] | None,
                exc_stmt: str,
                bind_vals: tuple = None,
                engine: str = None,
                conn: Any = None,
                logger: Logger = None) -> int:
     """
```

### Comparing `pypomes_db-0.5.4/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.5.5/src/pypomes_db/sqlserver_pomes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from logging import Logger
-from oracledb import Connection, connect, init_oracle_client
+from pyodbc import Binary, Connection, Row, connect
+from pathlib import Path
+from tempfile import NamedTemporaryFile
 from typing import Any
 
 from .db_common import (
-    _DB_CONN_DATA,
     _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 from .db_pomes import db_bulk_insert as db_bulk_insert_to
-
-# TODO: db_call_function, db_call_procedure
+from .db_pomes import db_update_lob as db_update_lob_to
 
 
 def db_connect(errors: list[str],
-               logger: Logger) -> Connection:
+               logger: Logger = None) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
-    # initialize the return variable
+    # initialize the return valiable
     result: Connection | None = None
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
+    # retrieve the connection parameters and build the connection string
+    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
+    connection_kwargs: str = (
+        f"DRIVER={{{driver}}};SERVER={host},{port};"
+        f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
+    )
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = connect(service_name=name,
-                         host=host,
-                         port=port,
-                         user=user,
-                         password=pwd)
+        result = connect(connection_kwargs)
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
@@ -67,52 +67,50 @@
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
-    :return: list of tuples containing the search result, or [] if the search is empty
+    :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
+    err_msg: str | None = None
     if isinstance(require_max, int) and require_max > 0:
-        sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
+        sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
 
-    err_msg: str | None = None
     try:
-        # obtain a cursor and perform the operation
+        # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            # execute the query
-            cursor.execute(statement=sel_stmt,
-                           parameters=where_vals)
+            cursor.execute(sel_stmt, where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
                                    require_min=require_min,
                                    require_max=require_max):
                 # yes, retrieve the returned tuples
-                rows: list = cursor.fetchall()
+                rows: list[Row] = cursor.fetchall()
                 result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -128,17 +126,16 @@
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    conn: Connection,
                    logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
-    The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
-    must contain as many ':n' placeholders as there are elements in the tuples found in the
-    list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
+    The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
+    as there are elements in the tuples found in the list provided in *insert_vals*.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
@@ -150,22 +147,26 @@
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            cursor.executemany(statement=insert_stmt,
-                               parameters=insert_vals)
-            result = len(insert_vals)
+            cursor.fast_executemany = True
+            try:
+                cursor.executemany(insert_stmt, insert_vals)
+                result = len(insert_vals)
+            except Exception:
+                conn.rollback()
+                raise
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -183,15 +184,15 @@
                  target_engine: str,
                  batch_size: int,
                  where_vals: tuple,
                  target_conn: Any,
                  conn: Connection,
                  logger: Logger) -> int:
     """
-    Bulk copy data from a Oracle database to another database.
+    Bulk copy data from a SQLServer database to another database.
 
     The destination database brand must be in the list of databases configured and supported by this package.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param insert_stmt: the insert statement to use for bulk-inserting
     :param target_engine: the destination database engine type
@@ -211,49 +212,51 @@
 
     err_msg: str | None = None
     try:
         # noinspection DuplicatedCode
         with curr_conn.cursor() as cursor:
 
             # execute the query
-            cursor.execute(statement=sel_stmt,
-                           parameters=where_vals)
+            cursor.execute(sel_stmt, where_vals)
 
             # fetch rows in batches/all rows
             result = 0
             op_errors: list[str] = []
-            rows: list[tuple]
+            rows: list[Row]
             if batch_size:
                 rows = cursor.fetchmany(batch_size)
             else:
                 rows = cursor.fetchall()
             while rows:
+                tuples: list[tuple] = [tuple(row) for row in rows]
                 result += db_bulk_insert_to(errors=op_errors,
                                             insert_stmt=insert_stmt,
-                                            insert_vals=rows,
+                                            insert_vals=tuples,
                                             engine=target_engine,
                                             conn=target_conn,
                                             logger=logger) or 0
                 # errors ?
                 if op_errors:
                     # yes, register them and abort the operation
                     errors.extend(op_errors)
                     break
                 if not batch_size:
                     break
                 rows = cursor.fetchmany(batch_size)
 
         # commit the source and target transactions
         curr_conn.commit()
-        target_conn.commit()
+        if target_conn:
+            target_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
         curr_conn.rollback()
-        target_conn.rollback()
+        if target_conn:
+            target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -261,14 +264,214 @@
             logger=logger,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
+def db_copy_lobs(errors: list[str],
+                 lob_table: str,
+                 lob_column: str,
+                 pk_columns: list[str],
+                 target_engine: str,
+                 where_clause: tuple,
+                 temp_file: str | Path,
+                 chunk_size: int,
+                 target_table: str,
+                 target_column: str,
+                 target_conn: Any,
+                 conn: Connection,
+                 logger: Logger) -> int:
+    """
+    Copy large binary objects (LOBs) from a SQLServer database to another database.
+
+    The destination database must be in the list of databases configured and supported by this package.
+    One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
+    and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
+    and are of equivalent types, in both the origin and the destination database.
+    If *temp_file* is not provided, a plataform-specific temporary file is used.
+
+    :param errors: incidental error messages
+    :param lob_table: the column holding the LOBs
+    :param lob_column: the column holding the LOB
+    :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
+    :param target_engine: the destination database engine type
+    :param where_clause: the criteria for tuple selection
+    :param temp_file: temporary file to use (a file object or a valid file path)
+    :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
+    :param target_table: the table to write the lob to (defaults to the source table)
+    :param target_column: the column to write the lob to (defaults to the source column)
+    :param target_conn: the connection to the destination database
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    :return: number of LOBs effectively copied
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
+
+    # make sure to have a target table
+    if not target_table:
+        target_table = lob_table
+
+    # make sure to have a temporary file
+    lob_file: Any
+    if temp_file is None:
+        lob_file = NamedTemporaryFile("wb")
+    elif isinstance(temp_file, str | Path):
+        lob_file = Path(temp_file)
+    else:
+        lob_file = temp_file
+
+    # normalize the chunk size
+    if not chunk_size:
+        chunk_size = -1
+
+    # buid the query
+    pks: str = ", ".join(pk_columns)
+    sel_stmt: str = f"SELECT {pks}, {lob_column} FROM {lob_table}"
+    if where_clause:
+        sel_stmt += f" WHERE {where_clause}"
+    blob_index: int = len(pk_columns)
+
+    err_msg: str | None = None
+    try:
+        # noinspection DuplicatedCode
+        with curr_conn.cursor() as cursor:
+
+            # execute the query
+            cursor.execute(sel_stmt)
+
+            # fetch rows
+            for row in cursor:
+
+                # retrieve the values of the primary key columns (leave blob column out)
+                pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
+
+                # access the blob in chunks and write it to file
+                blob: Any = row[blob_index]
+                with lob_file.open(mode="wb") as file:
+                    blob_data: bytes = blob.read(chunk_size)
+                    while blob_data:
+                        file.write(blob_data)
+                        blob_data = blob.read(chunk_size)
+
+                # send blob to the destination database
+                op_errors: list[str] = []
+                db_update_lob_to(errors=op_errors,
+                                 lob_table=target_table,
+                                 lob_column=target_column,
+                                 lob_file=lob_file,
+                                 chunk_size=chunk_size,
+                                 pk_columns=pk_columns,
+                                 pk_vals=pk_vals,
+                                 engine=target_engine,
+                                 conn=target_conn,
+                                 logger=logger)
+
+                # register possible errors
+                errors.extend(op_errors)
+
+        # commit the source and target transactions
+        curr_conn.commit()
+        target_conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+        curr_conn.rollback()
+        if target_conn:
+            target_conn.rollback()
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=sel_stmt)
+
+    return result
+
+
+def db_update_lob(errors: list[str],
+                  lob_table: str,
+                  lob_column: str,
+                  pk_columns: list[str],
+                  pk_vals: tuple,
+                  lob_file: str | Path,
+                  chunk_size: int,
+                  conn: Connection,
+                  logger: Logger) -> None:
+    """
+    Update a large binary objects (LOB) in the given table and column.
+
+    :param errors: incidental error messages
+    :param lob_table: the column to be update with the new LOB
+    :param lob_column: the column to be updated with the new LOB
+    :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
+    :param pk_vals: values with which to locate the tuple to be updated
+    :param lob_file: file holding the LOB (a file object or a valid path)
+    :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    """
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
+
+    # make sure to have a data file
+    data_file: Path = Path(lob_file) if isinstance(lob_file, str | Path) else lob_file
+
+    # normalize the chunk size
+    if not chunk_size:
+        chunk_size = -1
+
+    # build the UPDATE query
+    where_clause: str = " AND ".join([f"{column} = ?" for column in pk_columns])
+    update_stmt: str = (f"UPDATE {lob_table} "
+                        f"SET {lob_column} = ? "
+                        f"WHERE {where_clause}")
+
+    err_msg: str | None = None
+    try:
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+
+            # retrieve the lob data from file in chunks and write to the file
+            lob_data : bytes
+            with data_file.open("rb") as file:
+                lob_data = file.read(chunk_size)
+                while lob_data:
+                    cursor.execute(update_stmt, (Binary(lob_data), *pk_vals))
+                    lob_data = file.read(chunk_size)
+
+        # commit the transaction
+        curr_conn.commit()
+    except Exception as e:
+        curr_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=update_stmt,
+            bind_vals=pk_vals)
+
+
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
                conn: Connection,
                logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
@@ -295,23 +498,22 @@
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(statement=exc_stmt,
-                           parameters=bind_vals)
+            cursor.execute(exc_stmt, bind_vals)
             result = cursor.rowcount
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -319,116 +521,61 @@
             logger=logger,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
-# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
-# noinspection PyUnusedLocal
-def db_call_function(errors: list[str],
-                     func_name: str,
-                     func_vals: tuple,
-                     conn: Connection,
-                     logger: Logger) -> list[tuple]:
-    """
-    Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
-
-    :param errors: incidental error messages
-    :param func_name: name of the stored function
-    :param func_vals: parameters for the stored function
-    :param conn: optional connection to use (obtains a new one, if not specified)
-    :param logger: optional logger
-    :return: the data returned by the function
-    """
-    # initialize the return variable
-    result: list[tuple] = []
-
-    return result
-
-
-# TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def db_call_procedure(errors: list[str],
                       proc_name: str,
                       proc_vals: tuple,
                       conn: Connection,
-                      logger: Logger) -> list[tuple]:
+                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
-    # noinspection DuplicatedCode
-    result: list[tuple] = []
+    result: list[tuple] | None = None
 
     # make sure to have a connection
     curr_conn: Connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
+    # build the command
+    proc_stmt: str | None = None
+
     # execute the stored procedure
     err_msg: str | None = None
     try:
-        # obtain a cursor and perform the operation
+        # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.callproc(name=proc_name,
-                            parameters=proc_vals)
-
+            proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
+            cursor.execute(proc_stmt, proc_vals)
             # retrieve the returned tuples
-            result = list(cursor)
+            rows: list[Row] = cursor.fetchall()
+            result = [tuple(row) for row in rows]
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine="sqlserver")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=proc_name,
+            query_stmt=proc_stmt,
             bind_vals=proc_vals)
 
     return result
-
-__is_initialized: str | None = None
-
-def initialize(errors: list[str],
-               logger: Logger) -> bool:
-    """
-    Setup the oracle engine to access the database throught the installed client software.
-
-    :param errors: incidental error messages
-    :param logger: optional logger
-    :return: False if an error happened, True otherwise
-    """
-    # initialize the return variable
-    result: bool = True
-
-    global __is_initialized
-    if not __is_initialized:
-        err_msg: str | None = None
-        client: str = _DB_CONN_DATA["oracle"]["client"]
-        try:
-            init_oracle_client(client)
-            __is_initialized = True
-        except Exception as e:
-            result = False
-            err_msg = _db_except_msg(exception=e,
-                                     engine="oracle")
-        # log the results
-        _db_log(errors=errors,
-                err_msg=err_msg,
-                logger=logger,
-                query_stmt="Initializing the client")
-
-    return result
```

### Comparing `pypomes_db-0.5.4/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.5.5/src/pypomes_db/postgres_pomes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 from logging import Logger
-from pyodbc import connect, Connection, Row
+from pathlib import Path
+from psycopg2 import Binary, connect
+from psycopg2.extras import DictCursor, execute_values
+# noinspection PyProtectedMember
+from psycopg2._psycopg import connection
+from tempfile import NamedTemporaryFile
 from typing import Any
 
 from .db_common import (
     _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 from .db_pomes import db_bulk_insert as db_bulk_insert_to
+from .db_pomes import db_update_lob as db_update_lob_to
 
 
 def db_connect(errors: list[str],
-               logger: Logger = None) -> Connection:
+               logger: Logger = None) -> connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
-    # initialize the return valiable
-    result: Connection | None = None
+    # initialize the return variable
+    result: connection | None = None
 
-    # retrieve the connection parameters and build the connection string
-    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
-    connection_kwargs: str = (
-        f"DRIVER={{{driver}}};SERVER={host},{port};"
-        f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
-    )
+    # retrieve the connection parameters
+    name, user, pwd, host, port = _db_get_params("postgres")
 
     # obtain a connection to the database
     err_msg: str | None = None
     try:
-        result = connect(connection_kwargs)
+        result = connect(host=host,
+                         port=port,
+                         database=name,
+                         user=user,
+                         password=pwd)
         # make sure the connection is not in autocommit mode
         result.autocommit = False
     except Exception as e:
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+        err_msg = _db_except_msg(e, "postgres")
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
@@ -47,15 +52,15 @@
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
                   where_vals: tuple,
                   require_min: int,
                   require_max: int,
-                  conn: Connection,
+                  conn: connection,
                   logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
@@ -70,44 +75,45 @@
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
+    curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
-    err_msg: str | None = None
-    if isinstance(require_max, int) and require_max > 0:
-        sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
+    if isinstance(require_max, int) and require_max >= 0:
+        sel_stmt += f" LIMIT {require_max}"
 
+    err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(sel_stmt, where_vals)
+            cursor.execute(query=f"{sel_stmt};",
+                           vars=where_vals)
             # obtain the number of tuples returned
             count: int = cursor.rowcount
 
             # has the query quota been satisfied ?
             if _assert_query_quota(errors=errors,
                                    query=sel_stmt,
                                    where_vals=where_vals,
                                    count=count,
                                    require_min=require_min,
                                    require_max=require_max):
                 # yes, retrieve the returned tuples
-                rows: list[Row] = cursor.fetchall()
-                result = [tuple(row) for row in rows]
+                result = list(cursor)
+
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -118,78 +124,77 @@
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
-                   conn: Connection,
+                   conn: connection,
                    logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
-    The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
-    as there are elements in the tuples found in the list provided in *insert_vals*.
+    The *VALUES* clause in *insert_stmt* must be simply *VALUES %s*.
+    Note that, after the execution of *execute_values*, the *cursor.rowcount* property
+    will not contain a total result, and thus the value 1 (one) is returned on success.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
+    curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
+    # execute the bulk insert
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            cursor.fast_executemany = True
-            try:
-                cursor.executemany(insert_stmt, insert_vals)
-                result = len(insert_vals)
-            except Exception:
-                conn.rollback()
-                raise
+            execute_values(cur=cursor,
+                           sql=insert_stmt,
+                           argslist=insert_vals)
+            result = len(insert_vals)
+        # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
-            query_stmt=insert_stmt,
-            bind_vals=insert_vals[0])
+            query_stmt=insert_stmt)
 
     return result
 
 
 def db_bulk_copy(errors: list[str],
                  sel_stmt: str,
                  insert_stmt: str,
                  target_engine: str,
                  batch_size: int,
                  where_vals: tuple,
                  target_conn: Any,
-                 conn: Connection,
+                 conn: connection,
                  logger: Logger) -> int:
     """
-    Bulk copy data from a Oracle database to another database.
+    Bulk copy data from a Postgres database to another database.
 
     The destination database brand must be in the list of databases configured and supported by this package.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param insert_stmt: the insert statement to use for bulk-inserting
     :param target_engine: the destination database engine type
@@ -200,58 +205,60 @@
     :param logger: optional logger
     :return: number of tuples effectively copied
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
+    curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         # noinspection DuplicatedCode
         with curr_conn.cursor() as cursor:
 
             # execute the query
-            cursor.execute(sel_stmt, where_vals)
+            cursor.execute(statement=sel_stmt,
+                           parameters=where_vals)
 
             # fetch rows in batches/all rows
             result = 0
             op_errors: list[str] = []
-            rows: list[Row]
+            rows: list[tuple]
             if batch_size:
                 rows = cursor.fetchmany(batch_size)
             else:
                 rows = cursor.fetchall()
             while rows:
-                tuples: list[tuple] = [tuple(row) for row in rows]
                 result += db_bulk_insert_to(errors=op_errors,
                                             insert_stmt=insert_stmt,
-                                            insert_vals=tuples,
+                                            insert_vals=rows,
                                             engine=target_engine,
                                             conn=target_conn,
                                             logger=logger) or 0
                 # errors ?
                 if op_errors:
                     # yes, register them and abort the operation
                     errors.extend(op_errors)
                     break
                 if not batch_size:
                     break
                 rows = cursor.fetchmany(batch_size)
 
         # commit the source and target transactions
         curr_conn.commit()
-        target_conn.commit()
+        if target_conn:
+          target_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
         curr_conn.rollback()
-        target_conn.rollback()
+        if target_conn:
+            target_conn.rollback()
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -259,18 +266,219 @@
             logger=logger,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
+def db_copy_lobs(errors: list[str],
+                 lob_table: str,
+                 lob_column: str,
+                 pk_columns: list[str],
+                 target_engine: str,
+                 where_clause: tuple,
+                 temp_file: str | Path,
+                 chunk_size: int,
+                 target_table: str,
+                 target_column: str,
+                 target_conn: Any,
+                 conn: connection,
+                 logger: Logger) -> int:
+    """
+    Copy large binary objects (LOBs) from a Postgres database to another database.
+
+    The destination database must be in the list of databases configured and supported by this package.
+    One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
+    and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
+    and are of equivalent types, in both the origin and the destination database.
+    If *temp_file* is not provided, a plataform-specific temporary file is used.
+
+    :param errors: incidental error messages
+    :param lob_table: the column holding the LOBs
+    :param lob_column: the column holding the LOB
+    :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
+    :param target_engine: the destination database engine type
+    :param where_clause: the criteria for tuple selection
+    :param temp_file: temporary file to use (a file object or a valid file path)
+    :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
+    :param target_table: the table to write the lob to (defaults to the source table)
+    :param target_column: the column to write the lob to (defaults to the source column)
+    :param target_conn: the connection to the destination database
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    :return: number of LOBs effectively copied
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # make sure to have a connection
+    curr_conn: connection = conn or db_connect(errors=errors,
+                                               logger=logger)
+
+    # make sure to have a target table
+    if not target_table:
+        target_table = lob_table
+
+    # make sure to have a temporary file
+    lob_file: Any
+    if temp_file is None:
+        lob_file = NamedTemporaryFile("wb")
+    elif isinstance(temp_file, str | Path):
+        lob_file = Path(temp_file)
+    else:
+        lob_file = temp_file
+
+    # normalize the chunk size
+    if not chunk_size:
+        chunk_size = -1
+
+    # buid the query
+    pks: str = ", ".join(pk_columns)
+    sel_stmt: str = f"SELECT {pks}, {lob_column} FROM {lob_table}"
+    if where_clause:
+        sel_stmt += f" WHERE {where_clause}"
+    blob_index: int = len(pk_columns)
+
+    err_msg: str | None = None
+    try:
+        # noinspection DuplicatedCode
+        with curr_conn.cursor(cursor_factory=DictCursor) as cursor:
+
+            # execute the query
+            cursor.execute(statement=sel_stmt)
+
+            # fetch rows
+            for row in cursor:
+
+                # retrieve the values of the primary key columns (leave blob column out)
+                pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
+
+                # access the blob in chunks and write it to file
+                blob: Any = row[blob_index]
+                with lob_file.open(mode="wb") as file:
+                    blob_data: bytes = blob.read(chunk_size)
+                    while blob_data:
+                        file.write(blob_data)
+                        blob_data = blob.read(chunk_size)
+
+                # send blob to the destination database
+                op_errors: list[str] = []
+                db_update_lob_to(errors=op_errors,
+                                 lob_table=target_table,
+                                 lob_column=target_column,
+                                 lob_file=lob_file,
+                                 chunk_size=chunk_size,
+                                 pk_columns=pk_columns,
+                                 pk_vals=pk_vals,
+                                 engine=target_engine,
+                                 conn=target_conn,
+                                 logger=logger)
+
+                # register possible errors
+                errors.extend(op_errors)
+
+        # commit the source and target transactions
+        curr_conn.commit()
+        target_conn.commit()
+    except Exception as e:
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+        curr_conn.rollback()
+        if target_conn:
+            target_conn.rollback()
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=sel_stmt)
+
+    return result
+
+
+def db_update_lob(errors: list[str],
+                  lob_table: str,
+                  lob_column: str,
+                  pk_columns: list[str],
+                  pk_vals: tuple,
+                  lob_file: str | Path,
+                  chunk_size: int,
+                  conn: connection,
+                  logger: Logger) -> None:
+    """
+    Update a large binary objects (LOB) in the given table and column.
+
+    :param errors: incidental error messages
+    :param lob_table: the column to be update with the new LOB
+    :param lob_column: the column to be updated with the new LOB
+    :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
+    :param pk_vals: values with which to locate the tuple to be updated
+    :param lob_file: file holding the LOB (a file object or a valid path)
+    :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
+    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param logger: optional logger
+    """
+    # make sure to have a connection
+    curr_conn: connection = conn or db_connect(errors=errors,
+                                               logger=logger)
+
+    # make sure to have a data file
+    data_file: Path = Path(lob_file) if isinstance(lob_file, str | Path) else lob_file
+
+    # normalize the chunk size
+    if not chunk_size:
+        chunk_size = -1
+
+    # build the UPDATE query
+    where_clause: str = " AND ".join([f"{column} = %s" for column in pk_columns])
+    update_stmt: str = (f"UPDATE {lob_table} "
+                        f"SET {lob_column} = %s "
+                        f"WHERE {where_clause}")
+
+    err_msg: str | None = None
+    try:
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+
+            # retrieve the lob data from file in chunks and write to the file
+            lob_data : bytes
+            with data_file.open("rb") as file:
+                lob_data = file.read(chunk_size)
+                while lob_data:
+                    cursor.execute(statement=update_stmt,
+                                   parameters=(Binary(lob_data), *pk_vals))
+                    lob_data = file.read(chunk_size)
+
+        # commit the transaction
+        curr_conn.commit()
+    except Exception as e:
+        curr_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
+
+    # log the results
+    _db_log(errors=errors,
+            err_msg=err_msg,
+            logger=logger,
+            query_stmt=update_stmt,
+            bind_vals=pk_vals)
+
+
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
-               conn: Connection,
+               conn: connection,
                logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
@@ -286,29 +494,30 @@
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
+    curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
-            cursor.execute(exc_stmt, bind_vals)
+            cursor.execute(query=f"{exc_stmt};",
+                           vars=bind_vals)
             result = cursor.rowcount
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
@@ -316,55 +525,55 @@
             logger=logger,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
+
 def db_call_procedure(errors: list[str],
                       proc_name: str,
                       proc_vals: tuple,
-                      conn: Connection,
-                      logger: Logger = None) -> list[tuple]:
+                      conn: connection,
+                      logger: Logger) -> list[tuple]:
     """
-    Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
+    Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
 
-    :param errors: incidental error messages
-    :param proc_name: name of the stored procedure
-    :param proc_vals: parameters for the stored procedure
+    :param errors:  incidental error messages
+    :param proc_name: the name of the sotred procedure
+    :param proc_vals: the arguments to be passed
     :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
-    result: list[tuple] | None = None
+    result: list[tuple] = [()]
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
+    curr_conn: connection = conn or db_connect(errors=errors,
                                                logger=logger)
 
     # build the command
-    proc_stmt: str | None = None
+    proc_stmt: str = f"{proc_name}(" + "%s, " * (len(proc_vals) - 1) + "%s)"
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
-        # obtain a cursor and execute the operation
+        # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
-            cursor.execute(proc_stmt, proc_vals)
+            cursor.execute(query=proc_stmt,
+                           argslist=proc_vals)
             # retrieve the returned tuples
-            rows: list[Row] = cursor.fetchall()
-            result = [tuple(row) for row in rows]
+            result = list(cursor)
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
+                                 engine="postgres")
     finally:
         # close the connection, if locally acquired
         if not conn:
             curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
```

### Comparing `pypomes_db-0.5.4/LICENSE` & `pypomes_db-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.4/pyproject.toml` & `pypomes_db-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.5.4/PKG-INFO` & `pypomes_db-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.5.4
+Version: 0.5.5
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


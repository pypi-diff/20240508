# Comparing `tmp/ehdtd-0.2.0.tar.gz` & `tmp/ehdtd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd-0.2.0.tar", max compression
+gzip compressed data, was "ehdtd-0.2.1.tar", max compression
```

## Comparing `ehdtd-0.2.0.tar` & `ehdtd-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.2.0/LICENSE
--rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.2.0/README.md
--rw-r--r--   0        0        0      952 2024-04-12 05:36:22.441712 ehdtd-0.2.0/ehdtd/__init__.py
--rw-r--r--   0        0        0    23764 2024-04-07 11:48:58.674464 ehdtd-0.2.0/ehdtd/binance.py
--rw-r--r--   0        0        0   121539 2024-04-12 05:34:53.319946 ehdtd-0.2.0/ehdtd/ehdtd.py
--rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.2.0/ehdtd/ehdtd_common_functions.py
--rw-r--r--   0        0        0      683 2024-04-12 05:41:00.397957 ehdtd-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.2.1/README.md
+-rw-r--r--   0        0        0      952 2024-04-12 05:36:22.441712 ehdtd-0.2.1/ehdtd/__init__.py
+-rw-r--r--   0        0        0    23764 2024-04-07 11:48:58.674464 ehdtd-0.2.1/ehdtd/binance.py
+-rw-r--r--   0        0        0   121687 2024-05-08 04:30:39.346014 ehdtd-0.2.1/ehdtd/ehdtd.py
+-rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.2.1/ehdtd/ehdtd_common_functions.py
+-rw-r--r--   0        0        0      705 2024-05-08 04:32:31.702555 ehdtd-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.2.1/PKG-INFO
```

### Comparing `ehdtd-0.2.0/LICENSE` & `ehdtd-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.0/README.md` & `ehdtd-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.0/ehdtd/__init__.py` & `ehdtd-0.2.1/ehdtd/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.0/ehdtd/binance.py` & `ehdtd-0.2.1/ehdtd/binance.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.0/ehdtd/ehdtd.py` & `ehdtd-0.2.1/ehdtd/ehdtd.py`

 * *Files 0% similar despite different names*

```diff
@@ -513,15 +513,15 @@
             next_year = year + 1
 
             time_ini = int(datetime.datetime(year, 1, 1, 0, 0, 0,\
                                              tzinfo=datetime.timezone.utc).timestamp())
             time_end = int(datetime.datetime(next_year, 1, 1, 0, 0, 0,\
                                              tzinfo=datetime.timezone.utc).timestamp())
 
-            if exists_partition is not None and exists_partition is False:
+            if exists_partition is not None and not exists_partition:
                 if self.__db_type == 'postgresql':
 
                     sql_query = "CREATE TABLE " + str(partition_name)\
                         + " PARTITION OF " + str(table_name)\
                         + " FOR VALUES FROM (" + str(time_ini) + ") TO (" + str(time_end) + ") ;"
 
                 elif self.__db_type == 'mysql':
@@ -1254,14 +1254,15 @@
             db_conn_local = self.__db_engine.connect()
 
         table_name = self.__get_table_name(symbol, interval)
         column_open_time = 'open_time'
         column_open_date = 'open_date'
         column_close_time = 'close_time'
         column_close_date = 'close_date'
+        column_volume = 'volume'
         column_status = 'status'
 
         last_open_time_in_db = self.get_last_open_time_in_db(symbol, interval, db_conn_local)
         time_ini = int(time.time_ns())
 
         table = sqlalchemy.Table(table_name, self.__db_metadata, autoload_with=db_conn_local)
 
@@ -1293,15 +1294,16 @@
             stmt = None
 
             try:
                 stmt = sqlalchemy.select(sqlalchemy.column(column_open_time),\
                                          sqlalchemy.column(column_close_time),\
                                          sqlalchemy.column(column_status),\
                                          sqlalchemy.column(column_open_date),\
-                                         sqlalchemy.column(column_close_date))\
+                                         sqlalchemy.column(column_close_date),\
+                                         sqlalchemy.column(column_volume))\
                                          .select_from(sqlalchemy.table(table_name))\
                                          .where(sqlalchemy.column(column_open_time) >= start_from)\
                                          .order_by(sqlalchemy.column(column_open_time).asc())\
                                          .offset(offset).limit(limit_local)
 
 
                 results = db_conn_local.execute(stmt).fetchall()
@@ -1323,23 +1325,24 @@
 
                     if interval == '1mo':
                         __year, __month, __day = Ehdtd.get_ymd_from_time(int(fila[0]))
                         __delta_seconds = (
                             Ehdtd.get_delta_seconds_for_interval(interval, __year, __month)
                         )
 
-                    elif i >= 0:
+                    if i >= 0:
                         if i == last_index:
                             if i == last_open_time_in_db:
                                 status = '__NON_CHECK__'
                             else:
                                 status = fila[2]
 
                         elif fila[1] == results[i+1][0]\
-                            and __delta_seconds == (fila[1] - fila[0]):
+                            and __delta_seconds == (fila[1] - fila[0])\
+                            and fila[5] != 0:
                             status = '__OK__'
                         else:
                             status = '__ERROR__'
 
                     if status == '__ERROR__':
                         result_counter = result_counter + 1
```

### Comparing `ehdtd-0.2.0/ehdtd/ehdtd_common_functions.py` & `ehdtd-0.2.1/ehdtd/ehdtd_common_functions.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.2.0/pyproject.toml` & `ehdtd-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd"
-version = "0.2.0"
+version = "0.2.1"
 description = "Ehdtd - cryptoCurrency Exchange history data to database"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/rmalvarezkai/ehdtd"
 
 [tool.poetry.dependencies]
@@ -20,11 +20,12 @@
 pandas = "^2.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.0.2"
 pytest = "^7.4.3"
 pytest-xdist = "^3.5.0"
+ipykernel = "^6.29.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ehdtd-0.2.0/PKG-INFO` & `ehdtd-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ehdtd - cryptoCurrency Exchange history data to database
 Home-page: https://github.com/rmalvarezkai/ehdtd
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


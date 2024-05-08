# Comparing `tmp/clickhousepandaswrapper-1.1.0.tar.gz` & `tmp/clickhousepandaswrapper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhousepandaswrapper-1.1.0.tar", last modified: Wed May  1 01:51:23 2024, max compression
+gzip compressed data, was "clickhousepandaswrapper-1.1.1.tar", last modified: Wed May  8 02:33:42 2024, max compression
```

## Comparing `clickhousepandaswrapper-1.1.0.tar` & `clickhousepandaswrapper-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 01:51:20.000000 clickhousepandaswrapper-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 01:51:20.000000 clickhousepandaswrapper-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 01:51:20.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-01 01:51:20.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper/insert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-01 01:51:23.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-01 01:51:23.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:51:23.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 01:51:23.000000 clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-01 01:51:21.000000 clickhousepandaswrapper-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 01:51:23.678708 clickhousepandaswrapper-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:33:42.977073 clickhousepandaswrapper-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-08 02:33:36.000000 clickhousepandaswrapper-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-08 02:33:42.977073 clickhousepandaswrapper-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 02:33:36.000000 clickhousepandaswrapper-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:33:42.977073 clickhousepandaswrapper-1.1.1/clickhousePandasWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 02:33:36.000000 clickhousepandaswrapper-1.1.1/clickhousePandasWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17323 2024-05-08 02:33:36.000000 clickhousepandaswrapper-1.1.1/clickhousePandasWrapper/insert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:33:42.977073 clickhousepandaswrapper-1.1.1/clickhousePandasWrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-08 02:33:42.000000 clickhousepandaswrapper-1.1.1/clickhousePandasWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 02:33:42.000000 clickhousepandaswrapper-1.1.1/clickhousePandasWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:33:42.000000 clickhousepandaswrapper-1.1.1/clickhousePandasWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 02:33:42.000000 clickhousepandaswrapper-1.1.1/clickhousePandasWrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-08 02:33:40.000000 clickhousepandaswrapper-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:33:42.977073 clickhousepandaswrapper-1.1.1/setup.cfg
```

### Comparing `clickhousepandaswrapper-1.1.0/LICENSE` & `clickhousepandaswrapper-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhousepandaswrapper-1.1.0/PKG-INFO` & `clickhousepandaswrapper-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhousePandasWrapper
-Version: 1.1.0
+Version: 1.1.1
 Author-email: Grigory Efimov <grigory.efimov@gmail.com>
 Maintainer-email: Grigory Efimov <grigory.efimov@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Grigory Efimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clickhousepandaswrapper-1.1.0/clickhousePandasWrapper/insert.py` & `clickhousepandaswrapper-1.1.1/clickhousePandasWrapper/insert.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,49 @@
 import logging
 import re
 import inspect
 import pandas as pd
 import clickhouse_driver
+import json
 
-columnTypeMap = {
+pandasTypeToClickhouseTypeMap = {
+    'uint8': 'UInt8',
+    'uint16': 'UInt16',
+    'uint32': 'UInt32',
+    'uint64': 'UInt64',
+    'int8': 'Int8',
+    'int16': 'Int16',
+    'int32': 'Int32',
+    'int64': 'Int64',
+    'float16': 'Float32',
+    'float32': 'Float32',
+    'float64': 'Float64',
+    'float128': 'Float64',
+    'object': 'String',
+    'datetime64[D]': 'Date',
+    'datetime64[ns]': 'DateTime',
+    'bool': 'Bool',
+}
+clickhouseTypeToPandasTypeMap = {
+    'UInt8': 'uint8',
+    'UInt16': 'uint16',
+    'UInt32': 'uint32',
+    'UInt64': 'uint64',
+    'Int8': 'int8',
+    'Int16': 'int16',
+    'Int32': 'int32',
+    'Int64': 'int64',
+    'Float32': 'float32',
+    'Float64': 'float64',
+    'String': 'object',
+    'Date': 'datetime64[D]',
+    'DateTime': 'datetime64[ns]',
+    'Bool': 'bool',
+}
+columnNameToTypeMap = {
     'Date': 'DateTime64(3)',
     'date': 'DateTime64(3)',
 }
 
 class Insert():
     """
     init class
@@ -21,28 +56,41 @@
 clickhouseInserter = clickhousePandasWrapper.Insert(host='127.0.0.1', port='9000', db='default')
 ```
     insert data
 ```
 clickhouseInserter.insertDataInClickhouse(df=df,table='test')
 ```
     """
-    def __init__(self, host='127.0.0.1', port=9000, db='default', columnTypeMap=columnTypeMap, logLevel=None):
+    def __init__(self,
+        host = '127.0.0.1',
+        port = 9000,
+        db = 'default',
+        columnTypeMap = None, # backward compatibility, new variable columnNameToTypeMap
+        columnNameToTypeMap = columnNameToTypeMap,
+        logLevel = None,
+        pandasTypeToClickhouseTypeMap = pandasTypeToClickhouseTypeMap,
+        clickhouseTypeToPandasTypeMap = clickhouseTypeToPandasTypeMap,
+    ):
         self.logger = logging.getLogger(__name__)
         if logLevel:
             if re.match(r"^(warn|warning)$", logLevel, re.IGNORECASE):
                 self.logger.setLevel(logging.WARNING)
             elif re.match(r"^debug$", logLevel, re.IGNORECASE):
                 self.logger.setLevel(logging.DEBUG)
             else:
                 self.logger.setLevel(logging.INFO)
         args = locals()
         for argName, argValue in args.items():
             if argName != 'self':
                 setattr(self, argName, argValue)
 
+        # backward compatibility
+        if columnTypeMap:
+            self.columnNameToTypeMap = columnTypeMap
+
         # create clickhouse client connect
         self.ch = clickhouse_driver.Client(
             host=self.host,
             port=self.port,
         )
         self.logger.debug(f"created clickhouse client connect: host={self.host}, port={self.port}, db={self.db}")
         self.createDatabase()
@@ -68,37 +116,29 @@
 
     def pandasToClickhouseType(self, columnName, pandasType):
         """
         matching data type from pandas to clickhouse
         """
 
         defName = inspect.stack()[0][3]
-        mapping = {
-            'int32': 'Int32',
-            'int64': 'Int64',
-            'float32': 'Float32',
-            'float64': 'Float64',
-            'bool': 'Bool',
-            'object': 'String',
-        }
-        if columnName in self.columnTypeMap:
+        if columnName in self.columnNameToTypeMap:
             # define type by column name
-            return self.columnTypeMap.get(columnName)
+            return self.columnNameToTypeMap.get(columnName)
         else:
             # define type by pandas types
-            return mapping.get(str(pandasType), 'String')
+            return self.pandasTypeToClickhouseTypeMap.get(str(pandasType), 'String')
 
     def generateCreateTableQuery(self, df, db, table, engine = 'MergeTree', partitionBy = None, orderBy = None, primaryKey = None, settings = 'index_granularity = 8192'):
         """
         generate create table query
         """
 
         defName = inspect.stack()[0][3]
 
-        self.logger.debug(f"{defName}: dtypes={df.dtypes}")
+        self.logger.debug(f"{defName}: df.dtypes='{df.dtypes}'")
         self.logger.debug(f"{defName}: df.sample='{self.dfSample(df)}'")
         columnDefinitions = []
         columnsStr = ''
         for columnName, dtype in df.dtypes.items():
             chType = self.pandasToClickhouseType(columnName,dtype)
             columnDefinitions.append(f"{columnName} {chType}")
             if columnsStr:
@@ -191,14 +231,56 @@
             self.logger.debug(f"{defName}: sql='{sql}'")
             try:
                 self.ch.execute(sql)
             except Exception as e:
                 raise Exception(f"{defName}: failed execute in clickhouse, sql={sql}: host={self.host}, port={self.port}, db={db}, table={table}, error='{str(e)}'")
         return None
 
+    def syncDataTypes(self,df,table,db):
+        """
+        Sync data types from clickhouse table to dataframe.
+        When working with small-sized dataframes, it often happens that the data type changes drastically.
+        For example, one dataframe might contain a float, while the next one might have None (string).
+        """
+
+        defName = inspect.stack()[0][3]
+        self.logger.debug(f"{defName}: sync data types from clickhouse to df: host={self.host}, port={self.port}, db={db}, table={table}")
+        query = f"DESCRIBE TABLE {db}.{table}"
+        try:
+            columnsInfo = self.ch.execute(query)
+        except Exception as e:
+            raise Exception(f"{defName}: failed execute: query='{query}' host={self.host}, port={self.port}, db={db}, table={table}")
+
+        for columnInfo in columnsInfo:
+            chColumnName = columnInfo[0]
+            chColumnType = columnInfo[1]
+            dfColumntType = self.clickhouseTypeToPandasTypeMap.get(chColumnType, 'object')
+            if chColumnName in df.columns:
+                # convert arrays to string
+                if df[chColumnName].apply(lambda x: isinstance(x, list)).any():
+                    self.logger.debug(f"{defName}: chColumnName={chColumnName} convert list to string")
+                    df[chColumnName] = df[chColumnName].astype("string")
+
+                # None not possible value for int\float types
+                if dfColumntType in ['int8', 'int16', 'int32', 'int64', 'uint8', 'uint16', 'uint32', 'uint64', 'float16', 'float32', 'float64']:
+                    df[chColumnName] = df[chColumnName].fillna(0)
+
+                # fix astype for String
+                if chColumnType == 'String':
+                    df[chColumnName] = df[chColumnName].astype("string")
+
+                # try convert astype for df
+                try:
+                    self.logger.debug(f"{defName}: set astype={dfColumntType}, chColumnName={chColumnName}, chColumnType={chColumnType}")
+                    df[chColumnName] = df[chColumnName].astype(dfColumntType)
+                except Exception as e:
+                    raise Exception(f"{defName}: failed run astype. chColumnName='{chColumnName}', chColumnType='{chColumnType}', dfColumntType='{dfColumntType}', dfValues='{df[chColumnName].to_string()}', error='{str(e)}'")
+
+        return df
+
     def insertDataInClickhouse(self,
             df,
             table,
             db=None,
             cleanDataInDateRange=True,
             cleanDataWhereColumns=list(),
             cleanAllData=False,
@@ -300,26 +382,29 @@
         for column in df.columns.values.tolist():
             if columnsString:
                 columnsString = columnsString +","
             columnsString = columnsString +"`"+ column +"`"
         insertString = 'INSERT INTO %s.%s (%s) VALUES' % (db,table,columnsString)
         self.logger.debug(insertString)
 
-        # convert df type objects to string
-        objectColumns = df.select_dtypes(include=[object]).columns
-        df[objectColumns] = df[objectColumns].astype(str)
+        # sync data typs from clickhouse to df
+        df = self.syncDataTypes(df,table,db)
 
         try:
             self.ch.insert_dataframe(
                 insertString,
                 df,
                 settings={ "use_numpy": True },
             )
         except Exception as e:
-            self.logger.warning(f"{defName}: failed insert error={str(e)}")
+            pd.set_option('display.max_rows', None)
+            pd.set_option('display.max_columns', None)
+            self.logger.warning(f"{defName}: failed insert error='{str(e)}'")
+            self.logger.warning(f"{defName}: df.dtypes='{df.dtypes}'")
+            self.logger.warning(f"{defName}: df='{json.dumps(json.loads(df.to_json(orient='table')), indent=4)}'")
             if e.code == 16: # NO_SUCH_COLUMN_IN_TABLE https://github.com/mymarilyn/clickhouse-driver/blob/master/clickhouse_driver/errors.py#L17
                 self.logger.warning(f"{defName}: schema in clickhouse table does not match df schema: host={self.host}, port={self.port}, db={db}, table={table}'")
                 self.syncTableSchema(df,table,db)
                 # retry
                 if retryCounter >= 1:
                     raise Exception(f"{defName}: failed insert_dataframe in clickhouse: host={self.host}, port={self.port}, db={db}, table={table}, error='{str(e)}'")
                 else:
```

### Comparing `clickhousepandaswrapper-1.1.0/clickhousePandasWrapper.egg-info/PKG-INFO` & `clickhousepandaswrapper-1.1.1/clickhousePandasWrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhousePandasWrapper
-Version: 1.1.0
+Version: 1.1.1
 Author-email: Grigory Efimov <grigory.efimov@gmail.com>
 Maintainer-email: Grigory Efimov <grigory.efimov@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Grigory Efimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


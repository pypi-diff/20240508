# Comparing `tmp/beetl-0.4.8.tar.gz` & `tmp/beetl-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beetl-0.4.8.tar", last modified: Fri May  3 15:06:05 2024, max compression
+gzip compressed data, was "beetl-0.4.9.tar", last modified: Wed May  8 10:10:33 2024, max compression
```

## Comparing `beetl-0.4.8.tar` & `beetl-0.4.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:06:05.088682 beetl-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 15:06:05.088682 beetl-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-03 15:05:27.000000 beetl-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:06:05.088682 beetl-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-03 15:05:27.000000 beetl-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:06:05.084682 beetl-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:06:05.084682 beetl-0.4.8/src/beetl/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/beetl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:06:05.088682 beetl-0.4.8/src/beetl/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/sqlserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/sources/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:06:05.088682 beetl-0.4.8/src/beetl/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/transformers/frames.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/transformers/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/transformers/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/transformers/itop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/transformers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/transformers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/transformers/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-03 15:05:27.000000 beetl-0.4.8/src/beetl/transformers/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:06:05.088682 beetl-0.4.8/src/beetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-03 15:06:05.000000 beetl-0.4.8/src/beetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 15:06:05.000000 beetl-0.4.8/src/beetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:06:05.000000 beetl-0.4.8/src/beetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 15:06:05.000000 beetl-0.4.8/src/beetl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-03 15:06:05.000000 beetl-0.4.8/src/beetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 15:06:05.000000 beetl-0.4.8/src/beetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:06:05.000000 beetl-0.4.8/src/beetl.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:10:33.228185 beetl-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-08 10:10:33.228185 beetl-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-08 10:09:54.000000 beetl-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:10:33.228185 beetl-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-08 10:09:54.000000 beetl-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:10:33.224185 beetl-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:10:33.224185 beetl-0.4.9/src/beetl/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/beetl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:10:33.228185 beetl-0.4.9/src/beetl/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/sqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/sources/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:10:33.228185 beetl-0.4.9/src/beetl/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/transformers/frames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/transformers/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/transformers/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/transformers/itop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/transformers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/transformers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/transformers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-08 10:09:54.000000 beetl-0.4.9/src/beetl/transformers/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:10:33.228185 beetl-0.4.9/src/beetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-08 10:10:33.000000 beetl-0.4.9/src/beetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 10:10:33.000000 beetl-0.4.9/src/beetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:10:33.000000 beetl-0.4.9/src/beetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 10:10:33.000000 beetl-0.4.9/src/beetl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 10:10:33.000000 beetl-0.4.9/src/beetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 10:10:33.000000 beetl-0.4.9/src/beetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:10:33.000000 beetl-0.4.9/src/beetl.egg-info/zip-safe
```

### Comparing `beetl-0.4.8/PKG-INFO` & `beetl-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.8
+Version: 0.4.9
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beetl-0.4.8/README.md` & `beetl-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/setup.py` & `beetl-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/__version__.py` & `beetl-0.4.9/src/beetl/__version__.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/beetl.py` & `beetl-0.4.9/src/beetl/beetl.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/config.py` & `beetl-0.4.9/src/beetl/config.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/sources/faker.py` & `beetl-0.4.9/src/beetl/sources/faker.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/sources/interface.py` & `beetl-0.4.9/src/beetl/sources/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/sources/itop.py` & `beetl-0.4.9/src/beetl/sources/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/sources/mongodb.py` & `beetl-0.4.9/src/beetl/sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/sources/mysql.py` & `beetl-0.4.9/src/beetl/sources/mysql.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/sources/postgres.py` & `beetl-0.4.9/src/beetl/sources/postgres.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/sources/rest.py` & `beetl-0.4.9/src/beetl/sources/rest.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/sources/sqlserver.py` & `beetl-0.4.9/src/beetl/sources/sqlserver.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/sources/static.py` & `beetl-0.4.9/src/beetl/sources/static.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/transformers/frames.py` & `beetl-0.4.9/src/beetl/transformers/frames.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/transformers/integer.py` & `beetl-0.4.9/src/beetl/transformers/misc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 import polars as pl
 from .interface import TransformerInterface, register_transformer_class
 
-@register_transformer_class("int")
-class IntegerTransformer(TransformerInterface):
+
+def dn_to_samaccountname(dn):
+    return dn.split(",")[0].split("=")[1]
+
+
+@register_transformer_class("misc")
+class MiscTransformer(TransformerInterface):
     @staticmethod
-    def divide(data: pl.DataFrame, inField: str, outField: str, factor: int, inType: str = "Int64", outType: str = "Int32") -> pl.DataFrame:
-        """Divide the numbers in a given column with the given factor to a rounded integer
+    def sam_from_dn(
+        data: pl.DataFrame, inField: str, outField: str = None
+    ) -> pl.DataFrame:
+        """Get the SAM account name from a distinguished name
 
         Args:
-            data (pl.DataFrame): The dataFrame to modify
-            inField (str): The field to process
-            outField (str): The field to put the output into
-            factor (int): The field to divide by
+            data (pl.DataFrame): The data to be modified
+            inField (str): The field to work on
+            outField (str, optional): The field to add/replace. Defaults to None.
 
         Returns:
-            pl.DataFrame: The resulting DataFrame
+            pl.DataFrame: Dataframe with the modified column
         """
-        inType = getattr(pl, inType)
-        outType = getattr(pl, outType)
-        
-        data = data.with_columns((data[inField].cast(inType) / factor).round(0).cast(outType).alias(outField))
-        
-        return data
+
+        data = data.with_columns(
+            data[inField]
+            .str.splitn(",", 2)
+            .struct.unnest()["field_0"]
+            .str.splitn("=", 2)
+            .struct.unnest()["field_1"]
+            .alias(outField if outField is not None else inField)
+        )
+
+        return data
```

### Comparing `beetl-0.4.8/src/beetl/transformers/interface.py` & `beetl-0.4.9/src/beetl/transformers/interface.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/transformers/itop.py` & `beetl-0.4.9/src/beetl/transformers/itop.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/transformers/regex.py` & `beetl-0.4.9/src/beetl/transformers/regex.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl/transformers/strings.py` & `beetl-0.4.9/src/beetl/transformers/strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,28 +37,28 @@
         """
         __class__._validate_fields(data.columns, inField)
         
         data = data.with_columns(data[inField].fill_null(defaultValue))
         return data
 
     @staticmethod
-    def strip(data: pl.DataFrame, inField: str, stripChars: str) -> pl.DataFrame:
+    def strip(data: pl.DataFrame, inField: str, stripChars: str, outField: str = None) -> pl.DataFrame:
         """Strip all given characters from a column
 
         Args:
             data (pl.DataFrame): The dataFrame to modify
             inField (str): The field to process
             stripChar (str): The character to strip
 
         Returns:
             pl.DataFrame: The resulting DataFrame
         """
         __class__._validate_fields(data.columns, inField)
 
-        data = data.with_columns(data[inField].str.strip(stripChars))
+        data = data.with_columns(data[inField].str.strip(stripChars).alias(outField if outField is not None else inField))
         return data
 
     @staticmethod
     def lowercase(data: pl.DataFrame, inField: str = "", outField: str = "", inOutMap: dict = {}) -> pl.DataFrame:
         """Transform all values in a column to lowercase and insert
             them into another (or the same) column
 
@@ -175,8 +175,15 @@
         return data.with_columns(data[inField].str.replace(search, replace).alias(outField if outField is not None else inField))
                                  
     @staticmethod
     def replace_all(data: pl.DataFrame, search: str, replace: str, inField: str, outField: str = None):
         """Replace all matching sections in a string with another section"""
 
         return data.with_columns(data[inField].str.replace_all(search, replace).alias(outField if outField is not None else inField))
+
+    @staticmethod
+    def substring(data: pl.DataFrame, inField: str, outField: str = None, start: int = 0, length: int = None):
+        """Returns a substring of the given string column"""
+
+        return data.with_columns(data[inField].str.slice(start, length).alias(outField if outField is not None else inField))
+
```

### Comparing `beetl-0.4.8/src/beetl/transformers/structs.py` & `beetl-0.4.9/src/beetl/transformers/structs.py`

 * *Files identical despite different names*

### Comparing `beetl-0.4.8/src/beetl.egg-info/PKG-INFO` & `beetl-0.4.9/src/beetl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beetl
-Version: 0.4.8
+Version: 0.4.9
 Summary: BeETL is a Python package for extracting data from one datasource, 
 Home-page: https://github.com/Hoglandets-IT/beetl
 Author: Lars Scheibling
 Author-email: lars.scheibling@hoglandet.se
 License: GnuPG 3.0
 Keywords: python template package module cli
 Classifier: Programming Language :: Python :: 3
```

### Comparing `beetl-0.4.8/src/beetl.egg-info/SOURCES.txt` & `beetl-0.4.9/src/beetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*


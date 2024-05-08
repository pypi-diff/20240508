# Comparing `tmp/dq_check-0.1.0.tar.gz` & `tmp/dq_check-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dq_check-0.1.0.tar", last modified: Tue May  7 04:19:09 2024, max compression
+gzip compressed data, was "dq_check-0.2.0.tar", last modified: Wed May  8 05:11:18 2024, max compression
```

## Comparing `dq_check-0.1.0.tar` & `dq_check-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-07 04:19:09.958976 dq_check-0.1.0/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2342 2024-05-07 04:19:09.958613 dq_check-0.1.0/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2103 2024-05-07 04:16:06.000000 dq_check-0.1.0/README.md
--rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-07 04:18:56.000000 dq_check-0.1.0/pyproject.toml
--rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-07 04:19:09.959925 dq_check-0.1.0/setup.cfg
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-07 04:19:09.950766 dq_check-0.1.0/src/
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-07 04:19:09.953648 dq_check-0.1.0/src/dq_check/
--rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.1.0/src/dq_check/__init__.py
--rw-r--r--   0 rohan.goel   (502) staff       (20)    15293 2024-05-06 04:54:08.000000 dq_check-0.1.0/src/dq_check/dq_check.py
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-07 04:19:09.957803 dq_check-0.1.0/src/dq_check.egg-info/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2342 2024-05-07 04:19:09.000000 dq_check-0.1.0/src/dq_check.egg-info/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-07 04:19:09.000000 dq_check-0.1.0/src/dq_check.egg-info/SOURCES.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-07 04:19:09.000000 dq_check-0.1.0/src/dq_check.egg-info/dependency_links.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-07 04:19:09.000000 dq_check-0.1.0/src/dq_check.egg-info/requires.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-07 04:19:09.000000 dq_check-0.1.0/src/dq_check.egg-info/top_level.txt
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-08 05:11:18.555849 dq_check-0.2.0/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2408 2024-05-08 05:11:18.555546 dq_check-0.2.0/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2169 2024-05-07 14:36:16.000000 dq_check-0.2.0/README.md
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-08 05:09:36.000000 dq_check-0.2.0/pyproject.toml
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-08 05:11:18.556427 dq_check-0.2.0/setup.cfg
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-08 05:11:18.546672 dq_check-0.2.0/src/
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-08 05:11:18.550401 dq_check-0.2.0/src/dq_check/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.2.0/src/dq_check/__init__.py
+-rw-r--r--   0 rohan.goel   (502) staff       (20)    10728 2024-05-08 05:09:04.000000 dq_check-0.2.0/src/dq_check/dq_check.py
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-08 05:11:18.554590 dq_check-0.2.0/src/dq_check.egg-info/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2408 2024-05-08 05:11:18.000000 dq_check-0.2.0/src/dq_check.egg-info/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-08 05:11:18.000000 dq_check-0.2.0/src/dq_check.egg-info/SOURCES.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-08 05:11:18.000000 dq_check-0.2.0/src/dq_check.egg-info/dependency_links.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-08 05:11:18.000000 dq_check-0.2.0/src/dq_check.egg-info/requires.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-08 05:11:18.000000 dq_check-0.2.0/src/dq_check.egg-info/top_level.txt
```

### Comparing `dq_check-0.1.0/PKG-INFO` & `dq_check-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: dq_check
-Version: 0.1.0
-Summary: A data quality check module for Spark
-Author-email: rohan goel <rohan.goel@databricks.com>
-Description-Content-Type: text/markdown
-Requires-Dist: pyspark
-Requires-Dist: pandas
-
 ## dq_check
 
 
 ## Overview
 
 `dq_check` is a Python package that provides a data quality check function encapsulated in the `DQCheck` class. It allows you to perform data quality checks on tables using SQL queries and save the results into a Delta table for auditing purposes.
 
@@ -31,38 +22,52 @@
 
 
 ## Usage
 
 Here's an example of how to use the DQCheck class from the dq_check package:
 
 from pyspark.sql import SparkSession
+
 from dq_check import DQCheck
 
 ## Initialize Spark session
 spark = SparkSession.builder.appName("DQCheckExample").getOrCreate()
 
 ## Create an instance of DQCheck
-dq_checker = DQCheck(spark)
+
+dq_checker = DQCheck(spark,audit_table) #audit table name should have catalog and schema.
 
 ## Define the data quality check parameters
+
 table_type = "delta"  # Type of the table ('delta' or 'asql')
-table_name = "your_table_name"  # Name of the table
+
+table_name = "your_table_name"  # Name of the table, should have catalog/schema for delta and schema for asql.
+
 primary_keys = ["your_primary_key"]  # List of primary key columns
-sql_query = "SELECT * FROM your_table WHERE condition"  # Data quality check query
+
+sql_query = "SELECT * FROM your_table WHERE condition"  # Data quality check query # should have table name with catalog and schema.
 
 ## Perform the data quality check
 dq_checker.perform_dq_check(
+
     table_type,
+
     table_name,
+
     primary_keys,
+
     sql_query,
-    quality_threshold_percentage=5,  # Quality threshold percentage
+
+    secret= None, # Optional, required for asql only
+
     data_batch_identifier_name=None,  # Optional batch identifier name
+
     data_batch_identifier_value=None,  # Optional batch identifier value
-    audit_table_name="your_audit_log_table"  # Name of the Delta table to store audit logs
+
+    quality_threshold_percentage=5,  # Quality threshold percentage
 )
 
 
 ## Configuration
 
 Adjust the parameters passed to the perform_dq_check method based on your requirements.
 
@@ -72,11 +77,11 @@
 Pandas
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues and pull requests on the GitHub repository.
 
 ## License
-This project is licensed under the MIT License. See the LICENSE file for more details.
+None.
 
 ## Contact
-For any questions or feedback, open a github issue
+For any questions or feedback, open a github issue
```

### Comparing `dq_check-0.1.0/README.md` & `dq_check-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: dq_check
+Version: 0.2.0
+Summary: A data quality check module for Spark
+Author-email: rohan goel <rohan.goel@databricks.com>
+Description-Content-Type: text/markdown
+Requires-Dist: pyspark
+Requires-Dist: pandas
+
 ## dq_check
 
 
 ## Overview
 
 `dq_check` is a Python package that provides a data quality check function encapsulated in the `DQCheck` class. It allows you to perform data quality checks on tables using SQL queries and save the results into a Delta table for auditing purposes.
 
@@ -22,38 +31,52 @@
 
 
 ## Usage
 
 Here's an example of how to use the DQCheck class from the dq_check package:
 
 from pyspark.sql import SparkSession
+
 from dq_check import DQCheck
 
 ## Initialize Spark session
 spark = SparkSession.builder.appName("DQCheckExample").getOrCreate()
 
 ## Create an instance of DQCheck
-dq_checker = DQCheck(spark)
+
+dq_checker = DQCheck(spark,audit_table) #audit table name should have catalog and schema.
 
 ## Define the data quality check parameters
+
 table_type = "delta"  # Type of the table ('delta' or 'asql')
-table_name = "your_table_name"  # Name of the table
+
+table_name = "your_table_name"  # Name of the table, should have catalog/schema for delta and schema for asql.
+
 primary_keys = ["your_primary_key"]  # List of primary key columns
-sql_query = "SELECT * FROM your_table WHERE condition"  # Data quality check query
+
+sql_query = "SELECT * FROM your_table WHERE condition"  # Data quality check query # should have table name with catalog and schema.
 
 ## Perform the data quality check
 dq_checker.perform_dq_check(
+
     table_type,
+
     table_name,
+
     primary_keys,
+
     sql_query,
-    quality_threshold_percentage=5,  # Quality threshold percentage
+
+    secret= None, # Optional, required for asql only
+
     data_batch_identifier_name=None,  # Optional batch identifier name
+
     data_batch_identifier_value=None,  # Optional batch identifier value
-    audit_table_name="your_audit_log_table"  # Name of the Delta table to store audit logs
+
+    quality_threshold_percentage=5,  # Quality threshold percentage
 )
 
 
 ## Configuration
 
 Adjust the parameters passed to the perform_dq_check method based on your requirements.
 
@@ -63,11 +86,11 @@
 Pandas
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues and pull requests on the GitHub repository.
 
 ## License
-This project is licensed under the MIT License. See the LICENSE file for more details.
+None.
 
 ## Contact
-For any questions or feedback, open a github issue
+For any questions or feedback, open a github issue
```

### Comparing `dq_check-0.1.0/src/dq_check.egg-info/PKG-INFO` & `dq_check-0.2.0/src/dq_check.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.1.0
+Version: 0.2.0
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
@@ -31,38 +31,52 @@
 
 
 ## Usage
 
 Here's an example of how to use the DQCheck class from the dq_check package:
 
 from pyspark.sql import SparkSession
+
 from dq_check import DQCheck
 
 ## Initialize Spark session
 spark = SparkSession.builder.appName("DQCheckExample").getOrCreate()
 
 ## Create an instance of DQCheck
-dq_checker = DQCheck(spark)
+
+dq_checker = DQCheck(spark,audit_table) #audit table name should have catalog and schema.
 
 ## Define the data quality check parameters
+
 table_type = "delta"  # Type of the table ('delta' or 'asql')
-table_name = "your_table_name"  # Name of the table
+
+table_name = "your_table_name"  # Name of the table, should have catalog/schema for delta and schema for asql.
+
 primary_keys = ["your_primary_key"]  # List of primary key columns
-sql_query = "SELECT * FROM your_table WHERE condition"  # Data quality check query
+
+sql_query = "SELECT * FROM your_table WHERE condition"  # Data quality check query # should have table name with catalog and schema.
 
 ## Perform the data quality check
 dq_checker.perform_dq_check(
+
     table_type,
+
     table_name,
+
     primary_keys,
+
     sql_query,
-    quality_threshold_percentage=5,  # Quality threshold percentage
+
+    secret= None, # Optional, required for asql only
+
     data_batch_identifier_name=None,  # Optional batch identifier name
+
     data_batch_identifier_value=None,  # Optional batch identifier value
-    audit_table_name="your_audit_log_table"  # Name of the Delta table to store audit logs
+
+    quality_threshold_percentage=5,  # Quality threshold percentage
 )
 
 
 ## Configuration
 
 Adjust the parameters passed to the perform_dq_check method based on your requirements.
 
@@ -72,11 +86,11 @@
 Pandas
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues and pull requests on the GitHub repository.
 
 ## License
-This project is licensed under the MIT License. See the LICENSE file for more details.
+None.
 
 ## Contact
 For any questions or feedback, open a github issue
```


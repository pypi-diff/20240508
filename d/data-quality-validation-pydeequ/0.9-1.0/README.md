# Comparing `tmp/data-quality-validation-pydeequ-0.9.tar.gz` & `tmp/data-quality-validation-pydeequ-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-quality-validation-pydeequ-0.9.tar", last modified: Tue May  7 08:42:27 2024, max compression
+gzip compressed data, was "data-quality-validation-pydeequ-1.0.tar", last modified: Wed May  8 02:41:53 2024, max compression
```

## Comparing `data-quality-validation-pydeequ-0.9.tar` & `data-quality-validation-pydeequ-1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:42:27.004926 data-quality-validation-pydeequ-0.9/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6286 2024-05-07 08:42:27.004499 data-quality-validation-pydeequ-0.9/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5805 2024-05-07 08:40:56.000000 data-quality-validation-pydeequ-0.9/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:42:27.003877 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6286 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/top_level.txt
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:42:27.002548 data-quality-validation-pydeequ-0.9/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.9/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.9/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.9/dqv/dqv_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 08:42:27.004994 data-quality-validation-pydeequ-0.9/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 08:41:40.000000 data-quality-validation-pydeequ-0.9/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-08 02:41:53.968831 data-quality-validation-pydeequ-1.0/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     7223 2024-05-08 02:41:53.968424 data-quality-validation-pydeequ-1.0/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6711 2024-05-08 02:41:43.000000 data-quality-validation-pydeequ-1.0/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-08 02:41:53.967971 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     7223 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/top_level.txt
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-08 02:41:53.966956 data-quality-validation-pydeequ-1.0/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-1.0/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-1.0/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5358 2024-05-07 16:43:25.000000 data-quality-validation-pydeequ-1.0/dqv/dqv_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-08 02:41:53.968906 data-quality-validation-pydeequ-1.0/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      857 2024-05-08 02:41:51.000000 data-quality-validation-pydeequ-1.0/setup.py
```

### Comparing `data-quality-validation-pydeequ-0.9/PKG-INFO` & `data-quality-validation-pydeequ-1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 0.9
-Summary: A library for data quality validation using PyDeequ.
+Version: 1.0
+Summary: A library for data quality validation using PyDeequ and to send email notification.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -13,15 +13,16 @@
 Requires-Dist: pydeequ
 Requires-Dist: boto3
 Requires-Dist: pyyaml
 
 <span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
 This package is designed for performing data quality validation using PyDeequ.  
-It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.
+It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  
+Also, to send email notification about the validation result.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Ajay Rahul Raja, Ruth Mifsud
 
 This package contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
@@ -96,19 +97,19 @@
 <span style="font-size:11pt; color:green"> **Apache Spark:** </span> [Apache Spark 3.3.0 Release](https://spark.apache.org/releases/spark-release-3-3-0.html)
 
 - Step 2: Install PyDeequ in the terminal if you encounter an error related to "PyDeequ module is not installed on the machine."
 
 <span style="font-size:13pt; color:orange"> **How to install PyDeequ? Use the following command:** </span>  
   `pip install pydeequ`
 
-- step 3: Install our ‘Data Quality Validation’ python library in terminal.  
+- Step 3: Install our ‘Data Quality Validation’ python library in terminal.  
   `pip install data-quality-validation-pydeequ`
 
-- step 4: To run the Data Quality Validation function, import the library as below:  
-  `from dqv.dqv_pydeequ import DqvPydeequ`  
+- Step 4: To run the Data Quality Validation function, import the library as below:  
+  `from dqv.dqv_pydeequ import DqvPydeequ, sendEmailNotification`  
 
 - Step 5: Create a config file in a folder with the columns that need to be validated.  
   Name the file as you wish, but remember to use the name in the DqvPydeequ function.
 
 - Step 6: Upload your data to S3 and save it in a new directory if you are running locally.
 
 - Step 7: Pass your source and target file paths in the DqvPydeequ function.
@@ -118,11 +119,37 @@
         "", #config_file
         "", #source_data_path
         "") #target_data_path
    ```
 
 - Step 8: Run the file to validate.
 
+- Step 9: After validating the data, the result can be sent via email.  
+  For this, import the library as below:  
+  `from email_notification import sendEmailNotification`
+
+- Step 10: save your aws administration imputs, sender email, and region as dictionary.
+  Then pass source path, target path and this config in the sendEmailNotification function.
+
+   ```
+   email_config = {
+    "aws_access_key_id": "", #aws administration
+    "aws_secret_access_key": "", #aws administration
+    "aws_session_token": "", #aws administration
+    "sender_email": "", #sender email
+    "receiver_email": "", #receiver email 
+    "aws_region": "" #region
+    }
+   ```
+
+  ``` 
+   send_notification = sendEmailNotification(
+        "", #source_data_path
+        "", #target_data_path
+        email_config #dictionary
+    )
+   ```  
+
 
 <br></br>
 Refer this repo to follow the structure of config file format  <br></br>
 Git: <a href="https://github.com/dataruk/data-quality-validation">https://github.com/dataruk/data-quality-validation</a>
```

### Comparing `data-quality-validation-pydeequ-0.9/README.md` & `data-quality-validation-pydeequ-1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 <span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
 This package is designed for performing data quality validation using PyDeequ.  
-It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.
+It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  
+Also, to send email notification about the validation result.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Ajay Rahul Raja, Ruth Mifsud
 
 This package contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
@@ -80,19 +81,19 @@
 <span style="font-size:11pt; color:green"> **Apache Spark:** </span> [Apache Spark 3.3.0 Release](https://spark.apache.org/releases/spark-release-3-3-0.html)
 
 - Step 2: Install PyDeequ in the terminal if you encounter an error related to "PyDeequ module is not installed on the machine."
 
 <span style="font-size:13pt; color:orange"> **How to install PyDeequ? Use the following command:** </span>  
   `pip install pydeequ`
 
-- step 3: Install our ‘Data Quality Validation’ python library in terminal.  
+- Step 3: Install our ‘Data Quality Validation’ python library in terminal.  
   `pip install data-quality-validation-pydeequ`
 
-- step 4: To run the Data Quality Validation function, import the library as below:  
-  `from dqv.dqv_pydeequ import DqvPydeequ`  
+- Step 4: To run the Data Quality Validation function, import the library as below:  
+  `from dqv.dqv_pydeequ import DqvPydeequ, sendEmailNotification`  
 
 - Step 5: Create a config file in a folder with the columns that need to be validated.  
   Name the file as you wish, but remember to use the name in the DqvPydeequ function.
 
 - Step 6: Upload your data to S3 and save it in a new directory if you are running locally.
 
 - Step 7: Pass your source and target file paths in the DqvPydeequ function.
@@ -102,11 +103,37 @@
         "", #config_file
         "", #source_data_path
         "") #target_data_path
    ```
 
 - Step 8: Run the file to validate.
 
+- Step 9: After validating the data, the result can be sent via email.  
+  For this, import the library as below:  
+  `from email_notification import sendEmailNotification`
+
+- Step 10: save your aws administration imputs, sender email, and region as dictionary.
+  Then pass source path, target path and this config in the sendEmailNotification function.
+
+   ```
+   email_config = {
+    "aws_access_key_id": "", #aws administration
+    "aws_secret_access_key": "", #aws administration
+    "aws_session_token": "", #aws administration
+    "sender_email": "", #sender email
+    "receiver_email": "", #receiver email 
+    "aws_region": "" #region
+    }
+   ```
+
+  ``` 
+   send_notification = sendEmailNotification(
+        "", #source_data_path
+        "", #target_data_path
+        email_config #dictionary
+    )
+   ```  
+
 
 <br></br>
 Refer this repo to follow the structure of config file format  <br></br>
 Git: <a href="https://github.com/dataruk/data-quality-validation">https://github.com/dataruk/data-quality-validation</a>
```

### Comparing `data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/PKG-INFO` & `data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 0.9
-Summary: A library for data quality validation using PyDeequ.
+Version: 1.0
+Summary: A library for data quality validation using PyDeequ and to send email notification.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -13,15 +13,16 @@
 Requires-Dist: pydeequ
 Requires-Dist: boto3
 Requires-Dist: pyyaml
 
 <span style='color: Pink; font-size:25px'>  **Data Quality Validation** </span>
 
 This package is designed for performing data quality validation using PyDeequ.  
-It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.
+It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  
+Also, to send email notification about the validation result.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Ajay Rahul Raja, Ruth Mifsud
 
 This package contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
@@ -96,19 +97,19 @@
 <span style="font-size:11pt; color:green"> **Apache Spark:** </span> [Apache Spark 3.3.0 Release](https://spark.apache.org/releases/spark-release-3-3-0.html)
 
 - Step 2: Install PyDeequ in the terminal if you encounter an error related to "PyDeequ module is not installed on the machine."
 
 <span style="font-size:13pt; color:orange"> **How to install PyDeequ? Use the following command:** </span>  
   `pip install pydeequ`
 
-- step 3: Install our ‘Data Quality Validation’ python library in terminal.  
+- Step 3: Install our ‘Data Quality Validation’ python library in terminal.  
   `pip install data-quality-validation-pydeequ`
 
-- step 4: To run the Data Quality Validation function, import the library as below:  
-  `from dqv.dqv_pydeequ import DqvPydeequ`  
+- Step 4: To run the Data Quality Validation function, import the library as below:  
+  `from dqv.dqv_pydeequ import DqvPydeequ, sendEmailNotification`  
 
 - Step 5: Create a config file in a folder with the columns that need to be validated.  
   Name the file as you wish, but remember to use the name in the DqvPydeequ function.
 
 - Step 6: Upload your data to S3 and save it in a new directory if you are running locally.
 
 - Step 7: Pass your source and target file paths in the DqvPydeequ function.
@@ -118,11 +119,37 @@
         "", #config_file
         "", #source_data_path
         "") #target_data_path
    ```
 
 - Step 8: Run the file to validate.
 
+- Step 9: After validating the data, the result can be sent via email.  
+  For this, import the library as below:  
+  `from email_notification import sendEmailNotification`
+
+- Step 10: save your aws administration imputs, sender email, and region as dictionary.
+  Then pass source path, target path and this config in the sendEmailNotification function.
+
+   ```
+   email_config = {
+    "aws_access_key_id": "", #aws administration
+    "aws_secret_access_key": "", #aws administration
+    "aws_session_token": "", #aws administration
+    "sender_email": "", #sender email
+    "receiver_email": "", #receiver email 
+    "aws_region": "" #region
+    }
+   ```
+
+  ``` 
+   send_notification = sendEmailNotification(
+        "", #source_data_path
+        "", #target_data_path
+        email_config #dictionary
+    )
+   ```  
+
 
 <br></br>
 Refer this repo to follow the structure of config file format  <br></br>
 Git: <a href="https://github.com/dataruk/data-quality-validation">https://github.com/dataruk/data-quality-validation</a>
```

### Comparing `data-quality-validation-pydeequ-0.9/dqv/data_quality_validation_pydeequ.py` & `data-quality-validation-pydeequ-1.0/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.9/setup.py` & `data-quality-validation-pydeequ-1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 # Reading the README.md file for long description in PyPI site
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='data-quality-validation-pydeequ',
-    version='0.9',
+    version='1.0',
     author='Ketan Kirange',
     author_email='k.kirange@reply.com',
-    description='A library for data quality validation using PyDeequ.',
+    description='A library for data quality validation using PyDeequ and to send email notification.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'pydeequ',
         'boto3',
```


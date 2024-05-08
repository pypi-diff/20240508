# Comparing `tmp/data-quality-validation-pydeequ-0.8.tar.gz` & `tmp/data-quality-validation-pydeequ-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-quality-validation-pydeequ-0.8.tar", last modified: Tue May  7 08:35:22 2024, max compression
+gzip compressed data, was "data-quality-validation-pydeequ-0.9.tar", last modified: Tue May  7 08:42:27 2024, max compression
```

## Comparing `data-quality-validation-pydeequ-0.8.tar` & `data-quality-validation-pydeequ-0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:35:22.591226 data-quality-validation-pydeequ-0.8/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6080 2024-05-07 08:35:22.590797 data-quality-validation-pydeequ-0.8/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5599 2024-05-07 08:35:09.000000 data-quality-validation-pydeequ-0.8/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:35:22.590237 data-quality-validation-pydeequ-0.8/data_quality_validation_pydeequ.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6080 2024-05-07 08:35:22.000000 data-quality-validation-pydeequ-0.8/data_quality_validation_pydeequ.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 08:35:22.000000 data-quality-validation-pydeequ-0.8/data_quality_validation_pydeequ.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 08:35:22.000000 data-quality-validation-pydeequ-0.8/data_quality_validation_pydeequ.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 08:35:22.000000 data-quality-validation-pydeequ-0.8/data_quality_validation_pydeequ.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 08:35:22.000000 data-quality-validation-pydeequ-0.8/data_quality_validation_pydeequ.egg-info/top_level.txt
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:35:22.589288 data-quality-validation-pydeequ-0.8/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.8/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.8/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.8/dqv/dqv_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 08:35:22.591297 data-quality-validation-pydeequ-0.8/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 08:35:19.000000 data-quality-validation-pydeequ-0.8/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:42:27.004926 data-quality-validation-pydeequ-0.9/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6286 2024-05-07 08:42:27.004499 data-quality-validation-pydeequ-0.9/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5805 2024-05-07 08:40:56.000000 data-quality-validation-pydeequ-0.9/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:42:27.003877 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6286 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-07 08:42:26.000000 data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/top_level.txt
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-07 08:42:27.002548 data-quality-validation-pydeequ-0.9/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.9/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.9/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.9/dqv/dqv_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-07 08:42:27.004994 data-quality-validation-pydeequ-0.9/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      826 2024-05-07 08:41:40.000000 data-quality-validation-pydeequ-0.9/setup.py
```

### Comparing `data-quality-validation-pydeequ-0.8/PKG-INFO` & `data-quality-validation-pydeequ-0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 0.8
+Version: 0.9
 Summary: A library for data quality validation using PyDeequ.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -117,7 +117,12 @@
    DqvPydeequ(
         "", #config_file
         "", #source_data_path
         "") #target_data_path
    ```
 
 - Step 8: Run the file to validate.
+
+
+<br></br>
+Refer this repo to follow the structure of config file format  <br></br>
+Git: <a href="https://github.com/dataruk/data-quality-validation">https://github.com/dataruk/data-quality-validation</a>
```

### Comparing `data-quality-validation-pydeequ-0.8/README.md` & `data-quality-validation-pydeequ-0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -100,8 +100,13 @@
    ```
    DqvPydeequ(
         "", #config_file
         "", #source_data_path
         "") #target_data_path
    ```
 
-- Step 8: Run the file to validate.
+- Step 8: Run the file to validate.
+
+
+<br></br>
+Refer this repo to follow the structure of config file format  <br></br>
+Git: <a href="https://github.com/dataruk/data-quality-validation">https://github.com/dataruk/data-quality-validation</a>
```

### Comparing `data-quality-validation-pydeequ-0.8/data_quality_validation_pydeequ.egg-info/PKG-INFO` & `data-quality-validation-pydeequ-0.9/data_quality_validation_pydeequ.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 0.8
+Version: 0.9
 Summary: A library for data quality validation using PyDeequ.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -117,7 +117,12 @@
    DqvPydeequ(
         "", #config_file
         "", #source_data_path
         "") #target_data_path
    ```
 
 - Step 8: Run the file to validate.
+
+
+<br></br>
+Refer this repo to follow the structure of config file format  <br></br>
+Git: <a href="https://github.com/dataruk/data-quality-validation">https://github.com/dataruk/data-quality-validation</a>
```

### Comparing `data-quality-validation-pydeequ-0.8/dqv/data_quality_validation_pydeequ.py` & `data-quality-validation-pydeequ-0.9/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.8/dqv/dqv_pydeequ.py` & `data-quality-validation-pydeequ-0.9/dqv/dqv_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.8/setup.py` & `data-quality-validation-pydeequ-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reading the README.md file for long description in PyPI site
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='data-quality-validation-pydeequ',
-    version='0.8',
+    version='0.9',
     author='Ketan Kirange',
     author_email='k.kirange@reply.com',
     description='A library for data quality validation using PyDeequ.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```


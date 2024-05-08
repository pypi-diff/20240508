# Comparing `tmp/hrbdataproject-2.3.tar.gz` & `tmp/hrbdataproject-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrbdataproject-2.3.tar", last modified: Wed May  8 09:01:27 2024, max compression
+gzip compressed data, was "hrbdataproject-2.4.tar", last modified: Wed May  8 09:12:58 2024, max compression
```

## Comparing `hrbdataproject-2.3.tar` & `hrbdataproject-2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 09:01:27.050285 hrbdataproject-2.3/
--rw-rw-rw-   0        0        0      367 2024-05-08 09:01:27.047393 hrbdataproject-2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2281 2024-05-03 16:01:44.000000 hrbdataproject-2.3/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 09:01:27.031047 hrbdataproject-2.3/hrbdataproject/
--rw-rw-rw-   0        0        0      125 2024-05-03 09:51:07.000000 hrbdataproject-2.3/hrbdataproject/__init__.py
--rw-rw-rw-   0        0        0     7267 2024-05-03 15:43:43.000000 hrbdataproject-2.3/hrbdataproject/data_quality_checks.py
--rw-rw-rw-   0        0        0        0 2024-05-08 09:00:14.000000 hrbdataproject-2.3/hrbdataproject/datachecks.py
-drwxrwxrwx   0        0        0        0 2024-05-08 09:01:27.044869 hrbdataproject-2.3/hrbdataproject.egg-info/
--rw-rw-rw-   0        0        0      367 2024-05-08 09:01:26.000000 hrbdataproject-2.3/hrbdataproject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-08 09:01:26.000000 hrbdataproject-2.3/hrbdataproject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 09:01:26.000000 hrbdataproject-2.3/hrbdataproject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-08 09:01:26.000000 hrbdataproject-2.3/hrbdataproject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 09:01:27.050285 hrbdataproject-2.3/setup.cfg
--rw-rw-rw-   0        0        0      581 2024-05-08 09:00:49.000000 hrbdataproject-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:12:58.774194 hrbdataproject-2.4/
+-rw-rw-rw-   0        0        0      367 2024-05-08 09:12:58.769102 hrbdataproject-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2281 2024-05-03 16:01:44.000000 hrbdataproject-2.4/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 09:12:58.764405 hrbdataproject-2.4/hrbdataproject/
+-rw-rw-rw-   0        0        0      149 2024-05-08 09:11:21.000000 hrbdataproject-2.4/hrbdataproject/__init__.py
+-rw-rw-rw-   0        0        0     7267 2024-05-03 15:43:43.000000 hrbdataproject-2.4/hrbdataproject/data_quality_checks.py
+-rw-rw-rw-   0        0        0        0 2024-05-08 09:00:14.000000 hrbdataproject-2.4/hrbdataproject/datachecks.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:12:58.769102 hrbdataproject-2.4/hrbdataproject.egg-info/
+-rw-rw-rw-   0        0        0      367 2024-05-08 09:12:58.000000 hrbdataproject-2.4/hrbdataproject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-08 09:12:58.000000 hrbdataproject-2.4/hrbdataproject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 09:12:58.000000 hrbdataproject-2.4/hrbdataproject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-08 09:12:58.000000 hrbdataproject-2.4/hrbdataproject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 09:12:58.774194 hrbdataproject-2.4/setup.cfg
+-rw-rw-rw-   0        0        0      581 2024-05-08 09:11:34.000000 hrbdataproject-2.4/setup.py
```

### Comparing `hrbdataproject-2.3/README.txt` & `hrbdataproject-2.4/README.txt`

 * *Files identical despite different names*

### Comparing `hrbdataproject-2.3/hrbdataproject/data_quality_checks.py` & `hrbdataproject-2.4/hrbdataproject/data_quality_checks.py`

 * *Files identical despite different names*

### Comparing `hrbdataproject-2.3/setup.py` & `hrbdataproject-2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hrbdataproject',
-    version='2.3',
+    version='2.4',
     packages=find_packages(),
     #py_modules=['data_quality_checks'],  # Specify the individual Python file here
     description='A library for data quality checks in Databricks notebooks',
     author='Harun Raseed Basheer',
     author_email='harun.raseed093@gmail.com',
     url='https://github.com/harunraseed/hrbdataproject',
     license='MIT',
```


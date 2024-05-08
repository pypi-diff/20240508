# Comparing `tmp/hrbdataproject-2.2.tar.gz` & `tmp/hrbdataproject-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrbdataproject-2.2.tar", last modified: Fri May  3 16:10:25 2024, max compression
+gzip compressed data, was "hrbdataproject-2.3.tar", last modified: Wed May  8 09:01:27 2024, max compression
```

## Comparing `hrbdataproject-2.2.tar` & `hrbdataproject-2.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 16:10:25.841214 hrbdataproject-2.2/
--rw-rw-rw-   0        0        0      367 2024-05-03 16:10:25.841214 hrbdataproject-2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2281 2024-05-03 16:01:44.000000 hrbdataproject-2.2/README.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 16:10:25.831955 hrbdataproject-2.2/hrbdataproject/
--rw-rw-rw-   0        0        0      125 2024-05-03 09:51:07.000000 hrbdataproject-2.2/hrbdataproject/__init__.py
--rw-rw-rw-   0        0        0     7267 2024-05-03 15:43:43.000000 hrbdataproject-2.2/hrbdataproject/data_quality_checks.py
-drwxrwxrwx   0        0        0        0 2024-05-03 16:10:25.839216 hrbdataproject-2.2/hrbdataproject.egg-info/
--rw-rw-rw-   0        0        0      367 2024-05-03 16:10:25.000000 hrbdataproject-2.2/hrbdataproject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-03 16:10:25.000000 hrbdataproject-2.2/hrbdataproject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 16:10:25.000000 hrbdataproject-2.2/hrbdataproject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-03 16:10:25.000000 hrbdataproject-2.2/hrbdataproject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 16:10:25.841214 hrbdataproject-2.2/setup.cfg
--rw-rw-rw-   0        0        0      581 2024-05-03 16:10:09.000000 hrbdataproject-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:01:27.050285 hrbdataproject-2.3/
+-rw-rw-rw-   0        0        0      367 2024-05-08 09:01:27.047393 hrbdataproject-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2281 2024-05-03 16:01:44.000000 hrbdataproject-2.3/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 09:01:27.031047 hrbdataproject-2.3/hrbdataproject/
+-rw-rw-rw-   0        0        0      125 2024-05-03 09:51:07.000000 hrbdataproject-2.3/hrbdataproject/__init__.py
+-rw-rw-rw-   0        0        0     7267 2024-05-03 15:43:43.000000 hrbdataproject-2.3/hrbdataproject/data_quality_checks.py
+-rw-rw-rw-   0        0        0        0 2024-05-08 09:00:14.000000 hrbdataproject-2.3/hrbdataproject/datachecks.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:01:27.044869 hrbdataproject-2.3/hrbdataproject.egg-info/
+-rw-rw-rw-   0        0        0      367 2024-05-08 09:01:26.000000 hrbdataproject-2.3/hrbdataproject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-08 09:01:26.000000 hrbdataproject-2.3/hrbdataproject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 09:01:26.000000 hrbdataproject-2.3/hrbdataproject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-08 09:01:26.000000 hrbdataproject-2.3/hrbdataproject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 09:01:27.050285 hrbdataproject-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      581 2024-05-08 09:00:49.000000 hrbdataproject-2.3/setup.py
```

### Comparing `hrbdataproject-2.2/README.txt` & `hrbdataproject-2.3/README.txt`

 * *Files identical despite different names*

### Comparing `hrbdataproject-2.2/hrbdataproject/data_quality_checks.py` & `hrbdataproject-2.3/hrbdataproject/data_quality_checks.py`

 * *Files identical despite different names*

### Comparing `hrbdataproject-2.2/setup.py` & `hrbdataproject-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hrbdataproject',
-    version='2.2',
+    version='2.3',
     packages=find_packages(),
     #py_modules=['data_quality_checks'],  # Specify the individual Python file here
     description='A library for data quality checks in Databricks notebooks',
     author='Harun Raseed Basheer',
     author_email='harun.raseed093@gmail.com',
     url='https://github.com/harunraseed/hrbdataproject',
     license='MIT',
```


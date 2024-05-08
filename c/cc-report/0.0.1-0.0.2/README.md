# Comparing `tmp/cc_report-0.0.1.tar.gz` & `tmp/cc_report-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc_report-0.0.1.tar", last modified: Wed May  8 10:47:57 2024, max compression
+gzip compressed data, was "cc_report-0.0.2.tar", last modified: Wed May  8 13:08:55 2024, max compression
```

## Comparing `cc_report-0.0.1.tar` & `cc_report-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 10:47:57.916348 cc_report-0.0.1/
--rw-r--r--   0 cc         (501) staff       (20)      313 2024-05-08 10:47:57.916232 cc_report-0.0.1/PKG-INFO
-drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 10:47:57.915782 cc_report-0.0.1/cc_report.egg-info/
--rw-r--r--   0 cc         (501) staff       (20)      313 2024-05-08 10:47:57.000000 cc_report-0.0.1/cc_report.egg-info/PKG-INFO
--rw-r--r--   0 cc         (501) staff       (20)      194 2024-05-08 10:47:57.000000 cc_report-0.0.1/cc_report.egg-info/SOURCES.txt
--rw-r--r--   0 cc         (501) staff       (20)        1 2024-05-08 10:47:57.000000 cc_report-0.0.1/cc_report.egg-info/dependency_links.txt
--rw-r--r--   0 cc         (501) staff       (20)       14 2024-05-08 10:47:57.000000 cc_report-0.0.1/cc_report.egg-info/requires.txt
--rw-r--r--   0 cc         (501) staff       (20)       10 2024-05-08 10:47:57.000000 cc_report-0.0.1/cc_report.egg-info/top_level.txt
--rw-r--r--   0 cc         (501) staff       (20)       38 2024-05-08 10:47:57.916401 cc_report-0.0.1/setup.cfg
--rw-r--r--   0 cc         (501) staff       (20)      622 2024-05-08 10:18:05.000000 cc_report-0.0.1/setup.py
-drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 10:47:57.915939 cc_report-0.0.1/templates/
--rw-r--r--   0 cc         (501) staff       (20)      166 2024-05-08 09:17:46.000000 cc_report-0.0.1/templates/__init__.py
+drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 13:08:55.251009 cc_report-0.0.2/
+-rw-r--r--   0 cc         (501) staff       (20)      313 2024-05-08 13:08:55.250825 cc_report-0.0.2/PKG-INFO
+drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 13:08:55.243902 cc_report-0.0.2/cc_report/
+-rw-r--r--   0 cc         (501) staff       (20)      114 2024-05-08 11:24:39.000000 cc_report-0.0.2/cc_report/__init__.py
+-rw-r--r--   0 cc         (501) staff       (20)     6016 2024-05-08 09:20:09.000000 cc_report-0.0.2/cc_report/pytest_testreport.py
+drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 13:08:55.250477 cc_report-0.0.2/cc_report/templates/
+-rw-r--r--   0 cc         (501) staff       (20)      114 2024-05-08 11:24:39.000000 cc_report-0.0.2/cc_report/templates/__init__.py
+-rw-r--r--   0 cc         (501) staff       (20)    17611 2024-05-08 09:17:46.000000 cc_report-0.0.2/cc_report/templates/templates.html
+-rw-r--r--   0 cc         (501) staff       (20)    27983 2024-05-08 09:17:46.000000 cc_report-0.0.2/cc_report/templates/templates2.html
+drwxr-xr-x   0 cc         (501) staff       (20)        0 2024-05-08 13:08:55.248760 cc_report-0.0.2/cc_report.egg-info/
+-rw-r--r--   0 cc         (501) staff       (20)      313 2024-05-08 13:08:55.000000 cc_report-0.0.2/cc_report.egg-info/PKG-INFO
+-rw-r--r--   0 cc         (501) staff       (20)      328 2024-05-08 13:08:55.000000 cc_report-0.0.2/cc_report.egg-info/SOURCES.txt
+-rw-r--r--   0 cc         (501) staff       (20)        1 2024-05-08 13:08:55.000000 cc_report-0.0.2/cc_report.egg-info/dependency_links.txt
+-rw-r--r--   0 cc         (501) staff       (20)       14 2024-05-08 13:08:55.000000 cc_report-0.0.2/cc_report.egg-info/requires.txt
+-rw-r--r--   0 cc         (501) staff       (20)       10 2024-05-08 13:08:55.000000 cc_report-0.0.2/cc_report.egg-info/top_level.txt
+-rw-r--r--   0 cc         (501) staff       (20)       38 2024-05-08 13:08:55.251075 cc_report-0.0.2/setup.cfg
+-rw-r--r--   0 cc         (501) staff       (20)      702 2024-05-08 13:08:18.000000 cc_report-0.0.2/setup.py
```

### Comparing `cc_report-0.0.1/setup.py` & `cc_report-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 # @Site   :
 # @File   :setup.py
 
 import setuptools
 
 setuptools.setup(
     name='cc_report',
-    version='0.0.1',
+    version='0.0.2',
     packages=setuptools.find_packages(),
     license='MIT',
     author='cc.cheng',
     author_email='chaicc145@gmail.com',
     description='A MODIFIED REPORT',
     install_requires=['pytest', 'jinja2'],
+    # data_files=[('cc_report',['aa.ini'])],
+    package_data={"": ['*.html']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```


# Comparing `tmp/YW_matchups-2.1.0.tar.gz` & `tmp/YW_matchups-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YW_matchups-2.1.0.tar", last modified: Fri Mar 22 21:17:25 2024, max compression
+gzip compressed data, was "YW_matchups-2.1.1.tar", last modified: Tue May  7 04:02:43 2024, max compression
```

## Comparing `YW_matchups-2.1.0.tar` & `YW_matchups-2.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-22 21:17:25.348500 YW_matchups-2.1.0/
--rw-r--r--   0 yw         (501) staff       (20)      617 2024-03-22 21:17:25.348226 YW_matchups-2.1.0/PKG-INFO
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-22 21:17:25.339895 YW_matchups-2.1.0/YW_matchups/
--rw-r--r--   0 yw         (501) staff       (20)     2986 2024-03-20 16:12:00.000000 YW_matchups-2.1.0/YW_matchups/AC_acolite.py
--rw-r--r--   0 yw         (501) staff       (20)     3906 2023-12-28 03:02:04.000000 YW_matchups-2.1.0/YW_matchups/AC_l2gen.py
--rw-r--r--   0 yw         (501) staff       (20)     2835 2023-12-26 17:52:26.000000 YW_matchups-2.1.0/YW_matchups/AC_polymer.py
--rw-r--r--   0 yw         (501) staff       (20)      297 2023-12-16 21:20:26.000000 YW_matchups-2.1.0/YW_matchups/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     9676 2024-03-22 21:02:20.000000 YW_matchups-2.1.0/YW_matchups/run.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-22 21:17:25.341390 YW_matchups-2.1.0/YW_matchups.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)      617 2024-03-22 21:17:25.000000 YW_matchups-2.1.0/YW_matchups.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)      447 2024-03-22 21:17:25.000000 YW_matchups-2.1.0/YW_matchups.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2024-03-22 21:17:25.000000 YW_matchups-2.1.0/YW_matchups.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       28 2024-03-22 21:17:25.000000 YW_matchups-2.1.0/YW_matchups.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)       12 2024-03-22 21:17:25.000000 YW_matchups-2.1.0/YW_matchups.egg-info/top_level.txt
--rw-r--r--   0 yw         (501) staff       (20)       38 2024-03-22 21:17:25.348572 YW_matchups-2.1.0/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)      644 2024-03-22 21:15:34.000000 YW_matchups-2.1.0/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-03-22 21:17:25.347853 YW_matchups-2.1.0/tests/
--rw-r--r--   0 yw         (501) staff       (20)      822 2023-12-26 16:46:40.000000 YW_matchups-2.1.0/tests/test_acolite_L8.py
--rw-r--r--   0 yw         (501) staff       (20)      853 2023-12-18 19:48:30.000000 YW_matchups-2.1.0/tests/test_acolite_S2.py
--rw-r--r--   0 yw         (501) staff       (20)      673 2023-12-26 18:27:02.000000 YW_matchups-2.1.0/tests/test_l2gen_L8.py
--rw-r--r--   0 yw         (501) staff       (20)      961 2023-12-23 19:30:03.000000 YW_matchups-2.1.0/tests/test_l2gen_S2.py
--rw-r--r--   0 yw         (501) staff       (20)      555 2023-12-31 21:17:41.000000 YW_matchups-2.1.0/tests/test_polymer_L8.py
--rw-r--r--   0 yw         (501) staff       (20)      689 2023-12-17 19:16:32.000000 YW_matchups-2.1.0/tests/test_polymer_S2.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-07 04:02:43.764460 YW_matchups-2.1.1/
+-rw-r--r--   0 yw         (501) staff       (20)      617 2024-05-07 04:02:43.764186 YW_matchups-2.1.1/PKG-INFO
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-07 04:02:43.761119 YW_matchups-2.1.1/YW_matchups/
+-rw-r--r--   0 yw         (501) staff       (20)     3104 2024-05-02 03:17:42.000000 YW_matchups-2.1.1/YW_matchups/AC_acolite.py
+-rw-r--r--   0 yw         (501) staff       (20)     3906 2023-12-28 03:02:04.000000 YW_matchups-2.1.1/YW_matchups/AC_l2gen.py
+-rw-r--r--   0 yw         (501) staff       (20)     2835 2023-12-26 17:52:26.000000 YW_matchups-2.1.1/YW_matchups/AC_polymer.py
+-rw-r--r--   0 yw         (501) staff       (20)      297 2023-12-16 21:20:26.000000 YW_matchups-2.1.1/YW_matchups/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     9676 2024-03-22 21:02:20.000000 YW_matchups-2.1.1/YW_matchups/run.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-07 04:02:43.761989 YW_matchups-2.1.1/YW_matchups.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)      617 2024-05-07 04:02:43.000000 YW_matchups-2.1.1/YW_matchups.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)      447 2024-05-07 04:02:43.000000 YW_matchups-2.1.1/YW_matchups.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2024-05-07 04:02:43.000000 YW_matchups-2.1.1/YW_matchups.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       28 2024-05-07 04:02:43.000000 YW_matchups-2.1.1/YW_matchups.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)       12 2024-05-07 04:02:43.000000 YW_matchups-2.1.1/YW_matchups.egg-info/top_level.txt
+-rw-r--r--   0 yw         (501) staff       (20)       38 2024-05-07 04:02:43.764531 YW_matchups-2.1.1/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)      644 2024-05-07 04:01:47.000000 YW_matchups-2.1.1/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-07 04:02:43.763753 YW_matchups-2.1.1/tests/
+-rw-r--r--   0 yw         (501) staff       (20)      822 2023-12-26 16:46:40.000000 YW_matchups-2.1.1/tests/test_acolite_L8.py
+-rw-r--r--   0 yw         (501) staff       (20)      853 2023-12-18 19:48:30.000000 YW_matchups-2.1.1/tests/test_acolite_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)      673 2023-12-26 18:27:02.000000 YW_matchups-2.1.1/tests/test_l2gen_L8.py
+-rw-r--r--   0 yw         (501) staff       (20)      961 2023-12-23 19:30:03.000000 YW_matchups-2.1.1/tests/test_l2gen_S2.py
+-rw-r--r--   0 yw         (501) staff       (20)      555 2023-12-31 21:17:41.000000 YW_matchups-2.1.1/tests/test_polymer_L8.py
+-rw-r--r--   0 yw         (501) staff       (20)      689 2023-12-17 19:16:32.000000 YW_matchups-2.1.1/tests/test_polymer_S2.py
```

### Comparing `YW_matchups-2.1.0/PKG-INFO` & `YW_matchups-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YW_matchups
-Version: 2.1.0
+Version: 2.1.1
 Summary: Find satellite matchups for aquatic remote sensing
 Author: Yulun Wu
 Author-email: yulunwu8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyproj
```

### Comparing `YW_matchups-2.1.0/YW_matchups/AC_acolite.py` & `YW_matchups-2.1.1/YW_matchups/AC_acolite.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,27 @@
 
 
 
 # Get datetime object 
 def get_datetime(sat_file):
     with nc4.Dataset(sat_file,"r") as nc:
         
+        sensor = nc.getncattr('sensor')
+
+        
         ### full resolution ###
         # datetime_sat_string = nc.getncattr('isodate')
         # format_string = '%Y-%m-%dT%H:%M:%S.%f%z'
         
-        
         # March 20, 2024 update: prioritize inputfile name instead
         
         try: 
+            
+            if sensor=='L8_OLI': raise Exception()
+            
             inputfile = nc.getncattr('inputfile').split('/')[-1]
             datetime_sat_string = inputfile[11:26]
             format_string = '%Y%m%dT%H%M%S'
             
         except:
             # nearest second 
             datetime_sat_string = nc.getncattr('isodate').split('.', 1)[0]
```

### Comparing `YW_matchups-2.1.0/YW_matchups/AC_l2gen.py` & `YW_matchups-2.1.1/YW_matchups/AC_l2gen.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.0/YW_matchups/AC_polymer.py` & `YW_matchups-2.1.1/YW_matchups/AC_polymer.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.0/YW_matchups/run.py` & `YW_matchups-2.1.1/YW_matchups/run.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.0/YW_matchups.egg-info/PKG-INFO` & `YW_matchups-2.1.1/YW_matchups.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YW-matchups
-Version: 2.1.0
+Version: 2.1.1
 Summary: Find satellite matchups for aquatic remote sensing
 Author: Yulun Wu
 Author-email: yulunwu8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pyproj
```

### Comparing `YW_matchups-2.1.0/setup.py` & `YW_matchups-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='YW_matchups',
-    version='2.1.0',
+    version='2.1.1',
     author='Yulun Wu',
     author_email='yulunwu8@gmail.com',
     description='Find satellite matchups for aquatic remote sensing',
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `YW_matchups-2.1.0/tests/test_acolite_L8.py` & `YW_matchups-2.1.1/tests/test_acolite_L8.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.0/tests/test_acolite_S2.py` & `YW_matchups-2.1.1/tests/test_acolite_S2.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.0/tests/test_l2gen_L8.py` & `YW_matchups-2.1.1/tests/test_l2gen_L8.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.0/tests/test_l2gen_S2.py` & `YW_matchups-2.1.1/tests/test_l2gen_S2.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.0/tests/test_polymer_L8.py` & `YW_matchups-2.1.1/tests/test_polymer_L8.py`

 * *Files identical despite different names*

### Comparing `YW_matchups-2.1.0/tests/test_polymer_S2.py` & `YW_matchups-2.1.1/tests/test_polymer_S2.py`

 * *Files identical despite different names*


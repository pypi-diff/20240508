# Comparing `tmp/baysalt_christmas-1.1.5.tar.gz` & `tmp/baysalt_christmas-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-1.1.5.tar", last modified: Mon Apr 22 09:37:02 2024, max compression
+gzip compressed data, was "baysalt_christmas-1.1.6.tar", last modified: Wed May  8 03:12:06 2024, max compression
```

## Comparing `baysalt_christmas-1.1.5.tar` & `baysalt_christmas-1.1.6.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:37:02.501271 baysalt_christmas-1.1.5/
--rw-r--r--   0 christmas   (501) staff       (20)      117 2024-04-16 09:59:40.000000 baysalt_christmas-1.1.5/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4183 2024-04-22 09:37:02.501037 baysalt_christmas-1.1.5/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-1.1.5/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:37:02.500684 baysalt_christmas-1.1.5/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4183 2024-04-22 09:37:02.000000 baysalt_christmas-1.1.5/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      848 2024-04-22 09:37:02.000000 baysalt_christmas-1.1.5/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2024-04-22 09:37:02.000000 baysalt_christmas-1.1.5/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2024-04-22 09:37:02.000000 baysalt_christmas-1.1.5/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2024-04-22 09:37:02.000000 baysalt_christmas-1.1.5/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:37:02.498058 baysalt_christmas-1.1.5/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    22673 2023-09-24 17:35:32.000000 baysalt_christmas-1.1.5/christmas/Blogging.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:37:02.498383 baysalt_christmas-1.1.5/christmas/Pyshell/
--rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-1.1.5/christmas/Pyshell/RS_File.py
--rw-r--r--   0 christmas   (501) staff       (20)      232 2023-09-18 07:37:39.000000 baysalt_christmas-1.1.5/christmas/Pyshell/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     3787 2023-12-24 15:59:53.000000 baysalt_christmas-1.1.5/christmas/S_DateTime.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:37:02.498690 baysalt_christmas-1.1.5/christmas/SameAsMATLAB/
--rw-r--r--   0 christmas   (501) staff       (20)     1270 2024-03-15 18:59:22.000000 baysalt_christmas-1.1.5/christmas/SameAsMATLAB/CoorTrans.py
--rw-r--r--   0 christmas   (501) staff       (20)      236 2023-11-27 08:58:33.000000 baysalt_christmas-1.1.5/christmas/SameAsMATLAB/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:37:02.498995 baysalt_christmas-1.1.5/christmas/Standard/
--rw-r--r--   0 christmas   (501) staff       (20)      234 2023-09-18 07:38:49.000000 baysalt_christmas-1.1.5/christmas/Standard/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     5903 2023-10-08 09:19:02.000000 baysalt_christmas-1.1.5/christmas/Standard/xr_attrs.py
--rw-r--r--   0 christmas   (501) staff       (20)      479 2023-11-27 08:58:33.000000 baysalt_christmas-1.1.5/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     6481 2024-04-22 09:15:53.000000 baysalt_christmas-1.1.5/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1812 2023-09-24 17:45:18.000000 baysalt_christmas-1.1.5/christmas/cprintfs.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:37:02.500029 baysalt_christmas-1.1.5/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-1.1.5/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-1.1.5/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-1.1.5/christmas/mncPy/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-1.1.5/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-1.1.5/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)    10216 2023-09-24 17:47:39.000000 baysalt_christmas-1.1.5/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     4786 2024-04-22 09:36:50.000000 baysalt_christmas-1.1.5/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     2651 2024-03-15 19:01:03.000000 baysalt_christmas-1.1.5/christmas/server_info.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-04-22 09:37:02.500486 baysalt_christmas-1.1.5/christmas/tools/
--rw-r--r--   0 christmas   (501) staff       (20)      916 2023-09-24 17:50:48.000000 baysalt_christmas-1.1.5/christmas/tools/P_params.py
--rw-r--r--   0 christmas   (501) staff       (20)      264 2023-07-20 11:57:28.000000 baysalt_christmas-1.1.5/christmas/tools/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4052 2023-10-08 16:11:23.000000 baysalt_christmas-1.1.5/christmas/tools/download_check.py
--rw-r--r--   0 christmas   (501) staff       (20)      749 2024-03-21 07:10:04.000000 baysalt_christmas-1.1.5/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2024-04-22 09:37:02.501324 baysalt_christmas-1.1.5/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      794 2024-04-22 09:36:59.000000 baysalt_christmas-1.1.5/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-05-08 03:12:06.146638 baysalt_christmas-1.1.6/
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2024-04-16 09:59:40.000000 baysalt_christmas-1.1.6/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4183 2024-05-08 03:12:06.146249 baysalt_christmas-1.1.6/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-1.1.6/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-05-08 03:12:06.145903 baysalt_christmas-1.1.6/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4183 2024-05-08 03:12:06.000000 baysalt_christmas-1.1.6/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      907 2024-05-08 03:12:06.000000 baysalt_christmas-1.1.6/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2024-05-08 03:12:06.000000 baysalt_christmas-1.1.6/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2024-05-08 03:12:06.000000 baysalt_christmas-1.1.6/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2024-05-08 03:12:06.000000 baysalt_christmas-1.1.6/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-05-08 03:12:06.139131 baysalt_christmas-1.1.6/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    22673 2023-09-24 17:35:32.000000 baysalt_christmas-1.1.6/christmas/Blogging.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-05-08 03:12:06.139877 baysalt_christmas-1.1.6/christmas/Pyshell/
+-rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-1.1.6/christmas/Pyshell/RS_File.py
+-rw-r--r--   0 christmas   (501) staff       (20)      232 2023-09-18 07:37:39.000000 baysalt_christmas-1.1.6/christmas/Pyshell/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4036 2024-05-08 02:47:29.000000 baysalt_christmas-1.1.6/christmas/S_DateTime.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-05-08 03:12:06.140496 baysalt_christmas-1.1.6/christmas/SameAsMATLAB/
+-rw-r--r--   0 christmas   (501) staff       (20)     1270 2024-03-15 18:59:22.000000 baysalt_christmas-1.1.6/christmas/SameAsMATLAB/CoorTrans.py
+-rw-r--r--   0 christmas   (501) staff       (20)      236 2023-11-27 08:58:33.000000 baysalt_christmas-1.1.6/christmas/SameAsMATLAB/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-05-08 03:12:06.141157 baysalt_christmas-1.1.6/christmas/Standard/
+-rw-r--r--   0 christmas   (501) staff       (20)      234 2023-09-18 07:38:49.000000 baysalt_christmas-1.1.6/christmas/Standard/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     5903 2023-10-08 09:19:02.000000 baysalt_christmas-1.1.6/christmas/Standard/xr_attrs.py
+-rw-r--r--   0 christmas   (501) staff       (20)      479 2023-11-27 08:58:33.000000 baysalt_christmas-1.1.6/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     6481 2024-04-22 09:15:53.000000 baysalt_christmas-1.1.6/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1812 2023-09-24 17:45:18.000000 baysalt_christmas-1.1.6/christmas/cprintfs.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-05-08 03:12:06.143132 baysalt_christmas-1.1.6/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-1.1.6/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-1.1.6/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-1.1.6/christmas/mncPy/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-1.1.6/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-1.1.6/christmas/mncPy/compress.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-05-08 03:12:06.143761 baysalt_christmas-1.1.6/christmas/pFVCOM/
+-rw-r--r--   0 christmas   (501) staff       (20)      215 2024-04-23 13:42:07.000000 baysalt_christmas-1.1.6/christmas/pFVCOM/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     2187 2024-04-23 13:48:55.000000 baysalt_christmas-1.1.6/christmas/pFVCOM/writeFile.py
+-rw-r--r--   0 christmas   (501) staff       (20)    10216 2023-09-24 17:47:39.000000 baysalt_christmas-1.1.6/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4786 2024-04-22 09:36:50.000000 baysalt_christmas-1.1.6/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     2651 2024-03-15 19:01:03.000000 baysalt_christmas-1.1.6/christmas/server_info.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2024-05-08 03:12:06.145630 baysalt_christmas-1.1.6/christmas/tools/
+-rw-r--r--   0 christmas   (501) staff       (20)      916 2023-09-24 17:50:48.000000 baysalt_christmas-1.1.6/christmas/tools/P_params.py
+-rw-r--r--   0 christmas   (501) staff       (20)      264 2023-07-20 11:57:28.000000 baysalt_christmas-1.1.6/christmas/tools/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4052 2023-10-08 16:11:23.000000 baysalt_christmas-1.1.6/christmas/tools/download_check.py
+-rw-r--r--   0 christmas   (501) staff       (20)      749 2024-03-21 07:10:04.000000 baysalt_christmas-1.1.6/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2024-05-08 03:12:06.146700 baysalt_christmas-1.1.6/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      794 2024-05-08 03:12:04.000000 baysalt_christmas-1.1.6/setup.py
```

### Comparing `baysalt_christmas-1.1.5/PKG-INFO` & `baysalt_christmas-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 1.1.5
+Version: 1.1.6
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-1.1.5/README.md` & `baysalt_christmas-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-1.1.6/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 1.1.5
+Version: 1.1.6
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-1.1.5/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-1.1.6/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -22,10 +22,12 @@
 christmas/Standard/__init__.py
 christmas/Standard/xr_attrs.py
 christmas/mncPy/.gitignore
 christmas/mncPy/LICENSE
 christmas/mncPy/__init__.py
 christmas/mncPy/common.py
 christmas/mncPy/compress.py
+christmas/pFVCOM/__init__.py
+christmas/pFVCOM/writeFile.py
 christmas/tools/P_params.py
 christmas/tools/__init__.py
 christmas/tools/download_check.py
```

### Comparing `baysalt_christmas-1.1.5/christmas/Blogging.py` & `baysalt_christmas-1.1.6/christmas/Blogging.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/Pyshell/RS_File.py` & `baysalt_christmas-1.1.6/christmas/Pyshell/RS_File.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/S_DateTime.py` & `baysalt_christmas-1.1.6/christmas/S_DateTime.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     ymd_yes3 = (datetime.datetime.strptime(today, '%Y%m%d') - datetime.timedelta(days=3)).strftime('%Y%m%d')
     year_yes = ymd_yes[:4]
     month_yes = ymd_yes[4:6]
     year_yes2 = ymd_yes2[:4]
     month_yes2 = ymd_yes2[4:6]
     year_yes3 = ymd_yes3[:4]
     month_yes3 = ymd_yes3[4:6]
+
+    ymd_today = datetime.datetime.strptime(today, '%Y%m%d').strftime('%Y%m%d')
+    year_today = ymd_today[:4]
+    month_today = ymd_today[4:6]
+
     ymd_tom = (datetime.datetime.strptime(today, '%Y%m%d') + datetime.timedelta(days=1)).strftime('%Y%m%d')
     ymd_tom2 = (datetime.datetime.strptime(today, '%Y%m%d') + datetime.timedelta(days=2)).strftime('%Y%m%d')
     ymd_tom3 = (datetime.datetime.strptime(today, '%Y%m%d') + datetime.timedelta(days=3)).strftime('%Y%m%d')
     year_tom = ymd_tom[:4]
     month_tom = ymd_tom[4:6]
     year_tom2 = ymd_tom2[:4]
     month_tom2 = ymd_tom2[4:6]
@@ -46,14 +51,19 @@
         'month_yes': month_yes,
         'ymd_yes2': ymd_yes2,
         'year_yes2': year_yes2,
         'month_yes2': month_yes2,
         'ymd_yes3': ymd_yes3,
         'year_yes3': year_yes3,
         'month_yes3': month_yes3,
+
+        'ymd_today': ymd_today,
+        'year_today': year_today,
+        'month_today': month_today,
+
         'ymd_tom': ymd_tom,
         'year_tom': year_tom,
         'month_tom': month_tom,
         'ymd_tom2': ymd_tom2,
         'year_tom2': year_tom2,
         'month_tom2': month_tom2,
         'ymd_tom3': ymd_tom3,
```

### Comparing `baysalt_christmas-1.1.5/christmas/SameAsMATLAB/CoorTrans.py` & `baysalt_christmas-1.1.6/christmas/SameAsMATLAB/CoorTrans.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/Standard/xr_attrs.py` & `baysalt_christmas-1.1.6/christmas/Standard/xr_attrs.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/commonCode.py` & `baysalt_christmas-1.1.6/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/cprintfs.py` & `baysalt_christmas-1.1.6/christmas/cprintfs.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/mncPy/.gitignore` & `baysalt_christmas-1.1.6/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/mncPy/LICENSE` & `baysalt_christmas-1.1.6/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/mncPy/common.py` & `baysalt_christmas-1.1.6/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/mncPy/compress.py` & `baysalt_christmas-1.1.6/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/processBar.py` & `baysalt_christmas-1.1.6/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/read_conf.py` & `baysalt_christmas-1.1.6/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/server_info.py` & `baysalt_christmas-1.1.6/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/tools/P_params.py` & `baysalt_christmas-1.1.6/christmas/tools/P_params.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/christmas/tools/download_check.py` & `baysalt_christmas-1.1.6/christmas/tools/download_check.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/run_twine.py` & `baysalt_christmas-1.1.6/run_twine.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-1.1.5/setup.py` & `baysalt_christmas-1.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="1.1.5",
+    version="1.1.6",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```


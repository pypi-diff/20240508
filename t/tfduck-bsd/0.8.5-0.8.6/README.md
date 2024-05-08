# Comparing `tmp/tfduck-bsd-0.8.5.tar.gz` & `tmp/tfduck-bsd-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tfduck-bsd-0.8.5.tar", last modified: Mon Feb 28 08:13:20 2022, max compression
+gzip compressed data, was "dist/tfduck-bsd-0.8.6.tar", last modified: Mon Feb 28 08:43:56 2022, max compression
```

## Comparing `tfduck-bsd-0.8.5.tar` & `tfduck-bsd-0.8.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/
--rw-r--r--   0 yuanxiao   (501) staff       (20)     1073 2020-04-10 08:39:05.000000 tfduck-bsd-0.8.5/LICENSE
--rw-r--r--   0 yuanxiao   (501) staff       (20)      723 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/PKG-INFO
--rw-r--r--   0 yuanxiao   (501) staff       (20)      300 2020-04-10 09:28:02.000000 tfduck-bsd-0.8.5/README.md
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/bin/
--rw-r--r--   0 yuanxiao   (501) staff       (20)      205 2020-04-17 10:46:05.000000 tfduck-bsd-0.8.5/bin/tfduck
--rw-r--r--   0 yuanxiao   (501) staff       (20)       38 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/setup.cfg
--rw-r--r--   0 yuanxiao   (501) staff       (20)      907 2022-02-28 08:12:33.000000 tfduck-bsd-0.8.5/setup.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/
--rw-r--r--   0 yuanxiao   (501) staff       (20)       19 2022-02-28 08:12:38.000000 tfduck-bsd-0.8.5/tfduck/__init__.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/
--rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 04:01:02.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/__init__.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/config/
--rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 04:14:53.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/config/__init__.py
--rwxrwxrwx   0 yuanxiao   (501) staff       (20)     7405 2020-04-23 06:20:33.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/config/bdpmanager.py
--rwxrwxrwx   0 yuanxiao   (501) staff       (20)      897 2020-04-23 04:13:00.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/config/table_config.py
--rwxrwxrwx   0 yuanxiao   (501) staff       (20)     2879 2020-04-23 04:13:12.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/example.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/opends/
--rwxr-xr-x   0 yuanxiao   (501) staff       (20)       83 2020-04-23 04:01:02.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/opends/__init__.py
--rwxr-xr-x   0 yuanxiao   (501) staff       (20)    15266 2020-06-15 03:52:13.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/opends/opends.py
--rwxr-xr-x   0 yuanxiao   (501) staff       (20)    19136 2020-04-23 04:01:02.000000 tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/opends/sdk.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/common/
--rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 04:15:03.000000 tfduck-bsd-0.8.5/tfduck/common/__init__.py
--rwxrwxrwx   0 yuanxiao   (501) staff       (20)    17298 2022-02-16 10:12:45.000000 tfduck-bsd-0.8.5/tfduck/common/defines.py
--rwxrwxrwx   0 yuanxiao   (501) staff       (20)     1521 2020-04-23 03:56:35.000000 tfduck-bsd-0.8.5/tfduck/common/extendEncoder.py
--rw-r--r--   0 yuanxiao   (501) staff       (20)    14664 2021-03-15 06:42:01.000000 tfduck-bsd-0.8.5/tfduck/main.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/oss/
--rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 07:04:57.000000 tfduck-bsd-0.8.5/tfduck/oss/__init__.py
--rw-r--r--   0 yuanxiao   (501) staff       (20)    18783 2022-02-28 08:12:19.000000 tfduck-bsd-0.8.5/tfduck/oss/oss.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/pyspark_k8s/
--rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2021-04-25 06:50:03.000000 tfduck-bsd-0.8.5/tfduck/pyspark_k8s/__init__.py
--rw-r--r--   0 yuanxiao   (501) staff       (20)     4491 2021-10-27 02:06:20.000000 tfduck-bsd-0.8.5/tfduck/pyspark_k8s/k8s_manage.py
--rw-r--r--   0 yuanxiao   (501) staff       (20)    19023 2022-02-18 09:45:35.000000 tfduck-bsd-0.8.5/tfduck/pyspark_k8s/spark_manage.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/s3/
--rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2021-09-07 06:16:58.000000 tfduck-bsd-0.8.5/tfduck/s3/__init__.py
--rw-r--r--   0 yuanxiao   (501) staff       (20)    17436 2022-02-22 03:23:33.000000 tfduck-bsd-0.8.5/tfduck/s3/s3oper.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/tga/
--rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2021-09-27 10:23:41.000000 tfduck-bsd-0.8.5/tfduck/tga/__init__.py
--rw-r--r--   0 yuanxiao   (501) staff       (20)     9877 2022-02-28 01:57:50.000000 tfduck-bsd-0.8.5/tfduck/tga/tga.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck/thinkdata/
--rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 03:50:25.000000 tfduck-bsd-0.8.5/tfduck/thinkdata/__init__.py
--rw-r--r--   0 yuanxiao   (501) staff       (20)     1314 2021-09-27 10:17:18.000000 tfduck-bsd-0.8.5/tfduck/thinkdata/query.py
-drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck_bsd.egg-info/
--rw-r--r--   0 yuanxiao   (501) staff       (20)      723 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck_bsd.egg-info/PKG-INFO
--rw-r--r--   0 yuanxiao   (501) staff       (20)      880 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck_bsd.egg-info/SOURCES.txt
--rw-r--r--   0 yuanxiao   (501) staff       (20)        1 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck_bsd.egg-info/dependency_links.txt
--rw-r--r--   0 yuanxiao   (501) staff       (20)      101 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck_bsd.egg-info/requires.txt
--rw-r--r--   0 yuanxiao   (501) staff       (20)        7 2022-02-28 08:13:20.000000 tfduck-bsd-0.8.5/tfduck_bsd.egg-info/top_level.txt
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)     1073 2020-04-10 08:39:05.000000 tfduck-bsd-0.8.6/LICENSE
+-rw-r--r--   0 yuanxiao   (501) staff       (20)      723 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/PKG-INFO
+-rw-r--r--   0 yuanxiao   (501) staff       (20)      300 2020-04-10 09:28:02.000000 tfduck-bsd-0.8.6/README.md
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/bin/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)      205 2020-04-17 10:46:05.000000 tfduck-bsd-0.8.6/bin/tfduck
+-rw-r--r--   0 yuanxiao   (501) staff       (20)       38 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/setup.cfg
+-rw-r--r--   0 yuanxiao   (501) staff       (20)      907 2022-02-28 08:43:48.000000 tfduck-bsd-0.8.6/setup.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)       19 2022-02-28 08:43:44.000000 tfduck-bsd-0.8.6/tfduck/__init__.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 04:01:02.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/__init__.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/config/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 04:14:53.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/config/__init__.py
+-rwxrwxrwx   0 yuanxiao   (501) staff       (20)     7405 2020-04-23 06:20:33.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/config/bdpmanager.py
+-rwxrwxrwx   0 yuanxiao   (501) staff       (20)      897 2020-04-23 04:13:00.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/config/table_config.py
+-rwxrwxrwx   0 yuanxiao   (501) staff       (20)     2879 2020-04-23 04:13:12.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/example.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/opends/
+-rwxr-xr-x   0 yuanxiao   (501) staff       (20)       83 2020-04-23 04:01:02.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/opends/__init__.py
+-rwxr-xr-x   0 yuanxiao   (501) staff       (20)    15266 2020-06-15 03:52:13.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/opends/opends.py
+-rwxr-xr-x   0 yuanxiao   (501) staff       (20)    19136 2020-04-23 04:01:02.000000 tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/opends/sdk.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/common/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 04:15:03.000000 tfduck-bsd-0.8.6/tfduck/common/__init__.py
+-rwxrwxrwx   0 yuanxiao   (501) staff       (20)    17298 2022-02-16 10:12:45.000000 tfduck-bsd-0.8.6/tfduck/common/defines.py
+-rwxrwxrwx   0 yuanxiao   (501) staff       (20)     1521 2020-04-23 03:56:35.000000 tfduck-bsd-0.8.6/tfduck/common/extendEncoder.py
+-rw-r--r--   0 yuanxiao   (501) staff       (20)    14664 2021-03-15 06:42:01.000000 tfduck-bsd-0.8.6/tfduck/main.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/oss/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 07:04:57.000000 tfduck-bsd-0.8.6/tfduck/oss/__init__.py
+-rw-r--r--   0 yuanxiao   (501) staff       (20)    19141 2022-02-28 08:41:29.000000 tfduck-bsd-0.8.6/tfduck/oss/oss.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/pyspark_k8s/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2021-04-25 06:50:03.000000 tfduck-bsd-0.8.6/tfduck/pyspark_k8s/__init__.py
+-rw-r--r--   0 yuanxiao   (501) staff       (20)     4491 2021-10-27 02:06:20.000000 tfduck-bsd-0.8.6/tfduck/pyspark_k8s/k8s_manage.py
+-rw-r--r--   0 yuanxiao   (501) staff       (20)    19023 2022-02-18 09:45:35.000000 tfduck-bsd-0.8.6/tfduck/pyspark_k8s/spark_manage.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/s3/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2021-09-07 06:16:58.000000 tfduck-bsd-0.8.6/tfduck/s3/__init__.py
+-rw-r--r--   0 yuanxiao   (501) staff       (20)    17436 2022-02-22 03:23:33.000000 tfduck-bsd-0.8.6/tfduck/s3/s3oper.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/tga/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2021-09-27 10:23:41.000000 tfduck-bsd-0.8.6/tfduck/tga/__init__.py
+-rw-r--r--   0 yuanxiao   (501) staff       (20)     9877 2022-02-28 01:57:50.000000 tfduck-bsd-0.8.6/tfduck/tga/tga.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck/thinkdata/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        0 2020-04-23 03:50:25.000000 tfduck-bsd-0.8.6/tfduck/thinkdata/__init__.py
+-rw-r--r--   0 yuanxiao   (501) staff       (20)     1314 2021-09-27 10:17:18.000000 tfduck-bsd-0.8.6/tfduck/thinkdata/query.py
+drwxr-xr-x   0 yuanxiao   (501) staff       (20)        0 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck_bsd.egg-info/
+-rw-r--r--   0 yuanxiao   (501) staff       (20)      723 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck_bsd.egg-info/PKG-INFO
+-rw-r--r--   0 yuanxiao   (501) staff       (20)      880 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck_bsd.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        1 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck_bsd.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanxiao   (501) staff       (20)      101 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck_bsd.egg-info/requires.txt
+-rw-r--r--   0 yuanxiao   (501) staff       (20)        7 2022-02-28 08:43:56.000000 tfduck-bsd-0.8.6/tfduck_bsd.egg-info/top_level.txt
```

### Comparing `tfduck-bsd-0.8.5/LICENSE` & `tfduck-bsd-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/PKG-INFO` & `tfduck-bsd-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfduck-bsd
-Version: 0.8.5
+Version: 0.8.6
 Summary: A small example package
 Home-page: UNKNOWN
 Author: yuanxiao
 Author-email: yuan6785@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tfduck-bsd-0.8.5/setup.py` & `tfduck-bsd-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tfduck-bsd",
-    version="0.8.5",
+    version="0.8.6",
     author="yuanxiao",
     author_email="yuan6785@163.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

### Comparing `tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/config/bdpmanager.py` & `tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/config/bdpmanager.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/config/table_config.py` & `tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/config/table_config.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/example.py` & `tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/example.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/opends/opends.py` & `tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/opends/opends.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/bdp_sdk_py/opends/sdk.py` & `tfduck-bsd-0.8.6/tfduck/bdp_sdk_py/opends/sdk.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/common/defines.py` & `tfduck-bsd-0.8.6/tfduck/common/defines.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/common/extendEncoder.py` & `tfduck-bsd-0.8.6/tfduck/common/extendEncoder.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/main.py` & `tfduck-bsd-0.8.6/tfduck/main.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/oss/oss.py` & `tfduck-bsd-0.8.6/tfduck/oss/oss.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                              self.gconf.oss_access_key, self.gconf.oss_endpoint)
     oss_file_path = self.gconf.oss_result_key
     aoss.bucket.put_object_from_file(oss_file_path, local_file_path)
     """
 
     def __init__(self, bucket_name, aly_access_key_id, aly_access_key_secret,
                  aly_endpoint,
-                 pool_connections=210, pool_maxsize=210, timeout=None):
+                 pool_connections=210, pool_maxsize=210, timeout=None, retry_time_sleep=None):
         """
         @des:初始化
         """
         self.access_key_id = aly_access_key_id
         self.access_key_secret = aly_access_key_secret
         self.bucket_name = bucket_name
         # oss-us-east-1.aliyuncs.com
@@ -57,14 +57,15 @@
         oss_session = OssSession(pool_connections, pool_maxsize)
         self.bucket = oss2.Bucket(oss2.Auth(self.access_key_id, self.access_key_secret),
                                   self.endpoint, self.bucket_name, session=oss_session,
                                   connect_timeout=timeout
                                   # connect_timeout = 60
                                   # connect_timeout=(30, 300)  # 这个参数可以用tuple，看了原来，是支持的，(connect_timeout, read_timeout)
                                   )
+        self.retry_time_sleep = retry_time_sleep
 
     def gen_local_unique_file(self, ext="csv"):
         """
         @des:生成本地文件唯一路径
         """
         if BMOBJ.get_current_env() == "server":
             media_root = settings.MEDIA_ROOT
@@ -217,15 +218,18 @@
                 BMOBJ.clog(
                     ctx, f"{local_file} download status {result.status}, sub time {_e-_s}", )
                 break
             except Exception as e:
                 BMOBJ.clog(
                     ctx, f"{local_file} download oss fail, repeat {i}, error: {e}")
                 if i < retry_count-1:
-                    sleep_time = random.randint(60, 120)
+                    if self.retry_time_sleep is None:
+                        sleep_time = random.randint(60, 120)
+                    else:
+                        sleep_time = self.retry_time_sleep
                     time.sleep(sleep_time)
                     continue
                 else:
                     BMOBJ.clog(
                         ctx, f"{local_file} download oss finally fail: {e}")
                     raise Et(2, f"download fail {td_file} {local_file}")
 
@@ -306,15 +310,18 @@
                     ctx, f"{local_file} upload status {result.status}, sub time {_e-_s}", )
                 break
             except Exception as e:
                 BMOBJ.clog(
                     ctx, f"{local_file} upload oss fail, repeat {i}, error: {e}")
                 #
                 if i < retry_count-1:
-                    sleep_time = random.randint(60, 120)
+                    if self.retry_time_sleep is None:
+                        sleep_time = random.randint(60, 120)
+                    else:
+                        sleep_time = self.retry_time_sleep
                     time.sleep(sleep_time)
                     continue
                 else:
                     BMOBJ.clog(
                         ctx, f"{local_file} upload oss finally fail: {e}")
                     raise Et(2, f"upload fail {td_file} {local_file}")
```

### Comparing `tfduck-bsd-0.8.5/tfduck/pyspark_k8s/k8s_manage.py` & `tfduck-bsd-0.8.6/tfduck/pyspark_k8s/k8s_manage.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/pyspark_k8s/spark_manage.py` & `tfduck-bsd-0.8.6/tfduck/pyspark_k8s/spark_manage.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/s3/s3oper.py` & `tfduck-bsd-0.8.6/tfduck/s3/s3oper.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/tga/tga.py` & `tfduck-bsd-0.8.6/tfduck/tga/tga.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck/thinkdata/query.py` & `tfduck-bsd-0.8.6/tfduck/thinkdata/query.py`

 * *Files identical despite different names*

### Comparing `tfduck-bsd-0.8.5/tfduck_bsd.egg-info/PKG-INFO` & `tfduck-bsd-0.8.6/tfduck_bsd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfduck-bsd
-Version: 0.8.5
+Version: 0.8.6
 Summary: A small example package
 Home-page: UNKNOWN
 Author: yuanxiao
 Author-email: yuan6785@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tfduck-bsd-0.8.5/tfduck_bsd.egg-info/SOURCES.txt` & `tfduck-bsd-0.8.6/tfduck_bsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*


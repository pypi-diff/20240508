# Comparing `tmp/dhuodata_lib-0.2.9.tar.gz` & `tmp/dhuodata_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.2.9.tar", last modified: Wed May  8 00:01:13 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.3.0.tar", last modified: Wed May  8 00:57:11 2024, max compression
```

## Comparing `dhuodata_lib-0.2.9.tar` & `dhuodata_lib-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:01:13.267854 dhuodata_lib-0.2.9/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 00:01:13.267854 dhuodata_lib-0.2.9/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.9/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-08 00:01:13.267854 dhuodata_lib-0.2.9/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-08 00:01:00.000000 dhuodata_lib-0.2.9/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:01:13.263854 dhuodata_lib-0.2.9/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:01:13.263854 dhuodata_lib-0.2.9/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 00:01:13.000000 dhuodata_lib-0.2.9/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-08 00:01:13.000000 dhuodata_lib-0.2.9/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-08 00:01:13.000000 dhuodata_lib-0.2.9/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-08 00:01:13.000000 dhuodata_lib-0.2.9/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-08 00:01:13.000000 dhuodata_lib-0.2.9/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:01:13.263854 dhuodata_lib-0.2.9/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.9/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.2.9/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     7008 2024-05-07 23:52:34.000000 dhuodata_lib-0.2.9/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.2.9/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.2.9/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     2000 2024-05-08 00:00:53.000000 dhuodata_lib-0.2.9/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      789 2024-05-07 16:57:09.000000 dhuodata_lib-0.2.9/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.2.9/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:01:13.263854 dhuodata_lib-0.2.9/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.2.9/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:57:11.221367 dhuodata_lib-0.3.0/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 00:57:11.221367 dhuodata_lib-0.3.0/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.0/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-08 00:57:11.221367 dhuodata_lib-0.3.0/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-08 00:56:40.000000 dhuodata_lib-0.3.0/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:57:11.221367 dhuodata_lib-0.3.0/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:57:11.221367 dhuodata_lib-0.3.0/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 00:57:11.000000 dhuodata_lib-0.3.0/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-08 00:57:11.000000 dhuodata_lib-0.3.0/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-08 00:57:11.000000 dhuodata_lib-0.3.0/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-08 00:57:11.000000 dhuodata_lib-0.3.0/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-08 00:57:11.000000 dhuodata_lib-0.3.0/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:57:11.221367 dhuodata_lib-0.3.0/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.0/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.3.0/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     7008 2024-05-07 23:52:34.000000 dhuodata_lib-0.3.0/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.3.0/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.3.0/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1995 2024-05-08 00:57:02.000000 dhuodata_lib-0.3.0/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      789 2024-05-07 16:57:09.000000 dhuodata_lib-0.3.0/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.3.0/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 00:57:11.221367 dhuodata_lib-0.3.0/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.3.0/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.2.9/PKG-INFO` & `dhuodata_lib-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.9
+Version: 0.3.0
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.2.9/README.md` & `dhuodata_lib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.9/setup.py` & `dhuodata_lib-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.2.9",
+    version="0.3.0",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.2.9/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.3.0/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.9
+Version: 0.3.0
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.2.9/src/dhuolib/clients.py` & `dhuodata_lib-0.3.0/src/dhuolib/clients.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.9/src/dhuolib/predict.py` & `dhuodata_lib-0.3.0/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.9/src/dhuolib/services.py` & `dhuodata_lib-0.3.0/src/dhuolib/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 
         if 'model_pkl_file' in experiment_params.keys():
             return requests.post(
                 f"{self.service_endpoint}/save", data=experiment_params, headers={"Content-Type": "multipart/form-data"}
             )
             
         print(experiment_params)
-        return requests.post(
-            f"{self.service_endpoint}/save", data=experiment_params, headers=self.headers)
-    
+        return requests.post(f"{self.service_endpoint}/save", data=json.dumps(experiment_params), headers=self.headers)
+
     def run_experiment(self, params):
         if params is None and isinstance(params, str):
             raise ValueError("json_data must be a dict")
         
         response = requests.post(
             f"{self.service_endpoint}/run",
             data=params,
```

### Comparing `dhuodata_lib-0.2.9/src/dhuolib/validations.py` & `dhuodata_lib-0.3.0/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.9/tests/test_dhuolib.py` & `dhuodata_lib-0.3.0/tests/test_dhuolib.py`

 * *Files identical despite different names*


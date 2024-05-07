# Comparing `tmp/dhuodata_lib-0.2.6.tar.gz` & `tmp/dhuodata_lib-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.2.6.tar", last modified: Tue May  7 18:33:30 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.2.7.tar", last modified: Tue May  7 18:51:25 2024, max compression
```

## Comparing `dhuodata_lib-0.2.6.tar` & `dhuodata_lib-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:33:30.869717 dhuodata_lib-0.2.6/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 18:33:30.869717 dhuodata_lib-0.2.6/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.6/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-07 18:33:30.869717 dhuodata_lib-0.2.6/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-07 18:33:23.000000 dhuodata_lib-0.2.6/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:33:30.869717 dhuodata_lib-0.2.6/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:33:30.869717 dhuodata_lib-0.2.6/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 18:33:30.000000 dhuodata_lib-0.2.6/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-07 18:33:30.000000 dhuodata_lib-0.2.6/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-07 18:33:30.000000 dhuodata_lib-0.2.6/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-07 18:33:30.000000 dhuodata_lib-0.2.6/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-07 18:33:30.000000 dhuodata_lib-0.2.6/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:33:30.869717 dhuodata_lib-0.2.6/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.6/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.2.6/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     6880 2024-05-07 16:59:59.000000 dhuodata_lib-0.2.6/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.2.6/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.2.6/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     2122 2024-05-07 18:33:14.000000 dhuodata_lib-0.2.6/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      789 2024-05-07 16:57:09.000000 dhuodata_lib-0.2.6/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.2.6/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:33:30.869717 dhuodata_lib-0.2.6/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.2.6/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.7/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-07 18:51:18.000000 dhuodata_lib-0.2.7/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.7/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.2.7/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     6867 2024-05-07 18:47:09.000000 dhuodata_lib-0.2.7/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.2.7/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.2.7/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2254 2024-05-07 18:48:54.000000 dhuodata_lib-0.2.7/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      789 2024-05-07 16:57:09.000000 dhuodata_lib-0.2.7/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.2.7/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.2.7/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.2.6/PKG-INFO` & `dhuodata_lib-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.6
+Version: 0.2.7
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.2.6/README.md` & `dhuodata_lib-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.6/setup.py` & `dhuodata_lib-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.2.6",
+    version="0.2.7",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.2.6/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.6
+Version: 0.2.7
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.2.6/src/dhuolib/clients.py` & `dhuodata_lib-0.2.7/src/dhuolib/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                     return {"error": str(e)}
 
                 response = self.service.create_experiment_by_conf_json(
                     experiment_params=experiment_params, files=files
                 )
             else:
                 response = self.service.create_experiment_by_conf_json(
-                    experiment_params=experiment_params, files=files
+                    experiment_params=experiment_params
                 )
 
             experiment = response.json()
             logger.info(
                 f"Experiment Name: {experiment_params['experiment_name']}"
                 f"Experiment ID: {experiment['experiment_id']} created"
             )
```

### Comparing `dhuodata_lib-0.2.6/src/dhuolib/predict.py` & `dhuodata_lib-0.2.7/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.6/src/dhuolib/services.py` & `dhuodata_lib-0.2.7/src/dhuolib/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 
         if not isinstance(service_endpoint, str):
             raise ValueError("service_endpoint must be a string")
 
         self.service_endpoint = f"{service_endpoint}/api/experiment"
         self.headers = {"Content-Type": "application/json"}
 
-    def create_experiment_by_conf_json(self, experiment_params, files):
+    def create_experiment_by_conf_json(self, experiment_params, files=None):
         if experiment_params is None and isinstance(experiment_params, dict):
             raise ValueError("json_data must be a dict")
 
-        response = requests.post(
-            f"{self.service_endpoint}/save", data=experiment_params, files=files, headers={"Content-Type": "multipart/form-data"}
-        )
-        return response
-
+        if files:
+            return requests.post(
+                f"{self.service_endpoint}/save", data=experiment_params, files=files, headers={"Content-Type": "multipart/form-data"}
+            )
+        return requests.post(
+            f"{self.service_endpoint}/save", data=experiment_params, headers=self.headers)
+    
     def run_experiment(self, run_params, files=None):
         if run_params is None and isinstance(run_params, str):
             raise ValueError("json_data must be a dict")
         if files:
             response = requests.post(
                 f"{self.service_endpoint}/run",
                 data=run_params,
```

### Comparing `dhuodata_lib-0.2.6/src/dhuolib/validations.py` & `dhuodata_lib-0.2.7/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.6/tests/test_dhuolib.py` & `dhuodata_lib-0.2.7/tests/test_dhuolib.py`

 * *Files identical despite different names*


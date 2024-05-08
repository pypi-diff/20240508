# Comparing `tmp/dhuodata_lib-0.3.4.tar.gz` & `tmp/dhuodata_lib-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.3.4.tar", last modified: Wed May  8 01:50:29 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.3.5.tar", last modified: Wed May  8 13:28:24 2024, max compression
```

## Comparing `dhuodata_lib-0.3.4.tar` & `dhuodata_lib-0.3.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:50:29.257039 dhuodata_lib-0.3.4/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 01:50:29.257039 dhuodata_lib-0.3.4/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.4/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-08 01:50:29.257039 dhuodata_lib-0.3.4/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-08 01:49:56.000000 dhuodata_lib-0.3.4/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:50:29.253039 dhuodata_lib-0.3.4/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:50:29.253039 dhuodata_lib-0.3.4/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 01:50:29.000000 dhuodata_lib-0.3.4/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-08 01:50:29.000000 dhuodata_lib-0.3.4/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-08 01:50:29.000000 dhuodata_lib-0.3.4/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-08 01:50:29.000000 dhuodata_lib-0.3.4/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-08 01:50:29.000000 dhuodata_lib-0.3.4/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:50:29.253039 dhuodata_lib-0.3.4/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.4/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.3.4/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     7257 2024-05-08 01:50:20.000000 dhuodata_lib-0.3.4/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.3.4/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.3.4/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1900 2024-05-08 01:43:38.000000 dhuodata_lib-0.3.4/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-08 01:22:24.000000 dhuodata_lib-0.3.4/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.3.4/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:50:29.253039 dhuodata_lib-0.3.4/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.3.4/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 13:28:24.788027 dhuodata_lib-0.3.5/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 13:28:24.788027 dhuodata_lib-0.3.5/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.5/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-08 13:28:24.788027 dhuodata_lib-0.3.5/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-08 13:28:06.000000 dhuodata_lib-0.3.5/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 13:28:24.788027 dhuodata_lib-0.3.5/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 13:28:24.788027 dhuodata_lib-0.3.5/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 13:28:24.000000 dhuodata_lib-0.3.5/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-08 13:28:24.000000 dhuodata_lib-0.3.5/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-08 13:28:24.000000 dhuodata_lib-0.3.5/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-08 13:28:24.000000 dhuodata_lib-0.3.5/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-08 13:28:24.000000 dhuodata_lib-0.3.5/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 13:28:24.788027 dhuodata_lib-0.3.5/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.5/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.3.5/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     7171 2024-05-08 13:26:40.000000 dhuodata_lib-0.3.5/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.3.5/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.3.5/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1940 2024-05-08 13:24:45.000000 dhuodata_lib-0.3.5/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-08 01:22:24.000000 dhuodata_lib-0.3.5/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.3.5/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 13:28:24.788027 dhuodata_lib-0.3.5/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.3.5/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.3.4/PKG-INFO` & `dhuodata_lib-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.4
+Version: 0.3.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.3.4/README.md` & `dhuodata_lib-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.4/setup.py` & `dhuodata_lib-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.3.4",
+    version="0.3.5",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.3.4/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.3.5/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.4
+Version: 0.3.5
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.3.4/src/dhuolib/clients.py` & `dhuodata_lib-0.3.5/src/dhuolib/clients.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,43 +60,41 @@
         logger.info(
             f"Experiment Name: {params['experiment_name']}"
             f"Experiment ID: {experiment['experiment_id']} created"
         )
         return experiment
 
     def run_experiment(self, params) -> dict:
-        run_params = {}
         try:
             RunExperimentBody.parse_obj(params)
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
         
         try:
             with open(params["requirements_file"], "rb") as f1, open(
                 params["model_pkl_file"], "rb"
             ) as f2:
-                run_params = {
+                files = {
                     "requirements_file": FileStorage(
                         stream=f1, filename="requirements.txt", content_type="text/plain"
                     ),
                     "model_pkl_file": FileStorage(
                         stream=f2,
                         filename="model.pkl",
                         content_type="application/octet-stream",
                     ),
                 }
-                
-                run_params = {**run_params, **params}
-                if run_params["experiment_id"] is None:
-                    experiment_id = self.create_experiment(run_params)
-                    run_params["experiment_id"] = experiment_id
+             
+                if params["experiment_id"] is None:
+                    experiment_id = self.create_experiment(params)
+                    params["experiment_id"] = experiment_id
 
-                response = self.service.run_experiment(run_params)
-                logger.info(f"Experiment ID: {run_params['experiment_id']} running")
+                response = self.service.run_experiment(params=params, files=files)
+                logger.info(f"Experiment ID: {params['experiment_id']} running")
                 return response.json()
         except FileNotFoundError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
 
     def create_model(self, model_params) -> dict:
         try:
```

### Comparing `dhuodata_lib-0.3.4/src/dhuolib/predict.py` & `dhuodata_lib-0.3.5/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.4/src/dhuolib/services.py` & `dhuodata_lib-0.3.5/src/dhuolib/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,22 @@
         if 'model_pkl_file' in experiment_params.keys():
             return requests.post(
                 f"{self.service_endpoint}/save", data=experiment_params, headers={"Content-Type": "multipart/form-data"}
             )
             
         return requests.post(f"{self.service_endpoint}/save", data=json.dumps(experiment_params), headers=self.headers)
 
-    def run_experiment(self, params):
+    def run_experiment(self, params={}, files=None):
         if params is None and isinstance(params, str):
             raise ValueError("json_data must be a dict")
         
         response = requests.post(
             f"{self.service_endpoint}/run",
-            data=params
+            data=params,
+            files=files
         )
         return response
 
     def create_model(self, model_params):
         if model_params is None and not isinstance(model_params, dict):
             raise ValueError("json_data must be a dict")
         response = requests.post(
```

### Comparing `dhuodata_lib-0.3.4/src/dhuolib/validations.py` & `dhuodata_lib-0.3.5/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.4/tests/test_dhuolib.py` & `dhuodata_lib-0.3.5/tests/test_dhuolib.py`

 * *Files identical despite different names*


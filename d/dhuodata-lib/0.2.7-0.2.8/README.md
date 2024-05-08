# Comparing `tmp/dhuodata_lib-0.2.7.tar.gz` & `tmp/dhuodata_lib-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.2.7.tar", last modified: Tue May  7 18:51:25 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.2.8.tar", last modified: Tue May  7 23:54:17 2024, max compression
```

## Comparing `dhuodata_lib-0.2.7.tar` & `dhuodata_lib-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.7/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-07 18:51:18.000000 dhuodata_lib-0.2.7/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-07 18:51:25.000000 dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.7/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.2.7/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     6867 2024-05-07 18:47:09.000000 dhuodata_lib-0.2.7/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.2.7/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.2.7/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     2254 2024-05-07 18:48:54.000000 dhuodata_lib-0.2.7/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      789 2024-05-07 16:57:09.000000 dhuodata_lib-0.2.7/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.2.7/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 18:51:25.292645 dhuodata_lib-0.2.7/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.2.7/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 23:54:17.532149 dhuodata_lib-0.2.8/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 23:54:17.532149 dhuodata_lib-0.2.8/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.8/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-07 23:54:17.532149 dhuodata_lib-0.2.8/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-07 23:51:04.000000 dhuodata_lib-0.2.8/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 23:54:17.532149 dhuodata_lib-0.2.8/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 23:54:17.532149 dhuodata_lib-0.2.8/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-07 23:54:17.000000 dhuodata_lib-0.2.8/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-07 23:54:17.000000 dhuodata_lib-0.2.8/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-07 23:54:17.000000 dhuodata_lib-0.2.8/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-07 23:54:17.000000 dhuodata_lib-0.2.8/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-07 23:54:17.000000 dhuodata_lib-0.2.8/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 23:54:17.532149 dhuodata_lib-0.2.8/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.2.8/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.2.8/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     7008 2024-05-07 23:52:34.000000 dhuodata_lib-0.2.8/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.2.8/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.2.8/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1966 2024-05-07 23:47:10.000000 dhuodata_lib-0.2.8/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      789 2024-05-07 16:57:09.000000 dhuodata_lib-0.2.8/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.2.8/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-07 23:54:17.532149 dhuodata_lib-0.2.8/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.2.8/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.2.7/PKG-INFO` & `dhuodata_lib-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.7
+Version: 0.2.8
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.2.7/README.md` & `dhuodata_lib-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.7/setup.py` & `dhuodata_lib-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.2.7",
+    version="0.2.8",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.2.7/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.2.8/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.2.7
+Version: 0.2.8
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.2.7/src/dhuolib/clients.py` & `dhuodata_lib-0.2.8/src/dhuolib/clients.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,136 +1,133 @@
 from pydantic import ValidationError
 import json
 from dhuolib.config import logger
 from dhuolib.services import ServiceAPIML
 from dhuolib.validations import ExperimentBody, RunExperimentBody, PredictModelBody
+from werkzeug.datastructures import FileStorage
 
 
 class DhuolibClient:
     def __init__(self, service_endpoint=None):
         if not service_endpoint:
             raise ValueError("service_endpoint is required")
 
         self.service = ServiceAPIML(service_endpoint)
 
     def create_experiment(self, experiment_params: dict) -> dict:
-        files = {}
+        params = {}
         response = None
         try:
             ExperimentBody.parse_obj(experiment_params)
-            experiment_params["experiment_tags"] = json.dumps(
+            params["experiment_tags"] = json.dumps(
                 experiment_params["experiment_tags"]
             )
-            if "requirements_file" in experiment_params.keys() and "model_pkl_file" in experiment_params.keys() :
+            if "requirements_file" in experiment_params.keys() and "model_pkl_file" in experiment_params.keys():
                 try:
-                    files = {
-                        "requirements_file": (
-                            "requirements.txt",
-                            open(experiment_params["requirements_file"], "rb"),
-                            "text/plain",
-                        ),
-                        "model_pkl_file": (
-                            "model.pkl",
-                            open(experiment_params["model_pkl_file"], "rb"),
-                            "application/octet-stream",
-                        ),
-                    }
+                    with open(experiment_params["requirements_file"], "rb") as f1, open(
+                        experiment_params["model_pkl_file"], "rb"
+                    ) as f2:
+                        params = {
+                            "requirements_file": FileStorage(
+                                stream=f1, filename="requirements.txt", content_type="text/plain"
+                            ),
+                            "model_pkl_file": FileStorage(
+                                stream=f2,
+                                filename="model.pkl",
+                                content_type="application/octet-stream",
+                            ),
+                        }
                 except FileNotFoundError as e:
                     logger.error(f"Error: {e}")
                     return {"error": str(e)}
-
-                response = self.service.create_experiment_by_conf_json(
-                    experiment_params=experiment_params, files=files
-                )
-            else:
-                response = self.service.create_experiment_by_conf_json(
-                    experiment_params=experiment_params
-                )
+           
+            params = {**params, **experiment_params}
+            response = self.service.create_experiment_by_conf_json(params)
 
             experiment = response.json()
             logger.info(
-                f"Experiment Name: {experiment_params['experiment_name']}"
+                f"Experiment Name: {params['experiment_name']}"
                 f"Experiment ID: {experiment['experiment_id']} created"
             )
             return experiment
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
 
-    def run_experiment(self, run_params) -> dict:
-        files = {}
+    def run_experiment(self, params) -> dict:
+        run_params = {}
         try:
-            RunExperimentBody.parse_obj(run_params)
-            
+            RunExperimentBody.parse_obj(params)
             try:
-                files = {
-                    "requirements_file": (
-                        "requirements.txt",
-                        open(run_params["requirements_file"], "rb"),
-                        "text/plain",
-                    ),
-                    "model_pkl_file": (
-                        "model.pkl",
-                        open(run_params["model_pkl_file"], "rb"),
-                        "application/octet-stream",
-                    ),
-                }
+                with open(params["requirements_file"], "rb") as f1, open(
+                    params["model_pkl_file"], "rb"
+                ) as f2:
+                    run_params = {
+                        "requirements_file": FileStorage(
+                            stream=f1, filename="requirements.txt", content_type="text/plain"
+                        ),
+                        "model_pkl_file": FileStorage(
+                            stream=f2,
+                            filename="model.pkl",
+                            content_type="application/octet-stream",
+                        ),
+                    }
             except FileNotFoundError as e:
                 logger.error(f"Error: {e}")
                 return {"error": str(e)}
-            
-            if run_params["experiment_id"] is None:
-                experiment_id = self.create_experiment(
-                    run_params=run_params)
+
+            if params["experiment_id"] is not None:
+                experiment_id = self.create_experiment(run_params)
                 run_params["experiment_id"] = experiment_id
+            else:
+                run_params["experiment_id"] = params['experiment_id']
 
-            response = self.service.run_experiment(run_params=run_params, files=files)
+            response = self.service.run_experiment(run_params)
             logger.info(f"Experiment ID: {run_params['experiment_id']} running")
             return response.json()
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
-        
+
     def create_model(self, model_params) -> dict:
         try:
             if model_params["stage"] is None:
                 model_params["stage"] = "STAGING"
-            
+
             response = self.service.create_model(model_params)
             logger.info(f"Model Name: {model_params['modelname']} created")
             return response.json()
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
-        
+
     def predict_online(self, run_params) -> dict:
-        files = {}
+        params = {}
         try:
             PredictModelBody.parse_obj(run_params)
-            
+
             try:
-                files = {
-                    "data": (
-                        "data_predict.csv",
-                        open(run_params["data"], "rb"),
-                        "csv",
-                    )
-                }
+                with open(run_params["data"], "rb") as f1:
+                    params = {
+                        "data": FileStorage(
+                            stream=f1, filename="data.csv", content_type="csv"
+                        )
+                    }
+                    params = {**params, **run_params}
             except FileNotFoundError as e:
                 logger.error(f"Error: {e}")
                 return {"error": str(e)}
-        
-            response = self.service.predict_online(run_params=run_params, files=files)
-            logger.info(f"Model Name: {run_params['modelname']} predictions")
+
+            response = self.service.predict_online(params)
+            logger.info(f"Model Name: {params['modelname']} predictions")
             return response.json()
-        
+
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
-        
 
     def load_model(self, model_name, tag) -> str:
         print("loading model")
         return "model_name.pkl"
 
     def predict(self):
         pass
```

### Comparing `dhuodata_lib-0.2.7/src/dhuolib/predict.py` & `dhuodata_lib-0.2.8/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.7/src/dhuolib/services.py` & `dhuodata_lib-0.2.8/src/dhuolib/services.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,54 +8,46 @@
 
         if not isinstance(service_endpoint, str):
             raise ValueError("service_endpoint must be a string")
 
         self.service_endpoint = f"{service_endpoint}/api/experiment"
         self.headers = {"Content-Type": "application/json"}
 
-    def create_experiment_by_conf_json(self, experiment_params, files=None):
+    def create_experiment_by_conf_json(self, experiment_params):
         if experiment_params is None and isinstance(experiment_params, dict):
             raise ValueError("json_data must be a dict")
 
-        if files:
+        if 'model_pkl_file' in experiment_params.keys():
             return requests.post(
-                f"{self.service_endpoint}/save", data=experiment_params, files=files, headers={"Content-Type": "multipart/form-data"}
+                f"{self.service_endpoint}/save", data=experiment_params, headers={"Content-Type": "multipart/form-data"}
             )
         return requests.post(
-            f"{self.service_endpoint}/save", data=experiment_params, headers=self.headers)
+            f"{self.service_endpoint}/save", data=json.dumps(experiment_params), headers=self.headers)
     
-    def run_experiment(self, run_params, files=None):
-        if run_params is None and isinstance(run_params, str):
+    def run_experiment(self, params):
+        if params is None and isinstance(params, str):
             raise ValueError("json_data must be a dict")
-        if files:
-            response = requests.post(
-                f"{self.service_endpoint}/run",
-                data=run_params,
-                files=files,
-                headers={"Content-Type": "multipart/form-data"},
-            )
-            return response
-
+        
         response = requests.post(
             f"{self.service_endpoint}/run",
-            data=json.dumps(run_params),
-            headers=self.headers,
+            data=params,
+            headers={"Content-Type": "multipart/form-data"},
         )
         return response
 
     def create_model(self, model_params):
         if model_params is None and not isinstance(model_params, dict):
             raise ValueError("json_data must be a dict")
         response = requests.post(
             f"{self.service_endpoint}/model",
             data=json.dumps(model_params),
             headers=self.headers,
         )
         return response
 
-    def predict_online(self, run_params, files):
-        if run_params is None and not isinstance(run_params, dict):
+    def predict_online(self, params):
+        if params is None and not isinstance(params, dict):
             raise ValueError("json_data must be a dict")
         response = requests.post(
-            f"{self.service_endpoint}/predict_online", data=run_params, files=files, headers={"Content-Type": "multipart/form-data"}
+            f"{self.service_endpoint}/predict_online", data=params, headers={"Content-Type": "multipart/form-data"}
         )
         return response
```

### Comparing `dhuodata_lib-0.2.7/src/dhuolib/validations.py` & `dhuodata_lib-0.2.8/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.2.7/tests/test_dhuolib.py` & `dhuodata_lib-0.2.8/tests/test_dhuolib.py`

 * *Files identical despite different names*


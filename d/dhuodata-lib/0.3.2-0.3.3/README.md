# Comparing `tmp/dhuodata_lib-0.3.2.tar.gz` & `tmp/dhuodata_lib-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.3.2.tar", last modified: Wed May  8 01:31:53 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.3.3.tar", last modified: Wed May  8 01:43:57 2024, max compression
```

## Comparing `dhuodata_lib-0.3.2.tar` & `dhuodata_lib-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:31:53.425919 dhuodata_lib-0.3.2/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 01:31:53.425919 dhuodata_lib-0.3.2/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.2/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-08 01:31:53.425919 dhuodata_lib-0.3.2/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-08 01:30:45.000000 dhuodata_lib-0.3.2/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:31:53.421919 dhuodata_lib-0.3.2/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:31:53.421919 dhuodata_lib-0.3.2/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 01:31:53.000000 dhuodata_lib-0.3.2/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-08 01:31:53.000000 dhuodata_lib-0.3.2/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-08 01:31:53.000000 dhuodata_lib-0.3.2/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-08 01:31:53.000000 dhuodata_lib-0.3.2/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-08 01:31:53.000000 dhuodata_lib-0.3.2/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:31:53.421919 dhuodata_lib-0.3.2/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.2/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.3.2/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     7651 2024-05-08 01:31:36.000000 dhuodata_lib-0.3.2/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.3.2/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.3.2/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1962 2024-05-08 00:57:26.000000 dhuodata_lib-0.3.2/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-08 01:22:24.000000 dhuodata_lib-0.3.2/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.3.2/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:31:53.421919 dhuodata_lib-0.3.2/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.3.2/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:43:57.890067 dhuodata_lib-0.3.3/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 01:43:57.890067 dhuodata_lib-0.3.3/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.3/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-08 01:43:57.890067 dhuodata_lib-0.3.3/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-08 01:43:51.000000 dhuodata_lib-0.3.3/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:43:57.886067 dhuodata_lib-0.3.3/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:43:57.886067 dhuodata_lib-0.3.3/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 01:43:57.000000 dhuodata_lib-0.3.3/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-08 01:43:57.000000 dhuodata_lib-0.3.3/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-08 01:43:57.000000 dhuodata_lib-0.3.3/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-08 01:43:57.000000 dhuodata_lib-0.3.3/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-08 01:43:57.000000 dhuodata_lib-0.3.3/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:43:57.886067 dhuodata_lib-0.3.3/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.3/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.3.3/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     7547 2024-05-08 01:36:19.000000 dhuodata_lib-0.3.3/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.3.3/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.3.3/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1900 2024-05-08 01:43:38.000000 dhuodata_lib-0.3.3/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-08 01:22:24.000000 dhuodata_lib-0.3.3/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.3.3/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 01:43:57.886067 dhuodata_lib-0.3.3/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.3.3/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.3.2/PKG-INFO` & `dhuodata_lib-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.2
+Version: 0.3.3
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.3.2/README.md` & `dhuodata_lib-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.2/setup.py` & `dhuodata_lib-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.3.2",
+    version="0.3.3",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.3.2/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.3.3/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.2
+Version: 0.3.3
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.3.2/src/dhuolib/clients.py` & `dhuodata_lib-0.3.3/src/dhuolib/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,14 @@
                         ),
                     }
                     
                     run_params = {**params, **run_params}
                     if params["experiment_id"] is not None:
                         experiment_id = self.create_experiment(run_params)
                         run_params["experiment_id"] = experiment_id
-                    else:
-                        run_params["experiment_id"] = params['experiment_id']
 
                     response = self.service.run_experiment(run_params)
                     logger.info(f"Experiment ID: {run_params['experiment_id']} running")
                     return response.json()
             except FileNotFoundError as e:
                 logger.error(f"Error: {e}")
                 return {"error": str(e)}
```

### Comparing `dhuodata_lib-0.3.2/src/dhuolib/predict.py` & `dhuodata_lib-0.3.3/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.2/src/dhuolib/services.py` & `dhuodata_lib-0.3.3/src/dhuolib/services.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,16 +25,15 @@
 
     def run_experiment(self, params):
         if params is None and isinstance(params, str):
             raise ValueError("json_data must be a dict")
         
         response = requests.post(
             f"{self.service_endpoint}/run",
-            data=params,
-            headers={"Content-Type": "multipart/form-data"},
+            data=params
         )
         return response
 
     def create_model(self, model_params):
         if model_params is None and not isinstance(model_params, dict):
             raise ValueError("json_data must be a dict")
         response = requests.post(
```

### Comparing `dhuodata_lib-0.3.2/src/dhuolib/validations.py` & `dhuodata_lib-0.3.3/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.2/tests/test_dhuolib.py` & `dhuodata_lib-0.3.3/tests/test_dhuolib.py`

 * *Files identical despite different names*


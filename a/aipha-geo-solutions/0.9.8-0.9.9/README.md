# Comparing `tmp/aipha_geo_solutions-0.9.8.tar.gz` & `tmp/aipha_geo_solutions-0.9.9.tar.gz`

## Comparing `aipha_geo_solutions-0.9.8.tar` & `aipha_geo_solutions-0.9.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/example.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/requirements.txt
--rw-r--r--   0        0        0   469513 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/src/aipha_geo_solutions/AIPHAProcessing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/src/aipha_geo_solutions/__init__.py
--rw-r--r--   0        0        0   448325 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/src/aipha_geo_solutions/operators.py
--rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/src/aipha_geo_solutions/webservice_api.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/LICENSE
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/example.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/requirements.txt
+-rw-r--r--   0        0        0   469513 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/src/aipha_geo_solutions/AIPHAProcessing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/src/aipha_geo_solutions/__init__.py
+-rw-r--r--   0        0        0   448360 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/src/aipha_geo_solutions/operators.py
+-rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/src/aipha_geo_solutions/webservice_api.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/LICENSE
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.9/PKG-INFO
```

### Comparing `aipha_geo_solutions-0.9.8/example.py` & `aipha_geo_solutions-0.9.9/example.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.9.8/src/aipha_geo_solutions/AIPHAProcessing.py` & `aipha_geo_solutions-0.9.9/src/aipha_geo_solutions/AIPHAProcessing.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.9.8/src/aipha_geo_solutions/operators.py` & `aipha_geo_solutions-0.9.9/src/aipha_geo_solutions/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
           result = json.loads(retried_service[0].text)
           if 'error' in result:
               raise RuntimeError('AIPHAProcessingError: ' + str(result['error']))
           results.append(result)
           break
         except Exception as e:
           if idx == 9:
+            print(retried_service)
             result = json.loads(retried_service[0].text)
             results.append(result)
       raise RuntimeError(str(e))
   
   def await_completion(client, services):
     pid_services = []  
     for service in services:
```

### Comparing `aipha_geo_solutions-0.9.8/src/aipha_geo_solutions/webservice_api.py` & `aipha_geo_solutions-0.9.9/src/aipha_geo_solutions/webservice_api.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.9.8/LICENSE` & `aipha_geo_solutions-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.9.8/pyproject.toml` & `aipha_geo_solutions-0.9.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aipha_geo_solutions"
-version = "0.9.8"
+version = "0.9.9"
 authors = [
   { name="Timo Hackel", email="timo.hackel@aipha.ch" },
 ]
 description = "A python API to the AIPHA webservices"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `aipha_geo_solutions-0.9.8/PKG-INFO` & `aipha_geo_solutions-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipha_geo_solutions
-Version: 0.9.8
+Version: 0.9.9
 Summary: A python API to the AIPHA webservices
 Project-URL: Homepage, https://github.com/AIPHA-Geo-Solutions/
 Project-URL: Bug Tracker, https://github.com/AIPHA-Geo-Solutions/AIPHAPythonAPI/issues
 Author-email: Timo Hackel <timo.hackel@aipha.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


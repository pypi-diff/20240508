# Comparing `tmp/nightingalejsonadapter-2.7.0.tar.gz` & `tmp/nightingalejsonadapter-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nightingalejsonadapter-2.7.0.tar", last modified: Tue May  7 14:05:25 2024, max compression
+gzip compressed data, was "nightingalejsonadapter-2.8.0.tar", last modified: Wed May  8 13:03:54 2024, max compression
```

## Comparing `nightingalejsonadapter-2.7.0.tar` & `nightingalejsonadapter-2.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-07 14:05:25.321929 nightingalejsonadapter-2.7.0/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-07 14:05:25.321929 nightingalejsonadapter-2.7.0/PKG-INFO
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-07 14:05:25.321929 nightingalejsonadapter-2.7.0/nightingalejsonadapter/
--rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:22:01.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter/__init__.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      452 2023-04-05 17:04:25.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter/intervention_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      700 2024-05-03 18:33:03.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter/patient_info_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      434 2024-05-02 14:49:08.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter/trigger_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      516 2023-03-15 15:22:55.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter/uuid_generator.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      606 2024-05-04 00:53:27.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter/vital_kafka_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      601 2023-04-05 17:04:40.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter/vitals_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      993 2024-05-07 13:41:30.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter/vitals_response.py
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-07 14:05:25.321929 nightingalejsonadapter-2.7.0/nightingalejsonadapter.egg-info/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-07 14:05:25.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter.egg-info/PKG-INFO
--rw-r--r--   0 nuno      (1000) nuno      (1000)      578 2024-05-07 14:05:25.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter.egg-info/SOURCES.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2024-05-07 14:05:25.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter.egg-info/dependency_links.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        9 2024-05-07 14:05:25.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter.egg-info/requires.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       23 2024-05-07 14:05:25.000000 nightingalejsonadapter-2.7.0/nightingalejsonadapter.egg-info/top_level.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2024-05-07 14:05:25.321929 nightingalejsonadapter-2.7.0/setup.cfg
--rw-r--r--   0 nuno      (1000) nuno      (1000)      774 2024-05-07 14:05:18.000000 nightingalejsonadapter-2.7.0/setup.py
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-08 13:03:54.149876 nightingalejsonadapter-2.8.0/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-08 13:03:54.149876 nightingalejsonadapter-2.8.0/PKG-INFO
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-08 13:03:54.149876 nightingalejsonadapter-2.8.0/nightingalejsonadapter/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:22:01.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter/__init__.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      452 2023-04-05 17:04:25.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter/intervention_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      700 2024-05-03 18:33:03.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter/patient_info_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      434 2024-05-02 14:49:08.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter/trigger_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      516 2023-03-15 15:22:55.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter/uuid_generator.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      606 2024-05-04 00:53:27.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter/vital_kafka_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      601 2023-04-05 17:04:40.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter/vitals_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)     1019 2024-05-08 13:02:29.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter/vitals_response.py
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-08 13:03:54.149876 nightingalejsonadapter-2.8.0/nightingalejsonadapter.egg-info/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-08 13:03:54.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter.egg-info/PKG-INFO
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      578 2024-05-08 13:03:54.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter.egg-info/SOURCES.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2024-05-08 13:03:54.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter.egg-info/dependency_links.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        9 2024-05-08 13:03:54.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter.egg-info/requires.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)       23 2024-05-08 13:03:54.000000 nightingalejsonadapter-2.8.0/nightingalejsonadapter.egg-info/top_level.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2024-05-08 13:03:54.149876 nightingalejsonadapter-2.8.0/setup.cfg
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      774 2024-05-08 13:02:39.000000 nightingalejsonadapter-2.8.0/setup.py
```

### Comparing `nightingalejsonadapter-2.7.0/nightingalejsonadapter/patient_info_adapter.py` & `nightingalejsonadapter-2.8.0/nightingalejsonadapter/patient_info_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.7.0/nightingalejsonadapter/uuid_generator.py` & `nightingalejsonadapter-2.8.0/nightingalejsonadapter/uuid_generator.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.7.0/nightingalejsonadapter/vital_kafka_adapter.py` & `nightingalejsonadapter-2.8.0/nightingalejsonadapter/vital_kafka_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.7.0/nightingalejsonadapter/vitals_adapter.py` & `nightingalejsonadapter-2.8.0/nightingalejsonadapter/vitals_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.7.0/nightingalejsonadapter/vitals_response.py` & `nightingalejsonadapter-2.8.0/nightingalejsonadapter/vitals_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     shockIndex: float
 
 
 class Model(BaseModel):
     UUID: str
     timestamp: datetime
     requestId: str
+    globalIncidentId: str
     lastMeasurementTimestamp: datetime
     predictionTimestampId: str
     predictionTimeDeltaMinutes: int
     victimId: str
     procedureMessageCount: int
     procedureMessages: List[ProcedureMessage]
     predictions: List[Prediction]
```

### Comparing `nightingalejsonadapter-2.7.0/nightingalejsonadapter.egg-info/SOURCES.txt` & `nightingalejsonadapter-2.8.0/nightingalejsonadapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.7.0/setup.py` & `nightingalejsonadapter-2.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.7.0' 
+VERSION = '2.8.0' 
 DESCRIPTION = 'JSON adapter'
 LONG_DESCRIPTION = 'JSON adapters and validators for Nightingale Communication and Integration'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="nightingalejsonadapter",
```


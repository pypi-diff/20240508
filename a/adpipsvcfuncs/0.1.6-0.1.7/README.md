# Comparing `tmp/adpipsvcfuncs-0.1.6.tar.gz` & `tmp/adpipsvcfuncs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adpipsvcfuncs-0.1.6.tar", last modified: Fri May  3 01:47:33 2024, max compression
+gzip compressed data, was "adpipsvcfuncs-0.1.7.tar", last modified: Tue May  7 21:56:43 2024, max compression
```

## Comparing `adpipsvcfuncs-0.1.6.tar` & `adpipsvcfuncs-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 01:47:33.328475 adpipsvcfuncs-0.1.6/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-03 01:46:59.000000 adpipsvcfuncs-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      329 2024-05-03 01:47:33.324474 adpipsvcfuncs-0.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-03 01:46:59.000000 adpipsvcfuncs-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 01:47:33.324474 adpipsvcfuncs-0.1.6/adpipsvcfuncs/
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-03 01:46:59.000000 adpipsvcfuncs-0.1.6/adpipsvcfuncs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-05-03 01:46:59.000000 adpipsvcfuncs-0.1.6/adpipsvcfuncs/adpipsvcfuncs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 01:47:33.324474 adpipsvcfuncs-0.1.6/adpipsvcfuncs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      329 2024-05-03 01:47:33.000000 adpipsvcfuncs-0.1.6/adpipsvcfuncs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-03 01:47:33.000000 adpipsvcfuncs-0.1.6/adpipsvcfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 01:47:33.000000 adpipsvcfuncs-0.1.6/adpipsvcfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-05-03 01:47:33.000000 adpipsvcfuncs-0.1.6/adpipsvcfuncs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-03 01:47:33.000000 adpipsvcfuncs-0.1.6/adpipsvcfuncs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 01:47:33.328475 adpipsvcfuncs-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      493 2024-05-03 01:46:59.000000 adpipsvcfuncs-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:56:43.149719 adpipsvcfuncs-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 21:56:02.000000 adpipsvcfuncs-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-07 21:56:43.149719 adpipsvcfuncs-0.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-07 21:56:02.000000 adpipsvcfuncs-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:56:43.145719 adpipsvcfuncs-0.1.7/adpipsvcfuncs/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-07 21:56:02.000000 adpipsvcfuncs-0.1.7/adpipsvcfuncs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-05-07 21:56:02.000000 adpipsvcfuncs-0.1.7/adpipsvcfuncs/adpipsvcfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:56:43.149719 adpipsvcfuncs-0.1.7/adpipsvcfuncs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-07 21:56:43.000000 adpipsvcfuncs-0.1.7/adpipsvcfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-07 21:56:43.000000 adpipsvcfuncs-0.1.7/adpipsvcfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 21:56:43.000000 adpipsvcfuncs-0.1.7/adpipsvcfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2024-05-07 21:56:43.000000 adpipsvcfuncs-0.1.7/adpipsvcfuncs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-07 21:56:43.000000 adpipsvcfuncs-0.1.7/adpipsvcfuncs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 21:56:43.149719 adpipsvcfuncs-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-07 21:56:02.000000 adpipsvcfuncs-0.1.7/setup.py
```

### Comparing `adpipsvcfuncs-0.1.6/LICENSE` & `adpipsvcfuncs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adpipsvcfuncs-0.1.6/adpipsvcfuncs/adpipsvcfuncs.py` & `adpipsvcfuncs-0.1.7/adpipsvcfuncs/adpipsvcfuncs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from google.cloud import pubsub_v1, secretmanager
 import requests
 import logging
+from openai import OpenAI
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)  # Capture DEBUG, INFO, WARNING, ERROR, CRITICAL
 
 def fetch_gcp_secret(secret_name: str) -> str:
     # Fetch Project ID from Metadata Server
     metadata_server_url = "http://metadata/computeMetadata/v1/project/project-id"
@@ -36,8 +37,25 @@
         topic_path = publisher.topic_path(project_id, topic_name)
         data = json.dumps(data).encode("utf-8")
         future = publisher.publish(topic_path, data)
         logger.debug(f"Published message to topic: {topic_name} and project_id: {project_id}")
         return True
     except Exception as e:
         logger.error(f"Failed to publish message: {str(e)}")
-        return False
+        return False
+    
+def openAI_request(api_key: str, role: str, request: str) -> dict:
+    client = OpenAI(api_key=api_key)
+    try:
+        completion = client.chat.completions.create(
+            model="gpt-4-turbo",
+            messages=[
+                {"role": "system", "content": role},
+                {"role": "user", "content": request},
+            ])
+    except Exception as e:
+        logger.error(f"Failed to get completion from OpenAI: {str(e)}")
+        return None
+    return completion
+
+
+
```


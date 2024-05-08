# Comparing `tmp/zeblok_sdk-1.1.0.tar.gz` & `tmp/zeblok_sdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeblok_sdk-1.1.0.tar", last modified: Sat May  4 05:01:02 2024, max compression
+gzip compressed data, was "zeblok_sdk-1.1.1.tar", last modified: Wed May  8 04:11:47 2024, max compression
```

## Comparing `zeblok_sdk-1.1.0.tar` & `zeblok_sdk-1.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.605584 zeblok_sdk-1.1.0/
--rw-rw-rw-   0        0        0      158 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     3730 2024-05-04 05:01:02.604012 zeblok_sdk-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3302 2024-05-04 04:55:41.000000 zeblok_sdk-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 05:01:02.605584 zeblok_sdk-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      876 2024-05-04 04:40:25.000000 zeblok_sdk-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.561550 zeblok_sdk-1.1.0/tests/
--rw-rw-rw-   0        0        0     3913 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/tests/test_auth.py
--rw-rw-rw-   0        0        0     3107 2024-04-05 01:26:57.000000 zeblok_sdk-1.1.0/tests/test_namespace.py
--rw-rw-rw-   0        0        0     7198 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/tests/test_orchestration.py
--rw-rw-rw-   0        0        0    13891 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/tests/test_plan.py
--rw-rw-rw-   0        0        0     9559 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.0/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.575035 zeblok_sdk-1.1.0/zeblok/
--rw-rw-rw-   0        0        0      406 2024-04-10 09:30:10.000000 zeblok_sdk-1.1.0/zeblok/__init__.py
--rw-rw-rw-   0        0        0     9679 2024-05-02 05:12:43.000000 zeblok_sdk-1.1.0/zeblok/api.py
--rw-rw-rw-   0        0        0     2490 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.0/zeblok/auth.py
-drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.584569 zeblok_sdk-1.1.0/zeblok/base/
--rw-rw-rw-   0        0        0        0 2023-11-21 08:39:11.000000 zeblok_sdk-1.1.0/zeblok/base/__init__.py
--rw-rw-rw-   0        0        0     3493 2024-04-10 10:49:32.000000 zeblok_sdk-1.1.0/zeblok/base/base_airuns.py
--rw-rw-rw-   0        0        0     1057 2023-12-20 15:23:23.000000 zeblok_sdk-1.1.0/zeblok/base/base_auth.py
--rw-rw-rw-   0        0        0     5250 2024-05-01 05:23:24.000000 zeblok_sdk-1.1.0/zeblok/base/base_dataset.py
--rw-rw-rw-   0        0        0     1535 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.0/zeblok/base/base_service.py
--rw-rw-rw-   0        0        0      292 2023-11-23 06:00:40.000000 zeblok_sdk-1.1.0/zeblok/base/base_zbl.py
--rw-rw-rw-   0        0        0     9729 2024-05-01 04:41:34.000000 zeblok_sdk-1.1.0/zeblok/dataset.py
--rw-rw-rw-   0        0        0     8945 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.0/zeblok/microservice.py
--rw-rw-rw-   0        0        0     4720 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.0/zeblok/namespace.py
--rw-rw-rw-   0        0        0     8274 2024-05-03 08:09:55.000000 zeblok_sdk-1.1.0/zeblok/orchestration.py
--rw-rw-rw-   0        0        0    14379 2024-05-03 07:28:33.000000 zeblok_sdk-1.1.0/zeblok/pipeline.py
--rw-rw-rw-   0        0        0     6569 2024-05-03 10:47:22.000000 zeblok_sdk-1.1.0/zeblok/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.592406 zeblok_sdk-1.1.0/zeblok/utils/
--rw-rw-rw-   0        0        0        0 2023-11-15 02:39:00.000000 zeblok_sdk-1.1.0/zeblok/utils/__init__.py
--rw-rw-rw-   0        0        0     3261 2024-03-30 04:04:56.000000 zeblok_sdk-1.1.0/zeblok/utils/error_message.py
--rw-rw-rw-   0        0        0     2916 2024-04-30 10:37:29.000000 zeblok_sdk-1.1.0/zeblok/utils/errors.py
--rw-rw-rw-   0        0        0      727 2023-11-02 04:35:55.000000 zeblok_sdk-1.1.0/zeblok/utils/misc.py
--rw-rw-rw-   0        0        0     5347 2023-11-15 02:39:40.000000 zeblok_sdk-1.1.0/zeblok/utils/progressbar.py
--rw-rw-rw-   0        0        0    13599 2024-04-28 03:10:00.000000 zeblok_sdk-1.1.0/zeblok/utils/validations.py
-drwxrwxrwx   0        0        0        0 2024-05-04 05:01:02.602048 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/
--rw-rw-rw-   0        0        0     3730 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      786 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-04 05:01:02.000000 zeblok_sdk-1.1.0/zeblok_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.966150 zeblok_sdk-1.1.1/
+-rw-rw-rw-   0        0        0      158 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0     3730 2024-05-08 04:11:47.965147 zeblok_sdk-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3302 2024-05-04 04:55:41.000000 zeblok_sdk-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 04:11:47.966150 zeblok_sdk-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-05-04 04:40:25.000000 zeblok_sdk-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.917597 zeblok_sdk-1.1.1/tests/
+-rw-rw-rw-   0        0        0     3913 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/tests/test_auth.py
+-rw-rw-rw-   0        0        0     3107 2024-04-05 01:26:57.000000 zeblok_sdk-1.1.1/tests/test_namespace.py
+-rw-rw-rw-   0        0        0     7198 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/tests/test_orchestration.py
+-rw-rw-rw-   0        0        0    13891 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/tests/test_plan.py
+-rw-rw-rw-   0        0        0     9559 2024-04-04 11:34:04.000000 zeblok_sdk-1.1.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.933167 zeblok_sdk-1.1.1/zeblok/
+-rw-rw-rw-   0        0        0      406 2024-05-07 09:16:30.000000 zeblok_sdk-1.1.1/zeblok/__init__.py
+-rw-rw-rw-   0        0        0     9679 2024-05-02 05:12:43.000000 zeblok_sdk-1.1.1/zeblok/api.py
+-rw-rw-rw-   0        0        0     2490 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.1/zeblok/auth.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.942945 zeblok_sdk-1.1.1/zeblok/base/
+-rw-rw-rw-   0        0        0        0 2023-11-21 08:39:11.000000 zeblok_sdk-1.1.1/zeblok/base/__init__.py
+-rw-rw-rw-   0        0        0     3493 2024-04-10 10:49:32.000000 zeblok_sdk-1.1.1/zeblok/base/base_airuns.py
+-rw-rw-rw-   0        0        0     1057 2023-12-20 15:23:23.000000 zeblok_sdk-1.1.1/zeblok/base/base_auth.py
+-rw-rw-rw-   0        0        0     5250 2024-05-01 05:23:24.000000 zeblok_sdk-1.1.1/zeblok/base/base_dataset.py
+-rw-rw-rw-   0        0        0     1535 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.1/zeblok/base/base_service.py
+-rw-rw-rw-   0        0        0      292 2023-11-23 06:00:40.000000 zeblok_sdk-1.1.1/zeblok/base/base_zbl.py
+-rw-rw-rw-   0        0        0    10366 2024-05-07 09:04:39.000000 zeblok_sdk-1.1.1/zeblok/dataset.py
+-rw-rw-rw-   0        0        0     8945 2024-04-05 00:33:45.000000 zeblok_sdk-1.1.1/zeblok/microservice.py
+-rw-rw-rw-   0        0        0     4720 2023-12-20 09:11:18.000000 zeblok_sdk-1.1.1/zeblok/namespace.py
+-rw-rw-rw-   0        0        0     8274 2024-05-03 08:09:55.000000 zeblok_sdk-1.1.1/zeblok/orchestration.py
+-rw-rw-rw-   0        0        0    14379 2024-05-03 07:28:33.000000 zeblok_sdk-1.1.1/zeblok/pipeline.py
+-rw-rw-rw-   0        0        0     6569 2024-05-03 10:47:22.000000 zeblok_sdk-1.1.1/zeblok/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.953529 zeblok_sdk-1.1.1/zeblok/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-15 02:39:00.000000 zeblok_sdk-1.1.1/zeblok/utils/__init__.py
+-rw-rw-rw-   0        0        0     3261 2024-03-30 04:04:56.000000 zeblok_sdk-1.1.1/zeblok/utils/error_message.py
+-rw-rw-rw-   0        0        0     3045 2024-05-07 08:40:36.000000 zeblok_sdk-1.1.1/zeblok/utils/errors.py
+-rw-rw-rw-   0        0        0      727 2023-11-02 04:35:55.000000 zeblok_sdk-1.1.1/zeblok/utils/misc.py
+-rw-rw-rw-   0        0        0     5347 2023-11-15 02:39:40.000000 zeblok_sdk-1.1.1/zeblok/utils/progressbar.py
+-rw-rw-rw-   0        0        0    13599 2024-04-28 03:10:00.000000 zeblok_sdk-1.1.1/zeblok/utils/validations.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:11:47.964137 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/
+-rw-rw-rw-   0        0        0     3730 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 04:11:47.000000 zeblok_sdk-1.1.1/zeblok_sdk.egg-info/top_level.txt
```

### Comparing `zeblok_sdk-1.1.0/PKG-INFO` & `zeblok_sdk-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeblok-sdk
-Version: 1.1.0
+Version: 1.1.1
 Summary: Zeblok Python SDK
 Home-page: 
 Author: Karan Pathak
 Author-email: karan@dataturtles.com
 Keywords: python,zeblok
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `zeblok_sdk-1.1.0/README.md` & `zeblok_sdk-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/setup.py` & `zeblok_sdk-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/tests/test_auth.py` & `zeblok_sdk-1.1.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/tests/test_namespace.py` & `zeblok_sdk-1.1.1/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/tests/test_orchestration.py` & `zeblok_sdk-1.1.1/tests/test_orchestration.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/tests/test_plan.py` & `zeblok_sdk-1.1.1/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/tests/test_utils.py` & `zeblok_sdk-1.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/api.py` & `zeblok_sdk-1.1.1/zeblok/api.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/auth.py` & `zeblok_sdk-1.1.1/zeblok/auth.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/base/base_airuns.py` & `zeblok_sdk-1.1.1/zeblok/base/base_airuns.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/base/base_auth.py` & `zeblok_sdk-1.1.1/zeblok/base/base_auth.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/base/base_dataset.py` & `zeblok_sdk-1.1.1/zeblok/base/base_dataset.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/base/base_service.py` & `zeblok_sdk-1.1.1/zeblok/base/base_service.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/dataset.py` & `zeblok_sdk-1.1.1/zeblok/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 from .base.base_dataset import DataSetBase
-from .utils.errors import api_error
+from .utils.errors import api_error, ObjectStoreRegionIdentificationError
 import boto3
 from botocore.exceptions import ClientError
 from boto3.s3.transfer import TransferConfig
 from pathlib import Path
 from .auth import APIAuth
 import os
 from azure.storage.blob import BlobServiceClient, generate_blob_sas, BlobSasPermissions
-from typing import Union
+from typing import Union, Dict
 from tqdm import tqdm
 import requests
 from . import PRESIGNED_URL_EXPIRATION_SECS
 from datetime import datetime, timedelta
 
 
 class AwsS3(DataSetBase):
     def __init__(self, access_key: str, secret_key: str, bucket_name: str):
-        self.__s3_client = boto3.client('s3', aws_access_key_id=access_key, aws_secret_access_key=secret_key)
+        init_params = {
+            'aws_access_key_id': access_key, 'aws_secret_access_key': secret_key,
+        }
+        self.__s3_client = boto3.client('s3', **init_params)
+        super().__init__(access_key=access_key, access_secret=secret_key, bucket_name=bucket_name)
 
-        super().__init__(
-            access_key=access_key, access_secret=secret_key, bucket_name=bucket_name
-        )
+        self.__update_client_with_region(init_params=init_params)
+
+    def __update_client_with_region(self, init_params: Dict) -> None:
+        try:
+            region_name = self.__s3_client.get_bucket_location(Bucket=self.bucket_name)['LocationConstraint']
+            self.__s3_client = boto3.client('s3', **init_params, region_name=region_name)
+        except ClientError as e:
+            raise ObjectStoreRegionIdentificationError(
+                f"Could not identify the region of the bucket `{self.bucket_name}`"
+            )
 
     def _bucket_exists(self) -> bool:
         try:
             return self.__s3_client.head_bucket(Bucket=self.bucket_name)['ResponseMetadata']['HTTPStatusCode'] == 200
         except ClientError as e:
             print(e)
             return False
```

### Comparing `zeblok_sdk-1.1.0/zeblok/microservice.py` & `zeblok_sdk-1.1.1/zeblok/microservice.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/namespace.py` & `zeblok_sdk-1.1.1/zeblok/namespace.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/orchestration.py` & `zeblok_sdk-1.1.1/zeblok/orchestration.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/pipeline.py` & `zeblok_sdk-1.1.1/zeblok/pipeline.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/plan.py` & `zeblok_sdk-1.1.1/zeblok/plan.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/utils/error_message.py` & `zeblok_sdk-1.1.1/zeblok/utils/error_message.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/utils/errors.py` & `zeblok_sdk-1.1.1/zeblok/utils/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,19 @@
 
 
 class CaaSUploadError(Exception):
     def __init__(self, message):
         super().__init__(message)
 
 
+class ObjectStoreRegionIdentificationError(Exception):
+    def __init__(self, message):
+        super().__init__(message)
+
+
 def api_error(status_code: int, message: str = ""):
     if status_code == 200:
         raise NoResourcesError(message if message else "No respective resources in this environment.")
 
     if status_code == 401:
         raise AuthenticationError(
             "User not authenticated. Please check your token or api_access_key or api_access_secret"
```

### Comparing `zeblok_sdk-1.1.0/zeblok/utils/misc.py` & `zeblok_sdk-1.1.1/zeblok/utils/misc.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/utils/progressbar.py` & `zeblok_sdk-1.1.1/zeblok/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok/utils/validations.py` & `zeblok_sdk-1.1.1/zeblok/utils/validations.py`

 * *Files identical despite different names*

### Comparing `zeblok_sdk-1.1.0/zeblok_sdk.egg-info/PKG-INFO` & `zeblok_sdk-1.1.1/zeblok_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeblok-sdk
-Version: 1.1.0
+Version: 1.1.1
 Summary: Zeblok Python SDK
 Home-page: 
 Author: Karan Pathak
 Author-email: karan@dataturtles.com
 Keywords: python,zeblok
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `zeblok_sdk-1.1.0/zeblok_sdk.egg-info/SOURCES.txt` & `zeblok_sdk-1.1.1/zeblok_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/reversinglabs_sdk_py3-2.5.2.tar.gz` & `tmp/reversinglabs_sdk_py3-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reversinglabs_sdk_py3-2.5.2.tar", last modified: Tue Apr 30 15:51:38 2024, max compression
+gzip compressed data, was "reversinglabs_sdk_py3-2.5.3.tar", last modified: Wed May  8 15:39:26 2024, max compression
```

## Comparing `reversinglabs_sdk_py3-2.5.2.tar` & `reversinglabs_sdk_py3-2.5.3.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    47537 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    46179 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.634877 reversinglabs_sdk_py3-2.5.2/ReversingLabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.634877 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96422 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)    19593 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/clouddeepscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)   250836 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/tiscale.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/ReversingLabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47537 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-30 15:51:38.000000 reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:51:38.638877 reversinglabs_sdk_py3-2.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/tests/test_a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/tests/test_ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 15:51:34.000000 reversinglabs_sdk_py3-2.5.2/tests/test_tiscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:26.140555 reversinglabs_sdk_py3-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    46146 2024-05-08 15:39:26.140555 reversinglabs_sdk_py3-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    44788 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:26.136555 reversinglabs_sdk_py3-2.5.3/ReversingLabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:26.140555 reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96422 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250906 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/tiscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/ReversingLabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:26.140555 reversinglabs_sdk_py3-2.5.3/reversinglabs_sdk_py3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46146 2024-05-08 15:39:26.000000 reversinglabs_sdk_py3-2.5.3/reversinglabs_sdk_py3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-08 15:39:26.000000 reversinglabs_sdk_py3-2.5.3/reversinglabs_sdk_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:39:26.000000 reversinglabs_sdk_py3-2.5.3/reversinglabs_sdk_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:39:25.000000 reversinglabs_sdk_py3-2.5.3/reversinglabs_sdk_py3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 15:39:26.000000 reversinglabs_sdk_py3-2.5.3/reversinglabs_sdk_py3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 15:39:26.000000 reversinglabs_sdk_py3-2.5.3/reversinglabs_sdk_py3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 15:39:26.140555 reversinglabs_sdk_py3-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:26.140555 reversinglabs_sdk_py3-2.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/tests/test_a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/tests/test_ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-08 15:39:17.000000 reversinglabs_sdk_py3-2.5.3/tests/test_tiscale.py
```

### Comparing `reversinglabs_sdk_py3-2.5.2/CHANGELOG.md` & `reversinglabs_sdk_py3-2.5.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -237,8 +237,20 @@
 
 
 2.5.2 (2024-04-30)
 -------------------
 
 #### Improvements
 - **a1000** module:
-  - The function for checking file analysis status is now public. It is called `file_analysis_status`.
+  - The function for checking file analysis status is now public. It is called `file_analysis_status`.
+
+
+2.5.3 (2024-05-08)
+-------------------
+
+#### Bugfixes
+- **ticloud** module:
+  - The classification override parameter in the `override_classification` method of the `FileReputationUserOverride` now works as expected due to a payload fix.
+
+#### Removals
+- **clouddeepscan** module:
+  - Dropped support for the clouddeepscan module. As of this version, the module is removed from the SDK.
```

### Comparing `reversinglabs_sdk_py3-2.5.2/LICENSE` & `reversinglabs_sdk_py3-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.2/PKG-INFO` & `reversinglabs_sdk_py3-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.2
+Version: 2.5.3
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.2
-Requires-Dist: urllib3>=1.26.14
+Requires-Dist: urllib3>=1.26.17
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 ![ReversingLabs](https://raw.githubusercontent.com/reversinglabs/reversinglabs-sdk-py3/master/logo.png)
 
 # ReversingLabs SDK
 
@@ -940,52 +940,14 @@
   - Deletes multiple task records from the system based on the time when they were submitted.
 - `get_yara_id`
   - Retrieves the identifier of the current set of YARA rules on the TitaniumScale Worker instance.
 
 
 ***
 
-## Module: clouddeepscan
-Handles communication with Cloud Deep Scan API endpoints.
-
-#### Class:
-```python
-class CloudDeepScan(object)
-```
-
-#### Parameters:
-`token_endpoint` - token endpoint that is used to fetch authorization token  
-`rest_hostname` - REST API hostname that is used as base URL to generate endpoints  
-`client_id` - ID of OAuth2.0 client used for authorization  
-`client_secret` - secret of OAuth2.0 client used for authorization  
-
-
-#### Methods:
-- `upload_sample`
-    - Accepts a file path string of a file that should be scanned and optional configuration of how many part uploads to do concurrently, returns submission ID
-- `fetch_submission`
-    - Accepts submission ID and returns an instance of CloudDeepScanSubmissionStatus
-- `fetch_submission_history`
-    - Accepts either sample name or sample hash and returns list of CloudDeepScanSubmissionStatus objects
-- `download_report`
-    - Accepts sha1 hash of the sample and path of the output file where JSON report will be stored and stores report to that location
-
-#### Class:
-```python
-class CloudDeepScanSubmissionStatus(object)
-```
-
-#### Parameters:
-`id_` - submission ID of the submission  
-`created_at` - datetime instance of time when submission is created  
-`status` - submission status, can be one of: scanned, scanning, error
-`report` - URL pointing to report location, None if status is not "scanned"
-
-***
-
 ## Examples
 #### A1000
 ```python
 from ReversingLabs.SDK.a1000 import A1000
 
 # Using username and password for authorization
 a1000 = A1000(
```

### Comparing `reversinglabs_sdk_py3-2.5.2/README.md` & `reversinglabs_sdk_py3-2.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -908,52 +908,14 @@
   - Deletes multiple task records from the system based on the time when they were submitted.
 - `get_yara_id`
   - Retrieves the identifier of the current set of YARA rules on the TitaniumScale Worker instance.
 
 
 ***
 
-## Module: clouddeepscan
-Handles communication with Cloud Deep Scan API endpoints.
-
-#### Class:
-```python
-class CloudDeepScan(object)
-```
-
-#### Parameters:
-`token_endpoint` - token endpoint that is used to fetch authorization token  
-`rest_hostname` - REST API hostname that is used as base URL to generate endpoints  
-`client_id` - ID of OAuth2.0 client used for authorization  
-`client_secret` - secret of OAuth2.0 client used for authorization  
-
-
-#### Methods:
-- `upload_sample`
-    - Accepts a file path string of a file that should be scanned and optional configuration of how many part uploads to do concurrently, returns submission ID
-- `fetch_submission`
-    - Accepts submission ID and returns an instance of CloudDeepScanSubmissionStatus
-- `fetch_submission_history`
-    - Accepts either sample name or sample hash and returns list of CloudDeepScanSubmissionStatus objects
-- `download_report`
-    - Accepts sha1 hash of the sample and path of the output file where JSON report will be stored and stores report to that location
-
-#### Class:
-```python
-class CloudDeepScanSubmissionStatus(object)
-```
-
-#### Parameters:
-`id_` - submission ID of the submission  
-`created_at` - datetime instance of time when submission is created  
-`status` - submission status, can be one of: scanned, scanning, error
-`report` - URL pointing to report location, None if status is not "scanned"
-
-***
-
 ## Examples
 #### A1000
 ```python
 from ReversingLabs.SDK.a1000 import A1000
 
 # Using username and password for authorization
 a1000 = A1000(
```

### Comparing `reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/a1000.py` & `reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/a1000.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/helper.py` & `reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,20 +127,14 @@
 class NotAcceptableError(Exception):
     def __init__(self, response_object, message="This content is not acceptable"):
         super(NotAcceptableError, self).__init__(message)
 
         self.response_object = response_object
 
 
-class CloudDeepScanException(Exception):
-    """Base exception for the clouddeepscan module
-    """
-    pass
-
-
 RESPONSE_CODE_ERROR_MAP = {
     HTTPStatus.UNAUTHORIZED: UnauthorizedError,
     HTTPStatus.FORBIDDEN: ForbiddenError,
     HTTPStatus.NOT_FOUND: NotFoundError,
     HTTPStatus.METHOD_NOT_ALLOWED: NotAllowedError,
     HTTPStatus.NOT_ACCEPTABLE: NotAcceptableError,
     HTTPStatus.TOO_MANY_REQUESTS: TooManyRequestsError,
```

### Comparing `reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/ticloud.py` & `reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/ticloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,17 +273,18 @@
 
         self._url = "{host}{{endpoint}}".format(host=self._host)
 
     def override_classification(self, override_samples=None, remove_override=None):
         """Accepts two parameters:
             1. A list of samples whose classification needs to be overriden
             2. A list of samples whose classification override needs to me removed
-        Both parameters are lists of Python dictionaries.
+        Both parameters are lists of Python dictionaries and
+        both need to contain all three of the following hashes of a sample: sha1, sha256, md5
         For specific examples and a more detailed explanation, read the API documentation.
-            :param override_samples: samples whose classification needs to be overriden
+            :param override_samples: samples whose classification needs to be overriden;
             :type override_samples: list[dict]
             :param remove_override: samples whose classification override needs to me removed
             :type remove_override: list[dict]
             :return: response
             :rtype: requests.Response
         """
         if override_samples is None:
@@ -292,16 +293,15 @@
         if remove_override is None:
             remove_override = []
 
         endpoint = self.__OVERRIDE_REQUEST_ENDPOINT.format(post_format="json")
 
         url = self._url.format(endpoint=endpoint)
 
-        post_json = {"rl": {"query": {"override_samples": override_samples},
-                            "remove_override": remove_override}}
+        post_json = {"rl": {"query": {"override_samples": override_samples, "remove_override": remove_override}}}
 
         response = self._post_request(
             url=url,
             post_json=post_json
         )
 
         self._raise_on_error(response)
```

### Comparing `reversinglabs_sdk_py3-2.5.2/ReversingLabs/SDK/tiscale.py` & `reversinglabs_sdk_py3-2.5.3/ReversingLabs/SDK/tiscale.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.2/logo.png` & `reversinglabs_sdk_py3-2.5.3/logo.png`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/PKG-INFO` & `reversinglabs_sdk_py3-2.5.3/reversinglabs_sdk_py3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.2
+Version: 2.5.3
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.28.2
-Requires-Dist: urllib3>=1.26.14
+Requires-Dist: urllib3>=1.26.17
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 ![ReversingLabs](https://raw.githubusercontent.com/reversinglabs/reversinglabs-sdk-py3/master/logo.png)
 
 # ReversingLabs SDK
 
@@ -940,52 +940,14 @@
   - Deletes multiple task records from the system based on the time when they were submitted.
 - `get_yara_id`
   - Retrieves the identifier of the current set of YARA rules on the TitaniumScale Worker instance.
 
 
 ***
 
-## Module: clouddeepscan
-Handles communication with Cloud Deep Scan API endpoints.
-
-#### Class:
-```python
-class CloudDeepScan(object)
-```
-
-#### Parameters:
-`token_endpoint` - token endpoint that is used to fetch authorization token  
-`rest_hostname` - REST API hostname that is used as base URL to generate endpoints  
-`client_id` - ID of OAuth2.0 client used for authorization  
-`client_secret` - secret of OAuth2.0 client used for authorization  
-
-
-#### Methods:
-- `upload_sample`
-    - Accepts a file path string of a file that should be scanned and optional configuration of how many part uploads to do concurrently, returns submission ID
-- `fetch_submission`
-    - Accepts submission ID and returns an instance of CloudDeepScanSubmissionStatus
-- `fetch_submission_history`
-    - Accepts either sample name or sample hash and returns list of CloudDeepScanSubmissionStatus objects
-- `download_report`
-    - Accepts sha1 hash of the sample and path of the output file where JSON report will be stored and stores report to that location
-
-#### Class:
-```python
-class CloudDeepScanSubmissionStatus(object)
-```
-
-#### Parameters:
-`id_` - submission ID of the submission  
-`created_at` - datetime instance of time when submission is created  
-`status` - submission status, can be one of: scanned, scanning, error
-`report` - URL pointing to report location, None if status is not "scanned"
-
-***
-
 ## Examples
 #### A1000
 ```python
 from ReversingLabs.SDK.a1000 import A1000
 
 # Using username and password for authorization
 a1000 = A1000(
```

### Comparing `reversinglabs_sdk_py3-2.5.2/reversinglabs_sdk_py3.egg-info/SOURCES.txt` & `reversinglabs_sdk_py3-2.5.3/reversinglabs_sdk_py3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 README.md
 logo.png
 setup.cfg
 setup.py
 ReversingLabs/__init__.py
 ReversingLabs/SDK/__init__.py
 ReversingLabs/SDK/a1000.py
-ReversingLabs/SDK/clouddeepscan.py
 ReversingLabs/SDK/helper.py
 ReversingLabs/SDK/ticloud.py
 ReversingLabs/SDK/tiscale.py
 reversinglabs_sdk_py3.egg-info/PKG-INFO
 reversinglabs_sdk_py3.egg-info/SOURCES.txt
 reversinglabs_sdk_py3.egg-info/dependency_links.txt
 reversinglabs_sdk_py3.egg-info/not-zip-safe
```

### Comparing `reversinglabs_sdk_py3-2.5.2/setup.py` & `reversinglabs_sdk_py3-2.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from ReversingLabs.SDK import __version__
 
 
-requires = ["requests>=2.28.2", "urllib3>=1.26.14"]
+requires = ["requests>=2.28.2", "urllib3>=1.26.17"]
 
 packages = ["ReversingLabs",
             "ReversingLabs.SDK"]
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
```

### Comparing `reversinglabs_sdk_py3-2.5.2/tests/test_a1000.py` & `reversinglabs_sdk_py3-2.5.3/tests/test_a1000.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.2/tests/test_helper.py` & `reversinglabs_sdk_py3-2.5.3/tests/test_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 STATUS_ERRORS = (
 	NotFoundError, NoFileTypeError, UnauthorizedError, WrongInputError, ForbiddenError, BadRequestError,
 	RequestTimeoutError, ConflictError, RequestTooLargeError, InternalServerError, BadGatewayError,
 	ServiceUnavailableError, NotAllowedError, TooManyRequestsError, NotAcceptableError
 )
 OTHER_ERRORS = (
-	WrongInputError, CloudDeepScanException
+	WrongInputError,
 )
 ALL_ERRORS = STATUS_ERRORS + OTHER_ERRORS
 
 
 def test_vars():
 	assert HASH_LENGTH_MAP.get(32) == MD5
 	assert HASH_LENGTH_MAP.get(40) == SHA1
```

### Comparing `reversinglabs_sdk_py3-2.5.2/tests/test_ticloud.py` & `reversinglabs_sdk_py3-2.5.3/tests/test_ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs_sdk_py3-2.5.2/tests/test_tiscale.py` & `reversinglabs_sdk_py3-2.5.3/tests/test_tiscale.py`

 * *Files identical despite different names*


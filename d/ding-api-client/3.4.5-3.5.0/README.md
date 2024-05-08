# Comparing `tmp/ding_api_client-3.4.5.tar.gz` & `tmp/ding_api_client-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ding_api_client-3.4.5.tar", last modified: Fri May  3 00:12:26 2024, max compression
+gzip compressed data, was "ding_api_client-3.5.0.tar", last modified: Tue May  7 14:57:32 2024, max compression
```

## Comparing `ding_api_client-3.4.5.tar` & `ding_api_client-3.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/ding/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/ding/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/ding/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.674560 ding_api_client-3.4.5/src/ding/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/createauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/createauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/createcheckrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/createcheckresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/feedbackrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/feedbackresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/lookupresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/retryauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/retryauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/src/ding/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/errors/errorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/src/ding/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/create_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/models/operations/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/src/ding/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-05-03 00:12:14.000000 ding_api_client-3.4.5/src/ding/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 00:12:26.678560 ding_api_client-3.4.5/src/ding_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 00:12:26.000000 ding_api_client-3.4.5/src/ding_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.027762 ding_api_client-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9580 2024-05-07 14:57:32.027762 ding_api_client-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:57:32.027762 ding_api_client-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.019762 ding_api_client-3.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.023762 ding_api_client-3.5.0/src/ding/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.023762 ding_api_client-3.5.0/src/ding/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.023762 ding_api_client-3.5.0/src/ding/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.023762 ding_api_client-3.5.0/src/ding/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/createauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/createauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/createcheckrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/createcheckresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/feedbackrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/feedbackresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/lookupresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/retryauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/retryauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.023762 ding_api_client-3.5.0/src/ding/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/errors/errorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.027762 ding_api_client-3.5.0/src/ding/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/operations/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/operations/create_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/operations/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/operations/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/models/operations/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.027762 ding_api_client-3.5.0/src/ding/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-07 14:57:20.000000 ding_api_client-3.5.0/src/ding/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:57:32.027762 ding_api_client-3.5.0/src/ding_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9580 2024-05-07 14:57:31.000000 ding_api_client-3.5.0/src/ding_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-07 14:57:31.000000 ding_api_client-3.5.0/src/ding_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:57:31.000000 ding_api_client-3.5.0/src/ding_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-07 14:57:31.000000 ding_api_client-3.5.0/src/ding_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 14:57:31.000000 ding_api_client-3.5.0/src/ding_api_client.egg-info/top_level.txt
```

### Comparing `ding_api_client-3.4.5/PKG-INFO` & `ding_api_client-3.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ding_api_client
-Version: 3.4.5
+Version: 3.5.0
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
@@ -31,20 +31,18 @@
         import ding
         from ding.models import components
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
+        res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
             customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
             phone_number='+1234567890',
-        )
-        
-        res = s.otp.create_authentication(req)
+        ))
         
         if res.create_authentication_response is not None:
             # handle response
             pass
         
         ```
         
@@ -57,21 +55,19 @@
         import ding
         from ding.models import components
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateCheckRequest(
+        res = s.otp.check(request=components.CreateCheckRequest(
             customer_uuid='e0e7b0e9-739d-424b-922f-1c2cb48ab077',
             authentication_uuid='8f1196d5-806e-4b71-9b24-5f96ec052808',
             check_code='123456',
-        )
-        
-        res = s.otp.check(req)
+        ))
         
         if res.create_check_response is not None:
             # handle response
             pass
         
         ```
         
@@ -84,20 +80,18 @@
         import ding
         from ding.models import components
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.RetryAuthenticationRequest(
+        res = s.otp.retry(request=components.RetryAuthenticationRequest(
             customer_uuid='a74ee547-564d-487a-91df-37fb25413a91',
             authentication_uuid='3c8b3a46-881e-4cdd-93a6-f7f238bf020a',
-        )
-        
-        res = s.otp.retry(req)
+        ))
         
         if res.retry_authentication_response is not None:
             # handle response
             pass
         
         ```
         <!-- End SDK Example Usage [usage] -->
@@ -133,22 +127,20 @@
         import ding
         from ding.models import components, errors
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
-            customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
-            phone_number='+1234567890',
-        )
-        
         res = None
         try:
-            res = s.otp.create_authentication(req)
+            res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
+            customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
+            phone_number='+1234567890',
+        ))
         except errors.ErrorResponse as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -177,20 +169,18 @@
         from ding.models import components
         
         s = ding.Ding(
             server_idx=0,
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
+        res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
             customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
             phone_number='+1234567890',
-        )
-        
-        res = s.otp.create_authentication(req)
+        ))
         
         if res.create_authentication_response is not None:
             # handle response
             pass
         
         ```
         
@@ -203,20 +193,18 @@
         from ding.models import components
         
         s = ding.Ding(
             server_url="https://api.ding.live/v1",
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
+        res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
             customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
             phone_number='+1234567890',
-        )
-        
-        res = s.otp.create_authentication(req)
+        ))
         
         if res.create_authentication_response is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -253,20 +241,18 @@
         import ding
         from ding.models import components
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
+        res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
             customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
             phone_number='+1234567890',
-        )
-        
-        res = s.otp.create_authentication(req)
+        ))
         
         if res.create_authentication_response is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
```

### Comparing `ding_api_client-3.4.5/README.md` & `ding_api_client-3.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,20 +24,18 @@
 import ding
 from ding.models import components
 
 s = ding.Ding(
     api_key="YOUR_API_KEY",
 )
 
-req = components.CreateAuthenticationRequest(
+res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
     customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
     phone_number='+1234567890',
-)
-
-res = s.otp.create_authentication(req)
+))
 
 if res.create_authentication_response is not None:
     # handle response
     pass
 
 ```
 
@@ -50,21 +48,19 @@
 import ding
 from ding.models import components
 
 s = ding.Ding(
     api_key="YOUR_API_KEY",
 )
 
-req = components.CreateCheckRequest(
+res = s.otp.check(request=components.CreateCheckRequest(
     customer_uuid='e0e7b0e9-739d-424b-922f-1c2cb48ab077',
     authentication_uuid='8f1196d5-806e-4b71-9b24-5f96ec052808',
     check_code='123456',
-)
-
-res = s.otp.check(req)
+))
 
 if res.create_check_response is not None:
     # handle response
     pass
 
 ```
 
@@ -77,20 +73,18 @@
 import ding
 from ding.models import components
 
 s = ding.Ding(
     api_key="YOUR_API_KEY",
 )
 
-req = components.RetryAuthenticationRequest(
+res = s.otp.retry(request=components.RetryAuthenticationRequest(
     customer_uuid='a74ee547-564d-487a-91df-37fb25413a91',
     authentication_uuid='3c8b3a46-881e-4cdd-93a6-f7f238bf020a',
-)
-
-res = s.otp.retry(req)
+))
 
 if res.retry_authentication_response is not None:
     # handle response
     pass
 
 ```
 <!-- End SDK Example Usage [usage] -->
@@ -126,22 +120,20 @@
 import ding
 from ding.models import components, errors
 
 s = ding.Ding(
     api_key="YOUR_API_KEY",
 )
 
-req = components.CreateAuthenticationRequest(
-    customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
-    phone_number='+1234567890',
-)
-
 res = None
 try:
-    res = s.otp.create_authentication(req)
+    res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
+    customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
+    phone_number='+1234567890',
+))
 except errors.ErrorResponse as e:
     # handle exception
     raise(e)
 except errors.SDKError as e:
     # handle exception
     raise(e)
 
@@ -170,20 +162,18 @@
 from ding.models import components
 
 s = ding.Ding(
     server_idx=0,
     api_key="YOUR_API_KEY",
 )
 
-req = components.CreateAuthenticationRequest(
+res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
     customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
     phone_number='+1234567890',
-)
-
-res = s.otp.create_authentication(req)
+))
 
 if res.create_authentication_response is not None:
     # handle response
     pass
 
 ```
 
@@ -196,20 +186,18 @@
 from ding.models import components
 
 s = ding.Ding(
     server_url="https://api.ding.live/v1",
     api_key="YOUR_API_KEY",
 )
 
-req = components.CreateAuthenticationRequest(
+res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
     customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
     phone_number='+1234567890',
-)
-
-res = s.otp.create_authentication(req)
+))
 
 if res.create_authentication_response is not None:
     # handle response
     pass
 
 ```
 <!-- End Server Selection [server] -->
@@ -246,20 +234,18 @@
 import ding
 from ding.models import components
 
 s = ding.Ding(
     api_key="YOUR_API_KEY",
 )
 
-req = components.CreateAuthenticationRequest(
+res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
     customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
     phone_number='+1234567890',
-)
-
-res = s.otp.create_authentication(req)
+))
 
 if res.create_authentication_response is not None:
     # handle response
     pass
 
 ```
 <!-- End Authentication [security] -->
```

### Comparing `ding_api_client-3.4.5/setup.py` & `ding_api_client-3.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='ding_api_client',
-    version='3.4.5',
+    version='3.5.0',
     author='Ding',
     description='Python Client SDK',
     url='https://github.com/ding-live/ding-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `ding_api_client-3.4.5/src/ding/_hooks/sdkhooks.py` & `ding_api_client-3.5.0/src/ding/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/_hooks/types.py` & `ding_api_client-3.5.0/src/ding/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/lookup.py` & `ding_api_client-3.5.0/src/ding/lookup.py`

 * *Files 12% similar despite different names*

```diff
@@ -57,21 +57,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.LookupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.LookupResponse])
                 res.lookup_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `ding_api_client-3.4.5/src/ding/models/components/__init__.py` & `ding_api_client-3.5.0/src/ding/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/components/createauthenticationrequest.py` & `ding_api_client-3.5.0/src/ding/models/components/createauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/components/createauthenticationresponse.py` & `ding_api_client-3.5.0/src/ding/models/components/createauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/components/createcheckrequest.py` & `ding_api_client-3.5.0/src/ding/models/components/createcheckrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/components/createcheckresponse.py` & `ding_api_client-3.5.0/src/ding/models/components/createcheckresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/components/feedbackrequest.py` & `ding_api_client-3.5.0/src/ding/models/components/feedbackrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/components/feedbackresponse.py` & `ding_api_client-3.5.0/src/ding/models/components/feedbackresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/components/lookupresponse.py` & `ding_api_client-3.5.0/src/ding/models/components/lookupresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/components/retryauthenticationrequest.py` & `ding_api_client-3.5.0/src/ding/models/components/retryauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/components/retryauthenticationresponse.py` & `ding_api_client-3.5.0/src/ding/models/components/retryauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/errors/errorresponse.py` & `ding_api_client-3.5.0/src/ding/models/errors/errorresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/errors/sdkerror.py` & `ding_api_client-3.5.0/src/ding/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/operations/check.py` & `ding_api_client-3.5.0/src/ding/models/operations/check.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/operations/create_authentication.py` & `ding_api_client-3.5.0/src/ding/models/operations/create_authentication.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/operations/feedback.py` & `ding_api_client-3.5.0/src/ding/models/operations/feedback.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/operations/lookup.py` & `ding_api_client-3.5.0/src/ding/models/operations/lookup.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/models/operations/retry.py` & `ding_api_client-3.5.0/src/ding/models/operations/retry.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/otp.py` & `ding_api_client-3.5.0/src/ding/otp.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_authentication(self, request: Optional[components.CreateAuthenticationRequest]) -> operations.CreateAuthenticationResponse:
+    def create_authentication(self, request: Optional[components.CreateAuthenticationRequest] = None) -> operations.CreateAuthenticationResponse:
         r"""Send a code"""
         hook_ctx = HookContext(operation_id='create-authentication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/authentication'
         
         if callable(self.sdk_configuration.security):
@@ -54,21 +54,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAuthenticationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CreateAuthenticationResponse])
                 res.create_authentication_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -76,15 +78,15 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def check(self, request: Optional[components.CreateCheckRequest]) -> operations.CheckResponse:
+    def check(self, request: Optional[components.CreateCheckRequest] = None) -> operations.CheckResponse:
         r"""Check a code"""
         hook_ctx = HookContext(operation_id='check', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/check'
         
         if callable(self.sdk_configuration.security):
@@ -118,21 +120,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CheckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CreateCheckResponse])
                 res.create_check_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -140,15 +144,15 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def feedback(self, request: Optional[components.FeedbackRequest]) -> operations.FeedbackResponse:
+    def feedback(self, request: Optional[components.FeedbackRequest] = None) -> operations.FeedbackResponse:
         r"""Send feedback"""
         hook_ctx = HookContext(operation_id='feedback', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/authentication/feedback'
         
         if callable(self.sdk_configuration.security):
@@ -182,35 +186,37 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.FeedbackResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.FeedbackResponse])
                 res.feedback_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.ErrorResponse])
                 res.error_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def retry(self, request: Optional[components.RetryAuthenticationRequest]) -> operations.RetryResponse:
+    def retry(self, request: Optional[components.RetryAuthenticationRequest] = None) -> operations.RetryResponse:
         r"""Perform a retry"""
         hook_ctx = HookContext(operation_id='retry', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/retry'
         
         if callable(self.sdk_configuration.security):
@@ -244,21 +250,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.RetryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.RetryAuthenticationResponse])
                 res.retry_authentication_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `ding_api_client-3.4.5/src/ding/sdk.py` & `ding_api_client-3.5.0/src/ding/sdk.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/sdkconfiguration.py` & `ding_api_client-3.5.0/src/ding/sdkconfiguration.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '3.4.5'
-    gen_version: str = '2.319.10'
-    user_agent: str = 'speakeasy-sdk/python 3.4.5 2.319.10 1.0.0 ding_api_client'
+    sdk_version: str = '3.5.0'
+    gen_version: str = '2.326.0'
+    user_agent: str = 'speakeasy-sdk/python 3.5.0 2.326.0 1.0.0 ding_api_client'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `ding_api_client-3.4.5/src/ding/utils/retries.py` & `ding_api_client-3.5.0/src/ding/utils/retries.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.5/src/ding/utils/utils.py` & `ding_api_client-3.5.0/src/ding/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -904,14 +904,41 @@
 
 
 def bigintdecoder(val):
     if isinstance(val, float):
         raise ValueError(f"{val} is a float")
     return int(val)
 
+def integerstrencoder(optional: bool):
+    def integerstrencode(val: int):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return integerstrencode
+
+
+def integerstrdecoder(val):
+    if isinstance(val, float):
+        raise ValueError(f"{val} is a float")
+    return int(val)
+
+
+def numberstrencoder(optional: bool):
+    def numberstrencode(val: float):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return numberstrencode
+
+
+def numberstrdecoder(val):
+    return float(val)
+
 
 def decimalencoder(optional: bool, as_str: bool):
     def decimalencode(val: Decimal):
         if optional and val is None:
             return None
 
         if as_str:
```

### Comparing `ding_api_client-3.4.5/src/ding_api_client.egg-info/PKG-INFO` & `ding_api_client-3.5.0/src/ding_api_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ding-api-client
-Version: 3.4.5
+Version: 3.5.0
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
@@ -31,20 +31,18 @@
         import ding
         from ding.models import components
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
+        res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
             customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
             phone_number='+1234567890',
-        )
-        
-        res = s.otp.create_authentication(req)
+        ))
         
         if res.create_authentication_response is not None:
             # handle response
             pass
         
         ```
         
@@ -57,21 +55,19 @@
         import ding
         from ding.models import components
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateCheckRequest(
+        res = s.otp.check(request=components.CreateCheckRequest(
             customer_uuid='e0e7b0e9-739d-424b-922f-1c2cb48ab077',
             authentication_uuid='8f1196d5-806e-4b71-9b24-5f96ec052808',
             check_code='123456',
-        )
-        
-        res = s.otp.check(req)
+        ))
         
         if res.create_check_response is not None:
             # handle response
             pass
         
         ```
         
@@ -84,20 +80,18 @@
         import ding
         from ding.models import components
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.RetryAuthenticationRequest(
+        res = s.otp.retry(request=components.RetryAuthenticationRequest(
             customer_uuid='a74ee547-564d-487a-91df-37fb25413a91',
             authentication_uuid='3c8b3a46-881e-4cdd-93a6-f7f238bf020a',
-        )
-        
-        res = s.otp.retry(req)
+        ))
         
         if res.retry_authentication_response is not None:
             # handle response
             pass
         
         ```
         <!-- End SDK Example Usage [usage] -->
@@ -133,22 +127,20 @@
         import ding
         from ding.models import components, errors
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
-            customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
-            phone_number='+1234567890',
-        )
-        
         res = None
         try:
-            res = s.otp.create_authentication(req)
+            res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
+            customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
+            phone_number='+1234567890',
+        ))
         except errors.ErrorResponse as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -177,20 +169,18 @@
         from ding.models import components
         
         s = ding.Ding(
             server_idx=0,
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
+        res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
             customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
             phone_number='+1234567890',
-        )
-        
-        res = s.otp.create_authentication(req)
+        ))
         
         if res.create_authentication_response is not None:
             # handle response
             pass
         
         ```
         
@@ -203,20 +193,18 @@
         from ding.models import components
         
         s = ding.Ding(
             server_url="https://api.ding.live/v1",
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
+        res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
             customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
             phone_number='+1234567890',
-        )
-        
-        res = s.otp.create_authentication(req)
+        ))
         
         if res.create_authentication_response is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -253,20 +241,18 @@
         import ding
         from ding.models import components
         
         s = ding.Ding(
             api_key="YOUR_API_KEY",
         )
         
-        req = components.CreateAuthenticationRequest(
+        res = s.otp.create_authentication(request=components.CreateAuthenticationRequest(
             customer_uuid='c9f826e0-deca-41ec-871f-ecd6e8efeb46',
             phone_number='+1234567890',
-        )
-        
-        res = s.otp.create_authentication(req)
+        ))
         
         if res.create_authentication_response is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
```

### Comparing `ding_api_client-3.4.5/src/ding_api_client.egg-info/SOURCES.txt` & `ding_api_client-3.5.0/src/ding_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


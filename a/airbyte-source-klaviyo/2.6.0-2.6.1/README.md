# Comparing `tmp/airbyte_source_klaviyo-2.6.0.tar.gz` & `tmp/airbyte_source_klaviyo-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_klaviyo-2.6.0.tar", max compression
+gzip compressed data, was "airbyte_source_klaviyo-2.6.1.tar", max compression
```

## Comparing `airbyte_source_klaviyo-2.6.0.tar` & `airbyte_source_klaviyo-2.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4519 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/README.md
--rw-r--r--   0        0        0      746 2024-04-18 16:17:22.539022 airbyte_source_klaviyo-2.6.0/pyproject.toml
--rw-r--r--   0        0        0      125 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/__init__.py
--rw-r--r--   0        0        0      975 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/availability_strategy.py
--rw-r--r--   0        0        0      865 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/components/datetime_based_cursor.py
--rw-r--r--   0        0        0      196 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/exceptions.py
--rw-r--r--   0        0        0     6817 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/manifest.yaml
--rw-r--r--   0        0        0      233 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/run.py
--rw-r--r--   0        0        0      167 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/campaigns.json
--rw-r--r--   0        0        0     1921 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/campaigns_detailed.json
--rw-r--r--   0        0        0      935 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/email_templates.json
--rw-r--r--   0        0        0     2136 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/events.json
--rw-r--r--   0        0        0     2262 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/flows.json
--rw-r--r--   0        0        0     3931 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/global_exclusions.json
--rw-r--r--   0        0        0      163 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/lists.json
--rw-r--r--   0        0        0      561 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/lists_detailed.json
--rw-r--r--   0        0        0      787 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/metrics.json
--rw-r--r--   0        0        0     3931 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/profiles.json
--rw-r--r--   0        0        0     4091 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/campaign_properties.json
--rw-r--r--   0        0        0     1591 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/list_properties.json
--rw-r--r--   0        0        0     2892 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/subscriptions.json
--rw-r--r--   0        0        0     1183 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/source.py
--rw-r--r--   0        0        0     1114 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/spec.json
--rw-r--r--   0        0        0    11531 2024-04-18 12:58:18.000000 airbyte_source_klaviyo-2.6.0/source_klaviyo/streams.py
--rw-r--r--   0        0        0     5224 1970-01-01 00:00:00.000000 airbyte_source_klaviyo-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/README.md
+-rw-r--r--   0        0        0      746 2024-05-07 11:47:26.653957 airbyte_source_klaviyo-2.6.1/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/availability_strategy.py
+-rw-r--r--   0        0        0      865 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/components/datetime_based_cursor.py
+-rw-r--r--   0        0        0      196 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/exceptions.py
+-rw-r--r--   0        0        0     7075 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/run.py
+-rw-r--r--   0        0        0      167 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/campaigns.json
+-rw-r--r--   0        0        0     1921 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/campaigns_detailed.json
+-rw-r--r--   0        0        0      935 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/email_templates.json
+-rw-r--r--   0        0        0     2136 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/events.json
+-rw-r--r--   0        0        0     2262 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/flows.json
+-rw-r--r--   0        0        0     3931 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/global_exclusions.json
+-rw-r--r--   0        0        0      163 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/lists.json
+-rw-r--r--   0        0        0      561 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/lists_detailed.json
+-rw-r--r--   0        0        0      787 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/metrics.json
+-rw-r--r--   0        0        0     3931 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/profiles.json
+-rw-r--r--   0        0        0     4091 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/shared/campaign_properties.json
+-rw-r--r--   0        0        0     1591 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/shared/list_properties.json
+-rw-r--r--   0        0        0     2892 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/shared/subscriptions.json
+-rw-r--r--   0        0        0     1183 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/source.py
+-rw-r--r--   0        0        0     1114 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/spec.json
+-rw-r--r--   0        0        0    11531 2024-05-07 11:12:22.000000 airbyte_source_klaviyo-2.6.1/source_klaviyo/streams.py
+-rw-r--r--   0        0        0     5224 1970-01-01 00:00:00.000000 airbyte_source_klaviyo-2.6.1/PKG-INFO
```

### Comparing `airbyte_source_klaviyo-2.6.0/README.md` & `airbyte_source_klaviyo-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/pyproject.toml` & `airbyte_source_klaviyo-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.6.0"
+version = "2.6.1"
 name = "airbyte-source-klaviyo"
 description = "Source implementation for Klaviyo."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/availability_strategy.py` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/components/datetime_based_cursor.py` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/components/datetime_based_cursor.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/manifest.yaml` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/manifest.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,31 @@
   # Requester
   requester:
     type: HttpRequester
     url_base: "https://a.klaviyo.com/api/"
     authenticator: "#/definitions/authenticator"
     http_method: GET
     error_handler:
-      type: DefaultErrorHandler
-      backoff_strategies:
-        - type: WaitTimeFromHeader
-          header: "Retry-After"
-      response_filters:
-        - type: HttpResponseFilter
-          action: FAIL
-          http_codes: [401, 403]
-          error_message: Please provide a valid API key and make sure it has permissions to read specified streams.
-        - type: HttpResponseFilter
-          action: RETRY
-          http_codes: [429]
+      type: CompositeErrorHandler
+      error_handlers:
+        - type: DefaultErrorHandler
+          backoff_strategies:
+            - type: WaitTimeFromHeader
+              header: "Retry-After"
+          response_filters:
+            - type: HttpResponseFilter
+              action: RETRY
+              http_codes: [429]
+        - type: DefaultErrorHandler # adding this DefaultErrorHandler for 5XX error codes
+        - type: DefaultErrorHandler
+          response_filters:
+            - type: HttpResponseFilter
+              action: FAIL
+              http_codes: [401, 403]
+              error_message: Please provide a valid API key and make sure it has permissions to read specified streams.
     request_headers:
       Accept: "application/json"
       Revision: "2023-10-15"
 
   # Selector
   selector:
     type: RecordSelector
```

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/campaigns_detailed.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/campaigns_detailed.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/email_templates.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/email_templates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/events.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/flows.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/flows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/global_exclusions.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/global_exclusions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/lists_detailed.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/lists_detailed.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/metrics.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/metrics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/profiles.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/profiles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/campaign_properties.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/shared/campaign_properties.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/list_properties.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/shared/list_properties.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/schemas/shared/subscriptions.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/schemas/shared/subscriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/source.py` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/spec.json` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/source_klaviyo/streams.py` & `airbyte_source_klaviyo-2.6.1/source_klaviyo/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_klaviyo-2.6.0/PKG-INFO` & `airbyte_source_klaviyo-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-klaviyo
-Version: 2.6.0
+Version: 2.6.1
 Summary: Source implementation for Klaviyo.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/drf_standardized_response-0.2.tar.gz` & `tmp/drf_standardized_response-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_standardized_response-0.2.tar", last modified: Mon May  6 05:08:56 2024, max compression
+gzip compressed data, was "drf_standardized_response-1.tar", last modified: Tue May  7 10:35:30 2024, max compression
```

## Comparing `drf_standardized_response-0.2.tar` & `drf_standardized_response-1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 05:08:56.781197 drf_standardized_response-0.2/
--rw-rw-rw-   0        0        0     1324 2024-05-05 12:23:50.000000 drf_standardized_response-0.2/LICENSE
--rw-rw-rw-   0        0        0       60 2024-04-29 15:40:10.000000 drf_standardized_response-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6999 2024-05-06 05:08:56.781197 drf_standardized_response-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5894 2024-05-06 05:07:38.000000 drf_standardized_response-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 05:08:56.767421 drf_standardized_response-0.2/drf_standardized_response/
--rw-rw-rw-   0        0        0        0 2024-04-29 15:25:16.000000 drf_standardized_response-0.2/drf_standardized_response/__init__.py
--rw-rw-rw-   0        0        0      218 2024-05-05 12:28:04.000000 drf_standardized_response-0.2/drf_standardized_response/apps.py
--rw-rw-rw-   0        0        0     2705 2024-05-06 04:40:46.000000 drf_standardized_response-0.2/drf_standardized_response/openapi.py
--rw-rw-rw-   0        0        0      744 2024-05-05 14:24:38.000000 drf_standardized_response-0.2/drf_standardized_response/renderers.py
--rw-rw-rw-   0        0        0     2448 2024-05-06 03:03:02.000000 drf_standardized_response-0.2/drf_standardized_response/response_standarizer.py
--rw-rw-rw-   0        0        0     2627 2024-05-05 16:04:30.000000 drf_standardized_response-0.2/drf_standardized_response/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-06 05:08:56.780197 drf_standardized_response-0.2/drf_standardized_response.egg-info/
--rw-rw-rw-   0        0        0     6999 2024-05-06 05:08:56.000000 drf_standardized_response-0.2/drf_standardized_response.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2024-05-06 05:08:56.000000 drf_standardized_response-0.2/drf_standardized_response.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 05:08:56.000000 drf_standardized_response-0.2/drf_standardized_response.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-06 05:08:56.000000 drf_standardized_response-0.2/drf_standardized_response.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-06 05:08:56.000000 drf_standardized_response-0.2/drf_standardized_response.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2024-05-06 03:07:32.000000 drf_standardized_response-0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1000 2024-05-06 05:08:56.783095 drf_standardized_response-0.2/setup.cfg
--rw-rw-rw-   0        0        0      122 2024-05-06 03:07:26.000000 drf_standardized_response-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:35:30.484206 drf_standardized_response-1/
+-rw-rw-rw-   0        0        0     1324 2024-05-05 12:23:50.000000 drf_standardized_response-1/LICENSE
+-rw-rw-rw-   0        0        0       60 2024-04-29 15:40:10.000000 drf_standardized_response-1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6948 2024-05-07 10:35:30.484206 drf_standardized_response-1/PKG-INFO
+-rw-rw-rw-   0        0        0     5845 2024-05-06 05:42:42.000000 drf_standardized_response-1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 10:35:30.463919 drf_standardized_response-1/drf_standardized_response/
+-rw-rw-rw-   0        0        0        0 2024-04-29 15:25:16.000000 drf_standardized_response-1/drf_standardized_response/__init__.py
+-rw-rw-rw-   0        0        0      218 2024-05-05 12:28:04.000000 drf_standardized_response-1/drf_standardized_response/apps.py
+-rw-rw-rw-   0        0        0     2996 2024-05-07 10:30:30.000000 drf_standardized_response-1/drf_standardized_response/openapi.py
+-rw-rw-rw-   0        0        0      800 2024-05-07 10:26:55.000000 drf_standardized_response-1/drf_standardized_response/renderers.py
+-rw-rw-rw-   0        0        0     2888 2024-05-07 10:30:30.000000 drf_standardized_response-1/drf_standardized_response/response_standarizer.py
+-rw-rw-rw-   0        0        0     2627 2024-05-05 16:04:30.000000 drf_standardized_response-1/drf_standardized_response/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:35:30.483206 drf_standardized_response-1/drf_standardized_response.egg-info/
+-rw-rw-rw-   0        0        0     6948 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      124 2024-05-06 03:07:32.000000 drf_standardized_response-1/pyproject.toml
+-rw-rw-rw-   0        0        0      998 2024-05-07 10:35:30.485203 drf_standardized_response-1/setup.cfg
+-rw-rw-rw-   0        0        0      122 2024-05-06 03:07:26.000000 drf_standardized_response-1/setup.py
```

### Comparing `drf_standardized_response-0.2/LICENSE` & `drf_standardized_response-1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-0.2/PKG-INFO` & `drf_standardized_response-1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-standardized-response
-Version: 0.2
+Version: 1
 Home-page: https://github.com/HasanAshab/drf-standardized-response
 Author: Hasan Ashab
 Author-email: hasanashab.18205@example.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.0
 Provides-Extra: openapi
 Requires-Dist: drf-spectacular>=0.27.0; extra == "openapi"
 
 # DRF Standardized Response
-A set of custom validators for validating date and datetime fields for Django.
+Standarize your API responses
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [How It Works](#how-it-works)
 - [Customizing](#customizing)
   - [Custom Wrapper Key](#custom-wrapper-key)
```

### Comparing `drf_standardized_response-0.2/README.md` & `drf_standardized_response-1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DRF Standardized Response
-A set of custom validators for validating date and datetime fields for Django.
+Standarize your API responses
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [How It Works](#how-it-works)
 - [Customizing](#customizing)
   - [Custom Wrapper Key](#custom-wrapper-key)
```

### Comparing `drf_standardized_response-0.2/drf_standardized_response/openapi.py` & `drf_standardized_response-1/drf_standardized_response/openapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+from django.test.client import RequestFactory
+from rest_framework.response import Response
 from drf_standardized_errors.openapi import AutoSchema as BaseAutoSchema
 from drf_spectacular.utils import OpenApiResponse
 from .settings import package_settings
 
 
 class StandardizedSchemaMixin:
     def _get_response_for_code(
         self, serializer, status_code, media_types=None, direction="response"
     ):
+        dummy_request = RequestFactory().get(self.path)
         self._response_standardizer = (
-            package_settings.RESPONSE_STANDARDIZER_CLASS(self._view)
+            package_settings.RESPONSE_STANDARDIZER_CLASS(
+                view=self._view,
+                request=dummy_request,
+            )
         )
+
         response = super()._get_response_for_code(
             serializer, status_code, media_types, direction
         )
         if not (content := response.get("content")):
             return response
         if "application/json" not in content:
             return response
@@ -36,23 +43,24 @@
             return response
 
         formatted_schema = self._standardize_response_schema(reference)
         content["application/json"]["schema"] = formatted_schema
         return response
 
     def _standardize_response_schema(self, reference):
+        dummy_response = Response(status=200)
         standardized_schema = {
             "type": "object",
             "properties": {
                 "success": {"type": "boolean"},
                 "message": {"type": "string"},
             },
         }
 
-        if not self._response_standardizer.should_wrap():
+        if not self._response_standardizer.should_wrap(dummy_response):
             return {
                 "allOf": [
                     {"$ref": reference},
                     standardized_schema,
                 ]
             }
```

### Comparing `drf_standardized_response-0.2/drf_standardized_response/renderers.py` & `drf_standardized_response-1/drf_standardized_response/renderers.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 class StandardizedJSONRenderer(DefaultJSONRenderer):
     def render(self, data, accepted_media_type=None, renderer_context=None):
         if not renderer_context:
             return super().render(data, accepted_media_type, renderer_context)
 
         response_standardizer = package_settings.RESPONSE_STANDARDIZER_CLASS(
-            renderer_context["view"]
+            view=renderer_context["view"],
+            request=renderer_context["request"],
         )
         if response_standardizer.should_standardize():
             data = response_standardizer.standardize(
                 renderer_context["response"]
             )
 
         return super().render(data, accepted_media_type, renderer_context)
```

### Comparing `drf_standardized_response-0.2/drf_standardized_response/response_standarizer.py` & `drf_standardized_response-1/drf_standardized_response/response_standarizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,15 @@
 from http.client import responses
 from .settings import package_settings
 
 
 class ResponseStandardizer:
-    def __init__(self, view):
+    def __init__(self, view, request):
         self.view = view
-
-    def should_standardize(self):
-        return getattr(
-            self.view,
-            "should_strandardize",
-            True,
-        )
-
-    def should_wrap(self):
-        pagination = getattr(
-            self.view,
-            "pagination_class",
-            None,
-        )
-        if (
-            not package_settings.WRAP_PAGINATED_RESPONSE
-            and pagination is not None
-        ):
-            return False
-
-        return True
+        self.request = request
 
     def get_wrapper_key(self):
         return getattr(
             self.view, "wrapper_key", package_settings.DEFFAULT_WRAPPER_KEY
         )
 
     def get_wrapping_excluded_fields(self):
@@ -41,36 +21,67 @@
 
     def get_standard_message(self, response):
         return responses[response.status_code]
 
     def is_successful_response(self, response):
         return 199 < response.status_code < 400
 
+    def is_paginated_response(self, response):
+        pagination = getattr(
+            self.view,
+            "pagination_class",
+            None,
+        )
+        return pagination is not None and self.request.method == "GET"
+
+    def should_standardize(self):
+        return getattr(
+            self.view,
+            "should_strandardize",
+            True,
+        )
+
+    def should_wrap(self, response):
+        if (
+            not package_settings.WRAP_PAGINATED_RESPONSE
+            and self.is_paginated_response(response)
+        ):
+            return False
+
+        if not self.is_successful_response(response):
+            return False
+
+        return True
+
     def standardize(self, response):
         wrapper_key = self.get_wrapper_key()
         is_successful = self.is_successful_response(response)
+        standard_message = self.get_standard_message(response)
         standardized_data = {} if response.data is None else response.data
 
         if isinstance(standardized_data, str):
             standardized_data = {"message": standardized_data}
-        elif self.should_wrap():
+        elif self.should_wrap(response):
             if isinstance(standardized_data, dict):
-                unwrapped_data = {
-                    field: standardized_data.pop(field, None)
-                    for field in self.get_wrapping_excluded_fields()
-                    if field is not None
-                }
+                unwrapped_data = {}
+                for field in self.get_wrapping_excluded_fields():
+                    try:
+                        unwrapped_data[field] = standardized_data.pop(field)
+                    except KeyError:
+                        continue
+
                 standardized_data = {
                     wrapper_key: standardized_data,
                     **unwrapped_data,
                 }
             elif isinstance(standardized_data, (list, tuple)):
                 standardized_data = {
                     wrapper_key: standardized_data,
                 }
 
-        if "success" not in standardized_data:
-            standardized_data["success"] = is_successful
-        if "message" not in standardized_data:
-            standardized_data["message"] = self.get_standard_message(response)
+        if isinstance(standardized_data, dict):
+            if "success" not in standardized_data:
+                standardized_data["success"] = is_successful
+            if "message" not in standardized_data:
+                standardized_data["message"] = standard_message
 
         return standardized_data
```

### Comparing `drf_standardized_response-0.2/drf_standardized_response/settings.py` & `drf_standardized_response-1/drf_standardized_response/settings.py`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-0.2/drf_standardized_response.egg-info/PKG-INFO` & `drf_standardized_response-1/drf_standardized_response.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-standardized-response
-Version: 0.2
+Version: 1
 Home-page: https://github.com/HasanAshab/drf-standardized-response
 Author: Hasan Ashab
 Author-email: hasanashab.18205@example.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
@@ -23,15 +23,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=4.0
 Provides-Extra: openapi
 Requires-Dist: drf-spectacular>=0.27.0; extra == "openapi"
 
 # DRF Standardized Response
-A set of custom validators for validating date and datetime fields for Django.
+Standarize your API responses
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [How It Works](#how-it-works)
 - [Customizing](#customizing)
   - [Custom Wrapper Key](#custom-wrapper-key)
```

### Comparing `drf_standardized_response-0.2/drf_standardized_response.egg-info/SOURCES.txt` & `drf_standardized_response-1/drf_standardized_response.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-0.2/setup.cfg` & `drf_standardized_response-1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 2d73 7461 6e64 6172 6469   = drf-standardi
 00000020: 7a65 642d 7265 7370 6f6e 7365 0d0a 7665  zed-response..ve
-00000030: 7273 696f 6e20 3d20 302e 320d 0a6c 6f6e  rsion = 0.2..lon
-00000040: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
-00000050: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-00000060: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000070: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000080: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000090: 7572 6c20 3d20 6874 7470 733a 2f2f 6769  url = https://gi
-000000a0: 7468 7562 2e63 6f6d 2f48 6173 616e 4173  thub.com/HasanAs
-000000b0: 6861 622f 6472 662d 7374 616e 6461 7264  hab/drf-standard
-000000c0: 697a 6564 2d72 6573 706f 6e73 650d 0a61  ized-response..a
-000000d0: 7574 686f 7220 3d20 4861 7361 6e20 4173  uthor = Hasan As
-000000e0: 6861 620d 0a61 7574 686f 725f 656d 6169  hab..author_emai
-000000f0: 6c20 3d20 6861 7361 6e61 7368 6162 2e31  l = hasanashab.1
-00000100: 3832 3035 4065 7861 6d70 6c65 2e63 6f6d  8205@example.com
-00000110: 0d0a 6c69 6365 6e73 6520 3d20 4253 442d  ..license = BSD-
-00000120: 332d 436c 6175 7365 0d0a 636c 6173 7369  3-Clause..classi
-00000130: 6669 6572 7320 3d20 0d0a 0945 6e76 6972  fiers = ...Envir
-00000140: 6f6e 6d65 6e74 203a 3a20 5765 6220 456e  onment :: Web En
-00000150: 7669 726f 6e6d 656e 740d 0a09 4672 616d  vironment...Fram
-00000160: 6577 6f72 6b20 3a3a 2044 6a61 6e67 6f0d  ework :: Django.
-00000170: 0a09 4672 616d 6577 6f72 6b20 3a3a 2044  ..Framework :: D
-00000180: 6a61 6e67 6f20 3a3a 2034 2e30 0d0a 0949  jango :: 4.0...I
-00000190: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-000001a0: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
-000001b0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-000001c0: 4170 7072 6f76 6564 203a 3a20 4253 4420  Approved :: BSD 
-000001d0: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
-000001e0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-000001f0: 2049 6e64 6570 656e 6465 6e74 0d0a 0950   Independent...P
-00000200: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000210: 6167 6520 3a3a 2050 7974 686f 6e0d 0a09  age :: Python...
-00000220: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000230: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000240: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
-00000250: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000260: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-00000270: 790d 0a09 5072 6f67 7261 6d6d 696e 6720  y...Programming 
-00000280: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000290: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
-000002a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000002b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000002c0: 2e31 310d 0a09 5072 6f67 7261 6d6d 696e  .11...Programmin
-000002d0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000002e0: 7468 6f6e 203a 3a20 332e 3132 0d0a 0954  thon :: 3.12...T
-000002f0: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
-00000300: 203a 3a20 5757 572f 4854 5450 0d0a 0954   :: WWW/HTTP...T
-00000310: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
-00000320: 203a 3a20 5757 572f 4854 5450 203a 3a20   :: WWW/HTTP :: 
-00000330: 4479 6e61 6d69 6320 436f 6e74 656e 740d  Dynamic Content.
-00000340: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 696e  ...[options]..in
-00000350: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-00000360: 7461 203d 2074 7275 650d 0a70 6163 6b61  ta = true..packa
-00000370: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-00000380: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000390: 3d33 2e31 300d 0a69 6e73 7461 6c6c 5f72  =3.10..install_r
-000003a0: 6571 7569 7265 7320 3d20 0d0a 0944 6a61  equires = ...Dja
-000003b0: 6e67 6f20 3e3d 2034 2e30 0d0a 0d0a 5b65  ngo >= 4.0....[e
-000003c0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000003d0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-000003e0: 203d 2030 0d0a 0d0a                       = 0....
+00000030: 7273 696f 6e20 3d20 310d 0a6c 6f6e 675f  rsion = 1..long_
+00000040: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+00000050: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
+00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
+00000070: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
+00000080: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
+00000090: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
+000000a0: 7562 2e63 6f6d 2f48 6173 616e 4173 6861  ub.com/HasanAsha
+000000b0: 622f 6472 662d 7374 616e 6461 7264 697a  b/drf-standardiz
+000000c0: 6564 2d72 6573 706f 6e73 650d 0a61 7574  ed-response..aut
+000000d0: 686f 7220 3d20 4861 7361 6e20 4173 6861  hor = Hasan Asha
+000000e0: 620d 0a61 7574 686f 725f 656d 6169 6c20  b..author_email 
+000000f0: 3d20 6861 7361 6e61 7368 6162 2e31 3832  = hasanashab.182
+00000100: 3035 4065 7861 6d70 6c65 2e63 6f6d 0d0a  05@example.com..
+00000110: 6c69 6365 6e73 6520 3d20 4253 442d 332d  license = BSD-3-
+00000120: 436c 6175 7365 0d0a 636c 6173 7369 6669  Clause..classifi
+00000130: 6572 7320 3d20 0d0a 0945 6e76 6972 6f6e  ers = ...Environ
+00000140: 6d65 6e74 203a 3a20 5765 6220 456e 7669  ment :: Web Envi
+00000150: 726f 6e6d 656e 740d 0a09 4672 616d 6577  ronment...Framew
+00000160: 6f72 6b20 3a3a 2044 6a61 6e67 6f0d 0a09  ork :: Django...
+00000170: 4672 616d 6577 6f72 6b20 3a3a 2044 6a61  Framework :: Dja
+00000180: 6e67 6f20 3a3a 2034 2e30 0d0a 0949 6e74  ngo :: 4.0...Int
+00000190: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+000001a0: 3a20 4465 7665 6c6f 7065 7273 0d0a 094c  : Developers...L
+000001b0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000001c0: 7072 6f76 6564 203a 3a20 4253 4420 4c69  proved :: BSD Li
+000001d0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
+000001e0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+000001f0: 6e64 6570 656e 6465 6e74 0d0a 0950 726f  ndependent...Pro
+00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000210: 6520 3a3a 2050 7974 686f 6e0d 0a09 5072  e :: Python...Pr
+00000220: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000230: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000240: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
+00000250: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000260: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790d  on :: 3 :: Only.
+00000270: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000280: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000290: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
+000002a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
+000002c0: 310d 0a09 5072 6f67 7261 6d6d 696e 6720  1...Programming 
+000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002e0: 6f6e 203a 3a20 332e 3132 0d0a 0954 6f70  on :: 3.12...Top
+000002f0: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
+00000300: 3a20 5757 572f 4854 5450 0d0a 0954 6f70  : WWW/HTTP...Top
+00000310: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
+00000320: 3a20 5757 572f 4854 5450 203a 3a20 4479  : WWW/HTTP :: Dy
+00000330: 6e61 6d69 6320 436f 6e74 656e 740d 0a0d  namic Content...
+00000340: 0a5b 6f70 7469 6f6e 735d 0d0a 696e 636c  .[options]..incl
+00000350: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+00000360: 203d 2074 7275 650d 0a70 6163 6b61 6765   = true..package
+00000370: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
+00000380: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000390: 2e31 300d 0a69 6e73 7461 6c6c 5f72 6571  .10..install_req
+000003a0: 7569 7265 7320 3d20 0d0a 0944 6a61 6e67  uires = ...Djang
+000003b0: 6f20 3e3d 2034 2e30 0d0a 0d0a 5b65 6767  o >= 4.0....[egg
+000003c0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000003d0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+000003e0: 2030 0d0a 0d0a                            0....
```


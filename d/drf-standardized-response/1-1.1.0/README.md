# Comparing `tmp/drf_standardized_response-1.tar.gz` & `tmp/drf_standardized_response-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_standardized_response-1.tar", last modified: Tue May  7 10:35:30 2024, max compression
+gzip compressed data, was "drf_standardized_response-1.1.0.tar", last modified: Wed May  8 10:17:15 2024, max compression
```

## Comparing `drf_standardized_response-1.tar` & `drf_standardized_response-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 10:35:30.484206 drf_standardized_response-1/
--rw-rw-rw-   0        0        0     1324 2024-05-05 12:23:50.000000 drf_standardized_response-1/LICENSE
--rw-rw-rw-   0        0        0       60 2024-04-29 15:40:10.000000 drf_standardized_response-1/MANIFEST.in
--rw-rw-rw-   0        0        0     6948 2024-05-07 10:35:30.484206 drf_standardized_response-1/PKG-INFO
--rw-rw-rw-   0        0        0     5845 2024-05-06 05:42:42.000000 drf_standardized_response-1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 10:35:30.463919 drf_standardized_response-1/drf_standardized_response/
--rw-rw-rw-   0        0        0        0 2024-04-29 15:25:16.000000 drf_standardized_response-1/drf_standardized_response/__init__.py
--rw-rw-rw-   0        0        0      218 2024-05-05 12:28:04.000000 drf_standardized_response-1/drf_standardized_response/apps.py
--rw-rw-rw-   0        0        0     2996 2024-05-07 10:30:30.000000 drf_standardized_response-1/drf_standardized_response/openapi.py
--rw-rw-rw-   0        0        0      800 2024-05-07 10:26:55.000000 drf_standardized_response-1/drf_standardized_response/renderers.py
--rw-rw-rw-   0        0        0     2888 2024-05-07 10:30:30.000000 drf_standardized_response-1/drf_standardized_response/response_standarizer.py
--rw-rw-rw-   0        0        0     2627 2024-05-05 16:04:30.000000 drf_standardized_response-1/drf_standardized_response/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-07 10:35:30.483206 drf_standardized_response-1/drf_standardized_response.egg-info/
--rw-rw-rw-   0        0        0     6948 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-07 10:35:30.000000 drf_standardized_response-1/drf_standardized_response.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      124 2024-05-06 03:07:32.000000 drf_standardized_response-1/pyproject.toml
--rw-rw-rw-   0        0        0      998 2024-05-07 10:35:30.485203 drf_standardized_response-1/setup.cfg
--rw-rw-rw-   0        0        0      122 2024-05-06 03:07:26.000000 drf_standardized_response-1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:17:15.340044 drf_standardized_response-1.1.0/
+-rw-rw-rw-   0        0        0     1324 2024-05-05 12:23:50.000000 drf_standardized_response-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2024-04-29 15:40:10.000000 drf_standardized_response-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7018 2024-05-08 10:17:15.340044 drf_standardized_response-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5911 2024-05-08 10:14:19.000000 drf_standardized_response-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 10:17:15.317082 drf_standardized_response-1.1.0/drf_standardized_response/
+-rw-rw-rw-   0        0        0        0 2024-04-29 15:25:16.000000 drf_standardized_response-1.1.0/drf_standardized_response/__init__.py
+-rw-rw-rw-   0        0        0      218 2024-05-05 12:28:04.000000 drf_standardized_response-1.1.0/drf_standardized_response/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:17:15.340044 drf_standardized_response-1.1.0/drf_standardized_response/openapi/
+-rw-rw-rw-   0        0        0      193 2024-05-08 10:16:25.000000 drf_standardized_response-1.1.0/drf_standardized_response/openapi/__init__.py
+-rw-rw-rw-   0        0        0     2848 2024-05-08 10:07:53.000000 drf_standardized_response-1.1.0/drf_standardized_response/openapi/mixins.py
+-rw-rw-rw-   0        0        0      246 2024-05-08 10:09:43.000000 drf_standardized_response-1.1.0/drf_standardized_response/openapi/serializers.py
+-rw-rw-rw-   0        0        0      535 2024-05-08 10:09:45.000000 drf_standardized_response-1.1.0/drf_standardized_response/openapi/utils.py
+-rw-rw-rw-   0        0        0      800 2024-05-07 10:26:55.000000 drf_standardized_response-1.1.0/drf_standardized_response/renderers.py
+-rw-rw-rw-   0        0        0     2888 2024-05-07 10:30:30.000000 drf_standardized_response-1.1.0/drf_standardized_response/response_standarizer.py
+-rw-rw-rw-   0        0        0     2627 2024-05-05 16:04:30.000000 drf_standardized_response-1.1.0/drf_standardized_response/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:17:15.340044 drf_standardized_response-1.1.0/drf_standardized_response.egg-info/
+-rw-rw-rw-   0        0        0     7018 2024-05-08 10:17:15.000000 drf_standardized_response-1.1.0/drf_standardized_response.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2024-05-08 10:17:15.000000 drf_standardized_response-1.1.0/drf_standardized_response.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 10:17:15.000000 drf_standardized_response-1.1.0/drf_standardized_response.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-08 10:17:15.000000 drf_standardized_response-1.1.0/drf_standardized_response.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-08 10:17:15.000000 drf_standardized_response-1.1.0/drf_standardized_response.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      124 2024-05-06 03:07:32.000000 drf_standardized_response-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1002 2024-05-08 10:17:15.340044 drf_standardized_response-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      122 2024-05-06 03:07:26.000000 drf_standardized_response-1.1.0/setup.py
```

### Comparing `drf_standardized_response-1/LICENSE` & `drf_standardized_response-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1/PKG-INFO` & `drf_standardized_response-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-standardized-response
-Version: 1
+Version: 1.1.0
 Home-page: https://github.com/HasanAshab/drf-standardized-response
 Author: Hasan Ashab
 Author-email: hasanashab.18205@example.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
@@ -223,15 +223,15 @@
 ```python
 REST_FRAMEWORK = {
     # other settings
     "DEFAULT_SCHEMA_CLASS": "drf_standardized_response.openapi.AutoSchema"
 }
 ```
 
-Alternatively, you can use the `drf_standardized_response.openapi.StandardizedAutoSchemaMixin` mixin to your own schema class. (useful when using `drf-standardized-errors`).
+Alternatively, you can use the `drf_standardized_response.openapi.mixins.StandardizedAutoSchemaMixin` mixin to your own schema class. (useful when using with [drf-standardized-errors](https://github.com/ghazi-git/drf-standardized-errors)).
 
 Now, the OpenAPI schema will be generated with the standardized response format.
 
 ### Disable Schema Standardization On Serializer
 You can disable openapi schema standardization on a serializer by setting the `should_standardize_schema` property to `False` on `Meta`.
 
 ```python
```

### Comparing `drf_standardized_response-1/README.md` & `drf_standardized_response-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 ```python
 REST_FRAMEWORK = {
     # other settings
     "DEFAULT_SCHEMA_CLASS": "drf_standardized_response.openapi.AutoSchema"
 }
 ```
 
-Alternatively, you can use the `drf_standardized_response.openapi.StandardizedAutoSchemaMixin` mixin to your own schema class. (useful when using `drf-standardized-errors`).
+Alternatively, you can use the `drf_standardized_response.openapi.mixins.StandardizedAutoSchemaMixin` mixin to your own schema class. (useful when using with [drf-standardized-errors](https://github.com/ghazi-git/drf-standardized-errors)).
 
 Now, the OpenAPI schema will be generated with the standardized response format.
 
 ### Disable Schema Standardization On Serializer
 You can disable openapi schema standardization on a serializer by setting the `should_standardize_schema` property to `False` on `Meta`.
 
 ```python
```

### Comparing `drf_standardized_response-1/drf_standardized_response/openapi.py` & `drf_standardized_response-1.1.0/drf_standardized_response/openapi/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from django.test.client import RequestFactory
 from rest_framework.response import Response
-from drf_standardized_errors.openapi import AutoSchema as BaseAutoSchema
 from drf_spectacular.utils import OpenApiResponse
 from .settings import package_settings
 
 
 class StandardizedSchemaMixin:
     def _get_response_for_code(
         self, serializer, status_code, media_types=None, direction="response"
@@ -76,11 +75,7 @@
             if field is not None
         }
 
         standardized_schema["properties"].update(unwrapped_data)
         standardized_schema["properties"]["data"] = schema
 
         return standardized_schema
-
-
-class AutoSchema(BaseAutoSchema, StandardizedSchemaMixin):
-    pass
```

### Comparing `drf_standardized_response-1/drf_standardized_response/renderers.py` & `drf_standardized_response-1.1.0/drf_standardized_response/renderers.py`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1/drf_standardized_response/response_standarizer.py` & `drf_standardized_response-1.1.0/drf_standardized_response/response_standarizer.py`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1/drf_standardized_response/settings.py` & `drf_standardized_response-1.1.0/drf_standardized_response/settings.py`

 * *Files identical despite different names*

### Comparing `drf_standardized_response-1/drf_standardized_response.egg-info/PKG-INFO` & `drf_standardized_response-1.1.0/drf_standardized_response.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-standardized-response
-Version: 1
+Version: 1.1.0
 Home-page: https://github.com/HasanAshab/drf-standardized-response
 Author: Hasan Ashab
 Author-email: hasanashab.18205@example.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
@@ -223,15 +223,15 @@
 ```python
 REST_FRAMEWORK = {
     # other settings
     "DEFAULT_SCHEMA_CLASS": "drf_standardized_response.openapi.AutoSchema"
 }
 ```
 
-Alternatively, you can use the `drf_standardized_response.openapi.StandardizedAutoSchemaMixin` mixin to your own schema class. (useful when using `drf-standardized-errors`).
+Alternatively, you can use the `drf_standardized_response.openapi.mixins.StandardizedAutoSchemaMixin` mixin to your own schema class. (useful when using with [drf-standardized-errors](https://github.com/ghazi-git/drf-standardized-errors)).
 
 Now, the OpenAPI schema will be generated with the standardized response format.
 
 ### Disable Schema Standardization On Serializer
 You can disable openapi schema standardization on a serializer by setting the `should_standardize_schema` property to `False` on `Meta`.
 
 ```python
```

### Comparing `drf_standardized_response-1/drf_standardized_response.egg-info/SOURCES.txt` & `drf_standardized_response-1.1.0/drf_standardized_response.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 drf_standardized_response/__init__.py
 drf_standardized_response/apps.py
-drf_standardized_response/openapi.py
 drf_standardized_response/renderers.py
 drf_standardized_response/response_standarizer.py
 drf_standardized_response/settings.py
 drf_standardized_response.egg-info/PKG-INFO
 drf_standardized_response.egg-info/SOURCES.txt
 drf_standardized_response.egg-info/dependency_links.txt
 drf_standardized_response.egg-info/requires.txt
-drf_standardized_response.egg-info/top_level.txt
+drf_standardized_response.egg-info/top_level.txt
+drf_standardized_response/openapi/__init__.py
+drf_standardized_response/openapi/mixins.py
+drf_standardized_response/openapi/serializers.py
+drf_standardized_response/openapi/utils.py
```

### Comparing `drf_standardized_response-1/setup.cfg` & `drf_standardized_response-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 2d73 7461 6e64 6172 6469   = drf-standardi
 00000020: 7a65 642d 7265 7370 6f6e 7365 0d0a 7665  zed-response..ve
-00000030: 7273 696f 6e20 3d20 310d 0a6c 6f6e 675f  rsion = 1..long_
-00000040: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-00000050: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00000070: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000080: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
-00000090: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
-000000a0: 7562 2e63 6f6d 2f48 6173 616e 4173 6861  ub.com/HasanAsha
-000000b0: 622f 6472 662d 7374 616e 6461 7264 697a  b/drf-standardiz
-000000c0: 6564 2d72 6573 706f 6e73 650d 0a61 7574  ed-response..aut
-000000d0: 686f 7220 3d20 4861 7361 6e20 4173 6861  hor = Hasan Asha
-000000e0: 620d 0a61 7574 686f 725f 656d 6169 6c20  b..author_email 
-000000f0: 3d20 6861 7361 6e61 7368 6162 2e31 3832  = hasanashab.182
-00000100: 3035 4065 7861 6d70 6c65 2e63 6f6d 0d0a  05@example.com..
-00000110: 6c69 6365 6e73 6520 3d20 4253 442d 332d  license = BSD-3-
-00000120: 436c 6175 7365 0d0a 636c 6173 7369 6669  Clause..classifi
-00000130: 6572 7320 3d20 0d0a 0945 6e76 6972 6f6e  ers = ...Environ
-00000140: 6d65 6e74 203a 3a20 5765 6220 456e 7669  ment :: Web Envi
-00000150: 726f 6e6d 656e 740d 0a09 4672 616d 6577  ronment...Framew
-00000160: 6f72 6b20 3a3a 2044 6a61 6e67 6f0d 0a09  ork :: Django...
-00000170: 4672 616d 6577 6f72 6b20 3a3a 2044 6a61  Framework :: Dja
-00000180: 6e67 6f20 3a3a 2034 2e30 0d0a 0949 6e74  ngo :: 4.0...Int
-00000190: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-000001a0: 3a20 4465 7665 6c6f 7065 7273 0d0a 094c  : Developers...L
-000001b0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001c0: 7072 6f76 6564 203a 3a20 4253 4420 4c69  proved :: BSD Li
-000001d0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
-000001e0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-000001f0: 6e64 6570 656e 6465 6e74 0d0a 0950 726f  ndependent...Pro
-00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000210: 6520 3a3a 2050 7974 686f 6e0d 0a09 5072  e :: Python...Pr
-00000220: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000230: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000240: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
-00000250: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000260: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790d  on :: 3 :: Only.
-00000270: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000280: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000290: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
-000002a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-000002c0: 310d 0a09 5072 6f67 7261 6d6d 696e 6720  1...Programming 
-000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002e0: 6f6e 203a 3a20 332e 3132 0d0a 0954 6f70  on :: 3.12...Top
-000002f0: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-00000300: 3a20 5757 572f 4854 5450 0d0a 0954 6f70  : WWW/HTTP...Top
-00000310: 6963 203a 3a20 496e 7465 726e 6574 203a  ic :: Internet :
-00000320: 3a20 5757 572f 4854 5450 203a 3a20 4479  : WWW/HTTP :: Dy
-00000330: 6e61 6d69 6320 436f 6e74 656e 740d 0a0d  namic Content...
-00000340: 0a5b 6f70 7469 6f6e 735d 0d0a 696e 636c  .[options]..incl
-00000350: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-00000360: 203d 2074 7275 650d 0a70 6163 6b61 6765   = true..package
-00000370: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000380: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000390: 2e31 300d 0a69 6e73 7461 6c6c 5f72 6571  .10..install_req
-000003a0: 7569 7265 7320 3d20 0d0a 0944 6a61 6e67  uires = ...Djang
-000003b0: 6f20 3e3d 2034 2e30 0d0a 0d0a 5b65 6767  o >= 4.0....[egg
-000003c0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000003d0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000003e0: 2030 0d0a 0d0a                            0....
+00000030: 7273 696f 6e20 3d20 312e 312e 300d 0a6c  rsion = 1.1.0..l
+00000040: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+00000050: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
+00000060: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+00000070: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+00000080: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+00000090: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
+000000a0: 6769 7468 7562 2e63 6f6d 2f48 6173 616e  github.com/Hasan
+000000b0: 4173 6861 622f 6472 662d 7374 616e 6461  Ashab/drf-standa
+000000c0: 7264 697a 6564 2d72 6573 706f 6e73 650d  rdized-response.
+000000d0: 0a61 7574 686f 7220 3d20 4861 7361 6e20  .author = Hasan 
+000000e0: 4173 6861 620d 0a61 7574 686f 725f 656d  Ashab..author_em
+000000f0: 6169 6c20 3d20 6861 7361 6e61 7368 6162  ail = hasanashab
+00000100: 2e31 3832 3035 4065 7861 6d70 6c65 2e63  .18205@example.c
+00000110: 6f6d 0d0a 6c69 6365 6e73 6520 3d20 4253  om..license = BS
+00000120: 442d 332d 436c 6175 7365 0d0a 636c 6173  D-3-Clause..clas
+00000130: 7369 6669 6572 7320 3d20 0d0a 0945 6e76  sifiers = ...Env
+00000140: 6972 6f6e 6d65 6e74 203a 3a20 5765 6220  ironment :: Web 
+00000150: 456e 7669 726f 6e6d 656e 740d 0a09 4672  Environment...Fr
+00000160: 616d 6577 6f72 6b20 3a3a 2044 6a61 6e67  amework :: Djang
+00000170: 6f0d 0a09 4672 616d 6577 6f72 6b20 3a3a  o...Framework ::
+00000180: 2044 6a61 6e67 6f20 3a3a 2034 2e30 0d0a   Django :: 4.0..
+00000190: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+000001a0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+000001b0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+000001c0: 4920 4170 7072 6f76 6564 203a 3a20 4253  I Approved :: BS
+000001d0: 4420 4c69 6365 6e73 650d 0a09 4f70 6572  D License...Oper
+000001e0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+000001f0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
+00000200: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000210: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
+00000220: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000230: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000240: 203a 3a20 330d 0a09 5072 6f67 7261 6d6d   :: 3...Programm
+00000250: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000260: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
+00000270: 6e6c 790d 0a09 5072 6f67 7261 6d6d 696e  nly...Programmin
+00000280: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000290: 7468 6f6e 203a 3a20 332e 3130 0d0a 0950  thon :: 3.10...P
+000002a0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002b0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002c0: 2033 2e31 310d 0a09 5072 6f67 7261 6d6d   3.11...Programm
+000002d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002e0: 5079 7468 6f6e 203a 3a20 332e 3132 0d0a  Python :: 3.12..
+000002f0: 0954 6f70 6963 203a 3a20 496e 7465 726e  .Topic :: Intern
+00000300: 6574 203a 3a20 5757 572f 4854 5450 0d0a  et :: WWW/HTTP..
+00000310: 0954 6f70 6963 203a 3a20 496e 7465 726e  .Topic :: Intern
+00000320: 6574 203a 3a20 5757 572f 4854 5450 203a  et :: WWW/HTTP :
+00000330: 3a20 4479 6e61 6d69 6320 436f 6e74 656e  : Dynamic Conten
+00000340: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
+00000350: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000360: 6461 7461 203d 2074 7275 650d 0a70 6163  data = true..pac
+00000370: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
+00000380: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000390: 203e 3d33 2e31 300d 0a69 6e73 7461 6c6c   >=3.10..install
+000003a0: 5f72 6571 7569 7265 7320 3d20 0d0a 0944  _requires = ...D
+000003b0: 6a61 6e67 6f20 3e3d 2034 2e30 0d0a 0d0a  jango >= 4.0....
+000003c0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000003d0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000003e0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```


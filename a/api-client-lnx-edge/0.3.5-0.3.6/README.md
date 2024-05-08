# Comparing `tmp/api-client-lnx-edge-0.3.5.tar.gz` & `tmp/api-client-lnx-edge-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ntulli/Leadnomics/edge-api-client/dist/.tmp-vrzgx_ds/api-client-lnx-edge-0.3.5.tar", last modified: Tue Oct 31 14:46:46 2023, max compression
+gzip compressed data, was "/Users/ntulli/Leadnomics/edge-api-client/dist/.tmp-ce3aveo1/api-client-lnx-edge-0.3.6.tar", last modified: Wed May  8 17:06:23 2024, max compression
```

## Comparing `api-client-lnx-edge-0.3.5.tar` & `api-client-lnx-edge-0.3.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/
--rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/PKG-INFO
--rw-r--r--   0 ntulli     (502) staff       (20)      738 2023-08-24 11:54:36.000000 api-client-lnx-edge-0.3.5/README.md
--rw-r--r--   0 ntulli     (502) staff       (20)      100 2021-08-23 17:29:30.000000 api-client-lnx-edge-0.3.5/pyproject.toml
--rw-r--r--   0 ntulli     (502) staff       (20)       38 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/setup.cfg
--rw-r--r--   0 ntulli     (502) staff       (20)      767 2023-10-31 14:46:10.000000 api-client-lnx-edge-0.3.5/setup.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/src/
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/src/api_client_lnx_edge.egg-info/
--rw-r--r--   0 ntulli     (502) staff       (20)     1104 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/src/api_client_lnx_edge.egg-info/PKG-INFO
--rw-r--r--   0 ntulli     (502) staff       (20)      542 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/src/api_client_lnx_edge.egg-info/SOURCES.txt
--rw-r--r--   0 ntulli     (502) staff       (20)        1 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/src/api_client_lnx_edge.egg-info/dependency_links.txt
--rw-r--r--   0 ntulli     (502) staff       (20)       50 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/src/api_client_lnx_edge.egg-info/requires.txt
--rw-r--r--   0 ntulli     (502) staff       (20)       16 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/src/api_client_lnx_edge.egg-info/top_level.txt
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/src/edge_api_client/
--rw-r--r--   0 ntulli     (502) staff       (20)       26 2022-10-11 15:31:34.000000 api-client-lnx-edge-0.3.5/src/edge_api_client/__init__.py
--rw-r--r--   0 ntulli     (502) staff       (20)     1577 2023-08-30 16:18:52.000000 api-client-lnx-edge-0.3.5/src/edge_api_client/base.py
--rw-r--r--   0 ntulli     (502) staff       (20)    22497 2023-10-31 12:57:35.000000 api-client-lnx-edge-0.3.5/src/edge_api_client/edge.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/src/edge_api_client/utilities/
--rw-r--r--   0 ntulli     (502) staff       (20)       90 2023-08-31 12:18:15.000000 api-client-lnx-edge-0.3.5/src/edge_api_client/utilities/__init__.py
--rw-r--r--   0 ntulli     (502) staff       (20)     2532 2023-08-31 12:17:35.000000 api-client-lnx-edge-0.3.5/src/edge_api_client/utilities/funcs.py
--rw-r--r--   0 ntulli     (502) staff       (20)     4978 2023-10-31 14:46:10.000000 api-client-lnx-edge-0.3.5/src/edge_api_client/utilities/schemas.py
-drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2023-10-31 14:46:46.000000 api-client-lnx-edge-0.3.5/tests/
--rw-r--r--   0 ntulli     (502) staff       (20)      322 2021-08-23 19:03:52.000000 api-client-lnx-edge-0.3.5/tests/test_auth.py
--rw-r--r--   0 ntulli     (502) staff       (20)     1075 2023-10-31 14:46:10.000000 api-client-lnx-edge-0.3.5/tests/test_endpoints.py
--rw-r--r--   0 ntulli     (502) staff       (20)      810 2023-06-05 21:15:05.000000 api-client-lnx-edge-0.3.5/tests/test_schemas.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/
+-rw-r--r--   0 ntulli     (502) staff       (20)     1104 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/PKG-INFO
+-rw-r--r--   0 ntulli     (502) staff       (20)      738 2023-08-24 11:54:36.000000 api-client-lnx-edge-0.3.6/README.md
+-rw-r--r--   0 ntulli     (502) staff       (20)      100 2021-08-23 17:29:30.000000 api-client-lnx-edge-0.3.6/pyproject.toml
+-rw-r--r--   0 ntulli     (502) staff       (20)       38 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/setup.cfg
+-rw-r--r--   0 ntulli     (502) staff       (20)      767 2024-05-08 17:04:00.000000 api-client-lnx-edge-0.3.6/setup.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/src/
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/src/api_client_lnx_edge.egg-info/
+-rw-r--r--   0 ntulli     (502) staff       (20)     1104 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/src/api_client_lnx_edge.egg-info/PKG-INFO
+-rw-r--r--   0 ntulli     (502) staff       (20)      542 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/src/api_client_lnx_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)        1 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/src/api_client_lnx_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)       50 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/src/api_client_lnx_edge.egg-info/requires.txt
+-rw-r--r--   0 ntulli     (502) staff       (20)       16 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/src/api_client_lnx_edge.egg-info/top_level.txt
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/src/edge_api_client/
+-rw-r--r--   0 ntulli     (502) staff       (20)       26 2022-10-11 15:31:34.000000 api-client-lnx-edge-0.3.6/src/edge_api_client/__init__.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     1577 2023-08-30 16:18:52.000000 api-client-lnx-edge-0.3.6/src/edge_api_client/base.py
+-rw-r--r--   0 ntulli     (502) staff       (20)    22623 2024-05-08 17:03:24.000000 api-client-lnx-edge-0.3.6/src/edge_api_client/edge.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/src/edge_api_client/utilities/
+-rw-r--r--   0 ntulli     (502) staff       (20)       90 2023-08-31 12:18:15.000000 api-client-lnx-edge-0.3.6/src/edge_api_client/utilities/__init__.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     2532 2023-08-31 12:17:35.000000 api-client-lnx-edge-0.3.6/src/edge_api_client/utilities/funcs.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     5166 2024-05-08 17:03:16.000000 api-client-lnx-edge-0.3.6/src/edge_api_client/utilities/schemas.py
+drwxr-xr-x   0 ntulli     (502) staff       (20)        0 2024-05-08 17:06:23.000000 api-client-lnx-edge-0.3.6/tests/
+-rw-r--r--   0 ntulli     (502) staff       (20)      322 2021-08-23 19:03:52.000000 api-client-lnx-edge-0.3.6/tests/test_auth.py
+-rw-r--r--   0 ntulli     (502) staff       (20)     1075 2023-10-31 14:46:10.000000 api-client-lnx-edge-0.3.6/tests/test_endpoints.py
+-rw-r--r--   0 ntulli     (502) staff       (20)      810 2023-06-05 21:15:05.000000 api-client-lnx-edge-0.3.6/tests/test_schemas.py
```

### Comparing `api-client-lnx-edge-0.3.5/PKG-INFO` & `api-client-lnx-edge-0.3.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-client-lnx-edge
-Version: 0.3.5
+Version: 0.3.6
 Summary: Client for the LNX Edge API
 Home-page: https://github.com/Lnmix/edge_api_client
 Author: Nick Tulli
 Author-email: ntulli@leadnomics.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `api-client-lnx-edge-0.3.5/README.md` & `api-client-lnx-edge-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.5/setup.py` & `api-client-lnx-edge-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='api-client-lnx-edge',
-    version='0.3.5',
+    version='0.3.6',
     description='Client for the LNX Edge API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Lnmix/edge_api_client',
     author='Nick Tulli',
     author_email='ntulli@leadnomics.com',
     package_dir={'': 'src'},
```

### Comparing `api-client-lnx-edge-0.3.5/src/api_client_lnx_edge.egg-info/PKG-INFO` & `api-client-lnx-edge-0.3.6/src/api_client_lnx_edge.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-client-lnx-edge
-Version: 0.3.5
+Version: 0.3.6
 Summary: Client for the LNX Edge API
 Home-page: https://github.com/Lnmix/edge_api_client
 Author: Nick Tulli
 Author-email: ntulli@leadnomics.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `api-client-lnx-edge-0.3.5/src/api_client_lnx_edge.egg-info/SOURCES.txt` & `api-client-lnx-edge-0.3.6/src/api_client_lnx_edge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.5/src/edge_api_client/base.py` & `api-client-lnx-edge-0.3.6/src/edge_api_client/base.py`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.5/src/edge_api_client/edge.py` & `api-client-lnx-edge-0.3.6/src/edge_api_client/edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
                      lifetime_affiliate_click_cap: int = None,
                      traffic_types: List = None,
                      pixel_behavior: str = 'dedupe',
                      allow_query_passthrough: bool = False,
                      allow_pageview_pixel: bool = False,
                      allow_forced_click_conversion: bool = False,
                      creatives: List[int] = None,
+                     traffic_type: str = None,
                      unsubscribe_link: str = None,
                      suppression_list: str = None,
                      from_lines: str = None,
                      subject_lines: str = None,
                      redirect_offer: int = None,
                      redirect_percent: float = None,
                      cap_redirect_offer: int = None,
@@ -175,14 +176,15 @@
             'defaultAffiliateConvCap': default_affiliate_conversion_cap or kwargs.get('defaultAffiliateConvCap'),
             'lifetimeAffiliateClickCap': lifetime_affiliate_click_cap or kwargs.get('lifetimeAffiliateClickCap'),
             'trafficTypes': traffic_types or kwargs.get('trafficTypes') or [],
             'pixelBehavior': pixel_behavior or kwargs.get('pixelBehavior'),
             'allowQueryPassthrough': allow_query_passthrough or kwargs.get('allowQueryPassthrough'),
             'allowPageviewPixel': allow_pageview_pixel or kwargs.get('allowPageviewPixel'),
             'allowForcedClickConversion': allow_forced_click_conversion or kwargs.get('allowForcedClickConversion'),
+            'trafficType': traffic_type or kwargs.get('trafficType', 'Click'),
             'unsubscribe_link': unsubscribe_link,
             'suppression_list': suppression_list,
             'from_lines': from_lines,
             'subject_lines': subject_lines,
             'redirectOffer': redirect_offer or kwargs.get('redirectOffer'),
             'redirectPercent': redirect_percent or kwargs.get('redirectPercent'),
             'capRedirectOffer': cap_redirect_offer or kwargs.get('capRedirectOffer')
```

### Comparing `api-client-lnx-edge-0.3.5/src/edge_api_client/utilities/funcs.py` & `api-client-lnx-edge-0.3.6/src/edge_api_client/utilities/funcs.py`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.5/src/edge_api_client/utilities/schemas.py` & `api-client-lnx-edge-0.3.6/src/edge_api_client/utilities/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     Contextual = 'Contextual'
     Display = 'Display'
     Search = 'Search'
     Social = 'Social'
     Native = 'Native'
     MobileAds = 'MobileAds'
 
+class OfferTrafficTypeEnum(enum.Enum):
+    Click = 'Click'
+    Call = 'Call'
+
 
 class CreateOfferSchema(marshmallow.Schema):
     friendlyName = marshmallow.fields.Str(required=True)
     category = marshmallow.fields.Int(required=True)
     description = marshmallow.fields.Str()
     domain = marshmallow.fields.Int(required=True)
     customFallbackUrl = marshmallow.fields.Str(required=True)
@@ -51,14 +55,15 @@
     defaultAffiliateConvCap = marshmallow.fields.Int(allow_none=True)
     lifetimeAffiliateClickCap = marshmallow.fields.Int(allow_none=True)
     trafficTypes = marshmallow.fields.List(marshmallow.fields.Enum(enum=TrafficTypesEnum))
     pixelBehavior = marshmallow.fields.Enum(enum=PixelBehaviorEnum, dump_default=PixelBehaviorEnum.dedupe)
     allowQueryPassthrough = marshmallow.fields.Bool(dump_default=False)
     allowPageviewPixel = marshmallow.fields.Bool(dump_default=False)
     allowForcedClickConversion = marshmallow.fields.Bool(dump_default=False)
+    trafficType = marshmallow.fields.Enum(enum=OfferTrafficTypeEnum, dump_default=OfferTrafficTypeEnum.Click)
     unsubscribe_link = marshmallow.fields.Str()
     suppression_list = marshmallow.fields.Str()
     from_lines = marshmallow.fields.Str()
     subject_lines = marshmallow.fields.Str()
     redirectOffer = marshmallow.fields.Int(allow_none=True)
     redirectPercent = marshmallow.fields.Float(allow_none=True)
     capRedirectOffer = marshmallow.fields.Int(allow_none=True)
```

### Comparing `api-client-lnx-edge-0.3.5/tests/test_endpoints.py` & `api-client-lnx-edge-0.3.6/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `api-client-lnx-edge-0.3.5/tests/test_schemas.py` & `api-client-lnx-edge-0.3.6/tests/test_schemas.py`

 * *Files identical despite different names*


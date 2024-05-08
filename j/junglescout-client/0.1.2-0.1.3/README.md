# Comparing `tmp/junglescout_client-0.1.2.tar.gz` & `tmp/junglescout_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junglescout_client-0.1.2.tar", max compression
+gzip compressed data, was "junglescout_client-0.1.3.tar", max compression
```

## Comparing `junglescout_client-0.1.2.tar` & `junglescout_client-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1068 2024-03-20 18:23:49.913683 junglescout_client-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1995 2024-03-20 18:23:49.913683 junglescout_client-0.1.2/README.md
--rw-r--r--   0        0        0     3346 2024-03-20 18:24:32.477738 junglescout_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      164 2024-03-20 18:24:32.477738 junglescout_client-0.1.2/src/junglescout/__init__.py
--rw-r--r--   0        0        0    15467 2024-03-20 18:23:49.913683 junglescout_client-0.1.2/src/junglescout/client.py
--rw-r--r--   0        0        0       54 2024-03-20 18:23:49.913683 junglescout_client-0.1.2/src/junglescout/models/__init__.py
--rw-r--r--   0        0        0      673 2024-03-20 18:23:49.913683 junglescout_client-0.1.2/src/junglescout/models/parameters/__init__.py
--rw-r--r--   0        0        0      260 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/api_type.py
--rw-r--r--   0        0        0      412 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/attributes.py
--rw-r--r--   0        0        0     1425 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/filter_options.py
--rw-r--r--   0        0        0     8737 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/marketplace.py
--rw-r--r--   0        0        0     1116 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/params.py
--rw-r--r--   0        0        0     3184 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/product_filter_options.py
--rw-r--r--   0        0        0      740 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/product_sort.py
--rw-r--r--   0        0        0      298 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/product_tiers.py
--rw-r--r--   0        0        0      372 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/seller_types.py
--rw-r--r--   0        0        0     1511 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/parameters/sort.py
--rw-r--r--   0        0        0      171 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/__init__.py
--rw-r--r--   0        0        0     1914 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/base_request.py
--rw-r--r--   0        0        0     1708 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/historical_search_volume_request.py
--rw-r--r--   0        0        0     2255 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/keyword_by_asin_request.py
--rw-r--r--   0        0        0     1950 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/keywords_by_keyword_request.py
--rw-r--r--   0        0        0      242 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/method.py
--rw-r--r--   0        0        0     3014 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/product_database_request.py
--rw-r--r--   0        0        0      341 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/request_type.py
--rw-r--r--   0        0        0     1828 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/sales_estimates_request.py
--rw-r--r--   0        0        0      826 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/requests/share_of_voice_request.py
--rw-r--r--   0        0        0     1298 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/responses/__init__.py
--rw-r--r--   0        0        0     1533 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/responses/api_response.py
--rw-r--r--   0        0        0     1282 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/responses/historical_search_volume.py
--rw-r--r--   0        0        0     4490 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/responses/keyword_by_asin.py
--rw-r--r--   0        0        0     2210 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/responses/keyword_by_keyword.py
--rw-r--r--   0        0        0     5305 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/responses/product_database.py
--rw-r--r--   0        0        0     1907 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/responses/sales_estimates.py
--rw-r--r--   0        0        0      318 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/responses/serializer_helpers.py
--rw-r--r--   0        0        0     4606 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/models/responses/share_of_voice.py
--rw-r--r--   0        0        0     1969 2024-03-20 18:23:49.917683 junglescout_client-0.1.2/src/junglescout/session.py
--rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 junglescout_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-08 16:34:11.965936 junglescout_client-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     1995 2024-05-08 16:34:11.965936 junglescout_client-0.1.3/README.md
+-rw-r--r--   0        0        0     3303 2024-05-08 16:34:54.710105 junglescout_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-05-08 16:34:54.710105 junglescout_client-0.1.3/src/junglescout/__init__.py
+-rw-r--r--   0        0        0    15485 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/client.py
+-rw-r--r--   0        0        0       54 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/__init__.py
+-rw-r--r--   0        0        0      673 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/__init__.py
+-rw-r--r--   0        0        0      260 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/api_type.py
+-rw-r--r--   0        0        0      412 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/attributes.py
+-rw-r--r--   0        0        0     1425 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/filter_options.py
+-rw-r--r--   0        0        0     8737 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/marketplace.py
+-rw-r--r--   0        0        0     1116 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/params.py
+-rw-r--r--   0        0        0     3184 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/product_filter_options.py
+-rw-r--r--   0        0        0      740 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/product_sort.py
+-rw-r--r--   0        0        0      298 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/product_tiers.py
+-rw-r--r--   0        0        0      372 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/seller_types.py
+-rw-r--r--   0        0        0     1511 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/parameters/sort.py
+-rw-r--r--   0        0        0      171 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/__init__.py
+-rw-r--r--   0        0        0     1914 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/base_request.py
+-rw-r--r--   0        0        0     1708 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/historical_search_volume_request.py
+-rw-r--r--   0        0        0     2255 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/keyword_by_asin_request.py
+-rw-r--r--   0        0        0     1950 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/keywords_by_keyword_request.py
+-rw-r--r--   0        0        0      242 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/method.py
+-rw-r--r--   0        0        0     3014 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/product_database_request.py
+-rw-r--r--   0        0        0      341 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/request_type.py
+-rw-r--r--   0        0        0     1828 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/sales_estimates_request.py
+-rw-r--r--   0        0        0      826 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/requests/share_of_voice_request.py
+-rw-r--r--   0        0        0     1298 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/responses/__init__.py
+-rw-r--r--   0        0        0     1533 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/responses/api_response.py
+-rw-r--r--   0        0        0     1282 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/responses/historical_search_volume.py
+-rw-r--r--   0        0        0     4490 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/responses/keyword_by_asin.py
+-rw-r--r--   0        0        0     2210 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/responses/keyword_by_keyword.py
+-rw-r--r--   0        0        0     5305 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/responses/product_database.py
+-rw-r--r--   0        0        0     2011 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/responses/sales_estimates.py
+-rw-r--r--   0        0        0      318 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/responses/serializer_helpers.py
+-rw-r--r--   0        0        0     4606 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/models/responses/share_of_voice.py
+-rw-r--r--   0        0        0     1969 2024-05-08 16:34:11.969936 junglescout_client-0.1.3/src/junglescout/session.py
+-rw-r--r--   0        0        0     3098 1970-01-01 00:00:00.000000 junglescout_client-0.1.3/PKG-INFO
```

### Comparing `junglescout_client-0.1.2/LICENSE.txt` & `junglescout_client-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/README.md` & `junglescout_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/pyproject.toml` & `junglescout_client-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 package-mode = true
 name = "junglescout-client"
 packages = [
     { include = "junglescout", from = "src" },
 ]
-version = "0.1.2"
+version = "0.1.3"
 license = "MIT"
 authors = ["Jungle Scout <support@junglescout.com>"]
 description = "Jungle Scout API Client"
 readme = "README.md"
 repository = "https://github.com/Junglescout/jungle-scout-python-client"
 
 [tool.poetry.dependencies]
@@ -146,11 +146,11 @@
 [tool.semantic_release.publish]
 dist_glob_patterns = ["dist/*"]
 upload_to_vcs_release = true
 
 
 [tool.poetry.urls]
 Homepage = "https://developer.junglescout.com/api"
-Documentation = "https://jungle-scout-junglescout-python-client.readthedocs-hosted.com/en/latest/"
+Documentation = "https://python-client.junglescout.com"
 "Postman Collection" = "https://postman.junglescout.com/"
 Repository = "https://github.com/Junglescout/junglescout-python-client.git"
 Issues = "https://github.com/Junglescout/junglescout-python-client/issues"
```

### Comparing `junglescout_client-0.1.2/src/junglescout/client.py` & `junglescout_client-0.1.3/src/junglescout/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,16 +305,16 @@
         marketplace: Optional[Marketplace] = None,
         page_size: Optional[int] = 10,
         page: Optional[str] = None,
     ) -> APIResponse[List[ProductDatabase]]:
         """Retrieves product data from the Jungle Scout Product Database.
 
         Args:
-            include_keywords: List of keywords to include in the search.
-            exclude_keywords: List of keywords to exclude from the search.
+            include_keywords: List of keywords or ASINs to include in the search.
+            exclude_keywords: List of keywords or ASINs to exclude from the search.
             categories: List of categories to filter the search by. Must be valid inside the
                 categories of the selected Marketplace.
             product_tiers: List of product tiers to filter the search by. Must use the ProductTiers enum.
             seller_types: List of seller types to filter the search by. Must use the SellerTypes enum.
             product_filter_options: Additional product filter options. Must use the ProductFilterOptions class.
             product_sort_option: Sorting option for the search results. Must use the ProductSort enum.
             marketplace: Marketplace to search in. If not provided, the default marketplace will be used.
```

### Comparing `junglescout_client-0.1.2/src/junglescout/models/parameters/__init__.py` & `junglescout_client-0.1.3/src/junglescout/models/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/parameters/filter_options.py` & `junglescout_client-0.1.3/src/junglescout/models/parameters/filter_options.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/parameters/marketplace.py` & `junglescout_client-0.1.3/src/junglescout/models/parameters/marketplace.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/parameters/params.py` & `junglescout_client-0.1.3/src/junglescout/models/parameters/params.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/parameters/product_filter_options.py` & `junglescout_client-0.1.3/src/junglescout/models/parameters/product_filter_options.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/parameters/product_sort.py` & `junglescout_client-0.1.3/src/junglescout/models/parameters/product_sort.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/parameters/sort.py` & `junglescout_client-0.1.3/src/junglescout/models/parameters/sort.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/requests/base_request.py` & `junglescout_client-0.1.3/src/junglescout/models/requests/base_request.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/requests/historical_search_volume_request.py` & `junglescout_client-0.1.3/src/junglescout/models/requests/historical_search_volume_request.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/requests/keyword_by_asin_request.py` & `junglescout_client-0.1.3/src/junglescout/models/requests/keyword_by_asin_request.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/requests/keywords_by_keyword_request.py` & `junglescout_client-0.1.3/src/junglescout/models/requests/keywords_by_keyword_request.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/requests/product_database_request.py` & `junglescout_client-0.1.3/src/junglescout/models/requests/product_database_request.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/requests/sales_estimates_request.py` & `junglescout_client-0.1.3/src/junglescout/models/requests/sales_estimates_request.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/requests/share_of_voice_request.py` & `junglescout_client-0.1.3/src/junglescout/models/requests/share_of_voice_request.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/responses/__init__.py` & `junglescout_client-0.1.3/src/junglescout/models/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/responses/api_response.py` & `junglescout_client-0.1.3/src/junglescout/models/responses/api_response.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/responses/historical_search_volume.py` & `junglescout_client-0.1.3/src/junglescout/models/responses/historical_search_volume.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/responses/keyword_by_asin.py` & `junglescout_client-0.1.3/src/junglescout/models/responses/keyword_by_asin.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/responses/keyword_by_keyword.py` & `junglescout_client-0.1.3/src/junglescout/models/responses/keyword_by_keyword.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/responses/product_database.py` & `junglescout_client-0.1.3/src/junglescout/models/responses/product_database.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/models/responses/sales_estimates.py` & `junglescout_client-0.1.3/src/junglescout/models/responses/sales_estimates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import List
+from typing import List, Optional
 
 from pydantic import BaseModel, Field, field_serializer
 
 from .serializer_helpers import serialize_date
 
 
 class SalesEstimateData(BaseModel):
@@ -17,24 +17,28 @@
     def _serialize_date(self, v: datetime):  # noqa: PLR6301
         return serialize_date(v)
 
 
 class SalesEstimateAttributes(BaseModel):
     """The attributes of the sales estimate."""
 
-    asin: str = Field(
-        default=..., description="The ASIN (Amazon Standard Identification Number) associated with the sales estimate."
+    asin: Optional[str] = Field(
+        default=None, description="The ASIN (Amazon Standard Identification Number) associated with the sales estimate."
     )
-    is_parent: bool = Field(default=..., description="A boolean indicating whether the ASIN is a parent ASIN.")
-    is_variant: bool = Field(default=..., description="A boolean indicating whether the ASIN is a variant.")
-    is_standalone: bool = Field(
-        default=..., description="A boolean indicating whether the ASIN is a standalone product."
+    is_parent: Optional[bool] = Field(
+        default=None, description="A boolean indicating whether the ASIN is a parent ASIN."
+    )
+    is_variant: Optional[bool] = Field(default=None, description="A boolean indicating whether the ASIN is a variant.")
+    is_standalone: Optional[bool] = Field(
+        default=None, description="A boolean indicating whether the ASIN is a standalone product."
+    )
+    parent_asin: Optional[str] = Field(default=None, description="The parent ASIN associated with the sales estimate.")
+    variants: Optional[List[str]] = Field(
+        default=None, description="The variant ASINs associated with the sales estimate."
     )
-    parent_asin: str = Field(default=..., description="The parent ASIN associated with the sales estimate.")
-    variants: List[str] = Field(default=..., description="The variant ASINs associated with the sales estimate.")
     data: List[SalesEstimateData] = Field(default=..., description="The sales estimate data.")
 
 
 class SalesEstimates(BaseModel):
     """Represents a list of sales estimates."""
 
     id: str = Field(default=..., description="The ID of the sales estimate.")
```

### Comparing `junglescout_client-0.1.2/src/junglescout/models/responses/share_of_voice.py` & `junglescout_client-0.1.3/src/junglescout/models/responses/share_of_voice.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/src/junglescout/session.py` & `junglescout_client-0.1.3/src/junglescout/session.py`

 * *Files identical despite different names*

### Comparing `junglescout_client-0.1.2/PKG-INFO` & `junglescout_client-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junglescout-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Jungle Scout API Client
 Home-page: https://github.com/Junglescout/jungle-scout-python-client
 License: MIT
 Author: Jungle Scout
 Author-email: support@junglescout.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Project-URL: Documentation, https://jungle-scout-junglescout-python-client.readthedocs-hosted.com/en/latest/
+Project-URL: Documentation, https://python-client.junglescout.com
 Project-URL: Homepage, https://developer.junglescout.com/api
 Project-URL: Issues, https://github.com/Junglescout/junglescout-python-client/issues
 Project-URL: Postman Collection, https://postman.junglescout.com/
 Project-URL: Repository, https://github.com/Junglescout/junglescout-python-client.git
 Description-Content-Type: text/markdown
 
 # Jungle Scout Python Client
```


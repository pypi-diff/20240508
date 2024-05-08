# Comparing `tmp/fast_tradier_client-0.3.4.tar.gz` & `tmp/fast_tradier_client-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_tradier_client-0.3.4.tar", last modified: Wed Apr 17 05:18:04 2024, max compression
+gzip compressed data, was "fast_tradier_client-1.0.tar", last modified: Wed May  8 02:11:48 2024, max compression
```

## Comparing `fast_tradier_client-0.3.4.tar` & `fast_tradier_client-1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:18:04.098229 fast_tradier_client-0.3.4/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11014 2024-04-17 05:18:04.098229 fast_tradier_client-0.3.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10270 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:18:04.090229 fast_tradier_client-0.3.4/fast_tradier/
--rw-rw-rw-   0 root         (0) root         (0)    16877 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/FastTradierAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)    16334 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/FastTradierClient.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:18:04.094229 fast_tradier_client-0.3.4/fast_tradier/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     3237 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/interfaces/IBrokerAsyncClient.py
--rw-rw-rw-   0 root         (0) root         (0)     3063 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/interfaces/IBrokerClient.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/interfaces/IModel.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/interfaces/IRealTimeQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:18:04.094229 fast_tradier_client-0.3.4/fast_tradier/models/
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/DataClassModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)     1248 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/ModelBase.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:18:04.094229 fast_tradier_client-0.3.4/fast_tradier/models/account/
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/account/AccountBalance.py
--rw-rw-rw-   0 root         (0) root         (0)     1664 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/account/AccountOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      359 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/account/Position.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:18:04.094229 fast_tradier_client-0.3.4/fast_tradier/models/market_data/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/market_data/Hlocv.py
--rw-rw-rw-   0 root         (0) root         (0)     1841 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/market_data/Quote.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/market_data/TradierQuote.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/market_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:18:04.094229 fast_tradier_client-0.3.4/fast_tradier/models/trading/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/trading/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/trading/EquityOrder.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/trading/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)     5606 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/trading/OptionOrder.py
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/trading/OrderBase.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/trading/PriceTypes.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/trading/Sides.py
--rw-rw-rw-   0 root         (0) root         (0)     2385 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/trading/TOSTradierConverter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/models/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:18:04.094229 fast_tradier_client-0.3.4/fast_tradier/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/utils/OptionUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/utils/TimeUtils.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/utils/YFinanceQuoteProvider.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/fast_tradier/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 05:18:04.094229 fast_tradier_client-0.3.4/fast_tradier_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11014 2024-04-17 05:18:04.000000 fast_tradier_client-0.3.4/fast_tradier_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1529 2024-04-17 05:18:04.000000 fast_tradier_client-0.3.4/fast_tradier_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 05:18:04.000000 fast_tradier_client-0.3.4/fast_tradier_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2024-04-17 05:18:04.000000 fast_tradier_client-0.3.4/fast_tradier_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-17 05:18:04.000000 fast_tradier_client-0.3.4/fast_tradier_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 05:18:04.098229 fast_tradier_client-0.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-04-17 05:17:36.000000 fast_tradier_client-0.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.530418 fast_tradier_client-1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11012 2024-05-08 02:11:48.530418 fast_tradier_client-1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10270 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/
+-rw-rw-rw-   0 root         (0) root         (0)    16877 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/FastTradierAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    16334 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/FastTradierClient.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/IBrokerAsyncClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3063 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/IBrokerClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/IModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/IRealTimeQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/models/
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/DataClassModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/ModelBase.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/models/account/
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/account/AccountBalance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1664 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/account/AccountOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      359 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/account/Position.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/models/market_data/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/market_data/Hlocv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1841 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/market_data/Quote.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/market_data/TradierQuote.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/market_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/models/trading/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/EquityOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)     2024 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/OptionOrder.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/OrderBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/PriceTypes.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/Sides.py
+-rw-rw-rw-   0 root         (0) root         (0)     2385 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/TOSTradierConverter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/models/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.526418 fast_tradier_client-1.0/fast_tradier/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/utils/OptionUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/utils/TimeUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/utils/YFinanceQuoteProvider.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/fast_tradier/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 02:11:48.530418 fast_tradier_client-1.0/fast_tradier_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11012 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-08 02:11:48.000000 fast_tradier_client-1.0/fast_tradier_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 02:11:48.530418 fast_tradier_client-1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-08 02:11:18.000000 fast_tradier_client-1.0/setup.py
```

### Comparing `fast_tradier_client-0.3.4/LICENSE` & `fast_tradier_client-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/PKG-INFO` & `fast_tradier_client-1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_tradier_client
-Version: 0.3.4
+Version: 1.0
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-0.3.4/README.md` & `fast_tradier_client-1.0/README.md`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/FastTradierAsyncClient.py` & `fast_tradier_client-1.0/fast_tradier/FastTradierAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/FastTradierClient.py` & `fast_tradier_client-1.0/fast_tradier/FastTradierClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/interfaces/IBrokerAsyncClient.py` & `fast_tradier_client-1.0/fast_tradier/interfaces/IBrokerAsyncClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/interfaces/IBrokerClient.py` & `fast_tradier_client-1.0/fast_tradier/interfaces/IBrokerClient.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/models/ModelBase.py` & `fast_tradier_client-1.0/fast_tradier/models/ModelBase.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from interface import implements
-from typing import Dict, Optional
+from typing import Dict, Optional, Mapping, Any
+from pydantic import BaseModel, ConfigDict
 
 from abc import abstractmethod
 import json
 import jsonpickle
 
 from fast_tradier.interfaces.IModel import IModel
 
@@ -34,8 +35,14 @@
     def serialize(self) -> Dict:
         '''serialize class object to json, which is parsable back to class object'''
         return jsonpickle.encode(self)
 
     @classmethod
     def deserialize_from_json(cls, json_obj) -> Optional[ModelBase]:
         '''Parse json object to class object. Could throw exception if not parsable'''
-        return jsonpickle.decode(json_obj)
+        return jsonpickle.decode(json_obj)
+
+class NewModelBase(BaseModel):
+    model_config = ConfigDict(use_enum_values=True)
+    
+    def to_json(self) -> Mapping[str, Any]:
+        return self.model_dump()
```

### Comparing `fast_tradier_client-0.3.4/fast_tradier/models/account/AccountBalance.py` & `fast_tradier_client-1.0/fast_tradier/models/account/AccountBalance.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/models/account/AccountOrder.py` & `fast_tradier_client-1.0/fast_tradier/models/account/AccountOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/models/market_data/Quote.py` & `fast_tradier_client-1.0/fast_tradier/models/market_data/Quote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/models/market_data/TradierQuote.py` & `fast_tradier_client-1.0/fast_tradier/models/market_data/TradierQuote.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/models/trading/EquityOrder.py` & `fast_tradier_client-1.0/fast_tradier/models/trading/EquityOrder.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/models/trading/TOSTradierConverter.py` & `fast_tradier_client-1.0/fast_tradier/models/trading/TOSTradierConverter.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/utils/OptionUtils.py` & `fast_tradier_client-1.0/fast_tradier/utils/OptionUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/utils/TimeUtils.py` & `fast_tradier_client-1.0/fast_tradier/utils/TimeUtils.py`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/fast_tradier/utils/YFinanceQuoteProvider.py` & `fast_tradier_client-1.0/fast_tradier/utils/YFinanceQuoteProvider.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def get_price(self, symbol: str) -> Optional[float]:
         try:
             url = self.__yfinance_base_url.format(symbol = YFinanceQuoteProvider.convert_to_yf_ticker(symbol))
             result = self.__scraper.get_result_similar(url)
             quote_price = None
             if result is not None and len(result) > 0:
-                quote_price = float(result[0].replace(',', ''))
+                quote_price = float(result[0])
             return quote_price
         except Exception as ex:
             return None
 
     @classmethod
     def convert_to_yf_ticker(cls, ticker: str):
         '''convert ticker/symbol to yahoo finance ticker'''
```

### Comparing `fast_tradier_client-0.3.4/fast_tradier_client.egg-info/PKG-INFO` & `fast_tradier_client-1.0/fast_tradier_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-tradier-client
-Version: 0.3.4
+Version: 1.0
 Summary: A Tradier client for trading stocks and options through Tradier API
 Home-page: https://pypi.org/project/fast-tradier-client/
 Author: Tony W
 Author-email: Tony Wang <ivytony@gmail.com>
 Project-URL: Homepage, https://bitbucket.org/rcholic/fast-tradier-client
 Project-URL: Bug Tracker, https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1
 Keywords: python,fast-tradier-client,tradier
```

### Comparing `fast_tradier_client-0.3.4/fast_tradier_client.egg-info/SOURCES.txt` & `fast_tradier_client-1.0/fast_tradier_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_tradier_client-0.3.4/pyproject.toml` & `fast_tradier_client-1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fast_tradier_client"
-version = "0.3.4"
+version = "1.0"
 authors = [
   { name="Tony Wang", email="ivytony@gmail.com" },
 ]
 description = "A Tradier client for trading stocks and options through Tradier API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -22,13 +22,14 @@
 "httpx",
 "arrow",
 "autoscraper",
 "pandas",
 "python-interface",
 "pytest",
 "pytest_httpx",
-"pytest-asyncio"
+"pytest-asyncio",
+"pydantic"
 ]
 
 [project.urls]
 "Homepage" = "https://bitbucket.org/rcholic/fast-tradier-client"
 "Bug Tracker" = "https://bitbucket.org/rcholic/fast-tradier-client/jira?statuses=new&statuses=indeterminate&sort=-updated&page=1"
```


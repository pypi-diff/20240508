# Comparing `tmp/pydolarvenezuela-1.5.4.tar.gz` & `tmp/pydolarvenezuela-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.5.4.tar", last modified: Sat May  4 08:13:53 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.5.5.tar", last modified: Wed May  8 05:25:45 2024, max compression
```

## Comparing `pydolarvenezuela-1.5.4.tar` & `pydolarvenezuela-1.5.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 08:13:53.271602 pydolarvenezuela-1.5.4/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.4/LICENSE
--rw-rw-rw-   0        0        0     7221 2024-05-04 08:13:53.266603 pydolarvenezuela-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     4830 2024-04-28 21:36:23.000000 pydolarvenezuela-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 08:13:53.078603 pydolarvenezuela-1.5.4/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2712 2024-05-04 08:09:53.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:13:53.118598 pydolarvenezuela-1.5.4/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:13:53.122602 pydolarvenezuela-1.5.4/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/assets/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:13:53.173600 pydolarvenezuela-1.5.4/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:13:53.187606 pydolarvenezuela-1.5.4/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:13:53.248602 pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     5234 2024-05-04 07:49:42.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2141 2024-04-28 15:44:15.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     1762 2024-04-29 16:09:28.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     2382 2024-05-04 07:56:14.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     1282 2024-05-04 08:02:51.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/italcambio.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:13:53.259600 pydolarvenezuela-1.5.4/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     2236 2024-04-28 11:49:26.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:13:53.264602 pydolarvenezuela-1.5.4/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7221 2024-05-04 08:13:52.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      897 2024-05-04 08:13:52.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 08:13:52.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-04 08:13:52.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-04 08:13:52.000000 pydolarvenezuela-1.5.4/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-05-04 08:09:45.000000 pydolarvenezuela-1.5.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 08:13:53.271602 pydolarvenezuela-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-05-04 08:09:49.000000 pydolarvenezuela-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.118536 pydolarvenezuela-1.5.5/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0     7221 2024-05-08 05:25:45.110580 pydolarvenezuela-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4830 2024-05-08 05:23:24.000000 pydolarvenezuela-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 05:25:44.915627 pydolarvenezuela-1.5.5/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2879 2024-05-08 05:22:33.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:25:44.950502 pydolarvenezuela-1.5.5/pyDolarVenezuela/assets/
+-rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:25:44.950502 pydolarvenezuela-1.5.5/pyDolarVenezuela/assets/icons/
+-rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/assets/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:25:44.998987 pydolarvenezuela-1.5.5/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.032525 pydolarvenezuela-1.5.5/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.082019 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     5345 2024-05-08 05:21:26.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2141 2024-04-28 15:44:15.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     1762 2024-04-29 16:09:28.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2382 2024-05-04 07:56:14.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1282 2024-05-04 08:02:51.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.102583 pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0     2236 2024-04-28 11:49:26.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:25:45.107586 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7221 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-08 05:25:44.000000 pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-05-08 05:22:42.000000 pydolarvenezuela-1.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 05:25:45.121532 pydolarvenezuela-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-05-08 05:22:38.000000 pydolarvenezuela-1.5.5/setup.py
```

### Comparing `pydolarvenezuela-1.5.4/LICENSE` & `pydolarvenezuela-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/PKG-INFO` & `pydolarvenezuela-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.4
+Version: 1.5.5
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.5.4/README.md` & `pydolarvenezuela-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import network
 from .models.pages import Page
 from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-version = '1.5.4'
+version = '1.5.5'
 """
 Versión actual de la biblioteca    
 """
 
 class CheckVersion:
     """
     Verificar actualización de la biblioteca    
@@ -45,14 +45,21 @@
         if not isinstance(provider, Page):
             raise TypeError("The parameter must be an object of type Monitor.")
         
         self.provider = provider
         self.currency = currency.lower()
         self.db       = db
     
+    def get_all_monitors(self):
+        return select_monitor(
+            self.provider,
+            db=self.db,
+            currency=self.currency
+        )
+
     def get_value_monitors(self, monitor_code: str = None, name_property: Literal['title', 'price', 'last_update'] = None, prettify: bool = False):
         """
         El método `get_value_monitors` permite acceder a los datos extraídos de los monitores.
 
         Parámetros:
         - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
         - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
```

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/assets/icons/__init__.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/assets/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,17 @@
         }
     }
 ]
 
 def select_monitor(provider: Page, db: Redis, **kwargs):
     global data
         
-    currency = kwargs.get('currency')
-    monitor_code = kwargs.get('monitor_code')
-    name_property = kwargs.get('name_property')
+    currency = kwargs.get('currency', None)
+    monitor_code = kwargs.get('monitor_code', None)
+    name_property = kwargs.get('name_property', None)
     prettify = kwargs.get('prettify', False)
 
     if currency not in currencies_list:
         raise ValueError(f"The currency type must be 'usd', 'eur'..., not {currency}")
 
     def _get_values_specifics():
         if not monitor_code:
@@ -114,17 +114,18 @@
 
                 existing_data_dict = json.loads(cache.get_data(key))
                 for name in existing_data_dict:
                     if not name == 'last_update' and not name == 'banks':
                         if name in existing_data_dict and name in data:
                             _update_item(existing_data_dict, name, data)
                     else:
-                        if name == 'banks' and name in data:
-                            for i in range(len(existing_data_dict[name])):
-                                _update_item(existing_data_dict[name], i, data[name])
+                        if name == 'banks':
+                            for i, bank in enumerate(existing_data_dict[name]):
+                                if i < len(data[name]) and bank['title'] == data[name][i]['title']:
+                                    _update_item(existing_data_dict[name], i, data[name])
                         elif name == 'last_update':
                             existing_data_dict[name] = data[name]
                             
                 cache.set_data(key, json.dumps(existing_data_dict), db.ttl)
                 data = json.loads(
                     cache.get_data(key)
                 )
```

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/provider/italcambio.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/provider/italcambio.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela/utils.py` & `pydolarvenezuela-1.5.5/pyDolarVenezuela/utils.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.4
+Version: 1.5.5
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
```

### Comparing `pydolarvenezuela-1.5.4/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.5.5/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.4/pyproject.toml` & `pydolarvenezuela-1.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.5.4"
+version = "1.5.5"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.5.4/setup.py` & `pydolarvenezuela-1.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.5.4'
+VERSION = '1.5.5'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```


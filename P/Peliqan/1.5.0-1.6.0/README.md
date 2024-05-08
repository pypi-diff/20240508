# Comparing `tmp/Peliqan-1.5.0.tar.gz` & `tmp/Peliqan-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-1.5.0.tar", last modified: Fri Apr  5 12:54:53 2024, max compression
+gzip compressed data, was "Peliqan-1.6.0.tar", last modified: Wed May  8 06:43:12 2024, max compression
```

## Comparing `Peliqan-1.5.0.tar` & `Peliqan-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-04-05 12:54:53.420385 Peliqan-1.5.0/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-04-05 12:54:53.420256 Peliqan-1.5.0/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-04-05 12:54:53.416301 Peliqan-1.5.0/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-04-05 12:54:53.000000 Peliqan-1.5.0/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.5.0/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-04-05 12:54:53.418156 Peliqan-1.5.0/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-04-05 12:21:53.000000 Peliqan-1.5.0/peliqan/__init__.py
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-04-05 12:54:53.419964 Peliqan-1.5.0/peliqan/client/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2023-11-07 06:42:14.000000 Peliqan-1.5.0/peliqan/client/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    15754 2024-04-05 12:21:53.000000 Peliqan-1.5.0/peliqan/client/backend_service.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     2657 2024-02-19 09:48:17.000000 Peliqan-1.5.0/peliqan/client/base.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    10609 2024-03-13 12:08:36.000000 Peliqan-1.5.0/peliqan/client/dbclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2023-09-12 06:13:12.000000 Peliqan-1.5.0/peliqan/client/sftpclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-04-05 12:21:53.000000 Peliqan-1.5.0/peliqan/client/writeback.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    26493 2024-04-05 12:21:53.000000 Peliqan-1.5.0/peliqan/core.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-02-16 11:30:10.000000 Peliqan-1.5.0/peliqan/exceptions.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.5.0/peliqan/local_test.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       23 2024-02-12 11:08:52.000000 Peliqan-1.5.0/peliqan/utils.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-04-05 12:54:53.420456 Peliqan-1.5.0/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-02-19 09:48:17.000000 Peliqan-1.5.0/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-08 06:43:12.826866 Peliqan-1.6.0/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-08 06:43:12.826574 Peliqan-1.6.0/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-08 06:43:12.818428 Peliqan-1.6.0/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-05-08 06:43:12.000000 Peliqan-1.6.0/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.6.0/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-08 06:43:12.822224 Peliqan-1.6.0/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-05-07 13:16:48.000000 Peliqan-1.6.0/peliqan/__init__.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-08 06:43:12.826061 Peliqan-1.6.0/peliqan/client/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2023-11-07 06:42:14.000000 Peliqan-1.6.0/peliqan/client/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    17466 2024-05-07 13:12:03.000000 Peliqan-1.6.0/peliqan/client/backend_service.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     2657 2024-04-22 06:47:06.000000 Peliqan-1.6.0/peliqan/client/base.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    10609 2024-04-23 09:30:50.000000 Peliqan-1.6.0/peliqan/client/dbclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2023-09-12 06:13:12.000000 Peliqan-1.6.0/peliqan/client/sftpclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-04-23 09:30:50.000000 Peliqan-1.6.0/peliqan/client/writeback.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    28999 2024-05-07 13:10:02.000000 Peliqan-1.6.0/peliqan/core.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-04-22 06:47:06.000000 Peliqan-1.6.0/peliqan/exceptions.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.6.0/peliqan/local_test.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       40 2024-05-07 09:05:00.000000 Peliqan-1.6.0/peliqan/utils.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-05-08 06:43:12.826951 Peliqan-1.6.0/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-04-22 06:47:06.000000 Peliqan-1.6.0/setup.py
```

### Comparing `Peliqan-1.5.0/PKG-INFO` & `Peliqan-1.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.5.0
+Version: 1.6.0
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.5.0/Peliqan.egg-info/PKG-INFO` & `Peliqan-1.6.0/Peliqan.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.5.0
+Version: 1.6.0
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.5.0/README.md` & `Peliqan-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `Peliqan-1.5.0/peliqan/__init__.py` & `Peliqan-1.6.0/peliqan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 __all__ = [
     "Peliqan",
     "BasePeliqanClient"
 ]
```

### Comparing `Peliqan-1.5.0/peliqan/client/backend_service.py` & `Peliqan-1.6.0/peliqan/client/backend_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from peliqan.exceptions import PeliqanClientException
 from peliqan.client import BaseClient
 
+from peliqan.utils import empty
+
 
 class BackendServiceClient(BaseClient):
     def __init__(self, jwt, backend_url):
         super(BackendServiceClient, self).__init__(jwt, backend_url)
         self._cache = {
             'connection': {},
             'database': {},
             'schema': {},
-            'table': {}
+            'table': {},
+            'interface': {}
         }
 
     def get_cached_results(self, resource_type, resource_id_or_name, property_name):
         try:
             resource_id_or_name = resource_id_or_name.lower()
         except AttributeError:
             pass
@@ -53,15 +56,14 @@
                     }
                 }
                 self._cache['database'].update(data_to_cache)
 
     def _cache_schema_data(self, data):
         schema_name = data.get('schema_name', '')
         if schema_name:
-            schema_name = schema_name.lower()
             schema_id = data['schema_id']
             if schema_id:
                 data_to_cache = {
                     schema_id: {
                         'schema_name': schema_name
                     },
                     schema_name: {
@@ -69,15 +71,14 @@
                     }
                 }
                 self._cache['schema'].update(data_to_cache)
 
     def _cache_table_and_field_data(self, data):
         table_name = data.get('table_name', '')
         if table_name:
-            table_name = table_name.lower()
             table_id = data['table_id']
             if table_id:
                 data_to_cache = {
                     table_name: {
                         'table_id': table_id,
                     },
                     table_id: {
@@ -90,19 +91,34 @@
                 field_name = data.get('field_name', '')
                 if field_name:
                     field_physical_name = data['field_physical_name']
                     if field_physical_name:
                         data_to_cache[table_name].update({field_name: field_physical_name})
                         data_to_cache[table_id].update({field_name: field_physical_name})
 
+    def _cache_interface_data(self, data):
+        interface_name = data.get('interface_name', '')
+        if interface_name:
+            interface_id = data['interface_id']
+            data_to_cache = {
+                interface_name: {
+                    'interface_id': interface_id,
+                },
+                interface_id: {
+                    'interface_name': interface_name
+                }
+            }
+            self._cache['interface'].update(data_to_cache)
+
     def _update_cache(self, data):
         self._cache_connection_data(data)
         self._cache_database_data(data)
         self._cache_schema_data(data)
         self._cache_table_and_field_data(data)
+        self._cache_interface_data(data)
 
     def find_connection(self, connection_id=None, connection_name=None):
         """
 
         :param connection_id:
         :param connection_name:
         :return:
@@ -190,60 +206,86 @@
         """
         url = f"{self.BACKEND_URL}/api/database/resource/lookup/table/"
         data = {
             'connection_id': connection_id,
             'connection_name': connection_name,
             'database_id': database_id,
             'database_name': database_name,
+            'schema_id': schema_id,
             'schema_name': schema_name,
             'table_id': table_id,
             'table_name': table_name,
             'field_id': field_id,
             'field_name': field_name
         }
         data = self.call_backend("get", url, json=data)
 
         self._update_cache(data)
         return data
 
+    def find_interface(self, interface_id=None, interface_name=None):
+        url = f"{self.BACKEND_URL}/api/resource/lookup/interface/"
+        data = {
+            'interface_id': interface_id,
+            'interface_name': interface_name
+        }
+        data = self.call_backend("get", url, json=data)
+
+        self._update_cache(data)
+        return data
+
     def find_resource(self, resource_type, resource_id=None, resource_name=None, **kwargs):
 
-        if resource_type not in ['connection', 'database', 'schema', 'table']:
-            raise PeliqanClientException(f"{resource_type} is not valid. "
-                                         f"Allowed resource types are 'connection', 'database', 'schema', 'table'.")
+        if resource_type not in ('connection', 'database', 'schema', 'table', 'interface'):
+            raise PeliqanClientException(
+                f"{resource_type} is not valid. "
+                "Allowed resource types are "
+                "'connection', 'database', 'schema', 'table', 'script'."
+            )
 
         if not resource_id and not resource_name:
             raise PeliqanClientException("resource_id or resource_name must be provided as kwargs.")
 
         if resource_type.lower() == 'connection':
             data = {
                 'connection_id': resource_id,
                 'connection_name': resource_name
             }
             # find connection
             return self.find_connection(**data)
+
         elif resource_type.lower() == 'database':
             data = {
                 'database_id': resource_id,
                 'database_name': resource_name,
             }
             # find database
             return self.find_database(**data, **kwargs)
+
         elif resource_type.lower() == 'schema':
             data = {
                 'schema_id': resource_id,
                 'schema_name': resource_name
             }
             return self.find_schema(**data, **kwargs)
+
         elif resource_type.lower() == 'table':
             data = {
                 'table_id': resource_id,
                 'table_name': resource_name
             }
             return self.find_table_or_field(**data, **kwargs)
+
+        elif resource_type.lower() == 'interface':
+            data = {
+                'interface_id': resource_id,
+                'interface_name': resource_name
+            }
+            return self.find_interface(**data)
+
         else:
             raise PeliqanClientException(f"{resource_type} is not valid. "
                                          f"Allowed resource types are 'connection', 'database', 'schema', 'table'.")
 
     def _is_refresh_allowed(self, resource_type):
         if resource_type not in ['connection', 'database', 'schema', 'table']:
             raise PeliqanClientException(f"{resource_type} is not valid. "
@@ -309,38 +351,31 @@
             "change_id": change_id,
             "writeback_status": writeback_status
         }
 
         response_dict = self.call_backend("patch", url, json=data)
         return response_dict
 
-    def get_databases(self):
+    def list_databases(self):
         url = f"{self.BACKEND_URL}/api/applications"
         response_dict = self.call_backend("get", url)
         return response_dict
 
     def get_table(self, table_id):
         url = f"{self.BACKEND_URL}/api/database/tables/{table_id}/"
         response_dict = self.call_backend("get", url)
         return response_dict
 
-    def update_table(self, id, name=None, table_type=None, query=None, external=None, primary_field_id=None,
-                     settings=None):
-        url = f"{self.BACKEND_URL}/api/database/tables/%s/" % id
+    def update_table(self, table_id, name=None, query=None, settings=None):
+        url = f"{self.BACKEND_URL}/api/database/tables/%s/" % table_id
         data = {}
         if name:
             data["name"] = name
-        if table_type:
-            data["table_type"] = table_type
         if query:
             data["query"] = query
-        if external:
-            data["external"] = external
-        if primary_field_id:
-            data["primary_field_id"] = primary_field_id
         if settings:
             data["settings"] = settings
         response_dict = self.call_backend("patch", url, json=data)
         return response_dict
 
     def update_database_metadata(self, id, description=None, tags=None):
         url = f"{self.BACKEND_URL}/api/applications/%s/data-catalog/" % id
@@ -348,38 +383,62 @@
         if description:
             data["description"] = description
         if tags:
             data["tags"] = tags
         response_dict = self.call_backend("patch", url, json=data)
         return response_dict
 
-    def update_table_metadata(self, id, description=None, tags=None):
-        url = f"{self.BACKEND_URL}/api/database/tables/%s/data-catalog/" % id
+    def update_table_metadata(self, table_id, description=None, tags=None, primary_field_id=None):
+        url = f"{self.BACKEND_URL}/api/database/tables/%s/details/" % table_id
         data = {}
         if description:
             data["description"] = description
         if tags:
             data["tags"] = tags
+
+        if primary_field_id:
+            data["primary_field_id"] = primary_field_id
         response_dict = self.call_backend("patch", url, json=data)
         return response_dict
 
-    def update_field_metadata(self, id, description=None, tags=None):
-        url = f"{self.BACKEND_URL}/api/database/fields/%s/data-catalog/" % id
+    def update_field_metadata(self, field_id, description=None, tags=None):
+        url = f"{self.BACKEND_URL}/api/database/fields/%s/data-catalog/" % field_id
         data = {}
         if description:
             data["description"] = description
         if tags:
             data["tags"] = tags
         response_dict = self.call_backend("patch", url, json=data)
         return response_dict
 
+    def list_interfaces(self):
+        url = f"{self.BACKEND_URL}/api/interfaces/"
+        response_dict = self.call_backend("get", url)
+        return response_dict
+
     def get_interface(self, interface_id):
         url = f"{self.BACKEND_URL}/api/interfaces/{interface_id}/"
         return self.call_backend("get", url)
 
+    def update_interface(
+        self,
+        interface_id,
+        **kwargs
+    ):
+        url = f"{self.BACKEND_URL}/api/interfaces/{interface_id}/"
+
+        data = {k: v for k, v in kwargs.items() if v is not empty}
+        return self.call_backend("patch", url, json=data)
+
+    def create_interface(self, group_id, **kwargs):
+        url = f"{self.BACKEND_URL}/api/interfaces/{group_id}/"
+
+        data = {k: v for k, v in kwargs.items() if v is not empty}
+        return self.call_backend("post", url, json=data)
+
     def get_interface_state(self, interface_id):
         data = self.get_interface(interface_id)
         return data.get('state', '')
 
     def set_interface_state(self, interface_id, state):
         url = f"{self.BACKEND_URL}/api/interfaces/{interface_id}/"
         data = {'state': state}
```

### Comparing `Peliqan-1.5.0/peliqan/client/base.py` & `Peliqan-1.6.0/peliqan/client/base.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.5.0/peliqan/client/dbclient.py` & `Peliqan-1.6.0/peliqan/client/dbclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.5.0/peliqan/client/sftpclient.py` & `Peliqan-1.6.0/peliqan/client/sftpclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.5.0/peliqan/client/writeback.py` & `Peliqan-1.6.0/peliqan/client/writeback.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.5.0/peliqan/core.py` & `Peliqan-1.6.0/peliqan/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # import necessary modules
 import logging
 import time
 
-import pandas as pd
-
 from peliqan.client import WritebackClient, BackendServiceClient, DBClient, SFTPClient, PeliqanTrinoDBClient
 from peliqan.exceptions import PeliqanClientException
-from peliqan.utils import Empty
+from peliqan.utils import empty
 
 # get logger
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 logger.propagate = False
 
 # get log handler
@@ -22,16 +20,14 @@
 
 # set format to log handler
 sh.setFormatter(formatter)
 
 # add handler to logger
 logger.addHandler(sh)
 
-empty = Empty()
-
 
 class BasePeliqanClient:
     """
     This base class wraps all operations we want to expose to our internal and external clients.
     """
 
     def __init__(self, jwt, backend_url):
@@ -413,106 +409,180 @@
 
     def list_databases(self):
         """
         Returns a list of all databases in the account including tables and fields in tables.
 
         :return: list of databases
         """
-        return self.__service_client__.get_databases()
+        return self.__service_client__.list_databases()
 
     def get_table(self, table_id):
         """
             Returns all meta-data for a table including fields.
 
             :return: list of databases
         """
         return self.__service_client__.get_table(table_id)
 
-    def update_field(self, id, description=None, tags=None):
+    def update_field(self, field_id, description=None, tags=None):
         """
         Updates a field (column).
 
-        :param id: required, integer, id of the field to update
+        :param field_id: required, integer, id of the field to update
         :param description: optional, string, description of the field (data catalog metadata)
         :param tags: optional, array of strings, tags assigned to the field (data catalog metadata)
         :return: result of update
         """
 
-        return self.__service_client__.update_field_metadata(id, description, tags)
+        return self.__service_client__.update_field_metadata(field_id, description, tags)
 
-    def update_table(self, id, name=None, table_type=None, query=None, external=None, primary_field_id=None,
+    def update_table(self, table_id, name=None, query=None, primary_field_id=None,
                      settings=None,
                      description=None, tags=None):
         """
         Updates a table.
 
-        :param id: required, integer, id of the table to update
+        :param table_id: required, integer, id of the table to update
         :param name: optional, string, new name of the table
-        :param table_type: optional, string, new type of the table, e.g. 'query'
         :param query: optional, string, new SQL query for tables of type 'query'
-        :param external: optional, boolean, true for external tables, false for internal tables
         :param primary_field_id: optional, integer, primary key field id for this table, i.e. the field id in Peliqan.
         See, table details page in Peliqan to get the primary_field_id for a table.
         :param settings: optional, string (json), settings of the table
         :param description: optional, string, description of the table (data catalog metadata)
         :param tags: optional, array of strings, tags assigned to the table (data catalog metadata)
         :return: result of update
         """
 
         update_result_dict = {}
         update_metadata_result_dict = {}
-        if name or table_type or query or external or primary_field_id or settings:
-            update_result_dict = self.__service_client__.update_table(id, name, table_type, query, external,
-                                                                      primary_field_id, settings)
-        if description or tags:
-            update_metadata_result_dict = self.__service_client__.update_table_metadata(id, description, tags)
+        if name or query or settings:
+            update_result_dict = self.__service_client__.update_table(table_id, name, query, settings)
+        if description or tags or primary_field_id:
+            update_metadata_result_dict = self.__service_client__.update_table_metadata(
+                table_id,
+                description,
+                tags,
+                primary_field_id
+            )
         return {**update_result_dict, **update_metadata_result_dict}
 
-    def update_database(self, id, description=None, tags=None):
+    def update_database(self, database_id, description=None, tags=None):
         """
         Updates a database.
 
-        :param id: required, integer, id of the database to update
+        :param database_id: required, integer, id of the database to update
         :param description: optional, string, description of the database (data catalog metadata)
         :param tags: optional, array of strings, tags assigned to the database (data catalog metadata)
         :return: result of update
         """
 
-        return self.__service_client__.update_database_metadata(id, description, tags)
+        return self.__service_client__.update_database_metadata(database_id, description, tags)
+
+    def list_scripts(self):
+        return self.__service_client__.list_interfaces()
+
+    def get_script(self, script_id=None, script_name=None):
+        if not script_id and not script_name:
+            raise PeliqanClientException("'script_id' or 'script_name' must be provided")
+
+        if not script_id and script_name:
+            script_id = self.__service_client__.get_cached_results('interface', script_name, 'interface_id')
+
+        if not script_id:
+            interface_data = self.__service_client__.find_resource('interface', resource_name=script_name)
+            script_id = interface_data['interface_id']
+
+        return self.__service_client__.get_interface(script_id)
+
+    def update_script(
+        self,
+        script_id,
+        name=empty,
+        group=empty,
+        raw_script=empty,
+        settings=empty,
+        state=empty,
+        flow=empty,
+        editor=empty
+    ):
+        """
+        A function to update a script in Peliqan.
+
+        :param script_id: The id of the script that needs to be updated.
+        :param name: A string value that represents the new name of the script.
+        :param group: The new group id that the script should belong to.
+        :param raw_script: The python code that should be associated with this script.
+        :param settings: Update the script run schedule settings.
+        :param state: Update the state of the script.
+        :param flow: The json settings associated with the visual flow editor.
+        :param editor: An enum value that decides which editor type must be opened in the Peliqan code editor.
+        Options: [RAW_SCRIPT_EDITOR, FLOW_EDITOR]
+        :return:
+        """
+        return self.__service_client__.update_interface(
+            script_id,
+            name=name,
+            group=group,
+            raw_script=raw_script,
+            settings=settings,
+            state=state,
+            flow=flow,
+            editor=editor
+        )
+
+    def add_script(self, group_id, name=empty, script_type=empty, run_mode=empty):
+        """
+
+        :param group_id: The group the script will belong to.
+        :param name: The name of the new script.
+        :param script_type: An enum value that decides the type of script. Options: [streamlit]
+        :param run_mode:  An enum value that decides whether the script will be triggered by an API or a streamlit app.
+        Options: [STREAMLIT, API]
+        :return:
+        """
+        return self.__service_client__.create_interface(
+            group_id,
+            name=name,
+            type=script_type,
+            run_mode=run_mode
+        )
 
     def generate_sql_union(self, table_ids, sources=None):
         """
         Generates an SQL UNION query for the given tables.
         All columns of all tables will be added to the UNION query.
         If a column does not exist in one of the tables, it will be added with a null value.
         Optionally, a "source" column can be added to indicate from which table each row originated.
 
         :param table_ids: required, list of integers, list of table ids to include in UNION query
         :param sources: optional, dict, if set an extra 'source' column will be added to indicate to which table the record belongs. Keys are table ids. Values are source value to include in UNION result. Example: { 1: "Paris", 2: "London" }. This will add a column "source" to the UNION where all records from table id 1 will have value "Paris" for the source.
         :return: result of update
         """
-        databases = self.__service_client__.get_databases()
+        databases = self.__service_client__.list_databases()
         tables = []
         fields = []
         field_types = {}
         fields_to_cast = []
         for database in databases:
             for table in database["tables"]:
                 if table["id"] in table_ids:
                     tables.append(table)
                     for field in table["all_fields"]:
                         if field["name"] not in fields:
                             fields.append(field["name"])
                             if field["sql_data_type"]:
-                                field_types[field["name"]] = field[
-                                    "sql_data_type"]  # Actual field type in source, e.g. timestamp, timestamptz... (might not be available for all sources)
+                                # Actual field type in source, e.g. timestamp, timestamptz...
+                                # (might not be available for all sources)
+                                field_types[field["name"]] = field["sql_data_type"]
                             else:
-                                field_types[field["name"]] = field["type"]  # Peliqan field type, e.g. "date"
-                        elif (field["sql_data_type"] and field["sql_data_type"] != field_types[field["name"]]) or field[
-                            "type"] != field_types[field["name"]]:
+                                # Peliqan field type, e.g. "date"
+                                field_types[field["name"]] = field["type"]
+                        elif (
+                            field["sql_data_type"] and field["sql_data_type"] != field_types[field["name"]]
+                        ) or field["type"] != field_types[field["name"]]:
                             fields_to_cast.append(field["name"])
 
         table_selects = []
         for table in tables:
             table_select_fields = []
             if sources:
                 source_name = ""
@@ -528,15 +598,16 @@
                         field[0] != '"' and table_field["name"].lower() == field.lower()
                     ):
                         table_has_field = True
                         break
                 if table_has_field:
                     if field in fields_to_cast:
                         if table_field["sql_data_type"] and table_field["sql_data_type"] == "timestamptz":
-                            # Postgres fields of type timestamptz (timestamp with timezone) cannot be cast to varchar directly by Trino
+                            # Postgres fields of type timestamptz (timestamp with timezone)
+                            # cannot be cast to varchar directly by Trino
                             table_select_fields.append("CAST(CAST(%s AS TIMESTAMP) AS VARCHAR) AS %s" % (field, field))
                         else:
                             table_select_fields.append("CAST(%s AS VARCHAR) AS %s" % (field, field))
                     else:
                         table_select_fields.append(field)
                 else:
                     table_select_fields.append("null " + field)
```

### Comparing `Peliqan-1.5.0/peliqan/local_test.py` & `Peliqan-1.6.0/peliqan/local_test.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.5.0/setup.py` & `Peliqan-1.6.0/setup.py`

 * *Files identical despite different names*


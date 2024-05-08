# Comparing `tmp/tmticket-0.2.1.tar.gz` & `tmp/tmticket-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.1.tar", last modified: Tue May  7 23:57:31 2024, max compression
+gzip compressed data, was "tmticket-0.2.2.tar", last modified: Wed May  8 00:06:29 2024, max compression
```

## Comparing `tmticket-0.2.1.tar` & `tmticket-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:57:31.558385 tmticket-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 22:01:04.000000 tmticket-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 23:57:31.558385 tmticket-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 22:01:04.000000 tmticket-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 23:57:31.558385 tmticket-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      968 2024-05-07 23:57:07.000000 tmticket-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:57:31.555385 tmticket-0.2.1/tmticket/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-07 23:51:23.000000 tmticket-0.2.1/tmticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5702 2024-05-07 23:51:23.000000 tmticket-0.2.1/tmticket/client.py
--rw-r--r--   0 root         (0) root         (0)    13241 2024-05-07 23:51:23.000000 tmticket-0.2.1/tmticket/model.py
--rw-r--r--   0 root         (0) root         (0)     4620 2024-05-07 23:51:23.000000 tmticket-0.2.1/tmticket/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:57:31.557385 tmticket-0.2.1/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 23:57:30.000000 tmticket-0.2.1/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2024-05-07 23:57:31.000000 tmticket-0.2.1/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 23:57:30.000000 tmticket-0.2.1/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 23:57:30.000000 tmticket-0.2.1/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 23:57:30.000000 tmticket-0.2.1/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.254469 tmticket-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 22:01:04.000000 tmticket-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:29.253469 tmticket-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 22:01:04.000000 tmticket-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 00:06:29.254469 tmticket-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      968 2024-05-08 00:06:04.000000 tmticket-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.250469 tmticket-0.2.2/tmticket/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5702 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/client.py
+-rw-r--r--   0 root         (0) root         (0)    13241 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/model.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.252469 tmticket-0.2.2/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-08 00:06:29.000000 tmticket-0.2.2/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.1/LICENSE` & `tmticket-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.1/PKG-INFO` & `tmticket-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmticket
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python wrapper for the Ticketmaster Discovery API
 Home-page: https://github.com/hokiebrian/pytmtickets
 Author: hokiebrian
 Author-email: hokiebrian@gmail.com
 License: MIT
 Keywords: Ticketmaster API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tmticket-0.2.1/setup.py` & `tmticket-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='tmticket',
-    version='0.2.1',
+    version='0.2.2',
     author='hokiebrian',
     author_email='hokiebrian@gmail.com',
     description="Python wrapper for the Ticketmaster Discovery API",
     #long_description=read('README.rst'), 
     license='MIT',
     keywords='Ticketmaster API',
     url='https://github.com/hokiebrian/pytmtickets',
```

### Comparing `tmticket-0.2.1/tmticket/client.py` & `tmticket-0.2.2/tmticket/client.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.1/tmticket/model.py` & `tmticket-0.2.2/tmticket/model.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.2.1/tmticket/query.py` & `tmticket-0.2.2/tmticket/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,38 +35,38 @@
     }
 
     def __init__(self, api_client, method, model):
         self.api_client = api_client
         self.method = method
         self.model = model
 
-    async def __get(self, session, **kwargs):
-        """Asynchronously sends a request to `ApiClient` using an existing session."""
-        url = f"{self.api_client.url}/{self.method}"
-        async with session.get(url, params={**self.api_client.api_key, **kwargs}) as response:
-            return await response.json()
+    async def __get(self, **kwargs):
+        """Asynchronously sends final request to `ApiClient`"""
+        async with aiohttp.ClientSession() as session:
+            async with session.get(f"{self.api_client.url}/{self.method}", params={**self.api_client.api_key, **kwargs}) as response:
+                return await response.json()
 
-    async def _get(self, session, keyword=None, entity_id=None, sort=None, include_test=None, page=None, size=None, locale=None, **kwargs):
+    async def _get(self, keyword=None, entity_id=None, sort=None, include_test=None, page=None, size=None, locale=None, **kwargs):
         """Asynchronously handles basic API search request"""
         search_args = {
             'keyword': keyword,
             'id': entity_id,
             'sort': sort,
             'include_test': include_test,
             'page': page,
             'size': size,
             'locale': locale,
             **kwargs
         }
         params = self._search_params(**search_args)
-        return await self.__get(session, **params)
+        return await self.__get(**params)
 
-    async def by_id(self, session, entity_id):
+    async def by_id(self, entity_id):
         """Asynchronously get a specific object by its ID"""
-        return await self._get(session, entity_id=entity_id)
+        return await self._get(entity_id=entity_id)
 
     def _search_params(self, **kwargs):
         """Maps parameter names to API-friendly parameters"""
         kw_map = {}
         for k, v in kwargs.items():
             api_key = self.attr_map.get(k)
             if api_key:
@@ -75,16 +75,16 @@
                 kw_map[k] = v
         return {k: v for k, v in kw_map.items() if v is not None}
 
 class AttractionQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'attractions', Attraction)
 
-    async def find(self, session, **kwargs):
-        return await self._get(session, **kwargs)
+    async def find(self, **kwargs):
+        return await self._get(**kwargs)
 
 class ClassificationQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'classifications', Classification)
 
 
     def segment_by_id(self, segment_id):
@@ -112,23 +112,23 @@
             ]
             for subg in subgenres:
                 if subg.id == subgenre_id:
                     subgenre = subg
         return subgenre
 
 
-    async def find(self, session, **kwargs):
-        return await self._get(session, **kwargs)
+    async def find(self, **kwargs):
+        return await self._get(**kwargs)
 
 class EventQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'events', Event)
 
-    async def find(self, session, **kwargs):
-        return await self._get(session, **kwargs)
+    async def find(self, **kwargs):
+        return await self._get(**kwargs)
 
 class VenueQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'venues', Venue)
 
-    async def find(self, session, **kwargs):
-        return await self._get(session, **kwargs)
+    async def find(self, **kwargs):
+        return await self._get(**kwargs)
```

### Comparing `tmticket-0.2.1/tmticket.egg-info/PKG-INFO` & `tmticket-0.2.2/tmticket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmticket
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python wrapper for the Ticketmaster Discovery API
 Home-page: https://github.com/hokiebrian/pytmtickets
 Author: hokiebrian
 Author-email: hokiebrian@gmail.com
 License: MIT
 Keywords: Ticketmaster API
 Classifier: Development Status :: 4 - Beta
```


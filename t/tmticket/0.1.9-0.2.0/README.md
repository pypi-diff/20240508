# Comparing `tmp/tmticket-0.1.9.tar.gz` & `tmp/tmticket-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.1.9.tar", last modified: Tue May  7 21:33:48 2024, max compression
+gzip compressed data, was "tmticket-0.2.0.tar", last modified: Tue May  7 23:52:13 2024, max compression
```

## Comparing `tmticket-0.1.9.tar` & `tmticket-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:33:48.474200 tmticket-0.1.9/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 21:33:12.000000 tmticket-0.1.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 21:33:48.474200 tmticket-0.1.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 21:33:12.000000 tmticket-0.1.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 21:33:48.474200 tmticket-0.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      968 2024-05-07 21:33:12.000000 tmticket-0.1.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:33:48.471201 tmticket-0.1.9/tmticket/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-07 21:33:12.000000 tmticket-0.1.9/tmticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5530 2024-05-07 21:33:12.000000 tmticket-0.1.9/tmticket/client.py
--rw-r--r--   0 root         (0) root         (0)    13241 2024-05-07 21:33:12.000000 tmticket-0.1.9/tmticket/model.py
--rw-r--r--   0 root         (0) root         (0)     4525 2024-05-07 21:33:12.000000 tmticket-0.1.9/tmticket/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:33:48.473200 tmticket-0.1.9/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 21:33:47.000000 tmticket-0.1.9/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2024-05-07 21:33:48.000000 tmticket-0.1.9/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 21:33:47.000000 tmticket-0.1.9/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 21:33:47.000000 tmticket-0.1.9/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 21:33:47.000000 tmticket-0.1.9/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:52:13.253806 tmticket-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 22:01:04.000000 tmticket-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 23:52:13.252806 tmticket-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 22:01:04.000000 tmticket-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 23:52:13.253806 tmticket-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      968 2024-05-07 23:51:23.000000 tmticket-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:52:13.250806 tmticket-0.2.0/tmticket/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-07 23:51:23.000000 tmticket-0.2.0/tmticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5702 2024-05-07 23:51:23.000000 tmticket-0.2.0/tmticket/client.py
+-rw-r--r--   0 root         (0) root         (0)    13241 2024-05-07 23:51:23.000000 tmticket-0.2.0/tmticket/model.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2024-05-07 23:51:23.000000 tmticket-0.2.0/tmticket/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 23:52:13.252806 tmticket-0.2.0/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 23:52:12.000000 tmticket-0.2.0/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-07 23:52:13.000000 tmticket-0.2.0/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 23:52:12.000000 tmticket-0.2.0/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 23:52:12.000000 tmticket-0.2.0/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 23:52:12.000000 tmticket-0.2.0/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.1.9/LICENSE` & `tmticket-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.9/PKG-INFO` & `tmticket-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmticket
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python wrapper for the Ticketmaster Discovery API
 Home-page: https://github.com/hokiebrian/pytmtickets
 Author: hokiebrian
 Author-email: hokiebrian@gmail.com
 License: MIT
 Keywords: Ticketmaster API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tmticket-0.1.9/setup.py` & `tmticket-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='tmticket',
-    version='0.1.9',
+    version='0.2.0',
     author='hokiebrian',
     author_email='hokiebrian@gmail.com',
     description="Python wrapper for the Ticketmaster Discovery API",
     #long_description=read('README.rst'), 
     license='MIT',
     keywords='Ticketmaster API',
     url='https://github.com/hokiebrian/pytmtickets',
```

### Comparing `tmticket-0.1.9/tmticket/client.py` & `tmticket-0.2.0/tmticket/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,63 +14,67 @@
 sf = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 sh.setFormatter(sf)
 log.addHandler(sh)
 
 
 class AsyncApiClient:
     """AsyncApiClient is the main wrapper for the Discovery API, updated for asynchronous operation.
-
+    
     Example:    
     Get the first page result for venues matching keyword 'Tabernacle':
     
     ```
-    import tmticket
+    import ticketpy
     import asyncio
     
     async def main():
-        client = tmticket.AsyncApiClient("your_api_key")
+        client = ticketpy.AsyncApiClient("your_api_key")
         resp = await client.venues.find(keyword="Tabernacle").one()
         for venue in resp:
             print(venue.name)
     if __name__ == "__main__":
         asyncio.run(main())
     ```
     """
     root_url = 'https://app.ticketmaster.com'
     url = 'https://app.ticketmaster.com/discovery/v2'
 
     def __init__(self, api_key):
-        self.__api_key = {'apikey': api_key}
-        self.session = aiohttp.ClientSession()
+        self.__api_key = None
+        self.api_key = api_key
         self.events = EventQuery(api_client=self)
         self.venues = VenueQuery(api_client=self)
         self.attractions = AttractionQuery(api_client=self)
         self.classifications = ClassificationQuery(api_client=self)
-        # Direct access shortcuts
         self.segment_by_id = self.classifications.segment_by_id
         self.genre_by_id = self.classifications.genre_by_id
         self.subgenre_by_id = self.classifications.subgenre_by_id
 
-    async def close(self):
-        await self.session.close()
-
     async def search(self, method, **kwargs):
         """Generic API request, converted for asynchronous operation"""
-        params = {k: v for k, v in kwargs.items() if v is not None}
-        params.update(self.__api_key)
+        kwargs = {k: v for (k, v) in kwargs.items() if v is not None}
+        updates = self.api_key
 
-        for k, v in params.items():
+        for k, v in kwargs.items():
             if k in ['includeTBA', 'includeTBD', 'includeTest']:
-                params[k] = self.__yes_no_only(v)
+                updates[k] = self.__yes_no_only(v)
             elif k in ['size', 'radius', 'marketId']:
-                params[k] = str(v)
+                updates[k] = str(v)
+        kwargs.update(updates)
 
-        url = self.__method_url(method)
-        async with self.session.get(url, params=params) as resp:
-            return await self._handle_response(resp)
+        urls = {
+            'events': self.__method_url('events'),
+            'venues': self.__method_url('venues'),
+            'attractions': self.__method_url('attractions'),
+            'classifications': self.__method_url('classifications')
+        }
+
+        async with aiohttp.ClientSession() as session:
+            async with session.get(urls[method], params=kwargs) as resp:
+                return await self._handle_response(resp)
 
     async def _handle_response(self, response):
         """Handles response, raising ApiException if needed or returning response JSON object asynchronously"""
         if response.status == 200:
             return await response.json()
         elif response.status == 401:
             self.__fault(await response.json())
@@ -78,39 +82,39 @@
             self.__error(await response.json())
         else:
             self.__unknown_error(await response.json())
 
     async def get_url(self, link):
         """Gets a specific href from '_links' object in a response, asynchronously"""
         parsed_link = self._parse_link(link)
-        async with self.session.get(parsed_link.url, params=parsed_link.params) as resp:
-            return Page.from_json(await self._handle_response(resp))
+        async with aiohttp.ClientSession() as session:
+            async with session.get(parsed_link.url, params=parsed_link.params) as resp:
+                return Page.from_json(await self._handle_response(resp))
+
+    @property
+    def api_key(self):
+        return self.__api_key
+
+    @api_key.setter
+    def api_key(self, api_key):
+        self.__api_key = {'apikey': api_key}
 
     @staticmethod
     def __method_url(method):
-        return f"{AsyncApiClient.url}/{method}.json"
+        return "{}/{}.json".format(AsyncApiClient.url, method)
 
     @staticmethod
     def __yes_no_only(s):
         s = str(s).lower()
         if s in ['true', 'yes']:
             s = 'yes'
         elif s in ['false', 'no']:
             s = 'no'
         return s
 
-    def __fault(self, data):
-        raise ApiException('Unauthorized access', data)
-
-    def __error(self, data):
-        raise ApiException('Bad request', data)
-
-    def __unknown_error(self, data):
-        raise ApiException('Unknown error', data)
-
 
 class ApiException(Exception):
     """Exception thrown for API-related error messages"""
     def __init__(self, *args):
         super().__init__(*args)
 
 class AsyncPagedResponse:
```

### Comparing `tmticket-0.1.9/tmticket/model.py` & `tmticket-0.2.0/tmticket/model.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.9/tmticket/query.py` & `tmticket-0.2.0/tmticket/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,38 +35,38 @@
     }
 
     def __init__(self, api_client, method, model):
         self.api_client = api_client
         self.method = method
         self.model = model
 
-    async def __get(self, **kwargs):
-        """Asynchronously sends final request to `ApiClient`"""
-        async with aiohttp.ClientSession() as session:
-            async with session.get(f"{self.api_client.url}/{self.method}", params={**self.api_client.api_key, **kwargs}) as response:
-                return await response.json()
+    async def __get(self, session, **kwargs):
+        """Asynchronously sends a request to `ApiClient` using an existing session."""
+        url = f"{self.api_client.url}/{self.method}"
+        async with session.get(url, params={**self.api_client.api_key, **kwargs}) as response:
+            return await response.json()
 
-    async def _get(self, keyword=None, entity_id=None, sort=None, include_test=None, page=None, size=None, locale=None, **kwargs):
+    async def _get(self, session, keyword=None, entity_id=None, sort=None, include_test=None, page=None, size=None, locale=None, **kwargs):
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
-        return await self.__get(**params)
+        return await self.__get(session, **params)
 
-    async def by_id(self, entity_id):
+    async def by_id(self, session, entity_id):
         """Asynchronously get a specific object by its ID"""
-        return await self._get(entity_id=entity_id)
+        return await self._get(session, entity_id=entity_id)
 
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
 
-    async def find(self, **kwargs):
-        return await self._get(**kwargs)
+    async def find(self, session, **kwargs):
+        return await self._get(session, **kwargs)
 
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
 
 
-    async def find(self, **kwargs):
-        return await self._get(**kwargs)
+    async def find(self, session, **kwargs):
+        return await self._get(session, **kwargs)
 
 class EventQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'events', Event)
 
-    async def find(self, **kwargs):
-        return await self._get(**kwargs)
+    async def find(self, session, **kwargs):
+        return await self._get(session, **kwargs)
 
 class VenueQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'venues', Venue)
 
-    async def find(self, **kwargs):
-        return await self._get(**kwargs)
+    async def find(self, session, **kwargs):
+        return await self._get(session, **kwargs)
```

### Comparing `tmticket-0.1.9/tmticket.egg-info/PKG-INFO` & `tmticket-0.2.0/tmticket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmticket
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python wrapper for the Ticketmaster Discovery API
 Home-page: https://github.com/hokiebrian/pytmtickets
 Author: hokiebrian
 Author-email: hokiebrian@gmail.com
 License: MIT
 Keywords: Ticketmaster API
 Classifier: Development Status :: 4 - Beta
```


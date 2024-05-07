# Comparing `tmp/tmticket-0.1.8.tar.gz` & `tmp/tmticket-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.1.8.tar", last modified: Tue May  7 21:09:18 2024, max compression
+gzip compressed data, was "tmticket-0.1.9.tar", last modified: Tue May  7 21:33:48 2024, max compression
```

## Comparing `tmticket-0.1.8.tar` & `tmticket-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:09:18.404718 tmticket-0.1.8/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 21:08:23.000000 tmticket-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 21:09:18.403718 tmticket-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 21:08:23.000000 tmticket-0.1.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 21:09:18.404718 tmticket-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      968 2024-05-07 21:08:23.000000 tmticket-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:09:18.401718 tmticket-0.1.8/tmticket/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-07 21:08:23.000000 tmticket-0.1.8/tmticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5702 2024-05-07 21:08:23.000000 tmticket-0.1.8/tmticket/client.py
--rw-r--r--   0 root         (0) root         (0)    13241 2024-05-07 21:08:23.000000 tmticket-0.1.8/tmticket/model.py
--rw-r--r--   0 root         (0) root         (0)     4525 2024-05-07 21:08:23.000000 tmticket-0.1.8/tmticket/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:09:18.403718 tmticket-0.1.8/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 21:09:17.000000 tmticket-0.1.8/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2024-05-07 21:09:18.000000 tmticket-0.1.8/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 21:09:17.000000 tmticket-0.1.8/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 21:09:17.000000 tmticket-0.1.8/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 21:09:17.000000 tmticket-0.1.8/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:33:48.474200 tmticket-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 21:33:12.000000 tmticket-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 21:33:48.474200 tmticket-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 21:33:12.000000 tmticket-0.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 21:33:48.474200 tmticket-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      968 2024-05-07 21:33:12.000000 tmticket-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:33:48.471201 tmticket-0.1.9/tmticket/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-07 21:33:12.000000 tmticket-0.1.9/tmticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2024-05-07 21:33:12.000000 tmticket-0.1.9/tmticket/client.py
+-rw-r--r--   0 root         (0) root         (0)    13241 2024-05-07 21:33:12.000000 tmticket-0.1.9/tmticket/model.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2024-05-07 21:33:12.000000 tmticket-0.1.9/tmticket/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 21:33:48.473200 tmticket-0.1.9/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-07 21:33:47.000000 tmticket-0.1.9/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-07 21:33:48.000000 tmticket-0.1.9/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 21:33:47.000000 tmticket-0.1.9/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 21:33:47.000000 tmticket-0.1.9/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-07 21:33:47.000000 tmticket-0.1.9/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.1.8/LICENSE` & `tmticket-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.8/PKG-INFO` & `tmticket-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmticket
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python wrapper for the Ticketmaster Discovery API
 Home-page: https://github.com/hokiebrian/pytmtickets
 Author: hokiebrian
 Author-email: hokiebrian@gmail.com
 License: MIT
 Keywords: Ticketmaster API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tmticket-0.1.8/setup.py` & `tmticket-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='tmticket',
-    version='0.1.8',
+    version='0.1.9',
     author='hokiebrian',
     author_email='hokiebrian@gmail.com',
     description="Python wrapper for the Ticketmaster Discovery API",
     #long_description=read('README.rst'), 
     license='MIT',
     keywords='Ticketmaster API',
     url='https://github.com/hokiebrian/pytmtickets',
```

### Comparing `tmticket-0.1.8/tmticket/client.py` & `tmticket-0.1.9/tmticket/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,67 +14,63 @@
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
-    import ticketpy
+    import tmticket
     import asyncio
     
     async def main():
-        client = ticketpy.AsyncApiClient("your_api_key")
+        client = tmticket.AsyncApiClient("your_api_key")
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
-        self.__api_key = None
-        self.api_key = api_key
+        self.__api_key = {'apikey': api_key}
+        self.session = aiohttp.ClientSession()
         self.events = EventQuery(api_client=self)
         self.venues = VenueQuery(api_client=self)
         self.attractions = AttractionQuery(api_client=self)
         self.classifications = ClassificationQuery(api_client=self)
+        # Direct access shortcuts
         self.segment_by_id = self.classifications.segment_by_id
         self.genre_by_id = self.classifications.genre_by_id
         self.subgenre_by_id = self.classifications.subgenre_by_id
 
+    async def close(self):
+        await self.session.close()
+
     async def search(self, method, **kwargs):
         """Generic API request, converted for asynchronous operation"""
-        kwargs = {k: v for (k, v) in kwargs.items() if v is not None}
-        updates = self.api_key
+        params = {k: v for k, v in kwargs.items() if v is not None}
+        params.update(self.__api_key)
 
-        for k, v in kwargs.items():
+        for k, v in params.items():
             if k in ['includeTBA', 'includeTBD', 'includeTest']:
-                updates[k] = self.__yes_no_only(v)
+                params[k] = self.__yes_no_only(v)
             elif k in ['size', 'radius', 'marketId']:
-                updates[k] = str(v)
-        kwargs.update(updates)
+                params[k] = str(v)
 
-        urls = {
-            'events': self.__method_url('events'),
-            'venues': self.__method_url('venues'),
-            'attractions': self.__method_url('attractions'),
-            'classifications': self.__method_url('classifications')
-        }
-
-        async with aiohttp.ClientSession() as session:
-            async with session.get(urls[method], params=kwargs) as resp:
-                return await self._handle_response(resp)
+        url = self.__method_url(method)
+        async with self.session.get(url, params=params) as resp:
+            return await self._handle_response(resp)
 
     async def _handle_response(self, response):
         """Handles response, raising ApiException if needed or returning response JSON object asynchronously"""
         if response.status == 200:
             return await response.json()
         elif response.status == 401:
             self.__fault(await response.json())
@@ -82,39 +78,39 @@
             self.__error(await response.json())
         else:
             self.__unknown_error(await response.json())
 
     async def get_url(self, link):
         """Gets a specific href from '_links' object in a response, asynchronously"""
         parsed_link = self._parse_link(link)
-        async with aiohttp.ClientSession() as session:
-            async with session.get(parsed_link.url, params=parsed_link.params) as resp:
-                return Page.from_json(await self._handle_response(resp))
-
-    @property
-    def api_key(self):
-        return self.__api_key
-
-    @api_key.setter
-    def api_key(self, api_key):
-        self.__api_key = {'apikey': api_key}
+        async with self.session.get(parsed_link.url, params=parsed_link.params) as resp:
+            return Page.from_json(await self._handle_response(resp))
 
     @staticmethod
     def __method_url(method):
-        return "{}/{}.json".format(AsyncApiClient.url, method)
+        return f"{AsyncApiClient.url}/{method}.json"
 
     @staticmethod
     def __yes_no_only(s):
         s = str(s).lower()
         if s in ['true', 'yes']:
             s = 'yes'
         elif s in ['false', 'no']:
             s = 'no'
         return s
 
+    def __fault(self, data):
+        raise ApiException('Unauthorized access', data)
+
+    def __error(self, data):
+        raise ApiException('Bad request', data)
+
+    def __unknown_error(self, data):
+        raise ApiException('Unknown error', data)
+
 
 class ApiException(Exception):
     """Exception thrown for API-related error messages"""
     def __init__(self, *args):
         super().__init__(*args)
 
 class AsyncPagedResponse:
```

### Comparing `tmticket-0.1.8/tmticket/model.py` & `tmticket-0.1.9/tmticket/model.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.8/tmticket/query.py` & `tmticket-0.1.9/tmticket/query.py`

 * *Files identical despite different names*

### Comparing `tmticket-0.1.8/tmticket.egg-info/PKG-INFO` & `tmticket-0.1.9/tmticket.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmticket
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python wrapper for the Ticketmaster Discovery API
 Home-page: https://github.com/hokiebrian/pytmtickets
 Author: hokiebrian
 Author-email: hokiebrian@gmail.com
 License: MIT
 Keywords: Ticketmaster API
 Classifier: Development Status :: 4 - Beta
```


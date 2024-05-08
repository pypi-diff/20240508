# Comparing `tmp/kellyapi-0.0.2.3.tar.gz` & `tmp/kellyapi-0.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kellyapi-0.0.2.3.tar", last modified: Sun May  5 16:39:30 2024, max compression
+gzip compressed data, was "kellyapi-0.0.2.4.tar", last modified: Wed May  8 04:36:26 2024, max compression
```

## Comparing `kellyapi-0.0.2.3.tar` & `kellyapi-0.0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/kellyapi/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/kellyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/kellyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/kellyapi/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/kellyapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 16:39:30.000000 kellyapi-0.0.2.3/kellyapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 16:39:30.384714 kellyapi-0.0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-05 16:39:26.000000 kellyapi-0.0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:36:26.688343 kellyapi-0.0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-08 04:36:21.000000 kellyapi-0.0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-08 04:36:26.688343 kellyapi-0.0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-08 04:36:21.000000 kellyapi-0.0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:36:26.688343 kellyapi-0.0.2.4/kellyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 04:36:21.000000 kellyapi-0.0.2.4/kellyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-05-08 04:36:21.000000 kellyapi-0.0.2.4/kellyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-08 04:36:21.000000 kellyapi-0.0.2.4/kellyapi/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 04:36:26.688343 kellyapi-0.0.2.4/kellyapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-08 04:36:26.000000 kellyapi-0.0.2.4/kellyapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-08 04:36:26.000000 kellyapi-0.0.2.4/kellyapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 04:36:26.000000 kellyapi-0.0.2.4/kellyapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 04:36:26.000000 kellyapi-0.0.2.4/kellyapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 04:36:26.000000 kellyapi-0.0.2.4/kellyapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 04:36:26.688343 kellyapi-0.0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-08 04:36:21.000000 kellyapi-0.0.2.4/setup.py
```

### Comparing `kellyapi-0.0.2.3/LICENSE` & `kellyapi-0.0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.2.3/PKG-INFO` & `kellyapi-0.0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.2.3/README.md` & `kellyapi-0.0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.2.3/kellyapi/api.py` & `kellyapi-0.0.2.4/kellyapi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     async def _post_json(self, route, data=None, timeout=60):
         try:
             async with self.session() as client:
                 resp = await client.post(
                     self.api + route,
                     json=data,
-                    headers={"Kelly-API-KEY": f"Bearer {self.api_key}"},
+                    headers={"Authorization": f"Bearer {self.api_key}"},
                     timeout=timeout,
                 )
                 if resp.status in (401, 403):
                     raise InvalidApiKey(
                         "Invalid API key, Get an api key from @KellyAIBot"
                     )
                 if resp.status == 502:
@@ -70,15 +70,14 @@
         except asyncio.TimeoutError:
             raise TimeoutError
         except ContentTypeError:
             raise InvalidContent
         except ClientConnectorError:
             raise ConnectionError
         return self._parse_result(response)
-    
 
     async def sd_models(self):
         content = await self._fetch("sd/models")
         return content
 
     async def sdxl_models(self):
         content = await self._fetch("sdxl/models")
@@ -94,15 +93,15 @@
     ):
         kwargs = dict(
             prompt=prompt,
             negative_prompt=negative_prompt,
             model=model,
             width=width,
             height=height,
-            responseType="base64data"
+            responseType="base64data",
         )
         content = await self._post_json("image/generate", data=kwargs)
         image_data = base64.b64decode(content.image)
         return image_data
 
     async def img2img(
         self,
@@ -114,15 +113,15 @@
     ):
         kwargs = dict(
             prompt=prompt,
             negative_prompt=negative_prompt,
             image_data=image_data,
             width=width,
             height=height,
-            responseType="base64data"
+            responseType="base64data",
         )
         content = await self._post_json("image/edit", data=kwargs)
         image_data = base64.b64decode(content.image)
         return image_data
 
     async def img2text(
         self,
@@ -178,8 +177,8 @@
         image_data = base64.b64decode(content.image)
         return image_data
 
     async def code2image(self, text: str):
         kwargs = dict(code=text, responseType="base64data")
         content = await self._post_json("write/code", data=kwargs)
         image_data = base64.b64decode(content.image)
-        return image_data
+        return image_data
```

### Comparing `kellyapi-0.0.2.3/kellyapi/errors.py` & `kellyapi-0.0.2.4/kellyapi/errors.py`

 * *Files identical despite different names*

### Comparing `kellyapi-0.0.2.3/kellyapi.egg-info/PKG-INFO` & `kellyapi-0.0.2.4/kellyapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kellyapi
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/NotReallyPrince/Prince-Api
 Author: NotReallyPrince
 Author-email: princebots3011@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/NotReallyPrince/Kelly-API/issues
 Project-URL: Community, https://t.me/PrincexUpdates
```

### Comparing `kellyapi-0.0.2.3/setup.py` & `kellyapi-0.0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="kellyapi",
     packages=setuptools.find_packages(),
-    version="0.0.2.3",
+    version="0.0.2.4",
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="NotReallyPrince",
     author_email="princebots3011@gmail.com",
     url="https://github.com/NotReallyPrince/Prince-Api",
```


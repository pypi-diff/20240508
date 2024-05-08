# Comparing `tmp/blueshed_gust-0.0.6.tar.gz` & `tmp/blueshed_gust-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueshed_gust-0.0.6.tar", last modified: Mon May  6 16:57:30 2024, max compression
+gzip compressed data, was "blueshed_gust-0.0.7.tar", last modified: Wed May  8 06:51:49 2024, max compression
```

## Comparing `blueshed_gust-0.0.6.tar` & `blueshed_gust-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:57:30.057122 blueshed_gust-0.0.6/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 16:57:30.056943 blueshed_gust-0.0.6/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.6/README.md
--rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-06 16:57:27.000000 blueshed_gust-0.0.6/pyproject.toml
--rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-06 16:57:30.057160 blueshed_gust-0.0.6/setup.cfg
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:57:30.054449 blueshed_gust-0.0.6/src/
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:57:30.054390 blueshed_gust-0.0.6/src/blueshed/
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:57:30.055817 blueshed_gust-0.0.6/src/blueshed/gust/
--rw-r--r--   0 peterb     (501) staff       (20)      145 2024-05-06 16:57:27.000000 blueshed_gust-0.0.6/src/blueshed/gust/__init__.py
--rw-r--r--   0 peterb     (501) staff       (20)      754 2024-05-06 10:00:21.000000 blueshed_gust-0.0.6/src/blueshed/gust/configs.py
--rw-r--r--   0 peterb     (501) staff       (20)      590 2024-05-06 10:00:21.000000 blueshed_gust-0.0.6/src/blueshed/gust/context.py
--rw-r--r--   0 peterb     (501) staff       (20)     1416 2024-05-06 10:00:21.000000 blueshed_gust-0.0.6/src/blueshed/gust/json_utils.py
--rw-r--r--   0 peterb     (501) staff       (20)     2541 2024-05-06 16:57:06.000000 blueshed_gust-0.0.6/src/blueshed/gust/main.py
--rw-r--r--   0 peterb     (501) staff       (20)     3829 2024-05-06 14:08:50.000000 blueshed_gust-0.0.6/src/blueshed/gust/routes.py
--rw-r--r--   0 peterb     (501) staff       (20)      919 2024-05-06 10:00:21.000000 blueshed_gust-0.0.6/src/blueshed/gust/static_file_handler.py
--rw-r--r--   0 peterb     (501) staff       (20)     2599 2024-05-06 13:33:43.000000 blueshed_gust-0.0.6/src/blueshed/gust/utils.py
--rw-r--r--   0 peterb     (501) staff       (20)       67 2024-05-06 13:33:43.000000 blueshed_gust-0.0.6/src/blueshed/gust/web.py
--rw-r--r--   0 peterb     (501) staff       (20)     2263 2024-05-06 10:00:21.000000 blueshed_gust-0.0.6/src/blueshed/gust/web_handler.py
--rw-r--r--   0 peterb     (501) staff       (20)     5670 2024-05-06 10:28:00.000000 blueshed_gust-0.0.6/src/blueshed/gust/websocket.py
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:57:30.056466 blueshed_gust-0.0.6/src/blueshed_gust.egg-info/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 16:57:30.000000 blueshed_gust-0.0.6/src/blueshed_gust.egg-info/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      559 2024-05-06 16:57:30.000000 blueshed_gust-0.0.6/src/blueshed_gust.egg-info/SOURCES.txt
--rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-06 16:57:30.000000 blueshed_gust-0.0.6/src/blueshed_gust.egg-info/dependency_links.txt
--rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-06 16:57:30.000000 blueshed_gust-0.0.6/src/blueshed_gust.egg-info/requires.txt
--rw-r--r--   0 peterb     (501) staff       (20)        9 2024-05-06 16:57:30.000000 blueshed_gust-0.0.6/src/blueshed_gust.egg-info/top_level.txt
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 06:51:49.874765 blueshed_gust-0.0.7/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-08 06:51:49.874573 blueshed_gust-0.0.7/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.7/README.md
+-rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-08 06:51:45.000000 blueshed_gust-0.0.7/pyproject.toml
+-rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-08 06:51:49.874800 blueshed_gust-0.0.7/setup.cfg
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 06:51:49.872048 blueshed_gust-0.0.7/src/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 06:51:49.871986 blueshed_gust-0.0.7/src/blueshed/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 06:51:49.873405 blueshed_gust-0.0.7/src/blueshed/gust/
+-rw-r--r--   0 peterb     (501) staff       (20)      145 2024-05-08 06:51:45.000000 blueshed_gust-0.0.7/src/blueshed/gust/__init__.py
+-rw-r--r--   0 peterb     (501) staff       (20)      754 2024-05-06 10:00:21.000000 blueshed_gust-0.0.7/src/blueshed/gust/configs.py
+-rw-r--r--   0 peterb     (501) staff       (20)      801 2024-05-07 21:45:19.000000 blueshed_gust-0.0.7/src/blueshed/gust/context.py
+-rw-r--r--   0 peterb     (501) staff       (20)     1416 2024-05-06 10:00:21.000000 blueshed_gust-0.0.7/src/blueshed/gust/json_utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2586 2024-05-07 21:46:56.000000 blueshed_gust-0.0.7/src/blueshed/gust/main.py
+-rw-r--r--   0 peterb     (501) staff       (20)     3829 2024-05-06 14:08:50.000000 blueshed_gust-0.0.7/src/blueshed/gust/routes.py
+-rw-r--r--   0 peterb     (501) staff       (20)      919 2024-05-06 10:00:21.000000 blueshed_gust-0.0.7/src/blueshed/gust/static_file_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2599 2024-05-06 13:33:43.000000 blueshed_gust-0.0.7/src/blueshed/gust/utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)       67 2024-05-06 13:33:43.000000 blueshed_gust-0.0.7/src/blueshed/gust/web.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2269 2024-05-07 21:46:04.000000 blueshed_gust-0.0.7/src/blueshed/gust/web_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     5676 2024-05-07 21:46:16.000000 blueshed_gust-0.0.7/src/blueshed/gust/websocket.py
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-08 06:51:49.874067 blueshed_gust-0.0.7/src/blueshed_gust.egg-info/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-08 06:51:49.000000 blueshed_gust-0.0.7/src/blueshed_gust.egg-info/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      559 2024-05-08 06:51:49.000000 blueshed_gust-0.0.7/src/blueshed_gust.egg-info/SOURCES.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-08 06:51:49.000000 blueshed_gust-0.0.7/src/blueshed_gust.egg-info/dependency_links.txt
+-rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-08 06:51:49.000000 blueshed_gust-0.0.7/src/blueshed_gust.egg-info/requires.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        9 2024-05-08 06:51:49.000000 blueshed_gust-0.0.7/src/blueshed_gust.egg-info/top_level.txt
```

### Comparing `blueshed_gust-0.0.6/PKG-INFO` & `blueshed_gust-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.6
+Version: 0.0.7
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `blueshed_gust-0.0.6/pyproject.toml` & `blueshed_gust-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,14 @@
 
 [tool.coverage.run]
 data_file = ".venv/cache/.coverage"
 [tool.coverage.report]
 data_file = ".venv/cache/.coverage"
 
 [tool.bumpversion]
-current_version = "0.0.6"
+current_version = "0.0.7"
 commit = false
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "src/blueshed/gust/__init__.py"
```

### Comparing `blueshed_gust-0.0.6/src/blueshed/gust/configs.py` & `blueshed_gust-0.0.7/src/blueshed/gust/configs.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.6/src/blueshed/gust/context.py` & `blueshed_gust-0.0.7/src/blueshed/gust/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """when functions are called we set up a context"""
 
 import contextlib
 import contextvars
 
 GUST = contextvars.ContextVar('_gust_GUST')
 USER = contextvars.ContextVar('_gust_USER')
+HANDLER = contextvars.ContextVar('_gust_HANDLER')
 
 
 @contextlib.contextmanager
-def gust(app, user):
+def gust(app, user, handler=None):
     """With this we setup contextvars and reset for our app"""
     token = GUST.set(app)
     utoken = USER.set(user)
+    htoken = HANDLER.set(handler)
     try:
         yield
     finally:
         GUST.reset(token)
         USER.reset(utoken)
+        HANDLER.reset(htoken)
 
 
 def get_app():
     """get the context app"""
     return GUST.get(None)
 
 
+def get_handler():
+    """get the current handler"""
+    return HANDLER.get(None)
+
 def get_current_user():
     """get the context app"""
     return USER.get(None)
```

### Comparing `blueshed_gust-0.0.6/src/blueshed/gust/json_utils.py` & `blueshed_gust-0.0.7/src/blueshed/gust/json_utils.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.6/src/blueshed/gust/main.py` & `blueshed_gust-0.0.7/src/blueshed/gust/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,31 +33,31 @@
         **kwargs,
     ):
         self.port = port if port else os.getenv('PORT', options.port)
         debug = debug if debug is not None else options.debug
         super().__init__(routes, debug=debug, **kwargs)
         web.install(self)
 
-    async def perform(self, user, func: Callable, *args, **kwargs) -> Any:
+    async def perform(self, handler, user, func: Callable, *args, **kwargs) -> Any:
         """await a function or call in a thread_pool, better yet call redis"""
         if inspect.iscoroutinefunction(func):
             log.debug('aperform: %s', func)
-            with context.gust(self, user):
+            with context.gust(self, user, handler):
                 result = await func(*args, **kwargs)
         else:
             log.debug('perform: %s', func)
             partial = functools.partial(
-                self.call_in_context, user, func, args, kwargs
+                self.call_in_context, user, handler, func, args, kwargs
             )
             result = await asyncio.to_thread(partial)
         return result
 
-    def call_in_context(self, user, func, args, kwargs):
+    def call_in_context(self, user, handler, func, args, kwargs):
         """set the context and call function"""
-        with context.gust(self, user):
+        with context.gust(self, user, handler):
             return func(*args, **kwargs)
 
     @classmethod
     def broadcast(cls, path, message, client_ids):
         """pass through, maybe point for redis gust"""
         Websocket.broadcast(path, message, client_ids)
```

### Comparing `blueshed_gust-0.0.6/src/blueshed/gust/routes.py` & `blueshed_gust-0.0.7/src/blueshed/gust/routes.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.6/src/blueshed/gust/static_file_handler.py` & `blueshed_gust-0.0.7/src/blueshed/gust/static_file_handler.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.6/src/blueshed/gust/utils.py` & `blueshed_gust-0.0.7/src/blueshed/gust/utils.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.6/src/blueshed/gust/web_handler.py` & `blueshed_gust-0.0.7/src/blueshed/gust/web_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         template, auth = settings.template, settings.auth
         if auth and self.current_user is None:
             self.not_authenticated()
 
         try:
             result = await self.application.perform(
-                self.current_user, settings.func, self
+                self, self.current_user, settings.func, self
             )
             log.debug('http outcome: %s', result)
         except Redirect as ex:
             self.redirect(ex.url)
             return
         except Exception as ex:
             log.exception(settings.func)
```

### Comparing `blueshed_gust-0.0.6/src/blueshed/gust/websocket.py` & `blueshed_gust-0.0.7/src/blueshed/gust/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             args = [self]
             kwargs = {'message': data} if data else {}
 
         if error is None:
             try:
                 log.debug('calling: %s %r, %r', handling, args, kwargs)
                 result = await self.application.perform(
-                    self.current_user, handling, *args, **kwargs
+                    self, self.current_user, handling, *args, **kwargs
                 )
                 if ref:
                     log.debug('have result: %s', result)
             except Exception as ex:  # pylint: disable=W0703
                 log.exception('%s: %r', method, data)
                 error = ex
             finally:
```

### Comparing `blueshed_gust-0.0.6/src/blueshed_gust.egg-info/PKG-INFO` & `blueshed_gust-0.0.7/src/blueshed_gust.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.6
+Version: 0.0.7
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `blueshed_gust-0.0.6/src/blueshed_gust.egg-info/SOURCES.txt` & `blueshed_gust-0.0.7/src/blueshed_gust.egg-info/SOURCES.txt`

 * *Files identical despite different names*


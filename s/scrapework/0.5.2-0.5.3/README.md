# Comparing `tmp/scrapework-0.5.2.tar.gz` & `tmp/scrapework-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapework-0.5.2.tar", max compression
+gzip compressed data, was "scrapework-0.5.3.tar", max compression
```

## Comparing `scrapework-0.5.2.tar` & `scrapework-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4204 2024-04-27 05:21:50.089646 scrapework-0.5.2/README.md
--rw-r--r--   0        0        0      897 2024-04-27 05:22:02.201630 scrapework-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/__init__.py
--rw-r--r--   0        0        0     2265 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/cache.py
--rw-r--r--   0        0        0        0 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/core/__init__.py
--rw-r--r--   0        0        0      506 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/core/collector.py
--rw-r--r--   0        0        0      567 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/core/context.py
--rw-r--r--   0        0        0      424 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/core/http_client.py
--rw-r--r--   0        0        0      873 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/core/logger.py
--rw-r--r--   0        0        0     2435 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/handlers.py
--rw-r--r--   0        0        0     3729 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/items.py
--rw-r--r--   0        0        0     2979 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/middleware.py
--rw-r--r--   0        0        0      221 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/module.py
--rw-r--r--   0        0        0      194 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/monitors.py
--rw-r--r--   0        0        0      862 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/observer.py
--rw-r--r--   0        0        0      979 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/parsers.py
--rw-r--r--   0        0        0      546 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/processors.py
--rw-r--r--   0        0        0     3258 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/reporter.py
--rw-r--r--   0        0        0     4638 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/request.py
--rw-r--r--   0        0        0     5901 2024-04-27 05:21:50.089646 scrapework-0.5.2/scrapework/scraper.py
--rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 scrapework-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     4204 2024-05-08 02:16:20.273519 scrapework-0.5.3/README.md
+-rw-r--r--   0        0        0      897 2024-05-08 02:16:31.117632 scrapework-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/__init__.py
+-rw-r--r--   0        0        0     2265 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/cache.py
+-rw-r--r--   0        0        0        0 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/__init__.py
+-rw-r--r--   0        0        0      506 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/collector.py
+-rw-r--r--   0        0        0      567 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/context.py
+-rw-r--r--   0        0        0      424 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/http_client.py
+-rw-r--r--   0        0        0      873 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/logger.py
+-rw-r--r--   0        0        0     2435 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/handlers.py
+-rw-r--r--   0        0        0     3729 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/items.py
+-rw-r--r--   0        0        0     2979 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/middleware.py
+-rw-r--r--   0        0        0      222 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/module.py
+-rw-r--r--   0        0        0      194 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/monitors.py
+-rw-r--r--   0        0        0      862 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/observer.py
+-rw-r--r--   0        0        0      979 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/parsers.py
+-rw-r--r--   0        0        0      547 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/processors.py
+-rw-r--r--   0        0        0     3258 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/reporter.py
+-rw-r--r--   0        0        0     4638 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/request.py
+-rw-r--r--   0        0        0     5951 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/scraper.py
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 scrapework-0.5.3/PKG-INFO
```

### Comparing `scrapework-0.5.2/README.md` & `scrapework-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/pyproject.toml` & `scrapework-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapework"
-version = "v0.5.2"
+version = "v0.5.3"
 description = "simple scraping framework"
 authors = ["Stéphane Busso <stephane.busso@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sbusso/scrapework"
 homepage = "https://github.com/sbusso/scrapework"
```

### Comparing `scrapework-0.5.2/scrapework/cache.py` & `scrapework-0.5.3/scrapework/cache.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/core/context.py` & `scrapework-0.5.3/scrapework/core/context.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/core/logger.py` & `scrapework-0.5.3/scrapework/core/logger.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/handlers.py` & `scrapework-0.5.3/scrapework/handlers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/items.py` & `scrapework-0.5.3/scrapework/items.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/middleware.py` & `scrapework-0.5.3/scrapework/middleware.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/observer.py` & `scrapework-0.5.3/scrapework/observer.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/parsers.py` & `scrapework-0.5.3/scrapework/parsers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/processors.py` & `scrapework-0.5.3/scrapework/processors.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Args:
         ABC (_type_): _description_
     """
 
     def __init__(self) -> None:
         self.logger = Logger().get_logger()
-        self.logger.info(f"Using processor: {self.__class__.__name__}")
+        self.logger.debug(f"Using processor: {self.__class__.__name__}")
 
     @abstractmethod
     def process_items(
         self,
         items: Union[Dict[str, Any], Iterable[Dict[str, Any]]],
     ):
         pass
```

### Comparing `scrapework-0.5.2/scrapework/reporter.py` & `scrapework-0.5.3/scrapework/reporter.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/request.py` & `scrapework-0.5.3/scrapework/request.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.2/scrapework/scraper.py` & `scrapework-0.5.3/scrapework/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,19 +140,20 @@
 
             self.visited_urls.append(url_with_callback.url)
 
             new_items = url_with_callback.extract(ctx, Selector(response.text))
 
             # TODO: self.process(ctx, new_items)
 
-            # append new_items to items, Items can be a list or a dict
-            if isinstance(new_items, dict):
-                items.append(new_items)
-            else:
-                items += new_items
+            # append new_items to items, Items can be a list or a dict or None
+            if new_items:
+                if isinstance(new_items, dict):
+                    items.append(new_items)
+                else:
+                    items += new_items
 
             iter_end_time = datetime.datetime.now()
             items_count = len(items)
             ctx.collector.set("items_count", items_count)
             ctx.collector.jobs.append(
                 JobCollector(
                     url=url_with_callback.url,
```

### Comparing `scrapework-0.5.2/PKG-INFO` & `scrapework-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapework
-Version: 0.5.2
+Version: 0.5.3
 Summary: simple scraping framework
 Home-page: https://github.com/sbusso/scrapework
 License: MIT
 Author: Stéphane Busso
 Author-email: stephane.busso@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


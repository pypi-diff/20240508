# Comparing `tmp/scrapework-0.5.3.tar.gz` & `tmp/scrapework-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapework-0.5.3.tar", max compression
+gzip compressed data, was "scrapework-0.5.4.tar", max compression
```

## Comparing `scrapework-0.5.3.tar` & `scrapework-0.5.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4204 2024-05-08 02:16:20.273519 scrapework-0.5.3/README.md
--rw-r--r--   0        0        0      897 2024-05-08 02:16:31.117632 scrapework-0.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/__init__.py
--rw-r--r--   0        0        0     2265 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/cache.py
--rw-r--r--   0        0        0        0 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/__init__.py
--rw-r--r--   0        0        0      506 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/collector.py
--rw-r--r--   0        0        0      567 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/context.py
--rw-r--r--   0        0        0      424 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/http_client.py
--rw-r--r--   0        0        0      873 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/core/logger.py
--rw-r--r--   0        0        0     2435 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/handlers.py
--rw-r--r--   0        0        0     3729 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/items.py
--rw-r--r--   0        0        0     2979 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/middleware.py
--rw-r--r--   0        0        0      222 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/module.py
--rw-r--r--   0        0        0      194 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/monitors.py
--rw-r--r--   0        0        0      862 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/observer.py
--rw-r--r--   0        0        0      979 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/parsers.py
--rw-r--r--   0        0        0      547 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/processors.py
--rw-r--r--   0        0        0     3258 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/reporter.py
--rw-r--r--   0        0        0     4638 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/request.py
--rw-r--r--   0        0        0     5951 2024-05-08 02:16:20.277520 scrapework-0.5.3/scrapework/scraper.py
--rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 scrapework-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     4204 2024-05-08 02:24:55.338067 scrapework-0.5.4/README.md
+-rw-r--r--   0        0        0      897 2024-05-08 02:25:05.638050 scrapework-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/__init__.py
+-rw-r--r--   0        0        0     2265 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/cache.py
+-rw-r--r--   0        0        0        0 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/core/__init__.py
+-rw-r--r--   0        0        0      506 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/core/collector.py
+-rw-r--r--   0        0        0      567 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/core/context.py
+-rw-r--r--   0        0        0      424 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/core/http_client.py
+-rw-r--r--   0        0        0      873 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/core/logger.py
+-rw-r--r--   0        0        0     2435 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/handlers.py
+-rw-r--r--   0        0        0     3729 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/items.py
+-rw-r--r--   0        0        0     2979 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/middleware.py
+-rw-r--r--   0        0        0      222 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/module.py
+-rw-r--r--   0        0        0      194 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/monitors.py
+-rw-r--r--   0        0        0      862 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/observer.py
+-rw-r--r--   0        0        0      979 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/parsers.py
+-rw-r--r--   0        0        0      547 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/processors.py
+-rw-r--r--   0        0        0     3258 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/reporter.py
+-rw-r--r--   0        0        0     4638 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/request.py
+-rw-r--r--   0        0        0     5951 2024-05-08 02:24:55.338067 scrapework-0.5.4/scrapework/scraper.py
+-rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 scrapework-0.5.4/PKG-INFO
```

### Comparing `scrapework-0.5.3/README.md` & `scrapework-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/pyproject.toml` & `scrapework-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapework"
-version = "v0.5.3"
+version = "v0.5.4"
 description = "simple scraping framework"
 authors = ["Stéphane Busso <stephane.busso@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sbusso/scrapework"
 homepage = "https://github.com/sbusso/scrapework"
```

### Comparing `scrapework-0.5.3/scrapework/cache.py` & `scrapework-0.5.4/scrapework/cache.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/core/context.py` & `scrapework-0.5.4/scrapework/core/context.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/core/logger.py` & `scrapework-0.5.4/scrapework/core/logger.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/handlers.py` & `scrapework-0.5.4/scrapework/handlers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/items.py` & `scrapework-0.5.4/scrapework/items.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/middleware.py` & `scrapework-0.5.4/scrapework/middleware.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/observer.py` & `scrapework-0.5.4/scrapework/observer.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/parsers.py` & `scrapework-0.5.4/scrapework/parsers.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/processors.py` & `scrapework-0.5.4/scrapework/processors.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/reporter.py` & `scrapework-0.5.4/scrapework/reporter.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/request.py` & `scrapework-0.5.4/scrapework/request.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/scrapework/scraper.py` & `scrapework-0.5.4/scrapework/scraper.py`

 * *Files identical despite different names*

### Comparing `scrapework-0.5.3/PKG-INFO` & `scrapework-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapework
-Version: 0.5.3
+Version: 0.5.4
 Summary: simple scraping framework
 Home-page: https://github.com/sbusso/scrapework
 License: MIT
 Author: Stéphane Busso
 Author-email: stephane.busso@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


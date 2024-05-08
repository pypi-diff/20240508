# Comparing `tmp/scrapy-playwright-full-0.0.3403.tar.gz` & `tmp/scrapy_playwright_full-0.0.3404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-playwright-full-0.0.3403.tar", last modified: Sat Apr  6 22:05:53 2024, max compression
+gzip compressed data, was "scrapy_playwright_full-0.0.3404.tar", last modified: Wed May  8 11:23:23 2024, max compression
```

## Comparing `scrapy-playwright-full-0.0.3403.tar` & `scrapy_playwright_full-0.0.3404.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:05:53.853783 scrapy-playwright-full-0.0.3403/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-04-06 22:05:53.853783 scrapy-playwright-full-0.0.3403/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34512 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:05:53.853783 scrapy-playwright-full-0.0.3403/scrapy_playwright/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33276 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright/memusage.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:05:53.853783 scrapy-playwright-full-0.0.3403/scrapy_playwright_full.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-04-06 22:05:53.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright_full.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-06 22:05:53.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright_full.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 22:05:53.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright_full.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 22:05:53.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright_full.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 22:05:53.000000 scrapy-playwright-full-0.0.3403/scrapy_playwright_full.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 22:05:53.853783 scrapy-playwright-full-0.0.3403/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-06 22:05:45.000000 scrapy-playwright-full-0.0.3403/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:23:23.482540 scrapy_playwright_full-0.0.3404/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-05-08 11:23:23.482540 scrapy_playwright_full-0.0.3404/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34512 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:23:23.482540 scrapy_playwright_full-0.0.3404/scrapy_playwright/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33276 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:23:23.482540 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 11:23:23.000000 scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 11:23:23.486540 scrapy_playwright_full-0.0.3404/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-08 11:23:12.000000 scrapy_playwright_full-0.0.3404/setup.py
```

### Comparing `scrapy-playwright-full-0.0.3403/LICENSE` & `scrapy_playwright_full-0.0.3404/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3403/PKG-INFO` & `scrapy_playwright_full-0.0.3404/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright-full
-Version: 0.0.3403
+Version: 0.0.3404
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy-playwright-full-0.0.3403/README.md` & `scrapy_playwright_full-0.0.3404/README.md`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3403/scrapy_playwright/_utils.py` & `scrapy_playwright_full-0.0.3404/scrapy_playwright/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ) -> str:
     """Wrapper around Page.content to retry if necessary.
     Arguments other than the page are only for logging.
     """
     try:
         return await page.content()
     except Error as err:
-        if err.message == _NAVIGATION_ERROR_MSG:
+        if _NAVIGATION_ERROR_MSG in err.message:
             logger.debug(
                 "Retrying to get content from page '%s', error: '%s'",
                 page.url,
                 _NAVIGATION_ERROR_MSG,
                 extra={
                     "spider": spider,
                     "context_name": context_name,
```

### Comparing `scrapy-playwright-full-0.0.3403/scrapy_playwright/handler.py` & `scrapy_playwright_full-0.0.3404/scrapy_playwright/handler.py`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3403/scrapy_playwright/headers.py` & `scrapy_playwright_full-0.0.3404/scrapy_playwright/headers.py`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3403/scrapy_playwright/memusage.py` & `scrapy_playwright_full-0.0.3404/scrapy_playwright/memusage.py`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3403/scrapy_playwright/page.py` & `scrapy_playwright_full-0.0.3404/scrapy_playwright/page.py`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3403/scrapy_playwright_full.egg-info/PKG-INFO` & `scrapy_playwright_full-0.0.3404/scrapy_playwright_full.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright-full
-Version: 0.0.3403
+Version: 0.0.3404
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy-playwright-full-0.0.3403/setup.py` & `scrapy_playwright_full-0.0.3404/setup.py`

 * *Files identical despite different names*


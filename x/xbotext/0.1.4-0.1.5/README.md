# Comparing `tmp/xbotext-0.1.4.tar.gz` & `tmp/xbotext-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbotext-0.1.4.tar", max compression
+gzip compressed data, was "xbotext-0.1.5.tar", max compression
```

## Comparing `xbotext-0.1.4.tar` & `xbotext-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       25 2024-05-07 12:19:53.414568 xbotext-0.1.4/README.md
--rw-r--r--   0        0        0      255 2024-05-07 12:25:04.258412 xbotext-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.4/xbotext/__init__.py
--rw-r--r--   0        0        0     3336 2024-05-07 12:12:34.225851 xbotext-0.1.4/xbotext/cache.py
--rw-r--r--   0        0        0      522 2024-05-07 11:55:00.763736 xbotext-0.1.4/xbotext/chromium.py
--rw-r--r--   0        0        0       76 2024-05-07 12:23:09.391571 xbotext-0.1.4/xbotext/client.py
--rw-r--r--   0        0        0      605 2024-05-07 11:55:00.763736 xbotext-0.1.4/xbotext/regedit.py
--rw-r--r--   0        0        0       20 2024-05-07 11:55:00.763736 xbotext-0.1.4/xbotext/sofaware.py
--rw-r--r--   0        0        0      101 2024-05-07 11:55:00.763736 xbotext-0.1.4/xbotext/system.py
--rw-r--r--   0        0        0      538 2024-05-07 12:24:54.194157 xbotext-0.1.4/xbotext/web.py
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 xbotext-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-05-07 12:19:53.414568 xbotext-0.1.5/README.md
+-rw-r--r--   0        0        0      255 2024-05-08 01:39:51.923335 xbotext-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-05-08 01:39:44.563338 xbotext-0.1.5/xbotext/__init__.py
+-rw-r--r--   0        0        0     3336 2024-05-07 12:12:34.225851 xbotext-0.1.5/xbotext/cache.py
+-rw-r--r--   0        0        0      522 2024-05-07 11:55:00.763736 xbotext-0.1.5/xbotext/chromium.py
+-rw-r--r--   0        0        0       76 2024-05-07 12:23:09.391571 xbotext-0.1.5/xbotext/client.py
+-rw-r--r--   0        0        0      605 2024-05-07 11:55:00.763736 xbotext-0.1.5/xbotext/regedit.py
+-rw-r--r--   0        0        0       20 2024-05-07 11:55:00.763736 xbotext-0.1.5/xbotext/sofaware.py
+-rw-r--r--   0        0        0      101 2024-05-07 11:55:00.763736 xbotext-0.1.5/xbotext/system.py
+-rw-r--r--   0        0        0      538 2024-05-07 12:29:59.187663 xbotext-0.1.5/xbotext/web.py
+-rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 xbotext-0.1.5/PKG-INFO
```

### Comparing `xbotext-0.1.4/xbotext/cache.py` & `xbotext-0.1.5/xbotext/cache.py`

 * *Files identical despite different names*

### Comparing `xbotext-0.1.4/xbotext/chromium.py` & `xbotext-0.1.5/xbotext/chromium.py`

 * *Files identical despite different names*

### Comparing `xbotext-0.1.4/xbotext/regedit.py` & `xbotext-0.1.5/xbotext/regedit.py`

 * *Files identical despite different names*

### Comparing `xbotext-0.1.4/xbotext/web.py` & `xbotext-0.1.5/xbotext/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import xbot.web
+from xbot import web
 
 def get_web_page_by_web_page(web_page):
     """根据网页对象获取网页对象"""
     product_name = getattr(
         web_page, "product_name",
         "cef" if web_page._controller == "CEFBrowser" else "firefox")
-    return xbot.web.get_active(mode=product_name)
+    return web.get_active(mode=product_name)
 
 
 def get_web_page_product_name(web_page):
     """根据网页对象获取浏览器的名称"""
     product_name = getattr(
         web_page, "product_name",
         "cef" if web_page._controller == "CEFBrowser" else "firefox")
```


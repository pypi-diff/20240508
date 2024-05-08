# Comparing `tmp/hosted-flasks-0.0.8.tar.gz` & `tmp/hosted-flasks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosted-flasks-0.0.8.tar", last modified: Mon Apr 29 19:41:37 2024, max compression
+gzip compressed data, was "hosted-flasks-0.0.9.tar", last modified: Mon Apr 29 19:50:15 2024, max compression
```

## Comparing `hosted-flasks-0.0.8.tar` & `hosted-flasks-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.020411 hosted-flasks-0.0.8/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.016322 hosted-flasks-0.0.8/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.8/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 19:41:37.020279 hosted-flasks-0.0.8/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.016533 hosted-flasks-0.0.8/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/docs/conf.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.017288 hosted-flasks-0.0.8/hosted_flasks/
--rw-r--r--   0 xtof       (501) staff       (20)      429 2024-04-29 19:38:18.000000 hosted-flasks-0.0.8/hosted_flasks/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      702 2024-04-28 11:59:41.000000 hosted-flasks-0.0.8/hosted_flasks/__main__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.018122 hosted-flasks-0.0.8/hosted_flasks/frontpage/
--rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/index.html
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.019221 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/
--rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/android-chrome-192x192.png
--rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/android-chrome-512x512.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/apple-touch-icon.png
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.019514 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/
--rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/default.css
--rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-28 14:20:24.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/style.css
--rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon-16x16.png
--rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon-32x32.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon.ico
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.019731 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/img/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/img/.gitkeep
--rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/img/logo.svg
--rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/robots.txt
--rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/site.webmanifest
--rw-r--r--   0 xtof       (501) staff       (20)      830 2024-04-28 14:20:16.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage.py
--rw-r--r--   0 xtof       (501) staff       (20)     3021 2024-04-29 19:32:45.000000 hosted-flasks-0.0.8/hosted_flasks/loader.py
--rw-r--r--   0 xtof       (501) staff       (20)     2335 2024-04-29 19:37:42.000000 hosted-flasks-0.0.8/hosted_flasks/monkeypatch.py
--rw-r--r--   0 xtof       (501) staff       (20)     1753 2024-04-29 19:33:59.000000 hosted-flasks-0.0.8/hosted_flasks/server.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.017987 hosted-flasks-0.0.8/hosted_flasks.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)     1139 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       36 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-29 19:41:37.020470 hosted-flasks-0.0.8/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1639 2024-04-28 10:59:13.000000 hosted-flasks-0.0.8/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.020078 hosted-flasks-0.0.8/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1029 2024-04-29 19:40:04.000000 hosted-flasks-0.0.8/tests/test_environ_get.py
--rw-r--r--   0 xtof       (501) staff       (20)     3678 2024-04-29 19:35:16.000000 hosted-flasks-0.0.8/tests/test_loader.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.735881 hosted-flasks-0.0.9/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.732169 hosted-flasks-0.0.9/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.9/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.9/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.9/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 19:50:15.735770 hosted-flasks-0.0.9/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.732366 hosted-flasks-0.0.9/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.9/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.9/docs/conf.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.733028 hosted-flasks-0.0.9/hosted_flasks/
+-rw-r--r--   0 xtof       (501) staff       (20)      429 2024-04-29 19:49:55.000000 hosted-flasks-0.0.9/hosted_flasks/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      702 2024-04-28 11:59:41.000000 hosted-flasks-0.0.9/hosted_flasks/__main__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.733829 hosted-flasks-0.0.9/hosted_flasks/frontpage/
+-rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/index.html
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.734816 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/
+-rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/android-chrome-192x192.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/android-chrome-512x512.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/apple-touch-icon.png
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.735071 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/css/
+-rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/css/default.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-28 14:20:24.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/css/style.css
+-rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/favicon-16x16.png
+-rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/favicon-32x32.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/favicon.ico
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.735275 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/img/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/img/.gitkeep
+-rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/img/logo.svg
+-rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/robots.txt
+-rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage/static/site.webmanifest
+-rw-r--r--   0 xtof       (501) staff       (20)      830 2024-04-28 14:20:16.000000 hosted-flasks-0.0.9/hosted_flasks/frontpage.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3021 2024-04-29 19:32:45.000000 hosted-flasks-0.0.9/hosted_flasks/loader.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2335 2024-04-29 19:37:42.000000 hosted-flasks-0.0.9/hosted_flasks/monkeypatch.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1757 2024-04-29 19:49:29.000000 hosted-flasks-0.0.9/hosted_flasks/server.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.733723 hosted-flasks-0.0.9/hosted_flasks.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 19:50:15.000000 hosted-flasks-0.0.9/hosted_flasks.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)     1139 2024-04-29 19:50:15.000000 hosted-flasks-0.0.9/hosted_flasks.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-29 19:50:15.000000 hosted-flasks-0.0.9/hosted_flasks.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-29 19:50:15.000000 hosted-flasks-0.0.9/hosted_flasks.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       36 2024-04-29 19:50:15.000000 hosted-flasks-0.0.9/hosted_flasks.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-29 19:50:15.000000 hosted-flasks-0.0.9/hosted_flasks.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-29 19:50:15.735928 hosted-flasks-0.0.9/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1639 2024-04-28 10:59:13.000000 hosted-flasks-0.0.9/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:50:15.735600 hosted-flasks-0.0.9/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.9/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1029 2024-04-29 19:40:04.000000 hosted-flasks-0.0.9/tests/test_environ_get.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3678 2024-04-29 19:35:16.000000 hosted-flasks-0.0.9/tests/test_loader.py
```

### Comparing `hosted-flasks-0.0.8/.github/README.md` & `hosted-flasks-0.0.9/.github/README.md`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/LICENSE.txt` & `hosted-flasks-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/PKG-INFO` & `hosted-flasks-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.8
+Version: 0.0.9
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.8/docs/conf.py` & `hosted-flasks-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/__main__.py` & `hosted-flasks-0.0.9/hosted_flasks/__main__.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/index.html` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/index.html`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/android-chrome-192x192.png` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/android-chrome-512x512.png` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/apple-touch-icon.png` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/default.css` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/static/css/default.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/style.css` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/static/css/style.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon-16x16.png` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon-32x32.png` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon.ico` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/img/logo.svg` & `hosted-flasks-0.0.9/hosted_flasks/frontpage/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/frontpage.py` & `hosted-flasks-0.0.9/hosted_flasks/frontpage.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/loader.py` & `hosted-flasks-0.0.9/hosted_flasks/loader.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/monkeypatch.py` & `hosted-flasks-0.0.9/hosted_flasks/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/hosted_flasks/server.py` & `hosted-flasks-0.0.9/hosted_flasks/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     self.paths     = DispatcherMiddleware(frontpage, paths)
 
   def __call__(self, environ, start_response):
     # first check if we have a hostname mapping
     hostname = environ["HTTP_HOST"]
     handler = self.hosts.get(hostname, None)
     if handler:
-      logger.info("🧭 dispatching {hostname} to {handler}")
+      logger.debug(f"🧭 dispatching {hostname} to {handler}")
     else:
-      logger.info("🧭 dispatching locally (no mapping for {hostname})")
+      logger.debug(f"🧭 dispatching locally (no mapping for {hostname})")
       handler = self.paths
     return handler(environ, start_response)
 
 # combine the apps with the frontpage
 
 hosts = { app.hostname : app.handler for app in get_apps() if app.hostname }
 paths = { app.path     : app.handler for app in get_apps() if app.path     }
```

### Comparing `hosted-flasks-0.0.8/hosted_flasks.egg-info/PKG-INFO` & `hosted-flasks-0.0.9/hosted_flasks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.8
+Version: 0.0.9
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.8/hosted_flasks.egg-info/SOURCES.txt` & `hosted-flasks-0.0.9/hosted_flasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/setup.py` & `hosted-flasks-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/tests/test_environ_get.py` & `hosted-flasks-0.0.9/tests/test_environ_get.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.8/tests/test_loader.py` & `hosted-flasks-0.0.9/tests/test_loader.py`

 * *Files identical despite different names*


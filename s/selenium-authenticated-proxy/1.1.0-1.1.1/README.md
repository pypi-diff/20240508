# Comparing `tmp/selenium_authenticated_proxy-1.1.0-py3-none-any.whl.zip` & `tmp/selenium_authenticated_proxy-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6979 bytes, number of entries: 10
--rw-r--r--  2.0 unx      125 b- defN 24-May-07 11:23 selenium_authenticated_proxy/__init__.py
--rw-r--r--  2.0 unx     2111 b- defN 24-May-07 11:23 selenium_authenticated_proxy/selenium_authenticated_proxy.py
--rw-r--r--  2.0 unx     3163 b- defN 24-May-07 11:23 selenium_authenticated_proxy/selenium_extension_generator.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-07 11:23 test/__init__.py
--rw-r--r--  2.0 unx     1699 b- defN 24-May-07 11:23 test/test_proxy.py
--rw-r--r--  2.0 unx     1076 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3208 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       34 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      966 b- defN 24-May-07 11:23 selenium_authenticated_proxy-1.1.0.dist-info/RECORD
-10 files, 12474 bytes uncompressed, 5281 bytes compressed:  57.7%
+Zip file size: 7057 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      125 b- defN 24-May-08 08:22 selenium_authenticated_proxy/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-May-08 08:22 selenium_authenticated_proxy/selenium_authenticated_proxy.py
+-rw-r--r--  2.0 unx     3163 b- defN 24-May-08 08:22 selenium_authenticated_proxy/selenium_extension_generator.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-08 08:22 test/__init__.py
+-rw-r--r--  2.0 unx     1699 b- defN 24-May-08 08:22 test/test_proxy.py
+-rw-r--r--  2.0 unx     1076 b- defN 24-May-08 08:22 selenium_authenticated_proxy-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3208 b- defN 24-May-08 08:22 selenium_authenticated_proxy-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 08:22 selenium_authenticated_proxy-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       34 b- defN 24-May-08 08:22 selenium_authenticated_proxy-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      966 b- defN 24-May-08 08:22 selenium_authenticated_proxy-1.1.1.dist-info/RECORD
+10 files, 12821 bytes uncompressed, 5359 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_proxy.py
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.1.0.dist-info/LICENSE
+Filename: selenium_authenticated_proxy-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.1.0.dist-info/METADATA
+Filename: selenium_authenticated_proxy-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.1.0.dist-info/WHEEL
+Filename: selenium_authenticated_proxy-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.1.0.dist-info/top_level.txt
+Filename: selenium_authenticated_proxy-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: selenium_authenticated_proxy-1.1.0.dist-info/RECORD
+Filename: selenium_authenticated_proxy-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## selenium_authenticated_proxy/selenium_authenticated_proxy.py

```diff
@@ -4,20 +4,21 @@
 
 from selenium_authenticated_proxy.selenium_extension_generator import (
     SeleniumExtensionGenerator,
 )
 
 
 class SeleniumAuthenticatedProxy:
-    def __init__(self, proxy_url=None, tmp_folder=None):
+    def __init__(self, proxy_url=None, tmp_folder=None, use_legacy_extension=False):
         """Constructor for initializing proxy_url and tmp_folder."""
         self.proxy_url = proxy_url
         self.tmp_folder = tmp_folder or os.path.abspath(
             os.path.join(os.path.dirname(__file__), "tmp")
         )
+        self.use_legacy_extension = use_legacy_extension
 
     def _get_zip_filename(self):
         input_string = f"{self.proxy_url}"
 
         hasher = hashlib.sha256()
         hasher.update(input_string.encode())
 
@@ -49,17 +50,23 @@
         result = urlparse(self.proxy_url)
         return result.scheme
 
     def _is_authenticated_url(self):
         result = urlparse(self.proxy_url)
         return result.username is not None
 
+    def _add_extension(self, chrome_options, extension_file: str):
+        if self.use_legacy_extension:
+            chrome_options.add_argument(f"--load-extension={extension_file}")
+        else:
+            chrome_options.add_extension(extension_file)
+
     def enrich_chrome_options(self, chrome_options):
         """Add the generated extension to Chrome options."""
         if not self.proxy_url:
             return chrome_options
         if self._is_authenticated_url():
-            chrome_options.add_extension(self._generate_plugin_file())
+            self._add_extension(chrome_options, self._generate_plugin_file())
         chrome_options.add_argument(
             f"--proxy-server={self._get_unauthenticated_url()}"
         )
         return chrome_options
```

## Comparing `selenium_authenticated_proxy-1.1.0.dist-info/LICENSE` & `selenium_authenticated_proxy-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `selenium_authenticated_proxy-1.1.0.dist-info/METADATA` & `selenium_authenticated_proxy-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-authenticated-proxy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python package to add authenticated proxy support to selenium.
 Home-page: https://github.com/bubblegumsoldier/selenium-authenticated-proxy
 Author: Henry Müssemann
 Author-email: hm@freezingdata.de
 License: MIT
 Keywords: proxy,selenium,auth,selenium
 Platform: UNKNOWN
```

## Comparing `selenium_authenticated_proxy-1.1.0.dist-info/RECORD` & `selenium_authenticated_proxy-1.1.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 selenium_authenticated_proxy/__init__.py,sha256=G3TCTIpfeaMSW8sGgEms5tTjJ7X6N9LMIE3YfAFOyQk,125
-selenium_authenticated_proxy/selenium_authenticated_proxy.py,sha256=xuC_Mxy7CxHdgodJ6b0SCLXOsfjsTtZLYzxoPUP5eSo,2111
+selenium_authenticated_proxy/selenium_authenticated_proxy.py,sha256=LBTlyiOFeG6QCz22zjFsfy0aiWjtq2z0HelD4NtHxBg,2458
 selenium_authenticated_proxy/selenium_extension_generator.py,sha256=yOJnidQ3fwmVN9wPvm1gczA3T2MV5JFmX15_USlCDlk,3163
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_proxy.py,sha256=BUIs0fthkAealjqyazzWt8kBGAp9CKe7MNNwgbspGi4,1699
-selenium_authenticated_proxy-1.1.0.dist-info/LICENSE,sha256=bhs5U3qqHxnr1T_NkQbie2dwXfWZLJdvzJvXfu__GlU,1076
-selenium_authenticated_proxy-1.1.0.dist-info/METADATA,sha256=YEHnaU1ZyZEpioilmJTboRLP-Hvg-TEFkWc1HjO5ync,3208
-selenium_authenticated_proxy-1.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-selenium_authenticated_proxy-1.1.0.dist-info/top_level.txt,sha256=GjQaO_8ocTo1xFNJ6rIqnC5SlVTfZkbI-3QK6ZNQSHM,34
-selenium_authenticated_proxy-1.1.0.dist-info/RECORD,,
+selenium_authenticated_proxy-1.1.1.dist-info/LICENSE,sha256=bhs5U3qqHxnr1T_NkQbie2dwXfWZLJdvzJvXfu__GlU,1076
+selenium_authenticated_proxy-1.1.1.dist-info/METADATA,sha256=BOVLcwaS2ZzHs7KZ4xaiqCltYaZe_Q1vfKd8Tb4VQOs,3208
+selenium_authenticated_proxy-1.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+selenium_authenticated_proxy-1.1.1.dist-info/top_level.txt,sha256=GjQaO_8ocTo1xFNJ6rIqnC5SlVTfZkbI-3QK6ZNQSHM,34
+selenium_authenticated_proxy-1.1.1.dist-info/RECORD,,
```


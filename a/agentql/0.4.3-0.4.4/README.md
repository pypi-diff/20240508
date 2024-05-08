# Comparing `tmp/agentql-0.4.3.tar.gz` & `tmp/agentql-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentql-0.4.3.tar", max compression
+gzip compressed data, was "agentql-0.4.4.tar", max compression
```

## Comparing `agentql-0.4.3.tar` & `agentql-0.4.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1066 2024-05-05 00:14:34.687824 agentql-0.4.3/LICENSE
--rw-r--r--   0        0        0      111 2024-05-05 00:14:34.687824 agentql-0.4.3/PACKAGE_README.md
--rw-r--r--   0        0        0      771 2024-05-05 00:14:34.775824 agentql-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      536 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/__init__.py
--rw-r--r--   0        0        0       78 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_api_constants.py
--rw-r--r--   0        0        0     4741 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_errors.py
--rw-r--r--   0        0        0        0 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_js_snippets/__init__.py
--rw-r--r--   0        0        0      322 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_js_snippets/add_dom_change_listener.js
--rw-r--r--   0        0        0     7241 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
--rw-r--r--   0        0        0      147 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_js_snippets/get_last_dom_change.js
--rw-r--r--   0        0        0      145 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
--rw-r--r--   0        0        0      506 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_js_snippets/scroll_to_bottom.js
--rw-r--r--   0        0        0      503 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_js_snippets/scroll_to_top.js
--rw-r--r--   0        0        0      843 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_js_snippets/set_iframe_path.js
--rw-r--r--   0        0        0      436 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_js_snippets/snippet_loader.py
--rw-r--r--   0        0        0        0 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_syntax/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_syntax/character_utils.py
--rw-r--r--   0        0        0     4997 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_syntax/lexer.py
--rw-r--r--   0        0        0     2431 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_syntax/node.py
--rw-r--r--   0        0        0     4686 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_syntax/parser.py
--rw-r--r--   0        0        0     1196 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_syntax/source.py
--rw-r--r--   0        0        0     1602 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_syntax/token.py
--rw-r--r--   0        0        0      213 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_syntax/token_kind.py
--rw-r--r--   0        0        0      535 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_typing.py
--rw-r--r--   0        0        0      377 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/_core/_utils.py
--rw-r--r--   0        0        0      363 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/async_api/__init__.py
--rw-r--r--   0        0        0     2893 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/async_api/_api.py
--rw-r--r--   0        0        0     1840 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/async_api/_popup.py
--rw-r--r--   0        0        0     5979 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/async_api/_response_proxy.py
--rw-r--r--   0        0        0    11329 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/async_api/_session.py
--rw-r--r--   0        0        0     5601 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/async_api/_web_driver.py
--rw-r--r--   0        0        0        0 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/ext/__init__.py
--rw-r--r--   0        0        0      288 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/ext/playwright/__init__.py
--rw-r--r--   0        0        0      193 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/ext/playwright/_driver_constants.py
--rw-r--r--   0        0        0      280 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/ext/playwright/_driver_settings.py
--rw-r--r--   0        0        0     1980 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/ext/playwright/_html_constants.py
--rw-r--r--   0        0        0     3813 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/ext/playwright/_network_monitor.py
--rw-r--r--   0        0        0    27588 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/ext/playwright/playwright_driver_async.py
--rw-r--r--   0        0        0    27290 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/ext/playwright/playwright_driver_sync.py
--rw-r--r--   0        0        0      363 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/sync_api/__init__.py
--rw-r--r--   0        0        0     2847 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/sync_api/_api.py
--rw-r--r--   0        0        0     1525 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/sync_api/_popup.py
--rw-r--r--   0        0        0     5291 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/sync_api/_response_proxy.py
--rw-r--r--   0        0        0    11068 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/sync_api/_session.py
--rw-r--r--   0        0        0     5017 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/sync_api/_web_driver.py
--rw-r--r--   0        0        0      291 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/trail_logger/__init__.py
--rw-r--r--   0        0        0     5151 2024-05-05 00:14:34.775824 agentql-0.4.3/src/agentql/trail_logger/trail_logger.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-08 14:57:21.100533 agentql-0.4.4/LICENSE
+-rw-r--r--   0        0        0      111 2024-05-08 14:57:21.100533 agentql-0.4.4/PACKAGE_README.md
+-rw-r--r--   0        0        0      771 2024-05-08 14:57:21.188532 agentql-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      536 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/__init__.py
+-rw-r--r--   0        0        0       78 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_api_constants.py
+-rw-r--r--   0        0        0     4741 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_errors.py
+-rw-r--r--   0        0        0        0 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/add_dom_change_listener.js
+-rw-r--r--   0        0        0     7207 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
+-rw-r--r--   0        0        0      147 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/get_last_dom_change.js
+-rw-r--r--   0        0        0      145 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
+-rw-r--r--   0        0        0      506 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/scroll_to_bottom.js
+-rw-r--r--   0        0        0      503 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/scroll_to_top.js
+-rw-r--r--   0        0        0      843 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/set_iframe_path.js
+-rw-r--r--   0        0        0      436 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/snippet_loader.py
+-rw-r--r--   0        0        0        0 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/character_utils.py
+-rw-r--r--   0        0        0     4997 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/lexer.py
+-rw-r--r--   0        0        0     2431 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/node.py
+-rw-r--r--   0        0        0     4686 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/parser.py
+-rw-r--r--   0        0        0     1196 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/source.py
+-rw-r--r--   0        0        0     1602 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/token.py
+-rw-r--r--   0        0        0      213 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/token_kind.py
+-rw-r--r--   0        0        0      535 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_typing.py
+-rw-r--r--   0        0        0      377 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_utils.py
+-rw-r--r--   0        0        0      363 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/__init__.py
+-rw-r--r--   0        0        0     2893 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_api.py
+-rw-r--r--   0        0        0     1840 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_popup.py
+-rw-r--r--   0        0        0     5979 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_response_proxy.py
+-rw-r--r--   0        0        0    11329 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_session.py
+-rw-r--r--   0        0        0     5601 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_web_driver.py
+-rw-r--r--   0        0        0        0 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/_driver_constants.py
+-rw-r--r--   0        0        0      280 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/_driver_settings.py
+-rw-r--r--   0        0        0     1980 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/_html_constants.py
+-rw-r--r--   0        0        0     3813 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/_network_monitor.py
+-rw-r--r--   0        0        0    27588 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/playwright_driver_async.py
+-rw-r--r--   0        0        0    27290 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/playwright_driver_sync.py
+-rw-r--r--   0        0        0      363 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/__init__.py
+-rw-r--r--   0        0        0     2847 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_api.py
+-rw-r--r--   0        0        0     1525 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_popup.py
+-rw-r--r--   0        0        0     5291 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_response_proxy.py
+-rw-r--r--   0        0        0    11068 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_session.py
+-rw-r--r--   0        0        0     5017 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_web_driver.py
+-rw-r--r--   0        0        0      291 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/trail_logger/__init__.py
+-rw-r--r--   0        0        0     5151 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/trail_logger/trail_logger.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.4.4/PKG-INFO
```

### Comparing `agentql-0.4.3/LICENSE` & `agentql-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/pyproject.toml` & `agentql-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentql"
-version = "0.4.3"
+version = "0.4.4"
 description = "Tiny Fish AgentQL Python Client"
 authors = []
 license = "MIT"
 readme = "PACKAGE_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `agentql-0.4.3/src/agentql/__init__.py` & `agentql-0.4.4/src/agentql/__init__.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/_core/_errors.py` & `agentql-0.4.4/src/agentql/_core/_errors.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/_core/_js_snippets/generate_accessibility_tree.js` & `agentql-0.4.4/src/agentql/_core/_js_snippets/generate_accessibility_tree.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -104,33 +104,35 @@
 
         // Fallback to empty string if no non-empty attribute is found
         return "";
     }
 
     function isElementHidden(element) {
         // Check if the element exists
-        if (!element || !element.offsetWidth || !element.offsetHeight) {
-            return false;
+        if (!element) {
+            return true;
         }
         const style = window.getComputedStyle(element);
 
         // Check if the element is hidden by display property
         if (style.display === "none") {
-            return false;
+            return true;
         }
 
         // Check if the element is hidden by visibility property
         if (style.visibility !== "visible") {
-            return false;
+            return true;
         }
 
         // Check if the element is hidden by opacity
         if (style.opacity === "0") {
-            return false;
+            return true;
         }
+
+        return false;
     }
 
     function createNode(node, currentIframePath = "") {
         const ariaHidden =
             node.getAttribute("aria-hidden") === "true" ||
             node.getAttribute("aria-hidden") === true;
         const tag = node.nodeName.toLowerCase();
```

### Comparing `agentql-0.4.3/src/agentql/_core/_js_snippets/set_iframe_path.js` & `agentql-0.4.4/src/agentql/_core/_js_snippets/set_iframe_path.js`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/_core/_syntax/character_utils.py` & `agentql-0.4.4/src/agentql/_core/_syntax/character_utils.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/_core/_syntax/lexer.py` & `agentql-0.4.4/src/agentql/_core/_syntax/lexer.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/_core/_syntax/node.py` & `agentql-0.4.4/src/agentql/_core/_syntax/node.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/_core/_syntax/parser.py` & `agentql-0.4.4/src/agentql/_core/_syntax/parser.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/_core/_syntax/source.py` & `agentql-0.4.4/src/agentql/_core/_syntax/source.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/_core/_syntax/token.py` & `agentql-0.4.4/src/agentql/_core/_syntax/token.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/_core/_typing.py` & `agentql-0.4.4/src/agentql/_core/_typing.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/async_api/_api.py` & `agentql-0.4.4/src/agentql/async_api/_api.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/async_api/_popup.py` & `agentql-0.4.4/src/agentql/async_api/_popup.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/async_api/_response_proxy.py` & `agentql-0.4.4/src/agentql/async_api/_response_proxy.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/async_api/_session.py` & `agentql-0.4.4/src/agentql/async_api/_session.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/async_api/_web_driver.py` & `agentql-0.4.4/src/agentql/async_api/_web_driver.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/ext/playwright/_html_constants.py` & `agentql-0.4.4/src/agentql/ext/playwright/_html_constants.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/ext/playwright/_network_monitor.py` & `agentql-0.4.4/src/agentql/ext/playwright/_network_monitor.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/ext/playwright/playwright_driver_async.py` & `agentql-0.4.4/src/agentql/ext/playwright/playwright_driver_async.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/ext/playwright/playwright_driver_sync.py` & `agentql-0.4.4/src/agentql/ext/playwright/playwright_driver_sync.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/sync_api/_api.py` & `agentql-0.4.4/src/agentql/sync_api/_api.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/sync_api/_popup.py` & `agentql-0.4.4/src/agentql/sync_api/_popup.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/sync_api/_response_proxy.py` & `agentql-0.4.4/src/agentql/sync_api/_response_proxy.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/sync_api/_session.py` & `agentql-0.4.4/src/agentql/sync_api/_session.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/sync_api/_web_driver.py` & `agentql-0.4.4/src/agentql/sync_api/_web_driver.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/src/agentql/trail_logger/trail_logger.py` & `agentql-0.4.4/src/agentql/trail_logger/trail_logger.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.3/PKG-INFO` & `agentql-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentql
-Version: 0.4.3
+Version: 0.4.4
 Summary: Tiny Fish AgentQL Python Client
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


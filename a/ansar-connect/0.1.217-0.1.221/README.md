# Comparing `tmp/ansar_connect-0.1.217.tar.gz` & `tmp/ansar_connect-0.1.221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.217.tar", last modified: Tue May  7 00:48:59 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.221.tar", last modified: Tue May  7 04:34:19 2024, max compression
```

## Comparing `ansar_connect-0.1.217.tar` & `ansar_connect-0.1.221.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.217/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.217/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.217/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.217/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.241938 ansar_connect-0.1.217/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.241938 ansar_connect-0.1.217/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.241938 ansar_connect-0.1.217/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.217/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.217/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.217/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.217/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3032 2024-05-07 00:48:56.000000 ansar_connect-0.1.217/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.217/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87388 2024-05-07 00:48:01.000000 ansar_connect-0.1.217/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9104 2024-05-07 00:25:17.000000 ansar_connect-0.1.217/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.217/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.217/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.217/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.217/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-06 04:43:32.000000 ansar_connect-0.1.217/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.217/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.217/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.217/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.217/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.217/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    40495 2024-05-07 00:48:01.000000 ansar_connect-0.1.217/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.217/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 00:41:36.000000 ansar_connect-0.1.217/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.217/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-06 04:43:32.000000 ansar_connect-0.1.217/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 00:48:59.245938 ansar_connect-0.1.217/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-07 00:48:59.000000 ansar_connect-0.1.217/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 04:34:19.624932 ansar_connect-0.1.221/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.221/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-07 04:34:19.624932 ansar_connect-0.1.221/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.221/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.221/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-07 04:34:19.624932 ansar_connect-0.1.221/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.221/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 04:34:19.620932 ansar_connect-0.1.221/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 04:34:19.620932 ansar_connect-0.1.221/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 04:34:19.624932 ansar_connect-0.1.221/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.221/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.221/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.221/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.221/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 04:34:19.624932 ansar_connect-0.1.221/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-07 04:34:16.000000 ansar_connect-0.1.221/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.221/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87388 2024-05-07 01:18:28.000000 ansar_connect-0.1.221/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.221/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.221/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.221/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.221/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.221/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.221/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.221/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.221/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.221/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.221/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.221/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    39924 2024-05-07 04:34:09.000000 ansar_connect-0.1.221/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.221/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.221/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.221/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.221/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-07 04:34:19.624932 ansar_connect-0.1.221/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-07 04:34:19.000000 ansar_connect-0.1.221/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-07 04:34:19.000000 ansar_connect-0.1.221/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-07 04:34:19.000000 ansar_connect-0.1.221/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-07 04:34:19.000000 ansar_connect-0.1.221/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-07 04:34:19.000000 ansar_connect-0.1.221/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-07 04:34:19.000000 ansar_connect-0.1.221/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.217/LICENSE` & `ansar_connect-0.1.221/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/PKG-INFO` & `ansar_connect-0.1.221/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.217
+Version: 0.1.221
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.217/README.md` & `ansar_connect-0.1.221/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/pyproject.toml` & `ansar_connect-0.1.221/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/setup.py` & `ansar_connect-0.1.221/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.221/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.221/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.221/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.221/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/__init__.py` & `ansar_connect-0.1.221/src/ansar/connect/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
-Branch: upgrade-pub-sub-messages
-Commit: d6bc546c0f99d5aac45600fc497588b40c6701bf
-Version: 0.1.216 (2024-05-07@12:48:56+NZST)
+Branch: main
+Commit: c65a1575896e8a89a6efac5eeb2ab710c972ec71
+Version: 0.1.220 (2024-05-07@16:34:16+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.217/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.221/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/directory.py` & `ansar_connect-0.1.221/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.221/src/ansar/connect/directory_if.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,101 +55,87 @@
 		self.requested_name = requested_name
 		self.requested_scope = requested_scope
 		self.listening_ipp = listening_ipp or HostPort()
 		self.published_at = published_at
 
 class NotPublished(ar.Faulted):
 	def __init__(self, requested_name=None, reason=None):
+		ar.Faulted.__init__(self, f'cannot publish "{requested_name}"', reason)
 		self.requested_name = requested_name
 		self.reason = reason
-		ar.Faulted.__init__(self, f'cannot publish "{requested_name}"', reason)
-		#self.condition = cannot
-		#self.explanation = reason
-		self.error_code = None
-		self.error_text = None
 
 class Subscribed(object):
 	def __init__(self, requested_search=None, requested_scope=ScopeOfService.WAN, subscribed_at=None):
 		self.requested_search = requested_search
 		self.requested_scope = requested_scope
 		self.subscribed_at = subscribed_at
 
-# The actual service directory with listings and searches.
 #
-
-# Session messages to publish/listen controllers.
-# Subscribe/client/calling/outbound end.
+#
 class Available(object):
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, opened_at=None, route_key=None, agent_address=None):
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.opened_at = opened_at
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotAvailable(ar.Faulted):
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, agent_address=None):
+		ar.Faulted.__init__(self, 'no subsciber peer', reason)
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.reason = reason
 		self.agent_address = agent_address
-		ar.Faulted.__init__(self, 'no subscibe peer', reason)
-		#self.condition = cannot
-		#self.explanation = reason
-		self.error_code = None
-		self.error_text = None
 
-# Publish/service/answering/inbound end.
 class Delivered(object):
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, opened_at=None, route_key=None, agent_address=None):
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.opened_at = opened_at
 		self.route_key = route_key
 		self.agent_address = agent_address
 
 class NotDelivered(ar.Faulted):
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, agent_address=None):
+		ar.Faulted.__init__(self, 'no publisher peer', reason)
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.reason = reason
 		self.agent_address = agent_address
-		ar.Faulted.__init__(self, 'no publish peer', reason)
-		self.error_code = None
-		self.error_text = None
 
 class Clear(object):
 	def __init__(self, session=None, value=None):
 		self.session = session
 		self.value = value
 
 class Cleared(object):
-	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, value=None):
+	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None, value=None):
+		ar.Faulted.__init__(self, 'peer cleared', reason)
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
+		self.reason = reason
 		self.value = value
 
 class Dropped(ar.Faulted):
 	def __init__(self, matched_search=None, matched_name=None, matched_scope=None, route_key=None, reason=None):
+		ar.Faulted.__init__(self, 'peer dropped', reason)
 		self.matched_search = matched_search
 		self.matched_name = matched_name
 		self.matched_scope = matched_scope
 		self.route_key = route_key
 		self.reason = reason
-		ar.Faulted.__init__(self, 'peer lost', reason)
-		self.error_code = None
-		self.error_text = None
 
 ENDING_SCHEMA = {
 	'matched_search': ar.Unicode(),
 	'matched_name': ar.Unicode(),
 	'matched_scope': ScopeOfService,
 	'opened_at': ar.WorldTime(),
 	'route_key': ar.Unicode(),
@@ -164,27 +150,19 @@
 }
 
 ar.bind(Clear, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Cleared, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Dropped, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 
 SHARED_SCHEMA = {
-	#'route_key': ar.VectorOf(ar.Integer8()),
-	'name': ar.Unicode(),
-	'requested_name': ar.Unicode(),
 	'requested_search': ar.Unicode(),
 	'requested_name': ar.Unicode(),
-	'remote_address': ar.Address(),
-	'session_address': ar.Address(),
 	'requested_scope': ScopeOfService,
-	'service_scope': ScopeOfService,
-	'reason': ar.Unicode(),
 	'listening_ipp': ar.UserDefined(HostPort),
 	'agent_address': ar.Address(),
-	'address': ar.Address(),
 	'published_at': ar.WorldTime(),
 	'subscribed_at': ar.WorldTime(),
 }
 
 SHARED_SCHEMA.update(ENDING_SCHEMA)
 
 ar.bind(Subscribed, object_schema=SHARED_SCHEMA)
```

### Comparing `ansar_connect-0.1.217/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.221/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/group_if.py` & `ansar_connect-0.1.221/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/grouping.py` & `ansar_connect-0.1.221/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/moving.py` & `ansar_connect-0.1.221/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/networking.py` & `ansar_connect-0.1.221/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.221/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/node.py` & `ansar_connect-0.1.221/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.221/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/procedure.py` & `ansar_connect-0.1.221/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/product.py` & `ansar_connect-0.1.221/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/socketry.py` & `ansar_connect-0.1.221/src/ansar/connect/socketry.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,41 +171,26 @@
 		self.requested_ipp = requested_ipp or HostPort()
 		self.connected_ipp = connected_ipp or HostPort()
 		self.remote_address = remote_address
 		self.opened_at = opened_at
 
 class NotListening(ar.Faulted):
 	def __init__(self, requested_ipp=None, error_code=0, error_text=None):
-		cannot = f'cannot listen at "{requested_ipp}"'
-		reason = error_text
-		ar.Faulted.__init__(self, cannot, reason, exit_code=error_code)
+		ar.Faulted.__init__(self, f'cannot listen at "{requested_ipp}"', error_text, exit_code=error_code)
 		self.requested_ipp = requested_ipp or HostPort()
-		self.error_code = error_code
-		self.error_text = error_text
 
 class NotAccepted(ar.Faulted):
 	def __init__(self, listening_ipp=None, error_code=0, error_text=None):
-		cannot = f'cannot accept at "{listening_ipp}"'
-		reason = error_text
-		ar.Faulted.__init__(self, cannot, reason, exit_code=error_code)
+		ar.Faulted.__init__(self, f'cannot accept at "{listening_ipp}"', error_text, exit_code=error_code)
 		self.listening_ipp = listening_ipp or HostPort()
-		self.error_code = error_code
-		self.error_text = error_text
 
 class NotConnected(ar.Faulted):
 	def __init__(self, requested_ipp=None, error_code=0, error_text=None):
-		cannot = f'cannot connect to "{requested_ipp}"'
-		reason = error_text
-		ar.Faulted.__init__(self, cannot, reason, exit_code=error_code)
-		#self.condition = cannot
-		#self.explanation = reason
-		#self.exit_code = error_code
+		ar.Faulted.__init__(self, f'cannot connect to "{requested_ipp}"', error_text, exit_code=error_code)
 		self.requested_ipp = requested_ipp or HostPort()
-		self.error_code = error_code
-		self.error_text = error_text
 
 CONTROL_SCHEMA = {
 	'requested_ipp': ar.UserDefined(HostPort),
 	'controller_address': ar.Address(),
 	'remote_address': ar.Address(),
 	'opened_at': ar.WorldTime(),
 	'upgrade': ar.Type(),
@@ -213,14 +198,15 @@
 	'connected_ipp': ar.UserDefined(HostPort),
 	'listening_ipp': ar.UserDefined(HostPort),
 	'accepted_ipp': ar.UserDefined(HostPort),
 	'condition': ar.Unicode(),
 	'explanation': ar.Unicode(),
 	'error_code': ar.Integer8(),
 	'error_text': ar.Unicode(),
+	'exit_code': ar.Integer8(),
 	'encrypted': ar.Boolean(),
 }
 
 ar.bind(ListenForStream, object_schema=CONTROL_SCHEMA)
 ar.bind(ConnectStream, object_schema=CONTROL_SCHEMA)
 ar.bind(StopListening, object_schema=CONTROL_SCHEMA)
 ar.bind(Listening, object_schema=CONTROL_SCHEMA, copy_before_sending=False)
@@ -233,40 +219,35 @@
 # Session termination messages. Handshake between app
 # and sockets thread to cleanly terminate a connection.
 class Close(object):
 	def __init__(self, value=None):
 		self.value = value
 
 class Closed(ar.Faulted):
-	def __init__(self, value=None, reason=None, opened_ipp=None, opened_at=None, closed_at=None):
+	def __init__(self, value=None, reason=None, opened_ipp=None, opened_at=None):
+		ar.Faulted.__init__(self, f'closed {opened_ipp}', reason)
 		self.value = value
 		self.opened_ipp = opened_ipp or HostPort()
-		cannot = f'closed {self.opened_ipp}'
-		ar.Faulted.__init__(self, cannot, reason)
 		self.opened_at = opened_at
-		self.closed_at = closed_at
 
 class Abandoned(ar.Faulted):
-	def __init__(self, opened_ipp=None, opened_at=None, closed_at=None):
+	def __init__(self, opened_ipp=None, opened_at=None):
+		ar.Faulted.__init__(self, f'abandoned by {opened_ipp}')
 		self.opened_ipp = opened_ipp or HostPort()
-		cannot = f'abandoned by {self.opened_ipp}'
-		reason = None
-		ar.Faulted.__init__(self, cannot, reason)
 		self.opened_at = opened_at
-		self.closed_at = closed_at
 
 ENDING_SCHEMA = {
 	'value': ar.Any,
 	'opened_ipp': ar.UserDefined(HostPort),
+	'opened_at': ar.WorldTime(),
 	'condition': ar.Unicode(),
 	'explanation': ar.Unicode(),
-	'exit_code': ar.Integer8(),
 	'error_code': ar.Integer8(),
-	'opened_at': ar.WorldTime(),
-	'closed_at': ar.WorldTime(),
+	'error_text': ar.Unicode(),
+	'exit_code': ar.Integer8(),
 }
 
 ar.bind(Close, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Closed, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 ar.bind(Abandoned, object_schema=ENDING_SCHEMA, copy_before_sending=False)
 
 #
@@ -1116,22 +1097,20 @@
 	else:
 		ipp = None
 
 	if stream.closing:
 		c = Closed(value=stream.value,
 			reason=reason,
 			opened_ipp=ipp,
-			opened_at=stream.opened.opened_at,
-			closed_at=ar.world_now())
+			opened_at=stream.opened.opened_at)
 		self.forward(c, stream.controller_address, stream.remote_address)
 	else:
 		self.send(ar.Stop(), stream.remote_address)
 		a = Abandoned(opened_ipp=ipp,
-			opened_at=stream.opened.opened_at,
-			closed_at=ar.world_now())
+			opened_at=stream.opened.opened_at)
 		self.forward(a, stream.controller_address, stream.remote_address)
 	self.clear(s, TcpStream)
 
 def TcpStream_ReadyToSend(self, stream, s):
 	try:
 		if stream.send_a_block(s):
 			return
```

### Comparing `ansar_connect-0.1.217/src/ansar/connect/standard.py` & `ansar_connect-0.1.221/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/transporting.py` & `ansar_connect-0.1.221/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.221/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar/connect/wan.py` & `ansar_connect-0.1.221/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.217/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.221/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.217
+Version: 0.1.221
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.217/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.221/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*


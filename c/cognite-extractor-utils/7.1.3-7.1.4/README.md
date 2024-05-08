# Comparing `tmp/cognite_extractor_utils-7.1.3.tar.gz` & `tmp/cognite_extractor_utils-7.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-7.1.3.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-7.1.4.tar", max compression
```

## Comparing `cognite_extractor_utils-7.1.3.tar` & `cognite_extractor_utils-7.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10173 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/LICENSE
--rw-r--r--   0        0        0     4090 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/README.md
--rw-r--r--   0        0        0      739 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1558 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0    16148 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/base.py
--rw-r--r--   0        0        0     3059 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/__init__.py
--rw-r--r--   0        0        0     4739 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/_util.py
--rw-r--r--   0        0        0    21334 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/elements.py
--rw-r--r--   0        0        0    16317 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/loaders.py
--rw-r--r--   0        0        0     1084 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0    15509 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0        0 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0    18645 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     3605 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/threading.py
--rw-r--r--   0        0        0     3110 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/__init__.py
--rw-r--r--   0        0        0     5282 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/_base.py
--rw-r--r--   0        0        0     3247 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/_metrics.py
--rw-r--r--   0        0        0     5628 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/assets.py
--rw-r--r--   0        0        0     5680 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/events.py
--rw-r--r--   0        0        0    18417 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/files.py
--rw-r--r--   0        0        0     6738 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/raw.py
--rw-r--r--   0        0        0    26817 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/time_series.py
--rw-r--r--   0        0        0     7732 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1020 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0    17198 2024-05-06 08:50:33.616455 cognite_extractor_utils-7.1.3/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2088 2024-05-06 08:50:33.620455 cognite_extractor_utils-7.1.3/pyproject.toml
--rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.1.3/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/LICENSE
+-rw-r--r--   0        0        0     4090 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/README.md
+-rw-r--r--   0        0        0      739 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1558 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    16391 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     3059 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4739 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    21564 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0    16317 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1084 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    15509 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0        0 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0    18667 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     3605 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/threading.py
+-rw-r--r--   0        0        0     3110 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     5304 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     3247 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     5628 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/assets.py
+-rw-r--r--   0        0        0     5680 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    18417 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     6738 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    26817 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7732 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1020 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    17198 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     2088 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.1.4/PKG-INFO
```

### Comparing `cognite_extractor_utils-7.1.3/LICENSE` & `cognite_extractor_utils-7.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/README.md` & `cognite_extractor_utils-7.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "7.1.3"
+__version__ = "7.1.4"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/base.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,17 +185,25 @@
                         return res
                 if isinstance(d[k], StateStoreConfig):
                     return d[k]
             return None
 
         state_store_config = recursive_find_state_store(self.config.__dict__)
         if state_store_config:
-            self.state_store = state_store_config.create_state_store(self.cognite_client, self.use_default_state_store)
+            self.state_store = state_store_config.create_state_store(
+                cdf_client=self.cognite_client,
+                default_to_local=self.use_default_state_store,
+                cancellation_token=self.cancellation_token,
+            )
         else:
-            self.state_store = LocalStateStore("states.json") if self.use_default_state_store else NoStateStore()
+            self.state_store = (
+                LocalStateStore("states.json", cancellation_token=self.cancellation_token)
+                if self.use_default_state_store
+                else NoStateStore()
+            )
 
         try:
             self.state_store.initialize()
         except ValueError:
             self.logger.exception("Could not load state store, using an empty state store as default")
 
         Extractor._statestore_singleton = self.state_store
```

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/__init__.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/_util.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/elements.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -619,15 +619,18 @@
     Configuration of the State Store, containing ``LocalStateStoreConfig`` or ``RawStateStoreConfig``
     """
 
     raw: Optional[RawStateStoreConfig] = None
     local: Optional[LocalStateStoreConfig] = None
 
     def create_state_store(
-        self, cdf_client: Optional[CogniteClient] = None, default_to_local: bool = True
+        self,
+        cdf_client: Optional[CogniteClient] = None,
+        default_to_local: bool = True,
+        cancellation_token: Optional[CancellationToken] = None,
     ) -> AbstractStateStore:
         """
         Create a state store object based on the config.
 
         Args:
             cdf_client: CogniteClient object to use in case of a RAW state store (ignored otherwise)
             default_to_local: If true, return a LocalStateStore if no state store is configured. Otherwise return a
@@ -644,19 +647,21 @@
                 raise TypeError("A cognite client object must be provided when state store is RAW")
 
             return RawStateStore(
                 cdf_client=cdf_client,
                 database=self.raw.database,
                 table=self.raw.table,
                 save_interval=self.raw.upload_interval.seconds,
+                cancellation_token=cancellation_token,
             )
 
         if self.local:
             return LocalStateStore(
                 file_path=self.local.path,
                 save_interval=self.local.save_interval.seconds,
+                cancellation_token=cancellation_token,
             )
 
         if default_to_local:
-            return LocalStateStore(file_path="states.json")
+            return LocalStateStore(file_path="states.json", cancellation_token=cancellation_token)
         else:
             return NoStateStore()
```

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/configtools/loaders.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/loaders.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/statestore.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         self._initialized = False
         self._local_state: Dict[str, Dict[str, Any]] = {}
         self.save_interval = save_interval
         self.trigger_log_level = _resolve_log_level(trigger_log_level)
 
         self.logger = logging.getLogger(__name__)
 
-        self.thread = threading.Thread(target=self._run, daemon=True, name=thread_name)
+        self.thread = threading.Thread(target=self._run, daemon=cancellation_token is None, name=thread_name)
         self.lock = threading.RLock()
         self.cancellation_token = cancellation_token.create_child_token() if cancellation_token else CancellationToken()
 
         self._deleted: List[str] = []
 
     def start(self, initialize: bool = True) -> None:
         """
```

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/threading.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/threading.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/__init__.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/_base.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         self.threshold = max_queue_size if max_queue_size is not None else -1
         self.upload_queue_size = 0
 
         self.trigger_log_level = _resolve_log_level(trigger_log_level)
         self.logger = logging.getLogger(__name__)
 
-        self.thread = threading.Thread(target=self._run, daemon=True, name=thread_name)
+        self.thread = threading.Thread(target=self._run, daemon=cancellation_token is None, name=thread_name)
         self.lock = threading.RLock()
         self.cancellation_token: CancellationToken = (
             cancellation_token.create_child_token() if cancellation_token else CancellationToken()
         )
 
         self.max_upload_interval = max_upload_interval
```

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/_metrics.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/_metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/assets.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/events.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/events.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/files.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/files.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/raw.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader/time_series.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/cognite/extractorutils/util.py` & `cognite_extractor_utils-7.1.4/cognite/extractorutils/util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.3/pyproject.toml` & `cognite_extractor_utils-7.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "7.1.3"
+version = "7.1.4"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
```

### Comparing `cognite_extractor_utils-7.1.3/PKG-INFO` & `cognite_extractor_utils-7.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 7.1.3
+Version: 7.1.4
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.1.3 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.1.4 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```


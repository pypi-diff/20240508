# Comparing `tmp/jupyter_server_ydoc-1.0.0a1.tar.gz` & `tmp/jupyter_server_ydoc-1.0.0a2.tar.gz`

## Comparing `jupyter_server_ydoc-1.0.0a1.tar` & `jupyter_server_ydoc-1.0.0a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/setup.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter-config/jupyter_server_ydoc.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/_version.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/app.py
--rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/handlers.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/loaders.py
--rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/rooms.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/stores.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/utils.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/websocketserver.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/events/awareness.yaml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/events/session.yaml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/__init__.py
--rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/conftest.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_app.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_documents.py
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_handlers.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_loaders.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/test_rooms.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/tests/utils.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/LICENSE
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/README.md
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/setup.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter-config/jupyter_server_ydoc.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/_version.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/app.py
+-rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/handlers.py
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/loaders.py
+-rw-r--r--   0        0        0    11671 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/rooms.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/stores.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/utils.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/websocketserver.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/events/awareness.yaml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/events/session.yaml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/tests/__init__.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/tests/conftest.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/tests/test_app.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/tests/test_documents.py
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/tests/test_handlers.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/tests/test_loaders.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/tests/test_rooms.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/tests/utils.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/README.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a2/PKG-INFO
```

### Comparing `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/app.py` & `jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,21 +87,17 @@
                 "collaborative_document_cleanup_delay": self.document_cleanup_delay,
                 "collaborative_document_save_delay": self.document_save_delay,
                 "collaborative_ystore_class": self.ystore_class,
             }
         )
 
     def initialize_handlers(self):
-        self.serverapp.web_app.settings.setdefault(
-            "page_config_data",
-            {
-                "disableRTC": self.disable_rtc,
-                "serverSideExecution": self.server_side_execution,
-            },
-        )
+        page_config = self.serverapp.web_app.settings.setdefault("page_config_data", {})
+        page_config.setdefault("disableRTC", self.disable_rtc)
+        page_config.setdefault("serverSideExecution", self.server_side_execution)
 
         # Set configurable parameters to YStore class
         for k, v in self.config.get(self.ystore_class.__name__, {}).items():
             setattr(self.ystore_class, k, v)
 
         self.ywebsocket_server = JupyterWebsocketServer(
             rooms_ready=False,
```

### Comparing `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/handlers.py` & `jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/loaders.py` & `jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/loaders.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/rooms.py` & `jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/rooms.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 YFILE = YDOCS["file"]
 
 
 class DocumentRoom(YRoom):
     """A Y room for a possibly stored document (e.g. a notebook)."""
 
+    _background_tasks: set[asyncio.Task]
+
     def __init__(
         self,
         room_id: str,
         file_format: str,
         file_type: str,
         file: FileLoader,
         logger: EventLogger,
@@ -44,14 +46,15 @@
         self._logger = logger
         self._save_delay = save_delay
 
         self._update_lock = asyncio.Lock()
         self._cleaner: asyncio.Task | None = None
         self._saving_document: asyncio.Task | None = None
         self._messages: dict[str, asyncio.Lock] = {}
+        self._background_tasks = set()
 
         # Listen for document changes
         self._document.observe(self._on_document_change)
         self._file.observe(self.room_id, self._on_outofband_change)
 
     @property
     def room_id(self) -> str:
@@ -96,14 +99,18 @@
 
         model = await self._file.load_content(self._file_format, self._file_type)
 
         async with self._update_lock:
             # try to apply Y updates from the YStore for this document
             read_from_source = True
             if self.ystore is not None:
+                async with self.ystore.start_lock:
+                    if not self.ystore.started.is_set():
+                        self.create_task(self.ystore.start())
+                        await self.ystore.started.wait()
                 try:
                     await self.ystore.apply_updates(self.ydoc)
                     self._emit(
                         LogLevel.INFO,
                         "load",
                         "Content loaded from the store {}".format(
                             self.ystore.__class__.__qualname__
@@ -173,14 +180,19 @@
         # TODO: Should we cancel or wait ?
         if self._saving_document:
             self._saving_document.cancel()
 
         self._document.unobserve()
         self._file.unobserve(self.room_id)
 
+    def create_task(self, aw):
+        task = asyncio.create_task(aw)
+        self._background_tasks.add(task)
+        task.add_done_callback(self._background_tasks.discard)
+
     async def _broadcast_updates(self):
         # FIXME should be upstreamed
         try:
             await super()._broadcast_updates()
         except asyncio.CancelledError:
             pass
```

### Comparing `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/stores.py` & `jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/stores.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/utils.py` & `jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/websocketserver.py` & `jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/websocketserver.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/events/awareness.yaml` & `jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/events/awareness.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/jupyter_server_ydoc/events/session.yaml` & `jupyter_server_ydoc-1.0.0a2/jupyter_server_ydoc/events/session.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/tests/conftest.py` & `jupyter_server_ydoc-1.0.0a2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 from __future__ import annotations
 
 import json
-from asyncio import Event, sleep
+from asyncio import Event, create_task, sleep
 from datetime import datetime
 from typing import Any
 
 import nbformat
 import pytest
 from jupyter_server_ydoc.loaders import FileLoader
 from jupyter_server_ydoc.rooms import DocumentRoom
@@ -172,15 +172,16 @@
 @pytest.fixture
 def rtc_create_SQLite_store(jp_serverapp):
     for k, v in jp_serverapp.config.get("SQLiteYStore").items():
         setattr(SQLiteYStore, k, v)
 
     async def _inner(type: str, path: str, content: str) -> DocumentRoom:
         db = SQLiteYStore(path=f"{type}:{path}")
-        await db.start()
+        task = create_task(db.start())
+        await db.started.wait()
 
         if type == "notebook":
             doc = YNotebook()
         else:
             doc = YUnicode()
 
         doc.source = content
```

### Comparing `jupyter_server_ydoc-1.0.0a1/tests/test_app.py` & `jupyter_server_ydoc-1.0.0a2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/tests/test_documents.py` & `jupyter_server_ydoc-1.0.0a2/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/tests/test_handlers.py` & `jupyter_server_ydoc-1.0.0a2/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/tests/test_loaders.py` & `jupyter_server_ydoc-1.0.0a2/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/tests/test_rooms.py` & `jupyter_server_ydoc-1.0.0a2/tests/test_rooms.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/tests/utils.py` & `jupyter_server_ydoc-1.0.0a2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/.gitignore` & `jupyter_server_ydoc-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/LICENSE` & `jupyter_server_ydoc-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-1.0.0a1/pyproject.toml` & `jupyter_server_ydoc-1.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 authors = [
     { name = "Jupyter Development Team", email = "jupyter@googlegroups.com" },
 ]
 dependencies = [
     "jupyter_server>=2.4.0,<3.0.0",
     "jupyter_ydoc>=2.0.0,<3.0.0",
-    "pycrdt-websocket>=0.13.1,<0.14.0",
+    "pycrdt-websocket>=0.13.4,<0.14.0",
     "jupyter_events>=0.10.0",
     "jupyter_server_fileid>=0.7.0,<1",
     "jsonschema>=4.18.0"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
```

### Comparing `jupyter_server_ydoc-1.0.0a1/PKG-INFO` & `jupyter_server_ydoc-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyter-server-ydoc
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: jupyter-server extension integrating collaborative shared models.
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
         This project is licensed under the terms of the Modified BSD License
         (also known as New or Revised or 3-Clause BSD), as follows:
         
@@ -76,15 +76,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: jsonschema>=4.18.0
 Requires-Dist: jupyter-events>=0.10.0
 Requires-Dist: jupyter-server-fileid<1,>=0.7.0
 Requires-Dist: jupyter-server<3.0.0,>=2.4.0
 Requires-Dist: jupyter-ydoc<3.0.0,>=2.0.0
-Requires-Dist: pycrdt-websocket<0.14.0,>=0.13.1
+Requires-Dist: pycrdt-websocket<0.14.0,>=0.13.4
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: importlib-metadata>=4.8.3; (python_version < '3.10') and extra == 'test'
 Requires-Dist: jupyter-server-fileid[test]; extra == 'test'
 Requires-Dist: jupyter-server[test]>=2.4.0; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
```


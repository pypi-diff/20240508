# Comparing `tmp/langgraph_sdk-0.1.1.tar.gz` & `tmp/langgraph_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_sdk-0.1.1.tar", max compression
+gzip compressed data, was "langgraph_sdk-0.1.2.tar", max compression
```

## Comparing `langgraph_sdk-0.1.1.tar` & `langgraph_sdk-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.778092 langgraph_sdk-0.1.1/README.md
--rw-r--r--   0        0        0       70 2024-05-02 17:41:01.189167 langgraph_sdk-0.1.1/langgraph_sdk/__init__.py
--rw-r--r--   0        0        0     9502 2024-05-03 18:22:21.613751 langgraph_sdk-0.1.1/langgraph_sdk/client.py
--rw-r--r--   0        0        0     3212 2024-05-03 18:21:58.272136 langgraph_sdk-0.1.1/langgraph_sdk/schema.py
--rw-r--r--   0        0        0     1005 2024-05-03 18:43:24.611307 langgraph_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.778092 langgraph_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0       70 2024-05-02 17:41:01.189167 langgraph_sdk-0.1.2/langgraph_sdk/__init__.py
+-rw-r--r--   0        0        0     9616 2024-05-08 02:00:16.426112 langgraph_sdk-0.1.2/langgraph_sdk/client.py
+-rw-r--r--   0        0        0     3212 2024-05-03 18:21:58.272136 langgraph_sdk-0.1.2/langgraph_sdk/schema.py
+-rw-r--r--   0        0        0     1005 2024-05-08 02:02:04.243805 langgraph_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.2/PKG-INFO
```

### Comparing `langgraph_sdk-0.1.1/langgraph_sdk/client.py` & `langgraph_sdk-0.1.2/langgraph_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,24 +183,31 @@
             json={"metadata": metadata, "limit": limit, "offset": offset},
         )
 
     async def get_state(self, thread_id: str) -> dict:
         """Get the state of a thread."""
         return await self.http.get(f"/threads/{thread_id}/state")
 
-    async def update_state(self, thread_id: Union[str, Config], values: dict) -> None:
+    async def update_state(
+        self,
+        thread_id: Union[str, Config],
+        values: dict,
+        *,
+        as_node: Optional[str] = None,
+    ) -> None:
         """Update the state of a thread."""
         if isinstance(thread_id, dict):
             config = thread_id
             thread_id_: str = thread_id["configurable"]["thread_id"]
         else:
             thread_id_ = thread_id
             config = None
         return await self.http.post(
-            f"/threads/{thread_id_}/state", json={"values": values, "config": config}
+            f"/threads/{thread_id_}/state",
+            json={"values": values, "config": config, "as_node": as_node},
         )
 
     async def get_history(
         self, thread_id: str, limit: int = 10, before: Optional[Config] = None
     ) -> list[dict]:
         """Get the history of a thread."""
         return await self.http.get(
```

### Comparing `langgraph_sdk-0.1.1/langgraph_sdk/schema.py` & `langgraph_sdk-0.1.2/langgraph_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `langgraph_sdk-0.1.1/pyproject.toml` & `langgraph_sdk-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-sdk"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9.0,<3.12"
```

### Comparing `langgraph_sdk-0.1.1/PKG-INFO` & `langgraph_sdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langgraph-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Nuno Campos
 Author-email: nuno@langchain.dev
 Requires-Python: >=3.9.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


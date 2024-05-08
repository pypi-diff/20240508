# Comparing `tmp/llama_index_embeddings_nvidia-0.1.0.tar.gz` & `tmp/llama_index_embeddings_nvidia-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_nvidia-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_embeddings_nvidia-0.1.1.tar", max compression
```

## Comparing `llama_index_embeddings_nvidia-0.1.0.tar` & `llama_index_embeddings_nvidia-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      694 2024-05-03 18:14:51.642844 llama_index_embeddings_nvidia-0.1.0/README.md
--rw-r--r--   0        0        0       94 2024-05-03 18:14:51.642844 llama_index_embeddings_nvidia-0.1.0/llama_index/embeddings/nvidia/__init__.py
--rw-r--r--   0        0        0     6505 2024-05-03 18:14:51.642844 llama_index_embeddings_nvidia-0.1.0/llama_index/embeddings/nvidia/base.py
--rw-r--r--   0        0        0     1533 2024-05-03 18:14:51.642844 llama_index_embeddings_nvidia-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 llama_index_embeddings_nvidia-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      694 2024-05-08 14:33:52.759347 llama_index_embeddings_nvidia-0.1.1/README.md
+-rw-r--r--   0        0        0       94 2024-05-08 14:33:52.759347 llama_index_embeddings_nvidia-0.1.1/llama_index/embeddings/nvidia/__init__.py
+-rw-r--r--   0        0        0     6584 2024-05-08 14:33:52.759347 llama_index_embeddings_nvidia-0.1.1/llama_index/embeddings/nvidia/base.py
+-rw-r--r--   0        0        0     1578 2024-05-08 14:33:52.759347 llama_index_embeddings_nvidia-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1253 1970-01-01 00:00:00.000000 llama_index_embeddings_nvidia-0.1.1/PKG-INFO
```

### Comparing `llama_index_embeddings_nvidia-0.1.0/README.md` & `llama_index_embeddings_nvidia-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_nvidia-0.1.0/llama_index/embeddings/nvidia/base.py` & `llama_index_embeddings_nvidia-0.1.1/llama_index/embeddings/nvidia/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,26 +157,28 @@
         )
 
     def _get_text_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Get text embeddings."""
         assert len(texts) <= 259, "The batch size should not be larger than 259."
 
         data = self._client.embeddings.create(
-            input=texts, model=self.model, extra_body={"input_type": "passage"}
+            input=texts,
+            model=self.model,
+            extra_body={"input_type": "passage", "truncate": self.truncate},
         ).data
         return [d.embedding for d in data]
 
     async def _aget_query_embedding(self, query: str) -> List[float]:
         """Asynchronously get query embedding."""
         return (
             (
                 await self._aclient.embeddings.create(
                     input=[query],
                     model=self.model,
-                    extra_body={"input_type": "query"},
+                    extra_body={"input_type": "query", "truncate": self.truncate},
                 )
             )
             .data[0]
             .embedding
         )
 
     async def _aget_text_embedding(self, text: str) -> List[float]:
```

### Comparing `llama_index_embeddings_nvidia-0.1.0/pyproject.toml` & `llama_index_embeddings_nvidia-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,28 +23,30 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings nvidia integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-nvidia"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.9"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
 pytest = "7.2.1"
+pytest-asyncio = "^0.23.6"
 pytest-mock = "3.11.1"
+respx = "^0.21.1"
 ruff = "0.0.292"
 tree-sitter-languages = "^1.8.0"
 types-Deprecated = ">=0.1.0"
 types-PyYAML = "^6.0.12.12"
 types-protobuf = "^4.24.0.4"
 types-redis = "4.5.5.0"
 types-requests = "2.28.11.8"
```

### Comparing `llama_index_embeddings_nvidia-0.1.0/PKG-INFO` & `llama_index_embeddings_nvidia-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-nvidia
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index embeddings nvidia integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


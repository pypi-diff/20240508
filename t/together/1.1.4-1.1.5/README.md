# Comparing `tmp/together-1.1.4.tar.gz` & `tmp/together-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together-1.1.4.tar", max compression
+gzip compressed data, was "together-1.1.5.tar", max compression
```

## Comparing `together-1.1.4.tar` & `together-1.1.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-05-03 03:50:53.189128 together-1.1.4/LICENSE
--rw-r--r--   0        0        0    10365 2024-05-03 03:50:53.189128 together-1.1.4/README.md
--rw-r--r--   0        0        0     2590 2024-05-03 03:50:53.189128 together-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1401 2024-05-03 03:50:53.189128 together-1.1.4/src/together/__init__.py
--rw-r--r--   0        0        0       57 2024-05-03 03:50:53.189128 together-1.1.4/src/together/abstract/__init__.py
--rw-r--r--   0        0        0    25103 2024-05-03 03:50:53.189128 together-1.1.4/src/together/abstract/api_requestor.py
--rw-r--r--   0        0        0        0 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/__init__.py
--rw-r--r--   0        0        0     9170 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/chat.py
--rw-r--r--   0        0        0     4199 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/completions.py
--rw-r--r--   0        0        0     3186 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/files.py
--rw-r--r--   0        0        0     5417 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/finetune.py
--rw-r--r--   0        0        0     2363 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/images.py
--rw-r--r--   0        0        0     1126 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/api/models.py
--rw-r--r--   0        0        0     1977 2024-05-03 03:50:53.189128 together-1.1.4/src/together/cli/cli.py
--rw-r--r--   0        0        0     4774 2024-05-03 03:50:53.189128 together-1.1.4/src/together/client.py
--rw-r--r--   0        0        0      908 2024-05-03 03:50:53.189128 together-1.1.4/src/together/constants.py
--rw-r--r--   0        0        0     5329 2024-05-03 03:50:53.189128 together-1.1.4/src/together/error.py
--rw-r--r--   0        0        0    11438 2024-05-03 03:50:53.189128 together-1.1.4/src/together/filemanager.py
--rw-r--r--   0        0        0        0 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/__init__.py
--rw-r--r--   0        0        0      727 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/base.py
--rw-r--r--   0        0        0     2343 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/complete.py
--rw-r--r--   0        0        0      591 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/embeddings.py
--rw-r--r--   0        0        0     3863 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/files.py
--rw-r--r--   0        0        0     4917 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/finetune.py
--rw-r--r--   0        0        0      582 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/images.py
--rw-r--r--   0        0        0     1053 2024-05-03 03:50:53.189128 together-1.1.4/src/together/legacy/models.py
--rw-r--r--   0        0        0      701 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/__init__.py
--rw-r--r--   0        0        0      617 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/chat/__init__.py
--rw-r--r--   0        0        0    14084 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/chat/completions.py
--rw-r--r--   0        0        0    11353 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/completions.py
--rw-r--r--   0        0        0     2546 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/embeddings.py
--rw-r--r--   0        0        0     4593 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/files.py
--rw-r--r--   0        0        0    12416 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/finetune.py
--rw-r--r--   0        0        0     4775 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/images.py
--rw-r--r--   0        0        0     1786 2024-05-03 03:50:53.189128 together-1.1.4/src/together/resources/models.py
--rw-r--r--   0        0        0     1319 2024-05-03 03:50:53.189128 together-1.1.4/src/together/together_response.py
--rw-r--r--   0        0        0     1432 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/__init__.py
--rw-r--r--   0        0        0      642 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/abstract.py
--rw-r--r--   0        0        0     4335 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/chat_completions.py
--rw-r--r--   0        0        0     1491 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/common.py
--rw-r--r--   0        0        0     2887 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/completions.py
--rw-r--r--   0        0        0      751 2024-05-03 03:50:53.189128 together-1.1.4/src/together/types/embeddings.py
--rw-r--r--   0        0        0      370 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/error.py
--rw-r--r--   0        0        0     1954 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/files.py
--rw-r--r--   0        0        0     5775 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/finetune.py
--rw-r--r--   0        0        0      915 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/images.py
--rw-r--r--   0        0        0     1013 2024-05-03 03:50:53.193128 together-1.1.4/src/together/types/models.py
--rw-r--r--   0        0        0      662 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/__init__.py
--rw-r--r--   0        0        0     1665 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/_log.py
--rw-r--r--   0        0        0     2407 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/api_helpers.py
--rw-r--r--   0        0        0     7165 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/files.py
--rw-r--r--   0        0        0     1788 2024-05-03 03:50:53.193128 together-1.1.4/src/together/utils/tools.py
--rw-r--r--   0        0        0      126 2024-05-03 03:50:53.193128 together-1.1.4/src/together/version.py
--rw-r--r--   0        0        0    11812 1970-01-01 00:00:00.000000 together-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 02:38:09.291025 together-1.1.5/LICENSE
+-rw-r--r--   0        0        0    10365 2024-05-08 02:38:09.291025 together-1.1.5/README.md
+-rw-r--r--   0        0        0     2590 2024-05-08 02:38:09.291025 together-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1401 2024-05-08 02:38:09.291025 together-1.1.5/src/together/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-08 02:38:09.291025 together-1.1.5/src/together/abstract/__init__.py
+-rw-r--r--   0        0        0    25103 2024-05-08 02:38:09.291025 together-1.1.5/src/together/abstract/api_requestor.py
+-rw-r--r--   0        0        0        0 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/__init__.py
+-rw-r--r--   0        0        0     9170 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/chat.py
+-rw-r--r--   0        0        0     4199 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/completions.py
+-rw-r--r--   0        0        0     3186 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/files.py
+-rw-r--r--   0        0        0     5417 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/finetune.py
+-rw-r--r--   0        0        0     2363 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/images.py
+-rw-r--r--   0        0        0     1126 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/api/models.py
+-rw-r--r--   0        0        0     1977 2024-05-08 02:38:09.291025 together-1.1.5/src/together/cli/cli.py
+-rw-r--r--   0        0        0     4774 2024-05-08 02:38:09.291025 together-1.1.5/src/together/client.py
+-rw-r--r--   0        0        0      908 2024-05-08 02:38:09.291025 together-1.1.5/src/together/constants.py
+-rw-r--r--   0        0        0     5329 2024-05-08 02:38:09.295025 together-1.1.5/src/together/error.py
+-rw-r--r--   0        0        0    11269 2024-05-08 02:38:09.295025 together-1.1.5/src/together/filemanager.py
+-rw-r--r--   0        0        0        0 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/base.py
+-rw-r--r--   0        0        0     2343 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/complete.py
+-rw-r--r--   0        0        0      591 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/embeddings.py
+-rw-r--r--   0        0        0     3863 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/files.py
+-rw-r--r--   0        0        0     4917 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/finetune.py
+-rw-r--r--   0        0        0      582 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/images.py
+-rw-r--r--   0        0        0     1053 2024-05-08 02:38:09.295025 together-1.1.5/src/together/legacy/models.py
+-rw-r--r--   0        0        0      701 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/__init__.py
+-rw-r--r--   0        0        0      617 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/chat/__init__.py
+-rw-r--r--   0        0        0    14084 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/chat/completions.py
+-rw-r--r--   0        0        0    11353 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/completions.py
+-rw-r--r--   0        0        0     2546 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/embeddings.py
+-rw-r--r--   0        0        0     4593 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/files.py
+-rw-r--r--   0        0        0    12416 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/finetune.py
+-rw-r--r--   0        0        0     4775 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/images.py
+-rw-r--r--   0        0        0     1786 2024-05-08 02:38:09.295025 together-1.1.5/src/together/resources/models.py
+-rw-r--r--   0        0        0     1319 2024-05-08 02:38:09.295025 together-1.1.5/src/together/together_response.py
+-rw-r--r--   0        0        0     1432 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/__init__.py
+-rw-r--r--   0        0        0      642 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/abstract.py
+-rw-r--r--   0        0        0     4335 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/chat_completions.py
+-rw-r--r--   0        0        0     1491 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/common.py
+-rw-r--r--   0        0        0     2887 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/completions.py
+-rw-r--r--   0        0        0      751 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/embeddings.py
+-rw-r--r--   0        0        0      370 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/error.py
+-rw-r--r--   0        0        0     1954 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/files.py
+-rw-r--r--   0        0        0     5775 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/finetune.py
+-rw-r--r--   0        0        0      915 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/images.py
+-rw-r--r--   0        0        0     1013 2024-05-08 02:38:09.295025 together-1.1.5/src/together/types/models.py
+-rw-r--r--   0        0        0      662 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1665 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/_log.py
+-rw-r--r--   0        0        0     2407 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/api_helpers.py
+-rw-r--r--   0        0        0     7165 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/files.py
+-rw-r--r--   0        0        0     1788 2024-05-08 02:38:09.295025 together-1.1.5/src/together/utils/tools.py
+-rw-r--r--   0        0        0      126 2024-05-08 02:38:09.295025 together-1.1.5/src/together/version.py
+-rw-r--r--   0        0        0    11812 1970-01-01 00:00:00.000000 together-1.1.5/PKG-INFO
```

### Comparing `together-1.1.4/LICENSE` & `together-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `together-1.1.4/README.md` & `together-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `together-1.1.4/pyproject.toml` & `together-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "oldest-supported-numpy>=0.14; python_version<'3.9'",
     "numpy>=1.25; python_version>='3.9'",
 ]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "together"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
     "Together AI <support@together.ai>"
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `together-1.1.4/src/together/__init__.py` & `together-1.1.5/src/together/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/abstract/api_requestor.py` & `together-1.1.5/src/together/abstract/api_requestor.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/cli/api/chat.py` & `together-1.1.5/src/together/cli/api/chat.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/cli/api/completions.py` & `together-1.1.5/src/together/cli/api/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/cli/api/files.py` & `together-1.1.5/src/together/cli/api/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/cli/api/finetune.py` & `together-1.1.5/src/together/cli/api/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/cli/api/images.py` & `together-1.1.5/src/together/cli/api/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/cli/api/models.py` & `together-1.1.5/src/together/cli/api/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/cli/cli.py` & `together-1.1.5/src/together/cli/cli.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/client.py` & `together-1.1.5/src/together/client.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/constants.py` & `together-1.1.5/src/together/constants.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/error.py` & `together-1.1.5/src/together/error.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/filemanager.py` & `together-1.1.5/src/together/filemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,21 +99,16 @@
 
     if step > 0:
         remote_name += f"-checkpoint-{step}"
 
     if "x-tar" in content_type.lower():
         remote_name += ".tar.gz"
 
-    elif "zstd" in content_type.lower() or step != -1:
-        remote_name += ".tar.zst"
-
     else:
-        raise FileTypeError(
-            f"Unknown file type {content_type} found. Aborting download."
-        )
+        remote_name += ".tar.zst"
 
     return Path(remote_name)
 
 
 class DownloadManager:
     def __init__(self, client: TogetherClient) -> None:
         self._client = client
```

### Comparing `together-1.1.4/src/together/legacy/base.py` & `together-1.1.5/src/together/legacy/base.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/legacy/complete.py` & `together-1.1.5/src/together/legacy/complete.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/legacy/embeddings.py` & `together-1.1.5/src/together/legacy/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/legacy/files.py` & `together-1.1.5/src/together/legacy/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/legacy/finetune.py` & `together-1.1.5/src/together/legacy/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/legacy/images.py` & `together-1.1.5/src/together/legacy/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/legacy/models.py` & `together-1.1.5/src/together/legacy/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/resources/__init__.py` & `together-1.1.5/src/together/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/resources/chat/__init__.py` & `together-1.1.5/src/together/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/resources/chat/completions.py` & `together-1.1.5/src/together/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/resources/completions.py` & `together-1.1.5/src/together/resources/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/resources/embeddings.py` & `together-1.1.5/src/together/resources/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/resources/files.py` & `together-1.1.5/src/together/resources/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/resources/finetune.py` & `together-1.1.5/src/together/resources/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/resources/images.py` & `together-1.1.5/src/together/resources/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/resources/models.py` & `together-1.1.5/src/together/resources/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/together_response.py` & `together-1.1.5/src/together/together_response.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/__init__.py` & `together-1.1.5/src/together/types/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/abstract.py` & `together-1.1.5/src/together/types/abstract.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/chat_completions.py` & `together-1.1.5/src/together/types/chat_completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/common.py` & `together-1.1.5/src/together/types/common.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/completions.py` & `together-1.1.5/src/together/types/completions.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/embeddings.py` & `together-1.1.5/src/together/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/files.py` & `together-1.1.5/src/together/types/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/finetune.py` & `together-1.1.5/src/together/types/finetune.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/images.py` & `together-1.1.5/src/together/types/images.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/types/models.py` & `together-1.1.5/src/together/types/models.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/utils/__init__.py` & `together-1.1.5/src/together/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/utils/_log.py` & `together-1.1.5/src/together/utils/_log.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/utils/api_helpers.py` & `together-1.1.5/src/together/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/utils/files.py` & `together-1.1.5/src/together/utils/files.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/src/together/utils/tools.py` & `together-1.1.5/src/together/utils/tools.py`

 * *Files identical despite different names*

### Comparing `together-1.1.4/PKG-INFO` & `together-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python client for Together's Cloud Platform!
 Home-page: https://github.com/togethercomputer/together-python
 License: Apache-2.0
 Author: Together AI
 Author-email: support@together.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: together Version: 1.1.4 Summary: Python client for
+Metadata-Version: 2.1 Name: together Version: 1.1.5 Summary: Python client for
 Together's Cloud Platform! Home-page: https://github.com/togethercomputer/
 together-python License: Apache-2.0 Author: Together AI Author-email:
 support@together.ai Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```


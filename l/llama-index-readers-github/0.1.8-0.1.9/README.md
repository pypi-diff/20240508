# Comparing `tmp/llama_index_readers_github-0.1.8.tar.gz` & `tmp/llama_index_readers_github-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_github-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_readers_github-0.1.9.tar", max compression
```

## Comparing `llama_index_readers_github-0.1.8.tar` & `llama_index_readers_github-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2113 2024-04-30 16:55:06.385854 llama_index_readers_github-0.1.8/README.md
--rw-r--r--   0        0        0      555 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/__init__.py
--rw-r--r--   0        0        0     5944 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/base.py
--rw-r--r--   0        0        0     5917 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/github_client.py
--rw-r--r--   0        0        0        0 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/issues/__init__.py
--rw-r--r--   0        0        0     7826 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/issues/base.py
--rw-r--r--   0        0        0     6496 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/issues/github_client.py
--rw-r--r--   0        0        0        0 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/repository/__init__.py
--rw-r--r--   0        0        0    21522 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/repository/base.py
--rw-r--r--   0        0        0    15377 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/repository/github_client.py
--rw-r--r--   0        0        0     5614 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/llama_index/readers/github/repository/utils.py
--rw-r--r--   0        0        0     1744 2024-04-30 16:55:06.389854 llama_index_readers_github-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 llama_index_readers_github-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2113 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/README.md
+-rw-r--r--   0        0        0      555 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/collaborators/__init__.py
+-rw-r--r--   0        0        0     5944 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/collaborators/base.py
+-rw-r--r--   0        0        0     5917 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/collaborators/github_client.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/issues/__init__.py
+-rw-r--r--   0        0        0     7826 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/issues/base.py
+-rw-r--r--   0        0        0     6496 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/issues/github_client.py
+-rw-r--r--   0        0        0        0 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/repository/__init__.py
+-rw-r--r--   0        0        0    21522 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/repository/base.py
+-rw-r--r--   0        0        0    15932 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/repository/github_client.py
+-rw-r--r--   0        0        0     5614 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/llama_index/readers/github/repository/utils.py
+-rw-r--r--   0        0        0     1744 2024-05-08 20:44:35.403685 llama_index_readers_github-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 llama_index_readers_github-0.1.9/PKG-INFO
```

### Comparing `llama_index_readers_github-0.1.8/README.md` & `llama_index_readers_github-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.8/llama_index/readers/github/__init__.py` & `llama_index_readers_github-0.1.9/llama_index/readers/github/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/base.py` & `llama_index_readers_github-0.1.9/llama_index/readers/github/collaborators/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.8/llama_index/readers/github/collaborators/github_client.py` & `llama_index_readers_github-0.1.9/llama_index/readers/github/collaborators/github_client.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.8/llama_index/readers/github/issues/base.py` & `llama_index_readers_github-0.1.9/llama_index/readers/github/issues/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.8/llama_index/readers/github/issues/github_client.py` & `llama_index_readers_github-0.1.9/llama_index/readers/github/issues/github_client.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.8/llama_index/readers/github/repository/base.py` & `llama_index_readers_github-0.1.9/llama_index/readers/github/repository/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.8/llama_index/readers/github/repository/github_client.py` & `llama_index_readers_github-0.1.9/llama_index/readers/github/repository/github_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import os
 
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional, Protocol
 
 from dataclasses_json import DataClassJsonMixin, config
+from httpx import HTTPError
 
 
 @dataclass
 class GitTreeResponseModel(DataClassJsonMixin):
     """
     Dataclass for the response from the Github API's getTree endpoint.
 
@@ -217,25 +218,28 @@
 
     def __init__(
         self,
         github_token: Optional[str] = None,
         base_url: str = DEFAULT_BASE_URL,
         api_version: str = DEFAULT_API_VERSION,
         verbose: bool = False,
+        fail_on_http_error: bool = True,
     ) -> None:
         """
         Initialize the GithubClient.
 
         Args:
             - github_token (str): Github token for authentication.
                 If not provided, the client will try to get it from
                 the GITHUB_TOKEN environment variable.
             - base_url (str): Base URL for the Github API
                 (defaults to "https://api.github.com").
             - api_version (str): Github API version (defaults to "2022-11-28").
+            - verbose (bool): Whether to print verbose output (defaults to False).
+            - fail_on_http_error (bool): Whether to raise an exception on HTTP errors (defaults to True).
 
         Raises:
             ValueError: If no Github token is provided.
         """
         if github_token is None:
             github_token = os.getenv("GITHUB_TOKEN")
             if github_token is None:
@@ -244,14 +248,15 @@
                     + "You can do so by passing it as an argument to the GithubReader,"
                     + "or by setting the GITHUB_TOKEN environment variable."
                 )
 
         self._base_url = base_url
         self._api_version = api_version
         self._verbose = verbose
+        self._fail_on_http_error = fail_on_http_error
 
         self._endpoints = {
             "getTree": "/repos/{owner}/{repo}/git/trees/{tree_sha}",
             "getBranch": "/repos/{owner}/{repo}/branches/{branch}",
             "getBlob": "/repos/{owner}/{repo}/git/blobs/{file_sha}",
             "getCommit": "/repos/{owner}/{repo}/commits/{commit_sha}",
         }
@@ -290,15 +295,15 @@
             - `**kwargs`: Keyword arguments to pass to the endpoint URL.
 
         Returns:
             - `response (httpx.Response)`: Response from the API request.
 
         Raises:
             - ImportError: If the `httpx` library is not installed.
-            - httpx.HTTPError: If the API request fails.
+            - httpx.HTTPError: If the API request fails and fail_on_http_error is True.
 
         Examples:
             >>> response = client.request("getTree", "GET",
                                 owner="owner", repo="repo",
                                 tree_sha="tree_sha", timeout=5, retries=0)
         """
         try:
@@ -447,14 +452,20 @@
                         retries=retries,
                     )
                 ).text
             )
         except KeyError:
             print(f"Failed to get blob for {owner}/{repo}/{file_sha}")
             return None
+        except HTTPError as excp:
+            print(f"HTTP Exception for {excp.request.url} - {excp}")
+            if self._fail_on_http_error:
+                raise
+            else:
+                return None
 
     async def get_commit(
         self,
         owner: str,
         repo: str,
         commit_sha: str,
         timeout: Optional[int] = 5,
```

### Comparing `llama_index_readers_github-0.1.8/llama_index/readers/github/repository/utils.py` & `llama_index_readers_github-0.1.9/llama_index/readers/github/repository/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_github-0.1.8/pyproject.toml` & `llama_index_readers_github-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 description = "llama-index readers github integration"
 exclude = ["**/BUILD"]
 keywords = ["code", "collaborators", "git", "github", "issues", "placeholder", "repository", "source code"]
 license = "MIT"
 maintainers = ["ahmetkca", "moncho", "rwood-97"]
 name = "llama-index-readers-github"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-readers-file = "^0.1.1"
 httpx = ">=0.26.0"
```

### Comparing `llama_index_readers_github-0.1.8/PKG-INFO` & `llama_index_readers_github-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-github
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index readers github integration
 License: MIT
 Keywords: code,collaborators,git,github,issues,placeholder,repository,source code
 Author: Your Name
 Author-email: you@example.com
 Maintainer: ahmetkca
 Requires-Python: >=3.8.1,<4.0
```


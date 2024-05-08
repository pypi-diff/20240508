# Comparing `tmp/zep_cloud-0.0.1rc1.tar.gz` & `tmp/zep_cloud-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_cloud-0.0.1rc1.tar", max compression
+gzip compressed data, was "zep_cloud-1.0.0rc1.tar", max compression
```

## Comparing `zep_cloud-0.0.1rc1.tar` & `zep_cloud-1.0.0rc1.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0     5078 2024-05-08 02:15:35.980426 zep_cloud-0.0.1rc1/README.md
--rw-r--r--   0        0        0      669 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0     1558 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/__init__.py
--rw-r--r--   0        0        0     6040 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/base_client.py
--rw-r--r--   0        0        0     2189 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/client.py
--rw-r--r--   0        0        0      853 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/api_error.py
--rw-r--r--   0        0        0     1495 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/core/request_options.py
--rw-r--r--   0        0        0       65 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/document/__init__.py
--rw-r--r--   0        0        0    93174 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/document/client.py
--rw-r--r--   0        0        0      158 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/environment.py
--rw-r--r--   0        0        0      352 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/errors/__init__.py
--rw-r--r--   0        0        0      356 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/errors/bad_request_error.py
--rw-r--r--   0        0        0      360 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/errors/internal_server_error.py
--rw-r--r--   0        0        0      354 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/errors/not_found_error.py
--rw-r--r--   0        0        0      358 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/errors/unauthorized_error.py
--rw-r--r--   0        0        0      569 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/external_clients/document.py
--rw-r--r--   0        0        0      551 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/external_clients/memory.py
--rw-r--r--   0        0        0      533 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/external_clients/user.py
--rw-r--r--   0        0        0      175 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/langchain/__init__.py
--rw-r--r--   0        0        0      374 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/langchain/helpers.py
--rw-r--r--   0        0        0     6828 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/langchain/history.py
--rw-r--r--   0        0        0    19612 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/langchain/vectorstore.py
--rw-r--r--   0        0        0      153 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/memory/__init__.py
--rw-r--r--   0        0        0   101464 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/memory/client.py
--rw-r--r--   0        0        0      178 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/memory/types/__init__.py
--rw-r--r--   0        0        0      208 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/memory/types/memory_get_request_memory_type.py
--rw-r--r--   0        0        0        0 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/py.typed
--rw-r--r--   0        0        0     1648 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/types/__init__.py
--rw-r--r--   0        0        0      872 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/types/api_error.py
--rw-r--r--   0        0        0     1044 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/types/classify_session_response.py
--rw-r--r--   0        0        0     1055 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/types/create_document_request.py
--rw-r--r--   0        0        0     1772 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/types/document_collection_response.py
--rw-r--r--   0        0        0     1342 2024-05-08 02:15:35.988426 zep_cloud-0.0.1rc1/src/zep/types/document_response.py
--rw-r--r--   0        0        0     1387 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/document_search_result.py
--rw-r--r--   0        0        0     1173 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/document_search_result_page.py
--rw-r--r--   0        0        0     1549 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/memory.py
--rw-r--r--   0        0        0     1155 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/memory_search_result.py
--rw-r--r--   0        0        0     2061 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/message.py
--rw-r--r--   0        0        0     1251 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/message_list_response.py
--rw-r--r--   0        0        0      962 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/models_zep_data_class.py
--rw-r--r--   0        0        0      873 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/question.py
--rw-r--r--   0        0        0      193 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/role_type.py
--rw-r--r--   0        0        0      158 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/search_scope.py
--rw-r--r--   0        0        0      155 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/search_type.py
--rw-r--r--   0        0        0     1564 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/session.py
--rw-r--r--   0        0        0      879 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/success_response.py
--rw-r--r--   0        0        0     1567 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/summary.py
--rw-r--r--   0        0        0     1019 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/summary_list_response.py
--rw-r--r--   0        0        0     1087 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/update_document_list_request.py
--rw-r--r--   0        0        0     1480 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/user.py
--rw-r--r--   0        0        0     1003 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/types/user_list_response.py
--rw-r--r--   0        0        0       65 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/user/__init__.py
--rw-r--r--   0        0        0    37780 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/user/client.py
--rw-r--r--   0        0        0       71 2024-05-08 02:15:35.992426 zep_cloud-0.0.1rc1/src/zep/version.py
--rw-r--r--   0        0        0     5576 1970-01-01 00:00:00.000000 zep_cloud-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     5078 2024-05-08 18:32:22.377254 zep_cloud-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      675 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1610 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/__init__.py
+-rw-r--r--   0        0        0     6052 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/base_client.py
+-rw-r--r--   0        0        0     2188 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/client.py
+-rw-r--r--   0        0        0      853 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/core/api_error.py
+-rw-r--r--   0        0        0     1501 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-08 18:32:22.385254 zep_cloud-1.0.0rc1/src/zep_cloud/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/document/__init__.py
+-rw-r--r--   0        0        0    93354 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/document/client.py
+-rw-r--r--   0        0        0      158 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/environment.py
+-rw-r--r--   0        0        0      352 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/bad_request_error.py
+-rw-r--r--   0        0        0      360 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/internal_server_error.py
+-rw-r--r--   0        0        0      354 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/not_found_error.py
+-rw-r--r--   0        0        0      358 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      581 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/document.py
+-rw-r--r--   0        0        0      563 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/memory.py
+-rw-r--r--   0        0        0      545 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/user.py
+-rw-r--r--   0        0        0      186 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/langchain/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/langchain/helpers.py
+-rw-r--r--   0        0        0     6905 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/langchain/history.py
+-rw-r--r--   0        0        0    19893 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/langchain/vectorstore.py
+-rw-r--r--   0        0        0      153 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/memory/__init__.py
+-rw-r--r--   0        0        0   101724 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/memory/client.py
+-rw-r--r--   0        0        0      178 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/memory/types/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/memory/types/memory_get_request_memory_type.py
+-rw-r--r--   0        0        0        0 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/py.typed
+-rw-r--r--   0        0        0     1730 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/api_error.py
+-rw-r--r--   0        0        0     1044 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/classify_session_response.py
+-rw-r--r--   0        0        0     1055 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/create_document_request.py
+-rw-r--r--   0        0        0     1772 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/document_collection_response.py
+-rw-r--r--   0        0        0     1342 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/document_response.py
+-rw-r--r--   0        0        0     1387 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/document_search_result.py
+-rw-r--r--   0        0        0     1173 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/document_search_result_page.py
+-rw-r--r--   0        0        0     1549 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/memory.py
+-rw-r--r--   0        0        0     1155 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/memory_search_result.py
+-rw-r--r--   0        0        0     2061 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/message.py
+-rw-r--r--   0        0        0     1251 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/message_list_response.py
+-rw-r--r--   0        0        0      962 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/models_zep_data_class.py
+-rw-r--r--   0        0        0      873 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/question.py
+-rw-r--r--   0        0        0      193 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/role_type.py
+-rw-r--r--   0        0        0      158 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/search_scope.py
+-rw-r--r--   0        0        0      155 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/search_type.py
+-rw-r--r--   0        0        0     1564 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/session.py
+-rw-r--r--   0        0        0     1023 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/session_list_response.py
+-rw-r--r--   0        0        0      879 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/success_response.py
+-rw-r--r--   0        0        0     1567 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/summary.py
+-rw-r--r--   0        0        0     1019 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/summary_list_response.py
+-rw-r--r--   0        0        0     1087 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/update_document_list_request.py
+-rw-r--r--   0        0        0     1480 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/user.py
+-rw-r--r--   0        0        0     1003 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/types/user_list_response.py
+-rw-r--r--   0        0        0       65 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/user/__init__.py
+-rw-r--r--   0        0        0    37852 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/user/client.py
+-rw-r--r--   0        0        0       77 2024-05-08 18:32:22.389254 zep_cloud-1.0.0rc1/src/zep_cloud/version.py
+-rw-r--r--   0        0        0     5576 1970-01-01 00:00:00.000000 zep_cloud-1.0.0rc1/PKG-INFO
```

### Comparing `zep_cloud-0.0.1rc1/README.md` & `zep_cloud-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/pyproject.toml` & `zep_cloud-1.0.0rc1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "zep-cloud"
-version = "0.0.1-rc.1"
+version = "1.0.0-rc.1"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
-    { include = "zep", from = "src"}
+    { include = "zep_cloud", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 httpx = ">=0.21.2"
 pydantic = ">= 1.9.2"
 typing_extensions = ">= 4.0.0"
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/__init__.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     MessageListResponse,
     ModelsZepDataClass,
     Question,
     RoleType,
     SearchScope,
     SearchType,
     Session,
+    SessionListResponse,
     SuccessResponse,
     Summary,
     SummaryListResponse,
     UpdateDocumentListRequest,
     User,
     UserListResponse,
 )
@@ -49,14 +50,15 @@
     "ModelsZepDataClass",
     "NotFoundError",
     "Question",
     "RoleType",
     "SearchScope",
     "SearchType",
     "Session",
+    "SessionListResponse",
     "SuccessResponse",
     "Summary",
     "SummaryListResponse",
     "UnauthorizedError",
     "UpdateDocumentListRequest",
     "User",
     "UserListResponse",
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/base_client.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
     httpx_client : typing.Optional[httpx.Client]
         The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
 
     Examples
     --------
-    from zep.client import Zep
+    from zep_cloud.client import Zep
 
     client = Zep(
         api_key="YOUR_API_KEY",
     )
     """
 
     def __init__(
@@ -104,15 +104,15 @@
         Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
     httpx_client : typing.Optional[httpx.AsyncClient]
         The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
 
     Examples
     --------
-    from zep.client import AsyncZep
+    from zep_cloud.client import AsyncZep
 
     client = AsyncZep(
         api_key="YOUR_API_KEY",
     )
     """
 
     def __init__(
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/client.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,8 @@
             api_key=api_key,
             timeout=timeout,
             follow_redirects=follow_redirects,
             httpx_client=httpx_client
         )
         self.memory = AsyncMemoryClient(client_wrapper=self._client_wrapper)
         self.document = AsyncDocumentClient(client_wrapper=self._client_wrapper)
-        self.user = AsyncUserClient(client_wrapper=self._client_wrapper)
+        self.user = AsyncUserClient(client_wrapper=self._client_wrapper)
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/core/__init__.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/core/__init__.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/core/client_wrapper.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
-            "X-Fern-SDK-Name": "zep",
+            "X-Fern-SDK-Name": "zep-cloud",
             "X-Fern-SDK-Version": "1.0.0",
         }
         headers["Authorization"] = f"Api-Key {self.api_key}"
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/core/datetime_utils.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/core/file.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/core/file.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/core/http_client.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/core/http_client.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/core/jsonable_encoder.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/core/request_options.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/core/request_options.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/document/client.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/document/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Returns
         -------
         typing.List[typing.List[DocumentCollectionResponse]]
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.list_collections()
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -109,15 +109,15 @@
         Returns
         -------
         DocumentCollectionResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.get_collection(
             collection_name="collectionName",
         )
@@ -190,15 +190,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.add_collection(
             collection_name="collectionName",
         )
@@ -273,15 +273,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.delete_collection(
             collection_name="collectionName",
         )
@@ -354,15 +354,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.update_collection(
             collection_name="collectionName",
         )
@@ -443,16 +443,16 @@
         Returns
         -------
         typing.List[str]
             OK
 
         Examples
         --------
-        from zep import CreateDocumentRequest
-        from zep.client import Zep
+        from zep_cloud import CreateDocumentRequest
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.add_documents(
             collection_name="collectionName",
             request=[CreateDocumentRequest()],
@@ -527,15 +527,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.batch_delete_documents(
             collection_name="collectionName",
             request=["string"],
@@ -614,15 +614,15 @@
         Returns
         -------
         typing.List[DocumentResponse]
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.batch_get_documents(
             collection_name="collectionName",
         )
@@ -702,16 +702,16 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep import UpdateDocumentListRequest
-        from zep.client import Zep
+        from zep_cloud import UpdateDocumentListRequest
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.batch_update_documents(
             collection_name="collectionName",
             request=[
@@ -788,15 +788,15 @@
         Returns
         -------
         DocumentResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.gets_a_document_from_a_document_collection_by_uuid(
             collection_name="collectionName",
             document_uuid="documentUUID",
@@ -863,15 +863,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.delete_document(
             collection_name="collectionName",
             document_uuid="documentUUID",
@@ -950,15 +950,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.updates_a_document(
             collection_name="collectionName",
             document_uuid="documentUUID",
@@ -1061,15 +1061,15 @@
         Returns
         -------
         DocumentSearchResultPage
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.document.search(
             collection_name="collectionName",
         )
@@ -1159,15 +1159,15 @@
         Returns
         -------
         typing.List[typing.List[DocumentCollectionResponse]]
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.list_collections()
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -1223,15 +1223,15 @@
         Returns
         -------
         DocumentCollectionResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.get_collection(
             collection_name="collectionName",
         )
@@ -1304,15 +1304,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.add_collection(
             collection_name="collectionName",
         )
@@ -1387,15 +1387,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.delete_collection(
             collection_name="collectionName",
         )
@@ -1468,15 +1468,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.update_collection(
             collection_name="collectionName",
         )
@@ -1557,16 +1557,16 @@
         Returns
         -------
         typing.List[str]
             OK
 
         Examples
         --------
-        from zep import CreateDocumentRequest
-        from zep.client import AsyncZep
+        from zep_cloud import CreateDocumentRequest
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.add_documents(
             collection_name="collectionName",
             request=[CreateDocumentRequest()],
@@ -1641,15 +1641,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.batch_delete_documents(
             collection_name="collectionName",
             request=["string"],
@@ -1728,15 +1728,15 @@
         Returns
         -------
         typing.List[DocumentResponse]
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.batch_get_documents(
             collection_name="collectionName",
         )
@@ -1816,16 +1816,16 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep import UpdateDocumentListRequest
-        from zep.client import AsyncZep
+        from zep_cloud import UpdateDocumentListRequest
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.batch_update_documents(
             collection_name="collectionName",
             request=[
@@ -1902,15 +1902,15 @@
         Returns
         -------
         DocumentResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.gets_a_document_from_a_document_collection_by_uuid(
             collection_name="collectionName",
             document_uuid="documentUUID",
@@ -1977,15 +1977,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.delete_document(
             collection_name="collectionName",
             document_uuid="documentUUID",
@@ -2064,15 +2064,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.updates_a_document(
             collection_name="collectionName",
             document_uuid="documentUUID",
@@ -2175,15 +2175,15 @@
         Returns
         -------
         DocumentSearchResultPage
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.document.search(
             collection_name="collectionName",
         )
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/external_clients/document.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/document.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from zep.core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from zep.document.client import DocumentClient as BaseDocumentClient, AsyncDocumentClient as AsyncBaseDocumentClient
+from zep_cloud.core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from zep_cloud.document.client import DocumentClient as BaseDocumentClient, AsyncDocumentClient as AsyncBaseDocumentClient
 
 
 class DocumentClient(BaseDocumentClient):
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         super().__init__(
             client_wrapper=client_wrapper
         )
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/external_clients/memory.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/external_clients/user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from zep.core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from zep.memory.client import MemoryClient as BaseMemoryClient, AsyncMemoryClient as AsyncBaseMemoryClient
+from zep_cloud.core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from zep_cloud.user.client import UserClient as BaseUserClient, AsyncUserClient as AsyncBaseUserClient
 
 
-class MemoryClient(BaseMemoryClient):
+class UserClient(BaseUserClient):
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         super().__init__(
             client_wrapper=client_wrapper
         )
 
 
-class AsyncMemoryClient(AsyncBaseMemoryClient):
+class AsyncUserClient(AsyncBaseUserClient):
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         super().__init__(
             client_wrapper=client_wrapper
         )
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/langchain/history.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/langchain/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import logging
 from typing import Any, Dict, List, Optional, Union
-from zep.client import Zep
-from zep.environment import ZepEnvironment
-from zep.types import Memory, Message
-from zep.errors import NotFoundError
-from zep.langchain.helpers import get_zep_message_role_type
+from zep_cloud.client import Zep
+from zep_cloud.environment import ZepEnvironment
+from zep_cloud.types import Memory, Message
+from zep_cloud.errors import NotFoundError
+from zep_cloud.langchain.helpers import get_zep_message_role_type
 try:
     from langchain_core.chat_history import BaseChatMessageHistory
     from langchain_core.messages import (
         AIMessage,
         BaseMessage,
         HumanMessage,
         SystemMessage,
@@ -43,23 +43,23 @@
         The type of memory to use. Can be "perpetual", "summary_retrieval",
         or "message_window". Defaults to "perpetual".
     summary_instruction : Optional[str]
         Additional instructions for generating dialog summaries.
     """
 
     def __init__(
-        self,
-        session_id: str,
-        zep_client: Optional[Zep] = None,
-        api_url: Optional[str] = str(ZepEnvironment.DEFAULT),
-        api_key: Optional[str] = None,
-        memory_type: Optional[str] = None,
-        ai_prefix: Optional[str] = None,
-        human_prefix: Optional[str] = None,
-        summary_instruction: Optional[str] = None,
+            self,
+            session_id: str,
+            zep_client: Optional[Zep] = None,
+            api_url: Optional[str] = str(ZepEnvironment.DEFAULT),
+            api_key: Optional[str] = None,
+            memory_type: Optional[str] = None,
+            ai_prefix: Optional[str] = None,
+            human_prefix: Optional[str] = None,
+            summary_instruction: Optional[str] = None,
     ) -> None:
         if zep_client is None:
             self._client = Zep(base_url=api_url, api_key=api_key)
         else:
             self._client = zep_client
 
         self.session_id = session_id
@@ -129,41 +129,41 @@
             logger.warning(
                 f"Session {self.session_id} not found in Zep. Returning None"
             )
             return None
         return zep_memory
 
     def add_user_message(  # type: ignore
-        self, message: str, metadata: Optional[Dict[str, Any]] = None
+            self, message: str, metadata: Optional[Dict[str, Any]] = None
     ) -> None:
         """Convenience method for adding a human message string to the store.
 
         Args:
             message: The string contents of a human message.
             metadata: Optional metadata to attach to the message.
         """
         from langchain_core.messages import HumanMessage
 
         self.add_message(HumanMessage(content=message), metadata=metadata)
 
     def add_ai_message(  # type: ignore
-        self, message: str, metadata: Optional[Dict[str, Any]] = None
+            self, message: str, metadata: Optional[Dict[str, Any]] = None
     ) -> None:
         """Convenience method for adding an AI message string to the store.
 
         Args:
             message: The string contents of an AI message.
             metadata: Optional metadata to attach to the message.
         """
         from langchain_core.messages import AIMessage
 
         self.add_message(AIMessage(content=message), metadata=metadata)
 
     def add_message(
-        self, message: BaseMessage, metadata: Optional[Dict[str, Any]] = None
+            self, message: BaseMessage, metadata: Optional[Dict[str, Any]] = None
     ) -> None:
         """Append the message to the Zep memory history"""
 
         if message.content is None:
             raise ValueError("Message content cannot be None")
 
         if isinstance(message.content, list):
@@ -189,8 +189,8 @@
         and this is not advised unless you have specific data retention requirements.
         """
         try:
             self._client.memory.delete(self.session_id)
         except NotFoundError:
             logger.warning(
                 f"Session {self.session_id} not found in Zep. Skipping delete."
-            )
+            )
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/langchain/vectorstore.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/langchain/vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import logging
 from typing import Any, Dict, Iterable, List, Optional, Tuple
-from zep.types import Memory, Message, DocumentCollectionResponse, DocumentResponse, CreateDocumentRequest
-from zep.errors import NotFoundError
-from zep.langchain.helpers import get_zep_message_role_type
-from zep.client import Zep, AsyncZep
-from zep.environment import ZepEnvironment
+from zep_cloud.types import DocumentCollectionResponse, CreateDocumentRequest
+from zep_cloud.errors import NotFoundError
+from zep_cloud.client import Zep, AsyncZep
+from zep_cloud.environment import ZepEnvironment
 
 try:
     from langchain_core.documents import Document
     from langchain_core.vectorstores import VectorStore
 except ImportError:
     raise ImportError(
         "Could not import langchain-core package. "
@@ -36,21 +35,21 @@
             collection.
         api_url (Optional[str]): The URL of the Zep API. Defaults to "https://api.getzep.com".
             Not required if passing in a ZepClient.
         api_key (str): The API key for the Zep API.
     """
 
     def __init__(
-        self,
-        collection_name: str,
-        description: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
+            self,
+            collection_name: str,
+            description: Optional[str] = None,
+            metadata: Optional[Dict[str, Any]] = None,
 
-        api_url: Optional[str] = str(ZepEnvironment.DEFAULT),
-        api_key: Optional[str] = None,
+            api_url: Optional[str] = str(ZepEnvironment.DEFAULT),
+            api_key: Optional[str] = None,
     ) -> None:
         super().__init__()
         if not collection_name:
             raise ValueError(
                 "collection_name must be specified when using ZepVectorStore."
             )
         self._client = Zep(api_key=api_key, base_url=api_url)
@@ -88,36 +87,36 @@
             description=self.c_description,
             metadata=self.c_metadata,
         )
         collection = self._client.document.get_collection(collection_name=self.collection_name)
         return collection
 
     def _generate_documents_to_add(
-        self,
-        texts: Iterable[str],
-        metadatas: Optional[List[Dict[Any, Any]]] = None,  # langchain spelling
-        document_ids: Optional[List[str]] = None,
+            self,
+            texts: Iterable[str],
+            metadatas: Optional[List[Dict[Any, Any]]] = None,  # langchain spelling
+            document_ids: Optional[List[str]] = None,
     ) -> List[CreateDocumentRequest]:
         documents: List[CreateDocumentRequest] = []
         for i, d in enumerate(texts):
             documents.append(
                 CreateDocumentRequest(
                     content=d,
                     metadata=metadatas[i] if metadatas else None,
                     document_id=document_ids[i] if document_ids else None,
                 )
             )
         return documents
 
     def add_texts(
-        self,
-        texts: Iterable[str],
-        metadatas: Optional[List[Dict[str, Any]]] = None,  # langchain spelling
-        document_ids: Optional[List[str]] = None,
-        **kwargs: Any,
+            self,
+            texts: Iterable[str],
+            metadatas: Optional[List[Dict[str, Any]]] = None,  # langchain spelling
+            document_ids: Optional[List[str]] = None,
+            **kwargs: Any,
     ) -> List[str]:
         """Run more texts through the embeddings and add to the vectorstore.
 
         Args:
             texts: Iterable of strings to add to the vectorstore.
             metadatas: Optional list of metadatas associated with the texts.
             document_ids: Optional list of document ids associated with the texts.
@@ -129,32 +128,32 @@
 
         documents = self._generate_documents_to_add(texts, metadatas, document_ids)
         uuids = self._client.document.add_documents(collection_name=self.collection_name, request=documents)
 
         return uuids
 
     async def aadd_texts(
-        self,
-        texts: Iterable[str],
-        metadatas: Optional[List[Dict[str, Any]]] = None,  # langchain spelling
-        document_ids: Optional[List[str]] = None,
-        **kwargs: Any,
+            self,
+            texts: Iterable[str],
+            metadatas: Optional[List[Dict[str, Any]]] = None,  # langchain spelling
+            document_ids: Optional[List[str]] = None,
+            **kwargs: Any,
     ) -> List[str]:
         documents = self._generate_documents_to_add(texts, metadatas, document_ids)
         uuids = await self._async_client.document.add_documents(collection_name=self.collection_name, request=documents)
 
         return uuids
 
     def search(
-        self,
-        query: str,
-        search_type: str,
-        metadata_filter: Optional[Dict[str, Any]] = None,
-        k: int = 3,
-        **kwargs: Any,
+            self,
+            query: str,
+            search_type: str,
+            metadata_filter: Optional[Dict[str, Any]] = None,
+            k: int = 3,
+            **kwargs: Any,
     ) -> List[Document]:
         """Return docs most similar to query using specified search type."""
         if search_type == "similarity":
             return self.similarity_search(
                 query, k=k, metadata=metadata_filter, **kwargs
             )
         elif search_type == "mmr":
@@ -164,20 +163,20 @@
         else:
             raise ValueError(
                 f"search_type of {search_type} not allowed. Expected "
                 "search_type to be 'similarity' or 'mmr'."
             )
 
     async def asearch(
-        self,
-        query: str,
-        search_type: str,
-        metadata_filter: Optional[Dict[str, Any]] = None,
-        k: int = 3,
-        **kwargs: Any,
+            self,
+            query: str,
+            search_type: str,
+            metadata_filter: Optional[Dict[str, Any]] = None,
+            k: int = 3,
+            **kwargs: Any,
     ) -> List[Document]:
         """Return docs most similar to query using specified search type."""
         if search_type == "similarity":
             return await self.asimilarity_search(
                 query, k=k, metadata=metadata_filter, **kwargs
             )
         elif search_type == "mmr":
@@ -187,46 +186,46 @@
         else:
             raise ValueError(
                 f"search_type of {search_type} not allowed. Expected "
                 "search_type to be 'similarity' or 'mmr'."
             )
 
     def similarity_search(
-        self,
-        query: str,
-        k: int = 4,
-        metadata: Optional[Dict[str, Any]] = None,
-        **kwargs: Any,
+            self,
+            query: str,
+            k: int = 4,
+            metadata: Optional[Dict[str, Any]] = None,
+            **kwargs: Any,
     ) -> List[Document]:
         """Return docs most similar to query."""
 
         results = self._similarity_search_with_relevance_scores(
             query, k=k, metadata_filter=metadata, **kwargs
         )
         return [doc for doc, _ in results]
 
     def similarity_search_with_score(
-        self,
-        query: str,
-        k: int = 4,
-        metadata: Optional[Dict[str, Any]] = None,
-        **kwargs: Any,
+            self,
+            query: str,
+            k: int = 4,
+            metadata: Optional[Dict[str, Any]] = None,
+            **kwargs: Any,
     ) -> List[Tuple[Document, float]]:
         """Run similarity search with distance."""
 
         return self._similarity_search_with_relevance_scores(
             query, k=k, metadata_filter=metadata, **kwargs
         )
 
     def _similarity_search_with_relevance_scores(
-        self,
-        query: str,
-        k: int = 4,
-        metadata_filter: Optional[Dict[str, Any]] = None,
-        **kwargs: Any,
+            self,
+            query: str,
+            k: int = 4,
+            metadata_filter: Optional[Dict[str, Any]] = None,
+            **kwargs: Any,
     ) -> List[Tuple[Document, float]]:
         """
         Default similarity search with relevance scores.
         Return docs and relevance scores in the range [0, 1].
 
         0 is dissimilar, 1 is most similar.
 
@@ -261,19 +260,19 @@
                 ),
                 doc.score or 0.0,
             )
             for doc in results.results
         ]
 
     async def asimilarity_search_with_relevance_scores(
-        self,
-        query: str,
-        k: int = 4,
-        metadata_filter: Optional[Dict[str, Any]] = None,
-        **kwargs: Any,
+            self,
+            query: str,
+            k: int = 4,
+            metadata_filter: Optional[Dict[str, Any]] = None,
+            **kwargs: Any,
     ) -> List[Tuple[Document, float]]:
         """Return docs most similar to query."""
 
         if not self._collection:
             raise ValueError(
                 "collection should be an instance of a Zep DocumentCollection"
             )
@@ -297,35 +296,35 @@
                 ),
                 doc.score or 0.0,
             )
             for doc in results.results
         ]
 
     async def asimilarity_search(
-        self,
-        query: str,
-        k: int = 4,
-        metadata: Optional[Dict[str, Any]] = None,
-        **kwargs: Any,
+            self,
+            query: str,
+            k: int = 4,
+            metadata: Optional[Dict[str, Any]] = None,
+            **kwargs: Any,
     ) -> List[Document]:
         """Return docs most similar to query."""
 
         results = await self.asimilarity_search_with_relevance_scores(
             query, k, metadata_filter=metadata, **kwargs
         )
 
         return [doc for doc, _ in results]
 
     def max_marginal_relevance_search(  # type: ignore # ignore inconsistent override
-        self,
-        query: str,
-        k: int = 4,
-        fetch_k: int = 20,
-        lambda_mult: float = 0.5,
-        metadata_filter: Optional[Dict[str, Any]] = None,
+            self,
+            query: str,
+            k: int = 4,
+            fetch_k: int = 20,
+            lambda_mult: float = 0.5,
+            metadata_filter: Optional[Dict[str, Any]] = None,
     ) -> List[Document]:
         """Return docs selected using the maximal marginal relevance reranking.
 
         Maximal marginal relevance optimizes for similarity to query AND diversity
         among selected documents.
 
         Args:
@@ -359,21 +358,21 @@
             return []
 
         return [
             Document(page_content=str(d.content), metadata=d.metadata or {}) for d in results.results
         ]
 
     async def amax_marginal_relevance_search(
-        self,
-        query: str,
-        k: int = 4,
-        fetch_k: int = 20,
-        lambda_mult: float = 0.5,
-        metadata_filter: Optional[Dict[str, Any]] = None,
-        **kwargs: Any,
+            self,
+            query: str,
+            k: int = 4,
+            fetch_k: int = 20,
+            lambda_mult: float = 0.5,
+            metadata_filter: Optional[Dict[str, Any]] = None,
+            **kwargs: Any,
     ) -> List[Document]:
         """Return docs selected using the maximal marginal relevance reranking.
 
         Maximal marginal relevance optimizes for similarity to query AND diversity
         among selected documents.
 
         Args:
@@ -413,23 +412,23 @@
 
         return [
             Document(page_content=str(d.content), metadata=d.metadata or {}) for d in results.results
         ]
 
     @classmethod
     def from_texts(  # type: ignore # ignore inconsistent override
-        cls,
-        texts: List[str],
-        collection_name: str,
-        metadatas: Optional[List[dict]] = None,
-        description: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
-        api_url: Optional[str] = str(ZepEnvironment.DEFAULT),
-        api_key: Optional[str] = None,
-        **kwargs: Any,
+            cls,
+            texts: List[str],
+            collection_name: str,
+            metadatas: Optional[List[dict]] = None,
+            description: Optional[str] = None,
+            metadata: Optional[Dict[str, Any]] = None,
+            api_url: Optional[str] = None,
+            api_key: Optional[str] = None,
+            **kwargs: Any,
     ) -> ZepVectorStore:
         """
         Class method that returns a ZepVectorStore instance initialized from texts.
 
         If the collection does not exist, it will be created.
 
         Args:
@@ -459,23 +458,23 @@
         )
         vecstore.add_texts(texts, metadatas)
 
         return vecstore
 
     @classmethod
     async def afrom_texts(  # type: ignore # ignore inconsistent override
-        cls,
-        texts: List[str],
-        collection_name: str,
-        metadatas: Optional[List[dict]] = None,
-        description: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
-        api_url: Optional[str] = str(ZepEnvironment.DEFAULT),
-        api_key: Optional[str] = None,
-        **kwargs: Any,
+            cls,
+            texts: List[str],
+            collection_name: str,
+            metadatas: Optional[List[dict]] = None,
+            description: Optional[str] = None,
+            metadata: Optional[Dict[str, Any]] = None,
+            api_url: Optional[str] = str(ZepEnvironment.DEFAULT),
+            api_key: Optional[str] = None,
+            **kwargs: Any,
     ) -> ZepVectorStore:
         """
         Class method that asynchronously returns a ZepVectorStore instance
         initialized from texts.
 
         If the collection does not exist, it will be created.
 
@@ -506,28 +505,28 @@
             api_key=api_key,
         )
         await vecstore.aadd_texts(texts, metadatas)
         return vecstore
 
     @classmethod
     def from_documents(  # type: ignore # ignore inconsistent override
-        cls,
-        documents: List[Document],
-        **kwargs: Any,
+            cls,
+            documents: List[Document],
+            **kwargs: Any,
     ) -> ZepVectorStore:
         """Return VectorStore initialized from documents."""
         texts = [d.page_content for d in documents]
         metadatas = [d.metadata for d in documents]
         return cls.from_texts(texts, metadatas=metadatas, **kwargs)
 
     @classmethod
     async def afrom_documents(  # type: ignore # ignore inconsistent override
-        cls,
-        documents: List[Document],
-        **kwargs: Any,
+            cls,
+            documents: List[Document],
+            **kwargs: Any,
     ) -> ZepVectorStore:
         """Asynchronously return VectorStore initialized from documents."""
         texts = [d.page_content for d in documents]
         metadatas = [d.metadata for d in documents]
         return await cls.afrom_texts(texts, metadatas=metadatas, **kwargs)
 
     def delete(self, ids: Optional[List[str]] = None, **kwargs: Any) -> None:
@@ -547,8 +546,8 @@
         if ids is None or len(ids) == 0:
             raise ValueError("No uuids provided to delete.")
 
         if self._collection is None:
             raise ValueError("No collection name provided.")
 
         for u in ids:
-            self._client.document.delete_document(collection_name=self.collection_name, document_uuid=u)
+            self._client.document.delete_document(collection_name=self.collection_name, document_uuid=u)
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/memory/client.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/memory/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from ..types.message import Message
 from ..types.message_list_response import MessageListResponse
 from ..types.models_zep_data_class import ModelsZepDataClass
 from ..types.question import Question
 from ..types.search_scope import SearchScope
 from ..types.search_type import SearchType
 from ..types.session import Session
+from ..types.session_list_response import SessionListResponse
 from ..types.success_response import SuccessResponse
 from ..types.summary_list_response import SummaryListResponse
 from .types.memory_get_request_memory_type import MemoryGetRequestMemoryType
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
@@ -64,15 +65,15 @@
         Returns
         -------
         Session
             The added session.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.add_session(
             session_id="session_id",
         )
@@ -126,15 +127,15 @@
         self,
         *,
         page_number: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         order_by: typing.Optional[str] = None,
         asc: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> typing.List[Session]:
+    ) -> SessionListResponse:
         """
         Get all sessions with optional page number, page size, order by field and order direction for pagination.
 
         Parameters
         ----------
         page_number : typing.Optional[int]
             Page number for pagination, starting from 1
@@ -149,20 +150,20 @@
             Order direction: true for ascending, false for descending
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        typing.List[Session]
+        SessionListResponse
             List of sessions
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.list_sessions()
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -194,15 +195,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(typing.List[Session], _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(SessionListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
             )
         try:
@@ -226,15 +227,15 @@
         Returns
         -------
         Session
             The session with the specified ID.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.get_session(
             session_id="sessionId",
         )
@@ -299,15 +300,15 @@
         Returns
         -------
         Session
             The updated session.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.update_session(
             session_id="sessionId",
             metadata={},
@@ -397,15 +398,15 @@
         Returns
         -------
         ClassifySessionResponse
             A response object containing the name and classification result.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.classify_session(
             session_id="sessionId",
             classes=["classes"],
@@ -487,16 +488,16 @@
         Returns
         -------
         typing.Dict[str, str]
             OK
 
         Examples
         --------
-        from zep import ModelsZepDataClass
-        from zep.client import Zep
+        from zep_cloud import ModelsZepDataClass
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.extract_session_data(
             session_id="sessionId",
             zep_data_classes=[ModelsZepDataClass()],
@@ -575,15 +576,15 @@
         Returns
         -------
         Memory
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.get(
             session_id="sessionId",
         )
@@ -662,16 +663,16 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep import Message
-        from zep.client import Zep
+        from zep_cloud import Message
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.add(
             session_id="sessionId",
             messages=[Message()],
@@ -735,15 +736,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.delete(
             session_id="sessionId",
         )
@@ -812,15 +813,15 @@
         Returns
         -------
         MessageListResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.get_session_messages(
             session_id="sessionId",
         )
@@ -891,15 +892,15 @@
         Returns
         -------
         Message
             The message.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.get_session_message(
             session_id="sessionId",
             message_uuid="messageUUID",
@@ -970,15 +971,15 @@
         Returns
         -------
         Message
             The updated message.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.update_message_metadata(
             session_id="sessionId",
             message_uuid="messageUUID",
@@ -1071,15 +1072,15 @@
         Returns
         -------
         typing.List[MemorySearchResult]
             A list of SearchResult objects representing the search results.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.search(
             session_id="sessionId",
         )
@@ -1165,15 +1166,15 @@
         Returns
         -------
         SummaryListResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.get_summaries(
             session_id="sessionId",
         )
@@ -1238,15 +1239,15 @@
         Returns
         -------
         Question
             The synthesized question.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.memory.synthesize_question(
             session_id="sessionId",
         )
@@ -1330,15 +1331,15 @@
         Returns
         -------
         Session
             The added session.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.add_session(
             session_id="session_id",
         )
@@ -1392,15 +1393,15 @@
         self,
         *,
         page_number: typing.Optional[int] = None,
         page_size: typing.Optional[int] = None,
         order_by: typing.Optional[str] = None,
         asc: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> typing.List[Session]:
+    ) -> SessionListResponse:
         """
         Get all sessions with optional page number, page size, order by field and order direction for pagination.
 
         Parameters
         ----------
         page_number : typing.Optional[int]
             Page number for pagination, starting from 1
@@ -1415,20 +1416,20 @@
             Order direction: true for ascending, false for descending
 
         request_options : typing.Optional[RequestOptions]
             Request-specific configuration.
 
         Returns
         -------
-        typing.List[Session]
+        SessionListResponse
             List of sessions
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.list_sessions()
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -1460,15 +1461,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic_v1.parse_obj_as(typing.List[Session], _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(SessionListResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json()))  # type: ignore
         if _response.status_code == 500:
             raise InternalServerError(
                 pydantic_v1.parse_obj_as(types_api_error_ApiError, _response.json())  # type: ignore
             )
         try:
@@ -1492,15 +1493,15 @@
         Returns
         -------
         Session
             The session with the specified ID.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.get_session(
             session_id="sessionId",
         )
@@ -1565,15 +1566,15 @@
         Returns
         -------
         Session
             The updated session.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.update_session(
             session_id="sessionId",
             metadata={},
@@ -1663,15 +1664,15 @@
         Returns
         -------
         ClassifySessionResponse
             A response object containing the name and classification result.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.classify_session(
             session_id="sessionId",
             classes=["classes"],
@@ -1753,16 +1754,16 @@
         Returns
         -------
         typing.Dict[str, str]
             OK
 
         Examples
         --------
-        from zep import ModelsZepDataClass
-        from zep.client import AsyncZep
+        from zep_cloud import ModelsZepDataClass
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.extract_session_data(
             session_id="sessionId",
             zep_data_classes=[ModelsZepDataClass()],
@@ -1841,15 +1842,15 @@
         Returns
         -------
         Memory
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.get(
             session_id="sessionId",
         )
@@ -1928,16 +1929,16 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep import Message
-        from zep.client import AsyncZep
+        from zep_cloud import Message
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.add(
             session_id="sessionId",
             messages=[Message()],
@@ -2003,15 +2004,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.delete(
             session_id="sessionId",
         )
@@ -2080,15 +2081,15 @@
         Returns
         -------
         MessageListResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.get_session_messages(
             session_id="sessionId",
         )
@@ -2159,15 +2160,15 @@
         Returns
         -------
         Message
             The message.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.get_session_message(
             session_id="sessionId",
             message_uuid="messageUUID",
@@ -2238,15 +2239,15 @@
         Returns
         -------
         Message
             The updated message.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.update_message_metadata(
             session_id="sessionId",
             message_uuid="messageUUID",
@@ -2339,15 +2340,15 @@
         Returns
         -------
         typing.List[MemorySearchResult]
             A list of SearchResult objects representing the search results.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.search(
             session_id="sessionId",
         )
@@ -2433,15 +2434,15 @@
         Returns
         -------
         SummaryListResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.get_summaries(
             session_id="sessionId",
         )
@@ -2506,15 +2507,15 @@
         Returns
         -------
         Question
             The synthesized question.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.memory.synthesize_question(
             session_id="sessionId",
         )
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/__init__.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .message_list_response import MessageListResponse
 from .models_zep_data_class import ModelsZepDataClass
 from .question import Question
 from .role_type import RoleType
 from .search_scope import SearchScope
 from .search_type import SearchType
 from .session import Session
+from .session_list_response import SessionListResponse
 from .success_response import SuccessResponse
 from .summary import Summary
 from .summary_list_response import SummaryListResponse
 from .update_document_list_request import UpdateDocumentListRequest
 from .user import User
 from .user_list_response import UserListResponse
 
@@ -38,14 +39,15 @@
     "MessageListResponse",
     "ModelsZepDataClass",
     "Question",
     "RoleType",
     "SearchScope",
     "SearchType",
     "Session",
+    "SessionListResponse",
     "SuccessResponse",
     "Summary",
     "SummaryListResponse",
     "UpdateDocumentListRequest",
     "User",
     "UserListResponse",
 ]
```

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/api_error.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/api_error.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/classify_session_response.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/classify_session_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/create_document_request.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/create_document_request.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/document_collection_response.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/document_collection_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/document_response.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/document_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/document_search_result.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/document_search_result.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/document_search_result_page.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/document_search_result_page.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/memory.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/memory.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/memory_search_result.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/memory_search_result.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/message.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/message.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/message_list_response.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/message_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/models_zep_data_class.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/models_zep_data_class.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/question.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/question.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/session.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/session.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/success_response.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/success_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/summary.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/summary.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/summary_list_response.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/summary_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/update_document_list_request.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/update_document_list_request.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/user.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/user.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/types/user_list_response.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/types/user_list_response.py`

 * *Files identical despite different names*

### Comparing `zep_cloud-0.0.1rc1/src/zep/user/client.py` & `zep_cloud-1.0.0rc1/src/zep_cloud/user/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         Returns
         -------
         User
             The user that was added.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.user.add()
         """
         _request: typing.Dict[str, typing.Any] = {}
@@ -149,15 +149,15 @@
         Returns
         -------
         UserListResponse
             Successfully retrieved list of users
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.user.list_ordered()
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -219,15 +219,15 @@
         Returns
         -------
         User
             The user that was retrieved.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.user.get(
             user_id="userId",
         )
@@ -281,15 +281,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.user.delete(
             user_id="userId",
         )
@@ -364,15 +364,15 @@
         Returns
         -------
         User
             The user that was updated.
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.user.update(
             user_id="userId",
         )
@@ -445,15 +445,15 @@
         Returns
         -------
         typing.List[Session]
             OK
 
         Examples
         --------
-        from zep.client import Zep
+        from zep_cloud.client import Zep
 
         client = Zep(
             api_key="YOUR_API_KEY",
         )
         client.user.get_sessions(
             user_id="userId",
         )
@@ -533,15 +533,15 @@
         Returns
         -------
         User
             The user that was added.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.user.add()
         """
         _request: typing.Dict[str, typing.Any] = {}
@@ -619,15 +619,15 @@
         Returns
         -------
         UserListResponse
             Successfully retrieved list of users
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.user.list_ordered()
         """
         _response = await self._client_wrapper.httpx_client.request(
@@ -689,15 +689,15 @@
         Returns
         -------
         User
             The user that was retrieved.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.user.get(
             user_id="userId",
         )
@@ -751,15 +751,15 @@
         Returns
         -------
         SuccessResponse
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.user.delete(
             user_id="userId",
         )
@@ -834,15 +834,15 @@
         Returns
         -------
         User
             The user that was updated.
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.user.update(
             user_id="userId",
         )
@@ -915,15 +915,15 @@
         Returns
         -------
         typing.List[Session]
             OK
 
         Examples
         --------
-        from zep.client import AsyncZep
+        from zep_cloud.client import AsyncZep
 
         client = AsyncZep(
             api_key="YOUR_API_KEY",
         )
         await client.user.get_sessions(
             user_id="userId",
         )
```

### Comparing `zep_cloud-0.0.1rc1/PKG-INFO` & `zep_cloud-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zep-cloud
-Version: 0.0.1rc1
+Version: 1.0.0rc1
 Summary: 
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zep-cloud Version: 0.0.1rc1 Summary: Requires-
+Metadata-Version: 2.1 Name: zep-cloud Version: 1.0.0rc1 Summary: Requires-
 Python: >=3.8.1,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: httpx
 (>=0.21.2) Requires-Dist: pydantic (>=1.9.2) Requires-Dist: typing_extensions
 (>=4.0.0) Description-Content-Type: text/markdown [![Release to PyPI](https://
 github.com/getzep/zep-python/actions/workflows/release.yml/badge.svg)](https://
```


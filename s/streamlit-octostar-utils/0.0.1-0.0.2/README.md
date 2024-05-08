# Comparing `tmp/streamlit_octostar_utils-0.0.1.tar.gz` & `tmp/streamlit_octostar_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_octostar_utils-0.0.1.tar", max compression
+gzip compressed data, was "streamlit_octostar_utils-0.0.2.tar", max compression
```

## Comparing `streamlit_octostar_utils-0.0.1.tar` & `streamlit_octostar_utils-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-05-02 14:27:28.125523 streamlit_octostar_utils-0.0.1/LICENSE
--rw-r--r--   0        0        0      324 2024-05-02 14:27:28.125523 streamlit_octostar_utils-0.0.1/README.md
--rw-r--r--   0        0        0      706 2024-05-02 14:27:28.125523 streamlit_octostar_utils-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        1 2024-05-02 14:27:28.125523 streamlit_octostar_utils-0.0.1/streamlit_octostar_utils/__init__.py
--rw-r--r--   0        0        0       68 2024-05-02 14:27:28.125523 streamlit_octostar_utils-0.0.1/streamlit_octostar_utils/hello.py
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 streamlit_octostar_utils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/LICENSE
+-rw-r--r--   0        0        0      324 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/README.md
+-rw-r--r--   0        0        0      706 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/core/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/core/threading/__init__.py
+-rw-r--r--   0        0        0     2224 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/core/threading/key_queue.py
+-rw-r--r--   0        0        0       68 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/hello.py
+-rw-r--r--   0        0        0        1 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/__init__.py
+-rw-r--r--   0        0        0     4627 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/async_task_manager.py
+-rw-r--r--   0        0        0     4078 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/session_callback_manager.py
+-rw-r--r--   0        0        0      809 2024-05-08 07:57:16.536455 streamlit_octostar_utils-0.0.2/streamlit_octostar_utils/threading/session_state_hot_swapper.py
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 streamlit_octostar_utils-0.0.2/PKG-INFO
```

### Comparing `streamlit_octostar_utils-0.0.1/LICENSE` & `streamlit_octostar_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.1/pyproject.toml` & `streamlit_octostar_utils-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-octostar-utils"
-version = "0.0.1"
+version = "0.0.2"
 description = ""
 license = "MIT"
 authors = ["Valerio Tonelli <tonellivalerio97@gmail.com>"]
 readme = "README.md"
 include = [
     "streamlit-octostar-utils/**/*"
 ]
@@ -18,14 +18,14 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 pydantic = "^2.6.4"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
-streamlit = "^1.31.0"
+streamlit = "^1.33.0"
 streamlit-octostar-research = "^0.1.22"
 mypy = "^1.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `streamlit_octostar_utils-0.0.1/PKG-INFO` & `streamlit_octostar_utils-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-octostar-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 License: MIT
 Author: Valerio Tonelli
 Author-email: tonellivalerio97@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


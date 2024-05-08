# Comparing `tmp/cmem_plugin_loopwf-0.5.0.tar.gz` & `tmp/cmem_plugin_loopwf-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_loopwf-0.5.0.tar", max compression
+gzip compressed data, was "cmem_plugin_loopwf-0.5.1.tar", max compression
```

## Comparing `cmem_plugin_loopwf-0.5.0.tar` & `cmem_plugin_loopwf-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11334 2024-04-24 14:32:41.072847 cmem_plugin_loopwf-0.5.0/LICENSE
--rw-r--r--   0        0        0      368 2024-04-24 14:32:41.081079 cmem_plugin_loopwf-0.5.0/README-public.md
--rw-r--r--   0        0        0       28 2024-04-24 14:32:41.071218 cmem_plugin_loopwf-0.5.0/cmem_plugin_loopwf/__init__.py
--rw-r--r--   0        0        0      401 2024-04-24 17:07:49.776203 cmem_plugin_loopwf-0.5.0/cmem_plugin_loopwf/exceptions.py
--rw-r--r--   0        0        0      284 2024-04-30 12:42:57.032768 cmem_plugin_loopwf-0.5.0/cmem_plugin_loopwf/loopwf.svg
--rw-r--r--   0        0        0     5642 2024-04-30 12:43:23.409184 cmem_plugin_loopwf-0.5.0/cmem_plugin_loopwf/task.py
--rw-r--r--   0        0        0     2467 2024-04-30 06:52:45.020440 cmem_plugin_loopwf-0.5.0/cmem_plugin_loopwf/workflow_type.py
--rw-r--r--   0        0        0     2987 2024-04-30 13:05:18.187810 cmem_plugin_loopwf-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 cmem_plugin_loopwf-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2024-05-08 13:50:04.259394 cmem_plugin_loopwf-0.5.1/LICENSE
+-rw-r--r--   0        0        0      368 2024-05-08 13:50:04.259394 cmem_plugin_loopwf-0.5.1/README-public.md
+-rw-r--r--   0        0        0       28 2024-05-08 13:50:04.259394 cmem_plugin_loopwf-0.5.1/cmem_plugin_loopwf/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-08 13:50:04.259394 cmem_plugin_loopwf-0.5.1/cmem_plugin_loopwf/exceptions.py
+-rw-r--r--   0        0        0      284 2024-05-08 13:50:04.259394 cmem_plugin_loopwf-0.5.1/cmem_plugin_loopwf/loopwf.svg
+-rw-r--r--   0        0        0     5858 2024-05-08 13:50:04.259394 cmem_plugin_loopwf-0.5.1/cmem_plugin_loopwf/task.py
+-rw-r--r--   0        0        0     2467 2024-05-08 13:50:04.259394 cmem_plugin_loopwf-0.5.1/cmem_plugin_loopwf/workflow_type.py
+-rw-r--r--   0        0        0     2946 2024-05-08 13:50:21.467401 cmem_plugin_loopwf-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1179 1970-01-01 00:00:00.000000 cmem_plugin_loopwf-0.5.1/PKG-INFO
```

### Comparing `cmem_plugin_loopwf-0.5.0/LICENSE` & `cmem_plugin_loopwf-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_loopwf-0.5.0/cmem_plugin_loopwf/task.py` & `cmem_plugin_loopwf-0.5.1/cmem_plugin_loopwf/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,20 @@
 from cmem_plugin_base.dataintegration.ports import FixedNumberOfInputs, FlexibleSchemaPort
 from cmem_plugin_base.dataintegration.utils import setup_cmempy_user_access
 
 from cmem_plugin_loopwf import exceptions
 from cmem_plugin_loopwf.workflow_type import SuitableWorkflowParameterType
 
 DOCUMENTATION = """This workflow task operates on a list of incoming entities
-and starts a separated workflow for each entity. The started workflow needs to
-have a replaceable JSON dataset as input.
+and sequentially starts a single "inner" workflow for each entity.
+In case one "inner" workflow fails, the execution is stopped with an error.
+In this case the error message can be seen in the Activities view
+(see `Execute with payload of [inner workflow name]`).
+
+The started workflow needs to have a replaceable JSON dataset as input.
 
 Current notes and limitations:
 
 - The entities which are the input of the "inner" workflow can not be hierarchic.
 - The replaceable dataset of the "inner" workflow needs to be a JSON dataset.
 - There is no check for circles implemented!
 """
```

### Comparing `cmem_plugin_loopwf-0.5.0/cmem_plugin_loopwf/workflow_type.py` & `cmem_plugin_loopwf-0.5.1/cmem_plugin_loopwf/workflow_type.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_loopwf-0.5.0/pyproject.toml` & `cmem_plugin_loopwf-0.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-loopwf"
-version = "0.5.0"
+version = "0.5.1"
 license = "Apache-2.0"
 description = "Loop over the output of a task and start a sub-workflow for each entity."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
@@ -16,26 +16,27 @@
 homepage = "https://github.com/eccenca/cmem-plugin-loopwf"
 
 [tool.poetry.dependencies]
 # if you need to change python version here, change it also in .python-version
 python = "^3.11"
 
 [tool.poetry.dependencies.cmem-plugin-base]
-version = "^4.3.0"
+version = "^4.5.0"
 allow-prereleases = false
 
 [tool.poetry.group.dev.dependencies]
 genbadge = {extras = ["coverage"], version = "^1.1.1"}
-mypy = "^1.2.0"
-pip = ">=23.3" # Avoid safety issue 62044 for pip less than 23.3
-pytest = "^7.3.1"
+mypy = "^1.10.0"
+pip = "^24"
+pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
 pytest-dotenv = "^0.5.2"
-pytest-memray = { version = "^1.5.0",  markers = "platform_system != 'Windows'" }
-ruff = "^0.1.5"
+pytest-html = "^4.1.1"
+pytest-memray = { version = "^1.6.0",  markers = "platform_system != 'Windows'" }
+ruff = "^0.1.15"
 safety = "^1.10.3"
 cmem-cmemc = "^24.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
@@ -55,15 +56,14 @@
 [tool.coverage.report]
 exclude_also = [
     "def __repr__",
     "if self.debug:",
     "if settings.DEBUG",
     "raise AssertionError",
     "raise NotImplementedError",
-    "if 0:",
     "if TYPE_CHECKING:",
     "class .*\\bProtocol\\):",
     "@(abc\\.)?abstractmethod",
     ]
 
 [tool.ruff]
 line-length = 100
```

### Comparing `cmem_plugin_loopwf-0.5.0/PKG-INFO` & `cmem_plugin_loopwf-0.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-loopwf
-Version: 0.5.0
+Version: 0.5.1
 Summary: Loop over the output of a task and start a sub-workflow for each entity.
 Home-page: https://github.com/eccenca/cmem-plugin-loopwf
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cmem-plugin-base (>=4.3.0,<5.0.0)
+Requires-Dist: cmem-plugin-base (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # cmem-plugin-loopwf
 
 Loop over the output of a task and start a sub-workflow for each entity.
 
 This is a plugin for [eccenca](https://eccenca.com) [Corporate Memory](https://documentation.eccenca.com).
```


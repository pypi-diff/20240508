# Comparing `tmp/enact-0.4.6.tar.gz` & `tmp/enact-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enact-0.4.6.tar", last modified: Fri Apr 26 20:06:48 2024, max compression
+gzip compressed data, was "enact-0.4.7.tar", last modified: Wed May  8 17:24:21 2024, max compression
```

## Comparing `enact-0.4.6.tar` & `enact-0.4.7.tar`

### file list

```diff
@@ -1,51 +1,56 @@
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    11357 2023-08-07 17:31:37.000000 enact-0.4.6/LICENSE
--rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-04-26 20:06:48.669546 enact-0.4.6/PKG-INFO
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    14497 2023-12-06 01:14:11.000000 enact-0.4.6/README.md
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      550 2024-04-26 19:56:26.000000 enact-0.4.6/pyproject.toml
--rw-rw-r--   0 leo      (824781618) leo      (824781618)       38 2024-04-26 20:06:48.669546 enact-0.4.6/setup.cfg
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.665546 enact-0.4.6/src/
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/src/enact/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3260 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     8742 2024-04-08 21:41:00.000000 enact-0.4.6/src/enact/contexts.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     4062 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/digests.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/src/enact/fastapi/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      808 2024-04-02 22:20:36.000000 enact-0.4.6/src/enact/fastapi/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     4596 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/fastapi/fastapi.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    18263 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/function_wrappers.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/src/enact/gradio/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      813 2024-04-02 22:20:36.000000 enact-0.4.6/src/enact/gradio/__init__.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    26488 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/gradio/gradio.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     8972 2024-04-03 21:00:20.000000 enact-0.4.6/src/enact/interfaces.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     7394 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/invocation_generators.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    32624 2023-12-14 01:55:35.000000 enact-0.4.6/src/enact/invocations.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6992 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/pretty_print.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        0 2023-08-07 17:31:37.000000 enact-0.4.6/src/enact/py.typed
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    11286 2024-04-03 20:56:13.000000 enact-0.4.6/src/enact/references.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3333 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/registration.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)      273 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/resource_digests.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    15966 2024-04-26 19:56:26.000000 enact-0.4.6/src/enact/resource_registry.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5024 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/resources.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5760 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/serialization.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5913 2024-02-11 18:04:33.000000 enact-0.4.6/src/enact/type_wrappers.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1440 2023-12-06 01:14:11.000000 enact-0.4.6/src/enact/utils.py
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/src/enact.egg-info/
--rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/PKG-INFO
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1087 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/SOURCES.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        1 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/dependency_links.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)       19 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/requires.txt
--rw-rw-r--   0 leo      (824781618) leo      (824781618)        6 2024-04-26 20:06:48.000000 enact-0.4.6/src/enact.egg-info/top_level.txt
-drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-04-26 20:06:48.669546 enact-0.4.6/tests/
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     7525 2024-04-08 21:55:50.000000 enact-0.4.6/tests/test_contexts.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1379 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_digest.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    13705 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_function_wrappers.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3994 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_invocation_generator.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)    26951 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_invocations.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     1534 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_pretty_print.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     6787 2024-04-03 21:00:20.000000 enact-0.4.6/tests/test_references.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     3707 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_registration.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     8670 2024-04-26 19:51:23.000000 enact-0.4.6/tests/test_resource_registry.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     5680 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_resources.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2271 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_serialize.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2250 2024-02-11 18:04:33.000000 enact-0.4.6/tests/test_type_wrappers.py
--rw-rw-r--   0 leo      (824781618) leo      (824781618)     2538 2023-12-06 01:14:11.000000 enact-0.4.6/tests/test_utils.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-05-08 17:24:21.199905 enact-0.4.7/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    11357 2023-08-07 17:31:37.000000 enact-0.4.7/LICENSE
+-rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-05-08 17:24:21.199905 enact-0.4.7/PKG-INFO
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    14497 2023-12-06 01:14:11.000000 enact-0.4.7/README.md
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      550 2024-05-08 17:19:59.000000 enact-0.4.7/pyproject.toml
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)       38 2024-05-08 17:24:21.199905 enact-0.4.7/setup.cfg
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-05-08 17:24:21.199905 enact-0.4.7/src/
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-05-08 17:24:21.199905 enact-0.4.7/src/enact/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3580 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1550 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/acyclic.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     8758 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/contexts.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4074 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/digests.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     6307 2024-05-08 17:19:59.000000 enact-0.4.7/src/enact/distribution_registry.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-05-08 17:24:21.199905 enact-0.4.7/src/enact/fastapi/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      808 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/fastapi/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4596 2023-12-06 01:14:11.000000 enact-0.4.7/src/enact/fastapi/fastapi.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    18355 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/function_wrappers.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-05-08 17:24:21.199905 enact-0.4.7/src/enact/gradio/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      829 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/gradio/__init__.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    26432 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/gradio/gradio.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     8545 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/interfaces.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     7394 2023-12-06 01:14:11.000000 enact-0.4.7/src/enact/invocation_generators.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    32678 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/invocations.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     6992 2023-12-06 01:14:11.000000 enact-0.4.7/src/enact/pretty_print.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        0 2023-08-07 17:31:37.000000 enact-0.4.7/src/enact/py.typed
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    17910 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/references.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3333 2024-05-02 23:35:17.000000 enact-0.4.7/src/enact/registration.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)      273 2023-12-06 01:14:11.000000 enact-0.4.7/src/enact/resource_digests.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    18504 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/resource_registry.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     4747 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/resources.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5765 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/serialization.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5913 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/type_wrappers.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3475 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/utils.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1164 2024-05-08 17:10:36.000000 enact-0.4.7/src/enact/version.py
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-05-08 17:24:21.199905 enact-0.4.7/src/enact.egg-info/
+-rw-r--r--   0 leo      (824781618) leo      (824781618)    14900 2024-05-08 17:24:21.000000 enact-0.4.7/src/enact.egg-info/PKG-INFO
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1222 2024-05-08 17:24:21.000000 enact-0.4.7/src/enact.egg-info/SOURCES.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        1 2024-05-08 17:24:21.000000 enact-0.4.7/src/enact.egg-info/dependency_links.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)       19 2024-05-08 17:24:21.000000 enact-0.4.7/src/enact.egg-info/requires.txt
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)        6 2024-05-08 17:24:21.000000 enact-0.4.7/src/enact.egg-info/top_level.txt
+drwxrwxr-x   0 leo      (824781618) leo      (824781618)        0 2024-05-08 17:24:21.199905 enact-0.4.7/tests/
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     7525 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_contexts.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1379 2023-12-06 01:14:11.000000 enact-0.4.7/tests/test_digest.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2823 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_distribution_registry.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    13705 2023-12-06 01:14:11.000000 enact-0.4.7/tests/test_function_wrappers.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3994 2023-12-06 01:14:11.000000 enact-0.4.7/tests/test_invocation_generator.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    27180 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_invocations.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1534 2023-12-06 01:14:11.000000 enact-0.4.7/tests/test_pretty_print.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)    12133 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_references.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3707 2023-12-06 01:14:11.000000 enact-0.4.7/tests/test_registration.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     9763 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_resource_registry.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     5442 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_resources.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2335 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_serialize.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     2250 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_type_wrappers.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     3901 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_utils.py
+-rw-rw-r--   0 leo      (824781618) leo      (824781618)     1385 2024-05-08 17:10:36.000000 enact-0.4.7/tests/test_version.py
```

### Comparing `enact-0.4.6/LICENSE` & `enact-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/PKG-INFO` & `enact-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enact
-Version: 0.4.6
+Version: 0.4.7
 Summary: A framework for generative software.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enact-0.4.6/README.md` & `enact-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/pyproject.toml` & `enact-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "enact"
-version = "0.4.6"
+version = "0.4.7"
 dependencies = [
   "numpy",
   "Pillow",
   "wrapt",
 ]
 description = "A framework for generative software."
 readme = "README.md"
```

### Comparing `enact-0.4.6/src/enact/__init__.py` & `enact-0.4.7/src/enact/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,22 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Top-level definitions."""
 
+from enact.distribution_registry import register_distribution
+from enact.distribution_registry import get_path_distribution_info
+from enact.distribution_registry import get_distribution_info
+
+from enact.version import __version__
 from enact.function_wrappers import invoke
 from enact.function_wrappers import invoke_async
-
 from enact.resource_digests import resource_digest
 
 from enact.interfaces import FieldValue
 from enact.interfaces import ResourceDictValue
 from enact.interfaces import FieldTypeError
+from enact.interfaces import DistributionInfo
 from enact.interfaces import ResourceBase
 from enact.interfaces import TypeWrapperBase
 from enact.interfaces import ResourceDict
 
 from enact.invocations import _InvokableBase
 from enact.invocations import AsyncInvokableBase
 from enact.invocations import AsyncInvokable
@@ -72,14 +77,15 @@
 from enact.registration import register
 
 from enact.resource_registry import Registry
 from enact.resource_registry import RegistryError
 from enact.resource_registry import ResourceNotFound
 from enact.resource_registry import wrap
 from enact.resource_registry import unwrap
+from enact.resource_registry import deepcopy
 
 # Trigger registration of standard resource wrappers.
 import enact.type_wrappers
 
 from enact.serialization import Serializer
 from enact.serialization import JsonSerializer
 from enact.serialization import SerializationError
```

### Comparing `enact-0.4.6/src/enact/contexts.py` & `enact-0.4.7/src/enact/contexts.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 """Thread-safe context management."""
 
 import contextlib
 import contextvars
 from typing import Callable, Dict, Optional, Type, TypeVar, cast
 
 
-_context_vars: Dict[Type['Context'],
-                    contextvars.ContextVar[Optional['Context']]] = {}
+_context_vars: Dict[
+  Type['_ContextBase'],
+  contextvars.ContextVar[Optional['_ContextBase']]] = {}
 
 
 class ContextError(Exception):
   """Error raised when there is a problem with the context."""
 
 class ContextTypeError(ContextError):
   """Error raised when the context has an unexpected type"""
@@ -165,15 +166,15 @@
     self._token = context_var.set(self)
     return self
 
   async def __aexit__(self, exc_type, exc_value, traceback):
     """Exits the context."""
     context_var = self._get_context_var()
     assert self._token
-    context_var.reset(self._token)
+    context_var.reset(self._token)  # type: ignore
     await self.aexit()
     self._token = None
 
   async def aenter(self):
     """Overridable on context entry."""
 
   async def aexit(self):
@@ -181,15 +182,15 @@
 
 
 
 def register(cls: Type[ContextBaseT]) -> Type[ContextBaseT]:
   """Registers a context class."""
   assert cls not in _context_vars, (
     f'Context class already registered: {cls}')
-  ctx_var: contextvars.ContextVar[Optional[Context]] = (
+  ctx_var: contextvars.ContextVar[Optional[_ContextBase]] = (
     contextvars.ContextVar(cls.__qualname__))
   ctx_var.set(None)
   _context_vars[cls] = ctx_var
   return cls
 
 
 def register_to_superclass(superclass: Type[ContextSuperT]) -> Callable[
```

### Comparing `enact-0.4.6/src/enact/digests.py` & `enact-0.4.7/src/enact/digests.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,23 +50,23 @@
     raise interfaces.FieldTypeError(
       'Cyclic references are not allowed in field values.')
   stack.append(id(value))
   if isinstance(value, (interfaces.ResourceBase,
                         interfaces.ResourceDict)):
     items: Iterable[Tuple[str, Value]]
     if isinstance(value, interfaces.ResourceBase):
-      res_type = type(value)
+      type_id = type(value).type_id()
       # Use alphabetical ordering.
       items = sorted(value.field_items(), key=lambda x: x[0])
     else:
       assert isinstance(value, interfaces.ResourceDict)
-      res_type = value.type
+      type_id = value.type_info.type_id()
       items = sorted(value.items(), key=lambda x: x[0])
     hash_obj.update(b'res[')
-    hash_obj.update(res_type.type_id().encode('utf-8'))
+    hash_obj.update(type_id.encode('utf-8'))
     for k, v in items:
       hash_obj.update(repr(k).encode('utf-8'))
       _digest(v, hash_obj, stack)
     hash_obj.update(b']')
   elif isinstance(value, int):
     hash_obj.update(b'i')
     hash_obj.update(repr(int(value)).encode('utf-8'))
```

### Comparing `enact-0.4.6/src/enact/fastapi/__init__.py` & `enact-0.4.7/src/enact/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/src/enact/fastapi/fastapi.py` & `enact-0.4.7/src/enact/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/src/enact/function_wrappers.py` & `enact-0.4.7/src/enact/function_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,29 +264,30 @@
   # Override names and qualnames to match the wrapped function.
   for generated_type in (function_wrapper_type,
                          function_wrapper_type.method_wrapper()):
     generated_type.__module__ = fun.__module__
     generated_type.__name__ = fun.__name__
     generated_type.__qualname__ = fun.__qualname__
   function_wrapper_type.method_wrapper().__name__ += '__method_wrapper'
+  function_wrapper_type.method_wrapper().__qualname__ += '__method_wrapper'
   return function_wrapper_type
 
 
 def register(fun: C) -> C:
   """Decorator for registering a wrapped function."""
   if inspect.ismethod(fun):
     raise ValueError(
       'Bound methods (e.g., A().foo) cannot be registered. '
       'Please register the unbound function instead (e.g., A.foo)')
   wrapper_type = _create_function_wrapper(fun)
   wrapper_fun = _wrapt_wrapper(wrapper_type)(fun)
 
   # pylint: disable=protected-access
   wrapper_type._wrapper_function = [wrapper_fun]  # type: ignore
-  wrapper_type.method_wrapper()._wrapper_function = [
+  wrapper_type.method_wrapper()._wrapper_function = [  # type: ignore
     wrapper_fun]  # type: ignore
 
   resource_registry.register(wrapper_type)
   resource_registry.register(wrapper_type.method_wrapper())
   return wrapper_fun
 
 @resource_registry.register
```

### Comparing `enact-0.4.6/src/enact/gradio/__init__.py` & `enact-0.4.7/src/enact/gradio/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Top-level gradio package definitions."""
 
 try:
-  import gradio
+  import gradio  # type: ignore
 except ModuleNotFoundError as e:
   raise ModuleNotFoundError(
       'Please install gradio to enable enact.gradio') from e
 
 from enact.gradio.gradio import *
```

### Comparing `enact-0.4.6/src/enact/gradio/gradio.py` & `enact-0.4.7/src/enact/gradio/gradio.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,16 +315,15 @@
 
   def get(self, *component_values) -> Any:
     """Returns the current contents as a resource."""
     resource_dict = interfaces.ResourceDict(self._type)
     for field_name, value in zip(self._type.field_names(), component_values):
       json_val = json.loads(value)
       resource_dict[field_name] = self._serializer.from_json(json_val)
-    resource_type = resource_registry.wrap_type(self._type)
-    resource = resource_type.from_resource_dict(resource_dict)
+    resource = resource_registry.from_resource_dict(resource_dict)
     return resource_registry.unwrap(resource)
 
 
 class GUI:
   """A gradio GUI component for an invokable."""
 
   def __init__(
```

### Comparing `enact-0.4.6/src/enact/interfaces.py` & `enact-0.4.7/src/enact/interfaces.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 """Core resource interface."""
 
 import abc
 import functools
 import json
 from typing import (
-  Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union)
+  Dict, Generic, Iterable, List, NamedTuple, Optional, Tuple, Type, TypeVar,
+  Union, cast)
 
-from enact import contexts
+from enact import acyclic
 
 
 JsonLeaf = Union[int, float, str, bool, None]
 Json = Union[JsonLeaf, List['Json'], Dict[str, 'Json']]
 
 
 PRIMITIVES = (int, float, str, bytes, bool, type(None))
@@ -66,37 +67,56 @@
   """Superclass for errors where an implementaton is missing."""
 
 
 class FieldTypeError(FrameworkError):
   """Superclass for errors related to field types."""
 
 
-@contexts.register
-class _AcyclicContext(contexts.Context):
-  """Helper to safeguard against cyclic data-structures."""
-
-  def __init__(self, obj):
-    """Initializes the context."""
-    super().__init__()
-    self.parent: Optional[_AcyclicContext] = None
-    self.obj = obj
-
-  def enter(self):
-    """Check if the resource is already being committed."""
-    self.parent = _AcyclicContext.get_current()
-    parent = self.parent
-    parents: List[_AcyclicContext] = []
-    while parent is not None:
-      parents.append(parent)
-      if parent.obj is self.obj:
-        raise FieldTypeError(
-          f'Resources may not have cyclic graph structure. '
-          f'Encountered cycle: '
-          f'{" -> ".join(str(p.obj) for p in parents)}')
-      parent = parent.parent
+class TypeInfo(NamedTuple):
+  """Information about a resource type."""
+  name: str
+  distribution_info: Optional['DistributionInfo']
+
+  def type_id(self) -> str:
+    """Returns a unique string identifier for the type."""
+    return json.dumps(self.as_dict(), sort_keys=True)
+
+  def as_dict(self) -> Dict[str, Json]:
+    """Returns a dictionary representation of the distribution info."""
+    dist_info = (
+      self.distribution_info.as_dict() if self.distribution_info else None)
+    return {
+      'name': self.name,
+      'distribution_info': dist_info}
+
+  @staticmethod
+  def from_dict(d: Dict[str, Json]) -> 'TypeInfo':
+    """Instantiate TypeInfo from a dictionary."""
+    r: Dict = dict(d)
+    r['distribution_info'] = DistributionInfo.from_dict(r['distribution_info'])
+    return TypeInfo(**r)
+
+
+class DistributionInfo(NamedTuple):
+  """Information about a package where a resource is defined.
+
+  This information (together with qualified class names) is used to identify
+  compatible resources across different versions of a package.
+  """
+  name: str
+  version: str
+
+  def as_dict(self) -> Dict[str, Json]:
+    """Returns a dictionary representation of the distribution info."""
+    return {'name': self.name, 'version': self.version}
+
+  @staticmethod
+  def from_dict(d: Dict[str, Json]) -> 'DistributionInfo':
+    """Instantiate DistributionInfo from a dictionary."""
+    return DistributionInfo(**cast(Dict[str, str], d))
 
 
 class ResourceBase:
   """Base class for resources.
 
   Not an abstract base class in order to avoid meta-class conflict.
 
@@ -105,25 +125,38 @@
   that is, replacing a field by a copy should not change the meaning of the
   resource. This means, for example, that code using resources should not rely
   on aliasing assumptions (e.g., two resources sharing the same list instance).
 
   In particular, this also means that resources may not mutually reference each
   other.
   """
+  _enact_distribution_info: Optional[DistributionInfo] = None
 
   @classmethod
-  def type_descr(cls) -> Dict[str, Json]:
-    """Returns a unique descriptor for the type."""
-    return {'name': f'{cls.__module__}.{cls.__qualname__}'}
+  def type_info(cls) -> TypeInfo:
+    """Returns a descriptor for the type."""
+    return TypeInfo(
+      name=f'{cls.__module__}.{cls.__qualname__}',
+      distribution_info=cls.type_distribution_info())
+
+  @classmethod
+  def type_distribution_info(cls) -> Optional[DistributionInfo]:
+    """Returns package information for the type if set."""
+    return cls._enact_distribution_info
+
+  @classmethod
+  def set_type_distribution_info(cls, info: DistributionInfo):
+    """Sets the package information for the type."""
+    cls._enact_distribution_info = info
 
   @classmethod
   @functools.lru_cache
   def type_id(cls) -> str:
     """Returns a string descriptor of the type."""
-    return json.dumps(cls.type_descr(), sort_keys=True)
+    return cls.type_info().type_id()
 
   @classmethod
   @abc.abstractmethod
   def field_names(cls) -> Iterable[str]:
     """Returns the names of the fields of the resource."""
     raise NotImplementedError(f'{cls} does not implement field_names')
 
@@ -142,15 +175,15 @@
                   field_dict: Dict[str, FieldValue]) -> C:
     """Constructs the resource from a field dictionary."""
     raise NotImplementedError()
 
   @staticmethod
   def _to_dict_value(value: FieldValue) -> ResourceDictValue:
     """Transforms a field value to a resource dict value."""
-    with _AcyclicContext(value):
+    with acyclic.AcyclicContext(value):
       if isinstance(value, ResourceBase):
         return value.to_resource_dict()
       if isinstance(value, PRIMITIVES):
         return value
       if isinstance(value, type) and issubclass(value, ResourceBase):
         return value
       if isinstance(value, List):
@@ -163,60 +196,21 @@
           return maybe_str
         return {
           _assert_str(k): ResourceBase._to_dict_value(v)
           for k, v in value.items()}
       raise FieldTypeError(
         f'Encountered unsupported field type {type(value)}: {value}')
 
-  @staticmethod
-  def _from_dict_value(value: ResourceDictValue) -> FieldValue:
-    """Transforms a resource dict value to a field value."""
-    if isinstance(value, PRIMITIVES):
-      return value
-    if isinstance(value, type) and issubclass(value, ResourceBase):
-      return value
-    if isinstance(value, List):
-      return [ResourceBase._from_dict_value(x) for x in value]
-    if isinstance(value, ResourceDict):
-      return value.type.from_resource_dict(value)
-    if isinstance(value, Dict):
-      def _assert_str(maybe_str: str) -> str:
-        if type(maybe_str) is not str:  # pylint: disable=unidiomatic-typecheck
-          raise FieldTypeError(
-            f'Expected string key, got {type(maybe_str)}')
-        return maybe_str
-      return {
-        _assert_str(k): ResourceBase._from_dict_value(v)
-        for k, v in value.items()}
-    raise FieldTypeError(
-      f'Encountered unsupported resource '
-      f'dict value type {type(value)}: {value}')
-
-  def deepcopy_resource(self: C) -> C:
-    """Create a deep-copy of the resource."""
-    return self.from_resource_dict(self.to_resource_dict())
-
   def to_resource_dict(self: C) -> 'ResourceDict[C]':
     """Returns a ResourceDict dictionary representation."""
     result = ResourceDict(type(self))
     for field_name, value in self.field_items():
       result[field_name] = ResourceBase._to_dict_value(value)
     return result
 
-  @classmethod
-  def from_resource_dict(cls: Type[C], resorce_dict: 'ResourceDict') -> C:
-    """Constructs the resource from a ResourceDict dictionary."""
-    if not issubclass(resorce_dict.type, cls):
-      raise ResourceError(
-        f'Expected resource of type {cls}, got {resorce_dict.type}')
-    field_dict = {
-      k: ResourceBase._from_dict_value(v)
-      for k, v in resorce_dict.items()}
-    return cls.from_fields(field_dict)
-
   def set_from(self, other: 'ResourceBase'):
     """Sets the fields of this resource from another resource.
 
     Implementation of set_from is required to support replays of invokable
     resources that change their internal state during execution.
 
     Args:
@@ -225,23 +219,22 @@
 
     raise ImplementationMissing(
       f'Setting fields from another resource is not '
       f'supported by type {type(self)}.')
 
 
 class ResourceDict(Generic[C], Dict[str, ResourceDictValue]):
-  """A dictionary representing a resource with attached type info."""
+  """A dictionary representing a resource with attached TypeInfo."""
 
-  def __init__(self, resource_type: Type[C], *args, **kwargs):
+  def __init__(
+      self, resource_type: Union[Type[C], TypeInfo], *args, **kwargs):
     super().__init__(*args, **kwargs)
-    self.type = resource_type
-
-  def to_resource(self) -> C:
-    """Constructs the resource from the dictionary."""
-    return self.type.from_resource_dict(self)
+    if not isinstance(resource_type, TypeInfo):
+      resource_type = resource_type.type_info()
+    self.type_info = resource_type
 
 
 WrappedT = TypeVar('WrappedT')
 WrapperT = TypeVar('WrapperT', bound='TypeWrapperBase')
 
 
 class TypeWrapperBase(ResourceBase, Generic[WrappedT]):
```

### Comparing `enact-0.4.6/src/enact/invocation_generators.py` & `enact-0.4.7/src/enact/invocation_generators.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/src/enact/invocations.py` & `enact-0.4.7/src/enact/invocations.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
   def clear_output(self):
     """Clear the output of the invocation."""
     with self.response.modify() as response:
       response.output = None
 
   def rewind(self, num_calls=1) -> 'Invocation[I_contra, O_co]':
     """Rewinds the invocation by the specified number of calls."""
-    invocation = self.deepcopy_resource()
+    invocation = resource_registry.deepcopy(self)
     with invocation.response.modify() as response:
       response.output = None
       for _ in range(num_calls):
         if response.children:
           response.children.pop(-1)
     return invocation
 
@@ -662,52 +662,54 @@
         raise
       finally:
         self._create_invocation(output_ref, exception)
       return cast(O_co, output_value)
 
 class _InvokableBase(Generic[I_contra, O_co], interfaces.ResourceBase):
   """Base class for sync / async invokable resources."""
-  _input_type: Optional[Type[I_contra]] = None
-  _output_type: Optional[Type[O_co]] = None
+  _enact_input_type: Optional[Type[I_contra]] = None
+  _enact_output_type: Optional[Type[O_co]] = None
 
   @classmethod
   def get_input_type(cls) -> Optional[Type[I_contra]]:
     """Returns the type of the input if known."""
-    return cls._input_type
+    return cls._enact_input_type
 
   def __call__(self, *args, **kwargs):
     """Subclasses implement this directly or as async."""
     raise NotImplementedError()
 
   def call(self, *args, **kwargs):
     """Subclasses implement this directly or as async."""
     raise NotImplementedError()
 
   @classmethod
   def _check_input_type(cls, value: Any):
     """Check the input type."""
-    input_type: Optional[Type] = cls._input_type
+    input_type: Optional[Type] = cls._enact_input_type
     # pylint: disable=isinstance-second-argument-not-valid-type
     if input_type and not isinstance(value, input_type):
       raise InvokableTypeError(
-        f'Input must be of type {cls._input_type}, but got {type(value)}.')
+        f'Input must be of type {cls._enact_input_type}, '
+        f'but got {type(value)}.')
 
   @classmethod
   def _check_output_type(cls, value: Any):
     """Check the output type."""
-    output_type: Optional[Type] = cls._output_type
+    output_type: Optional[Type] = cls._enact_output_type
     # pylint: disable=isinstance-second-argument-not-valid-type
     if output_type is not None and not isinstance(value, output_type):
       raise InvokableTypeError(
-        f'Output must be of type {cls._output_type}, but got {type(value)}.')
+        f'Output must be of type {cls._enact_output_type}, '
+        f'but got {type(value)}.')
 
   @classmethod
   def get_output_type(cls) -> Optional[Type[O_co]]:
     """Returns the type of the output if known."""
-    return cls._output_type
+    return cls._enact_output_type
 
   @staticmethod
   def _process_invoke_arg(
       arg: Optional[references.Ref[I_contra]]) -> (
         references.Ref[I_contra]):
     """Processes an invocation argument."""
     if arg is None:
@@ -881,27 +883,25 @@
 
 
 I = TypeVar('I', bound=_InvokableBase)
 
 
 def typed_invokable(
     input_type: Optional[Type],
-    output_type: Optional[Type],
-    register=True) -> Callable[
+    output_type: Optional[Type]) -> Callable[
       [Type[I]], Type[I]]:
   """A decorator for creating typed invokables."""
   def _decorator(cls: Type[I]) -> Type[I]:
     """Decorates a class as a typed invokable."""
     if not issubclass(cls, _InvokableBase):
       raise TypeError('Invokable must be a subclass of InvokableBase.')
     # pylint: disable=protected-access
-    cls._input_type = input_type
-    cls._output_type = output_type
-    if register:
-      resource_registry.register(cls)
+    cls._enact_input_type = input_type
+    cls._enact_output_type = output_type
+    resource_registry.register(cls)
     return cls
   return _decorator
 
 
 @resource_registry.register
 @dataclasses.dataclass
 class RequestInput(Invokable):
```

### Comparing `enact-0.4.6/src/enact/pretty_print.py` & `enact-0.4.7/src/enact/pretty_print.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/src/enact/registration.py` & `enact-0.4.7/src/enact/registration.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/src/enact/resource_registry.py` & `enact-0.4.7/src/enact/resource_registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,197 +13,38 @@
 # limitations under the License.
 
 """Type registration functionality to allow deserialization of resources."""
 
 import inspect
 import types
 from typing import (
-  Any, Callable, Dict, Hashable, Iterable, Mapping, Optional, Set,
+  Any, Callable, Dict, Hashable, Iterable, List, Mapping, Optional, Set,
   Type, TypeVar, Union, cast)
 
+from enact import distribution_registry
 from enact import interfaces
 
+
+
 WrappedT = TypeVar('WrappedT')
 WrapperT = TypeVar('WrapperT', bound=interfaces.TypeWrapperBase)
+ResourceT = TypeVar('ResourceT', bound=interfaces.ResourceBase)
 
+FieldValueWrapperT = TypeVar('FieldValueWrapperT', bound='FieldValueWrapper')
+FunctionWrapperT = TypeVar('FunctionWrapperT', bound='FunctionWrapper')
+MethodWrapperT = TypeVar('MethodWrapperT', bound='MethodWrapper')
 
 class RegistryError(Exception):
   """Raised when there is an error with the registry."""
 
 
 class ResourceNotFound(RegistryError):
   """Raised when a resource is not found."""
 
 
-
-FieldValueWrapperT = TypeVar('FieldValueWrapperT', bound='FieldValueWrapper')
-
-
-class FieldValueWrapper(interfaces.TypeWrapperBase[WrappedT]):
-  """Base class for field value wrappers."""
-  value: interfaces.FieldValue
-
-  def __init__(self, value: interfaces.FieldValue):
-    """Initializes a wrapped field value."""
-    self.value = value
-
-  @classmethod
-  def field_names(cls) -> Iterable[str]:
-    """Returns the names of the fields of the resource."""
-    return ('wrapped',)
-
-  def field_values(self) -> Iterable[interfaces.FieldValue]:
-    return (self.value,)
-
-  @classmethod
-  def from_fields(
-      cls: Type[FieldValueWrapperT],
-      field_dict: Mapping[str, interfaces.FieldValue]) -> FieldValueWrapperT:
-    assert len(field_dict) == 1
-    return cls(field_dict['wrapped'])
-
-  def set_from(self, other: interfaces.ResourceBase):
-    """Sets the fields of this resource from another resource."""
-    if not type(self) is type(other):
-      raise RegistryError(
-        f'Cannot set fields from {type(other)} to {type(self)}.')
-    assert isinstance(other, FieldValueWrapper)
-    self.wrapped = other.deepcopy_resource().value
-
-  @classmethod
-  def wrap(cls: Type[FieldValueWrapperT],
-           value: WrappedT) -> FieldValueWrapperT:
-    """Wrap a value directly."""
-    assert isinstance(value, cls.wrapped_type()), (
-      'Cannot wrap value of type {type(value)} with wrapper {cls}.')
-    return cls(to_field_value(value))
-
-  def unwrap(self) -> WrappedT:
-    """Unwrap a value directly."""
-    assert isinstance(self.value, self.wrapped_type())
-    return from_field_value(self.value)
-
-
-class NoneWrapper(
-  interfaces.TypeWrapperBase):
-  """Wrapper for None."""
-  @classmethod
-  def wrapped_type(cls) -> Type[None]:
-    return type(None)
-
-  @classmethod
-  def field_names(cls) -> Iterable[str]:
-    """Returns the names of the fields of the resource."""
-    return ()
-
-  def field_values(self) -> Iterable[interfaces.FieldValue]:
-    return ()
-
-  @classmethod
-  def from_fields(
-      cls, field_dict: Mapping[str, interfaces.FieldValue]) -> 'NoneWrapper':
-    assert len(field_dict) == 0
-    return cls()
-
-  def set_from(self, other: interfaces.ResourceBase):
-    """Sets the fields of this resource from another resource."""
-    if not type(self) is type(other):
-      raise RegistryError(
-        f'Cannot set fields from {type(other)} to {type(self)}.')
-
-  @classmethod
-  def wrap(cls, value: WrappedT) -> 'NoneWrapper':
-    """Wrap a value directly."""
-    assert isinstance(value, cls.wrapped_type()), (
-      'Cannot wrap value of type {type(value)} with wrapper {cls}.')
-    return NoneWrapper()
-
-  def unwrap(self) -> None:
-    """Unwrap a value directly."""
-    return None
-
-
-class PrimitiveWrapper(FieldValueWrapper[WrappedT]):
-  """Wrapper for primitives."""
-
-  @classmethod
-  def is_immutable(cls) -> bool:
-    return True
-
-
-class IntWrapper(PrimitiveWrapper[int]):
-  """Wrapper for ints."""
-  @classmethod
-  def wrapped_type(cls) -> Type[int]:
-    return int
-
-
-class FloatWrapper(PrimitiveWrapper[float]):
-  """Wrapper for floats."""
-  @classmethod
-  def wrapped_type(cls) -> Type[float]:
-    return float
-
-
-class BoolWrapper(PrimitiveWrapper[bool]):
-  """Wrapper for bools."""
-  @classmethod
-  def wrapped_type(cls) -> Type[bool]:
-    return bool
-
-
-class StrWrapper(PrimitiveWrapper[str]):
-  """Wrapper for strs."""
-  @classmethod
-  def wrapped_type(cls) -> Type[str]:
-    return str
-
-
-class BytesWrapper(PrimitiveWrapper[bytes]):
-  """Wrapper for bytes."""
-  @classmethod
-  def wrapped_type(cls) -> Type[bytes]:
-    return bytes
-
-
-class ListWrapper(FieldValueWrapper[list]):
-  """Wrapper for lists."""
-  @classmethod
-  def wrapped_type(cls) -> Type[list]:
-    return list
-
-  @classmethod
-  def set_wrapped_value(cls, target: list, src: list):
-    target.clear()
-    target.extend(src)
-
-
-class DictWrapper(FieldValueWrapper[dict]):
-  """Wrapper for dicts."""
-  @classmethod
-  def wrapped_type(cls) -> Type[dict]:
-    return dict
-
-  @classmethod
-  def set_wrapped_value(cls, target: dict, src: dict):
-    target.clear()
-    target.update(src)
-
-class ResourceTypeWrapper(FieldValueWrapper[type]):
-  """Wrapper for type-valued fields."""
-
-  @classmethod
-  def wrapped_type(cls) -> Type[type]:
-    return type
-
-
-FunctionWrapperT = TypeVar('FunctionWrapperT', bound='FunctionWrapper')
-MethodWrapperT = TypeVar('MethodWrapperT', bound='MethodWrapper')
-
-
 class FunctionWrapper(interfaces.ResourceBase):
   """Base class for function wrappers.
 
   Should be subclassed as an Invokable or AsyncInvokable.
 
   Function wrapping require a three step approach:
   1) The native function is transparently wrapped using a python wrapper
@@ -267,68 +108,113 @@
     raise NotImplementedError()
 
   def get_instance(self) -> Any:
     """Added to interface to simplify typing."""
     return self.instance  # type: ignore
 
 
-
 class MissingWrapperError(interfaces.FieldTypeError):
   """Raised when a required wrapper is missing."""
 
 
 class Registry:
   """Registers resource types for deserialization."""
 
   _singleton: Optional['Registry'] = None
 
   def __init__(self):
     """Initializes a registry."""
+    # Ensure that the enact distribution is registered to its semantic version
+    # before registering any resource types.
+    distribution_registry.ensure_enact_registered()
     self.allow_reregistration = True
+
     # Map from type id to resource type.
     self._type_map: Dict[str, Type[interfaces.ResourceBase]] = {}
+
     # Map from python types to wrapper types.
     self._wrapped_types: Dict[Type, Type[interfaces.TypeWrapperBase]] = {}
     self._wrapper_types: Set[Type[interfaces.TypeWrapperBase]] = set()
     self._function_wrappers: Dict[Callable, Type[FunctionWrapper]] = {}
 
-    # Register basic wrappers for field values.
-    self.register(NoneWrapper)
-    self.register(IntWrapper)
-    self.register(FloatWrapper)
-    self.register(BoolWrapper)
-    self.register(StrWrapper)
-    self.register(BytesWrapper)
-    self.register(ListWrapper)
-    self.register(DictWrapper)
-    self.register(ResourceTypeWrapper)
+
+  def _from_dict_value(self, value: interfaces.ResourceDictValue) -> (
+      interfaces.FieldValue):
+    """Transforms a resource dict value to a field value."""
+    if isinstance(value, interfaces.PRIMITIVES):
+      return value
+    if isinstance(value, type) and issubclass(value, interfaces.ResourceBase):
+      return value
+    if isinstance(value, List):
+      return [self._from_dict_value(x) for x in value]
+    if isinstance(value, interfaces.ResourceDict):
+      return self.from_resource_dict(value)
+    if isinstance(value, Dict):
+      def _assert_str(maybe_str: str) -> str:
+        if type(maybe_str) is not str:  # pylint: disable=unidiomatic-typecheck
+          raise interfaces.FieldTypeError(
+            f'Expected string key, got {type(maybe_str)}')
+        return maybe_str
+      return {
+        _assert_str(k): self._from_dict_value(v)
+        for k, v in value.items()}
+    raise interfaces.FieldTypeError(
+      f'Encountered unsupported resource '
+      f'dict value type {type(value)}: {value}')
+
+  def deepcopy(self, resource: ResourceT) -> ResourceT:
+    """Create a deep-copy of the resource."""
+    return cast(ResourceT, self.from_resource_dict(resource.to_resource_dict()))
+
+  def from_resource_dict(self, resource_dict: interfaces.ResourceDict) -> (
+      interfaces.ResourceBase):
+    """Constructs the resource from a ResourceDict dictionary."""
+    if not isinstance(resource_dict, interfaces.ResourceDict):
+      raise TypeError(f'Input is not a ResourceDict: {resource_dict}')
+    resource_type = self.lookup(resource_dict.type_info)
+    field_dict = {
+      k: self._from_dict_value(v)
+      for k, v in resource_dict.items()}
+    return resource_type.from_fields(field_dict)
 
   def register(self, resource: Type[interfaces.ResourceBase]):
     """Registers the resource type."""
+    # Check argument type.
     if not issubclass(resource, interfaces.ResourceBase):
       raise RegistryError(
         f'Cannot register non-resource type: {resource}')
+    # Auto-add distribution info.
+    dist_info = resource.type_distribution_info()
+    if dist_info is None:
+      dist_info = distribution_registry.get_distribution_info(resource)
+      if dist_info is not None:
+        resource.set_type_distribution_info(dist_info)
+    # Record the type.
     type_id = resource.type_id()
     if (type_id in self._type_map and
         self._type_map[type_id] != resource and
         not self.allow_reregistration):
       raise RegistryError(
         f'{id(resource)} == {id(self._type_map[type_id])}\n'
         f'While registering {resource}: '
         f'Type with id {type_id} already '
         f'registered to a different type: '
         f'{self._type_map[type_id]}\n')
     self._type_map[type_id] = resource
+    # Handle special types.
     if issubclass(resource, interfaces.TypeWrapperBase):
       self._register_type_wrapper(resource)
     if issubclass(resource, FunctionWrapper):
       return self._register_function_wrapper(resource)
 
-  def lookup(self, type_id: str) -> Type[interfaces.ResourceBase]:
-    """Looks up a resource type by name."""
+  def lookup(self, type_id: Union[str, interfaces.TypeInfo]) -> (
+      Type[interfaces.ResourceBase]):
+    """Looks up a resource type by name or type_info."""
+    if isinstance(type_id, interfaces.TypeInfo):
+      type_id = type_id.type_id()
     resource_class = self._type_map.get(type_id)
     if not resource_class:
       raise ResourceNotFound(f'No type registered for {type_id}')
     return resource_class
 
   def _register_function_wrapper(self, wrapper_type: Type[FunctionWrapper]):
     """Register a function wrapper type."""
@@ -351,15 +237,15 @@
       if issubclass(t, k):
         if found:
           raise RegistryError(
             f'Found multiple wrappers for type {t}: {found} and {v}')
         found = v
     return found
 
-  def _get_function_wrapper_type(self, c: Callable) -> Type[FunctionWrapper]:
+  def _get_function_wrapper_type(self, c: Callable) -> Type['FunctionWrapper']:
     """Return the function wrapper for c or raise an error."""
     func = c
     if inspect.ismethod(c):
       func = c.__func__
     if not isinstance(func, Hashable):
       raise interfaces.FieldTypeError(
         'Only immutable callables (e.g. python functions) can be handled '
@@ -395,15 +281,15 @@
     wrapper = self.get_type_wrapper(value)
     if wrapper:
       return wrapper
     raise MissingWrapperError(
       f'Cannot wrap type {value}. Please register '
       f'a TypeWrapper for this type.')
 
-  def unwrap(self, value: interfaces.ResourceBase) -> Any:
+  def unwrap(self, value: Any) -> Any:
     """Unwrap a value if wrapped."""
     if isinstance(value, interfaces.TypeWrapperBase):
       return value.unwrap()
     if isinstance(value, FunctionWrapper):
       return value.wrapper_function()
     if isinstance(value, MethodWrapper):
       return types.MethodType(
@@ -420,37 +306,34 @@
   def get(cls) -> 'Registry':
     """Returns the singleton registry."""
     if not cls._singleton:
       cls._singleton = cls()
     return cls._singleton
 
 
-ResourceT = TypeVar('ResourceT', bound=interfaces.ResourceBase)
-
-
 def register(cls: Type[ResourceT]) -> Type[ResourceT]:
   """Decorator for resource classes."""
   Registry.get().register(cls)
   return cls
 
 
 def register_wrapper(cls: Type[WrapperT]) -> Type[WrapperT]:
   """Decorator for resource wrapper classes."""
   # pylint: disable=protected-access
   Registry.get()._register_type_wrapper(cls)
   return cls
 
 
 def wrap(value: Any) -> interfaces.ResourceBase:
-  """Wrap a value as a resource."""
+  """Wrap a value as a resource if necessary."""
   return Registry.get().wrap(value)
 
 
-def unwrap(value: interfaces.ResourceBase) -> Any:
-  """Wrap a value."""
+def unwrap(value: Any) -> Any:
+  """Unwrap a value if wrapped."""
   return Registry.get().unwrap(value)
 
 
 def wrap_type(value: Type) -> Type[interfaces.ResourceBase]:
   """Wrap a type as a resource."""
   return Registry.get().wrap_type(value)
 
@@ -458,15 +341,19 @@
 def unwrap_type(value: Type[interfaces.ResourceBase]) -> Type:
   """Wrap a type."""
   return Registry.get().unwrap_type(value)
 
 
 def deepcopy(value: WrappedT) -> WrappedT:
   """Deep copy a value."""
-  return from_field_value(to_field_value(value))
+  if isinstance(value, interfaces.ResourceBase):
+    result = from_resource_dict(value.to_resource_dict())
+  else:
+    result = unwrap(from_resource_dict(wrap(value).to_resource_dict()))
+  return cast(WrappedT, result)
 
 
 def _ensure_str_key(s: Any) -> str:
   """Ensure that a value is a string."""
   if not isinstance(s, str):
     raise ValueError(
       f'Cannot auto-wrap a dictionary with non-str keys: '
@@ -496,7 +383,178 @@
       issubclass(value, interfaces.TypeWrapperBase)):
     return unwrap_type(value)
   if isinstance(value, list):
     return [from_field_value(x) for x in value]
   if isinstance(value, dict):
     return {k: from_field_value(v) for k, v in value.items()}
   return value
+
+def from_resource_dict(resource_dict: interfaces.ResourceDict) -> (
+    interfaces.ResourceBase):
+  """Constructs the resource from a ResourceDict dictionary."""
+  return Registry.get().from_resource_dict(resource_dict)
+
+
+class FieldValueWrapper(interfaces.TypeWrapperBase[WrappedT]):
+  """Base class for field value wrappers."""
+  value: interfaces.FieldValue
+
+  def __init__(self, value: interfaces.FieldValue):
+    """Initializes a wrapped field value."""
+    self.value = value
+
+  @classmethod
+  def field_names(cls) -> Iterable[str]:
+    """Returns the names of the fields of the resource."""
+    return ('wrapped',)
+
+  def field_values(self) -> Iterable[interfaces.FieldValue]:
+    return (self.value,)
+
+  @classmethod
+  def from_fields(
+      cls: Type[FieldValueWrapperT],
+      field_dict: Mapping[str, interfaces.FieldValue]) -> FieldValueWrapperT:
+    assert len(field_dict) == 1
+    return cls(field_dict['wrapped'])
+
+  def set_from(self, other: interfaces.ResourceBase):
+    """Sets the fields of this resource from another resource."""
+    if not type(self) is type(other):
+      raise RegistryError(
+        f'Cannot set fields from {type(other)} to {type(self)}.')
+    assert isinstance(other, FieldValueWrapper)
+    self.wrapped = deepcopy(other).value
+
+  @classmethod
+  def wrap(cls: Type[FieldValueWrapperT],
+           value: WrappedT) -> FieldValueWrapperT:
+    """Wrap a value directly."""
+    assert isinstance(value, cls.wrapped_type()), (
+      'Cannot wrap value of type {type(value)} with wrapper {cls}.')
+    return cls(to_field_value(value))
+
+  def unwrap(self) -> WrappedT:
+    """Unwrap a value directly."""
+    assert isinstance(self.value, self.wrapped_type())
+    return from_field_value(self.value)
+
+
+@register
+class NoneWrapper(
+  interfaces.TypeWrapperBase):
+  """Wrapper for None."""
+  @classmethod
+  def wrapped_type(cls) -> Type[None]:
+    return type(None)
+
+  @classmethod
+  def field_names(cls) -> Iterable[str]:
+    """Returns the names of the fields of the resource."""
+    return ()
+
+  def field_values(self) -> Iterable[interfaces.FieldValue]:
+    return ()
+
+  @classmethod
+  def from_fields(
+      cls, field_dict: Mapping[str, interfaces.FieldValue]) -> 'NoneWrapper':
+    assert len(field_dict) == 0
+    return cls()
+
+  def set_from(self, other: interfaces.ResourceBase):
+    """Sets the fields of this resource from another resource."""
+    if not type(self) is type(other):
+      raise RegistryError(
+        f'Cannot set fields from {type(other)} to {type(self)}.')
+
+  @classmethod
+  def wrap(cls, value: WrappedT) -> 'NoneWrapper':
+    """Wrap a value directly."""
+    assert isinstance(value, cls.wrapped_type()), (
+      'Cannot wrap value of type {type(value)} with wrapper {cls}.')
+    return NoneWrapper()
+
+  def unwrap(self) -> None:
+    """Unwrap a value directly."""
+    return None
+
+class PrimitiveWrapper(FieldValueWrapper[WrappedT]):
+  """Wrapper for primitives."""
+
+  @classmethod
+  def is_immutable(cls) -> bool:
+    return True
+
+
+@register
+class IntWrapper(PrimitiveWrapper[int]):
+  """Wrapper for ints."""
+  @classmethod
+  def wrapped_type(cls) -> Type[int]:
+    return int
+
+
+@register
+class FloatWrapper(PrimitiveWrapper[float]):
+  """Wrapper for floats."""
+  @classmethod
+  def wrapped_type(cls) -> Type[float]:
+    return float
+
+
+@register
+class BoolWrapper(PrimitiveWrapper[bool]):
+  """Wrapper for bools."""
+  @classmethod
+  def wrapped_type(cls) -> Type[bool]:
+    return bool
+
+
+@register
+class StrWrapper(PrimitiveWrapper[str]):
+  """Wrapper for strs."""
+  @classmethod
+  def wrapped_type(cls) -> Type[str]:
+    return str
+
+
+@register
+class BytesWrapper(PrimitiveWrapper[bytes]):
+  """Wrapper for bytes."""
+  @classmethod
+  def wrapped_type(cls) -> Type[bytes]:
+    return bytes
+
+
+@register
+class ListWrapper(FieldValueWrapper[list]):
+  """Wrapper for lists."""
+  @classmethod
+  def wrapped_type(cls) -> Type[list]:
+    return list
+
+  @classmethod
+  def set_wrapped_value(cls, target: list, src: list):
+    target.clear()
+    target.extend(src)
+
+
+@register
+class DictWrapper(FieldValueWrapper[dict]):
+  """Wrapper for dicts."""
+  @classmethod
+  def wrapped_type(cls) -> Type[dict]:
+    return dict
+
+  @classmethod
+  def set_wrapped_value(cls, target: dict, src: dict):
+    target.clear()
+    target.update(src)
+
+@register
+class ResourceTypeWrapper(FieldValueWrapper[type]):
+  """Wrapper for type-valued fields."""
+
+  @classmethod
+  def wrapped_type(cls) -> Type[type]:
+    return type
```

### Comparing `enact-0.4.6/src/enact/resources.py` & `enact-0.4.7/src/enact/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,38 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Dataclass-based resources."""
 
 import abc
 import dataclasses
-from typing import Dict, Iterable, Mapping, Type, TypeVar
+from typing import Iterable, Mapping, Type, TypeVar
 
-from enact import digests
 from enact import interfaces
 from enact import resource_registry
 
 
 FieldValue = interfaces.FieldValue
 
 C = TypeVar('C', bound='_Resource')
 
 
 class _Resource(interfaces.ResourceBase):
   """Base class for Resource and FrozenResource."""
 
   @classmethod
-  def type_descr(cls) -> Dict[str, interfaces.Json]:
-    """Returns a unique identifier for the type."""
-    descr = super().type_descr()
-    assert isinstance(descr, dict)
-    descr['digest'] = digests.type_digest(cls)
-    return descr
-
-  @classmethod
   def field_names(cls) -> Iterable[str]:
     """Returns the names of the fields of the resource."""
     return (f.name for f in dataclasses.fields(cls))  # type: ignore
 
   def field_values(self) -> Iterable[FieldValue]:
     """Return a list of field values, aligned with field_names."""
     return (resource_registry.to_field_value(
@@ -70,15 +61,15 @@
     """Sets the fields of this resource from another resource.
 
     Implementation of set_from is required to support replays of invokable
     resources that change their internal state during execution.
     """
     if not type(self) == type(other):  # pylint: disable=unidiomatic-typecheck
       raise TypeError(f'Cannot set_from {type(other)} into {type(self)}.')
-    copy = other.deepcopy_resource()
+    copy = resource_registry.deepcopy(other)
     for field in dataclasses.fields(self):
       self_field = getattr(self, field.name)
       target = getattr(other, field.name)
       if self_field is target:
         continue
       if type(self_field) == type(target):  # pylint: disable=unidiomatic-typecheck
         if isinstance(self_field, interfaces.ResourceBase):
```

### Comparing `enact-0.4.6/src/enact/serialization.py` & `enact-0.4.7/src/enact/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """Escapes a string."""
     return f'{self._ESCAPE}{s}'
 
   def to_json(self, value: interfaces.ResourceDictValue) -> Json:
     """Converts a value to a JSON compatible value recursively."""
     if isinstance(value, interfaces.ResourceDict):
       result: Dict[str, Json] = {
-        self._escape('res'): (value.type.type_id())}
+        self._escape('res'): (value.type_info.type_id())}
       for k, v in value.items():
         if not isinstance(k, str):
           raise interfaces.FieldTypeError(
             f'Resource has non-string keys: {value}')
         if k.startswith(self._ESCAPE):
           raise SerializationError(
             f'Cannot serialize resource with fields starting with '
```

### Comparing `enact-0.4.6/src/enact/type_wrappers.py` & `enact-0.4.7/src/enact/type_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/src/enact/utils.py` & `enact-0.4.7/tests/test_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Utility functions and classes."""
-from typing import Any, Dict, Optional
 
-import enact
+"""Checks that the package version and python version match."""
+
+import os
+import unittest
+import re
 
-# pylint: disable=invalid-name
-class cached_property(property):
-  """A property that caches its result based on the digest of the resource.
+import enact
 
-  NOTE: This is effectively an LRU cache with a maxsize of 1, so the cache
-  is cleared when the digest of the resource changes.
-  """
-  def __init__(self, user_function):
-    self._user_function = user_function
-    self._cache: Dict[str, Any] = {}
-    super().__init__()
+class TestVersion(unittest.TestCase):
+  """Tests for the version."""
 
-  def __get__(self, instance: Any, unused_owner: Optional[type] = None):
-    """Cached property based on the digest of the resource."""
-    digest = enact.resource_digest(instance)
-    result = self._cache.get(digest, None)
-    if result is None:
-      result = self._user_function(instance)
-      self._cache = {digest: result}
-    return result
+  def test_version(self):
+    """Tests that the version matches."""
+    try:
+      pyproject_path = os.path.join(
+          os.path.dirname(__file__), os.pardir, 'pyproject.toml')
+      with open(pyproject_path, 'r', encoding='utf8') as f:
+        pyproject_contents = f.read()
+    except FileNotFoundError:
+      self.skipTest('pyproject.toml not found')
+    # Python 3.8 does not have tomllib, so we use a regex instead.
+    pyproject_contents = re.search(r'version = "(.*)"', pyproject_contents)
+    pyproject_version = pyproject_contents.group(1)
+    self.assertEqual(enact.__version__, pyproject_version)
```

### Comparing `enact-0.4.6/src/enact.egg-info/PKG-INFO` & `enact-0.4.7/src/enact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enact
-Version: 0.4.6
+Version: 0.4.7
 Summary: A framework for generative software.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `enact-0.4.6/src/enact.egg-info/SOURCES.txt` & `enact-0.4.7/src/enact.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 LICENSE
 README.md
 pyproject.toml
 src/enact/__init__.py
+src/enact/acyclic.py
 src/enact/contexts.py
 src/enact/digests.py
+src/enact/distribution_registry.py
 src/enact/function_wrappers.py
 src/enact/interfaces.py
 src/enact/invocation_generators.py
 src/enact/invocations.py
 src/enact/pretty_print.py
 src/enact/py.typed
 src/enact/references.py
 src/enact/registration.py
 src/enact/resource_digests.py
 src/enact/resource_registry.py
 src/enact/resources.py
 src/enact/serialization.py
 src/enact/type_wrappers.py
 src/enact/utils.py
+src/enact/version.py
 src/enact.egg-info/PKG-INFO
 src/enact.egg-info/SOURCES.txt
 src/enact.egg-info/dependency_links.txt
 src/enact.egg-info/requires.txt
 src/enact.egg-info/top_level.txt
 src/enact/fastapi/__init__.py
 src/enact/fastapi/fastapi.py
 src/enact/gradio/__init__.py
 src/enact/gradio/gradio.py
 tests/test_contexts.py
 tests/test_digest.py
+tests/test_distribution_registry.py
 tests/test_function_wrappers.py
 tests/test_invocation_generator.py
 tests/test_invocations.py
 tests/test_pretty_print.py
 tests/test_references.py
 tests/test_registration.py
 tests/test_resource_registry.py
 tests/test_resources.py
 tests/test_serialize.py
 tests/test_type_wrappers.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_version.py
```

### Comparing `enact-0.4.6/tests/test_contexts.py` & `enact-0.4.7/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/tests/test_digest.py` & `enact-0.4.7/tests/test_digest.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/tests/test_function_wrappers.py` & `enact-0.4.7/tests/test_function_wrappers.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/tests/test_invocation_generator.py` & `enact-0.4.7/tests/test_invocation_generator.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/tests/test_invocations.py` & `enact-0.4.7/tests/test_invocations.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 """Tests for invocations."""
 
 import asyncio
 import dataclasses
 import random
 import tempfile
 import time
-from typing import Optional, cast
+from typing import Any, Optional, cast
 import unittest
 from unittest import mock
 
 import enact
 from enact import invocations
 
+@enact.register
 class ValueErrorResource(invocations.ExceptionResource):
   """A value error that is also a resource."""
 
 
 @enact.typed_invokable(int, str)
 @dataclasses.dataclass
 class IntToStr(enact.Invokable):
@@ -43,27 +44,28 @@
 @enact.typed_invokable(int, str)
 class WrongOutputType(enact.Invokable):
 
   def call(self, value: int) -> str:
     return value  # type: ignore
 
 
-@dataclasses.dataclass
 @enact.typed_invokable(int, int)
+@dataclasses.dataclass
 class AddOne(enact.Invokable):
   fail: bool = False
   def call(self, input_resource: int) -> int:
     if self.fail:
       raise ValueErrorResource('fail')
     return input_resource + 1
 
 
+@enact.register
 @dataclasses.dataclass
 class Fail(enact.Invokable):
-  def call(self, arg: enact.ResourceBase) -> int:
+  def call(self, arg: Any) -> int:
     raise ValueErrorResource('fail')
 
 
 @enact.typed_invokable(int, int)
 @dataclasses.dataclass
 class NestedFunction(enact.Invokable):
   """A nested function that repeatedly calls another invokable."""
@@ -303,44 +305,53 @@
       self.assertFalse(subinvocation.get_raised_here())
       (subsubinvocation,) = subinvocation.get_children()
       self.assertTrue(subsubinvocation.get_raised_here())
 
   def test_no_reraise_in_replay(self):
     """Tests that exceptions are replayed."""
     native_errors_raised = 0
+    @enact.register
     class PythonErrorOnInvoke(enact.Invokable):
       def call(self, unused_input: enact.ResourceBase):
         nonlocal native_errors_raised
         native_errors_raised += 1
         raise ValueErrorResource('foo')
 
+    @enact.register
     @dataclasses.dataclass
     class SubCall(enact.Invokable):
       invokable: enact.Ref[enact.InvokableBase]
       def call(self, input_resource: enact.ResourceBase):
         self.invokable.checkout()(input_resource)
 
+    @enact.register
+    @dataclasses.dataclass
+    class MyResource(enact.Resource):
+      value: int
+
     with self.store as store:
       error_fun = PythonErrorOnInvoke()
       subcall_1 = SubCall(store.commit(error_fun))
       subcall_2 = SubCall(store.commit(subcall_1))
-      invocation = subcall_2.invoke(store.commit(5))
+      invocation = subcall_2.invoke(store.commit(MyResource(5)))
       self.assertEqual(native_errors_raised, 1)
       with self.assertRaises(ValueErrorResource):
         with invocations.ReplayContext(subinvocations=[
             enact.commit(invocation)]):
-          subcall_2(5)
+          subcall_2(MyResource(5))
       self.assertEqual(native_errors_raised, 2)
 
 
   def test_input_changed_error(self):
+    @enact.register
     @dataclasses.dataclass
     class Changeable(enact.Resource):
       x: int = 0
 
+    @enact.register
     class ChangesInput(enact.Invokable):
       def call(self, input_resource: Changeable):
         input_resource.x += 1
         return input_resource
 
     with self.assertRaises(enact.InputChanged):
       with self.store as store:
```

### Comparing `enact-0.4.6/tests/test_pretty_print.py` & `enact-0.4.7/tests/test_pretty_print.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/tests/test_registration.py` & `enact-0.4.7/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `enact-0.4.6/tests/test_resource_registry.py` & `enact-0.4.7/tests/test_resource_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for the resource_registry module."""
 
 import dataclasses
+import os
 import types
 from typing import Any, List, Tuple, Type
 import unittest
+from unittest import mock
 
 import enact
 from enact import resource_registry
+from enact import version
+from enact import distribution_registry
+
 
 @enact.register
 @dataclasses.dataclass
 class SimpleResource(enact.Resource):
   """A simple resource for testing."""
 
 
@@ -269,10 +274,33 @@
     copy = resource_registry.deepcopy(nest)
     self.assertEqual(copy, nest)
     self.assertIsNot(copy, nest)
     self.assertIsNot(copy[0], nest[0])
     self.assertIsNot(copy[1], nest[1])
     self.assertIsNot(copy[1]['a'], nest[1]['a'])
 
+  def test_enact_types_have_distribution_info(self):
+    """Tests that type distribution info is present for enact types."""
+    self.assertEqual(
+      resource_registry.IntWrapper.type_distribution_info(),
+      enact.DistributionInfo(version.DIST_NAME, version.__version__))
+
+  def test_auto_assign_distribution_info(self):
+    """Tests that type distribution info is auto-assigned on register"""
+    dist_registry = distribution_registry.DistributionRegistry()
+
+    # Patch out the singleton distribution registry.
+    with mock.patch.object(
+        distribution_registry, 'registry',  lambda: dist_registry):
+      dist_registry.register_distribution(
+        'enact-tests', '0.0.1', os.path.dirname(__file__))
+      class MyResource(enact.Resource):
+        pass
+      self.assertIsNone(MyResource.type_distribution_info())
+      enact.register(MyResource)
+      self.assertEqual(
+        MyResource.type_distribution_info(),
+        enact.DistributionInfo('enact-tests', '0.0.1'))
+
 
 if __name__ == 'main':
   unittest.main()
```

### Comparing `enact-0.4.6/tests/test_resources.py` & `enact-0.4.7/tests/test_resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,26 @@
 
 
 import dataclasses
 from typing import Any, Type
 import unittest
 
 import enact
+from enact import resource_registry
 
 
+@enact.register
 @dataclasses.dataclass
 class SimpleResource(enact.Resource):
   a: Any
   b: Any
   c: Any
 
 
+@enact.register
 @dataclasses.dataclass
 class OtherSimpleResource(enact.Resource):
   a: Any
   b: Any
   c: Any
 
 
@@ -55,26 +58,14 @@
   def test_field_items(self):
     """Tests that field_items works."""
     r = SimpleResource(1, 2, 3)
     self.assertEqual(
       list(r.field_items()),
       [('a', 1), ('b', 2), ('c', 3)])
 
-  def test_type_id_different_fields(self):
-    """Tests that the type id differs based on field."""
-    @dataclasses.dataclass
-    class R(enact.Resource):
-      a: Any
-    type_id = R.type_id()
-    # pylint: disable=function-redefined
-    @dataclasses.dataclass
-    class R(enact.Resource):  # type: ignore
-      b: Any
-    self.assertNotEqual(type_id, R.type_id())
-
   def test_type_id_same_fields(self):
     """Tests that the type id is correct."""
     @dataclasses.dataclass
     class R(enact.Resource):
       a: Any
     type_id = R.type_id()
     # pylint: disable=function-redefined
@@ -113,44 +104,44 @@
       w: Custom
       i: int
 
     r = CustomFieldsResource(Custom(1), 2)
     as_dict = r.to_resource_dict()
     w_dict = as_dict['w']
     assert isinstance(w_dict, enact.ResourceDict)
-    self.assertEqual(w_dict.type, CustomWrapper)
-    rebuilt = as_dict.to_resource()
+    self.assertEqual(w_dict.type_info, CustomWrapper.type_info())
+    rebuilt = resource_registry.from_resource_dict(as_dict)
     self.assertEqual(r.w.x, rebuilt.w.x)
     self.assertEqual(r.i, rebuilt.i)
 
 class RefTest(unittest.TestCase):
 
   def test_digest_identical(self):
     """Test that digest is identical for identical resources."""
     a = SimpleResource(1, 2, 3)
     b = SimpleResource(1, 2, 3)
-    r1 = enact.Ref.pack(a)
-    r2 = enact.Ref.pack(b)
+    _, r1 = enact.Ref.pack(a)
+    _, r2 = enact.Ref.pack(b)
     self.assertEqual(r1, r2)
 
   def test_typename_changes_hash(self):
     """Tests that changing the typename changes the hash."""
     a = SimpleResource(1, 2, 3)
     b = OtherSimpleResource(1, 2, 3)
-    r1 = enact.Ref.pack(a)
-    r2 = enact.Ref.pack(b)
-    self.assertNotEqual(r1.ref, r2.ref)
+    _, r1 = enact.Ref.pack(a)
+    _, r2 = enact.Ref.pack(b)
+    self.assertNotEqual(r1.ref(), r2.ref())
 
   def test_value_changes_hash(self):
     """Tests that changing values changes the hash."""
     a = SimpleResource(1, 2, 3)
     b = SimpleResource(1, 2, 4)
-    r1 = enact.Ref.pack(a)
-    r2 = enact.Ref.pack(b)
-    self.assertNotEqual(r1.ref, r2.ref)
+    _, r1 = enact.Ref.pack(a)
+    _, r2 = enact.Ref.pack(b)
+    self.assertNotEqual(r1.ref(), r2.ref())
 
   def test_hash_complex_nested(self):
     """Tests that nested resources are hashed correctly."""
     a = SimpleResource(
       [1, None, 2.0, True, False],
       [{'a': {'b': {'c': 1}}}],
       enact.Ref('1234'))
@@ -171,19 +162,19 @@
     """Tests that including an unknown type will raise an error."""
     class X:
       pass
     a = SimpleResource(X(), 2, 3)
     with self.assertRaises(enact.FieldTypeError):
       enact.Ref.pack(a)
 
-  def test_deepy_copy_resource(self):
+  def test_deep_copy_resource(self):
     """Tests that the resource can be deep-copied."""
     a = SimpleResource(SimpleResource(1, 2, 3), [4, None],
                        {'a': 0.0, 'b': [True, False]})
-    b = a.deepcopy_resource()
+    b = enact.deepcopy(a)
     self.assertEqual(a, b)
     self.assertNotEqual(id(a), id(b))
     self.assertNotEqual(id(a.a), id(b.a))
     self.assertNotEqual(id(a.b), id(b.b))
     self.assertNotEqual(id(a.c), id(b.c))
     self.assertEqual(enact.Ref.pack(a), enact.Ref.pack(b))
```

### Comparing `enact-0.4.6/tests/test_serialize.py` & `enact-0.4.7/tests/test_serialize.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,18 +52,20 @@
     """Tests that serialization/deserialization works."""
     self.registry.register(AllTypesResource)
     resource = AllTypesResource(
       i=2, f=3.0, bl=True, b=b'bytes', s='test', n=None,
       r=enact.Ref('12314'), m={'a': ['test']}, l=[{'b': 1}, {'c': 2}],
       t=AllTypesResource)
     got = self.serializer.serialize(resource.to_resource_dict())
-    deserialized = self.serializer.deserialize(got).to_resource()
+    deserialized = resource_registry.from_resource_dict(
+      self.serializer.deserialize(got))
     self.assertEqual(deserialized, resource)
 
   def test_serialize_deserialize_fuzz(self):
     """Fuzz test serialization and deserialization."""
     self.registry.register(random_value.R)
     for _ in range(100):
       resource = random_value.rand_resource()
       got = self.serializer.serialize(resource.to_resource_dict())
-      deserialized = self.serializer.deserialize(got).to_resource()
+      deserialized = resource_registry.from_resource_dict(
+        self.serializer.deserialize(got))
       self.assertEqual(deserialized, resource)
```

### Comparing `enact-0.4.6/tests/test_type_wrappers.py` & `enact-0.4.7/tests/test_type_wrappers.py`

 * *Files identical despite different names*


# Comparing `tmp/funcnodes-0.2.tar.gz` & `tmp/funcnodes-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes-0.2.tar", max compression
+gzip compressed data, was "funcnodes-0.2.1.tar", max compression
```

## Comparing `funcnodes-0.2.tar` & `funcnodes-0.2.1.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0     1648 2024-04-25 07:48:14.233810 funcnodes-0.2/funcnodes/__init__.py
--rw-r--r--   0        0        0     4533 2024-04-25 08:16:17.311632 funcnodes-0.2/funcnodes/__main__.py
--rw-r--r--   0        0        0     1236 2024-04-11 10:18:38.447318 funcnodes-0.2/funcnodes/_logging.py
--rw-r--r--   0        0        0      313 2024-04-11 20:53:13.157950 funcnodes-0.2/funcnodes/basic_nodes/__init__.py
--rw-r--r--   0        0        0     3365 2024-04-12 04:03:36.180995 funcnodes-0.2/funcnodes/basic_nodes/files.py
--rw-r--r--   0        0        0     3234 2024-03-22 12:20:39.208910 funcnodes-0.2/funcnodes/basic_nodes/logic.py
--rw-r--r--   0        0        0    11280 2024-03-22 12:20:39.204313 funcnodes-0.2/funcnodes/basic_nodes/math.py
--rw-r--r--   0        0        0     2645 2024-04-25 09:50:41.189375 funcnodes-0.2/funcnodes/config.py
--rw-r--r--   0        0        0    21052 2024-03-04 21:41:10.617653 funcnodes-0.2/funcnodes/eventmanager.py
--rw-r--r--   0        0        0       54 2024-02-23 07:11:27.803639 funcnodes-0.2/funcnodes/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2/funcnodes/frontends/__init__.py
--rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2/funcnodes/frontends/funcnodes_react/__init__.py
--rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2/funcnodes/frontends/funcnodes_react/asset-manifest.json
--rw-r--r--   0        0        0    28362 2024-04-25 08:34:16.885037 funcnodes-0.2/funcnodes/frontends/funcnodes_react/css/style.css
--rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2/funcnodes/frontends/funcnodes_react/favicon.ico
--rw-r--r--   0        0        0      658 2024-04-25 08:27:16.808142 funcnodes-0.2/funcnodes/frontends/funcnodes_react/index.html
--rw-r--r--   0        0        0  4138461 2024-04-25 08:27:16.808142 funcnodes-0.2/funcnodes/frontends/funcnodes_react/js/424.js
--rw-r--r--   0        0        0     3258 2024-04-25 08:27:16.808142 funcnodes-0.2/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt
--rw-r--r--   0        0        0   246139 2024-04-25 08:34:16.885037 funcnodes-0.2/funcnodes/frontends/funcnodes_react/js/main.js
--rw-r--r--   0        0        0    11348 2024-04-25 08:27:16.808142 funcnodes-0.2/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
--rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2/funcnodes/frontends/funcnodes_react/logo192.png
--rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2/funcnodes/frontends/funcnodes_react/logo512.png
--rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2/funcnodes/frontends/funcnodes_react/manifest.json
--rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2/funcnodes/frontends/funcnodes_react/robots.txt
--rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2/funcnodes/frontends/funcnodes_react/run.py
--rw-r--r--   0        0        0    27821 2024-03-26 10:45:48.904252 funcnodes-0.2/funcnodes/io.py
--rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2/funcnodes/lib/__init__.py
--rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2/funcnodes/lib/lib.py
--rw-r--r--   0        0        0     4984 2024-04-24 09:12:14.855752 funcnodes-0.2/funcnodes/lib/libfinder.py
--rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2/funcnodes/lib/libparser.py
--rw-r--r--   0        0        0    30703 2024-04-25 09:09:36.230702 funcnodes-0.2/funcnodes/node.py
--rw-r--r--   0        0        0    12512 2024-03-22 05:11:28.909207 funcnodes-0.2/funcnodes/nodemaker.py
--rw-r--r--   0        0        0     8792 2024-03-22 14:22:28.093134 funcnodes-0.2/funcnodes/nodespace.py
--rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2/funcnodes/triggerstack.py
--rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2/funcnodes/utils/__init__.py
--rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2/funcnodes/utils/data.py
--rw-r--r--   0        0        0     2744 2024-02-23 07:11:27.812331 funcnodes-0.2/funcnodes/utils/nodeutils.py
--rw-r--r--   0        0        0     4785 2024-04-16 09:49:12.882143 funcnodes-0.2/funcnodes/utils/serialization.py
--rw-r--r--   0        0        0      417 2024-03-08 10:17:34.548477 funcnodes-0.2/funcnodes/worker/__init__.py
--rw-r--r--   0        0        0     1150 2024-03-19 15:11:29.279085 funcnodes-0.2/funcnodes/worker/external_worker.py
--rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2/funcnodes/worker/loop.py
--rw-r--r--   0        0        0     4439 2024-04-16 08:30:59.942933 funcnodes-0.2/funcnodes/worker/websocket.py
--rw-r--r--   0        0        0    40882 2024-04-24 12:54:22.537255 funcnodes-0.2/funcnodes/worker/worker.py
--rw-r--r--   0        0        0    22709 2024-04-12 11:14:29.469695 funcnodes-0.2/funcnodes/worker/worker_manager.py
--rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2/LICENSE
--rw-r--r--   0        0        0      665 2024-04-25 07:48:23.084307 funcnodes-0.2/pyproject.toml
--rw-r--r--   0        0        0       38 2023-10-26 07:00:17.799913 funcnodes-0.2/README.md
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 funcnodes-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1680 2024-05-08 12:53:16.958919 funcnodes-0.2.1/funcnodes/__init__.py
+-rw-r--r--   0        0        0     6499 2024-05-07 08:28:48.305494 funcnodes-0.2.1/funcnodes/__main__.py
+-rw-r--r--   0        0        0     2032 2024-05-06 20:07:59.075924 funcnodes-0.2.1/funcnodes/_logging.py
+-rw-r--r--   0        0        0      313 2024-04-11 20:53:13.157950 funcnodes-0.2.1/funcnodes/basic_nodes/__init__.py
+-rw-r--r--   0        0        0     4391 2024-05-07 07:50:51.041520 funcnodes-0.2.1/funcnodes/basic_nodes/files.py
+-rw-r--r--   0        0        0     3474 2024-05-07 07:39:01.326392 funcnodes-0.2.1/funcnodes/basic_nodes/logic.py
+-rw-r--r--   0        0        0    11280 2024-05-05 22:02:37.701451 funcnodes-0.2.1/funcnodes/basic_nodes/math.py
+-rw-r--r--   0        0        0     3593 2024-05-06 20:07:58.990311 funcnodes-0.2.1/funcnodes/config.py
+-rw-r--r--   0        0        0    22123 2024-05-07 08:27:31.506589 funcnodes-0.2.1/funcnodes/eventmanager.py
+-rw-r--r--   0        0        0      125 2024-05-06 20:08:00.654935 funcnodes-0.2.1/funcnodes/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-26 12:43:49.198582 funcnodes-0.2.1/funcnodes/frontends/__init__.py
+-rw-r--r--   0        0        0       28 2024-02-26 12:44:57.877828 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-25 08:06:56.551013 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/asset-manifest.json
+-rw-r--r--   0        0        0    28362 2024-04-25 08:34:16.885037 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/css/style.css
+-rw-r--r--   0        0        0     3870 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/favicon.ico
+-rw-r--r--   0        0        0      658 2024-04-25 08:27:16.808142 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/index.html
+-rw-r--r--   0        0        0  4138461 2024-04-25 08:27:16.808142 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/424.js
+-rw-r--r--   0        0        0     3258 2024-04-25 08:27:16.808142 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt
+-rw-r--r--   0        0        0   246139 2024-04-25 08:34:16.885037 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/main.js
+-rw-r--r--   0        0        0    11348 2024-04-25 08:27:16.808142 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt
+-rw-r--r--   0        0        0     5347 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/logo192.png
+-rw-r--r--   0        0        0     9664 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/logo512.png
+-rw-r--r--   0        0        0      492 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/manifest.json
+-rw-r--r--   0        0        0       67 2024-01-19 12:49:44.602000 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/robots.txt
+-rw-r--r--   0        0        0     2952 2024-04-25 08:14:13.637341 funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/run.py
+-rw-r--r--   0        0        0    27882 2024-05-06 04:17:35.134204 funcnodes-0.2.1/funcnodes/io.py
+-rw-r--r--   0        0        0      421 2024-04-12 04:01:45.484336 funcnodes-0.2.1/funcnodes/lib/__init__.py
+-rw-r--r--   0        0        0     6807 2024-03-19 15:11:29.279085 funcnodes-0.2.1/funcnodes/lib/lib.py
+-rw-r--r--   0        0        0     7107 2024-05-08 11:06:44.923372 funcnodes-0.2.1/funcnodes/lib/libfinder.py
+-rw-r--r--   0        0        0     1792 2024-04-16 04:49:07.183174 funcnodes-0.2.1/funcnodes/lib/libparser.py
+-rw-r--r--   0        0        0    31452 2024-05-07 15:29:57.471965 funcnodes-0.2.1/funcnodes/node.py
+-rw-r--r--   0        0        0    19738 2024-05-07 08:39:11.933956 funcnodes-0.2.1/funcnodes/nodemaker.py
+-rw-r--r--   0        0        0    11850 2024-05-07 03:17:09.186518 funcnodes-0.2.1/funcnodes/nodespace.py
+-rw-r--r--   0        0        0     3043 2024-02-23 07:11:27.809136 funcnodes-0.2.1/funcnodes/triggerstack.py
+-rw-r--r--   0        0        0      362 2024-02-23 07:11:27.812331 funcnodes-0.2.1/funcnodes/utils/__init__.py
+-rw-r--r--   0        0        0     3189 2024-04-11 08:37:44.578407 funcnodes-0.2.1/funcnodes/utils/data.py
+-rw-r--r--   0        0        0     2744 2024-02-23 07:11:27.812331 funcnodes-0.2.1/funcnodes/utils/nodeutils.py
+-rw-r--r--   0        0        0     5271 2024-05-07 08:22:20.139829 funcnodes-0.2.1/funcnodes/utils/serialization.py
+-rw-r--r--   0        0        0      444 2024-05-07 13:05:54.019733 funcnodes-0.2.1/funcnodes/worker/__init__.py
+-rw-r--r--   0        0        0     1808 2024-05-07 08:35:08.888378 funcnodes-0.2.1/funcnodes/worker/external_worker.py
+-rw-r--r--   0        0        0     3736 2024-03-26 07:43:19.651903 funcnodes-0.2.1/funcnodes/worker/loop.py
+-rw-r--r--   0        0        0     3293 2024-05-07 08:43:41.552734 funcnodes-0.2.1/funcnodes/worker/remote_worker.py
+-rw-r--r--   0        0        0     8270 2024-05-07 08:43:38.346889 funcnodes-0.2.1/funcnodes/worker/websocket.py
+-rw-r--r--   0        0        0    37914 2024-05-07 08:42:49.613686 funcnodes-0.2.1/funcnodes/worker/worker.py
+-rw-r--r--   0        0        0    30152 2024-05-06 20:08:11.694569 funcnodes-0.2.1/funcnodes/worker/worker_manager.py
+-rw-r--r--   0        0        0     1091 2023-10-26 07:00:17.799913 funcnodes-0.2.1/LICENSE
+-rw-r--r--   0        0        0      666 2024-05-08 12:53:01.277391 funcnodes-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    13174 2024-05-07 11:03:57.250582 funcnodes-0.2.1/README.md
+-rw-r--r--   0        0        0    13528 1970-01-01 00:00:00.000000 funcnodes-0.2.1/PKG-INFO
```

### Comparing `funcnodes-0.2/funcnodes/__init__.py` & `funcnodes-0.2.1/funcnodes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     NodeInput,
     NodeOutput,
     NodeIO,
     NodeInputSerialization,
     NodeOutputSerialization,
     NodeConnectionError,
     MultipleConnectionsError,
+    NoValue,
     SameNodeConnectionError,
 )
 from .utils import run_until_complete, JSONEncoder, JSONDecoder
 from .node import Node, get_nodeclass, NodeJSON
 from .nodespace import NodeSpace, FullNodeSpaceJSON, NodeSpaceJSON
 from .lib import FullLibJSON, Shelf, Library, find_shelf, NodeClassNotFoundError
 from .nodemaker import NodeClassMixin, NodeDecorator, instance_nodefunction
@@ -17,14 +18,15 @@
 from .worker import (
     FuncNodesExternalWorker,
     RemoteWorker,
     WSWorker,
     WorkerManager,
     assert_worker_manager_running,
 )
+
 from . import config
 from .config import RenderOptions
 
 __all__ = [
     "NodeInput",
     "NodeOutput",
     "NodeIO",
@@ -55,12 +57,13 @@
     "FuncNodesExternalWorker",
     "RemoteWorker",
     "WSWorker",
     "WorkerManager",
     "assert_worker_manager_running",
     "config",
     "RenderOptions",
+    "NoValue",
 ]
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 DEBUG = True
```

### Comparing `funcnodes-0.2/funcnodes/basic_nodes/logic.py` & `funcnodes-0.2.1/funcnodes/basic_nodes/logic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Logic Nodes for control flow and decision making."""
 
 from funcnodes.node import Node, TriggerStack
-from typing import Any, List
+from typing import Any, List, Optional
 from funcnodes.io import NodeInput, NodeOutput, NoValue
 import asyncio
 from funcnodes.lib import module_to_shelf
 import sys
 
 
 class IfNode(Node):
@@ -63,23 +63,28 @@
     node_id = "for_node"
     node_name = "For"
     input = NodeInput(id="input", type=List[Any])
     do = NodeOutput(id="do", type=Any)
     collector = NodeInput(id="collector", type=Any, does_trigger=False, required=False)
     done = NodeOutput(id="done", type=List[Any])
 
-    async def func(self, input: list) -> None:
+    async def func(self, input: list, collector: Optional[Any] = None) -> None:
         results = []
         for i in input:
             self.outputs["do"].set_value(i, does_trigger=False)
             triggerstack = TriggerStack()
-
-            await self.outputs["do"].trigger(triggerstack)
-            await triggerstack
-            results.append(self.inputs["collector"].value)
+            try:
+                await self.outputs["do"].trigger(triggerstack)
+                await triggerstack
+            except Exception as e:
+                pass
+            v = self.inputs["collector"].value
+            if v is not NoValue:
+                results.append(v)
+                self.inputs["collector"].value = NoValue
         self.outputs["done"].value = results
 
 
 class CollectorNode(Node):
     node_id = "collector_node"
     node_name = "Collector"
```

### Comparing `funcnodes-0.2/funcnodes/basic_nodes/math.py` & `funcnodes-0.2.1/funcnodes/basic_nodes/math.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/config.py` & `funcnodes-0.2.1/funcnodes/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,140 @@
-from typing import TypedDict
-import os
-import json
-from .utils import deep_fill_dict
-
-from dotenv import load_dotenv
-from exposedfunctionality.function_parser.types import type_to_string
-
-load_dotenv(override=True)
-
-
-BASE_CONFIG_DIR = os.environ.get(
-    "FUNCNODES_CONFIG_DIR", os.path.join(os.path.expanduser("~"), ".funcnodes")
-)
-
-DEFAULT_CONFIG = {
-    "env_dir": os.path.join(BASE_CONFIG_DIR, "env"),
-    "worker_manager": {
-        "host": "localhost",
-        "port": 9380,
-    },
-    "frontend": {
-        "port": 8000,
-    },
-}
-
-
-CONFIG = DEFAULT_CONFIG
-CONFIG_DIR = BASE_CONFIG_DIR
-
-
-def load_config(path):
-    global CONFIG
-    if not os.path.exists(path):
-        config = DEFAULT_CONFIG
-    else:
-        with open(path, "r") as f:
-            config = json.load(f)
-    deep_fill_dict(config, DEFAULT_CONFIG)
-    with open(path, "w") as f:
-        json.dump(config, f, indent=2)
-    CONFIG = config
-
-
-def check_config_dir():
-    global CONFIG_DIR
-    if not os.path.exists(BASE_CONFIG_DIR):
-        os.makedirs(BASE_CONFIG_DIR)
-    load_config(os.path.join(BASE_CONFIG_DIR, "config.json"))
-    if "custom_config_dir" in CONFIG:
-        load_config(os.path.join(CONFIG["custom_config_dir"], "config.json"))
-        CONFIG_DIR = CONFIG["custom_config_dir"]
-
-
-check_config_dir()
-
-
-class RenderOptions(TypedDict, total=False):
-    typemap: dict[str, str]
-    inputconverter: dict[str, str]
-
-
-FUNCNODES_RENDER_OPTIONS: RenderOptions = {"typemap": {}, "inputconverter": {}}
-
-
-def update_render_options(options: RenderOptions):
-    if not isinstance(options, dict):
-        return
-    if "typemap" not in options:
-        options["typemap"] = {}
-    for k, v in list(options["typemap"].items()):
-        if not isinstance(k, str):
-            del options["typemap"][k]
-            k = type_to_string(k)
-            options["typemap"][k] = v
-
-        if not isinstance(v, str):
-            v = type_to_string(v)
-            options["typemap"][k] = v
-
-    if "inputconverter" not in options:
-        options["inputconverter"] = {}
-    for k, v in list(options["inputconverter"].items()):
-        if not isinstance(k, str):
-            del options["typemap"][k]
-            k = type_to_string(k)
-            options["inputconverter"][k] = v
-        if not isinstance(v, str):
-            v = type_to_string(v)
-            options["inputconverter"][k] = v
-        FUNCNODES_RENDER_OPTIONS["inputconverter"][k] = v
-
-    # make sure its json serializable
-    try:
-        json.dumps(options)
-    except json.JSONDecodeError:
-        return
-    deep_fill_dict(
-        FUNCNODES_RENDER_OPTIONS, options, merge_lists=True, unfify_lists=True
-    )
+from typing import TypedDict
+import os
+import json
+from .utils import deep_fill_dict
+
+from dotenv import load_dotenv
+from exposedfunctionality.function_parser.types import type_to_string
+
+load_dotenv(override=True)
+
+
+BASE_CONFIG_DIR = os.environ.get(
+    "FUNCNODES_CONFIG_DIR", os.path.join(os.path.expanduser("~"), ".funcnodes")
+)
+
+DEFAULT_CONFIG = {
+    "env_dir": os.path.join(BASE_CONFIG_DIR, "env"),
+    "worker_manager": {
+        "host": "localhost",
+        "port": 9380,
+    },
+    "frontend": {
+        "port": 8000,
+    },
+}
+
+
+CONFIG = DEFAULT_CONFIG
+CONFIG_DIR = BASE_CONFIG_DIR
+
+
+def load_config(path):
+    """
+    Loads the configuration file.
+
+    Args:
+      path (str): The path to the configuration file.
+
+    Returns:
+      None
+
+    Examples:
+      >>> load_config("config.json")
+    """
+    global CONFIG
+    if not os.path.exists(path):
+        config = DEFAULT_CONFIG
+    else:
+        with open(path, "r") as f:
+            config = json.load(f)
+    deep_fill_dict(config, DEFAULT_CONFIG)
+    with open(path, "w") as f:
+        json.dump(config, f, indent=2)
+    CONFIG = config
+
+
+def check_config_dir():
+    """
+    Checks the configuration directory.
+
+    Returns:
+      None
+
+    Examples:
+      >>> check_config_dir()
+    """
+    global CONFIG_DIR
+    if not os.path.exists(BASE_CONFIG_DIR):
+        os.makedirs(BASE_CONFIG_DIR)
+    load_config(os.path.join(BASE_CONFIG_DIR, "config.json"))
+    if "custom_config_dir" in CONFIG:
+        load_config(os.path.join(CONFIG["custom_config_dir"], "config.json"))
+        CONFIG_DIR = CONFIG["custom_config_dir"]
+
+
+check_config_dir()
+
+
+class RenderOptions(TypedDict, total=False):
+    """
+    A typed dictionary for render options.
+
+    Attributes:
+      typemap (dict[str, str]): A dictionary mapping types to strings.
+      inputconverter (dict[str, str]): A dictionary mapping input types to strings.
+    """
+    typemap: dict[str, str]
+    inputconverter: dict[str, str]
+
+
+FUNCNODES_RENDER_OPTIONS: RenderOptions = {"typemap": {}, "inputconverter": {}}
+
+
+def update_render_options(options: RenderOptions):
+    """
+    Updates the render options.
+
+    Args:
+      options (RenderOptions): The render options to update.
+
+    Returns:
+      None
+
+    Examples:
+      >>> update_render_options({"typemap": {"int": "int32"}, "inputconverter": {"str": "string"}})
+    """
+    if not isinstance(options, dict):
+        return
+    if "typemap" not in options:
+        options["typemap"] = {}
+    for k, v in list(options["typemap"].items()):
+        if not isinstance(k, str):
+            del options["typemap"][k]
+            k = type_to_string(k)
+            options["typemap"][k] = v
+
+        if not isinstance(v, str):
+            v = type_to_string(v)
+            options["typemap"][k] = v
+
+    if "inputconverter" not in options:
+        options["inputconverter"] = {}
+    for k, v in list(options["inputconverter"].items()):
+        if not isinstance(k, str):
+            del options["typemap"][k]
+            k = type_to_string(k)
+            options["inputconverter"][k] = v
+        if not isinstance(v, str):
+            v = type_to_string(v)
+            options["inputconverter"][k] = v
+        FUNCNODES_RENDER_OPTIONS["inputconverter"][k] = v
+
+    # make sure its json serializable
+    try:
+        json.dumps(options)
+    except json.JSONDecodeError:
+        return
+    deep_fill_dict(
+        FUNCNODES_RENDER_OPTIONS, options, merge_lists=True, unfify_lists=True
+    )
```

### Comparing `funcnodes-0.2/funcnodes/eventmanager.py` & `funcnodes-0.2.1/funcnodes/eventmanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,20 @@
         self._obj = weakref.ref(obj)
         self._lock = (
             asyncio.Lock()
         )  # Lock to ensure thread-safe access to the _async_events dictionary.
 
     @property
     def obj(self) -> Any:
+        """
+        Returns the object associated with the AsyncEventManager.
+
+        Returns:
+          Any: The object associated with the AsyncEventManager.
+        """
         return self._obj()
 
     async def wait(self, event: str) -> None:
         """
         Waits for the event to be set before continuing.
 
         Args:
@@ -107,55 +113,79 @@
             pass
 
 
 class MessageInArgs(dict):
     """MessageInArgs class is a dictionary that has src as a reserved required keyword
     but also accepts arbitary other ones."""
 
-    def __init__(
-        self,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        # if "src" not in self:
-        #    raise ValueError("src is a required keyword")
-
     @property
     def src(self) -> EventEmitterMixin:
+        """
+        Returns the src property of the MessageInArgs object.
+
+        Returns:
+          EventEmitterMixin: The src property of the MessageInArgs object.
+        """
         return self["src"]
 
     @src.setter
     def src(self, value: EventEmitterMixin):
+        """
+        Sets the src property of the MessageInArgs object.
+
+        Args:
+          value (EventEmitterMixin): The value to set the src property to.
+        """
         if not isinstance(value, EventEmitterMixin):
             raise TypeError("src must be an instance of EventEmitterMixin")
         self["src"] = value
 
 
 GenericMessageInArgs = TypeVar("GenericMessageInArgs", bound=MessageInArgs)
 
 
 class EventCallback(Protocol, Generic[GenericMessageInArgs]):
+    """
+    Callback Protocol for events.
+    """
+
     def __call__(self, **kwargs: Unpack[GenericMessageInArgs]) -> Any:  # type: ignore
+        """
+        Calls the EventCallback.
+
+        Args:
+          kwargs (Unpack[GenericMessageInArgs]): Keyword arguments for the callback.
+
+        Returns:
+          Any: The result of the callback.
+        """
         """Callback for events.""" ""
 
 
 class EventErrorCallback(Protocol):
+    """
+    Callback for event errors.
+    """
+
     def __call__(self, error: Exception, src: Any):
         """Callback for error events."""
 
 
 class EventEmitterMixin:
     """EventEmitterMixin is a mixin class that provides methods for
     emitting and listening to events.
     """
 
     default_listeners: Dict[str, List[EventCallback]] = {}
     default_error_listeners: List[EventErrorCallback] = []
 
     def __init__(self, *args, **kwargs):
+        """
+        Initializes a new EventEmitterMixin object.
+        """
         self._events: Dict[str, List[EventCallback]] = {}
         self._error_events: List[EventErrorCallback] = []
         super().__init__(*args, **kwargs)
         for event_name, listeners in self.default_listeners.items():
             for listener in listeners:
                 self.on(event_name, listener)
 
@@ -171,14 +201,17 @@
         # Remove error event listeners
         self.off_error()
 
         # Additional cleanup tasks here
 
     # Ensure to call cleanup before the object is deleted
     def __del__(self):
+        """
+        Cleans up the EventEmitterMixin object upon deletion.
+        """
         self.cleanup()
 
     def on(self, event_name: str, callback: EventCallback):
         """Adds a listener to the end of the listeners array for the specified event.
 
         Parameters
         ----------
@@ -247,14 +280,17 @@
         event_name : str
             The name of the event.
         callback : EventCallback
             The callback function.
         """
 
         def _callback(*args, **kwargs):
+            """
+            wrapper function to remove the listener after the first call.
+            """
             self.off(event_name, _callback)
             callback(*args, **kwargs)
 
         self.on(event_name, _callback)
 
     def once_error(self, callback: EventErrorCallback):
         """Adds a one time listener for the error event. This listener is invoked only the next
@@ -263,14 +299,17 @@
         Parameters
         ----------
         callback : EventErrorCallback
             The callback function.
         """
 
         def _callback(error: Exception, src: EventEmitterMixinGen):
+            """
+            wrapper function to remove the listener after the first call.
+            """
             self.off_error(_callback)
             callback(error, src=src)
 
         self.on_error(_callback)
 
     def emit(self, event_name: str, msg: MessageInArgs | None = None) -> bool:
         """Execute each of the listeners in order with the supplied arguments.
```

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/asset-manifest.json` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/css/style.css` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/css/style.css`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/favicon.ico` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/favicon.ico`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/index.html` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/index.html`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/js/424.js` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/424.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/424.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/js/main.js` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/main.js`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/js/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/logo192.png` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/logo192.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/logo512.png` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/logo512.png`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/frontends/funcnodes_react/run.py` & `funcnodes-0.2.1/funcnodes/frontends/funcnodes_react/run.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/io.py` & `funcnodes-0.2.1/funcnodes/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,14 +445,17 @@
             trg.uuid,
         ]
 
     def c(self, *args, **kwargs):
         """Alias for connect."""
         return self.connect(*args, **kwargs)
 
+    def __gt__(self, other):
+        self.connect(other)
+
     @emit_before()
     @emit_after()
     def disconnect(self, other: Optional[NodeIO] = None):
         """Disconnects this NodeIO instance from another NodeIO instance, or all if no specific one is provided.
 
         Args:
             other: The NodeIO instance to disconnect from. If None, disconnects from all.
```

### Comparing `funcnodes-0.2/funcnodes/lib/lib.py` & `funcnodes-0.2.1/funcnodes/lib/lib.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/lib/libparser.py` & `funcnodes-0.2.1/funcnodes/lib/libparser.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/node.py` & `funcnodes-0.2.1/funcnodes/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,22 +451,38 @@
 
     @property
     def triggerstack(self) -> Optional[TriggerStack]:
         """The trigger stack associated with the node's execution."""
         return self._triggerstack
 
     @property
-    def outputs(self):
+    def outputs(self) -> Dict[str, NodeOutput]:
+        """returns a dictionary of the outputs of this node
+        in the format {output.uuid:output}
+        """
         return {op.uuid: op for op in self._outputs}
 
     @property
-    def inputs(self):
+    def o(self) -> Dict[str, NodeOutput]:
+        """short for self.outputs"""
+        return self.outputs
+
+    @property
+    def inputs(self) -> Dict[str, NodeInput]:
+        """returns a dictionary of the inputs of this node
+        in the format {input.uuid:input}
+        """
         return {ip.uuid: ip for ip in self._inputs}
 
     @property
+    def i(self) -> Dict[str, NodeInput]:
+        """short for self.inputs"""
+        return self.inputs
+
+    @property
     def in_trigger(self):
         """Whether the node is currently in a trigger state."""
         if self._triggerstack is not None:
             if self._triggerstack.done():
                 self._triggerstack = None
         return self._triggerstack is not None
 
@@ -685,20 +701,20 @@
                 ip.uuid: ip.value for ip in self._inputs if ip.value is not NoValue
             }
             err = None
             if "_triggerinput" in kwargs:
                 del kwargs["_triggerinput"]
             try:
                 ans = await self.func(**kwargs)
+                # reset the inputs if requested
+                if self.reset_inputs_on_trigger:
+                    for ip in self._inputs:
+                        ip.set_value(ip.default, does_trigger=False)
             except Exception as e:
                 err = e
-            # reset the inputs if requested
-            if self.reset_inputs_on_trigger:
-                for ip in self._inputs:
-                    ip.value = NoValue
 
             self.emit("triggerdone")
             # set the triggerdone event
             await self.asynceventmanager.set_and_clear("triggerdone")
             if err:
                 self.error(NodeTriggerError.from_error(err))
                 ans = err
@@ -753,14 +769,20 @@
         a = await self._triggerstack
         return a
 
     async def wait_for_trigger_finish(self):
         if self.in_trigger:
             await self.asynceventmanager.wait("triggerdone")
 
+    async def await_until_complete(self):
+        """
+        Asynchronously runs the node until completion.
+        """
+        return await run_until_complete(self)
+
     def __await__(self):
         """
         Allows an instance of Node to be awaited. This will request the node to be triggered and
         waits for the trigger process to finish.
         Yields:
             The result of awaiting the last task in the stack.
         """
```

### Comparing `funcnodes-0.2/funcnodes/nodespace.py` & `funcnodes-0.2.1/funcnodes/nodespace.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 
 
 from .eventmanager import EventEmitterMixin, MessageInArgs, emit_after
 from .utils.serialization import JSONEncoder, JSONDecoder
 
 
 class NodeException(Exception):
+    """
+    Base exception class for node exceptions.
+    """
+
     pass
 
 
 class FullNodeSpaceJSON(TypedDict):
     """
     FullNodeSpaceJSON for a full serilization including temporary properties
     """
@@ -45,50 +49,82 @@
     nodes: List[NodeJSON]
     edges: List[Tuple[str, str, str, str]]
     prop: Dict[str, Any]
 
 
 class NodeSpace(EventEmitterMixin):
     """
-    NodeSpace is a collection of nodes and edges between them
+    NodeSpace is a manager and container for nodes and edges between them.
+    Also it contains a reference to a library of nodes.
     """
 
     def __init__(self, id: str | None = None):
+        """
+        Initializes a new NodeSpace object.
+
+        Args:
+          id (str | None): Optional ID for the NodeSpace. Defaults to None.
+
+        """
         super().__init__()
         self._nodes: Dict[str, Node] = {}
         self._properties: Dict[str, Any] = {}
         self.lib = Library()
         if id is None:
             id = uuid4().hex
         self._id = id
 
     # region Properties
     @property
     def id(self) -> str:
+        """
+        Returns the ID of the NodeSpace.
+
+        Returns:
+          str: The ID of the NodeSpace.
+        """
         return self._id
 
     @property
     def nodes(self) -> List[Node]:
+        """
+        Returns a list of all nodes in the NodeSpace.
+
+        Returns:
+          List[Node]: A list of all nodes in the NodeSpace.
+        """
         return list(self._nodes.values())
 
     @property
     def edges(self) -> List[Tuple[NodeOutput, NodeInput]]:
+        """
+        Returns a list of all edges in the NodeSpace.
+
+        Returns:
+          List[Tuple[NodeOutput, NodeInput]]: A list of all edges in the NodeSpace.
+        """
         edges: List[Tuple[NodeOutput, NodeInput]] = []
         for node in self.nodes:
             for output in node.outputs.values():
                 for input in output.connections:
                     edges.append((output, input))
 
         return edges
 
     # endregion Properties
 
     # region serialization
 
     def full_serialize(self) -> FullNodeSpaceJSON:
+        """
+        Serializes the NodeSpace and all of its nodes and edges.
+
+        Returns:
+          FullNodeSpaceJSON: A JSON object containing the serialized NodeSpace.
+        """
         return {
             "nodes": [node.full_serialize() for node in self.nodes],
             "prop": self._properties,
             "lib": self.lib.full_serialize(),
             "edges": self.serialize_edges(),
         }
 
@@ -114,14 +150,20 @@
             except NodeClassNotFoundError:
                 node_cls = PlaceHolderNode
             node_instance = node_cls()
             node_instance.deserialize(node)
             self.add_node_instance(node_instance)
 
     def deserialize_edges(self, data: List[Tuple[str, str, str, str]]):
+        """
+        Deserializes the edges in the NodeSpace.
+
+        Args:
+          data (List[Tuple[str, str, str, str]]): A list of tuples containing the UUIDs and IDs of the connected nodes.
+        """
         for output_uuid, output_id, input_uuid, input_id in data:
             try:
                 output = self.get_node_by_id(output_uuid).get_input_or_output(output_id)
                 input = self.get_node_by_id(input_uuid).get_input_or_output(input_id)
                 if isinstance(output, NodeOutput) and isinstance(input, NodeInput):
                     input.connect(output)
                 else:
@@ -139,14 +181,20 @@
         """
         ret = []
         for node in self.nodes:
             ret.append(node.serialize())
         return json.loads(json.dumps(ret, cls=JSONEncoder), cls=JSONDecoder)
 
     def serialize_edges(self) -> List[Tuple[str, str, str, str]]:
+        """
+        Serializes the edges in the NodeSpace.
+
+        Returns:
+          List[Tuple[str, str, str, str]]: A list of tuples containing the UUIDs and IDs of the connected nodes.
+        """
         return [
             (output.node.uuid, output.uuid, input.node.uuid, input.uuid)
             for output, input in self.edges
             if output.node is not None and input.node is not None
         ]
 
     def deserialize(self, data: NodeSpaceJSON):
@@ -206,29 +254,53 @@
         node_ser = node.serialize()
         msg = MessageInArgs(node=node_ser)
         self.emit("node_added", msg)
 
         return node
 
     def on_node_event(self, event: str, src: Node, **data):
+        """
+        Handles events emitted by nodes in the NodeSpace.
+
+        Args:
+          event (str): The name of the event.
+          src (Node): The node that emitted the event.
+          **data: Additional data passed with the event.
+        """
         msg = MessageInArgs(node=src.uuid, **data)
         self.emit(event, msg)
 
     def on_node_error(self, src: Node, error: Exception):
+        """
+        Handles errors emitted by nodes in the NodeSpace.
+
+        Args:
+          src (Node): The node that emitted the error.
+          error (Exception): The error that was emitted.
+        """
         key = "node_error"
         if isinstance(error, NodeTriggerError):
             key = "node_trigger_error"
         self.emit(
             key,
             MessageInArgs(
                 node=src.uuid, error=error, tb=traceback.format_exception(error)
             ),
         )
 
     def remove_node_instance(self, node: Node) -> str:
+        """
+        Removes a node instance from the NodeSpace.
+
+        Args:
+          node (Node): The node instance to remove.
+
+        Returns:
+          str: The UUID of the removed node.
+        """
         if node.uuid not in self._nodes:
             raise ValueError(f"node with uuid '{node.uuid}' not found in nodespace")
 
         node = self._nodes.pop(node.uuid)
         node.off("*", self.on_node_event)
 
         for output in node.outputs.values():
@@ -246,45 +318,82 @@
         self.emit("node_removed", msg)
         uuid = node.uuid
         node.prepdelete()
         del node
         return uuid
 
     def add_node_by_id(self, id: str, **kwargs):
+        """
+        Adds a new node instance to the NodeSpace using its ID.
+
+        Args:
+          id (str): The ID of the node to add.
+          **kwargs: Additional keyword arguments to pass to the node constructor.
+
+        Returns:
+          Node: The newly added node instance.
+        """
         # find node in lib
         node_cls = self.lib.get_node_by_id(id)
         if node_cls is None:
             raise ValueError(f"node with id '{id}' not found in lib")
 
         node = node_cls(**kwargs)
         return self.add_node_instance(node)
 
     def remove_node_by_id(self, nid: str) -> str | None:
+        """
+        Removes a node from the nodespace by its id.
+
+        Args:
+          nid (str): The id of the node to remove.
+
+        Returns:
+          str | None: The id of the removed node, or None if the node was not found.
+        """
         try:
             return self.remove_node_instance(self.get_node_by_id(nid))
         except ValueError as e:
             pass
 
     # endregion add/remove nodes
 
     def get_node_by_id(self, nid: str) -> Node:
+        """
+        Gets a node from the nodespace by its id.
+
+        Args:
+          nid (str): The id of the node to get.
+
+        Returns:
+          Node: The node with the given id.
+        """
         if nid not in self._nodes:
             raise ValueError(f"node with id '{nid}' not found in nodespace")
         return self._nodes[nid]
 
     # endregion nodes
 
     # region edges
     # region add/remove edges
     # endregion add/remove edges
     # endregion edges
 
     # region lib
     @emit_after()
     def add_shelf(self, shelf: Shelf):
+        """
+        Adds a shelf to the nodespace's library.
+
+        Args:
+          shelf (Shelf): The shelf to add.
+
+        Returns:
+          Library: The updated library.
+        """
         self.lib.add_shelf(shelf)
         return self.lib
 
     # endregion lib
     async def await_done(
         self,
     ):
```

### Comparing `funcnodes-0.2/funcnodes/triggerstack.py` & `funcnodes-0.2.1/funcnodes/triggerstack.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/utils/data.py` & `funcnodes-0.2.1/funcnodes/utils/data.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/utils/nodeutils.py` & `funcnodes-0.2.1/funcnodes/utils/nodeutils.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/utils/serialization.py` & `funcnodes-0.2.1/funcnodes/utils/serialization.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,22 +2,45 @@
 import json
 import base64
 
 VALID_JSON_TYPE = Union[int, float, str, bool, list, dict, type(None)]
 
 
 class JSONDecoder(json.JSONDecoder):
+    """
+    Custom JSON decoder that uses a list of decoders to decode JSON objects.
+
+    Args:
+      object_hook (Callable): A function that will be called with the result of any object literal decoded (a dict). The return value of object_hook will be used instead of the dict. This feature can be used to implement custom decoders (e.g. JSON-RPC class hinting).
+
+    Examples:
+      >>> JSONDecoder().decode('{"__complex__": true}', object_hook=complex_decoder)
+      (1+2j)
+    """
+
     decoder: List[Callable[[VALID_JSON_TYPE], tuple[Any, bool]]] = []
 
     def __init__(self, *args, **kwargs) -> None:
+        """
+        Initializes a new JSONDecoder object.
+        """
         kwargs["object_hook"] = JSONDecoder._object_hook
         super().__init__(*args, **kwargs)
 
     @classmethod
     def add_decoder(cls, dec: Callable[[VALID_JSON_TYPE], tuple[Any, bool]]):
+        """
+        Adds a new decoder to the list of decoders.
+
+        Args:
+          dec (Callable[[VALID_JSON_TYPE], tuple[Any, bool]]): A function that takes in a valid JSON type and returns a tuple containing the decoded object and a boolean indicating whether or not the object was decoded.
+
+        Examples:
+          >>> JSONDecoder.add_decoder(complex_decoder)
+        """
         cls.decoder.append(dec)
 
     @classmethod
     def _object_hook(cls, obj: VALID_JSON_TYPE):
         """"""
         if isinstance(obj, dict):
             for key in list(obj.keys()):
@@ -30,27 +53,44 @@
         for dec in JSONDecoder.decoder:
             res, handled = dec(obj)
             if handled:
                 return res
         return obj
 
 
-encodertyoe = Callable[
+encodertype = Callable[
     [Any, bool],
-    Union[tuple[Any, Literal[True]], tuple[Any, Literal[False]]],
+    tuple[Any, bool],
 ]
 
 
 class JSONEncoder(json.JSONEncoder):
-    encoder: List[encodertyoe] = []
+    """
+    Custom JSON encoder that uses a list of encoders to encode JSON objects.
+    """
+
+    encoder: List[encodertype] = []
 
     default_preview = False
 
     @classmethod
-    def add_encoder(cls, enc: encodertyoe):
+    def add_encoder(cls, enc: encodertype):
+        """
+        Adds a new encoder to the list of encoders.
+
+        Args:
+          enc (encodertyoe): A function that takes in an object and a boolean indicating whether or not to use a default preview and returns a tuple containing the encoded object and a boolean indicating whether or not the object was encoded.
+
+        Examples:
+          >>> def complex_encoder(obj, preview=False):
+          ...     if isinstance(obj, complex):
+          ...         return {"__complex__": True}, True
+          ...     return obj, False
+          >>> JSONEncoder.add_encoder(complex_encoder)
+        """
         cls.encoder.append(enc)
 
     @classmethod
     def apply_custom_encoding(cls, obj, preview=False):
         """
         Recursively apply custom encoding to an object, using the encoders defined in JSONEncoder.
         """
@@ -72,96 +112,51 @@
         else:
             # Attempt to apply custom encodings
             for enc in cls.encoder:
                 res, handled = enc(obj, preview)
                 if handled:
                     return cls.apply_custom_encoding(res)
 
+        # Fallback to string representation
         return str(obj)
 
     def default(self, obj):
-        return self.apply_custom_encoding(obj, self.default_preview)
+        """
+        Applies custom encoding to an object.
 
+        Args:
+          obj (Any): The object to be encoded.
 
-class PreviewJSONEncoder(JSONEncoder):
-    default_preview = True
+        Returns:
+          Any: The encoded object.
 
+        Examples:
+          >>> JSONEncoder.default(obj)
+        """
+        return self.apply_custom_encoding(obj, self.default_preview)
 
-def _repr_json_(obj, preview=False):
+
+def _repr_json_(obj, preview=False) -> Tuple[Any, bool]:
+    """
+    Encodes objects that have a _repr_json_ method.
+    """
     if hasattr(obj, "_repr_json_"):
         return obj._repr_json_(), True
     return obj, False
 
 
 JSONEncoder.add_encoder(_repr_json_)
 
 
 def bytes_handler(obj, preview=False):
+    """
+    Encodes bytes objects to base64 strings.
+    """
     if isinstance(obj, bytes):
         # Convert bytes to base64 string
         if preview:
             return base64.b64encode(obj).decode("utf-8")[:100], True
         return base64.b64encode(obj).decode("utf-8"), True
     return obj, False
 
 
 JSONEncoder.add_encoder(bytes_handler)
-
-
-def default_encodings(obj, preview=False):
-    if isinstance(obj, (tuple, set)):
-        return list(obj), True
-    if isinstance(obj, Exception):
-        return str(obj), True
-
-    return obj, False
-
-
-JSONEncoder.add_encoder(default_encodings)
-
-
-# Add image encoding
-try:
-    import cv2
-    from PIL import Image
-    import numpy as np
-
-    def cv2_imageHandler(obj: Image.Image, preview=False):
-        if isinstance(obj, Image.Image):
-
-            if preview:
-                obj.thumbnail((200, 200))
-
-            aobj = np.array(obj)
-
-            retval, buffer_cv2 = cv2.imencode(
-                ".jpeg",
-                cv2.cvtColor(aobj, cv2.COLOR_RGB2BGR),
-                [int(cv2.IMWRITE_JPEG_QUALITY), 50],
-            )
-            return buffer_cv2.tobytes(), True
-        return obj, False
-
-    JSONEncoder.add_encoder(cv2_imageHandler)
-except ImportError:
-    pass
-
-try:
-    from PIL import Image
-    import io
-
-    def imageHandler(obj: Image.Image, preview=False):
-        if isinstance(obj, Image.Image):
-            if preview:
-                obj.thumbnail((200, 200))
-
-            buffer = io.BytesIO()
-            obj.save(
-                buffer, format="webp", optimize=True, quality=50
-            )  # You can use 'JPEG' or other formats as needed
-            buffered_img_bytes = buffer.getvalue()
-            return buffered_img_bytes, True
-        return obj, False
-
-    JSONEncoder.add_encoder(imageHandler)
-except ImportError:
-    pass
```

### Comparing `funcnodes-0.2/funcnodes/worker/external_worker.py` & `funcnodes-0.2.1/funcnodes/worker/external_worker.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,50 @@
 from typing import Dict, List
 from funcnodes.worker.loop import CustomLoop
 from funcnodes import NodeClassMixin  # , instance_nodefunction
 from weakref import WeakValueDictionary
 
 
 class FuncNodesExternalWorker(NodeClassMixin, CustomLoop):
+    """
+    A class that represents an external worker with a loop and nodeable methods.
+    """
+
     RUNNING_WORKERS: Dict[str, WeakValueDictionary[str, FuncNodesExternalWorker]] = {}
     IS_ABSTRACT = True
 
     def __init__(self, workerid) -> None:
-        super().__init__(delay=1)
+        """
+        Initializes the FuncNodesExternalWorker class.
+
+        Args:
+          workerid (str): The id of the worker.
+        """
+        super().__init__(
+            delay=1,
+        )
         self.uuid = workerid
         if self.NODECLASSID not in FuncNodesExternalWorker.RUNNING_WORKERS:
-            FuncNodesExternalWorker.RUNNING_WORKERS[
-                self.NODECLASSID
-            ] = WeakValueDictionary()
+            FuncNodesExternalWorker.RUNNING_WORKERS[self.NODECLASSID] = (
+                WeakValueDictionary()
+            )
         FuncNodesExternalWorker.RUNNING_WORKERS[self.NODECLASSID][self.uuid] = self
 
     @classmethod
     def running_instances(cls) -> List[FuncNodesExternalWorker]:
+        """
+        Returns a list of running instances of FuncNodesExternalWorker.
+
+        Returns:
+          List[FuncNodesExternalWorker]: A list of running instances of FuncNodesExternalWorker.
+
+        Examples:
+          >>> FuncNodesExternalWorker.running_instances()
+          [FuncNodesExternalWorker("worker1"), FuncNodesExternalWorker("worker2")]
+        """
         if cls.NODECLASSID not in FuncNodesExternalWorker.RUNNING_WORKERS:
             return []
         return list(FuncNodesExternalWorker.RUNNING_WORKERS[cls.NODECLASSID].values())
 
 
 __all__ = [
     "FuncNodesExternalWorker",
```

### Comparing `funcnodes-0.2/funcnodes/worker/loop.py` & `funcnodes-0.2.1/funcnodes/worker/loop.py`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/funcnodes/worker/worker.py` & `funcnodes-0.2.1/funcnodes/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,18 +516,14 @@
     env_path: str
     python_path: str
 
     shelves_dependencies: List[ShelfDict]
     worker_dependencies: List[WorkerDict]
 
 
-class RemoteWorkerJson(WorkerJson):
-    pass
-
-
 class Worker(ABC):
     def __init__(
         self,
         data_path: str | None = None,
         default_nodes: List[Shelf] | None = None,
         nodespace_delay=0.005,
         local_worker_lookup_delay=5,
@@ -742,15 +738,14 @@
     @property
     def nodespace_id(self) -> str:
         return self._nodespace_id
 
     # endregion properties
 
     def add_local_worker(self, worker_class: Type[FuncNodesExternalWorker], nid: str):
-        print("AAAAAAA")
         return self.local_worker_lookup_loop.start_local_worker(worker_class, nid)
 
     @exposed_method()
     def add_external_worker(self, module: str, cls_module: str, cls_name: str):
         for wdep in self._worker_dependencies:
             if wdep["module"] == module:
                 for wcls in wdep["worker_classes"]:
@@ -966,15 +961,18 @@
     def add_shelf_by_module(self, module: str):
         return self.add_shelf(module)
 
     def add_worker_dependency(self, src: WorkerDict):
         if src not in self._worker_dependencies:
             self._worker_dependencies.append(src)
             for worker_class in src["worker_classes"]:
-                if worker_class["_classref"] not in self.local_worker_lookup_loop.worker_classes:
+                if (
+                    worker_class["_classref"]
+                    not in self.local_worker_lookup_loop.worker_classes
+                ):
                     self.local_worker_lookup_loop.worker_classes.append(
                         worker_class["_classref"]
                     )
 
     @exposed_method()
     def add_worker_package(self, src: Union[str, WorkerDict], save=True):
         self.set_progress_state_sync(
@@ -1208,93 +1206,7 @@
     id: str
 
 
 class NodeSpaceEvent(TypedDict):
     type: Literal["nsevent"]
     event: str
     data: Dict[str, Any]
-
-
-class RemoteWorker(Worker):
-    def __init__(self, *args, trigger_delay=0.05, data_delay=0.2, **kwargs) -> None:
-        super().__init__(*args, **kwargs)
-
-        self._messagehandlers: List[
-            Callable[[dict], Awaitable[Tuple[bool | None, str]]]
-        ] = []
-
-    async def set_progress_state(self, *args, **kwargs):
-        await super().set_progress_state(*args, **kwargs)
-        await self.send(ProgressStateMessage(type="progress", **self._progress_state))
-
-    async def send(self, data, **kwargs):
-        data = json.dumps(data, cls=JSONEncoder)
-        # self.logger.debug(f"Sending message {data}")
-        await self.sendmessage(data, **kwargs)
-
-    @abstractmethod
-    async def sendmessage(self, msg: str, **kwargs):
-        """send a message to the frontend"""
-
-    def _on_nodespaceevent(self, event, src: NodeSpace, **kwargs):
-        if event in {
-            "before_set_value",
-            "before_request_trigger",
-            "after_request_trigger",
-            "before_disconnect",
-            "before_connect",
-            "before_trigger",
-            "after_trigger",
-        }:
-            return
-        if event == "node_trigger_error":
-            self.logger.exception(kwargs["error"])
-        event_bundle: NodeSpaceEvent = {
-            "type": "nsevent",
-            "event": event,
-            "data": kwargs,
-        }
-
-        self.loop_manager.async_call(self.send(event_bundle))
-        return event_bundle
-
-    def _on_nodespaceerror(
-        self,
-        error: Exception,
-        src: NodeSpace,
-    ):
-        """handle nodespace errors"""
-        error_bundle = {
-            "type": "error_event",
-            "error": repr(error),
-            "tb": list(traceback.TracebackException.from_exception(error).format()),
-        }
-        self.logger.exception(error)
-        self.loop_manager.async_call(self.send(error_bundle))
-
-    async def recieve_message(self, json_msg: dict, **sendkwargs):
-        self.logger.debug(f"Recieved message {json_msg}")
-        if "type" not in json_msg:
-            return
-        try:
-            if json_msg["type"] == "cmd":
-                await self._handle_cmd_msg(json_msg, **sendkwargs)
-        except Exception as e:
-            self.logger.exception(e)
-            await self.send(
-                ErrorMessage(
-                    type="error",
-                    error=str(e),
-                    tb=traceback.format_exception(e),
-                    id=json_msg.get("id"),
-                )
-            )
-
-    async def _handle_cmd_msg(self, json_msg: CmdMessage, **sendkwargs):
-        result = await self.run_cmd(json_msg)
-        await self.send(
-            ResultMessage(type="result", result=result, id=json_msg.get("id")),
-            **sendkwargs,
-        )
-
-    def generate_config(self) -> RemoteWorkerJson:
-        return super().generate_config()
```

### Comparing `funcnodes-0.2/LICENSE` & `funcnodes-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcnodes-0.2/pyproject.toml` & `funcnodes-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "funcnodes"
-version = "0.2"
+version = "0.2.1"
 description = "funcnodes"
 authors = ["Julian Kimmig <julian.kimmig@linkdlab.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-exposedfunctionality = ">=0.3.5"
+exposedfunctionality = "^0.3.6"
 websockets = "^12.0"
 virtualenv = "^20.25.1"
 poetry-plugin-export = "^1.7.1"
 python-dotenv = "^1.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
```


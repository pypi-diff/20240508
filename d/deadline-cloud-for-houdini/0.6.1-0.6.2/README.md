# Comparing `tmp/deadline_cloud_for_houdini-0.6.1.tar.gz` & `tmp/deadline_cloud_for_houdini-0.6.2.tar.gz`

## Comparing `deadline_cloud_for_houdini-0.6.1.tar` & `deadline_cloud_for_houdini-0.6.2.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/_version.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/HoudiniAdaptor.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/__init__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py
--rw-r--r--   0        0        0    20824 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/__init__.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/_version.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/INDEX__SECTION
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Sections.list
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/houdini.hdalibrary
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/CreateScript
--rw-r--r--   0        0        0    23586 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Help
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/PythonModule
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Sections.list
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/TypePropertiesOptions
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_version.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml
--rw-r--r--   0        0        0    14973 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py
--rw-r--r--   0        0        0    28434 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/NOTICE
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/README.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/hatch.toml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/_version.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/HoudiniAdaptor.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/__init__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py
+-rw-r--r--   0        0        0    20824 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py
+-rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/_version.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/INDEX__SECTION
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Sections.list
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/houdini.hdalibrary
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/CreateScript
+-rw-r--r--   0        0        0    23586 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Help
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/PythonModule
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Sections.list
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/TypePropertiesOptions
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/__init__.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_assets.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/_version.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml
+-rw-r--r--   0        0        0    14973 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py
+-rw-r--r--   0        0        0    24481 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/NOTICE
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/README.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/hatch.toml
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 deadline_cloud_for_houdini-0.6.2/PKG-INFO
```

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/houdini_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from types import FrameType
 from typing import Optional
 
 # The Houdini Adaptor adds the `openjd` namespace directory to PYTHONPATH,
 # so that importing just the adaptor_runtime_client should work.
 try:
     from adaptor_runtime_client import (  # type: ignore[import]
-        HTTPClientInterface,
+        ClientInterface,
     )
     from houdini_adaptor.HoudiniClient.houdini_handler import HoudiniHandler  # type: ignore[import]
 except ImportError:
     from openjd.adaptor_runtime_client import (
-        HTTPClientInterface,
+        ClientInterface,
     )
     from deadline.houdini_adaptor.HoudiniClient.houdini_handler import HoudiniHandler
 
 try:
     import hou  # type: ignore
 except ImportError:  # pragma: no cover
     raise OSError("Could not find the Houdini module. Are you running this inside of Houdini?")
 
 
-class HoudiniClient(HTTPClientInterface):
+class HoudiniClient(ClientInterface):
     """
     Client that runs in Houdini for the Houdini Adaptor
     """
 
     def __init__(self, server_path: str) -> None:
         super().__init__(server_path=server_path)
         print(f"HoudiniClient: Houdini Version {hou.applicationVersionString()}")
```

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_adaptor/HoudiniClient/houdini_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,47 +35,66 @@
         self.render_kwargs = {"ignore_input_nodes": True}
         self.node = None
         self.wedge = None
         self.wegenum = None
 
     def set_node_settings(self, node):
         # this is a place holder function
-        # TODO remove after commom node library implemented
+        # TODO remove after common node library implemented
 
         node_type = node.type().nameWithCategory().split("/")
-        if node_type[0] == "Driver":
-            if node_type[1] == "ifd":
-                # mantra render node
-                alfredProgress = node.parm("vm_alfprogress")
-                if alfredProgress is not None:
-                    alfredProgress.set(1)
-                    print("Enabled Alfred style progress")
-
-                verbosity = node.parm("vm_verbose")
-                if verbosity is not None:
-                    verbosity.set(3)
-                    print("Set verbosity to 3")
-
-            elif node_type[1] == "karma":
-                alfredProgress = node.parm("alfprogress")
-                if alfredProgress is not None:
-                    alfredProgress.set(1)
-                    print("Enabled Alfred style progress")
-                verbosity = node.parm("verbosity")
-                if verbosity is not None:
-                    verbosity.set("3")
-                    hou.logging.setRenderLogVerbosity(3)
-                    print("Set verbosity to 3")
 
-        else:
-            pass
+        if node_type[0] != "Driver":
+            return
+
+        if len(node_type) < 2:
+            return
+
+        if node_type[1] == "ifd":
+            # Mantra render node
+            alfredProgress = node.parm("vm_alfprogress")
+            if alfredProgress is not None:
+                alfredProgress.set(1)
+                print("Enabled Alfred style progress")
+            verbosity = node.parm("vm_verbose")
+            if verbosity is not None:
+                # Mantra verbosity is an int with range 0 to 5
+                if isinstance(verbosity.eval(), int) and verbosity.eval() < 2:
+                    # 2 provides basic logging, we set it as a minimum to help with debugging issues
+                    verbosity.set(2)
+                    if verbosity.eval() == 2:
+                        # The verbosity won't be changed if the parameter is "keyed", so we check the value before
+                        # logging that it was increased
+                        # https://www.sidefx.com/docs/houdini/network/parms.html#color
+                        print("Increased verbosity to 2 to include basic logging")
+                print(f"Logging verbosity is set to {verbosity.eval()}")
+            return
+
+        if node_type[1] == "usdrender":
+            # Karma render node
+            alfredProgress = node.parm("alfprogress")
+            if alfredProgress is not None:
+                alfredProgress.set(1)
+                print("Enabled Alfred style progress")
+            verbosity = node.parm("verbosity")
+            if verbosity is not None:
+                # Karma verbosity is a str with options "", "3", "9", "9p", "9P"
+                # 3 means "Rendering Statistics", we set it as a minimum to help with debugging issues
+                if isinstance(verbosity.eval(), str) and verbosity.eval() == "":
+                    verbosity.set("3")
+                    if verbosity.eval() == "3":
+                        # The verbosity won't be changed if the parameter is "keyed", so we check the value before
+                        # logging that it was increased
+                        # https://www.sidefx.com/docs/houdini/network/parms.html#color
+                        print("Increased verbosity to '3' to include basic logging")
+                print(f"Logging verbosity is set to '{verbosity.eval()}'")
 
     def start_render(self, data: dict) -> None:
         """
-        Uses active node and calls hou's render, currently hardcoded to rendering a single fram
+        Uses active node and calls hou's render, currently hardcoded to rendering a single frame
 
         Args:
             data (dict):
 
         Raises:
             RuntimeError: .
         """
```

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/DialogScript`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/ExtraFileOptions`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/IconSVG`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/OnCreated`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/otls/deadline_cloud.hda/Driver_1deadline__cloud/Tools.shelf`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/adaptor_override_environment.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/queue_parameters.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py` & `deadline_cloud_for_houdini-0.6.2/src/deadline/houdini_submitter/python/deadline_cloud_for_houdini/submitter.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,95 +16,30 @@
 from deadline.client.config.config_file import str2bool
 from deadline.client.ui.dialogs.submit_job_progress_dialog import SubmitJobProgressDialog
 from deadline.client.ui.dialogs import DeadlineConfigDialog, DeadlineLoginDialog
 from deadline.job_attachments.upload import S3AssetManager
 from deadline.job_attachments.models import JobAttachmentS3Settings
 
 from .queue_parameters import update_queue_parameters, get_queue_parameter_values_as_openjd
-from ._version import version
-
-import hou
+from ._assets import _get_hip_file, _get_asset_references, _parse_files
 
-IGNORE_REF_VALUES = ("opdef:", "oplib:", "temp:", "op:")
-IGNORE_REF_PARMS = (
-    "taskgraphfile",
-    "pdg_workingdir",
-    "soho_program",
-    "BakeView_img_file_path",
-    "OutputDeepWriter_file",
-    "SettingsOutput_img_file_path",
-    "RS_outputFileNamePrefix",
-    "savetodirectory_directory",
+# For temporary backwards compatibility
+from ._assets import (
+    _IGNORE_REF_PARMS as IGNORE_REF_PARMS,  # noqa
+    _IGNORE_REF_VALUES as IGNORE_REF_VALUES,  # noqa
 )
+from ._version import version
 
-
-def _get_hip_file() -> str:
-    return hou.hipFile.path()
+import hou
 
 
 def _get_houdini_version() -> str:
     return hou.applicationVersionString()
 
 
-def _get_scene_asset_references(rop_node: hou.Node) -> AssetReferences:
-    # collect input filenames
-    asset_references = AssetReferences()
-    asset_references.input_filenames.add(_get_hip_file())
-
-    for parm, ref in hou.fileReferences():
-        if (
-            (not parm)
-            or (parm.node() == rop_node)
-            or (ref.startswith(IGNORE_REF_VALUES))
-            or (parm.name() in IGNORE_REF_PARMS)
-        ):
-            continue
-
-        path = parm.evalAsString()
-        if os.path.isdir(path):
-            asset_references.input_directories.add(path)
-        if os.path.isfile(path):
-            asset_references.input_filenames.add(path)
-
-    rop_dir_map = {
-        # Mantra/karma
-        "Driver/ifd": "vm_picture",
-        "Driver/karma": "picture",
-        # Husk
-        "Lop/usdrender_rop": _husk_outputs,
-        # Arnold
-        "Driver/arnold": "ar_picture",
-        # Vray
-        "Driver/vray_renderer": "SettingsOutput_img_file_path",
-        "Sop/rop_vrayproxy": "filepath",
-        "Driver/rop_vrayproxy": "filepath",
-        # Renderman
-        "Driver/ris::3.0": _renderman_outputs,
-        # Redshift
-        "Driver/Redshift_ROP": "RS_outputFileNamePrefix",
-        # Geo
-        "Driver/geometry": "sopoutput",
-        "Driver/alembic": "filename",
-        "Sop/filecache": "file",
-    }
-    # collect output dirs for each ROP
-    all_inputs = rop_node.inputAncestors()
-    for node in all_inputs:
-        type_name = node.type().nameWithCategory()
-        out_parm = rop_dir_map.get(type_name, None)
-        if out_parm is not None:
-            if callable(out_parm):
-                computed_dirs = out_parm(node)
-                asset_references.output_directories.update(computed_dirs)
-            else:
-                path = node.parm(out_parm).eval()
-                asset_references.output_directories.add(os.path.dirname(path))
-    return asset_references
-
-
 def _get_wedge_render_node(node: hou.Node):
     """Return ROP set as input or parameter to a wedge node
 
     This ROP may have a network of input ROP nodes that will also be modified
     by the wedge node
     """
     rendernode = None
@@ -284,47 +219,14 @@
         if not node:
             continue
         if node.isLockedHDA():
             return True
     return False
 
 
-def _renderman_outputs(node: hou.Node) -> set[str]:
-    """Obtain list of outputs from renderman displays with a file device"""
-    output_directories: set[str] = set()
-    displays = node.parm("ri_displays").eval()
-    for index in range(displays):
-        device = node.parm(f"ri_device_{index}").eval()
-        # skip display devices, only collect file devices
-        if device in ("it", "houdini"):
-            continue
-        path = node.parm(f"ri_display_{index}").eval()
-        output_directories.add(os.path.dirname(path))
-    return output_directories
-
-
-def _husk_outputs(node: hou.Node) -> set[str]:
-    """Obtain list of outputs by searching the standard /Render/Products scope
-    of the USD stage input
-    """
-    output_directories: set[str] = set()
-    for n in node.inputs():
-        try:
-            products = n.stage().GetPrimAtPath("/Render/Products")
-        except Exception:
-            # no products found in standard namespace
-            return output_directories
-        for child in products.GetChildren():
-            if child.GetTypeName() == "RenderProduct":
-                product_name_attr = child.GetAttribute("productName")
-                path = product_name_attr.Get(0)
-                output_directories.add(os.path.dirname(path))
-    return output_directories
-
-
 def _unlock_node(rop_path: str) -> bool:
     """Unlock the first locked node in the path lineage"""
     path_parts = rop_path.split("/")
     for i, _ in enumerate(path_parts):
         node_path = "/".join(path_parts[0:i])
         node = hou.node(node_path)
         if not node:
@@ -456,51 +358,28 @@
                 )
                 if "jobEnvironments" not in job_template:
                     job_template["jobEnvironments"] = []
                 job_template["jobEnvironments"].append(override_environment["environment"])
     return job_template
 
 
-def _get_asset_references(rop_node: hou.Node) -> AssetReferences:
-    asset_references = AssetReferences()
-    for n in rop_node.parm("input_filenames").multiParmInstances():
-        asset_references.input_filenames.add(n.eval())
-    for n in rop_node.parm("input_directories").multiParmInstances():
-        asset_references.input_directories.add(n.eval())
-    for n in rop_node.parm("output_directories").multiParmInstances():
-        asset_references.output_directories.add(n.eval())
-    return asset_references
-
-
 def _create_job_bundle(
     rop_node: hou.Node, job_bundle_dir: str, asset_references: AssetReferences
 ) -> None:
     job_bundle_path = Path(job_bundle_dir)
     job_template = _get_job_template(rop_node)
     parameter_values = _get_parameter_values(rop_node)
     with open(job_bundle_path / "template.yaml", "w", encoding="utf8") as f:
         deadline_yaml_dump(job_template, f, indent=1)
     with open(job_bundle_path / "parameter_values.yaml", "w", encoding="utf8") as f:
         deadline_yaml_dump(parameter_values, f, indent=1)
     with open(job_bundle_path / "asset_references.yaml", "w", encoding="utf8") as f:
         deadline_yaml_dump(asset_references.to_dict(), f, indent=1)
 
 
-def _parse_files(node):
-    asset_references = _get_scene_asset_references(node)
-    for ref in ("input_filenames", "input_directories", "output_directories"):
-        p = node.parm(ref)
-        while p.multiParmInstancesCount():
-            p.removeMultiParmInstance(0)
-        paths = sorted(list(getattr(asset_references, ref)))
-        p.set(len(paths))
-        for i, n in enumerate(p.multiParmInstances()):
-            n.set(paths[i])
-
-
 def callback(kwargs):
     """ROP parameter callback wrapper"""
     function_name = f"{kwargs['parm'].name()}_callback"
     globals()[function_name](kwargs)
 
 
 def parse_files_callback(kwargs):
@@ -528,21 +407,31 @@
         hou.ui.displayMessage(
             str(exc), title="Houdini Job Submission", severity=hou.severityType.Warning
         )
 
 
 def submit_callback(kwargs):
     node = kwargs["node"]
+    all_inputs = node.inputAncestors()
+
+    if not all_inputs:
+        # there are no inputs to the AWS Deadline Cloud render node
+        hou.ui.displayMessage(
+            "The AWS Deadline Cloud render node (ROP) must have an input ROP specified to submit a job",
+            title="Missing Input Render Node",
+            severity=hou.severityType.Warning,
+        )
+        return
+
     name = node.parm("name").evalAsString()
     # TODO: Populate from queue environment so that parameters can be overridden.
     queue_parameters: list[JobParameter] = []
     asset_references = _get_asset_references(node)
 
     # check for locked rops, Karma for example
-    all_inputs = node.inputAncestors()
     locked_rops = []
     for n in all_inputs:
         node_path = n.path()
         if _is_node_locked(node_path):
             locked_rops.append(node_path)
 
     if locked_rops:
```

### Comparing `deadline_cloud_for_houdini-0.6.1/LICENSE` & `deadline_cloud_for_houdini-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/README.md` & `deadline_cloud_for_houdini-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/hatch.toml` & `deadline_cloud_for_houdini-0.6.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/pyproject.toml` & `deadline_cloud_for_houdini-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_houdini-0.6.1/PKG-INFO` & `deadline_cloud_for_houdini-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-houdini
-Version: 0.6.1
+Version: 0.6.2
 Summary: AWS Deadline Cloud for Houdini
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-houdini
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-houdini
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
```


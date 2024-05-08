# Comparing `tmp/cubecoders_amp_api_wrapper-0.0.41b0.tar.gz` & `tmp/cubecoders_amp_api_wrapper-0.0.42b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubecoders_amp_api_wrapper-0.0.41b0.tar", last modified: Sun Apr 28 19:16:11 2024, max compression
+gzip compressed data, was "cubecoders_amp_api_wrapper-0.0.42b0.tar", last modified: Wed May  8 21:50:59 2024, max compression
```

## Comparing `cubecoders_amp_api_wrapper-0.0.41b0.tar` & `cubecoders_amp_api_wrapper-0.0.42b0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-28 19:16:10.190452 cubecoders_amp_api_wrapper-0.0.41b0/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     7842 2024-04-28 19:16:08.000000 cubecoders_amp_api_wrapper-0.0.41b0/CHANGELOG.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35149 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/LICENSE
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       76 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/MANIFEST.in
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4772 2024-04-28 19:16:10.185501 cubecoders_amp_api_wrapper-0.0.41b0/PKG-INFO
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3475 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/README.md
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-28 19:16:09.758454 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1575 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/__init__.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2408 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/ads.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    76652 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/adsmodule.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    14988 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/base.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1614 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/bridge.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    75470 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/core.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      258 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/emailsender.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     8024 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/filebackup.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    22707 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/filemanager.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2836 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/instance.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    19719 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/minecraft.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    34975 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/types.py
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3570 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/ampapi/util.py
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-28 19:16:10.151452 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4772 2024-04-28 19:16:08.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      696 2024-04-28 19:16:09.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        1 2024-04-28 19:16:08.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-04-28 19:16:08.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/requires.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        7 2024-04-28 19:16:09.000000 cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-04-28 19:16:10.123452 cubecoders_amp_api_wrapper-0.0.41b0/docs/
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    44032 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/ADS_api_spec.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    29384 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/Minecraft_api_spec.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/permission_nodes.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/permission_nodes.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4691 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/setting_nodes.md
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4649 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/docs/setting_nodes.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-04-12 19:04:59.000000 cubecoders_amp_api_wrapper-0.0.41b0/requirements.txt
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       38 2024-04-28 19:16:10.216585 cubecoders_amp_api_wrapper-0.0.41b0/setup.cfg
--rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2134 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.41b0/setup.py
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-08 21:50:59.077004 cubecoders_amp_api_wrapper-0.0.42b0/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     8872 2024-05-08 21:50:56.000000 cubecoders_amp_api_wrapper-0.0.42b0/CHANGELOG.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    35149 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.42b0/LICENSE
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       76 2024-04-28 19:14:36.000000 cubecoders_amp_api_wrapper-0.0.42b0/MANIFEST.in
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4778 2024-05-08 21:50:59.072454 cubecoders_amp_api_wrapper-0.0.42b0/PKG-INFO
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3481 2024-05-08 15:52:03.000000 cubecoders_amp_api_wrapper-0.0.42b0/README.md
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-08 21:50:58.626006 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1575 2024-05-08 21:48:22.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/__init__.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2501 2024-05-08 21:39:59.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/ads.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    76652 2024-05-08 21:43:40.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/adsmodule.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    15110 2024-05-08 21:36:15.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/base.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     1719 2024-05-08 21:38:55.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/bridge.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    75470 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/core.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      258 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/emailsender.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     8024 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/filebackup.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    22707 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/filemanager.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2836 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/instance.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    19680 2024-05-08 16:26:18.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/minecraft.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    34985 2024-05-08 16:35:09.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/types.py
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     3570 2024-05-08 16:26:31.000000 cubecoders_amp_api_wrapper-0.0.42b0/ampapi/util.py
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-08 21:50:59.038004 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4778 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)      696 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        1 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/dependency_links.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/requires.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        7 2024-05-08 21:50:57.000000 cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)        0 2024-05-08 21:50:59.010004 cubecoders_amp_api_wrapper-0.0.42b0/docs/
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    44032 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/ADS_api_spec.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    29384 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/Minecraft_api_spec.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/permission_nodes.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)    10444 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/permission_nodes.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4691 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/setting_nodes.md
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     4649 2024-04-28 19:14:37.000000 cubecoders_amp_api_wrapper-0.0.42b0/docs/setting_nodes.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       59 2024-05-08 21:36:33.000000 cubecoders_amp_api_wrapper-0.0.42b0/requirements.txt
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)       38 2024-05-08 21:50:59.117169 cubecoders_amp_api_wrapper-0.0.42b0/setup.cfg
+-rwxr-xr-x   0 k8thekat  (1000) k8thekat  (1000)     2134 2024-05-08 21:49:44.000000 cubecoders_amp_api_wrapper-0.0.42b0/setup.py
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/CHANGELOG.md` & `cubecoders_amp_api_wrapper-0.0.42b0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+## Version - 0.0.42b - [2bf7996](https://github.com/k8thekat/AMPAPI_Python/commit/2bf7996)
+#### Changelog.md
+- Version info from `0.0.41b`
+
+#### __init__.py
+- Version bump `0.0.42b`
+
+#### README.md
+- Added missing `await` in Quick Example - Sample_API().
+
+#### ads.py
+- Changed some prints to `_logger.debug()`.
+- Type-hinted `ads_list` inside `get_instances()` method.
+- Added logic check to `get_instances()` when not formatting data to prevent error.
+
+#### base.py
+- Removed `type:ignore` from `__init__()`.
+- Added return value to `format_data` setter.
+- Added `_logger.debug()` for monitoring data formatting.
+- Fixed logic when formatting data causing return failure using the `ADSInstance` class.
+- Improved readability of format logic of `_call_api()`.
+
+#### bridge.py
+- Added logging.
+- Changed `apiparams` to `api_params`.
+- Added type-hinting to `__new__()`.
+- Added `_logger.debug()` to `__init__()`.
+
+#### minecraft.py
+- Removed unused imports.
+
+#### types.py
+- added `repr = False` to the `Controller()` dataclass.
+
 ## Version - 0.0.41b - [5b0aed8](https://github.com/k8thekat/AMPAPI_Python/commit/5b0aed8)
 #### __init__.py
 - Version bump `0.0.41b
 
 #### types.py
 - Added `LastExecuteError` and `LastErrorReason` to `Triggers()` dataclass.
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/LICENSE` & `cubecoders_amp_api_wrapper-0.0.42b0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/PKG-INFO` & `cubecoders_amp_api_wrapper-0.0.42b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubecoders_amp_api_wrapper
-Version: 0.0.41b0
+Version: 0.0.42b0
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
@@ -72,15 +72,15 @@
 async def Sample_API():
     """
     Example API Function to call method Endpoints.
     """
     _bridge = Bridge(api_params=_params)
     ADS: ADSInstance = ADSInstance()
     # This would populate the ADS class property .AvailableInstances
-    ADS.get_instances()
+    await ADS.get_instances()
     # We can break out all our instances into their own attributes.
     arkinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[1]
     mcinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[2]
 
     # Pre populated from the dataclass and has the API methods too!
     # You can take a backup really easily.
     await arkinstance.take_backup(title="ARK1_backup", description="This is an ARK backup", sticky=True)
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/README.md` & `cubecoders_amp_api_wrapper-0.0.42b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 async def Sample_API():
     """
     Example API Function to call method Endpoints.
     """
     _bridge = Bridge(api_params=_params)
     ADS: ADSInstance = ADSInstance()
     # This would populate the ADS class property .AvailableInstances
-    ADS.get_instances()
+    await ADS.get_instances()
     # We can break out all our instances into their own attributes.
     arkinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[1]
     mcinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[2]
 
     # Pre populated from the dataclass and has the API methods too!
     # You can take a backup really easily.
     await arkinstance.take_backup(title="ARK1_backup", description="This is an ARK backup", sticky=True)
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/__init__.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    02110-1301, USA. 
 '''
 from __future__ import annotations
 
 __title__ = "CubeCoders AMP API"
 __author__ = "k8thekat"
 __license__ = "GNU"
-__version__ = "0.0.41b"
+__version__ = "0.0.42b"
 __credits__ = "AMP by CubeCoders and associates."
 
 from typing import Literal, NamedTuple
 
 from .ads import *
 from .adsmodule import *
 from .bridge import *
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/ads.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/ads.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
                 elif instances[i].Module == "Minecraft":
                     self._AvailableInstances.append(AMPMinecraftInstance(data=instances[i]))
 
                 else:
                     self._AvailableInstances.append(AMPInstance(data=instances[i]))
 
-    def __init__(self):
-        # print(f"DEBUG {type(self).__name__} __init__")
+    def __init__(self) -> None:
+        self._logger.debug(msg=f"DEBUG {type(self).__name__} __init__")
         super().__init__()
 
     async def get_instances(self, format_data: Union[bool, None] = None) -> list[Controller | Self]:
         """
         Returns a list of all Instances on the AMP Panel and updates our self object.
         `**ADSInstance Only**`
 
@@ -50,16 +50,16 @@
             format_data (Union[bool, None], optional): Format the JSON response data. Defaults to None. (Uses `FORMAT_DATA` global constant if None)
 
         Returns:
             list[Self] | str | bool | int | None: On success returns a list of Self dataclasses. 
 
         """
 
-        ads_list = []
+        ads_list: list[ADSInstance | Controller] = []
         result: list[Controller] = await super().get_instances(format_data=format_data)
-        if isinstance(result, list):
+        if isinstance(result, list) and isinstance(result[0], Controller):
             self.parse_data(data=result[0])  # Need to update our self object.
             for i in range(1, len(result)):
                 ads_list.append(ADSInstance().parse_data(data=result[i]))
             return ads_list
         else:
             return result
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/adsmodule.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/adsmodule.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/base.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         bridge: Bridge = Bridge.get_bridge()
         # Validate the bridge object is at the same memory address.
         self._logger.debug(f"bridge object -> {bridge}")
         if bridge == None:
             raise ValueError(self.NO_BRIDGE)
 
         if isinstance(bridge, Bridge):
-            self.parse_bridge(bridge=bridge)  # type:ignore
+            self.parse_bridge(bridge=bridge)
 
     @property
     def format_data(self) -> bool:
         """
         Controls whether the data returned from the API endpoint is formatted or not. \n
         `True` = formatted \n
         `False` = unformatted
@@ -64,15 +64,15 @@
         Returns:
             bool: `True` or `False`, defaults to `True`.
         """
         global FORMAT_DATA
         return FORMAT_DATA
 
     @format_data.setter
-    def format_data(self, value: bool):
+    def format_data(self, value: bool) -> None:
         global FORMAT_DATA
         FORMAT_DATA = value
 
     # def set_format_data(self, value: bool = True) -> bool:
     #     """
     #     Controls whether the data returned from the API endpoint is formatted or not. \n
     #     `True` = formatted \n
@@ -274,19 +274,19 @@
                 self._logger.error(f"{api} failed because of {post_req_json}")
                 raise ConnectionError(self.FAILED_API)
 
             elif isinstance(post_req_json, dict) and "Status" in post_req_json and post_req_json["Status"] == False:
                 self._logger.error(f"{api} failed because of Status: {post_req_json}")
                 return ConnectionError(self.FAILED_API)
 
-        # print("DEBUG", "FORMAT->", format_data, format)
-        if format is None or format_data is False:
+        self._logger.debug(msg=f"DEBUG _call_api | format_data = {format_data} | FORMAT_DATA = {FORMAT_DATA} | FORMAT-> {format}")
+        if (format is None or format_data is False) or (format_data is None and FORMAT_DATA is False):
             return post_req_json
 
-        elif format_data is True or format_data is None and FORMAT_DATA is True:
+        elif (format_data is True) or (format_data is None and FORMAT_DATA is True):
             return self.json_to_dataclass(json=post_req_json, format=format, _use_from_dict=_use_from_dict, _auto_unpack=_auto_unpack)
 
     async def _connect(self) -> LoginResults | None:
         """
         Handles your 2FA code and logging into AMP while also handling the session ID. \n
 
         Raises:
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/bridge.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/bridge.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+import logging
 from dataclasses import fields
 from typing import TYPE_CHECKING, Self
 
 from .types import APIParams
 
 __all__ = ("Bridge",)
 
 
 class Bridge(APIParams):
     """
     Handles the API login credentials for connecting to AMP.
 
     Simply create the class similar to the example and then access any other API class you wish.\n
-        *eg* `_bridge: Bridge | None = Bridge(apiparams= <class APIparams>)`
+        *eg* `_bridge: Bridge | None = Bridge(ap_params= <class APIparams>)`
                 `APICore = Core() #this will pull login details from the Bridge class`
 
     """
-    apiparams: APIParams
+    api_params: APIParams
+    _logger: logging.Logger = logging.getLogger()
 
     @classmethod
     def get_bridge(cls) -> Self:
         """
         Retrieves an existing Bridge class object.\n
         **`DO NOT CALL THIS METHOD OUTSIDE OF AN API CLASS (ADSModule, Core, etc..)`**
 
@@ -31,16 +33,16 @@
         """
         if cls._instance == None:
             raise ValueError("Failed to setup connection. You need to initiate `<class Bridge>` first.")
         return cls._instance
 
     def __new__(cls, api_params: APIParams | None = None, *args, **kwargs) -> Self | None:
         if not hasattr(cls, "_instance"):
-            cls._instance = super(Bridge, cls).__new__(cls, *args, **kwargs)
+            cls._instance: Self = super(Bridge, cls).__new__(cls, *args, **kwargs)
         return cls._instance
 
     def __init__(self, api_params: APIParams, *args, **kwargs) -> None:
-        # print("DEBUG Bridge __init__")
+        self._logger.debug(msg="DEBUG Bridge __init__")
         self.api_params: APIParams = api_params
         # We parse the api params for easier usage.
-        for field in fields(api_params):
+        for field in fields(class_or_instance=api_params):
             setattr(self, field.name, getattr(self.api_params, field.name))
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/core.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/core.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/filebackup.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/filebackup.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/filemanager.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/filemanager.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/instance.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/instance.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/minecraft.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/minecraft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
 
 from typing import Any, Union
 
-from dataclass_wizard import fromdict
-
 from .base import FORMAT_DATA, Base
 from .types import *
 
 __all__ = ("MinecraftModule",)
 
 
 class MinecraftModule(Base):
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/types.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
     SpecificDockerImage: str = ""
     ModuleDisplayName: str = ""  # 'Terraria'
     Metrics: Metric | None = field(default=None)
     DisplayImageSource: str = ""  # steam:105600
     Description: str = ""
 
 
-@dataclass()
+@dataclass(repr=False)
 class Controller():
     """
     Represents an AMP Controller (aka Target manager) that manages the Instances it has access to.
 
     """
 
     AvailableInstances: list[Instance]
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/ampapi/util.py` & `cubecoders_amp_api_wrapper-0.0.42b0/ampapi/util.py`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO` & `cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubecoders_amp_api_wrapper
-Version: 0.0.41b0
+Version: 0.0.42b0
 Summary: A python wrapper for the AMP API by CubeCoders
 Home-page: https://github.com/k8thekat/AMPAPI_Python
 Author: Katelynn Cadwallader
 Author-email: Cadwalladerkatelynn+AMPAPI@gmail.com
 License: GNU
 Project-URL: GitHub, https://github.com/k8thekat/AMPAPI_Python
 Project-URL: Changelog, https://github.com/k8thekat/AMPAPI_Python/blob/master/CHANGELOG.md
@@ -72,15 +72,15 @@
 async def Sample_API():
     """
     Example API Function to call method Endpoints.
     """
     _bridge = Bridge(api_params=_params)
     ADS: ADSInstance = ADSInstance()
     # This would populate the ADS class property .AvailableInstances
-    ADS.get_instances()
+    await ADS.get_instances()
     # We can break out all our instances into their own attributes.
     arkinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[1]
     mcinstance: AMPInstance | AMPMinecraftInstance = ADS.AvailableInstances[2]
 
     # Pre populated from the dataclass and has the API methods too!
     # You can take a backup really easily.
     await arkinstance.take_backup(title="ARK1_backup", description="This is an ARK backup", sticky=True)
```

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt` & `cubecoders_amp_api_wrapper-0.0.42b0/cubecoders_amp_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/docs/ADS_api_spec.md` & `cubecoders_amp_api_wrapper-0.0.42b0/docs/ADS_api_spec.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/docs/Minecraft_api_spec.md` & `cubecoders_amp_api_wrapper-0.0.42b0/docs/Minecraft_api_spec.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/docs/permission_nodes.md` & `cubecoders_amp_api_wrapper-0.0.42b0/docs/permission_nodes.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/docs/permission_nodes.txt` & `cubecoders_amp_api_wrapper-0.0.42b0/docs/permission_nodes.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/docs/setting_nodes.md` & `cubecoders_amp_api_wrapper-0.0.42b0/docs/setting_nodes.md`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/docs/setting_nodes.txt` & `cubecoders_amp_api_wrapper-0.0.42b0/docs/setting_nodes.txt`

 * *Files identical despite different names*

### Comparing `cubecoders_amp_api_wrapper-0.0.41b0/setup.py` & `cubecoders_amp_api_wrapper-0.0.42b0/setup.py`

 * *Files identical despite different names*


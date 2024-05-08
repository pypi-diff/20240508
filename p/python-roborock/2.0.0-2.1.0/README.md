# Comparing `tmp/python_roborock-2.0.0.tar.gz` & `tmp/python_roborock-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-2.0.0.tar", max compression
+gzip compressed data, was "python_roborock-2.1.0.tar", max compression
```

## Comparing `python_roborock-2.0.0.tar` & `python_roborock-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2024-04-11 14:48:23.714890 python_roborock-2.0.0/LICENSE
--rw-r--r--   0        0        0     1220 2024-04-11 14:48:23.714890 python_roborock-2.0.0/README.md
--rw-r--r--   0        0        0     1677 2024-04-11 14:48:24.430890 python_roborock-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      165 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/__init__.py
--rw-r--r--   0        0        0     4107 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/api.py
--rw-r--r--   0        0        0     6826 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/cli.py
--rw-r--r--   0        0        0     7144 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/cloud_api.py
--rw-r--r--   0        0        0    13571 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/code_mappings.py
--rw-r--r--   0        0        0     7912 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/command_cache.py
--rw-r--r--   0        0        0     2339 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/const.py
--rw-r--r--   0        0        0    27590 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/containers.py
--rw-r--r--   0        0        0     1962 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/exceptions.py
--rw-r--r--   0        0        0     4367 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/local_api.py
--rw-r--r--   0        0        0    12315 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/protocol.py
--rw-r--r--   0        0        0        0 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/py.typed
--rw-r--r--   0        0        0      834 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/roborock_future.py
--rw-r--r--   0        0        0     5464 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/roborock_message.py
--rw-r--r--   0        0        0    21816 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/roborock_typing.py
--rw-r--r--   0        0        0     3465 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/util.py
--rw-r--r--   0        0        0      183 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_1_apis/__init__.py
--rw-r--r--   0        0        0    19949 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_1_apis/roborock_client_v1.py
--rw-r--r--   0        0        0     3477 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_1_apis/roborock_local_client_v1.py
--rw-r--r--   0        0        0     3342 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_1_apis/roborock_mqtt_client_v1.py
--rw-r--r--   0        0        0      111 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_a01_apis/__init__.py
--rw-r--r--   0        0        0     7342 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_a01_apis/roborock_client_a01.py
--rw-r--r--   0        0        0     2961 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py
--rw-r--r--   0        0        0    13040 2024-04-11 14:48:23.718890 python_roborock-2.0.0/roborock/web_api.py
--rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 python_roborock-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-08 13:12:47.864147 python_roborock-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-08 13:12:47.864147 python_roborock-2.1.0/README.md
+-rw-r--r--   0        0        0     1677 2024-05-08 13:12:48.528159 python_roborock-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      165 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/__init__.py
+-rw-r--r--   0        0        0     4107 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/api.py
+-rw-r--r--   0        0        0     6826 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/cli.py
+-rw-r--r--   0        0        0     7144 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/cloud_api.py
+-rw-r--r--   0        0        0    14400 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/code_mappings.py
+-rw-r--r--   0        0        0     7912 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/command_cache.py
+-rw-r--r--   0        0        0     2386 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/const.py
+-rw-r--r--   0        0        0    27991 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/containers.py
+-rw-r--r--   0        0        0     1962 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/exceptions.py
+-rw-r--r--   0        0        0     4367 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/local_api.py
+-rw-r--r--   0        0        0    12315 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/protocol.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/py.typed
+-rw-r--r--   0        0        0      834 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/roborock_future.py
+-rw-r--r--   0        0        0     5464 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/roborock_message.py
+-rw-r--r--   0        0        0    23536 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/roborock_typing.py
+-rw-r--r--   0        0        0     3465 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/util.py
+-rw-r--r--   0        0        0      183 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/version_1_apis/__init__.py
+-rw-r--r--   0        0        0    19949 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/version_1_apis/roborock_client_v1.py
+-rw-r--r--   0        0        0     3477 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/version_1_apis/roborock_local_client_v1.py
+-rw-r--r--   0        0        0     3342 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/version_1_apis/roborock_mqtt_client_v1.py
+-rw-r--r--   0        0        0      111 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/version_a01_apis/__init__.py
+-rw-r--r--   0        0        0     7342 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/version_a01_apis/roborock_client_a01.py
+-rw-r--r--   0        0        0     2961 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py
+-rw-r--r--   0        0        0    13040 2024-05-08 13:12:47.868147 python_roborock-2.1.0/roborock/web_api.py
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 python_roborock-2.1.0/PKG-INFO
```

### Comparing `python_roborock-2.0.0/LICENSE` & `python_roborock-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/README.md` & `python_roborock-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/pyproject.toml` & `python_roborock-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "2.0.0"
+version = "2.1.0"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 documentation = "https://python-roborock.readthedocs.io/"
 classifiers = [
```

### Comparing `python_roborock-2.0.0/roborock/api.py` & `python_roborock-2.1.0/roborock/api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/cli.py` & `python_roborock-2.1.0/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/cloud_api.py` & `python_roborock-2.1.0/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/code_mappings.py` & `python_roborock-2.1.0/roborock/code_mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,20 @@
     updating = 14
     docking = 15
     going_to_target = 16
     zoned_cleaning = 17
     segment_cleaning = 18
     emptying_the_bin = 22  # on s7+
     washing_the_mop = 23  # on a46
+    washing_the_mop_2 = 25
     going_to_wash_the_mop = 26  # on a46
     in_call = 28
     mapping = 29
     egg_attack = 30
+    patrol = 32
     charging_complete = 100
     device_offline = 101
     locked = 103
     air_drying_stopping = 202
     robot_status_mopping = 6301
     clean_mop_cleaning = 6302
     clean_mop_mopping = 6303
@@ -122,14 +124,15 @@
     charging_error = 13
     battery_error = 14
     wall_sensor_dirty = 15
     robot_tilted = 16
     side_brush_error = 17
     fan_error = 18
     dock = 19  # Dock not connected to power
+    optical_flow_sensor_dirt = 20
     vertical_bumper_pressed = 21
     dock_locator_error = 22
     return_to_dock_fail = 23
     nogo_zone_detected = 24
     visual_sensor = 25  # Camera error
     light_touch = 26  # Wall sensor error
     vibrarise_jammed = 27
@@ -146,15 +149,22 @@
     dirty_water_box_hoare = 39  # Check the dirty water tank
     sink_strainer_hoare = 40  # Reinstall the water filter
     clear_water_box_exception = 41  # Clean water tank empty
     clear_brush_exception = 42  # Check that the water filter has been correctly installed
     clear_brush_exception_2 = 43  # Positioning button error
     filter_screen_exception = 44  # Clean the dock water filter
     mopping_roller_2 = 45  # Wash roller may be jammed
+    up_water_exception = 48
+    drain_water_exception = 49
     temperature_protection = 51  # Unit temperature protection
+    clean_carousel_exception = 52
+    clean_carousel_water_full = 53
+    water_carriage_drop = 54
+    check_clean_carouse = 55
+    audio_error = 56
 
 
 class RoborockFanPowerCode(RoborockEnum):
     """Describes the fan power of the vacuum cleaner."""
 
     # Fan speeds should have the first letter capitalized - as there is no way to change the name in translations as
     # far as I am aware
@@ -232,14 +242,22 @@
     balanced = 102
     turbo = 103
     max = 104
     custom = 106
     max_plus = 108
 
 
+class RoborockFanSpeedS8MaxVUltra(RoborockFanPowerCode):
+    off = 105
+    balanced = 102
+    custom = 106
+    max_plus = 108
+    smart_mode = 110
+
+
 class RoborockMopModeCode(RoborockEnum):
     """Describes the mop mode of the vacuum cleaner."""
 
 
 class RoborockMopModeS7(RoborockMopModeCode):
     """Describes the mop mode of the vacuum cleaner."""
 
@@ -253,14 +271,23 @@
     standard = 300
     deep = 301
     deep_plus = 303
     fast = 304
     custom = 302
 
 
+class RoborockMopModeS8MaxVUltra(RoborockMopModeCode):
+    standard = 300
+    deep = 301
+    deep_plus = 303
+    fast = 304
+    deep_plus_pearl = 305
+    smart_mode = 306
+
+
 class RoborockMopIntensityCode(RoborockEnum):
     """Describes the mop intensity of the vacuum cleaner."""
 
 
 class RoborockMopIntensityS7(RoborockMopIntensityCode):
     """Describes the mop intensity of the vacuum cleaner."""
 
@@ -288,14 +315,22 @@
     low = 201
     medium = 202
     high = 203
     custom = 204
     custom_water_flow = 207
 
 
+class RoborockMopIntensityS8MaxVUltra(RoborockMopIntensityCode):
+    off = 200
+    low = 201
+    medium = 202
+    smart_mode = 209
+    custom_water_flow = 207
+
+
 class RoborockMopIntensityS5Max(RoborockMopIntensityCode):
     """Describes the mop intensity of the vacuum cleaner."""
 
     off = 200
     low = 201
     medium = 202
     high = 203
@@ -317,28 +352,30 @@
 class RoborockDockErrorCode(RoborockEnum):
     """Describes the error code of the dock."""
 
     ok = 0
     duct_blockage = 34
     water_empty = 38
     waste_water_tank_full = 39
+    maintenance_brush_jammed = 42
     dirty_tank_latch_open = 44
     no_dustbin = 46
     cleaning_tank_full_or_blocked = 53
 
 
 class RoborockDockTypeCode(RoborockEnum):
     unknown = -9999
     no_dock = 0
     auto_empty_dock = 1
     empty_wash_fill_dock = 3
     auto_empty_dock_pure = 5
     s7_max_ultra_dock = 6
     s8_dock = 7
     p10_dock = 8
+    s8_maxv_ultra_dock = 10
 
 
 class RoborockDockDustCollectionModeCode(RoborockEnum):
     """Describes the dust collection mode of the vacuum cleaner."""
 
     # TODO: Get the correct values for various different docks
     unknown = -9999
```

### Comparing `python_roborock-2.0.0/roborock/command_cache.py` & `python_roborock-2.1.0/roborock/command_cache.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/const.py` & `python_roborock-2.1.0/roborock/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 ROBOROCK_S6_MAXV = "roborock.vacuum.a10"
 ROBOROCK_E2 = "roborock.vacuum.e2"
 ROBOROCK_1S = "roborock.vacuum.m1s"
 ROBOROCK_C1 = "roborock.vacuum.c1"
 ROBOROCK_S8_PRO_ULTRA = "roborock.vacuum.a70"
 ROBOROCK_S8 = "roborock.vacuum.a51"
 ROBOROCK_P10 = "roborock.vacuum.a75"
+ROBOROCK_S8_MAXV_ULTRA = "roborock.vacuum.a97"
 
 ROBOROCK_DYAD_AIR = "roborock.wetdryvac.a107"
 ROBOROCK_DYAD_PRO_COMBO = "roborock.wetdryvac.a83"
 ROBOROCK_DYAD_PRO = "roborock.wetdryvac.a56"
 
 # These are the devices that show up when you add a device - more could be supported and just not show up
 SUPPORTED_VACUUMS = [
```

### Comparing `python_roborock-2.0.0/roborock/containers.py` & `python_roborock-2.1.0/roborock/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,25 @@
     RoborockErrorCode,
     RoborockFanPowerCode,
     RoborockFanSpeedP10,
     RoborockFanSpeedQ7Max,
     RoborockFanSpeedS6Pure,
     RoborockFanSpeedS7,
     RoborockFanSpeedS7MaxV,
+    RoborockFanSpeedS8MaxVUltra,
     RoborockMopIntensityCode,
     RoborockMopIntensityP10,
     RoborockMopIntensityS5Max,
     RoborockMopIntensityS6MaxV,
     RoborockMopIntensityS7,
+    RoborockMopIntensityS8MaxVUltra,
     RoborockMopIntensityV2,
     RoborockMopModeCode,
     RoborockMopModeS7,
+    RoborockMopModeS8MaxVUltra,
     RoborockMopModeS8ProUltra,
     RoborockStateCode,
 )
 from .const import (
     CLEANING_BRUSH_REPLACE_TIME,
     DUST_COLLECTION_REPLACE_TIME,
     FILTER_REPLACE_TIME,
@@ -48,14 +51,15 @@
     ROBOROCK_S5_MAX,
     ROBOROCK_S6,
     ROBOROCK_S6_MAXV,
     ROBOROCK_S6_PURE,
     ROBOROCK_S7,
     ROBOROCK_S7_MAXV,
     ROBOROCK_S8,
+    ROBOROCK_S8_MAXV_ULTRA,
     ROBOROCK_S8_PRO_ULTRA,
     SENSOR_DIRTY_REPLACE_TIME,
     SIDE_BRUSH_REPLACE_TIME,
     STRAINER_REPLACE_TIME,
 )
 from .exceptions import RoborockException
 
@@ -546,27 +550,35 @@
 @dataclass
 class P10Status(Status):
     fan_power: RoborockFanSpeedP10 | None = None
     water_box_mode: RoborockMopIntensityP10 | None = None
     mop_mode: RoborockMopModeS8ProUltra | None = None
 
 
+@dataclass
+class S8MaxvUltraStatus(Status):
+    fan_power: RoborockFanSpeedS8MaxVUltra | None = None
+    water_box_mode: RoborockMopIntensityS8MaxVUltra | None = None
+    mop_mode: RoborockMopModeS8MaxVUltra | None = None
+
+
 ModelStatus: dict[str, type[Status]] = {
     ROBOROCK_S4_MAX: S4MaxStatus,
     ROBOROCK_S5_MAX: S5MaxStatus,
     ROBOROCK_Q7_MAX: Q7MaxStatus,
     ROBOROCK_S6: S6PureStatus,
     ROBOROCK_S6_MAXV: S6MaxVStatus,
     ROBOROCK_S6_PURE: S6PureStatus,
     ROBOROCK_S7_MAXV: S7MaxVStatus,
     ROBOROCK_S7: S7Status,
     ROBOROCK_S8: S8Status,
     ROBOROCK_S8_PRO_ULTRA: S8ProUltraStatus,
     ROBOROCK_G10S_PRO: S7MaxVStatus,
     ROBOROCK_P10: P10Status,
+    ROBOROCK_S8_MAXV_ULTRA: S8MaxvUltraStatus,
 }
 
 
 @dataclass
 class DnDTimer(RoborockBaseTimer):
     """DnDTimer"""
```

### Comparing `python_roborock-2.0.0/roborock/exceptions.py` & `python_roborock-2.1.0/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/local_api.py` & `python_roborock-2.1.0/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/protocol.py` & `python_roborock-2.1.0/roborock/protocol.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/roborock_future.py` & `python_roborock-2.1.0/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/roborock_message.py` & `python_roborock-2.1.0/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/roborock_typing.py` & `python_roborock-2.1.0/roborock/roborock_typing.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,29 +31,34 @@
     APP_KEEP_EASTER_EGG = "app_keep_easter_egg"
     APP_PAUSE = "app_pause"
     APP_RC_END = "app_rc_end"
     APP_RC_MOVE = "app_rc_move"
     APP_RC_START = "app_rc_start"
     APP_RC_STOP = "app_rc_stop"
     APP_RESUME_BUILD_MAP = "app_resume_build_map"
+    APP_RESUME_PATROL = "app_resume_patrol"
     APP_SEGMENT_CLEAN = "app_segment_clean"
     APP_SET_AMETHYST_STATUS = "app_set_amethyst_status"
     APP_SET_CARPET_DEEP_CLEAN_STATUS = "app_set_carpet_deep_clean_status"
+    APP_SET_CROSS_CARPET_CLEANING_STATUS = "app_set_cross_carpet_cleaning_status"
     APP_SET_DOOR_SILL_BLOCKS = "app_set_door_sill_blocks"
+    APP_SET_DIRTY_REPLENISH_CLEAN_STATUS = "app_set_dirty_replenish_clean_status"
     APP_SET_DRYER_SETTING = "app_set_dryer_setting"
     APP_SET_DRYER_STATUS = "app_set_dryer_status"
     APP_SET_DYNAMIC_CONFIG = "app_set_dynamic_config"
     APP_SET_IGNORE_STUCK_POINT = "app_set_ignore_stuck_point"
     APP_SET_SMART_CLIFF_FORBIDDEN = "app_set_smart_cliff_forbidden"
     APP_SET_SMART_DOOR_SILL = "app_set_smart_door_sill"
     APP_SPOT = "app_spot"
     APP_START = "app_start"
     APP_START_BUILD_MAP = "app_start_build_map"
     APP_START_COLLECT_DUST = "app_start_collect_dust"
     APP_START_EASTER_EGG = "app_start_easter_egg"
+    APP_START_PATROL = "app_start_patrol"
+    APP_START_PET_PATROL = "app_start_pet_patrol"
     APP_START_WASH = "app_start_wash"
     APP_STAT = "app_stat"
     APP_STOP = "app_stop"
     APP_STOP_COLLECT_DUST = "app_stop_collect_dust"
     APP_STOP_WASH = "app_stop_wash"
     APP_UPDATE_UNSAVE_MAP = "app_update_unsave_map"
     APP_WAKEUP_ROBOT = "app_wakeup_robot"
@@ -173,14 +178,15 @@
     SET_CARPET_AREA = "set_carpet_area"
     SET_CARPET_CLEAN_MODE = "set_carpet_clean_mode"
     SET_CARPET_MODE = "set_carpet_mode"
     SET_CHILD_LOCK_STATUS = "set_child_lock_status"
     SET_CLEAN_FOLLOW_GROUND_MATERIAL_STATUS = "set_clean_follow_ground_material_status"
     SET_CLEAN_MOTOR_MODE = "set_clean_motor_mode"
     SET_CLEAN_SEQUENCE = "set_clean_sequence"
+    SET_CLEAN_REPEAT_TIMES = "set_clean_repeat_times"
     SET_COLLISION_AVOID_STATUS = "set_collision_avoid_status"
     SET_CUSTOM_MODE = "set_custom_mode"
     SET_CUSTOMIZE_CLEAN_MODE = "set_customize_clean_mode"
     SET_DND_TIMER = "set_dnd_timer"
     SET_DND_TIMER_ACTIONS = "set_dnd_timer_actions"
     SET_DUST_COLLECTION_MODE = "set_dust_collection_mode"
     SET_DUST_COLLECTION_SWITCH_STATUS = "set_dust_collection_switch_status"
@@ -235,14 +241,37 @@
     UPDATE_DOCK = "update_dock"
     UPDATE_MOP_TEMPLATE_PARAMS = "update_mop_template_params"
     UPLOAD_DATA_FOR_DEBUG_MODE = "upload_data_for_debug_mode"
     UPLOAD_PHOTO = "upload_photo"
     USE_NEW_MAP = "use_new_map"
     USE_OLD_MAP = "use_old_map"
     USER_UPLOAD_LOG = "user_upload_log"
+    SET_STRETCH_TAG_STATUS = "set_stretch_tag_status"
+    GET_STRETCH_TAG_STATUS = "get_stretch_tag_status"
+    SET_RIGHT_BRUSH_STRETCH_STATUS = "set_right_brush_stretch_status"
+    GET_RIGHT_BRUSH_STRETCH_STATUS = "get_right_brush_stretch_status"
+    SET_DIRTY_OBJECT_DETECT_STATUS = "set_dirty_object_detect_status"
+    GET_DIRTY_OBJECT_DETECT_STATUS = "get_dirty_object_detect_status"
+    SET_WASH_WATER_TEMPERATURE = "set_wash_water_temperature"
+    GET_WASH_WATER_TEMPERATURE = "get_wash_water_temperature"
+    APP_EMPTY_RINSE_TANK_WATER = "app_empty_rinse_tank_water"
+    SET_PET_SUPPLIES_DEEP_CLEAN_STATUS = "set_pet_supplies_deep_clean_status"
+    GET_PET_SUPPLIES_DEEP_CLEAN_STATUS = "get_pet_supplies_deep_clean_status"
+    SET_AP_MIC_LED_STATUS = "set_ap_mic_led_status"
+    GET_AP_MIC_LED_STATUS = "get_ap_mic_led_status"
+    SET_HANDLE_LEAK_WATER_STATUS = "set_handle_leak_water_status"
+    GET_HANDLE_LEAK_WATER_STATUS = "get_handle_leak_water_status"
+    APP_IGNORE_DIRTY_OBJECTS = "app_ignore_dirty_objects"
+    MATTER_GET_STATUS = "matter.get_status"
+    MATTER_DNLD_KEY = "matter.dnld_key"
+    MATTER_RESET = "matter.reset"
+    SET_GAP_DEEP_CLEAN_STATUS = "set_gap_deep_clean_status"
+    GET_GAP_DEEP_CLEAN_STATUS = "get_gap_deep_clean_status"
+    APP_SET_ROBOT_SETTING = "app_set_robot_setting"
+    APP_GET_ROBOT_SETTING = "app_get_robot_setting"
 
 
 @dataclass
 class CommandInfo:
     params: list | dict | int | None = None
```

### Comparing `python_roborock-2.0.0/roborock/util.py` & `python_roborock-2.1.0/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/version_1_apis/roborock_client_v1.py` & `python_roborock-2.1.0/roborock/version_1_apis/roborock_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/version_1_apis/roborock_local_client_v1.py` & `python_roborock-2.1.0/roborock/version_1_apis/roborock_local_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/version_1_apis/roborock_mqtt_client_v1.py` & `python_roborock-2.1.0/roborock/version_1_apis/roborock_mqtt_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/version_a01_apis/roborock_client_a01.py` & `python_roborock-2.1.0/roborock/version_a01_apis/roborock_client_a01.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py` & `python_roborock-2.1.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/roborock/web_api.py` & `python_roborock-2.1.0/roborock/web_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.0.0/PKG-INFO` & `python_roborock-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 2.0.0
+Version: 2.1.0
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Keywords: roborock,vacuum,homeassistant
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 2.0.0 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 2.1.0 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Keywords: roborock,vacuum,homeassistant
 Author: humbertogontijo Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
```


# Comparing `tmp/paloalto_panorama_sdk-0.0.6.tar.gz` & `tmp/paloalto_panorama_sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paloalto_panorama_sdk-0.0.6.tar", last modified: Fri May  3 06:33:16 2024, max compression
+gzip compressed data, was "paloalto_panorama_sdk-0.0.7.tar", last modified: Wed May  8 12:26:08 2024, max compression
```

## Comparing `paloalto_panorama_sdk-0.0.6.tar` & `paloalto_panorama_sdk-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.128786 paloalto_panorama_sdk-0.0.6/
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.6/LICENSE
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.6/MANIFEST.in
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-03 06:33:16.128521 paloalto_panorama_sdk-0.0.6/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)      809 2024-04-29 13:58:58.000000 paloalto_panorama_sdk-0.0.6/README.md
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.092019 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/
--rw-r--r--   0 timoriedinger   (501) staff       (20)      184 2024-05-03 06:30:37.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1803 2024-04-29 05:10:18.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/address_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/address_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1022 2024-04-29 13:29:41.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/key_manager.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.109558 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:16:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      735 2024-04-30 08:19:39.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/adress_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      926 2024-05-03 05:32:44.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/adress_group_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     2244 2024-05-03 05:30:44.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      751 2024-05-03 06:29:49.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/service_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)      705 2024-05-03 06:23:45.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/service_group_data.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     2185 2024-05-03 06:25:49.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_sdk.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     3567 2024-04-30 11:56:00.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/security_post_rules_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1842 2024-04-29 05:08:19.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/service_groups_manager.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/service_manager.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.105023 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/PKG-INFO
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1070 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/requires.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-05-03 06:33:15.000000 paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/top_level.txt
--rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-05-03 06:33:16.128876 paloalto_panorama_sdk-0.0.6/setup.cfg
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.6/setup.py
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.116272 paloalto_panorama_sdk-0.0.6/tests/
-drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-03 06:33:16.128034 paloalto_panorama_sdk-0.0.6/tests/PanoramaAPIMock/
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.6/tests/PanoramaAPIMock/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.6/tests/PanoramaAPIMock/panoramaAPIMock.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.6/tests/__init__.py
--rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:45:42.000000 paloalto_panorama_sdk-0.0.6/tests/test_service.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:08.137727 paloalto_panorama_sdk-0.0.7/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1089 2024-04-29 04:53:42.000000 paloalto_panorama_sdk-0.0.7/LICENSE
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 04:53:58.000000 paloalto_panorama_sdk-0.0.7/MANIFEST.in
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-08 12:26:08.135636 paloalto_panorama_sdk-0.0.7/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      809 2024-04-29 13:58:58.000000 paloalto_panorama_sdk-0.0.7/README.md
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:07.731671 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      185 2024-05-08 12:25:57.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1803 2024-04-29 05:10:18.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/address_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1533 2024-04-29 05:09:18.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/address_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      631 2024-05-08 12:05:24.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/device_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1022 2024-04-29 13:29:41.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/key_manager.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:07.994731 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-30 04:16:15.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      735 2024-04-30 08:19:39.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/address_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      926 2024-05-03 05:32:44.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/address_group_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      559 2024-05-08 12:10:05.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/device_group_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     2373 2024-05-08 06:06:03.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      751 2024-05-03 06:29:49.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/service_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      705 2024-05-03 06:23:45.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/service_group_data.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     2845 2024-05-08 12:12:05.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_sdk.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     4786 2024-05-08 05:09:52.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/security_post_rules_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1842 2024-04-29 05:08:19.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/service_groups_manager.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1620 2024-04-29 05:35:20.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/service_manager.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:07.744476 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1155 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1180 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        1 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)      590 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/requires.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       28 2024-05-08 12:26:07.000000 paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/top_level.txt
+-rw-r--r--   0 timoriedinger   (501) staff       (20)       38 2024-05-08 12:26:08.137841 paloalto_panorama_sdk-0.0.7/setup.cfg
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1455 2024-04-29 08:37:29.000000 paloalto_panorama_sdk-0.0.7/setup.py
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:08.050080 paloalto_panorama_sdk-0.0.7/tests/
+drwxr-xr-x   0 timoriedinger   (501) staff       (20)        0 2024-05-08 12:26:08.134544 paloalto_panorama_sdk-0.0.7/tests/PanoramaAPIMock/
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 06:04:15.000000 paloalto_panorama_sdk-0.0.7/tests/PanoramaAPIMock/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1078 2024-04-29 07:13:18.000000 paloalto_panorama_sdk-0.0.7/tests/PanoramaAPIMock/panoramaAPIMock.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)        0 2024-04-29 05:34:25.000000 paloalto_panorama_sdk-0.0.7/tests/__init__.py
+-rw-r--r--   0 timoriedinger   (501) staff       (20)     1035 2024-04-29 08:45:42.000000 paloalto_panorama_sdk-0.0.7/tests/test_service.py
```

### Comparing `paloalto_panorama_sdk-0.0.6/LICENSE` & `paloalto_panorama_sdk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/PKG-INFO` & `paloalto_panorama_sdk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paloalto_panorama_sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: This SDK is designed to make it easier to work with the Palo Alto Panorama API.
 Author: Timo Riedinger
 Author-email: timo.riedinger@bechtle.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paloalto_panorama_sdk-0.0.6/README.md` & `paloalto_panorama_sdk-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/address_groups_manager.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/address_groups_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/address_manager.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/address_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/key_manager.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/key_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/adress_data.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/address_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/adress_group_data.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/address_group_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,31 +8,32 @@
     name: str
     uuid: str
     location: str
     device_group: str
     loc: str
     description: str
     action: str
-    log_settings: str
+    log_setting: str
     from_member: 'Members'
     to_member: 'Members'
     source_member: 'Members'
     destination_member: 'Members'
     service_member: 'Members'
     application_member: 'Members'
     tag_member: 'Members'
-    profile_setting: 'Members'
+    profile_type: str
+    profile_setting: 'ProfileSettingMembers'
 
     @dataclass
     class Members:
         member: List[str]
 
     @dataclass
     class ProfileSettingMembers:
-        group: 'SecurityPostRule.Members'
+        profile_type: 'SecurityPostRule.Members'
 
     def to_json(self):
         data_dict = asdict(self)
         data_dict['@name'] = data_dict.pop("name")
         data_dict['@uuid'] = data_dict.pop("uuid")
         data_dict['@location'] = data_dict.pop("location")
         data_dict['@device-group'] = data_dict.pop("device_group")
@@ -44,19 +45,20 @@
         name = json_data.get('@name')
         uuid = json_data.get('@uuid')
         location = json_data.get('@location')
         device_group = json_data.get('@device-group')
         loc = json_data.get('@loc')
         description = json_data.get('description')
         action = json_data.get('action')
-        log_settings = json_data.get('log-settings')
+        log_setting = json_data.get('log-setting')
         from_member = json_data.get("from", {}).get('member')
         to_member = json_data.get("to", {}).get('member')
         source_member = json_data.get("source", {}).get('member')
         destination_member = json_data.get("destination", {}).get('member')
         service_member = json_data.get("service", {}).get('member')
         application_member = json_data.get("application", {}).get('member')
         tag_member = json_data.get("tag", {}).get('member')
-        profile_setting = json_data.get("profile-setting", {}).get('member')
-        return cls(name, uuid, location, device_group, loc, description, action, log_settings,
+        profile_type = list(json_data.get('profile-setting').keys())[0]
+        profile_setting = json_data.get("profile-setting", {}).get(profile_type)
+        return cls(name, uuid, location, device_group, loc, description, action, log_setting,
                    from_member, to_member, source_member, destination_member, service_member,
-                   application_member, tag_member, profile_setting)
+                   application_member, tag_member, profile_type, profile_setting)
```

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/service_data.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/service_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_data_kit/service_group_data.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_data_kit/service_group_data.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/panorama_sdk.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/panorama_sdk.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 from pprint import pprint
 
 from paloalto_panorama_sdk.address_groups_manager import AddressGroupsManager
 from paloalto_panorama_sdk.address_manager import AddressManager
+from paloalto_panorama_sdk.device_groups_manager import DeviceGroupsManager
 from paloalto_panorama_sdk.key_manager import KeyManager
-from paloalto_panorama_sdk.panorama_data_kit.adress_data import Address
-from paloalto_panorama_sdk.panorama_data_kit.adress_group_data import AddressGroup
+from paloalto_panorama_sdk.panorama_data_kit.address_data import Address
+from paloalto_panorama_sdk.panorama_data_kit.address_group_data import AddressGroup
+from paloalto_panorama_sdk.panorama_data_kit.device_group_data import DeviceGroup
 from paloalto_panorama_sdk.panorama_data_kit.security_post_rule_data import SecurityPostRule
 from paloalto_panorama_sdk.panorama_data_kit.service_data import Service
 from paloalto_panorama_sdk.panorama_data_kit.service_group_data import ServiceGroup
 from paloalto_panorama_sdk.security_post_rules_manager import SecurityPostRulesManager
 from paloalto_panorama_sdk.service_groups_manager import ServiceGroupsManager
 from paloalto_panorama_sdk.service_manager import ServiceManager
 from dotenv import load_dotenv
@@ -26,24 +28,34 @@
             panorama_url=self.url,
             user=self.username,
             password=self.password,
             verify=verify
         )
         self.address_group = AddressGroupsManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
         self.address = AddressManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
+        self.device_group = DeviceGroupsManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
         self.security_post_rule = SecurityPostRulesManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
         self.service_group = ServiceGroupsManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
         self.service = ServiceManager(panorama_url=self.url, api_key=self.apikey, verify=verify)
 
 
 if __name__ == '__main__':
     panSDK = PanoramaSDK(
         url=os.getenv("url", ""),
         username=os.getenv("user", "test"),
         password=os.getenv("password", "testpass"),
         verify=False
     )
-    serOutput = panSDK.service.list_services()
-    se = Service.from_json(serOutput['result']['entry'][0])
-    pprint(serOutput)
-    print(se)
-    pprint(se.to_json())
+    # output = panSDK.device_group.list_device_groups()['result']['entry'][0]
+    # output2 = panSDK.device_group.list_device_groups()['result']['entry'][1]
+    # print(output)
+    # print(output2)
+    # obj = DeviceGroup.from_json(output)
+    # obj2 = DeviceGroup.from_json(output2)
+    # print(obj)
+    # print(obj2)
+
+    # output = panSDK.security_post_rule.list_post_rules(location='device-group', device_group='NewTest')
+    # obj = SecurityPostRule.from_json(output['result']['entry'][0])
+    # pprint(output)
+    # print(obj)
+    # pprint(obj.to_json())
```

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/security_post_rules_manager.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/security_post_rules_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,46 @@
 import json
 import requests
+from paloalto_panorama_sdk.panorama_data_kit.security_post_rule_data import SecurityPostRule
 
 
 class SecurityPostRulesManager:
     def __init__(self, panorama_url, api_key, verify=True):
         self.panorama_url = panorama_url
         self.api_key = api_key
         self.verify = verify
         self.url = f"{self.panorama_url}/restapi/v10.2/Policies/SecurityPostRules"
         self.headers = {'Content-Type': 'application/json',
                         'X-PAN-KEY': f"{self.api_key}"}
 
-    def list_post_rules(self, location='shared', devicegroup='TestGroup'):
-        params = {'location': location, 'device-group': devicegroup}
+    def get_security_post_rules(self, location='shared', device_group='TestGroup'):
+        post_rules_list = self.list_post_rules(location=location, device_group=device_group)
+        post_rules: [SecurityPostRule] = []
+        for post_rule in post_rules_list:
+            post_rules.append(post_rule)
+        return post_rules
+
+    def post_security_post_rule(self, security_post_rule: SecurityPostRule):
+        decoded_security_post_rule = self.create_post_rules(
+            device_group=security_post_rule.device_group,
+            name=security_post_rule.name,
+            action=security_post_rule.action,
+            description=security_post_rule.description,
+            from_zone=security_post_rule.from_member,
+            source_group=security_post_rule.source_member,
+            to_zone=security_post_rule.to_member,
+            destination_group=security_post_rule.destination_member,
+            service=security_post_rule.service_member,
+            profile_type=security_post_rule.profile_type,
+            profile=security_post_rule.profile_setting
+        )
+        print(decoded_security_post_rule)
+
+    def list_post_rules(self, location='shared', device_group='TestGroup'):
+        params = {'location': location, 'device-group': device_group}
         response = requests.get(url=self.url, headers=self.headers, params=params, verify=self.verify)
         post_rules = json.loads(response.content.decode('utf-8'))
         return post_rules
 
     def create_post_rules(self, device_group, name, action, description, from_zone, source_group,
                           to_zone, destination_group, service, profile_type, profile):
         location = "shared" if device_group == 'shared' else "device-group"
```

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/service_groups_manager.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/service_groups_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk/service_manager.py` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk/service_manager.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/PKG-INFO` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paloalto-panorama-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: This SDK is designed to make it easier to work with the Palo Alto Panorama API.
 Author: Timo Riedinger
 Author-email: timo.riedinger@bechtle.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/SOURCES.txt` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 paloalto_panorama_sdk/__init__.py
 paloalto_panorama_sdk/address_groups_manager.py
 paloalto_panorama_sdk/address_manager.py
+paloalto_panorama_sdk/device_groups_manager.py
 paloalto_panorama_sdk/key_manager.py
 paloalto_panorama_sdk/panorama_sdk.py
 paloalto_panorama_sdk/security_post_rules_manager.py
 paloalto_panorama_sdk/service_groups_manager.py
 paloalto_panorama_sdk/service_manager.py
 paloalto_panorama_sdk.egg-info/PKG-INFO
 paloalto_panorama_sdk.egg-info/SOURCES.txt
 paloalto_panorama_sdk.egg-info/dependency_links.txt
 paloalto_panorama_sdk.egg-info/requires.txt
 paloalto_panorama_sdk.egg-info/top_level.txt
 paloalto_panorama_sdk/panorama_data_kit/__init__.py
-paloalto_panorama_sdk/panorama_data_kit/adress_data.py
-paloalto_panorama_sdk/panorama_data_kit/adress_group_data.py
+paloalto_panorama_sdk/panorama_data_kit/address_data.py
+paloalto_panorama_sdk/panorama_data_kit/address_group_data.py
+paloalto_panorama_sdk/panorama_data_kit/device_group_data.py
 paloalto_panorama_sdk/panorama_data_kit/security_post_rule_data.py
 paloalto_panorama_sdk/panorama_data_kit/service_data.py
 paloalto_panorama_sdk/panorama_data_kit/service_group_data.py
 tests/__init__.py
 tests/test_service.py
 tests/PanoramaAPIMock/__init__.py
 tests/PanoramaAPIMock/panoramaAPIMock.py
```

### Comparing `paloalto_panorama_sdk-0.0.6/paloalto_panorama_sdk.egg-info/requires.txt` & `paloalto_panorama_sdk-0.0.7/paloalto_panorama_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/setup.py` & `paloalto_panorama_sdk-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/tests/PanoramaAPIMock/panoramaAPIMock.py` & `paloalto_panorama_sdk-0.0.7/tests/PanoramaAPIMock/panoramaAPIMock.py`

 * *Files identical despite different names*

### Comparing `paloalto_panorama_sdk-0.0.6/tests/test_service.py` & `paloalto_panorama_sdk-0.0.7/tests/test_service.py`

 * *Files identical despite different names*


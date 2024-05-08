# Comparing `tmp/pyneople-0.3.0.tar.gz` & `tmp/pyneople-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.3.0.tar", last modified: Mon May  6 14:02:07 2024, max compression
+gzip compressed data, was "pyneople-0.3.1.tar", last modified: Wed May  8 08:04:07 2024, max compression
```

## Comparing `pyneople-0.3.0.tar` & `pyneople-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:02:07.537819 pyneople-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 14:01:55.000000 pyneople-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 14:02:07.537819 pyneople-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-06 14:01:55.000000 pyneople-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 14:01:55.000000 pyneople-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:02:07.537819 pyneople-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-06 14:01:55.000000 pyneople-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:02:07.533819 pyneople-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:02:07.533819 pyneople-0.3.0/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39741 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)    22685 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/database_connecter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:02:07.537819 pyneople-0.3.0/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 14:02:07.000000 pyneople-0.3.0/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 14:02:07.000000 pyneople-0.3.0/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:02:07.000000 pyneople-0.3.0/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 14:02:07.000000 pyneople-0.3.0/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:04:07.364817 pyneople-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 08:03:57.000000 pyneople-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 08:04:07.360817 pyneople-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 08:03:57.000000 pyneople-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 08:03:57.000000 pyneople-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 08:04:07.364817 pyneople-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 08:03:57.000000 pyneople-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:04:07.360817 pyneople-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:04:07.360817 pyneople-0.3.1/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-08 08:03:57.000000 pyneople-0.3.1/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 08:03:57.000000 pyneople-0.3.1/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37543 2024-05-08 08:03:57.000000 pyneople-0.3.1/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-05-08 08:03:57.000000 pyneople-0.3.1/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-08 08:03:57.000000 pyneople-0.3.1/src/pyneople/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 08:04:07.360817 pyneople-0.3.1/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 08:04:07.000000 pyneople-0.3.1/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 08:04:07.000000 pyneople-0.3.1/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 08:04:07.000000 pyneople-0.3.1/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 08:04:07.000000 pyneople-0.3.1/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.3.0/LICENSE` & `pyneople-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.0/PKG-INFO` & `pyneople-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.3.0
+Version: 0.3.1
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.3.0/setup.py` & `pyneople-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.3.0",
+    version="0.3.1",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.3.0/src/pyneople/METADATA.py` & `pyneople-0.3.1/src/pyneople/METADATA.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.0/src/pyneople/character.py` & `pyneople-0.3.1/src/pyneople/character.py`

 * *Files 4% similar despite different names*

```diff
@@ -384,21 +384,15 @@
             else:
                 pass    
 
     def get_equipment_data(self, arg_equipment_dict):
         super().get_equipment_data(arg_equipment_dict)
         for sub_attribute in Weapon.sub_attribute_list:
             getattr(self, sub_attribute).get_info_data(arg_equipment_dict.get(WEAPON_NAME[sub_attribute], dict()))
-            # if sub_attribute == 'bakal_info':
-            #     self.bakal_info.get_bakal_info_data(arg_equipment_dict.get(WEAPON_NAME[sub_attribute], dict())) # 바칼 무기 융합
-            # elif sub_attribute == 'asrahan_info':
-            #     self.asrahan_info.get_asrahan_info_data(arg_equipment_dict.get("asrahanOption", dict()))
-            # else:
-            #     pass    
-
+            
 class Equipments(PyNeopleAttributeSetter):
     """
     Neople Open API 06. 캐릭터 '장착 장비' 조회
     """    
     default_sub_attribute_list = EQUIPMENT_LIST
     sub_attribute_list = default_sub_attribute_list
     
@@ -462,30 +456,22 @@
         for sub_attribute in Avatar.sub_attribute_list:
             if sub_attribute == "emblems":
                 for i in range(1,3):
                     setattr(self, f"{sub_attribute}_{i}", None)
             else:
                 setattr(self, sub_attribute, None)
 
-        # self.item_name = None       # 아바타 이름
-        # self.item_rarity = None     # 아바타 레어도
-        # self.option_ability = None  # 아바타 옵션
-        # self.emblem_1 = None        # 엠블렘1 옵션
-        # self.emblem_2 = None        # 엠블렘2 옵션
-
     def get_avatar_data(self, arg_avatar_dict):
         for sub_attribute in Avatar.sub_attribute_list:
             if sub_attribute == 'emblems':
                 for emblem in arg_avatar_dict.get('emblems', dict()):
                     setattr(self, f"{sub_attribute}_{emblem.get('slotNo')}", emblem.get('itemName'))
             else:    
                 setattr(self, sub_attribute, arg_avatar_dict.get(AVATAR_NAME[sub_attribute]))
-        # self.item_name = arg_avatar_dict.get("itemName")
-        # self.item_rarity = arg_avatar_dict.get("itemRarity")
-        # self.option_ability = arg_avatar_dict.get("optionAbility")
+
 
 
 
 class PlatinumAvatar(Avatar):
     """
     Avatars를 위해 사용되는 Class
     """   
@@ -495,20 +481,15 @@
             if sub_attribute == "emblems":
                 for i in range(1,3):
                     setattr(self, f"{sub_attribute}_{i}", None)
             elif sub_attribute == "platinum_emblem":
                 setattr(self, sub_attribute, None)    
             else:
                 setattr(self, sub_attribute, None)
-    # @classmethod
-    # def set_sub_attributes(cls, new_attribute_list : list[str]):
-    #     for new_attribute in new_attribute_list:
-    #         if not new_attribute in cls.sub_attribute_list:
-    #             raise ValueError("사용할 수 없는 하위 속성입니다.")         
-    #     cls.sub_attribute_list = new_attribute_list
+
     def get_avatar_data(self, arg_avatar_dict):
         
         for sub_attribute in PlatinumAvatar.sub_attribute_list:
             if sub_attribute == 'emblems':
                 for emblem in arg_avatar_dict.get(PLATINUM_AVATAR_NAME[sub_attribute], dict()):
                     if emblem.get('slotColor') != '플래티넘':
                         setattr(self, f"{sub_attribute}_{emblem.get('slotNo') - 1}", emblem.get('itemName'))
@@ -521,20 +502,14 @@
 
 class Avatars(PyNeopleAttributeSetter):
     """
     Neople Open API 07. 캐릭터 '장착 아바타' 조회
     """       
     default_sub_attribute_list = AVATAR_LIST
     sub_attribute_list = default_sub_attribute_list
-    def __init__(self, arg_api_key: str):
-        super().__init__(arg_api_key)
-    
-    @classmethod
-    def set_sub_attributes(cls, new_attribute_list : list[str]):
-        cls.sub_attribute_list = new_attribute_list
 
     def get_data(self, arg_server_id: str, arg_character_id : str):    
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 아바타 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
@@ -563,17 +538,14 @@
                 getattr(self, f'{avatar["slotId"].lower()}').get_avatar_data(avatar)
 
 
 class Creature(PyNeople):
     """
     Neople Open API 08. 캐릭터 '장착 크리쳐' 조회
     """
-    
-    def __init__(self, arg_api_key: str):
-        super().__init__(arg_api_key)
         
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 크리쳐 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
@@ -591,17 +563,14 @@
         """        
         self.creature = arg_data.get('creature', dict()).get('itemName')
         
 class Flag(PyNeople):
     """
     Neople Open API 09. 캐릭터 '장착 휘장' 조회
     """
-
-    def __init__(self, arg_api_key: str):
-        super().__init__(arg_api_key)
     
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 휘장 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
@@ -641,16 +610,14 @@
         for i, rune in enumerate(arg_talisman_data.get('runes', list())):
             setattr(self, f'rune_{i+1}', rune.get('itemName'))        
 
 class Talismans(PyNeople):
     """
     Neople Open API 10. 캐릭터 '장착 탈리스만' 조회
     """ 
-    def __init__(self, arg_api_key: str):
-        super().__init__(arg_api_key)
 
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 탈리스만 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
@@ -672,17 +639,14 @@
 
 
 class EquipmentTrait(PyNeople):
     """
     Neople Open API 11. 캐릭터 '장비 특성' 조회
     """ 
 
-    def __init__(self, arg_api_key: str):
-        super().__init__(arg_api_key)
-
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장비 특성 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
@@ -713,17 +677,14 @@
 
 
 class SkillStyle(PyNeople):
     """
     Neople Open API 12. 캐릭터 '스킬 스타일' 조회
     """ 
 
-    def __init__(self, arg_api_key: str):
-        super().__init__(arg_api_key)
-
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 스킬 스타일 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
@@ -774,17 +735,14 @@
 
 class Buff(PyNeople):
     """
     Neople Open API 13. 캐릭터 "버프 스킬 강화 장착 장비" 조회
     Neople Open API 14. 캐릭터 "버프 스킬 강화 장착 아바타" 조회
     Neople Open API 15. 캐릭터 "버프 스킬 강화 장착 크리쳐" 조회
     """
-
-    def __init__(self, arg_api_key: str):
-        super().__init__(arg_api_key)
          
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 버프 강화(장비, 아바타, 크리쳐) 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
@@ -843,35 +801,29 @@
     
         # 버프 강화 아바타
         if arg_buff_avatar_data.get("skill", dict()).get('buff'):
             arg_buff_avatar_data = arg_buff_avatar_data.get("skill", dict()).get('buff')
             if arg_buff_avatar_data.get("avatar"):
                 for buff_avatar in arg_buff_avatar_data.get("avatar"):
                     if buff_avatar.get("slotId").lower() in PLATINUM_AVATAR_LIST:
-                        # setattr(self, f'avatar_{buff_avatar.get("slotId").lower()}', BuffPlatimun())
                         getattr(self, f'avatar_{buff_avatar.get("slotId").lower()}').get_buff_avatar_data(buff_avatar)
                     else:
-                        # setattr(self, f'avatar_{buff_avatar.get("slotId").lower()}', BuffAvatar())
                         getattr(self, f'avatar_{buff_avatar.get("slotId").lower()}').get_buff_avatar_data(buff_avatar)
 
         # 버프 강화 크리쳐
         if arg_buff_creature_data.get("skill", dict()).get('buff'):
             arg_buff_creature_data = arg_buff_creature_data.get("skill", dict()).get('buff')
             if arg_buff_creature_data.get('creature'):
                 for creature in arg_buff_creature_data.get('creature'):
                     setattr(self, 'creature', creature.get('itemName'))
 
 class CharacterFame(PyNeople):
     """
     Neople Open API 16. 캐릭터 명성 검색
     """    
-
-    def __init__(self, arg_api_key: str):
-        super().__init__(arg_api_key)
-
     def get_data(self, arg_min_fame : int, 
                   arg_max_fame : int,
                   arg_job_id : str = "",
                   arg_job_grow_id : str = "",
                   arg_is_all_job_grow : bool = False, 
                   arg_is_buff : bool = "", 
                   arg_server_id : str = "all",
```

### Comparing `pyneople-0.3.0/src/pyneople/database_connecter.py` & `pyneople-0.3.1/src/pyneople/database_connecter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from multiprocessing import Process, Queue, Value
 from pymongo import MongoClient
 from typing import Callable
 from psycopg2 import sql
 from typing import Union
 import psycopg2
 
+__all__ = [
+    'store_fame_data_to_mongodb',
+    'store_character_data_to_mongodb',
+    'store_timeline_data_to_mongodb',
+    'PostgreSQLConnecter',
+    'mongodb_to_postgresql'
+]
+
 def store_fame_data_to_mongodb(
         arg_mongo_client_instance : MongoClient,
         arg_database_name : str,
         arg_collection_name : str,
         arg_api_key_list : list[str],
         arg_max_fame : int = 100000):
     """
```

### Comparing `pyneople-0.3.0/src/pyneople/functions.py` & `pyneople-0.3.1/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.3.0/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.3.1/src/pyneople.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.3.0
+Version: 0.3.1
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


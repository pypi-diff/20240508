# Comparing `tmp/audiostack-1.2.5.tar.gz` & `tmp/audiostack-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostack-1.2.5.tar", last modified: Wed May  1 09:11:43 2024, max compression
+gzip compressed data, was "audiostack-1.3.0.tar", last modified: Wed May  8 15:53:40 2024, max compression
```

## Comparing `audiostack-1.2.5.tar` & `audiostack-1.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.667961 audiostack-1.2.5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-05-01 09:11:22.000000 audiostack-1.2.5/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-01 09:11:43.667961 audiostack-1.2.5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2024-05-01 09:11:22.000000 audiostack-1.2.5/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.659961 audiostack-1.2.5/audiostack/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-05-01 09:11:38.000000 audiostack-1.2.5/audiostack/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/content/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6077 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/media.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/recommend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      947 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/root_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4183 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/content/script.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/delivery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/delivery/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3460 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/delivery/encoder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/delivery/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/docs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/docs/docs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/helpers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/api_item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/api_list.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4732 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/request_interface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/request_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/helpers/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/orchestrator/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/orchestrator/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/production/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      134 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/production/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4703 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/production/mix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/production/sound.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3844 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/production/suite.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack/speech/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2979 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/diction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/predict.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7488 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/tts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2024-05-01 09:11:22.000000 audiostack-1.2.5/audiostack/speech/voice.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-01 09:11:43.663961 audiostack-1.2.5/audiostack.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-05-01 09:11:43.000000 audiostack-1.2.5/audiostack.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-01 09:11:43.667961 audiostack-1.2.5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2024-05-01 09:11:22.000000 audiostack-1.2.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.317243 audiostack-1.3.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-05-08 15:53:07.000000 audiostack-1.3.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-08 15:53:40.317243 audiostack-1.3.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2024-05-08 15:53:07.000000 audiostack-1.3.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.309243 audiostack-1.3.0/audiostack/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2024-05-08 15:53:33.000000 audiostack-1.3.0/audiostack/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/content/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      592 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6077 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/media.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/recommend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      947 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/root_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4183 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/content/script.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/delivery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/delivery/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3462 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/delivery/encoder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2078 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/delivery/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/docs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/docs/docs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/helpers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      715 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/api_item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      972 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/api_list.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4732 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/request_interface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/request_types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      338 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/helpers/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/orchestrator/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/orchestrator/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.313243 audiostack-1.3.0/audiostack/production/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      134 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/production/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/production/mix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4286 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/production/sound.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4265 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/production/suite.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.317243 audiostack-1.3.0/audiostack/speech/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2979 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/diction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/predict.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7488 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/tts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2024-05-08 15:53:07.000000 audiostack-1.3.0/audiostack/speech/voice.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 15:53:40.317243 audiostack-1.3.0/audiostack.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5458 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2024-05-08 15:53:40.000000 audiostack-1.3.0/audiostack.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-08 15:53:40.317243 audiostack-1.3.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2024-05-08 15:53:07.000000 audiostack-1.3.0/setup.py
```

### Comparing `audiostack-1.2.5/LICENSE` & `audiostack-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/PKG-INFO` & `audiostack-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 1.2.5
+Version: 1.3.0
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 1.2.5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 1.3.0 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests>=2.28.1; python_version >= "3.6"
                                _[_a_p_i_._a_u_d_i_o_ _l_o_g_o_]
```

### Comparing `audiostack-1.2.5/README.md` & `audiostack-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/content/__init__.py` & `audiostack-1.3.0/audiostack/content/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/content/file.py` & `audiostack-1.3.0/audiostack/content/file.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/content/media.py` & `audiostack-1.3.0/audiostack/content/media.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/content/recommend.py` & `audiostack-1.3.0/audiostack/content/recommend.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/content/root_functions.py` & `audiostack-1.3.0/audiostack/content/root_functions.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/content/script.py` & `audiostack-1.3.0/audiostack/content/script.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/delivery/encoder.py` & `audiostack-1.3.0/audiostack/delivery/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         r = Encoder.interface.send_request(
             rtype=RequestTypes.POST, route="encoder", json=body
         )
         
         while r["statusCode"] == 202:
             encoderId = r["data"]["encoderId"]
             r = Encoder.interface.send_request(
-                rtype=RequestTypes.GET, route="video", path_parameters=encoderId
+                rtype=RequestTypes.GET, route="encoder", path_parameters=encoderId
             )
         return Encoder.Item(r)
 
     @staticmethod
     def list_presets() -> Item:
         r = Encoder.interface.send_request(
             rtype=RequestTypes.GET, route="encoder/presets", path_parameters=""
```

### Comparing `audiostack-1.2.5/audiostack/delivery/video.py` & `audiostack-1.3.0/audiostack/delivery/video.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/docs/docs.py` & `audiostack-1.3.0/audiostack/docs/docs.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/helpers/api_item.py` & `audiostack-1.3.0/audiostack/helpers/api_item.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/helpers/api_list.py` & `audiostack-1.3.0/audiostack/helpers/api_list.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/helpers/request_interface.py` & `audiostack-1.3.0/audiostack/helpers/request_interface.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/production/mix.py` & `audiostack-1.3.0/audiostack/production/mix.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,54 +41,59 @@
                 return
 
             else:
                 raise Exception()
 
     @staticmethod
     def create(
-        speechId="",
+        speechId: str="",
+        scriptId: str="",
         speechItem=None,
         soundTemplate: str = "",
         mediaFiles: dict = {},
         fxFiles: dict = {},
         sectionProperties: dict = {},
         timelineProperties: dict = {},
         masteringPreset: str = "",
         public: bool = False,
         exportSettings: dict = {},
         strictValidation: bool = True,
         validate: bool = False,
         soundLayer: str = "default"
     ) -> Item:
-        if speechId and speechItem:
-            raise Exception("speechId or scriptItem should be supplied not both")
-        if not (speechId or speechItem):
-            raise Exception("speechId or scriptItem should be supplied")
+        counts = sum([1 for i in [speechId, scriptId, speechItem] if i])
+        if counts != 1:
+            raise Exception("only 1 of the following is required; speechId, speechItem, or scriptId")
+        
         if speechItem:
             speechId = speechItem.speechId
 
         if not isinstance(soundTemplate, str):
             raise Exception("soundTemplate argument should be a string")
         if not isinstance(masteringPreset, str):
             raise Exception("masteringPreset should be a string")
         
 
         body = {
-            "speechId": speechId,
             "soundTemplate": soundTemplate,
             "mediaFiles": mediaFiles,
             "fxFiles": fxFiles,
             "sectionProperties": sectionProperties,
             "timelineProperties": timelineProperties,
             "soundLayer": soundLayer,
             "masteringPreset": masteringPreset,
             "public": public,
             "exportSettings" : exportSettings,
             "strictValidation" : strictValidation
         }
+        if speechId:
+            body["speechId"] = speechId
+        elif scriptId:
+            body["scriptId"] = scriptId
+
         if validate:
             r = Mix.interface.send_request(rtype=RequestTypes.POST, route="validate", json=body)
         else:
             r = Mix.interface.send_request(rtype=RequestTypes.POST, route="mix", json=body)
             
         while r["statusCode"] == 202:
             print("Response in progress please wait...")
```

### Comparing `audiostack-1.2.5/audiostack/production/sound.py` & `audiostack-1.3.0/audiostack/production/sound.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/production/suite.py` & `audiostack-1.3.0/audiostack/production/suite.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from audiostack.helpers.request_interface import RequestInterface
 from audiostack.helpers.request_types import RequestTypes
 from audiostack.helpers.api_item import APIResponseItem
 from audiostack.content.file import File
 from typing import List, Optional
 
 class Suite:
+    DENOISE_ENDPOINT = "suite/denoise"
+    class FailedPipeline(Exception):
+        pass
+    
     interface = RequestInterface(family="production")
 
     class EvaluationItem(APIResponseItem):
         def __init__(self, response) -> None:
             super().__init__(response)
 
     class PipelineInProgressItem(APIResponseItem):
@@ -80,25 +84,33 @@
     @staticmethod
     def denoise(fileId: str, level: Optional[int] = None, wait=True):
 
         body = {
             "fileId": fileId,
             "level": level
         }
-        r = Suite.interface.send_request(rtype=RequestTypes.POST, route="suite/denoise", json=body)
+        r = Suite.interface.send_request(rtype=RequestTypes.POST, route=Suite.DENOISE_ENDPOINT, json=body)
         item = Suite.PipelineInProgressItem(r)
         return Suite._poll(r, item.pipelineId) if wait else item
         
 
     @staticmethod
     def _poll(r, pipelineId: str):
         while r["statusCode"] == 202:
             r = Suite.interface.send_request(
                 rtype=RequestTypes.GET, route="suite/pipeline", path_parameters=pipelineId
             )
+        
+        status = r.get("data", {}).get("status", 200)
+        if status > 400:
+            msg = r.get("data", {}).get("message")
+            errors = r.get("data", {}).get("errors")
+            raise Suite.FailedPipeline("pipeline failed: ", msg, "errors are as follows: ", ','.join(errors))
+        
         return Suite.PipelineFinishedItem(r)
 
 
     @staticmethod
     def get(pipelineId: str):
         r = Suite.interface.send_request(rtype=RequestTypes.GET, route="suite/pipeline", path_parameters=pipelineId)
+        
         return Suite._poll(r, pipelineId)
```

### Comparing `audiostack-1.2.5/audiostack/speech/diction.py` & `audiostack-1.3.0/audiostack/speech/diction.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/speech/predict.py` & `audiostack-1.3.0/audiostack/speech/predict.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/speech/tts.py` & `audiostack-1.3.0/audiostack/speech/tts.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack/speech/voice.py` & `audiostack-1.3.0/audiostack/speech/voice.py`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/audiostack.egg-info/PKG-INFO` & `audiostack-1.3.0/audiostack.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostack
-Version: 1.2.5
+Version: 1.3.0
 Summary: Python SDK for Audiostack API
 Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic
 Author-email: sam@aflorithmic.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: audiostack Version: 1.2.5 Summary: Python SDK for
+Metadata-Version: 2.1 Name: audiostack Version: 1.3.0 Summary: Python SDK for
 Audiostack API Home-page: https://github.com/aflorithmic/audiostack-python
 Author: Aflorithmic Author-email: sam@aflorithmic.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests>=2.28.1; python_version >= "3.6"
                                _[_a_p_i_._a_u_d_i_o_ _l_o_g_o_]
```

### Comparing `audiostack-1.2.5/audiostack.egg-info/SOURCES.txt` & `audiostack-1.3.0/audiostack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostack-1.2.5/setup.py` & `audiostack-1.3.0/setup.py`

 * *Files identical despite different names*


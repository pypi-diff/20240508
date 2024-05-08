# Comparing `tmp/wonder-diffusion-sdk-0.0.6.dev1.tar.gz` & `tmp/wonder-diffusion-sdk-0.0.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-diffusion-sdk-0.0.6.dev1.tar", last modified: Mon May  6 11:35:20 2024, max compression
+gzip compressed data, was "wonder-diffusion-sdk-0.0.6.dev2.tar", last modified: Wed May  8 06:41:58 2024, max compression
```

## Comparing `wonder-diffusion-sdk-0.0.6.dev1.tar` & `wonder-diffusion-sdk-0.0.6.dev2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-06 11:35:20.878544 wonder-diffusion-sdk-0.0.6.dev1/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.6.dev1/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-05-06 11:35:20.878397 wonder-diffusion-sdk-0.0.6.dev1/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2024-05-06 11:35:20.878598 wonder-diffusion-sdk-0.0.6.dev1/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      319 2024-05-06 11:34:16.000000 wonder-diffusion-sdk-0.0.6.dev1/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-06 11:35:20.871247 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     7905 2024-05-06 11:33:19.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/__init__.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-06 11:35:20.874268 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/
--rw-r--r--   0 basri      (501) staff       (20)      344 2024-04-30 13:54:56.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/deepcache.py
--rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/dotdict.py
--rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/lightning.py
--rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/logger.py
--rw-r--r--   0 basri      (501) staff       (20)     2773 2024-04-30 13:54:27.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/lora.py
--rw-r--r--   0 basri      (501) staff       (20)     1551 2024-04-30 13:42:41.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/optimizations.py
--rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/safety_checker.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-06 11:35:20.876333 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/
--rw-r--r--   0 basri      (501) staff       (20)      255 2024-04-30 13:32:54.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      740 2024-04-30 13:29:32.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/controlnet_config.py
--rw-r--r--   0 basri      (501) staff       (20)       70 2024-04-30 13:32:07.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/globals.py
--rw-r--r--   0 basri      (501) staff       (20)     1139 2024-04-30 13:30:09.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/lora_config.py
--rw-r--r--   0 basri      (501) staff       (20)     2106 2024-04-30 13:33:56.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/model_config.py
--rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/sdk_config.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-06 11:35:20.878106 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/
--rw-r--r--   0 basri      (501) staff       (20)      257 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      112 2024-05-06 11:32:54.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/controlnet_type.py
--rw-r--r--   0 basri      (501) staff       (20)     1032 2024-05-06 11:32:51.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/controlnets.py
--rw-r--r--   0 basri      (501) staff       (20)      837 2024-05-06 11:31:51.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/pipeline_type.py
--rw-r--r--   0 basri      (501) staff       (20)     4336 2024-05-06 11:33:02.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/pipelines.py
--rw-r--r--   0 basri      (501) staff       (20)      815 2024-05-06 11:33:06.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/scheduler_type.py
--rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/schedulers.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-06 11:35:20.872198 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-05-06 11:35:20.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)     1180 2024-05-06 11:35:20.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2024-05-06 11:35:20.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       18 2024-05-06 11:35:20.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk.egg-info/requires.txt
--rw-r--r--   0 basri      (501) staff       (20)       21 2024-05-06 11:35:20.000000 wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:41:58.421918 wonder-diffusion-sdk-0.0.6.dev2/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.6.dev2/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      190 2024-05-08 06:41:58.421777 wonder-diffusion-sdk-0.0.6.dev2/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2024-05-08 06:41:58.421969 wonder-diffusion-sdk-0.0.6.dev2/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      319 2024-05-08 06:41:52.000000 wonder-diffusion-sdk-0.0.6.dev2/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:41:58.414480 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     8032 2024-05-08 06:41:20.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/__init__.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:41:58.417767 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/
+-rw-r--r--   0 basri      (501) staff       (20)      344 2024-04-30 13:54:56.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/deepcache.py
+-rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/dotdict.py
+-rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/lightning.py
+-rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/logger.py
+-rw-r--r--   0 basri      (501) staff       (20)     2773 2024-04-30 13:54:27.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/lora.py
+-rw-r--r--   0 basri      (501) staff       (20)     1551 2024-04-30 13:42:41.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/optimizations.py
+-rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/safety_checker.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:41:58.419568 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/
+-rw-r--r--   0 basri      (501) staff       (20)      255 2024-04-30 13:32:54.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      740 2024-04-30 13:29:32.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/controlnet_config.py
+-rw-r--r--   0 basri      (501) staff       (20)       70 2024-04-30 13:32:07.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/globals.py
+-rw-r--r--   0 basri      (501) staff       (20)     1139 2024-04-30 13:30:09.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/lora_config.py
+-rw-r--r--   0 basri      (501) staff       (20)     2106 2024-04-30 13:33:56.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/model_config.py
+-rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/sdk_config.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:41:58.421383 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/
+-rw-r--r--   0 basri      (501) staff       (20)      257 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      112 2024-05-06 11:32:54.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/controlnet_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     1032 2024-05-06 11:32:51.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/controlnets.py
+-rw-r--r--   0 basri      (501) staff       (20)      837 2024-05-06 11:31:51.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/pipeline_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     4336 2024-05-06 11:33:02.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/pipelines.py
+-rw-r--r--   0 basri      (501) staff       (20)      815 2024-05-06 11:33:06.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/scheduler_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/schedulers.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:41:58.415414 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      190 2024-05-08 06:41:58.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)     1180 2024-05-08 06:41:58.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2024-05-08 06:41:58.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       18 2024-05-08 06:41:58.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk.egg-info/requires.txt
+-rw-r--r--   0 basri      (501) staff       (20)       21 2024-05-08 06:41:58.000000 wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk.egg-info/top_level.txt
```

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/LICENCE` & `wonder-diffusion-sdk-0.0.6.dev2/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/__init__.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,18 @@
         # initialize controlnets
         if model_config.controlnet_config != None:
             controlnets = []
             for c in model_config.controlnet_config.controlnets:
                 controlnet = self.initialize_controlnet(c)
                 controlnets.append(controlnet)
                 controlnet.to(DEVICE)
-            model_config.kwargs['controlnet'] = controlnets
+            if len(controlnets) == 1:
+                model_config.kwargs['controlnet'] = controlnets[0]
+            else:
+                model_config.kwargs['controlnet'] = controlnets
 
         # initialize pipeline
         self.pipeline = PIPELINE_MAP[model_config.pipeline_type](
             model_config.pretrained_model_name_or_path, **model_config.kwargs)
 
         self.pipeline.scheduler = SCHEDULER_MAP[model_config.initial_scheduler](
             self.pipeline.scheduler.config)
```

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/lightning.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/lightning.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/logger.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/logger.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/lora.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/lora.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/optimizations.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/optimizations.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/components/safety_checker.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/components/safety_checker.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/controlnet_config.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/controlnet_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/lora_config.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/lora_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/config/model_config.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/config/model_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/controlnets.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/controlnets.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/pipeline_type.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/pipeline_type.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/pipelines.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/pipelines.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/scheduler_type.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/scheduler_type.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk/types/schedulers.py` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk/types/schedulers.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev1/wonder_diffusion_sdk.egg-info/SOURCES.txt` & `wonder-diffusion-sdk-0.0.6.dev2/wonder_diffusion_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


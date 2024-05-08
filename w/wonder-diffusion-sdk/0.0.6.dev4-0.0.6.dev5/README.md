# Comparing `tmp/wonder-diffusion-sdk-0.0.6.dev4.tar.gz` & `tmp/wonder-diffusion-sdk-0.0.6.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-diffusion-sdk-0.0.6.dev4.tar", last modified: Wed May  8 06:57:33 2024, max compression
+gzip compressed data, was "wonder-diffusion-sdk-0.0.6.dev5.tar", last modified: Wed May  8 08:54:39 2024, max compression
```

## Comparing `wonder-diffusion-sdk-0.0.6.dev4.tar` & `wonder-diffusion-sdk-0.0.6.dev5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:57:33.411345 wonder-diffusion-sdk-0.0.6.dev4/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.6.dev4/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-05-08 06:57:33.411202 wonder-diffusion-sdk-0.0.6.dev4/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2024-05-08 06:57:33.411403 wonder-diffusion-sdk-0.0.6.dev4/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      319 2024-05-08 06:57:30.000000 wonder-diffusion-sdk-0.0.6.dev4/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:57:33.403961 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/
--rw-r--r--   0 basri      (501) staff       (20)     8113 2024-05-08 06:57:22.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/__init__.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:57:33.406803 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/
--rw-r--r--   0 basri      (501) staff       (20)      344 2024-04-30 13:54:56.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/deepcache.py
--rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/dotdict.py
--rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/lightning.py
--rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/logger.py
--rw-r--r--   0 basri      (501) staff       (20)     2773 2024-04-30 13:54:27.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/lora.py
--rw-r--r--   0 basri      (501) staff       (20)     1551 2024-04-30 13:42:41.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/optimizations.py
--rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/safety_checker.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:57:33.408932 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/
--rw-r--r--   0 basri      (501) staff       (20)      307 2024-05-08 06:57:03.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      740 2024-04-30 13:29:32.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/controlnet_config.py
--rw-r--r--   0 basri      (501) staff       (20)       70 2024-04-30 13:32:07.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/globals.py
--rw-r--r--   0 basri      (501) staff       (20)     1139 2024-04-30 13:30:09.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/lora_config.py
--rw-r--r--   0 basri      (501) staff       (20)     2007 2024-05-08 06:53:26.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/model_config.py
--rw-r--r--   0 basri      (501) staff       (20)      399 2024-05-08 06:53:26.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/scheduler_config.py
--rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/sdk_config.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:57:33.410839 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/
--rw-r--r--   0 basri      (501) staff       (20)      257 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      112 2024-05-06 11:32:54.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/controlnet_type.py
--rw-r--r--   0 basri      (501) staff       (20)     1032 2024-05-06 11:32:51.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/controlnets.py
--rw-r--r--   0 basri      (501) staff       (20)      837 2024-05-06 11:31:51.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/pipeline_type.py
--rw-r--r--   0 basri      (501) staff       (20)     4336 2024-05-06 11:33:02.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/pipelines.py
--rw-r--r--   0 basri      (501) staff       (20)      815 2024-05-06 11:33:06.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/scheduler_type.py
--rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/schedulers.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 06:57:33.404789 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-05-08 06:57:33.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)     1228 2024-05-08 06:57:33.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2024-05-08 06:57:33.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       18 2024-05-08 06:57:33.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk.egg-info/requires.txt
--rw-r--r--   0 basri      (501) staff       (20)       21 2024-05-08 06:57:33.000000 wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 08:54:39.564473 wonder-diffusion-sdk-0.0.6.dev5/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.6.dev5/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      190 2024-05-08 08:54:39.564324 wonder-diffusion-sdk-0.0.6.dev5/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2024-05-08 08:54:39.564541 wonder-diffusion-sdk-0.0.6.dev5/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      319 2024-05-08 08:54:32.000000 wonder-diffusion-sdk-0.0.6.dev5/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 08:54:39.555428 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)     8223 2024-05-08 08:54:25.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/__init__.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 08:54:39.559286 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/
+-rw-r--r--   0 basri      (501) staff       (20)      344 2024-04-30 13:54:56.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/deepcache.py
+-rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/dotdict.py
+-rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/lightning.py
+-rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/logger.py
+-rw-r--r--   0 basri      (501) staff       (20)     2773 2024-04-30 13:54:27.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/lora.py
+-rw-r--r--   0 basri      (501) staff       (20)     1551 2024-04-30 13:42:41.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/optimizations.py
+-rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/safety_checker.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 08:54:39.561836 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/
+-rw-r--r--   0 basri      (501) staff       (20)      307 2024-05-08 06:57:03.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      740 2024-04-30 13:29:32.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/controlnet_config.py
+-rw-r--r--   0 basri      (501) staff       (20)       70 2024-04-30 13:32:07.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/globals.py
+-rw-r--r--   0 basri      (501) staff       (20)     1139 2024-04-30 13:30:09.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/lora_config.py
+-rw-r--r--   0 basri      (501) staff       (20)     2007 2024-05-08 06:53:26.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/model_config.py
+-rw-r--r--   0 basri      (501) staff       (20)      399 2024-05-08 06:53:26.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/scheduler_config.py
+-rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/sdk_config.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 08:54:39.563732 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/
+-rw-r--r--   0 basri      (501) staff       (20)      257 2024-04-30 13:01:39.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      112 2024-05-06 11:32:54.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/controlnet_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     1032 2024-05-06 11:32:51.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/controlnets.py
+-rw-r--r--   0 basri      (501) staff       (20)      837 2024-05-06 11:31:51.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/pipeline_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     4336 2024-05-06 11:33:02.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/pipelines.py
+-rw-r--r--   0 basri      (501) staff       (20)      815 2024-05-06 11:33:06.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/scheduler_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/schedulers.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-05-08 08:54:39.556520 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      190 2024-05-08 08:54:39.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)     1228 2024-05-08 08:54:39.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2024-05-08 08:54:39.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       18 2024-05-08 08:54:39.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk.egg-info/requires.txt
+-rw-r--r--   0 basri      (501) staff       (20)       21 2024-05-08 08:54:39.000000 wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk.egg-info/top_level.txt
```

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/LICENCE` & `wonder-diffusion-sdk-0.0.6.dev5/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/__init__.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,19 +154,21 @@
         elif hasattr(self, 'pipeline'):
             _pipeline = self.pipeline
 
         if _pipeline != None and scheduler in SCHEDULER_MAP:
             _pipeline.scheduler = SCHEDULER_MAP[scheduler](
                 _pipeline.scheduler.config)
 
-    def run(self, args: dict):
+    def run(self, args: dict, return_images=True):
         args['generator'], seed = self.generate_seed(args.get('seed', None))
         self.logger.info(f'DIFFUSION SDK LOG: Seed {seed}')
-
-        return self.pipeline(**args).images, seed
+        if return_images:
+            return self.pipeline(**args).images, seed
+        else:
+            return self.pipeline(**args), seed
 
     def generate_seed(self, seed=None):
         if seed == None or seed < 0:
             seed = randint(0, 2**32-1)
         return torch.Generator(device=DEVICE).manual_seed(seed), seed
 
     # Safety checker
```

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/lightning.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/lightning.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/logger.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/logger.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/lora.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/lora.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/optimizations.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/optimizations.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/components/safety_checker.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/components/safety_checker.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/controlnet_config.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/controlnet_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/lora_config.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/lora_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/config/model_config.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/config/model_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/controlnets.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/controlnets.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/pipeline_type.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/pipeline_type.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/pipelines.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/pipelines.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/scheduler_type.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/scheduler_type.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk/types/schedulers.py` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk/types/schedulers.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.6.dev4/wonder_diffusion_sdk.egg-info/SOURCES.txt` & `wonder-diffusion-sdk-0.0.6.dev5/wonder_diffusion_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


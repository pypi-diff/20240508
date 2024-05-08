# Comparing `tmp/objathor-0.0.4.tar.gz` & `tmp/objathor-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objathor-0.0.4.tar", last modified: Sat Apr  6 22:12:25 2024, max compression
+gzip compressed data, was "objathor-0.0.5.tar", last modified: Wed May  8 21:59:37 2024, max compression
```

## Comparing `objathor-0.0.4.tar` & `objathor-0.0.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.706651 objathor-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 22:12:16.000000 objathor-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-06 22:12:25.706651 objathor-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-06 22:12:16.000000 objathor-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.698651 objathor-0.0.4/objathor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/annotation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/embed_synset_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/gpt_from_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/objaverse_annotations_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/annotation/synset_from_description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor/asset_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/asset_conversion_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor/asset_conversion/colliders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/colliders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/colliders/decompose_convex_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/colliders/generate_colliders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/convert_obj_to_glb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor/asset_conversion/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/data/empty_house.json
--rw-r--r--   0 runner    (1001) docker     (127)    64921 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/object_consolidater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/object_consolidater_blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/object_consolidater_blender_package.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31364 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/pipeline_to_thor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/asset_conversion/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.706651 objathor-0.0.4/objathor/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/aggregate_asset_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/download_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/download_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/download_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/download_holodeck_base_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/generate_holodeck_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/postprocess_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/upgrade_2023_holodeck_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/dataset/upload_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.706651 objathor-0.0.4/objathor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.706651 objathor-0.0.4/objathor/utils/blender/
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/blender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/blender/render_glb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/gpt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-06 22:12:16.000000 objathor-0.0.4/objathor/utils/synsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:25.702651 objathor-0.0.4/objathor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 22:12:25.000000 objathor-0.0.4/objathor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 22:12:25.706651 objathor-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-06 22:12:16.000000 objathor-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.920493 objathor-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 21:59:28.000000 objathor-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-08 21:59:37.920493 objathor-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-08 21:59:28.000000 objathor-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.912494 objathor-0.0.5/objathor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.912494 objathor-0.0.5/objathor/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/annotation/annotation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/annotation/embed_synset_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11873 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/annotation/gpt_from_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/annotation/objaverse_annotations_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/annotation/synset_from_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.916494 objathor-0.0.5/objathor/asset_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/asset_conversion_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.916494 objathor-0.0.5/objathor/asset_conversion/colliders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/colliders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/colliders/decompose_convex_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/colliders/generate_colliders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/convert_obj_to_glb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.916494 objathor-0.0.5/objathor/asset_conversion/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/data/empty_house.json
+-rw-r--r--   0 runner    (1001) docker     (127)    64921 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/object_consolidater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/object_consolidater_blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/object_consolidater_blender_package.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31364 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/pipeline_to_thor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22629 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/asset_conversion/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.916494 objathor-0.0.5/objathor/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/aggregate_asset_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/download_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/download_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/download_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/download_holodeck_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/generate_holodeck_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/postprocess_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/upgrade_2023_holodeck_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/dataset/upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.916494 objathor-0.0.5/objathor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.916494 objathor-0.0.5/objathor/utils/blender/
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/utils/blender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/utils/blender/render_glb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/utils/download_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/utils/gpt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/utils/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 21:59:28.000000 objathor-0.0.5/objathor/utils/synsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:59:37.912494 objathor-0.0.5/objathor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-08 21:59:37.000000 objathor-0.0.5/objathor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-08 21:59:37.000000 objathor-0.0.5/objathor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 21:59:37.000000 objathor-0.0.5/objathor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-08 21:59:37.000000 objathor-0.0.5/objathor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 21:59:37.000000 objathor-0.0.5/objathor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 21:59:37.920493 objathor-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-08 21:59:28.000000 objathor-0.0.5/setup.py
```

### Comparing `objathor-0.0.4/LICENSE` & `objathor-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/PKG-INFO` & `objathor-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objathor
-Version: 0.0.4
+Version: 0.0.5
 Summary: Objaverse asset importer for THOR
 Home-page: https://github.com/allenai/objathor
 Author: Allen Institute for AI
 Author-email: contact@allenai.org
 License: Apache 2.0
 Keywords: 3D assets,annotation,
 Classifier: Development Status :: 4 - Beta
```

### Comparing `objathor-0.0.4/README.md` & `objathor-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/annotation/annotation_utils.py` & `objathor-0.0.5/objathor/annotation/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/annotation/embed_synset_definitions.py` & `objathor-0.0.5/objathor/annotation/embed_synset_definitions.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/annotation/gpt_from_views.py` & `objathor-0.0.5/objathor/annotation/gpt_from_views.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/annotation/objaverse_annotations_utils.py` & `objathor-0.0.5/objathor/annotation/objaverse_annotations_utils.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/annotation/synset_from_description.py` & `objathor-0.0.5/objathor/annotation/synset_from_description.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/asset_conversion/colliders/decompose_convex_obj.py` & `objathor-0.0.5/objathor/asset_conversion/colliders/decompose_convex_obj.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/asset_conversion/colliders/generate_colliders.py` & `objathor-0.0.5/objathor/asset_conversion/colliders/generate_colliders.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/asset_conversion/convert_obj_to_glb.py` & `objathor-0.0.5/objathor/asset_conversion/convert_obj_to_glb.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/asset_conversion/data/empty_house.json` & `objathor-0.0.5/objathor/asset_conversion/data/empty_house.json`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/asset_conversion/object_consolidater.py` & `objathor-0.0.5/objathor/asset_conversion/object_consolidater.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/asset_conversion/object_consolidater_blender.py` & `objathor-0.0.5/objathor/asset_conversion/object_consolidater_blender.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/asset_conversion/object_consolidater_blender_package.py` & `objathor-0.0.5/objathor/asset_conversion/object_consolidater_blender_package.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/asset_conversion/pipeline_to_thor.py` & `objathor-0.0.5/objathor/asset_conversion/pipeline_to_thor.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/asset_conversion/util.py` & `objathor-0.0.5/objathor/asset_conversion/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,16 @@
             if os.path.realpath(build_target_dir) != os.path.realpath(asset_directory):
                 os.remove(build_target_dir)
 
         if (not os.path.exists(build_target_dir)) and (
             not os.path.islink(build_target_dir)
         ):
             # Add symlink if it doesn't already exist
-            print(f"Symlink from {asset_directory} to {build_target_dir}")
+            if verbose:
+                logger.info(f"Symlink from {asset_directory} to {build_target_dir}")
             os.symlink(
                 os.path.abspath(asset_directory), os.path.abspath(build_target_dir)
             )
 
         if not load_file_in_unity:
             return load_existing_thor_asset_file(
                 out_dir=build_target_dir, object_name=asset_id
```

### Comparing `objathor-0.0.4/objathor/dataset/__init__.py` & `objathor-0.0.5/objathor/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/dataset/aggregate_asset_annotations.py` & `objathor-0.0.5/objathor/dataset/aggregate_asset_annotations.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/dataset/download_annotations.py` & `objathor-0.0.5/objathor/dataset/download_annotations.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/dataset/example.py` & `objathor-0.0.5/objathor/dataset/example.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/dataset/generate_holodeck_features.py` & `objathor-0.0.5/objathor/dataset/generate_holodeck_features.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/dataset/postprocess_assets.py` & `objathor-0.0.5/objathor/dataset/postprocess_assets.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/dataset/upgrade_2023_holodeck_databases.py` & `objathor-0.0.5/objathor/dataset/upgrade_2023_holodeck_databases.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/dataset/upload_dataset.py` & `objathor-0.0.5/objathor/dataset/upload_dataset.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/main.py` & `objathor-0.0.5/objathor/main.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/utils/blender/__init__.py` & `objathor-0.0.5/objathor/utils/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/utils/blender/render_glb.py` & `objathor-0.0.5/objathor/utils/blender/render_glb.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/utils/download_utils.py` & `objathor-0.0.5/objathor/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/utils/gpt_utils.py` & `objathor-0.0.5/objathor/utils/gpt_utils.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/utils/queries.py` & `objathor-0.0.5/objathor/utils/queries.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor/utils/synsets.py` & `objathor-0.0.5/objathor/utils/synsets.py`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/objathor.egg-info/PKG-INFO` & `objathor-0.0.5/objathor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objathor
-Version: 0.0.4
+Version: 0.0.5
 Summary: Objaverse asset importer for THOR
 Home-page: https://github.com/allenai/objathor
 Author: Allen Institute for AI
 Author-email: contact@allenai.org
 License: Apache 2.0
 Keywords: 3D assets,annotation,
 Classifier: Development Status :: 4 - Beta
```

### Comparing `objathor-0.0.4/objathor.egg-info/SOURCES.txt` & `objathor-0.0.5/objathor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `objathor-0.0.4/setup.py` & `objathor-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     REQUIREMENTS = _read_reqs("requirements.txt")
     REQUIREMENTS_ANNOTATION = _read_reqs("requirements-annotation.txt")
 
     setup(
         name="objathor",
         packages=find_packages(),
         include_package_data=True,
-        version="0.0.4",
+        version="0.0.5",
         license="Apache 2.0",
         description="Objaverse asset importer for THOR",
         long_description=long_description,
         long_description_content_type="text/markdown",
         author="Allen Institute for AI",
         author_email="contact@allenai.org",
         url="https://github.com/allenai/objathor",
```


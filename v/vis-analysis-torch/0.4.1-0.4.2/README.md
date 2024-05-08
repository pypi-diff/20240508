# Comparing `tmp/vis_analysis_torch-0.4.1.tar.gz` & `tmp/vis_analysis_torch-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vis_analysis_torch-0.4.1.tar", last modified: Wed May  8 08:11:57 2024, max compression
+gzip compressed data, was "vis_analysis_torch-0.4.2.tar", last modified: Wed May  8 08:15:55 2024, max compression
```

## Comparing `vis_analysis_torch-0.4.1.tar` & `vis_analysis_torch-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/setup.cfg
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      498 2024-05-08 08:11:54.000000 vis_analysis_torch-0.4.1/setup.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/vis_analysis_torch/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/__init__.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     3338 2024-05-08 08:11:41.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/bbox_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 02:55:56.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/common_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     7369 2024-05-08 08:11:50.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/pose_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     2776 2024-05-08 07:55:53.000000 vis_analysis_torch-0.4.1/vis_analysis_torch/utils.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:11:57.948718 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      401 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/SOURCES.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/dependency_links.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/requires.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-08 08:11:57.000000 vis_analysis_torch-0.4.1/vis_analysis_torch.egg-info/top_level.txt
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:15:55.685692 vis_analysis_torch-0.4.2/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 08:15:55.685692 vis_analysis_torch-0.4.2/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-08 08:15:55.685692 vis_analysis_torch-0.4.2/setup.cfg
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      498 2024-05-08 08:15:52.000000 vis_analysis_torch-0.4.2/setup.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:15:55.685692 vis_analysis_torch-0.4.2/vis_analysis_torch/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.4.2/vis_analysis_torch/__init__.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     3338 2024-05-08 08:11:41.000000 vis_analysis_torch-0.4.2/vis_analysis_torch/bbox_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     1569 2024-05-08 08:15:40.000000 vis_analysis_torch-0.4.2/vis_analysis_torch/common_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     7369 2024-05-08 08:11:50.000000 vis_analysis_torch-0.4.2/vis_analysis_torch/pose_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     2776 2024-05-08 07:55:53.000000 vis_analysis_torch-0.4.2/vis_analysis_torch/utils.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:15:55.685692 vis_analysis_torch-0.4.2/vis_analysis_torch.egg-info/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 08:15:55.000000 vis_analysis_torch-0.4.2/vis_analysis_torch.egg-info/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      401 2024-05-08 08:15:55.000000 vis_analysis_torch-0.4.2/vis_analysis_torch.egg-info/SOURCES.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-08 08:15:55.000000 vis_analysis_torch-0.4.2/vis_analysis_torch.egg-info/dependency_links.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-08 08:15:55.000000 vis_analysis_torch-0.4.2/vis_analysis_torch.egg-info/requires.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-08 08:15:55.000000 vis_analysis_torch-0.4.2/vis_analysis_torch.egg-info/top_level.txt
```

### Comparing `vis_analysis_torch-0.4.1/vis_analysis_torch/bbox_visualization.py` & `vis_analysis_torch-0.4.2/vis_analysis_torch/bbox_visualization.py`

 * *Files identical despite different names*

### Comparing `vis_analysis_torch-0.4.1/vis_analysis_torch/pose_visualization.py` & `vis_analysis_torch-0.4.2/vis_analysis_torch/pose_visualization.py`

 * *Files identical despite different names*

### Comparing `vis_analysis_torch-0.4.1/vis_analysis_torch/utils.py` & `vis_analysis_torch-0.4.2/vis_analysis_torch/utils.py`

 * *Files identical despite different names*


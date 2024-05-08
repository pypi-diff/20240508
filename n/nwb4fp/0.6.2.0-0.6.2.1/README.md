# Comparing `tmp/nwb4fp-0.6.2.0.tar.gz` & `tmp/nwb4fp-0.6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.2.0.tar", last modified: Wed May  8 17:51:10 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.2.1.tar", last modified: Wed May  8 18:43:05 2024, max compression
```

## Comparing `nwb4fp-0.6.2.0.tar` & `nwb4fp-0.6.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 17:51:10.652887 nwb4fp-0.6.2.0/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.2.0/LICENSE
--rw-rw-rw-   0        0        0     5746 2024-05-08 17:51:10.645889 nwb4fp-0.6.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 17:51:10.665884 nwb4fp-0.6.2.0/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-05-08 17:51:04.000000 nwb4fp-0.6.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:51:09.837886 nwb4fp-0.6.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 17:51:09.960886 nwb4fp-0.6.2.0/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.2.0/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:51:10.088886 nwb4fp-0.6.2.0/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.2.0/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.2.0/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:51:10.264886 nwb4fp-0.6.2.0/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.2.0/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.2.0/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1850 2024-05-06 11:49:17.000000 nwb4fp-0.6.2.0/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.2.0/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.2.0/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.2.0/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.2.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    14405 2024-05-08 17:50:56.000000 nwb4fp-0.6.2.0/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:51:09.851886 nwb4fp-0.6.2.0/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.0/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.0/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.0/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8242 2024-05-06 12:27:58.000000 nwb4fp-0.6.2.0/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.0/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.0/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.0/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.0/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:51:09.859887 nwb4fp-0.6.2.0/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-05-08 17:51:09.859887 nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-05-08 11:40:42.000000 nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1466 2024-05-08 11:41:48.000000 nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0     1448 2024-05-07 08:56:13.000000 nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/readnwb_09PD.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:51:10.063898 nwb4fp-0.6.2.0/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5746 2024-05-08 17:51:09.000000 nwb4fp-0.6.2.0/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-05-08 17:51:09.000000 nwb4fp-0.6.2.0/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 17:51:09.000000 nwb4fp-0.6.2.0/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2892 2024-05-08 17:51:09.000000 nwb4fp-0.6.2.0/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 17:51:09.000000 nwb4fp-0.6.2.0/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 18:43:05.783665 nwb4fp-0.6.2.1/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5746 2024-05-08 18:43:05.773664 nwb4fp-0.6.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 18:43:05.810662 nwb4fp-0.6.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-05-08 18:43:00.000000 nwb4fp-0.6.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:43:04.949665 nwb4fp-0.6.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 18:43:05.062666 nwb4fp-0.6.2.1/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.2.1/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:43:05.145664 nwb4fp-0.6.2.1/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.2.1/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.2.1/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:43:05.282666 nwb4fp-0.6.2.1/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.2.1/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.2.1/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1850 2024-05-06 11:49:17.000000 nwb4fp-0.6.2.1/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.2.1/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.2.1/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.2.1/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.2.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    14407 2024-05-08 18:42:49.000000 nwb4fp-0.6.2.1/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:43:04.967670 nwb4fp-0.6.2.1/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.1/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.1/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.1/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8242 2024-05-06 12:27:58.000000 nwb4fp-0.6.2.1/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.1/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.1/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.1/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.1/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:43:04.978665 nwb4fp-0.6.2.1/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-08 18:43:04.978665 nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-05-08 11:40:42.000000 nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1466 2024-05-08 11:41:48.000000 nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0     1448 2024-05-07 08:56:13.000000 nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/readnwb_09PD.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:43:05.124665 nwb4fp-0.6.2.1/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5746 2024-05-08 18:43:04.000000 nwb4fp-0.6.2.1/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-05-08 18:43:04.000000 nwb4fp-0.6.2.1/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 18:43:04.000000 nwb4fp-0.6.2.1/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2892 2024-05-08 18:43:04.000000 nwb4fp-0.6.2.1/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 18:43:04.000000 nwb4fp-0.6.2.1/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.2.0/LICENSE` & `nwb4fp-0.6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/PKG-INFO` & `nwb4fp-0.6.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.2.0
+Version: 0.6.2.1
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.2.0/README.md` & `nwb4fp-0.6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/setup.py` & `nwb4fp-0.6.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.2.0',
+    version='0.6.2.1',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.2.1/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.2.1/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.2.1/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.2.1/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.2.1/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.2.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.2.1/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,25 +224,25 @@
     qm_ext = analyzer1.compute(input={"principal_components": dict(n_components=5, mode="by_channel_local"),
                                 "quality_metrics": dict(skip_pc_metrics=False)})
     qm_data = analyzer1.get_extension("quality_metrics").get_data()
 
     keep_mask = (qm_data["presence_ratio"] > 0.9) & (qm_data["isi_violations_ratio"] < 0.2) & (qm_data["l_ratio"] < 0.1)
     q = sort_merge.get_property('quality')
     q[keep_mask] = 'good'
-    sort_merge.set_property(key='quality', values = q)
+    sort_merge1.set_property(key='quality', values = q)
 
-    analyzer1 = si.create_sorting_analyzer(sorting=sort_merge, recording=rec_w, format='binary_folder', folder=fr"{temp_folder}_output",overwrite=True)
-    we1 = analyzer1.compute("random_spikes","waveforms")
-    we1 = analyzer1.compute("waveforms")
-    we1 = analyzer1.compute("noise_levels")
-    we1 = analyzer1.compute("templates")
-    qm = analyzer1.compute("quality_metrics")
-    sim = analyzer1.compute("template_similarity", method="cosine_similarity")
-    unit_locations = analyzer1.compute(input="unit_locations", method="monopolar_triangulation")
-    qm_ext = analyzer1.compute(input={"principal_components": dict(n_components=5, mode="by_channel_local"),
+    analyzer2 = si.create_sorting_analyzer(sorting=sort_merge1, recording=rec_w, format='binary_folder', folder=fr"{temp_folder}_output",overwrite=True)
+    we1 = analyzer2.compute("random_spikes","waveforms")
+    we1 = analyzer2.compute("waveforms")
+    we1 = analyzer2.compute("noise_levels")
+    we1 = analyzer2.compute("templates")
+    qm = analyzer2.compute("quality_metrics")
+    sim = analyzer2.compute("template_similarity", method="cosine_similarity")
+    unit_locations = analyzer2.compute(input="unit_locations", method="monopolar_triangulation")
+    qm_ext = analyzer2.compute(input={"principal_components": dict(n_components=5, mode="by_channel_local"),
                                 "quality_metrics": dict(skip_pc_metrics=False)})
 
 
     # print(sort_merge.get_property_keys())
     # print(f"get times for merge sorts{sort_merge.get_times()}")
     # wfm = si.extract_waveforms(rec_save, sort_merge, folder=fr"{temp_folder}", overwrite=True, 
     #                           sparse=True, method="by_property",by_property="group",max_spikes_per_unit=None)
```

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.2.1/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.2.1/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.2.1/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.2.1/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/readnwb_09PD.py` & `nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/readnwb_09PD.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.2.1/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.2.1/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.2.0
+Version: 0.6.2.1
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.2.1/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.0/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.2.1/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*


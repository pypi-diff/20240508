# Comparing `tmp/nwb4fp-0.6.1.6.tar.gz` & `tmp/nwb4fp-0.6.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.1.6.tar", last modified: Wed May  8 16:32:20 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.1.7.tar", last modified: Wed May  8 16:41:43 2024, max compression
```

## Comparing `nwb4fp-0.6.1.6.tar` & `nwb4fp-0.6.1.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 16:32:21.141252 nwb4fp-0.6.1.6/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.1.6/LICENSE
--rw-rw-rw-   0        0        0     5746 2024-05-08 16:32:21.135243 nwb4fp-0.6.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 16:32:21.160249 nwb4fp-0.6.1.6/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-05-08 16:30:21.000000 nwb4fp-0.6.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:32:20.439245 nwb4fp-0.6.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 16:32:20.558252 nwb4fp-0.6.1.6/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.1.6/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:32:20.653257 nwb4fp-0.6.1.6/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.1.6/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.1.6/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:32:20.835244 nwb4fp-0.6.1.6/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.1.6/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.1.6/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1850 2024-05-06 11:49:17.000000 nwb4fp-0.6.1.6/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.1.6/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.1.6/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.1.6/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.1.6/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    13566 2024-05-08 16:31:49.000000 nwb4fp-0.6.1.6/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:32:20.989246 nwb4fp-0.6.1.6/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.6/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.6/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.6/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8242 2024-05-06 12:27:58.000000 nwb4fp-0.6.1.6/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.6/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.6/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.6/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.6/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:32:20.465263 nwb4fp-0.6.1.6/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-05-08 16:32:21.096254 nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-05-08 11:40:42.000000 nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1466 2024-05-08 11:41:48.000000 nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0     1448 2024-05-07 08:56:13.000000 nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/readnwb_09PD.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-05-08 16:32:20.630319 nwb4fp-0.6.1.6/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5746 2024-05-08 16:32:20.000000 nwb4fp-0.6.1.6/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-05-08 16:32:20.000000 nwb4fp-0.6.1.6/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 16:32:20.000000 nwb4fp-0.6.1.6/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2892 2024-05-08 16:32:20.000000 nwb4fp-0.6.1.6/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 16:32:20.000000 nwb4fp-0.6.1.6/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 16:41:43.531188 nwb4fp-0.6.1.7/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.1.7/LICENSE
+-rw-rw-rw-   0        0        0     5746 2024-05-08 16:41:43.500186 nwb4fp-0.6.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 16:41:43.555192 nwb4fp-0.6.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-05-08 16:41:00.000000 nwb4fp-0.6.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:41:42.413188 nwb4fp-0.6.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 16:41:42.556187 nwb4fp-0.6.1.7/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.1.7/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:41:42.701187 nwb4fp-0.6.1.7/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.1.7/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.1.7/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:41:42.422188 nwb4fp-0.6.1.7/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.1.7/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.1.7/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1850 2024-05-06 11:49:17.000000 nwb4fp-0.6.1.7/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.1.7/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.1.7/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.1.7/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.1.7/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    13985 2024-05-08 16:40:55.000000 nwb4fp-0.6.1.7/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:41:43.241188 nwb4fp-0.6.1.7/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.7/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.7/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.7/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8242 2024-05-06 12:27:58.000000 nwb4fp-0.6.1.7/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.7/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.7/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.7/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.1.7/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:41:42.443193 nwb4fp-0.6.1.7/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-08 16:41:42.443193 nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-05-08 11:40:42.000000 nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1466 2024-05-08 11:41:48.000000 nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0     1448 2024-05-07 08:56:13.000000 nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/readnwb_09PD.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:41:42.413188 nwb4fp-0.6.1.7/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5746 2024-05-08 16:41:42.000000 nwb4fp-0.6.1.7/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-05-08 16:41:42.000000 nwb4fp-0.6.1.7/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 16:41:42.000000 nwb4fp-0.6.1.7/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2892 2024-05-08 16:41:42.000000 nwb4fp-0.6.1.7/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-08 16:41:42.000000 nwb4fp-0.6.1.7/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.1.6/LICENSE` & `nwb4fp-0.6.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/PKG-INFO` & `nwb4fp-0.6.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.1.6
+Version: 0.6.1.7
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.1.6/README.md` & `nwb4fp-0.6.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/setup.py` & `nwb4fp-0.6.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.1.6',
+    version='0.6.1.7',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.1.7/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.1.7/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.1.7/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.1.7/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.1.7/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.1.7/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.1.7/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,23 @@
     qm_ext = analyzer1.compute(input={"principal_components": dict(n_components=5, mode="by_channel_local"),
                                 "quality_metrics": dict(skip_pc_metrics=False)})
     
     keep_mask = (qm["presence_ratio"] > 0.9) & (qm["isi_violations_ratio"] < 0.2) & (qm_ext["l_ratio"] < 0.1)
     q = sort_merge.get_property('quality')
     q[keep_mask] = 'good'
     sort_merge.set_property(key='quality', values = q)
+
+    analyzer = si.create_sorting_analyzer(sorting=sorting, recording=rec_w, format='binary_folder', folder=fr"{temp_folder}",overwrite=True)
+    we1 = analyzer.compute("random_spikes","waveforms")
+    we1 = analyzer.compute("waveforms")
+    we1 = analyzer.compute("noise_levels")
+    we1 = analyzer.compute("templates")
+    #get potential merging sorting objects
+    print("processing potential merge...\n")
+
     # print(sort_merge.get_property_keys())
     # print(f"get times for merge sorts{sort_merge.get_times()}")
     # wfm = si.extract_waveforms(rec_save, sort_merge, folder=fr"{temp_folder}", overwrite=True, 
     #                           sparse=True, method="by_property",by_property="group",max_spikes_per_unit=None)
     # post.compute_unit_locations(waveform_extractor=wfm,
     #                             method= 'monopolar_triangulation',
     #                             radius_um=50.)
```

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.1.7/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.1.7/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.1.7/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.1.7/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/readnwb_09PD.py` & `nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/readnwb_09PD.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.1.7/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.1.7/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.1.6
+Version: 0.6.1.7
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.1.7/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.1.6/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.1.7/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*


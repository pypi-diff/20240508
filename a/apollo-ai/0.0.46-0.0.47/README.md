# Comparing `tmp/apollo-ai-0.0.46.tar.gz` & `tmp/apollo-ai-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-ai-0.0.46.tar", last modified: Mon May  6 16:02:30 2024, max compression
+gzip compressed data, was "apollo-ai-0.0.47.tar", last modified: Wed May  8 03:40:18 2024, max compression
```

## Comparing `apollo-ai-0.0.46.tar` & `apollo-ai-0.0.47.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 16:02:30.476616 apollo-ai-0.0.46/
--rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.46/LICENSE
--rw-rw-rw-   0        0        0     9511 2024-05-06 16:02:30.475617 apollo-ai-0.0.46/PKG-INFO
--rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.46/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 16:02:30.428619 apollo-ai-0.0.46/apollo/
-drwxrwxrwx   0        0        0        0 2024-05-06 16:02:30.442610 apollo-ai-0.0.46/apollo/apollo_ai.egg-info/
--rw-rw-rw-   0        0        0     9511 2024-05-06 16:02:30.000000 apollo-ai-0.0.46/apollo/apollo_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-05-06 16:02:30.000000 apollo-ai-0.0.46/apollo/apollo_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 16:02:30.000000 apollo-ai-0.0.46/apollo/apollo_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      596 2024-05-06 16:02:30.000000 apollo-ai-0.0.46/apollo/apollo_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 16:02:30.000000 apollo-ai-0.0.46/apollo/apollo_ai.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 16:02:30.451606 apollo-ai-0.0.46/apollo/argus/
--rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.46/apollo/argus/__init__.py
--rw-rw-rw-   0        0        0    12355 2024-05-06 16:01:37.000000 apollo-ai-0.0.46/apollo/argus/argus.py
--rw-rw-rw-   0        0        0     6864 2024-05-06 03:28:49.000000 apollo-ai-0.0.46/apollo/argus/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:02:30.456606 apollo-ai-0.0.46/apollo/lyre/
--rw-rw-rw-   0        0        0      149 2024-05-06 03:28:49.000000 apollo-ai-0.0.46/apollo/lyre/__init__.py
--rw-rw-rw-   0        0        0     9151 2024-05-06 03:28:49.000000 apollo-ai-0.0.46/apollo/lyre/lyre.py
--rw-rw-rw-   0        0        0     3140 2024-05-06 03:28:49.000000 apollo-ai-0.0.46/apollo/lyre/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 16:02:30.473607 apollo-ai-0.0.46/apollo/pythia/
--rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.46/apollo/pythia/__init__.py
--rw-rw-rw-   0        0        0    10013 2024-05-02 14:32:40.000000 apollo-ai-0.0.46/apollo/pythia/pythia.py
--rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.46/apollo/pythia/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-06 16:02:30.476616 apollo-ai-0.0.46/setup.cfg
--rw-rw-rw-   0        0        0     1821 2024-05-06 16:02:23.000000 apollo-ai-0.0.46/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.173225 apollo-ai-0.0.47/
+-rw-rw-rw-   0        0        0    35823 2023-09-19 22:57:32.000000 apollo-ai-0.0.47/LICENSE
+-rw-rw-rw-   0        0        0     9511 2024-05-08 03:40:18.171709 apollo-ai-0.0.47/PKG-INFO
+-rw-rw-rw-   0        0        0     8994 2023-11-08 20:42:11.000000 apollo-ai-0.0.47/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.067527 apollo-ai-0.0.47/apollo/
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.093175 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/
+-rw-rw-rw-   0        0        0     9511 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      596 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 03:40:17.000000 apollo-ai-0.0.47/apollo/apollo_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.106299 apollo-ai-0.0.47/apollo/argus/
+-rw-rw-rw-   0        0        0       65 2024-05-02 14:32:40.000000 apollo-ai-0.0.47/apollo/argus/__init__.py
+-rw-rw-rw-   0        0        0    12485 2024-05-08 03:26:33.000000 apollo-ai-0.0.47/apollo/argus/argus.py
+-rw-rw-rw-   0        0        0     6864 2024-05-08 03:20:05.000000 apollo-ai-0.0.47/apollo/argus/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.118837 apollo-ai-0.0.47/apollo/lyre/
+-rw-rw-rw-   0        0        0      149 2024-05-06 03:28:49.000000 apollo-ai-0.0.47/apollo/lyre/__init__.py
+-rw-rw-rw-   0        0        0     9151 2024-05-06 03:28:49.000000 apollo-ai-0.0.47/apollo/lyre/lyre.py
+-rw-rw-rw-   0        0        0     3140 2024-05-06 03:28:49.000000 apollo-ai-0.0.47/apollo/lyre/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:40:18.132404 apollo-ai-0.0.47/apollo/pythia/
+-rw-rw-rw-   0        0        0      201 2024-05-02 14:32:40.000000 apollo-ai-0.0.47/apollo/pythia/__init__.py
+-rw-rw-rw-   0        0        0    10013 2024-05-02 14:32:40.000000 apollo-ai-0.0.47/apollo/pythia/pythia.py
+-rw-rw-rw-   0        0        0     4339 2024-05-02 14:32:40.000000 apollo-ai-0.0.47/apollo/pythia/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:40:18.174246 apollo-ai-0.0.47/setup.cfg
+-rw-rw-rw-   0        0        0     1821 2024-05-08 03:28:10.000000 apollo-ai-0.0.47/setup.py
```

### Comparing `apollo-ai-0.0.46/LICENSE` & `apollo-ai-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.46/PKG-INFO` & `apollo-ai-0.0.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.46
+Version: 0.0.47
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.46/README.md` & `apollo-ai-0.0.47/README.md`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.46/apollo/apollo_ai.egg-info/PKG-INFO` & `apollo-ai-0.0.47/apollo/apollo_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apollo-ai
-Version: 0.0.46
+Version: 0.0.47
 Summary: Framework to process 3 channels in one: Video, Audio & Text
 Home-page: https://github.com/VerbaNexAI/APOLLO.AI
 Author: VerbaNex, Riddle
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `apollo-ai-0.0.46/apollo/apollo_ai.egg-info/requires.txt` & `apollo-ai-0.0.47/apollo/apollo_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.46/apollo/argus/argus.py` & `apollo-ai-0.0.47/apollo/argus/argus.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     ensure_dir_created(output_dir)
 
     file_direction = output_dir + "/" + filepath.split("/")[-1].split(".")[0]
 
     distances_data = []
 
     video_source = cv2.VideoCapture(filepath)
-    logging.info("Video found, starting processing...")
     mp_face_dots = mp.solutions.face_mesh
 
     fps_general = int(video_source.get(cv2.CAP_PROP_FPS))
     frame_width = int(video_source.get(cv2.CAP_PROP_FRAME_WIDTH))
     frame_height = int(video_source.get(cv2.CAP_PROP_FRAME_HEIGHT))
     total_frames = int(video_source.get(cv2.CAP_PROP_FRAME_COUNT))
 
@@ -120,14 +119,20 @@
 
         out.write(frame)  # Write the frame to the output video file
         frame_counter += 1
 
     video_source.release()
     cv2.destroyAllWindows()
 
+    if len(distances_data) <= 0:
+        logging.info("Video not found, check directory")
+        return "Video not found"
+
+    logging.info("Video found, starting processing...")
+
     distances_data = filter_video_data(distances_data, normalize)
     x_values = distances_data['Timestamp'].tolist()
     y_values = distances_data['Distance'].tolist()
 
     data = {"x_values": x_values, "y_values": y_values, "fps": fps_general, "min_distance": min_distance,
             "max_distance": max_distance, "frame_width": frame_width, "frame_height": frame_height}
```

### Comparing `apollo-ai-0.0.46/apollo/argus/utils.py` & `apollo-ai-0.0.47/apollo/argus/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         # Calculate the normalization based on min and max values
         if normalize:
             max_value = df['Distance'].max()
             min_value = df['Distance'].min()
             df['Distance'] = (df['Distance'] - min_value) / (max_value - min_value)
 
-        df['Distance'] = signal.savgol_filter(df["Distance"], min(len(df["Distance"]), 51), 3)
+        df['Distance'] = signal.savgol_filter(df["Distance"], min(len(df["Distance"]), 51), 2)
 
         return df
     except Exception as e:
         raise Exception("Error normalizing the data: {0}".format(e))
 
 
 def plot_pose_cube(img, yaw, pitch, roll, tdx=None, tdy=None, size=150.):
```

### Comparing `apollo-ai-0.0.46/apollo/lyre/lyre.py` & `apollo-ai-0.0.47/apollo/lyre/lyre.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.46/apollo/lyre/utils.py` & `apollo-ai-0.0.47/apollo/lyre/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.46/apollo/pythia/pythia.py` & `apollo-ai-0.0.47/apollo/pythia/pythia.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.46/apollo/pythia/utils.py` & `apollo-ai-0.0.47/apollo/pythia/utils.py`

 * *Files identical despite different names*

### Comparing `apollo-ai-0.0.46/setup.py` & `apollo-ai-0.0.47/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="apollo-ai",
-    version="0.0.46",
+    version="0.0.47",
     description="Framework to process 3 channels in one: Video, Audio & Text",
     package_dir={"": "apollo"},
     packages=find_packages(where="apollo"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VerbaNexAI/APOLLO.AI",
     author="VerbaNex, Riddle",
```


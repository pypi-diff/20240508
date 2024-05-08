# Comparing `tmp/cvvideoplayer-0.1.3.tar.gz` & `tmp/cvvideoplayer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvvideoplayer-0.1.3.tar", last modified: Wed Apr 10 15:03:22 2024, max compression
+gzip compressed data, was "cvvideoplayer-0.1.4.tar", last modified: Wed May  8 18:38:28 2024, max compression
```

## Comparing `cvvideoplayer-0.1.3.tar` & `cvvideoplayer-0.1.4.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.404600 cvvideoplayer-0.1.3/
--rw-rw-rw-   0        0        0     1067 2024-03-17 19:44:52.000000 cvvideoplayer-0.1.3/License.txt
--rw-rw-rw-   0        0        0      727 2024-04-10 15:03:22.402371 cvvideoplayer-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4979 2024-04-10 14:54:37.000000 cvvideoplayer-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.350108 cvvideoplayer-0.1.3/cvvideoplayer/
--rw-rw-rw-   0        0        0      202 2024-04-10 14:54:37.000000 cvvideoplayer-0.1.3/cvvideoplayer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.372202 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/
--rw-rw-rw-   0        0        0      303 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/__init__.py
--rw-rw-rw-   0        0        0     4127 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/base_bbox_plotter.py
--rw-rw-rw-   0        0        0     2606 2024-04-02 09:54:25.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/base_frame_editor.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.383983 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/
--rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/__init__.py
--rw-rw-rw-   0        0        0     2373 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py
--rw-rw-rw-   0        0        0     1868 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py
--rw-rw-rw-   0        0        0     1108 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py
--rw-rw-rw-   0        0        0     1387 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/detections_csv_plotter.py
--rw-rw-rw-   0        0        0     3363 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.3/cvvideoplayer/frame_reader.py
--rw-rw-rw-   0        0        0     1404 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.3/cvvideoplayer/recorder.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.397074 cvvideoplayer-0.1.3/cvvideoplayer/utils/
--rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/__init__.py
--rw-rw-rw-   0        0        0      863 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/bbox_utils.py
--rw-rw-rw-   0        0        0     2233 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/drawing_utils.py
--rw-rw-rw-   0        0        0     3277 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/video_player_utils.py
--rw-rw-rw-   0        0        0     3012 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.3/cvvideoplayer/utils/windows_vk_dict.py
--rw-rw-rw-   0        0        0    13039 2024-04-06 17:07:18.000000 cvvideoplayer-0.1.3/cvvideoplayer/video_player.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.361073 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/
--rw-rw-rw-   0        0        0      727 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 15:03:22.000000 cvvideoplayer-0.1.3/cvvideoplayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 15:03:22.404600 cvvideoplayer-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      931 2024-04-10 14:56:05.000000 cvvideoplayer-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:03:22.400279 cvvideoplayer-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-03-18 19:35:21.000000 cvvideoplayer-0.1.3/tests/test_video_player_basic_functionality.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:38:28.917397 cvvideoplayer-0.1.4/
+-rw-rw-rw-   0        0        0     1067 2024-03-17 19:44:52.000000 cvvideoplayer-0.1.4/License.txt
+-rw-rw-rw-   0        0        0      704 2024-05-08 18:38:28.916362 cvvideoplayer-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5670 2024-05-05 18:53:04.000000 cvvideoplayer-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 18:38:28.885563 cvvideoplayer-0.1.4/cvvideoplayer/
+-rw-rw-rw-   0        0        0      228 2024-05-05 18:54:07.000000 cvvideoplayer-0.1.4/cvvideoplayer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:38:28.899566 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/
+-rw-rw-rw-   0        0        0      369 2024-05-06 19:04:41.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/__init__.py
+-rw-rw-rw-   0        0        0     4476 2024-05-06 18:11:40.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/base_bbox_plotter.py
+-rw-rw-rw-   0        0        0     2606 2024-04-02 09:54:25.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/base_frame_editor.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:38:28.907091 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/basic_frame_editors/
+-rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/basic_frame_editors/__init__.py
+-rw-rw-rw-   0        0        0     1856 2024-05-06 18:11:40.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/basic_frame_editors/frame_info_overlay.py
+-rw-rw-rw-   0        0        0     2373 2024-05-06 18:11:40.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py
+-rw-rw-rw-   0        0        0     1189 2024-05-06 19:04:43.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py
+-rw-rw-rw-   0        0        0     1787 2024-05-06 19:04:43.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/basic_frame_editors/key_map_overlay.py
+-rw-rw-rw-   0        0        0     1387 2024-05-06 18:11:40.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/detections_csv_plotter.py
+-rw-rw-rw-   0        0        0     3351 2024-05-06 18:11:40.000000 cvvideoplayer-0.1.4/cvvideoplayer/frame_reader.py
+-rw-rw-rw-   0        0        0     5132 2024-05-06 19:04:43.000000 cvvideoplayer-0.1.4/cvvideoplayer/input_manager.py
+-rw-rw-rw-   0        0        0     1404 2024-04-24 18:58:49.000000 cvvideoplayer-0.1.4/cvvideoplayer/recorder.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:38:28.913856 cvvideoplayer-0.1.4/cvvideoplayer/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.4/cvvideoplayer/utils/__init__.py
+-rw-rw-rw-   0        0        0      863 2024-05-06 18:11:40.000000 cvvideoplayer-0.1.4/cvvideoplayer/utils/bbox_utils.py
+-rw-rw-rw-   0        0        0     3083 2024-05-06 19:04:43.000000 cvvideoplayer-0.1.4/cvvideoplayer/utils/drawing_utils.py
+-rw-rw-rw-   0        0        0     3850 2024-05-06 19:04:43.000000 cvvideoplayer-0.1.4/cvvideoplayer/utils/video_player_utils.py
+-rw-rw-rw-   0        0        0     3012 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.4/cvvideoplayer/utils/windows_vk_dict.py
+-rw-rw-rw-   0        0        0     8483 2024-05-08 18:23:34.000000 cvvideoplayer-0.1.4/cvvideoplayer/video_player.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:38:28.892107 cvvideoplayer-0.1.4/cvvideoplayer.egg-info/
+-rw-rw-rw-   0        0        0      704 2024-05-08 18:38:28.000000 cvvideoplayer-0.1.4/cvvideoplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2024-05-08 18:38:28.000000 cvvideoplayer-0.1.4/cvvideoplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 18:38:28.000000 cvvideoplayer-0.1.4/cvvideoplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-08 18:38:28.000000 cvvideoplayer-0.1.4/cvvideoplayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 18:38:28.000000 cvvideoplayer-0.1.4/cvvideoplayer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 18:38:28.917397 cvvideoplayer-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      912 2024-05-08 18:34:42.000000 cvvideoplayer-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 18:38:28.914876 cvvideoplayer-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-18 19:35:21.000000 cvvideoplayer-0.1.4/tests/test_video_player_basic_functionality.py
```

### Comparing `cvvideoplayer-0.1.3/License.txt` & `cvvideoplayer-0.1.4/License.txt`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.3/PKG-INFO` & `cvvideoplayer-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: cvvideoplayer
-Version: 0.1.3
+Version: 0.1.4
 Summary: moduler multi purpose video player for python
 Author: Daniel Tomer
 Author-email: danieltomer1@gmail.com
 Project-URL: Homepage, https://github.com/danieltomer1/CVVideoPlayer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 License-File: License.txt
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: pynput
-Requires-Dist: decord
 Requires-Dist: python-xlib
 Requires-Dist: matplotlib
 
 CV video player is a Python-based customizable video player that helps computer vision practitioners to develop, analyze and debug their video related algorithms and model.
```

### Comparing `cvvideoplayer-0.1.3/README.md` & `cvvideoplayer-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,40 @@
 <div align="center"><img src="assets/logo.jpeg" width="250"></div>
 
 ## Introduction
 CV video player is a Python-based customizable video player that helps computer vision practitioners
 to develop, analyze, and debug their video-related algorithms and models.
 
+The video player is interactive, operating only with keyboard presses (no UI buttons). The user can register 
+shortcuts using the VideoPlayer class's API.
+
+## See it in action
+<details>
+<summary>Running frame by frame</summary>
+    
+![frame_by_frame](https://github.com/danieltomer1/CVVideoPlayer/assets/163285251/7db8cb8c-0075-416c-9901-aa2f4bb49080)
+</details>
+
+<details>
+<summary>Play/Pause and control play speed and direction</summary>
+    
+![playpause](https://github.com/danieltomer1/CVVideoPlayer/assets/163285251/fcf38b37-ec9c-4250-8c2f-6f123154c1e4)
+</details>
+
+<details>
+<summary>Draw bounding boxes and adjust labels</summary>
+    
+![bboxes](https://github.com/danieltomer1/CVVideoPlayer/assets/163285251/0a6e07de-a015-48b4-b510-2c203e0d69f4)
+</details>
 
 ## Installation
 `pip install cvvideoplayer`
 
 ## Usage
-The player is interactive and operates only with keyboard presses (no buttons). The user can register 
-shortcuts using the VideoPlayer class's API.
+
 
 **Design overview**
 <div align="center"><img src="assets/video_player_design_chart.png" width="500"></div>
 
 The player receives an image from the FrameReader, the frame is then passed to a list of frame editors
 which alter it in any way desirable and return the frame. The frame editors also specify whether 
 to perform the edit after the frame has been resized to fit the screen or before.
@@ -121,19 +141,20 @@
 
 </details>
 
 ## Quick Start
 ```python
 from cvvideoplayer import LocalFrameReader, Recorder, VideoPlayer
 
+VIDEO_OR_FRAME_FOLDER_PATH = <add local path here>
 
 def run_player():
     video_player = VideoPlayer(
         video_name="example_video",
-        frame_reader=LocalFrameReader(source_path="assets/example_video.mp4"),
+        frame_reader=LocalFrameReader(source_path=VIDEO_OR_FRAME_FOLDER_PATH),
         recorder=Recorder(),
         add_basic_frame_editors=True,
     )
 
     with video_player:
         video_player.run()
```

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/base_bbox_plotter.py` & `cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/base_bbox_plotter.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
     @property
     def key_function_to_register(self):
         return [
             KeyFunction(key="d", func=self.enable_disable, description="Show/Hide Detections"),
             KeyFunction(key="l", func=self.toggle_show_above_bbox_label, description="Show/Hide above label"),
             KeyFunction(key="b", func=self.toggle_show_below_bbox_label, description="Show/Hide below label"),
+            KeyFunction(key="ctrl+i", func=lambda: self.change_font_size(0.1), description="increase label size"),
+            KeyFunction(key="ctrl+u", func=lambda: self.change_font_size(-0.1), description="decrease label size"),
         ]
 
     def _edit_frame(self, frame, frame_num):
         for bbox in self.get_bboxes(frame, frame_num):
             draw_rectangle(
                 frame,
                 x=bbox.x1,
@@ -93,7 +95,10 @@
         return frame
 
     def toggle_show_above_bbox_label(self):
         self._show_above_bbox_label = not self._show_above_bbox_label
 
     def toggle_show_below_bbox_label(self):
         self._show_below_bbox_label = not self._show_below_bbox_label
+
+    def change_font_size(self, by: float):
+        self._font_scale = max(0.1, min(5.0, self._font_scale + by))
```

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/base_frame_editor.py` & `cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/base_frame_editor.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py` & `cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py` & `cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/basic_frame_editors/frame_info_overlay.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,58 +2,58 @@
 
 import numpy as np
 
 from ..base_frame_editor import BaseFrameEditor
 from ...utils.video_player_utils import write_text_on_img, KeyFunction
 
 
-class FrameNumPrinter(BaseFrameEditor):
+class FrameInfoOverlay(BaseFrameEditor):
     def __init__(
         self,
         enable_by_default: bool = True,
         video_total_frame_num=None,
         font_scale: float = 2,
         font_thickness: int = 2,
-        bottom_left_coordinate: Tuple[int, int] = (25, 10),
+        top_left_coordinate: Tuple[int, int] = (10, 10),
     ):
         super().__init__(enable_by_default)
         self._video_total_frame_num = video_total_frame_num
         self._font_scale = font_scale
         self._font_thickness = font_thickness
-        self._bl_coordinate = bottom_left_coordinate
+        self._tl_coordinate = top_left_coordinate
         self._orig_res = None
 
     @property
     def key_function_to_register(self):
         return [
-            KeyFunction(key="ctrl+f", func=self.enable_disable, description="Enable/Disable frame number"),
+            KeyFunction(key="ctrl+f", func=self.enable_disable, description="Show/Hide frame info"),
         ]
 
     def setup(self, frame) -> None:
         self._orig_res = frame.shape
 
     def _edit_frame(self, frame: np.ndarray, frame_num: int) -> np.ndarray:
         text = f"{frame_num}"
         if self._video_total_frame_num is not None:
             text += f"/{self._video_total_frame_num - 1}"
 
         line = write_text_on_img(
             frame,
             text,
-            row=self._bl_coordinate[0],
-            col=self._bl_coordinate[1],
+            row=self._tl_coordinate[0],
+            col=self._tl_coordinate[1],
             font_scale=self._font_scale,
             thickness=self._font_thickness,
         )
 
         write_text_on_img(
             frame,
             f"{self._orig_res[1]}x{self._orig_res[0]}",
             row=line,
-            col=self._bl_coordinate[1],
+            col=self._tl_coordinate[1],
             font_scale=self._font_scale / 1.5,
             thickness=self._font_thickness,
         )
         return frame
 
     @property
     def edit_after_resize(self) -> bool:
```

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py` & `cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 class HistogramEqualizer(BaseFrameEditor):
     def __init__(self, enable_by_default: bool = False):
         super().__init__(enable_by_default)
 
     @property
     def key_function_to_register(self):
         return [
-            KeyFunction(key="ctrl+h", func=self.enable_disable, description="Enable/Disable frame number"),
+            KeyFunction(
+                key="ctrl+alt+h",
+                func=self.enable_disable,
+                description="Enable/Disable histogram equalization",
+            ),
         ]
 
     def _edit_frame(self, frame: np.ndarray, frame_num: int) -> np.ndarray:
         if frame.dtype == "uint8":
             norm_factor = 255
         elif frame.dtype == "uint16":
             norm_factor = 65535
```

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/frame_editors/detections_csv_plotter.py` & `cvvideoplayer-0.1.4/cvvideoplayer/frame_editors/detections_csv_plotter.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/frame_reader.py` & `cvvideoplayer-0.1.4/cvvideoplayer/frame_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import random
 from pathlib import Path
 import mimetypes
 from typing import Optional
 
 import cv2
 import numpy as np
-from decord import VideoReader, cpu
 
 RANDOM_STATE = random.Random(42)
 
 
 class FrameReader(abc.ABC):
     """
     The frame reader is used in the video player to fetch frames according to a frame number
@@ -51,27 +50,27 @@
         return len(self._reader)
 
 
 class LocalVideoFileReader(FrameReader):
     def __init__(self, local_video_path: str):
         self._video_path = Path(local_video_path)
         assert self._video_path.is_file()
-        self._video_reader = VideoReader(str(self._video_path), ctx=cpu(0))
+        self._video_reader = cv2.VideoCapture(str(self._video_path))
+        self._total_frames = int(self._video_reader.get(cv2.CAP_PROP_FRAME_COUNT))
 
     def get_frame(self, frame_num):
         if frame_num >= len(self):
             return
-        img = self._video_reader[frame_num].asnumpy()
-        if img.shape[-1] == 3:
-            img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
-        assert img is not None, f"no image found in {self._video_reader[frame_num]}"
-        return img
+        self._video_reader.set(cv2.CAP_PROP_POS_FRAMES, frame_num)
+        ret, frame = self._video_reader.read()
+        assert ret, f"frame number = {frame_num} is corrupted"
+        return frame
 
     def __len__(self):
-        return len(self._video_reader)
+        return self._total_frames
 
 
 class LocalDirReader(FrameReader):
     def __init__(self, local_frame_dir):
         self.local_frame_dir = local_frame_dir
         self._frame_paths = self._create_frame_list()
```

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/recorder.py` & `cvvideoplayer-0.1.4/cvvideoplayer/recorder.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/utils/bbox_utils.py` & `cvvideoplayer-0.1.4/cvvideoplayer/utils/bbox_utils.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer/utils/windows_vk_dict.py` & `cvvideoplayer-0.1.4/cvvideoplayer/utils/windows_vk_dict.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer.egg-info/PKG-INFO` & `cvvideoplayer-0.1.4/cvvideoplayer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: cvvideoplayer
-Version: 0.1.3
+Version: 0.1.4
 Summary: moduler multi purpose video player for python
 Author: Daniel Tomer
 Author-email: danieltomer1@gmail.com
 Project-URL: Homepage, https://github.com/danieltomer1/CVVideoPlayer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 License-File: License.txt
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: pynput
-Requires-Dist: decord
 Requires-Dist: python-xlib
 Requires-Dist: matplotlib
 
 CV video player is a Python-based customizable video player that helps computer vision practitioners to develop, analyze and debug their video related algorithms and model.
```

### Comparing `cvvideoplayer-0.1.3/cvvideoplayer.egg-info/SOURCES.txt` & `cvvideoplayer-0.1.4/cvvideoplayer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 License.txt
 README.md
 setup.py
 cvvideoplayer/__init__.py
 cvvideoplayer/frame_reader.py
+cvvideoplayer/input_manager.py
 cvvideoplayer/recorder.py
 cvvideoplayer/video_player.py
 cvvideoplayer.egg-info/PKG-INFO
 cvvideoplayer.egg-info/SOURCES.txt
 cvvideoplayer.egg-info/dependency_links.txt
 cvvideoplayer.egg-info/requires.txt
 cvvideoplayer.egg-info/top_level.txt
 cvvideoplayer/frame_editors/__init__.py
 cvvideoplayer/frame_editors/base_bbox_plotter.py
 cvvideoplayer/frame_editors/base_frame_editor.py
 cvvideoplayer/frame_editors/detections_csv_plotter.py
 cvvideoplayer/frame_editors/basic_frame_editors/__init__.py
+cvvideoplayer/frame_editors/basic_frame_editors/frame_info_overlay.py
 cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py
-cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py
 cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py
+cvvideoplayer/frame_editors/basic_frame_editors/key_map_overlay.py
 cvvideoplayer/utils/__init__.py
 cvvideoplayer/utils/bbox_utils.py
 cvvideoplayer/utils/drawing_utils.py
 cvvideoplayer/utils/video_player_utils.py
 cvvideoplayer/utils/windows_vk_dict.py
 tests/test_video_player_basic_functionality.py
```

### Comparing `cvvideoplayer-0.1.3/setup.py` & `cvvideoplayer-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cvvideoplayer",
-    version="0.1.3",
+    version="0.1.4",
     author="Daniel Tomer",
     author_email="danieltomer1@gmail.com",
     description="moduler multi purpose video player for python",
     long_description=(
         "CV video player is a Python-based customizable video player that helps"
         " computer vision practitioners to develop, analyze and debug their video"
         " related algorithms and model."
@@ -16,15 +16,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     install_requires=[
         "numpy",
         "opencv-python",
         "pynput",
-        "decord",
         "python-xlib",
         "matplotlib",
     ],
     python_requires=">=3.8",
     project_urls={
         "Homepage": "https://github.com/danieltomer1/CVVideoPlayer",
     },
```


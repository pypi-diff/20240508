# Comparing `tmp/headless_kivy_pi-0.7.2.tar.gz` & `tmp/headless_kivy_pi-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headless_kivy_pi-0.7.2.tar", max compression
+gzip compressed data, was "headless_kivy_pi-0.7.3.tar", max compression
```

## Comparing `headless_kivy_pi-0.7.2.tar` & `headless_kivy_pi-0.7.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-24 12:26:07.826318 headless_kivy_pi-0.7.2/LICENSE
--rw-r--r--   0        0        0     3771 2024-03-24 12:26:07.826318 headless_kivy_pi-0.7.2/README.md
--rw-r--r--   0        0        0     9642 2024-03-24 12:26:07.826318 headless_kivy_pi-0.7.2/headless_kivy_pi/__init__.py
--rw-r--r--   0        0        0     8602 2024-03-24 12:26:07.826318 headless_kivy_pi-0.7.2/headless_kivy_pi/config.py
--rw-r--r--   0        0        0     1271 2024-03-24 12:26:07.826318 headless_kivy_pi-0.7.2/headless_kivy_pi/constants.py
--rw-r--r--   0        0        0     1373 2024-03-24 12:26:07.826318 headless_kivy_pi-0.7.2/headless_kivy_pi/display.py
--rw-r--r--   0        0        0      930 2024-03-24 12:26:07.826318 headless_kivy_pi-0.7.2/headless_kivy_pi/fake.py
--rw-r--r--   0        0        0      917 2024-03-24 12:26:07.826318 headless_kivy_pi-0.7.2/headless_kivy_pi/logger.py
--rw-r--r--   0        0        0     1410 2024-03-24 12:26:07.826318 headless_kivy_pi-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 headless_kivy_pi-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 15:56:26.140995 headless_kivy_pi-0.7.3/LICENSE
+-rw-r--r--   0        0        0     3771 2024-05-08 15:56:26.140995 headless_kivy_pi-0.7.3/README.md
+-rw-r--r--   0        0        0     9642 2024-05-08 15:56:26.140995 headless_kivy_pi-0.7.3/headless_kivy_pi/__init__.py
+-rw-r--r--   0        0        0     9512 2024-05-08 15:56:26.140995 headless_kivy_pi-0.7.3/headless_kivy_pi/config.py
+-rw-r--r--   0        0        0     1271 2024-05-08 15:56:26.140995 headless_kivy_pi-0.7.3/headless_kivy_pi/constants.py
+-rw-r--r--   0        0        0     1509 2024-05-08 15:56:26.140995 headless_kivy_pi-0.7.3/headless_kivy_pi/display.py
+-rw-r--r--   0        0        0      930 2024-05-08 15:56:26.140995 headless_kivy_pi-0.7.3/headless_kivy_pi/fake.py
+-rw-r--r--   0        0        0      917 2024-05-08 15:56:26.140995 headless_kivy_pi-0.7.3/headless_kivy_pi/logger.py
+-rw-r--r--   0        0        0     1410 2024-05-08 15:56:26.140995 headless_kivy_pi-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 headless_kivy_pi-0.7.3/PKG-INFO
```

### Comparing `headless_kivy_pi-0.7.2/LICENSE` & `headless_kivy_pi-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `headless_kivy_pi-0.7.2/README.md` & `headless_kivy_pi-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `headless_kivy_pi-0.7.2/headless_kivy_pi/__init__.py` & `headless_kivy_pi-0.7.3/headless_kivy_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `headless_kivy_pi-0.7.2/headless_kivy_pi/config.py` & `headless_kivy_pi-0.7.3/headless_kivy_pi/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # pyright: reportMissingImports=false
 """Implement `setup_headless_kivy`, it configures headless-kivy-pi."""
+
 from __future__ import annotations
 
 import atexit
 import sys
 from functools import cache
 from typing import TYPE_CHECKING, NoReturn, NotRequired, TypedDict
 
@@ -72,36 +73,42 @@
     up or not at the expense of possible frame skipping."""
     synchronous_clock: NotRequired[bool]
     """If set to `True`, it will monitor the hash of the screen data, if this hash
     changes, it will increase the fps to the maximum and if the hash doesn't change for
     a while, it will drop the fps to the minimum."""
     automatic_fps: NotRequired[bool]
     """If set to `True`, it will clear the screen before exiting."""
-    clear_at_eixt: NotRequired[bool]
+    clear_at_exit: NotRequired[bool]
 
 
 _config: SetupHeadlessConfig | None = None
 _display: DisplaySPI = None
 
 
 def report_uninitialized() -> NoReturn:
     """Report that the module has not been initialized."""
     msg = """You need to run `setup_headless_kivy` before importing \
 `kivy.core.window` module. \
 Note that it might have been imported by another module unintentionally."""
     raise RuntimeError(msg)
 
 
-def setup_headless_kivy(config: SetupHeadlessConfig) -> None:
+def setup_headless_kivy(
+    config: SetupHeadlessConfig,
+    splash_screen: bytes | None = None,
+) -> None:
     """Configure the headless mode for the Kivy application.
 
     Arguments:
     ---------
     config: `SetupHeadlessConfig`
 
+    splash_screen: `bytes`
+        it should have a length of `width` x `height` x 2
+
     """
     global _config, _display  # noqa: PLW0603
     _config = config
 
     if is_debug_mode():
         add_stdout_handler()
         add_file_handler()
@@ -155,14 +162,21 @@
             y_offset=80,
             x_offset=0,
             cs=cs_pin,
             dc=dc_pin,
             rst=reset_pin,
             baudrate=baudrate,
         )
+        _display._block(  # noqa: SLF001
+            0,
+            0,
+            width() - 1,
+            height() - 1,
+            bytes(width() * height() * 2) if splash_screen is None else splash_screen,
+        )
         if clear_at_exit:
             atexit.register(
                 lambda: _display
                 and _display._block(  # noqa: SLF001
                     0,
                     0,
                     width() - 1,
@@ -261,14 +275,38 @@
 def automatic_fps() -> bool:
     """headless-kivy-pi adjusts the FPS automatically."""
     if _config:
         return _config.get('automatic_fps', AUTOMATIC_FPS)
     report_uninitialized()
 
 
+@cache
+def rotation() -> int:
+    """Return the rotation of the display."""
+    if _config:
+        return _config.get('rotation', 0)
+    report_uninitialized()
+
+
+@cache
+def flip_horizontal() -> bool:
+    """Return `True` if the display is flipped horizontally."""
+    if _config:
+        return _config.get('flip_horizontal', False)
+    report_uninitialized()
+
+
+@cache
+def flip_vertical() -> bool:
+    """Return `True` if the display is flipped vertically."""
+    if _config:
+        return _config.get('flip_vertical', False)
+    report_uninitialized()
+
+
 _is_paused: bool = False
 
 
 def is_paused() -> bool:
     """Return `True` if rendering the application is paused."""
     return _is_paused
```

### Comparing `headless_kivy_pi-0.7.2/headless_kivy_pi/constants.py` & `headless_kivy_pi-0.7.3/headless_kivy_pi/constants.py`

 * *Files identical despite different names*

### Comparing `headless_kivy_pi-0.7.2/headless_kivy_pi/display.py` & `headless_kivy_pi-0.7.3/headless_kivy_pi/display.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,20 @@
     data: NDArray[np.uint16],
     data_hash: int,
     last_render_thread: Thread,
 ) -> None:
     """Transfer data to the display via SPI controller."""
     logger.debug(f'Rendering frame with hash "{data_hash}"')
 
-    # Flip the image vertically
-    data = data.reshape(rectangle[2], rectangle[3], -1)[::-1, :, :3].astype(np.uint16)
+    data = data.reshape(rectangle[2], rectangle[3], -1)[:, :, :3].astype(np.uint16)
+    data = np.rot90(data, config.rotation())
+    if config.flip_horizontal():
+        data = np.fliplr(data)
+    if config.flip_vertical():
+        data = np.flipud(data)
 
     color = (
         ((data[:, :, 0] & 0xF8) << 8)
         | ((data[:, :, 1] & 0xFC) << 3)
         | (data[:, :, 2] >> 3)
     )
     data_bytes = bytes(
```

### Comparing `headless_kivy_pi-0.7.2/headless_kivy_pi/fake.py` & `headless_kivy_pi-0.7.3/headless_kivy_pi/fake.py`

 * *Files identical despite different names*

### Comparing `headless_kivy_pi-0.7.2/headless_kivy_pi/logger.py` & `headless_kivy_pi-0.7.3/headless_kivy_pi/logger.py`

 * *Files identical despite different names*

### Comparing `headless_kivy_pi-0.7.2/pyproject.toml` & `headless_kivy_pi-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "headless-kivy-pi"
-version = "0.7.2"
+version = "0.7.3"
 description = "Headless renderer for Kivy framework on Raspberry Pi"
 authors = ["Sassan Haradji <sassanh@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "headless_kivy_pi" }]
 
 [tool.poetry.dependencies]
```

### Comparing `headless_kivy_pi-0.7.2/PKG-INFO` & `headless_kivy_pi-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headless-kivy-pi
-Version: 0.7.2
+Version: 0.7.3
 Summary: Headless renderer for Kivy framework on Raspberry Pi
 License: Apache-2.0
 Author: Sassan Haradji
 Author-email: sassanh@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


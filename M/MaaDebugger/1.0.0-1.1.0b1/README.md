# Comparing `tmp/maadebugger-1.0.0.tar.gz` & `tmp/maadebugger-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadebugger-1.0.0.tar", last modified: Sat May  4 12:27:41 2024, max compression
+gzip compressed data, was "maadebugger-1.1.0b1.tar", last modified: Wed May  8 07:09:02 2024, max compression
```

## Comparing `maadebugger-1.0.0.tar` & `maadebugger-1.1.0b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-05-04 12:27:32.398086 maadebugger-1.0.0/LICENSE
--rw-r--r--   0        0        0       13 2024-05-04 12:27:32.402086 maadebugger-1.0.0/README.md
--rw-r--r--   0        0        0      470 2024-05-04 12:27:41.962095 maadebugger-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       62 2024-05-04 12:27:32.402086 maadebugger-1.0.0/src/MaaDebugger/__main__.py
--rw-r--r--   0        0        0     3927 2024-05-04 12:27:32.402086 maadebugger-1.0.0/src/MaaDebugger/maafw/__init__.py
--rw-r--r--   0        0        0      254 2024-05-04 12:27:32.402086 maadebugger-1.0.0/src/MaaDebugger/main.py
--rw-r--r--   0        0        0      201 2024-05-04 12:27:32.402086 maadebugger-1.0.0/src/MaaDebugger/utils/__init__.py
--rw-r--r--   0        0        0      799 2024-05-04 12:27:32.402086 maadebugger-1.0.0/src/MaaDebugger/webpage/components/status_indicator.py
--rw-r--r--   0        0        0      240 2024-05-04 12:27:32.402086 maadebugger-1.0.0/src/MaaDebugger/webpage/index_page/__init__.py
--rw-r--r--   0        0        0     6213 2024-05-04 12:27:32.402086 maadebugger-1.0.0/src/MaaDebugger/webpage/index_page/master_control.py
--rw-r--r--   0        0        0     2788 2024-05-04 12:27:32.402086 maadebugger-1.0.0/src/MaaDebugger/webpage/index_page/runtime_control.py
--rw-r--r--   0        0        0      901 2024-05-04 12:27:32.402086 maadebugger-1.0.0/src/MaaDebugger/webpage/reco_page/__init__.py
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 maadebugger-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-08 07:08:50.589925 maadebugger-1.1.0b1/LICENSE
+-rw-r--r--   0        0        0      123 2024-05-08 07:08:50.589925 maadebugger-1.1.0b1/README.md
+-rw-r--r--   0        0        0      478 2024-05-08 07:09:02.693932 maadebugger-1.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/__main__.py
+-rw-r--r--   0        0        0     4854 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/maafw/__init__.py
+-rw-r--r--   0        0        0      254 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/main.py
+-rw-r--r--   0        0        0      201 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/utils/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/components/status_indicator.py
+-rw-r--r--   0        0        0      240 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/index_page/__init__.py
+-rw-r--r--   0        0        0     8775 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/index_page/master_control.py
+-rw-r--r--   0        0        0     2788 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/index_page/runtime_control.py
+-rw-r--r--   0        0        0      901 2024-05-08 07:08:50.593925 maadebugger-1.1.0b1/src/MaaDebugger/webpage/reco_page/__init__.py
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 maadebugger-1.1.0b1/PKG-INFO
```

### Comparing `maadebugger-1.0.0/LICENSE` & `maadebugger-1.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `maadebugger-1.0.0/src/MaaDebugger/maafw/__init__.py` & `maadebugger-1.1.0b1/src/MaaDebugger/maafw/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
+from dataclasses import dataclass
 from pathlib import Path
 from typing import Callable, List, Optional
 
-from maa.controller import AdbController
+from maa.controller import AdbController, Win32Controller
 from maa.instance import Instance
 from maa.resource import Resource
 from maa.toolkit import Toolkit
 from PIL import Image
 
 from ..utils import cvmat_to_image
 
@@ -31,23 +32,52 @@
         self.on_miss_all = on_miss_all
         self.on_recognition_result = on_recognition_result
 
     @staticmethod
     async def detect_adb() -> List["AdbDevice"]:
         return await Toolkit.adb_devices()
 
+    @dataclass
+    class Window:
+        hwnd: int
+        class_name: str
+        window_name: str
+
+    @staticmethod
+    async def detect_win32hwnd(class_regex: str, window_regex: str) -> List[Window]:
+        hwnds = Toolkit.search_window(class_regex, window_regex)
+        windows = []
+        for hwnd in hwnds:
+            class_name = Toolkit.get_class_name(hwnd)
+            window_name = Toolkit.get_window_name(hwnd)
+            windows.append(MaaFW.Window(hwnd, class_name, window_name))
+
+        return windows
+
     async def connect_adb(self, path: Path, address: str) -> bool:
         self.controller = AdbController(path, address)
         connected = await self.controller.connect()
         if not connected:
             print(f"Failed to connect {path} {address}")
             return False
 
         return True
 
+    async def connect_win32hwnd(self, hwnd: int | str) -> bool:
+        if isinstance(hwnd, str):
+            hwnd = int(hwnd, 16)
+
+        self.controller = Win32Controller(hwnd)
+        connected = await self.controller.connect()
+        if not connected:
+            print(f"Failed to connect {hwnd}")
+            return False
+
+        return True
+
     async def load_resource(self, dir: Path) -> bool:
         if not self.resource:
             self.resource = Resource()
 
         return self.resource.clear() and await self.resource.load(dir)
 
     async def run_task(self, entry: str, param: dict = {}) -> bool:
```

### Comparing `maadebugger-1.0.0/src/MaaDebugger/webpage/components/status_indicator.py` & `maadebugger-1.1.0b1/src/MaaDebugger/webpage/components/status_indicator.py`

 * *Files identical despite different names*

### Comparing `maadebugger-1.0.0/src/MaaDebugger/webpage/index_page/runtime_control.py` & `maadebugger-1.1.0b1/src/MaaDebugger/webpage/index_page/runtime_control.py`

 * *Files identical despite different names*

### Comparing `maadebugger-1.0.0/src/MaaDebugger/webpage/reco_page/__init__.py` & `maadebugger-1.1.0b1/src/MaaDebugger/webpage/reco_page/__init__.py`

 * *Files identical despite different names*


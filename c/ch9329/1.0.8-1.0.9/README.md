# Comparing `tmp/ch9329-1.0.8.tar.gz` & `tmp/ch9329-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch9329-1.0.8.tar", last modified: Tue Apr 30 15:28:21 2024, max compression
+gzip compressed data, was "ch9329-1.0.9.tar", last modified: Wed May  8 10:49:10 2024, max compression
```

## Comparing `ch9329-1.0.8.tar` & `ch9329-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:21.601718 ch9329-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-30 15:28:12.000000 ch9329-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-30 15:28:12.000000 ch9329-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-30 15:28:21.601718 ch9329-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-30 15:28:12.000000 ch9329-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:21.601718 ch9329-1.0.8/ch9329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-30 15:28:12.000000 ch9329-1.0.8/ch9329/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:28:21.601718 ch9329-1.0.8/ch9329.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 15:28:21.000000 ch9329-1.0.8/ch9329.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-30 15:28:12.000000 ch9329-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:28:21.601718 ch9329-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:10.631512 ch9329-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 10:49:06.000000 ch9329-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 10:49:06.000000 ch9329-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-08 10:49:10.631512 ch9329-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-08 10:49:06.000000 ch9329-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:10.631512 ch9329-1.0.9/ch9329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:10.631512 ch9329-1.0.9/ch9329.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-08 10:49:06.000000 ch9329-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:49:10.631512 ch9329-1.0.9/setup.cfg
```

### Comparing `ch9329-1.0.8/LICENSE` & `ch9329-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.8/PKG-INFO` & `ch9329-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.0.8/README.md` & `ch9329-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.8/ch9329/config.py` & `ch9329-1.0.9/ch9329/config.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.8/ch9329/hid.py` & `ch9329-1.0.9/ch9329/hid.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,18 +165,20 @@
 HID_KEY_EXSEL = b"\xa4"
 
 # RESERVED
 HID_KEY_CONTROL_LEFT = b"\x01"
 HID_KEY_SHIFT_LEFT = b"\x02"
 HID_KEY_ALT_LEFT = b"\x04"
 HID_KEY_GUI_LEFT = b"\x08"
+HID_KEY_WIN_LEFT = b"\xe3"
 HID_KEY_CONTROL_RIGHT = b"\x10"
 HID_KEY_SHIFT_RIGHT = b"\x20"
 HID_KEY_ALT_RIGHT = b"\x40"
 HID_KEY_GUI_RIGHT = b"\x80"
+HID_KEY_WIN_RIGHT = b"\xe7"
 
 HID_MAPPING = {
     "a": (HID_KEY_A, None),
     "b": (HID_KEY_B, None),
     "c": (HID_KEY_C, None),
     "d": (HID_KEY_D, None),
     "e": (HID_KEY_E, None),
@@ -346,15 +348,17 @@
     "ctrl_right": (HID_KEY_CONTROL_RIGHT, None),
     "shift": (HID_KEY_SHIFT_LEFT, None),
     "shift_left": (HID_KEY_SHIFT_LEFT, None),
     "shift_right": (HID_KEY_SHIFT_RIGHT, None),
     "alt": (HID_KEY_ALT_LEFT, None),
     "alt_left": (HID_KEY_ALT_LEFT, None),
     "alt_right": (HID_KEY_ALT_RIGHT, None),
-    "win": (HID_KEY_GUI_LEFT, None),
+    "win": (HID_KEY_WIN_LEFT, None),
+    "win_left": (HID_KEY_WIN_LEFT, None),
+    "win_right": (HID_KEY_WIN_RIGHT, None),
     "gui": (HID_KEY_GUI_LEFT, None),
     "gui_left": (HID_KEY_GUI_LEFT, None),
     "gui_right": (HID_KEY_GUI_RIGHT, None),
     # white spaces
     " ": (HID_KEY_SPACE, None),
     "\t": (HID_KEY_TAB, None),
     "\n": (HID_KEY_ENTER, None),
@@ -431,8 +435,11 @@
     "shift_right",
     "alt",
     "alt_left",
     "alt_right",
     "gui",
     "gui_left",
     "gui_right",
+    "win",
+    "win_left",
+    "win_right",
 }
```

### Comparing `ch9329-1.0.8/ch9329/keyboard.py` & `ch9329-1.0.9/ch9329/keyboard.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.8/ch9329/mouse.py` & `ch9329-1.0.9/ch9329/mouse.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.8/ch9329/utils.py` & `ch9329-1.0.9/ch9329/utils.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.8/ch9329.egg-info/PKG-INFO` & `ch9329-1.0.9/ch9329.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `ch9329-1.0.8/pyproject.toml` & `ch9329-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ch9329"
-version = "1.0.8"
+version = "1.0.9"
 dependencies = ["pyserial"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Python module to control ch9329"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```


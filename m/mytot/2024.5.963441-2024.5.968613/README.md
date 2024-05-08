# Comparing `tmp/mytot-2024.5.963441-py3-none-any.whl.zip` & `tmp/mytot-2024.5.968613-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 27764 bytes, number of entries: 9
+Zip file size: 27767 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-18 09:16 mytot/__init__.py
--rw-rw-r--  2.0 unx     4094 b- defN 24-May-01 03:30 mytot/main.py
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.5.963441.data/data/LICENSE
--rwxrwxr-x  2.0 unx    35149 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/LICENSE
--rw-rw-r--  2.0 unx      774 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/WHEEL
--rw-rw-r--  2.0 unx       85 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      752 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/RECORD
-9 files, 76101 bytes uncompressed, 26454 bytes compressed:  65.2%
+-rw-rw-r--  2.0 unx     4127 b- defN 24-May-01 03:38 mytot/main.py
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.5.968613.data/data/LICENSE
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-May-01 03:38 mytot-2024.5.968613.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      774 b- defN 24-May-01 03:38 mytot-2024.5.968613.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-01 03:38 mytot-2024.5.968613.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       85 b- defN 24-May-01 03:38 mytot-2024.5.968613.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 24-May-01 03:38 mytot-2024.5.968613.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      752 b- defN 24-May-01 03:38 mytot-2024.5.968613.dist-info/RECORD
+9 files, 76134 bytes uncompressed, 26457 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: mytot/__init__.py
 Comment: 
 
 Filename: mytot/main.py
 Comment: 
 
-Filename: mytot-2024.5.963441.data/data/LICENSE
+Filename: mytot-2024.5.968613.data/data/LICENSE
 Comment: 
 
-Filename: mytot-2024.5.963441.dist-info/LICENSE
+Filename: mytot-2024.5.968613.dist-info/LICENSE
 Comment: 
 
-Filename: mytot-2024.5.963441.dist-info/METADATA
+Filename: mytot-2024.5.968613.dist-info/METADATA
 Comment: 
 
-Filename: mytot-2024.5.963441.dist-info/WHEEL
+Filename: mytot-2024.5.968613.dist-info/WHEEL
 Comment: 
 
-Filename: mytot-2024.5.963441.dist-info/entry_points.txt
+Filename: mytot-2024.5.968613.dist-info/entry_points.txt
 Comment: 
 
-Filename: mytot-2024.5.963441.dist-info/top_level.txt
+Filename: mytot-2024.5.968613.dist-info/top_level.txt
 Comment: 
 
-Filename: mytot-2024.5.963441.dist-info/RECORD
+Filename: mytot-2024.5.968613.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mytot/main.py

```diff
@@ -3,16 +3,20 @@
 import signal
 import datetime
 import subprocess
 import psutil
 
 from loguru import logger
 
+PID = os.getpid()
+
 
 def kill_process_tree(pid, sig_n=signal.SIGKILL):
+    if pid == PID:
+        return
     sig = signal.SIGTERM
     if sig_n == 9:
         sig = signal.SIGKILL
     pid_list = [pid]
     while True:
         if len(pid_list) == 0:
             break
@@ -26,17 +30,14 @@
                 for child in children:
                     pid_list.append(child.pid)
             cmdline = " ".join(parent.cmdline())
             print(f"kill {parent.pid} {cmdline}")
             parent.send_signal(sig)
 
 
-PID = os.getpid()
-
-
 def mkdir(path):
     if not os.path.exists(path):
         os.makedirs(path)
 
 
 def RUN():
     if len(sys.argv) < 2:
```

## Comparing `mytot-2024.5.963441.data/data/LICENSE` & `mytot-2024.5.968613.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `mytot-2024.5.963441.dist-info/LICENSE` & `mytot-2024.5.968613.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mytot-2024.5.963441.dist-info/METADATA` & `mytot-2024.5.968613.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytot
-Version: 2024.5.963441
+Version: 2024.5.968613
 Summary: Tool of Tool
 Author: Xin-Xin Ma
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: psutil
```


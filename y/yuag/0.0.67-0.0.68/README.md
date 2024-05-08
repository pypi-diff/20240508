# Comparing `tmp/yuag-0.0.67.tar.gz` & `tmp/yuag-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.67.tar", last modified: Sun May  5 13:54:32 2024, max compression
+gzip compressed data, was "yuag-0.0.68.tar", last modified: Wed May  8 20:48:41 2024, max compression
```

## Comparing `yuag-0.0.67.tar` & `yuag-0.0.68.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 13:54:32.257105 yuag-0.0.67/
--rw-rw-rw-   0        0        0       52 2024-05-05 13:54:32.255106 yuag-0.0.67/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-05 13:54:32.257105 yuag-0.0.67/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-05-05 13:51:38.000000 yuag-0.0.67/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:54:32.238118 yuag-0.0.67/yuag/
--rw-rw-rw-   0        0        0     2838 2024-05-05 13:20:05.000000 yuag-0.0.67/yuag/__init__.py
--rw-rw-rw-   0        0        0    42998 2024-05-05 13:21:47.000000 yuag-0.0.67/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:54:32.253108 yuag-0.0.67/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-05 13:54:32.000000 yuag-0.0.67/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-05-05 13:54:32.000000 yuag-0.0.67/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 13:54:32.000000 yuag-0.0.67/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-05 13:54:32.000000 yuag-0.0.67/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 20:48:41.591204 yuag-0.0.68/
+-rw-rw-rw-   0        0        0       52 2024-05-08 20:48:41.590205 yuag-0.0.68/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-08 20:48:41.592203 yuag-0.0.68/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-05-08 20:47:20.000000 yuag-0.0.68/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:48:41.573215 yuag-0.0.68/yuag/
+-rw-rw-rw-   0        0        0     2853 2024-05-08 20:47:05.000000 yuag-0.0.68/yuag/__init__.py
+-rw-rw-rw-   0        0        0    43228 2024-05-08 20:46:14.000000 yuag-0.0.68/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-05-08 20:48:41.588207 yuag-0.0.68/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-08 20:48:41.000000 yuag-0.0.68/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-05-08 20:48:41.000000 yuag-0.0.68/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 20:48:41.000000 yuag-0.0.68/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-08 20:48:41.000000 yuag-0.0.68/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.67/yuag/__init__.py` & `yuag-0.0.68/yuag/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 دوال عامة:
 -----------------
 ```
 wait()
 clear()
 detect_lang()
 rangeNum()
+python_path()
 ```
 \n\n
 
 دوال للملفات:
 -----------------
 ```
 filesIn()
```

### Comparing `yuag-0.0.67/yuag/yuag.py` & `yuag-0.0.68/yuag/yuag.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,25 @@
         i = 0
         while i < num:
             res.append(i)
             i += 1
 
         return res
 
+def python_path():
+    """
+    اللهم صل على سيدنا محمد ﷺ\n
+    ارجاع قيمة مسار بايثون، مثل:
+    `C:\Python\python.exe`
+    """
+    
+    import sys
+
+    return sys.executable
+
 # file defs
 def filesIn(folder_path: str = "./"):
     import os
 
     return os.listdir(folder_path)
 
 def rename_file(file_path: str, new_name: str):
```


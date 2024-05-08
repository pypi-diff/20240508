# Comparing `tmp/mhdwriter-0.2.0.tar.gz` & `tmp/mhdwriter-0.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhdwriter-0.2.0.tar", max compression
+gzip compressed data, was "mhdwriter-0.2.0.1.tar", max compression
```

## Comparing `mhdwriter-0.2.0.tar` & `mhdwriter-0.2.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-07 22:27:59.694556 mhdwriter-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-07 22:27:25.533994 mhdwriter-0.2.0/mhdwriter/__init__.py
--rw-r--r--   0        0        0      525 2024-05-07 22:27:25.534380 mhdwriter-0.2.0/mhdwriter/args.py
--rw-r--r--   0        0        0     4616 2024-05-07 22:27:25.533839 mhdwriter-0.2.0/mhdwriter/header.py
--rw-r--r--   0        0        0     2900 2024-05-07 22:27:25.534647 mhdwriter-0.2.0/mhdwriter/writer.py
--rw-r--r--   0        0        0      356 2024-05-08 00:12:58.158670 mhdwriter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 mhdwriter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-08 13:57:58.812358 mhdwriter-0.2.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 13:57:58.812621 mhdwriter-0.2.0.1/mhdwriter/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-08 13:57:58.812724 mhdwriter-0.2.0.1/mhdwriter/args.py
+-rw-r--r--   0        0        0     4616 2024-05-08 13:57:58.812840 mhdwriter-0.2.0.1/mhdwriter/header.py
+-rw-r--r--   0        0        0     2967 2024-05-08 15:44:38.795651 mhdwriter-0.2.0.1/mhdwriter/writer.py
+-rw-r--r--   0        0        0      358 2024-05-08 15:46:32.893735 mhdwriter-0.2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      395 1970-01-01 00:00:00.000000 mhdwriter-0.2.0.1/PKG-INFO
```

### Comparing `mhdwriter-0.2.0/mhdwriter/args.py` & `mhdwriter-0.2.0.1/mhdwriter/args.py`

 * *Files identical despite different names*

### Comparing `mhdwriter-0.2.0/mhdwriter/header.py` & `mhdwriter-0.2.0.1/mhdwriter/header.py`

 * *Files identical despite different names*

### Comparing `mhdwriter-0.2.0/mhdwriter/writer.py` & `mhdwriter-0.2.0.1/mhdwriter/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
                 print(f"Error reading {str(img_file)}: {e}")
                 continue
             if img is None:
                 print(f"Error reading {str(img_file)}")
                 continue
             if args.is_rgb:
                 img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+            if not out_path.exists():
+                return False
 
             if args.downsample_factor > 0:
                 img = cv2.resize(
                     img, (args.width, args.height), interpolation=cv2.INTER_AREA
                 )
 
             if args.write_type == WriteType.NONE:
```


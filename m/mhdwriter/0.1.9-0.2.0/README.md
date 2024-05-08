# Comparing `tmp/mhdwriter-0.1.9.tar.gz` & `tmp/mhdwriter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhdwriter-0.1.9.tar", last modified: Sat Dec 23 13:49:09 2023, max compression
+gzip compressed data, was "mhdwriter-0.2.0.tar", max compression
```

## Comparing `mhdwriter-0.1.9.tar` & `mhdwriter-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 white      (501) staff       (20)        0 2023-12-23 13:49:09.328038 mhdwriter-0.1.9/
--rw-r--r--   0 white      (501) staff       (20)      312 2023-12-23 13:49:09.327873 mhdwriter-0.1.9/PKG-INFO
-drwxr-xr-x   0 white      (501) staff       (20)        0 2023-12-23 13:49:09.326892 mhdwriter-0.1.9/mhdwriter/
--rw-r--r--   0 white      (501) staff       (20)        0 2023-12-18 18:57:37.000000 mhdwriter-0.1.9/mhdwriter/__init__.py
--rw-r--r--   0 white      (501) staff       (20)      568 2023-12-23 13:46:21.000000 mhdwriter-0.1.9/mhdwriter/args.py
--rw-r--r--   0 white      (501) staff       (20)     4824 2023-12-22 15:30:14.000000 mhdwriter-0.1.9/mhdwriter/header.py
--rw-r--r--   0 white      (501) staff       (20)     3703 2023-12-23 13:48:14.000000 mhdwriter-0.1.9/mhdwriter/writer.py
-drwxr-xr-x   0 white      (501) staff       (20)        0 2023-12-23 13:49:09.327725 mhdwriter-0.1.9/mhdwriter.egg-info/
--rw-r--r--   0 white      (501) staff       (20)      312 2023-12-23 13:49:09.000000 mhdwriter-0.1.9/mhdwriter.egg-info/PKG-INFO
--rw-r--r--   0 white      (501) staff       (20)      300 2023-12-23 13:49:09.000000 mhdwriter-0.1.9/mhdwriter.egg-info/SOURCES.txt
--rw-r--r--   0 white      (501) staff       (20)        1 2023-12-23 13:49:09.000000 mhdwriter-0.1.9/mhdwriter.egg-info/dependency_links.txt
--rw-r--r--   0 white      (501) staff       (20)       35 2023-12-23 13:49:09.000000 mhdwriter-0.1.9/mhdwriter.egg-info/requires.txt
--rw-r--r--   0 white      (501) staff       (20)       10 2023-12-23 13:49:09.000000 mhdwriter-0.1.9/mhdwriter.egg-info/top_level.txt
--rw-r--r--   0 white      (501) staff       (20)      459 2023-12-23 13:48:39.000000 mhdwriter-0.1.9/pyproject.toml
--rw-r--r--   0 white      (501) staff       (20)       38 2023-12-23 13:49:09.328077 mhdwriter-0.1.9/setup.cfg
-drwxr-xr-x   0 white      (501) staff       (20)        0 2023-12-23 13:49:09.327595 mhdwriter-0.1.9/tests/
--rw-r--r--   0 white      (501) staff       (20)     1920 2023-12-19 15:39:52.000000 mhdwriter-0.1.9/tests/test_header.py
--rw-r--r--   0 white      (501) staff       (20)     1126 2023-12-19 15:19:14.000000 mhdwriter-0.1.9/tests/test_writer.py
+-rw-r--r--   0        0        0        0 2024-05-07 22:27:59.694556 mhdwriter-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 22:27:25.533994 mhdwriter-0.2.0/mhdwriter/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-07 22:27:25.534380 mhdwriter-0.2.0/mhdwriter/args.py
+-rw-r--r--   0        0        0     4616 2024-05-07 22:27:25.533839 mhdwriter-0.2.0/mhdwriter/header.py
+-rw-r--r--   0        0        0     2900 2024-05-07 22:27:25.534647 mhdwriter-0.2.0/mhdwriter/writer.py
+-rw-r--r--   0        0        0      356 2024-05-08 00:12:58.158670 mhdwriter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 mhdwriter-0.2.0/PKG-INFO
```

### Comparing `mhdwriter-0.1.9/mhdwriter/args.py` & `mhdwriter-0.2.0/mhdwriter/args.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,20 @@
     NONE = 0
     RAW = 1
     RAW_COMPRESSED = 2
 
 
 @dataclass
 class WriteArgs:
+    write_type: WriteType
     fov: str
     series_description: str
     study_description: str
     protocol: str
     date_time: datetime | str
-    write_type: WriteType = WriteType.RAW
     root_site_id: str = "1.2.826.0.1.3680043.10.1341"
     downsample_factor: int = 0
     height: int = 0
     width: int = 0
     length: int = 0
     is_rgb: bool = False
     is_hdr: bool = False
-    skip_files: bool = True
```

### Comparing `mhdwriter-0.1.9/mhdwriter/header.py` & `mhdwriter-0.2.0/mhdwriter/header.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,19 @@
 
     assert type(args) == WriteArgs, "Invalid WriteArgs"
 
     if isinstance(args.date_time, str):
         study_date_time = parse_datetime(args.date_time)
     else:
         study_date_time = args.date_time
-    if not args.is_rgb and args.write_type == WriteType.NONE:
-        args.write_type = WriteType.RAW
 
     is_multi = True if args.write_type == WriteType.NONE else False
 
-    raw_name = args.series_description + ".raw"
-    raw_name = raw_name.replace(" ", "_")
+    raw_name = args.study_description + ".raw"
+
     if args.write_type == WriteType.RAW_COMPRESSED:
         raw_name += ".gz"
     pixel_sz = _pixel_size(args.fov.upper()) * (2 ** args.downsample_factor)
     pixel_sz = round(pixel_sz, 5)
 
     metadata = {
         "ObjectType": "Image",
@@ -75,16 +73,14 @@
     else:
         metadata["ElementDataFile"] = raw_name
     return metadata
 
 
 def _pixel_size(fov: str) -> float:
     fov = fov.upper()
-    fov = fov.replace("FOV", "")
-    fov = fov.replace(" ", "")
     xy = 0.00
     if fov == "A":
         xy = 0.020
     elif fov == "B":
         xy = 0.025
     elif fov == "C":
         xy = 0.035
```

### Comparing `mhdwriter-0.1.9/mhdwriter/writer.py` & `mhdwriter-0.2.0/mhdwriter/writer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,84 @@
 import shutil
 from pathlib import Path
 from typing import Optional
 
 import cv2
 import numpy as np
-from tqdm import tqdm
 
 from mhdwriter.args import WriteArgs, WriteType
 from mhdwriter.header import generate_header
 
 
 def write_mhd_raw(
-    input_dir: Path, args: WriteArgs, out_path: Optional[Path] = None, show_progress: bool = True
-) -> Optional[Path]:
+    input_dir: Path, args: WriteArgs, out_path: Optional[Path] = None
+) -> bool:
     """
     Convert a stack of files in a directory to a mhd/raw pair.
 
     Args:
         input_dir (Path): The directory containing the stack of files to convert to a volume.
         args (WriteArgs): WriteArgs object specifying parameters for the MHD header creation.
         out_path (Path): Optional path to specify output directory/file_base. If missing, metadata will be used
             to determine output file/path name in the input_dir.
 
     Returns:
-        Optional[Path]: Returns pathlib Path to mhd file upon successful mhd/raw creation, else None.
+        bool: Returns True upon successful mhd/raw creation, else False.
 
     """
-    if not args.is_rgb and args.write_type == WriteType.NONE:
-        args.write_type = WriteType.RAW
-
-    all_files = sorted(list(input_dir.glob("*")))
+    all_files = list(input_dir.glob("*"))
     all_files = [
         f
         for f in all_files
-        if f.is_file() and f.suffix.lower()
+        if f.suffix.lower()
         in [".jpg", ".jxl", ".jp2", ".jpeg", ".png", ".tif", ".tiff"]
     ]
     img = cv2.imread(str(all_files[0]), cv2.IMREAD_UNCHANGED)
     args.height, args.width = img.shape[:2]
     if args.downsample_factor > 0:
         dx_factor = 2 ** args.downsample_factor
-        if args.skip_files:
-            all_files = all_files[::dx_factor]
         args.height = args.height//dx_factor
         args.width = args.width//dx_factor
     args.length = len(all_files)
     metadata = generate_header(args)
 
     if not input_dir.exists():
         raise FileNotFoundError(f"Missing input dir {input_dir}")
 
     if out_path is None:
-        out_path = input_dir
-
-    outfile = None
-
-    if args.write_type == WriteType.NONE:
-        out_path = out_path.joinpath(f"{metadata['SeriesDescription']}")
-        out_path.mkdir(exist_ok=True, parents=True)
-    else:
-        out_path = out_path.joinpath(f"{metadata['ElementDataFile']}")
-        if out_path.exists():
-            print(f"File {out_path} already exists. Skipping.")
-            return
-        outfile = out_path.open(mode="wb")
-
-    out_name = out_path.name
-    file_iterator = tqdm(all_files, desc=f"Generating {out_name}") if show_progress else all_files
-
-    idx = 0
-    for img_file in file_iterator:
-        try:
-            img = cv2.imread(str(img_file), cv2.IMREAD_UNCHANGED)
-        except Exception as e:
-            print(f"Error reading {str(img_file)}: {e}")
-            continue
-        if img is None:
-            print(f"Error reading {str(img_file)}")
-            continue
-        idx += 1
-        if args.is_rgb and not args.write_type == WriteType.NONE:
-            img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-
-        if args.downsample_factor > 0:
-            img = cv2.resize(
-                img, (args.width, args.height), interpolation=cv2.INTER_AREA
-            )
-
         if args.write_type == WriteType.NONE:
-            file_path = out_path.joinpath("slice_{0:04d}.jpg".format(idx + 1))
-            cv2.imwrite(str(file_path), img)
+            out_path = input_dir
         else:
-            squeezed = np.squeeze(img)
-            outfile.write(squeezed.tobytes())
+            out_path = input_dir.joinpath(f"{metadata['ElementDataFile']}")
+
+    with out_path.open(mode="wb") as outfile:
+        for idx, img_file in enumerate(all_files):
+            try:
+                img = cv2.imread(str(img_file), cv2.IMREAD_UNCHANGED)
+            except Exception as e:
+                print(f"Error reading {str(img_file)}: {e}")
+                continue
+            if img is None:
+                print(f"Error reading {str(img_file)}")
+                continue
+            if args.is_rgb:
+                img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+
+            if args.downsample_factor > 0:
+                img = cv2.resize(
+                    img, (args.width, args.height), interpolation=cv2.INTER_AREA
+                )
+
+            if args.write_type == WriteType.NONE:
+                file_path = out_path.joinpath("slice_{0:04d}.jpg".format(idx + 1))
+                cv2.imwrite(str(file_path), img)
+            else:
+                squeezed = np.squeeze(img)
+                outfile.write(squeezed.tobytes())
 
-    if outfile is not None:
-        outfile.close()
     if not out_path.exists():
         return False
-    if args.write_type == WriteType.NONE:
-        mhd_path = out_path.joinpath(f"{out_path.stem}.mhd")
-    else:
-        mhd_path = out_path.parent.joinpath(f"{out_path.stem}.mhd")
+    mhd_path = out_path.parent.joinpath(f"{out_path.stem}.mhd")
     with mhd_path.open("w") as mhd:
         for key in metadata:
             mhd.write(f"{key} = {metadata[key]}\n")
     return True
```


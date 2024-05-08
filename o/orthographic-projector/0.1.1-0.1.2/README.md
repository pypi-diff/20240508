# Comparing `tmp/orthographic_projector-0.1.1.tar.gz` & `tmp/orthographic_projector-0.1.2.tar.gz`

## Comparing `orthographic_projector-0.1.1.tar` & `orthographic_projector-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 orthographic_projector-0.1.1/Cargo.toml
--rw-r--r--   0     1000     1000       47 2024-05-06 23:23:15.000000 orthographic_projector-0.1.1/.gitignore
--rw-r--r--   0     1000     1000    18092 2024-04-28 13:42:19.000000 orthographic_projector-0.1.1/LICENSE
--rw-r--r--   0     1000     1000     1117 2024-05-06 23:10:43.000000 orthographic_projector-0.1.1/README.md
--rw-r--r--   0     1000     1000      879 2024-05-07 16:28:28.000000 orthographic_projector-0.1.1/examples/example_generate_projections.py
--rw-r--r--   0     1000     1000     1828 2024-05-07 16:30:17.000000 orthographic_projector-0.1.1/orthographic_projector/__init__.py
--rw-r--r--   0     1000     1000       43 2024-05-06 23:11:31.000000 orthographic_projector-0.1.1/requirements.txt
--rw-r--r--   0     1000     1000     4247 2024-05-06 23:10:43.000000 orthographic_projector-0.1.1/src/lib.rs
--rw-r--r--   0     1000     1000     8811 2024-05-07 16:15:04.000000 orthographic_projector-0.1.1/Cargo.lock
--rw-r--r--   0     1000     1000      526 2024-05-06 23:38:04.000000 orthographic_projector-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 orthographic_projector-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 orthographic_projector-0.1.2/Cargo.toml
+-rw-r--r--   0     1000     1000       47 2024-05-06 23:23:15.000000 orthographic_projector-0.1.2/.gitignore
+-rw-r--r--   0     1000     1000    18092 2024-04-28 13:42:19.000000 orthographic_projector-0.1.2/LICENSE
+-rw-r--r--   0     1000     1000     3099 2024-05-08 20:30:36.000000 orthographic_projector-0.1.2/README.md
+-rw-r--r--   0     1000     1000 12233470 2024-05-08 20:32:41.000000 orthographic_projector-0.1.2/argcomplete
+-rw-r--r--   0     1000     1000     1265 2024-05-08 20:30:25.000000 orthographic_projector-0.1.2/examples/example_generate_projections.py
+-rwxr-xr-x   0     1000     1000 16335043 2024-04-29 03:08:27.000000 orthographic_projector-0.1.2/examples/redandblack_vox10_1550.ply
+-rw-r--r--   0     1000     1000     1828 2024-05-07 16:30:17.000000 orthographic_projector-0.1.2/orthographic_projector/__init__.py
+-rw-r--r--   0     1000     1000       43 2024-05-06 23:11:31.000000 orthographic_projector-0.1.2/requirements.txt
+-rw-r--r--   0     1000     1000     4247 2024-05-06 23:10:43.000000 orthographic_projector-0.1.2/src/lib.rs
+-rw-r--r--   0     1000     1000 12233469 2024-05-08 20:32:40.000000 orthographic_projector-0.1.2/subprocess
+-rw-r--r--   0     1000     1000 12233462 2024-05-08 20:32:41.000000 orthographic_projector-0.1.2/sys
+-rw-r--r--   0     1000     1000     8811 2024-05-08 20:34:37.000000 orthographic_projector-0.1.2/Cargo.lock
+-rw-r--r--   0     1000     1000      526 2024-05-06 23:38:04.000000 orthographic_projector-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 orthographic_projector-0.1.2/PKG-INFO
```

### Comparing `orthographic_projector-0.1.1/LICENSE` & `orthographic_projector-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orthographic_projector-0.1.1/orthographic_projector/__init__.py` & `orthographic_projector-0.1.2/orthographic_projector/__init__.py`

 * *Files identical despite different names*

### Comparing `orthographic_projector-0.1.1/src/lib.rs` & `orthographic_projector-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `orthographic_projector-0.1.1/Cargo.lock` & `orthographic_projector-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "orthographic_projector"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `orthographic_projector-0.1.1/pyproject.toml` & `orthographic_projector-0.1.2/pyproject.toml`

 * *Files identical despite different names*


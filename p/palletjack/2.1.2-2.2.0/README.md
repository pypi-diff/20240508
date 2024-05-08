# Comparing `tmp/palletjack-2.1.2.tar.gz` & `tmp/palletjack-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palletjack-2.1.2.tar", last modified: Fri Apr 12 11:45:15 2024, max compression
+gzip compressed data, was "palletjack-2.2.0.tar", last modified: Wed May  8 15:35:39 2024, max compression
```

## Comparing `palletjack-2.1.2.tar` & `palletjack-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:45:15.346387 palletjack-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 11:44:46.000000 palletjack-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-12 11:45:15.346387 palletjack-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-12 11:44:46.000000 palletjack-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:45:15.342388 palletjack-2.1.2/palletjack/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/cpalletjack.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    28644 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/palletjack.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/palletjack.h
--rw-r--r--   0 runner    (1001) docker     (127)  1745720 2024-04-12 11:45:14.000000 palletjack-2.1.2/palletjack/palletjack_cython.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/palletjack_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   216223 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/parquet_types_palletjack.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    86184 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/parquet_types_palletjack.h
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-12 11:44:46.000000 palletjack-2.1.2/palletjack/windows_fixup.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:45:15.346387 palletjack-2.1.2/palletjack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:45:14.000000 palletjack-2.1.2/palletjack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 11:45:15.000000 palletjack-2.1.2/palletjack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-12 11:44:46.000000 palletjack-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:45:15.346387 palletjack-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-12 11:44:46.000000 palletjack-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:45:15.346387 palletjack-2.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-04-12 11:44:46.000000 palletjack-2.1.2/test/test_palletjack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-12 11:44:46.000000 palletjack-2.1.2/test/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:39.140204 palletjack-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 15:29:22.000000 palletjack-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-08 15:35:39.136204 palletjack-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-08 15:29:22.000000 palletjack-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:39.136204 palletjack-2.2.0/palletjack/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/cpalletjack.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    28644 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/palletjack.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/palletjack.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1757552 2024-05-08 15:35:37.000000 palletjack-2.2.0/palletjack/palletjack_cython.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/palletjack_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   216223 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/parquet_types_palletjack.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    86184 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/parquet_types_palletjack.h
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 15:29:22.000000 palletjack-2.2.0/palletjack/windows_fixup.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:39.136204 palletjack-2.2.0/palletjack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:35:37.000000 palletjack-2.2.0/palletjack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 15:35:39.000000 palletjack-2.2.0/palletjack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 15:29:22.000000 palletjack-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:35:39.140204 palletjack-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-08 15:29:22.000000 palletjack-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:35:39.136204 palletjack-2.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-05-08 15:29:22.000000 palletjack-2.2.0/test/test_palletjack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-08 15:29:22.000000 palletjack-2.2.0/test/test_readme.py
```

### Comparing `palletjack-2.1.2/LICENSE` & `palletjack-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/PKG-INFO` & `palletjack-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: palletjack
-Version: 2.1.2
+Version: 2.2.0
 Summary: Faster parquet metadata reading
 Author-email: Marcin Krystianc <marcin.krystianc@gmail.com>
 Project-URL: Homepage, https://github.com/marcin-krystianc/PalletJack
 Project-URL: Issues, https://github.com/marcin-krystianc/PalletJack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyarrow~=15.0
+Requires-Dist: pyarrow~=16.0
 
 # PalletJack
 PalletJack was created as a workaround for apache/arrow#38149. The standard parquet reader is not efficient for files with numerous columns and row groups, as it requires parsing the entire metadata section each time the file is opened. The size of this metadata section is proportional to the number of columns and row groups in the file.
 
 PalletJack reduces the amount of metadata bytes that need to be read and decoded by storing metadata in a different format. This approach enables reading only the essential subset of metadata as required.
 
 ## Features
 
 - Storing parquet metadata in an indexed format
 - Reading parquet metadata for a subset of row groups and columns
 
 ## Required:
 
-- pyarrow  ~= 15.0
+- pyarrow  ~= 16.0
  
 PalletJack operates on top of pyarrow, making it an essential requirement for both building and using PalletJack. While our source package is compatible with recent versions of pyarrow, the binary distribution package specifically requires the latest major version of pyarrow.
 
 ##  Installation
 
 ```
 pip install palletjack
```

### Comparing `palletjack-2.1.2/README.md` & `palletjack-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ## Features
 
 - Storing parquet metadata in an indexed format
 - Reading parquet metadata for a subset of row groups and columns
 
 ## Required:
 
-- pyarrow  ~= 15.0
+- pyarrow  ~= 16.0
  
 PalletJack operates on top of pyarrow, making it an essential requirement for both building and using PalletJack. While our source package is compatible with recent versions of pyarrow, the binary distribution package specifically requires the latest major version of pyarrow.
 
 ##  Installation
 
 ```
 pip install palletjack
```

### Comparing `palletjack-2.1.2/palletjack/cpalletjack.pxd` & `palletjack-2.2.0/palletjack/cpalletjack.pxd`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/palletjack/palletjack.cc` & `palletjack-2.2.0/palletjack/palletjack.cc`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/palletjack/palletjack.h` & `palletjack-2.2.0/palletjack/palletjack.h`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/palletjack/palletjack_cython.cpp` & `palletjack-2.2.0/palletjack/palletjack_cython.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/numpy/core/include/numpy/halffloat.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/api.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/array/concatenate.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/builder.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/c/abi.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/c/bridge.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack_abi.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/compute/api.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/compute/expression.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/config.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/csv/api.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/extension/fixed_shape_tensor.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/extension_type.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/io/api.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/ipc/api.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/json/options.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/json/reader.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/api.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/arrow_to_pandas.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/async.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/benchmark.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/common.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/csv.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/extension_type.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/gdb.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/inference.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/init.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/ipc.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/platform.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/pyarrow.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/python/udf.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/result.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/byte_size.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/cancel.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/compression.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/decimal.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/future.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/io_util.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/iterator.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/key_value_metadata.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/thread_pool.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/arrow/util/value_parsing.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/api/reader.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/api/schema.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/api/writer.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/reader.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/schema.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/writer.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/encryption/encryption.h",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include/parquet/properties.h"
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/numpy/core/include/numpy/halffloat.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/api.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/array/concatenate.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/builder.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/c/abi.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/c/bridge.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/c/dlpack_abi.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/compute/api.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/compute/cast.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/compute/expression.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/config.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/csv/api.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/extension/fixed_shape_tensor.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/extension_type.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/io/api.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/ipc/api.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/json/options.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/json/reader.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/api.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/arrow_to_pandas.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/async.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/benchmark.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/common.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/csv.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/extension_type.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/gdb.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/inference.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/init.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/ipc.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/platform.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/pyarrow.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/python/udf.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/result.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/byte_size.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/cancel.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/compression.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/decimal.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/future.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/io_util.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/iterator.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/key_value_metadata.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/thread_pool.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/arrow/util/value_parsing.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/api/reader.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/api/schema.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/api/writer.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/reader.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/schema.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/arrow/writer.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/encryption/encryption.h",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include/parquet/properties.h"
         ],
         "extra_compile_args": [
             "-std=c++17"
         ],
         "include_dirs": [
             ".",
             "/home/runner/work/PalletJack/PalletJack/python/vcpkg_installed/include",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow/include",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow/include",
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "libraries": [
             "arrow",
             "parquet",
             "thrift"
         ],
         "library_dirs": [
             "/home/runner/work/PalletJack/PalletJack/python/vcpkg_installed/lib",
-            "/tmp/build-env-1299802c/lib/python3.10/site-packages/pyarrow"
+            "/tmp/build-env-2bej78g8/lib/python3.10/site-packages/pyarrow"
         ],
         "name": "palletjack.palletjack_cython",
         "sources": [
             "palletjack/palletjack_cython.pyx",
             "palletjack/palletjack.cc",
             "palletjack/parquet_types_palletjack.cpp"
         ]
@@ -1502,14 +1503,15 @@
 #include "arrow/util/io_util.h"
 #include "arrow/util/iterator.h"
 #include "arrow/array/concatenate.h"
 #include "arrow/c/abi.h"
 #include "arrow/c/bridge.h"
 #include "arrow/util/byte_size.h"
 #include "arrow/python/udf.h"
+#include "arrow/compute/cast.h"
 #include "arrow/python/csv.h"
 #include "arrow/python/api.h"
 #include "arrow/python/arrow_to_pandas.h"
 #include "arrow/python/init.h"
 #include "arrow/python/pyarrow.h"
 #include "arrow/python/inference.h"
 #include "arrow/python/ipc.h"
@@ -1935,14 +1937,16 @@
 struct __pyx_obj_7pyarrow_3lib_IpcWriteOptions;
 struct __pyx_obj_7pyarrow_3lib_IpcReadOptions;
 struct __pyx_obj_7pyarrow_3lib_Message;
 struct __pyx_obj_7pyarrow_3lib_MemoryPool;
 struct __pyx_obj_7pyarrow_3lib_DataType;
 struct __pyx_obj_7pyarrow_3lib_ListType;
 struct __pyx_obj_7pyarrow_3lib_LargeListType;
+struct __pyx_obj_7pyarrow_3lib_ListViewType;
+struct __pyx_obj_7pyarrow_3lib_LargeListViewType;
 struct __pyx_obj_7pyarrow_3lib_MapType;
 struct __pyx_obj_7pyarrow_3lib_FixedSizeListType;
 struct __pyx_obj_7pyarrow_3lib_StructType;
 struct __pyx_obj_7pyarrow_3lib_DictionaryMemo;
 struct __pyx_obj_7pyarrow_3lib_DictionaryType;
 struct __pyx_obj_7pyarrow_3lib_TimestampType;
 struct __pyx_obj_7pyarrow_3lib_Time32Type;
@@ -1987,19 +1991,23 @@
 struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray;
 struct __pyx_obj_7pyarrow_3lib_Decimal128Array;
 struct __pyx_obj_7pyarrow_3lib_Decimal256Array;
 struct __pyx_obj_7pyarrow_3lib_StructArray;
 struct __pyx_obj_7pyarrow_3lib_BaseListArray;
 struct __pyx_obj_7pyarrow_3lib_ListArray;
 struct __pyx_obj_7pyarrow_3lib_LargeListArray;
+struct __pyx_obj_7pyarrow_3lib_ListViewArray;
+struct __pyx_obj_7pyarrow_3lib_LargeListViewArray;
 struct __pyx_obj_7pyarrow_3lib_MapArray;
 struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray;
 struct __pyx_obj_7pyarrow_3lib_UnionArray;
 struct __pyx_obj_7pyarrow_3lib_StringArray;
 struct __pyx_obj_7pyarrow_3lib_BinaryArray;
+struct __pyx_obj_7pyarrow_3lib_StringViewArray;
+struct __pyx_obj_7pyarrow_3lib_BinaryViewArray;
 struct __pyx_obj_7pyarrow_3lib_DictionaryArray;
 struct __pyx_obj_7pyarrow_3lib_ExtensionArray;
 struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray;
 struct __pyx_obj_7pyarrow_3lib_ChunkedArray;
 struct __pyx_obj_7pyarrow_3lib__Tabular;
 struct __pyx_obj_7pyarrow_3lib_Table;
 struct __pyx_obj_7pyarrow_3lib_RecordBatch;
@@ -2157,45 +2165,45 @@
 
 #line 312 "cpython/datetime.pxd"
   PyObject *tz;
 
 #line 312 "cpython/datetime.pxd"
 };
 
-/* "pyarrow/includes/libarrow.pxd":1315
+/* "pyarrow/includes/libarrow.pxd":1431
  * 
  * # Use typedef to emulate syntax for std::function<void(..)>
  * ctypedef void CallbackTransform(object, const shared_ptr[CBuffer]& src,             # <<<<<<<<<<<<<<
  *                                 shared_ptr[CBuffer]* dest)
  * 
  */
 
-#line 1315 "pyarrow/includes/libarrow.pxd"
+#line 1431 "pyarrow/includes/libarrow.pxd"
 typedef void __pyx_t_7pyarrow_8includes_8libarrow_CallbackTransform(PyObject *, std::shared_ptr< arrow::Buffer>  const &, std::shared_ptr< arrow::Buffer>  *);
 
-/* "pyarrow/includes/libarrow.pxd":1318
+/* "pyarrow/includes/libarrow.pxd":1434
  *                                 shared_ptr[CBuffer]* dest)
  * 
  * ctypedef CResult[shared_ptr[CInputStream]] StreamWrapFunc(             # <<<<<<<<<<<<<<
  *     shared_ptr[CInputStream])
  * 
  */
 
-#line 1318 "pyarrow/includes/libarrow.pxd"
+#line 1434 "pyarrow/includes/libarrow.pxd"
 typedef arrow::Result<std::shared_ptr< arrow::io::InputStream> >  __pyx_t_7pyarrow_8includes_8libarrow_StreamWrapFunc(std::shared_ptr< arrow::io::InputStream> );
 
-/* "pyarrow/includes/libarrow.pxd":2845
+/* "pyarrow/includes/libarrow.pxd":2981
  *     int64_t TotalBufferSize(const CTable& table)
  * 
  * ctypedef PyObject* CallbackUdf(object user_function, const CUdfContext& context, object inputs)             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
-#line 2845 "pyarrow/includes/libarrow.pxd"
+#line 2981 "pyarrow/includes/libarrow.pxd"
 typedef PyObject *__pyx_t_7pyarrow_8includes_8libarrow_CallbackUdf(PyObject *,  arrow::py::UdfContext const &, PyObject *);
 
 /* "pyarrow/includes/libarrow_python.pxd":24
  * 
  * 
  * ctypedef CInvalidRowResult PyInvalidRowCallback(object,             # <<<<<<<<<<<<<<
  *                                                 const CCSVInvalidRow&)
@@ -2204,38 +2212,38 @@
 
 #line 24 "pyarrow/includes/libarrow_python.pxd"
 typedef  arrow::csv::InvalidRowResult __pyx_t_7pyarrow_8includes_15libarrow_python_PyInvalidRowCallback(PyObject *,  arrow::csv::InvalidRow const &);
 
 #line 24 "pyarrow/includes/libarrow_python.pxd"
 struct __pyx_opt_args_7pyarrow_3lib_ensure_type;
 
-/* "pyarrow/lib.pxd":606
+/* "pyarrow/lib.pxd":634
  * 
  * # Default is allow_none=False
  * cpdef DataType ensure_type(object type, bint allow_none=*)             # <<<<<<<<<<<<<<
  * 
  * cdef timeunit_to_string(TimeUnit unit)
  */
 
-#line 606 "pyarrow/lib.pxd"
+#line 634 "pyarrow/lib.pxd"
 struct __pyx_opt_args_7pyarrow_3lib_ensure_type {
 
-#line 606 "pyarrow/lib.pxd"
+#line 634 "pyarrow/lib.pxd"
   int __pyx_n;
 
-#line 606 "pyarrow/lib.pxd"
+#line 634 "pyarrow/lib.pxd"
   int allow_none;
 
-#line 606 "pyarrow/lib.pxd"
+#line 634 "pyarrow/lib.pxd"
 };
 
-#line 606 "pyarrow/lib.pxd"
+#line 634 "pyarrow/lib.pxd"
 struct __pyx_opt_args_7pyarrow_8_parquet__create_writer_properties;
 
-#line 606 "pyarrow/lib.pxd"
+#line 634 "pyarrow/lib.pxd"
 struct __pyx_opt_args_7pyarrow_8_parquet__create_arrow_writer_properties;
 
 /* "pyarrow/_parquet.pxd":580
  *         return self.properties
  * 
  * cdef shared_ptr[WriterProperties] _create_writer_properties(             # <<<<<<<<<<<<<<
  *     use_dictionary=*,
@@ -2584,1793 +2592,1925 @@
 
 #line 118 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":123
  * 
  * 
- * cdef class MapType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class ListViewType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CMapType* map_type
+ *         const CListViewType* list_view_type
  */
 
 #line 123 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_MapType {
+struct __pyx_obj_7pyarrow_3lib_ListViewType {
 
 #line 123 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
 #line 123 "pyarrow/lib.pxd"
-   arrow::MapType const *map_type;
+   arrow::ListViewType const *list_view_type;
 
 #line 123 "pyarrow/lib.pxd"
 };
 
 #line 123 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":128
  * 
  * 
- * cdef class FixedSizeListType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class LargeListViewType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CFixedSizeListType* list_type
+ *         const CLargeListViewType* list_view_type
  */
 
 #line 128 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_FixedSizeListType {
+struct __pyx_obj_7pyarrow_3lib_LargeListViewType {
 
 #line 128 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
 #line 128 "pyarrow/lib.pxd"
-   arrow::FixedSizeListType const *list_type;
+   arrow::LargeListViewType const *list_view_type;
 
 #line 128 "pyarrow/lib.pxd"
 };
 
 #line 128 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":133
  * 
  * 
- * cdef class StructType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class MapType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CStructType* struct_type
+ *         const CMapType* map_type
  */
 
 #line 133 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_StructType {
+struct __pyx_obj_7pyarrow_3lib_MapType {
 
 #line 133 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
 #line 133 "pyarrow/lib.pxd"
-   arrow::StructType const *struct_type;
+   arrow::MapType const *map_type;
 
 #line 133 "pyarrow/lib.pxd"
 };
 
 #line 133 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":140
+/* "pyarrow/lib.pxd":138
+ * 
+ * 
+ * cdef class FixedSizeListType(DataType):             # <<<<<<<<<<<<<<
+ *     cdef:
+ *         const CFixedSizeListType* list_type
+ */
+
+#line 138 "pyarrow/lib.pxd"
+struct __pyx_obj_7pyarrow_3lib_FixedSizeListType {
+
+#line 138 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
+
+#line 138 "pyarrow/lib.pxd"
+   arrow::FixedSizeListType const *list_type;
+
+#line 138 "pyarrow/lib.pxd"
+};
+
+#line 138 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":143
+ * 
+ * 
+ * cdef class StructType(DataType):             # <<<<<<<<<<<<<<
+ *     cdef:
+ *         const CStructType* struct_type
+ */
+
+#line 143 "pyarrow/lib.pxd"
+struct __pyx_obj_7pyarrow_3lib_StructType {
+
+#line 143 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
+
+#line 143 "pyarrow/lib.pxd"
+   arrow::StructType const *struct_type;
+
+#line 143 "pyarrow/lib.pxd"
+};
+
+#line 143 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":150
  * 
  * 
  * cdef class DictionaryMemo(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         # Even though the CDictionaryMemo instance is private, we allocate
  */
 
-#line 140 "pyarrow/lib.pxd"
+#line 150 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_DictionaryMemo {
 
-#line 140 "pyarrow/lib.pxd"
+#line 150 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 140 "pyarrow/lib.pxd"
+#line 150 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::ipc::DictionaryMemo>  sp_memo;
 
-#line 140 "pyarrow/lib.pxd"
+#line 150 "pyarrow/lib.pxd"
    arrow::ipc::DictionaryMemo *memo;
 
-#line 140 "pyarrow/lib.pxd"
+#line 150 "pyarrow/lib.pxd"
 };
 
-#line 140 "pyarrow/lib.pxd"
+#line 150 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":148
+/* "pyarrow/lib.pxd":158
  * 
  * 
  * cdef class DictionaryType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CDictionaryType* dict_type
  */
 
-#line 148 "pyarrow/lib.pxd"
+#line 158 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_DictionaryType {
 
-#line 148 "pyarrow/lib.pxd"
+#line 158 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
-#line 148 "pyarrow/lib.pxd"
+#line 158 "pyarrow/lib.pxd"
    arrow::DictionaryType const *dict_type;
 
-#line 148 "pyarrow/lib.pxd"
+#line 158 "pyarrow/lib.pxd"
 };
 
-#line 148 "pyarrow/lib.pxd"
+#line 158 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":153
+/* "pyarrow/lib.pxd":163
  * 
  * 
  * cdef class TimestampType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CTimestampType* ts_type
  */
 
-#line 153 "pyarrow/lib.pxd"
+#line 163 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_TimestampType {
 
-#line 153 "pyarrow/lib.pxd"
+#line 163 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
-#line 153 "pyarrow/lib.pxd"
+#line 163 "pyarrow/lib.pxd"
    arrow::TimestampType const *ts_type;
 
-#line 153 "pyarrow/lib.pxd"
+#line 163 "pyarrow/lib.pxd"
 };
 
-#line 153 "pyarrow/lib.pxd"
+#line 163 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":158
+/* "pyarrow/lib.pxd":168
  * 
  * 
  * cdef class Time32Type(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CTime32Type* time_type
  */
 
-#line 158 "pyarrow/lib.pxd"
+#line 168 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Time32Type {
 
-#line 158 "pyarrow/lib.pxd"
+#line 168 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
-#line 158 "pyarrow/lib.pxd"
+#line 168 "pyarrow/lib.pxd"
    arrow::Time32Type const *time_type;
 
-#line 158 "pyarrow/lib.pxd"
+#line 168 "pyarrow/lib.pxd"
 };
 
-#line 158 "pyarrow/lib.pxd"
+#line 168 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":163
+/* "pyarrow/lib.pxd":173
  * 
  * 
  * cdef class Time64Type(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CTime64Type* time_type
  */
 
-#line 163 "pyarrow/lib.pxd"
+#line 173 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Time64Type {
 
-#line 163 "pyarrow/lib.pxd"
+#line 173 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
-#line 163 "pyarrow/lib.pxd"
+#line 173 "pyarrow/lib.pxd"
    arrow::Time64Type const *time_type;
 
-#line 163 "pyarrow/lib.pxd"
+#line 173 "pyarrow/lib.pxd"
 };
 
-#line 163 "pyarrow/lib.pxd"
+#line 173 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":168
+/* "pyarrow/lib.pxd":178
  * 
  * 
  * cdef class DurationType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CDurationType* duration_type
  */
 
-#line 168 "pyarrow/lib.pxd"
+#line 178 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_DurationType {
 
-#line 168 "pyarrow/lib.pxd"
+#line 178 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
-#line 168 "pyarrow/lib.pxd"
+#line 178 "pyarrow/lib.pxd"
    arrow::DurationType const *duration_type;
 
-#line 168 "pyarrow/lib.pxd"
+#line 178 "pyarrow/lib.pxd"
 };
 
-#line 168 "pyarrow/lib.pxd"
+#line 178 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":173
+/* "pyarrow/lib.pxd":183
  * 
  * 
  * cdef class FixedSizeBinaryType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CFixedSizeBinaryType* fixed_size_binary_type
  */
 
-#line 173 "pyarrow/lib.pxd"
+#line 183 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType {
 
-#line 173 "pyarrow/lib.pxd"
+#line 183 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
-#line 173 "pyarrow/lib.pxd"
+#line 183 "pyarrow/lib.pxd"
    arrow::FixedSizeBinaryType const *fixed_size_binary_type;
 
-#line 173 "pyarrow/lib.pxd"
+#line 183 "pyarrow/lib.pxd"
 };
 
-#line 173 "pyarrow/lib.pxd"
+#line 183 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":178
+/* "pyarrow/lib.pxd":188
  * 
  * 
  * cdef class Decimal128Type(FixedSizeBinaryType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CDecimal128Type* decimal128_type
  */
 
-#line 178 "pyarrow/lib.pxd"
+#line 188 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Decimal128Type {
 
-#line 178 "pyarrow/lib.pxd"
+#line 188 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType __pyx_base;
 
-#line 178 "pyarrow/lib.pxd"
+#line 188 "pyarrow/lib.pxd"
    arrow::Decimal128Type const *decimal128_type;
 
-#line 178 "pyarrow/lib.pxd"
+#line 188 "pyarrow/lib.pxd"
 };
 
-#line 178 "pyarrow/lib.pxd"
+#line 188 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":183
+/* "pyarrow/lib.pxd":193
  * 
  * 
  * cdef class Decimal256Type(FixedSizeBinaryType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CDecimal256Type* decimal256_type
  */
 
-#line 183 "pyarrow/lib.pxd"
+#line 193 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Decimal256Type {
 
-#line 183 "pyarrow/lib.pxd"
+#line 193 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType __pyx_base;
 
-#line 183 "pyarrow/lib.pxd"
+#line 193 "pyarrow/lib.pxd"
    arrow::Decimal256Type const *decimal256_type;
 
-#line 183 "pyarrow/lib.pxd"
+#line 193 "pyarrow/lib.pxd"
 };
 
-#line 183 "pyarrow/lib.pxd"
+#line 193 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":188
+/* "pyarrow/lib.pxd":198
  * 
  * 
  * cdef class RunEndEncodedType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CRunEndEncodedType* run_end_encoded_type
  */
 
-#line 188 "pyarrow/lib.pxd"
+#line 198 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_RunEndEncodedType {
 
-#line 188 "pyarrow/lib.pxd"
+#line 198 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
-#line 188 "pyarrow/lib.pxd"
+#line 198 "pyarrow/lib.pxd"
    arrow::RunEndEncodedType const *run_end_encoded_type;
 
-#line 188 "pyarrow/lib.pxd"
+#line 198 "pyarrow/lib.pxd"
 };
 
-#line 188 "pyarrow/lib.pxd"
+#line 198 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":193
+/* "pyarrow/lib.pxd":203
  * 
  * 
  * cdef class BaseExtensionType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CExtensionType* ext_type
  */
 
-#line 193 "pyarrow/lib.pxd"
+#line 203 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_BaseExtensionType {
 
-#line 193 "pyarrow/lib.pxd"
+#line 203 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType __pyx_base;
 
-#line 193 "pyarrow/lib.pxd"
+#line 203 "pyarrow/lib.pxd"
    arrow::ExtensionType const *ext_type;
 
-#line 193 "pyarrow/lib.pxd"
+#line 203 "pyarrow/lib.pxd"
 };
 
-#line 193 "pyarrow/lib.pxd"
+#line 203 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":198
+/* "pyarrow/lib.pxd":208
  * 
  * 
  * cdef class ExtensionType(BaseExtensionType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CPyExtensionType* cpy_ext_type
  */
 
-#line 198 "pyarrow/lib.pxd"
+#line 208 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_ExtensionType {
 
-#line 198 "pyarrow/lib.pxd"
+#line 208 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_BaseExtensionType __pyx_base;
 
-#line 198 "pyarrow/lib.pxd"
+#line 208 "pyarrow/lib.pxd"
    arrow::py::PyExtensionType const *cpy_ext_type;
 
-#line 198 "pyarrow/lib.pxd"
+#line 208 "pyarrow/lib.pxd"
 };
 
-#line 198 "pyarrow/lib.pxd"
+#line 208 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":203
+/* "pyarrow/lib.pxd":213
  * 
  * 
  * cdef class FixedShapeTensorType(BaseExtensionType):             # <<<<<<<<<<<<<<
  *     cdef:
  *         const CFixedShapeTensorType* tensor_ext_type
  */
 
-#line 203 "pyarrow/lib.pxd"
+#line 213 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_FixedShapeTensorType {
 
-#line 203 "pyarrow/lib.pxd"
+#line 213 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_BaseExtensionType __pyx_base;
 
-#line 203 "pyarrow/lib.pxd"
+#line 213 "pyarrow/lib.pxd"
    arrow::extension::FixedShapeTensorType const *tensor_ext_type;
 
-#line 203 "pyarrow/lib.pxd"
+#line 213 "pyarrow/lib.pxd"
 };
 
-#line 203 "pyarrow/lib.pxd"
+#line 213 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":208
+/* "pyarrow/lib.pxd":218
  * 
  * 
  * cdef class PyExtensionType(ExtensionType):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 208 "pyarrow/lib.pxd"
+#line 218 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_PyExtensionType {
 
-#line 208 "pyarrow/lib.pxd"
+#line 218 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_ExtensionType __pyx_base;
 
-#line 208 "pyarrow/lib.pxd"
+#line 218 "pyarrow/lib.pxd"
 };
 
-#line 208 "pyarrow/lib.pxd"
+#line 218 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":212
+/* "pyarrow/lib.pxd":222
  * 
  * 
  * cdef class _Metadata(_Weakrefable):             # <<<<<<<<<<<<<<
  *     # required because KeyValueMetadata also extends collections.abc.Mapping
  *     # and the first parent class must be an extension type
  */
 
-#line 212 "pyarrow/lib.pxd"
+#line 222 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib__Metadata {
 
-#line 212 "pyarrow/lib.pxd"
+#line 222 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 212 "pyarrow/lib.pxd"
+#line 222 "pyarrow/lib.pxd"
 };
 
-#line 212 "pyarrow/lib.pxd"
+#line 222 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":218
+/* "pyarrow/lib.pxd":228
  * 
  * 
  * cdef class KeyValueMetadata(_Metadata):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[const CKeyValueMetadata] wrapped
  */
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata {
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Metadata __pyx_base;
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_KeyValueMetadata *__pyx_vtab;
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::KeyValueMetadata const >  wrapped;
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
    arrow::KeyValueMetadata const *metadata;
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
 };
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":230
+/* "pyarrow/lib.pxd":240
  * 
  * 
  * cdef class Field(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CField] sp_field
  */
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Field {
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Field *__pyx_vtab;
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::Field>  sp_field;
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
    arrow::Field *field;
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType *type;
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
 };
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":241
+/* "pyarrow/lib.pxd":251
  * 
  * 
  * cdef class Schema(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSchema] sp_schema
  */
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Schema {
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Schema *__pyx_vtab;
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::Schema>  sp_schema;
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
    arrow::Schema *schema;
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
 };
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":250
+/* "pyarrow/lib.pxd":260
  * 
  * 
  * cdef class Scalar(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CScalar] wrapped
  */
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Scalar {
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Scalar *__pyx_vtab;
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::Scalar>  wrapped;
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
 };
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":262
+/* "pyarrow/lib.pxd":272
  * 
  * 
  * cdef class _PandasConvertible(_Weakrefable):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 262 "pyarrow/lib.pxd"
+#line 272 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib__PandasConvertible {
 
-#line 262 "pyarrow/lib.pxd"
+#line 272 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 262 "pyarrow/lib.pxd"
+#line 272 "pyarrow/lib.pxd"
 };
 
-#line 262 "pyarrow/lib.pxd"
+#line 272 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":266
+/* "pyarrow/lib.pxd":276
  * 
  * 
  * cdef class Array(_PandasConvertible):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CArray] sp_array
  */
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Array {
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__PandasConvertible __pyx_base;
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Array *__pyx_vtab;
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::Array>  sp_array;
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
    arrow::Array *ap;
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType *type;
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
   PyObject *_name;
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
 };
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":281
+/* "pyarrow/lib.pxd":291
  * 
  * 
  * cdef class Tensor(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CTensor] sp_tensor
  */
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Tensor {
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Tensor *__pyx_vtab;
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::Tensor>  sp_tensor;
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
    arrow::Tensor *tp;
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType *type;
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
+  PyObject *_ssize_t_shape;
+
+#line 291 "pyarrow/lib.pxd"
+  PyObject *_ssize_t_strides;
+
+#line 291 "pyarrow/lib.pxd"
 };
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":292
+/* "pyarrow/lib.pxd":304
  * 
  * 
  * cdef class SparseCSRMatrix(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSparseCSRMatrix] sp_sparse_tensor
  */
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix {
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSRMatrix *__pyx_vtab;
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::SparseCSRMatrix>  sp_sparse_tensor;
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
    arrow::SparseCSRMatrix *stp;
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType *type;
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
 };
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":303
+/* "pyarrow/lib.pxd":315
  * 
  * 
  * cdef class SparseCSCMatrix(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSparseCSCMatrix] sp_sparse_tensor
  */
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix {
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSCMatrix *__pyx_vtab;
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::SparseCSCMatrix>  sp_sparse_tensor;
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
    arrow::SparseCSCMatrix *stp;
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType *type;
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
 };
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":314
+/* "pyarrow/lib.pxd":326
  * 
  * 
  * cdef class SparseCOOTensor(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSparseCOOTensor] sp_sparse_tensor
  */
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor {
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_SparseCOOTensor *__pyx_vtab;
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::SparseCOOTensor>  sp_sparse_tensor;
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
    arrow::SparseCOOTensor *stp;
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType *type;
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
 };
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":325
+/* "pyarrow/lib.pxd":337
  * 
  * 
  * cdef class SparseCSFTensor(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSparseCSFTensor] sp_sparse_tensor
  */
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor {
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSFTensor *__pyx_vtab;
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::SparseCSFTensor>  sp_sparse_tensor;
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
    arrow::SparseCSFTensor *stp;
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_DataType *type;
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
 };
 
-#line 325 "pyarrow/lib.pxd"
-
-
-/* "pyarrow/lib.pxd":336
- * 
- * 
- * cdef class NullArray(Array):             # <<<<<<<<<<<<<<
- *     pass
- * 
- */
-
-#line 336 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_NullArray {
-
-#line 336 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
-
-#line 336 "pyarrow/lib.pxd"
-};
-
-#line 336 "pyarrow/lib.pxd"
-
-
-/* "pyarrow/lib.pxd":340
- * 
- * 
- * cdef class BooleanArray(Array):             # <<<<<<<<<<<<<<
- *     pass
- * 
- */
-
-#line 340 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_BooleanArray {
-
-#line 340 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
-
-#line 340 "pyarrow/lib.pxd"
-};
-
-#line 340 "pyarrow/lib.pxd"
-
-
-/* "pyarrow/lib.pxd":344
- * 
- * 
- * cdef class NumericArray(Array):             # <<<<<<<<<<<<<<
- *     pass
- * 
- */
-
-#line 344 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_NumericArray {
-
-#line 344 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
-
-#line 344 "pyarrow/lib.pxd"
-};
-
-#line 344 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":348
  * 
  * 
- * cdef class IntegerArray(NumericArray):             # <<<<<<<<<<<<<<
+ * cdef class NullArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 348 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_IntegerArray {
+struct __pyx_obj_7pyarrow_3lib_NullArray {
 
 #line 348 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_NumericArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
 #line 348 "pyarrow/lib.pxd"
 };
 
 #line 348 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":352
  * 
  * 
- * cdef class FloatingPointArray(NumericArray):             # <<<<<<<<<<<<<<
+ * cdef class BooleanArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 352 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_FloatingPointArray {
+struct __pyx_obj_7pyarrow_3lib_BooleanArray {
 
 #line 352 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_NumericArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
 #line 352 "pyarrow/lib.pxd"
 };
 
 #line 352 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":356
  * 
  * 
- * cdef class Int8Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class NumericArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 356 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_Int8Array {
+struct __pyx_obj_7pyarrow_3lib_NumericArray {
 
 #line 356 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
 #line 356 "pyarrow/lib.pxd"
 };
 
 #line 356 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":360
  * 
  * 
- * cdef class UInt8Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class IntegerArray(NumericArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 360 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_UInt8Array {
+struct __pyx_obj_7pyarrow_3lib_IntegerArray {
 
 #line 360 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_NumericArray __pyx_base;
 
 #line 360 "pyarrow/lib.pxd"
 };
 
 #line 360 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":364
  * 
  * 
- * cdef class Int16Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class FloatingPointArray(NumericArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 364 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_Int16Array {
+struct __pyx_obj_7pyarrow_3lib_FloatingPointArray {
 
 #line 364 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_NumericArray __pyx_base;
 
 #line 364 "pyarrow/lib.pxd"
 };
 
 #line 364 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":368
  * 
  * 
- * cdef class UInt16Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class Int8Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 368 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_UInt16Array {
+struct __pyx_obj_7pyarrow_3lib_Int8Array {
 
 #line 368 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 368 "pyarrow/lib.pxd"
 };
 
 #line 368 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":372
  * 
  * 
- * cdef class Int32Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class UInt8Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 372 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_Int32Array {
+struct __pyx_obj_7pyarrow_3lib_UInt8Array {
 
 #line 372 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 372 "pyarrow/lib.pxd"
 };
 
 #line 372 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":376
  * 
  * 
- * cdef class UInt32Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class Int16Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 376 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_UInt32Array {
+struct __pyx_obj_7pyarrow_3lib_Int16Array {
 
 #line 376 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 376 "pyarrow/lib.pxd"
 };
 
 #line 376 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":380
  * 
  * 
- * cdef class Int64Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class UInt16Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 380 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_Int64Array {
+struct __pyx_obj_7pyarrow_3lib_UInt16Array {
 
 #line 380 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 380 "pyarrow/lib.pxd"
 };
 
 #line 380 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":384
  * 
  * 
- * cdef class UInt64Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class Int32Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 384 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_UInt64Array {
+struct __pyx_obj_7pyarrow_3lib_Int32Array {
 
 #line 384 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 384 "pyarrow/lib.pxd"
 };
 
 #line 384 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":388
  * 
  * 
- * cdef class HalfFloatArray(FloatingPointArray):             # <<<<<<<<<<<<<<
+ * cdef class UInt32Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 388 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_HalfFloatArray {
+struct __pyx_obj_7pyarrow_3lib_UInt32Array {
 
 #line 388 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_FloatingPointArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 388 "pyarrow/lib.pxd"
 };
 
 #line 388 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":392
  * 
  * 
- * cdef class FloatArray(FloatingPointArray):             # <<<<<<<<<<<<<<
+ * cdef class Int64Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 392 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_FloatArray {
+struct __pyx_obj_7pyarrow_3lib_Int64Array {
 
 #line 392 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_FloatingPointArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 392 "pyarrow/lib.pxd"
 };
 
 #line 392 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":396
  * 
  * 
- * cdef class DoubleArray(FloatingPointArray):             # <<<<<<<<<<<<<<
+ * cdef class UInt64Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 396 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_DoubleArray {
+struct __pyx_obj_7pyarrow_3lib_UInt64Array {
 
 #line 396 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_FloatingPointArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 396 "pyarrow/lib.pxd"
 };
 
 #line 396 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":400
  * 
  * 
- * cdef class FixedSizeBinaryArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class HalfFloatArray(FloatingPointArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 400 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray {
+struct __pyx_obj_7pyarrow_3lib_HalfFloatArray {
 
 #line 400 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_FloatingPointArray __pyx_base;
 
 #line 400 "pyarrow/lib.pxd"
 };
 
 #line 400 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":404
  * 
  * 
- * cdef class Decimal128Array(FixedSizeBinaryArray):             # <<<<<<<<<<<<<<
+ * cdef class FloatArray(FloatingPointArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 404 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_Decimal128Array {
+struct __pyx_obj_7pyarrow_3lib_FloatArray {
 
 #line 404 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_FloatingPointArray __pyx_base;
 
 #line 404 "pyarrow/lib.pxd"
 };
 
 #line 404 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":408
  * 
  * 
- * cdef class Decimal256Array(FixedSizeBinaryArray):             # <<<<<<<<<<<<<<
+ * cdef class DoubleArray(FloatingPointArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 408 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_Decimal256Array {
+struct __pyx_obj_7pyarrow_3lib_DoubleArray {
 
 #line 408 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_FloatingPointArray __pyx_base;
 
 #line 408 "pyarrow/lib.pxd"
 };
 
 #line 408 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":412
  * 
  * 
- * cdef class StructArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class FixedSizeBinaryArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 412 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_StructArray {
+struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray {
 
 #line 412 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
 #line 412 "pyarrow/lib.pxd"
 };
 
 #line 412 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":416
  * 
  * 
- * cdef class BaseListArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class Decimal128Array(FixedSizeBinaryArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 416 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_BaseListArray {
+struct __pyx_obj_7pyarrow_3lib_Decimal128Array {
 
 #line 416 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray __pyx_base;
 
 #line 416 "pyarrow/lib.pxd"
 };
 
 #line 416 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":420
  * 
  * 
- * cdef class ListArray(BaseListArray):             # <<<<<<<<<<<<<<
+ * cdef class Decimal256Array(FixedSizeBinaryArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 420 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_ListArray {
+struct __pyx_obj_7pyarrow_3lib_Decimal256Array {
 
 #line 420 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_BaseListArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray __pyx_base;
 
 #line 420 "pyarrow/lib.pxd"
 };
 
 #line 420 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":424
  * 
  * 
- * cdef class LargeListArray(BaseListArray):             # <<<<<<<<<<<<<<
+ * cdef class StructArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 424 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_LargeListArray {
+struct __pyx_obj_7pyarrow_3lib_StructArray {
 
 #line 424 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_BaseListArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
 #line 424 "pyarrow/lib.pxd"
 };
 
 #line 424 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":428
  * 
  * 
- * cdef class MapArray(ListArray):             # <<<<<<<<<<<<<<
+ * cdef class BaseListArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 428 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_MapArray {
+struct __pyx_obj_7pyarrow_3lib_BaseListArray {
 
 #line 428 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_ListArray __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
 #line 428 "pyarrow/lib.pxd"
 };
 
 #line 428 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":432
  * 
  * 
- * cdef class FixedSizeListArray(BaseListArray):             # <<<<<<<<<<<<<<
+ * cdef class ListArray(BaseListArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 432 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray {
+struct __pyx_obj_7pyarrow_3lib_ListArray {
 
 #line 432 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_BaseListArray __pyx_base;
 
 #line 432 "pyarrow/lib.pxd"
 };
 
 #line 432 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":436
  * 
  * 
- * cdef class UnionArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class LargeListArray(BaseListArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 436 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_UnionArray {
+struct __pyx_obj_7pyarrow_3lib_LargeListArray {
 
 #line 436 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
+  struct __pyx_obj_7pyarrow_3lib_BaseListArray __pyx_base;
 
 #line 436 "pyarrow/lib.pxd"
 };
 
 #line 436 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":440
  * 
  * 
- * cdef class StringArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class ListViewArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 440 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_StringArray {
+struct __pyx_obj_7pyarrow_3lib_ListViewArray {
 
 #line 440 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
 #line 440 "pyarrow/lib.pxd"
 };
 
 #line 440 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":444
  * 
  * 
- * cdef class BinaryArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class LargeListViewArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 444 "pyarrow/lib.pxd"
-struct __pyx_obj_7pyarrow_3lib_BinaryArray {
+struct __pyx_obj_7pyarrow_3lib_LargeListViewArray {
 
 #line 444 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
 #line 444 "pyarrow/lib.pxd"
 };
 
 #line 444 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":448
  * 
  * 
+ * cdef class MapArray(ListArray):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 448 "pyarrow/lib.pxd"
+struct __pyx_obj_7pyarrow_3lib_MapArray {
+
+#line 448 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_ListArray __pyx_base;
+
+#line 448 "pyarrow/lib.pxd"
+};
+
+#line 448 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":452
+ * 
+ * 
+ * cdef class FixedSizeListArray(BaseListArray):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 452 "pyarrow/lib.pxd"
+struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray {
+
+#line 452 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_BaseListArray __pyx_base;
+
+#line 452 "pyarrow/lib.pxd"
+};
+
+#line 452 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":456
+ * 
+ * 
+ * cdef class UnionArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 456 "pyarrow/lib.pxd"
+struct __pyx_obj_7pyarrow_3lib_UnionArray {
+
+#line 456 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
+
+#line 456 "pyarrow/lib.pxd"
+};
+
+#line 456 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":460
+ * 
+ * 
+ * cdef class StringArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 460 "pyarrow/lib.pxd"
+struct __pyx_obj_7pyarrow_3lib_StringArray {
+
+#line 460 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
+
+#line 460 "pyarrow/lib.pxd"
+};
+
+#line 460 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":464
+ * 
+ * 
+ * cdef class BinaryArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 464 "pyarrow/lib.pxd"
+struct __pyx_obj_7pyarrow_3lib_BinaryArray {
+
+#line 464 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
+
+#line 464 "pyarrow/lib.pxd"
+};
+
+#line 464 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":468
+ * 
+ * 
+ * cdef class StringViewArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 468 "pyarrow/lib.pxd"
+struct __pyx_obj_7pyarrow_3lib_StringViewArray {
+
+#line 468 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
+
+#line 468 "pyarrow/lib.pxd"
+};
+
+#line 468 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":472
+ * 
+ * 
+ * cdef class BinaryViewArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 472 "pyarrow/lib.pxd"
+struct __pyx_obj_7pyarrow_3lib_BinaryViewArray {
+
+#line 472 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
+
+#line 472 "pyarrow/lib.pxd"
+};
+
+#line 472 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":476
+ * 
+ * 
  * cdef class DictionaryArray(Array):             # <<<<<<<<<<<<<<
  *     cdef:
  *         object _indices, _dictionary
  */
 
-#line 448 "pyarrow/lib.pxd"
+#line 476 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_DictionaryArray {
 
-#line 448 "pyarrow/lib.pxd"
+#line 476 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
-#line 448 "pyarrow/lib.pxd"
+#line 476 "pyarrow/lib.pxd"
   PyObject *_indices;
 
-#line 448 "pyarrow/lib.pxd"
+#line 476 "pyarrow/lib.pxd"
   PyObject *_dictionary;
 
-#line 448 "pyarrow/lib.pxd"
+#line 476 "pyarrow/lib.pxd"
 };
 
-#line 448 "pyarrow/lib.pxd"
+#line 476 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":453
+/* "pyarrow/lib.pxd":481
  * 
  * 
  * cdef class ExtensionArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_ExtensionArray {
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
 };
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":457
+/* "pyarrow/lib.pxd":485
  * 
  * 
  * cdef class MonthDayNanoIntervalArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray {
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_Array __pyx_base;
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
 };
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":465
+/* "pyarrow/lib.pxd":493
  * 
  * 
  * cdef class ChunkedArray(_PandasConvertible):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CChunkedArray] sp_chunked_array
  */
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_ChunkedArray {
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__PandasConvertible __pyx_base;
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_ChunkedArray *__pyx_vtab;
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::ChunkedArray>  sp_chunked_array;
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
    arrow::ChunkedArray *chunked_array;
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
   PyObject *_name;
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
 };
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":478
+/* "pyarrow/lib.pxd":506
  * 
  * 
  * cdef class _Tabular(_PandasConvertible):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 478 "pyarrow/lib.pxd"
+#line 506 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib__Tabular {
 
-#line 478 "pyarrow/lib.pxd"
+#line 506 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__PandasConvertible __pyx_base;
 
-#line 478 "pyarrow/lib.pxd"
+#line 506 "pyarrow/lib.pxd"
 };
 
-#line 478 "pyarrow/lib.pxd"
+#line 506 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":482
+/* "pyarrow/lib.pxd":510
  * 
  * 
  * cdef class Table(_Tabular):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CTable] sp_table
  */
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Table {
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Tabular __pyx_base;
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Table *__pyx_vtab;
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::Table>  sp_table;
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
    arrow::Table *table;
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
 };
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":490
+/* "pyarrow/lib.pxd":518
  * 
  * 
  * cdef class RecordBatch(_Tabular):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CRecordBatch] sp_batch
  */
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_RecordBatch {
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Tabular __pyx_base;
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_RecordBatch *__pyx_vtab;
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::RecordBatch>  sp_batch;
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
    arrow::RecordBatch *batch;
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_Schema *_schema;
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
 };
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":499
+/* "pyarrow/lib.pxd":527
  * 
  * 
  * cdef class Buffer(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CBuffer] buffer
  */
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Buffer {
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Buffer *__pyx_vtab;
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::Buffer>  buffer;
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
   Py_ssize_t shape[1];
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
   Py_ssize_t strides[1];
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
 };
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":509
+/* "pyarrow/lib.pxd":537
  * 
  * 
  * cdef class ResizableBuffer(Buffer):             # <<<<<<<<<<<<<<
  * 
  *     cdef void init_rz(self, const shared_ptr[CResizableBuffer]& buffer)
  */
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_ResizableBuffer {
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_Buffer __pyx_base;
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
 };
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":514
+/* "pyarrow/lib.pxd":542
  * 
  * 
  * cdef class NativeFile(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CInputStream] input_stream
  */
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_NativeFile {
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile *__pyx_vtab;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::io::InputStream>  input_stream;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::io::RandomAccessFile>  random_access;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::io::OutputStream>  output_stream;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   int is_readable;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   int is_writable;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   int is_seekable;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   int _is_appending;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   int own_file;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
 };
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":538
+/* "pyarrow/lib.pxd":566
  * 
  * 
  * cdef class BufferedInputStream(NativeFile):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_BufferedInputStream {
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_NativeFile __pyx_base;
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
 };
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":542
+/* "pyarrow/lib.pxd":570
  * 
  * 
  * cdef class BufferedOutputStream(NativeFile):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_BufferedOutputStream {
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_NativeFile __pyx_base;
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
 };
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":546
+/* "pyarrow/lib.pxd":574
  * 
  * 
  * cdef class CompressedInputStream(NativeFile):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_CompressedInputStream {
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_NativeFile __pyx_base;
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
 };
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":550
+/* "pyarrow/lib.pxd":578
  * 
  * 
  * cdef class CompressedOutputStream(NativeFile):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_CompressedOutputStream {
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib_NativeFile __pyx_base;
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
 };
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":554
+/* "pyarrow/lib.pxd":582
  * 
  * 
  * cdef class _CRecordBatchWriter(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         SharedPtrNoGIL[CRecordBatchWriter] writer
  */
 
-#line 554 "pyarrow/lib.pxd"
+#line 582 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib__CRecordBatchWriter {
 
-#line 554 "pyarrow/lib.pxd"
+#line 582 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 554 "pyarrow/lib.pxd"
+#line 582 "pyarrow/lib.pxd"
   arrow::py::SharedPtrNoGIL< arrow::ipc::RecordBatchWriter>  writer;
 
-#line 554 "pyarrow/lib.pxd"
+#line 582 "pyarrow/lib.pxd"
 };
 
-#line 554 "pyarrow/lib.pxd"
+#line 582 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":559
+/* "pyarrow/lib.pxd":587
  * 
  * 
  * cdef class RecordBatchReader(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         SharedPtrNoGIL[CRecordBatchReader] reader
  */
 
-#line 559 "pyarrow/lib.pxd"
+#line 587 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_RecordBatchReader {
 
-#line 559 "pyarrow/lib.pxd"
+#line 587 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 559 "pyarrow/lib.pxd"
+#line 587 "pyarrow/lib.pxd"
   arrow::py::SharedPtrNoGIL< arrow::RecordBatchReader>  reader;
 
-#line 559 "pyarrow/lib.pxd"
+#line 587 "pyarrow/lib.pxd"
 };
 
-#line 559 "pyarrow/lib.pxd"
+#line 587 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":564
+/* "pyarrow/lib.pxd":592
  * 
  * 
  * cdef class CacheOptions(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         CCacheOptions wrapped
  */
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_CacheOptions {
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_CacheOptions *__pyx_vtab;
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
   arrow::io::CacheOptions wrapped;
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
 };
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":576
+/* "pyarrow/lib.pxd":604
  * 
  * 
  * cdef class Codec(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CCodec] wrapped
  */
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_Codec {
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
   struct __pyx_obj_7pyarrow_3lib__Weakrefable __pyx_base;
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Codec *__pyx_vtab;
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::util::Codec>  wrapped;
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
 };
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":584
+/* "pyarrow/lib.pxd":612
  * 
  * # This class is only used internally for now
  * cdef class StopToken:             # <<<<<<<<<<<<<<
  *     cdef:
  *         CStopToken stop_token
  */
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
 struct __pyx_obj_7pyarrow_3lib_StopToken {
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
   PyObject_HEAD
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_StopToken *__pyx_vtab;
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
   arrow::StopToken stop_token;
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
 };
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/_parquet.pxd":564
  *         const COutputStream* sink)
  * 
  * cdef class FileEncryptionProperties:             # <<<<<<<<<<<<<<
  *     """File-level encryption properties for the low-level API"""
@@ -4845,1883 +4985,2039 @@
 
 #line 118 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":123
  * 
  * 
- * cdef class MapType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class ListViewType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CMapType* map_type
+ *         const CListViewType* list_view_type
  */
 
 #line 123 "pyarrow/lib.pxd"
 
 
 #line 123 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_MapType {
+struct __pyx_vtabstruct_7pyarrow_3lib_ListViewType {
 
 #line 123 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 123 "pyarrow/lib.pxd"
 };
 
 #line 123 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_MapType *__pyx_vtabptr_7pyarrow_3lib_MapType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_ListViewType *__pyx_vtabptr_7pyarrow_3lib_ListViewType;
 
 #line 123 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":128
  * 
  * 
- * cdef class FixedSizeListType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class LargeListViewType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CFixedSizeListType* list_type
+ *         const CLargeListViewType* list_view_type
  */
 
 #line 128 "pyarrow/lib.pxd"
 
 
 #line 128 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListType {
+struct __pyx_vtabstruct_7pyarrow_3lib_LargeListViewType {
 
 #line 128 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 128 "pyarrow/lib.pxd"
 };
 
 #line 128 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListType *__pyx_vtabptr_7pyarrow_3lib_FixedSizeListType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_LargeListViewType *__pyx_vtabptr_7pyarrow_3lib_LargeListViewType;
 
 #line 128 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":133
  * 
  * 
- * cdef class StructType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class MapType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CStructType* struct_type
+ *         const CMapType* map_type
  */
 
 #line 133 "pyarrow/lib.pxd"
 
 
 #line 133 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_StructType {
+struct __pyx_vtabstruct_7pyarrow_3lib_MapType {
 
 #line 133 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 133 "pyarrow/lib.pxd"
-  struct __pyx_obj_7pyarrow_3lib_Field *(*field_by_name)(struct __pyx_obj_7pyarrow_3lib_StructType *, PyObject *);
-
-#line 133 "pyarrow/lib.pxd"
 };
 
 #line 133 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_StructType *__pyx_vtabptr_7pyarrow_3lib_StructType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_MapType *__pyx_vtabptr_7pyarrow_3lib_MapType;
 
 #line 133 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":148
+/* "pyarrow/lib.pxd":138
  * 
  * 
- * cdef class DictionaryType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class FixedSizeListType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CDictionaryType* dict_type
+ *         const CFixedSizeListType* list_type
  */
 
-#line 148 "pyarrow/lib.pxd"
+#line 138 "pyarrow/lib.pxd"
 
 
-#line 148 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryType {
+#line 138 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListType {
 
-#line 148 "pyarrow/lib.pxd"
+#line 138 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
-#line 148 "pyarrow/lib.pxd"
+#line 138 "pyarrow/lib.pxd"
 };
 
-#line 148 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryType *__pyx_vtabptr_7pyarrow_3lib_DictionaryType;
+#line 138 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListType *__pyx_vtabptr_7pyarrow_3lib_FixedSizeListType;
 
-#line 148 "pyarrow/lib.pxd"
+#line 138 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":153
+/* "pyarrow/lib.pxd":143
  * 
  * 
- * cdef class TimestampType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class StructType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CTimestampType* ts_type
+ *         const CStructType* struct_type
  */
 
-#line 153 "pyarrow/lib.pxd"
+#line 143 "pyarrow/lib.pxd"
 
 
-#line 153 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_TimestampType {
+#line 143 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_StructType {
 
-#line 153 "pyarrow/lib.pxd"
+#line 143 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
-#line 153 "pyarrow/lib.pxd"
+#line 143 "pyarrow/lib.pxd"
+  struct __pyx_obj_7pyarrow_3lib_Field *(*field_by_name)(struct __pyx_obj_7pyarrow_3lib_StructType *, PyObject *);
+
+#line 143 "pyarrow/lib.pxd"
 };
 
-#line 153 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_TimestampType *__pyx_vtabptr_7pyarrow_3lib_TimestampType;
+#line 143 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_StructType *__pyx_vtabptr_7pyarrow_3lib_StructType;
 
-#line 153 "pyarrow/lib.pxd"
+#line 143 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":158
  * 
  * 
- * cdef class Time32Type(DataType):             # <<<<<<<<<<<<<<
+ * cdef class DictionaryType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CTime32Type* time_type
+ *         const CDictionaryType* dict_type
  */
 
 #line 158 "pyarrow/lib.pxd"
 
 
 #line 158 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Time32Type {
+struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryType {
 
 #line 158 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 158 "pyarrow/lib.pxd"
 };
 
 #line 158 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Time32Type *__pyx_vtabptr_7pyarrow_3lib_Time32Type;
+static struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryType *__pyx_vtabptr_7pyarrow_3lib_DictionaryType;
 
 #line 158 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":163
  * 
  * 
- * cdef class Time64Type(DataType):             # <<<<<<<<<<<<<<
+ * cdef class TimestampType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CTime64Type* time_type
+ *         const CTimestampType* ts_type
  */
 
 #line 163 "pyarrow/lib.pxd"
 
 
 #line 163 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Time64Type {
+struct __pyx_vtabstruct_7pyarrow_3lib_TimestampType {
 
 #line 163 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 163 "pyarrow/lib.pxd"
 };
 
 #line 163 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Time64Type *__pyx_vtabptr_7pyarrow_3lib_Time64Type;
+static struct __pyx_vtabstruct_7pyarrow_3lib_TimestampType *__pyx_vtabptr_7pyarrow_3lib_TimestampType;
 
 #line 163 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":168
  * 
  * 
- * cdef class DurationType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class Time32Type(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CDurationType* duration_type
+ *         const CTime32Type* time_type
  */
 
 #line 168 "pyarrow/lib.pxd"
 
 
 #line 168 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_DurationType {
+struct __pyx_vtabstruct_7pyarrow_3lib_Time32Type {
 
 #line 168 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 168 "pyarrow/lib.pxd"
 };
 
 #line 168 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_DurationType *__pyx_vtabptr_7pyarrow_3lib_DurationType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Time32Type *__pyx_vtabptr_7pyarrow_3lib_Time32Type;
 
 #line 168 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":173
  * 
  * 
- * cdef class FixedSizeBinaryType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class Time64Type(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CFixedSizeBinaryType* fixed_size_binary_type
+ *         const CTime64Type* time_type
  */
 
 #line 173 "pyarrow/lib.pxd"
 
 
 #line 173 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType {
+struct __pyx_vtabstruct_7pyarrow_3lib_Time64Type {
 
 #line 173 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 173 "pyarrow/lib.pxd"
 };
 
 #line 173 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType *__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Time64Type *__pyx_vtabptr_7pyarrow_3lib_Time64Type;
 
 #line 173 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":178
  * 
  * 
- * cdef class Decimal128Type(FixedSizeBinaryType):             # <<<<<<<<<<<<<<
+ * cdef class DurationType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CDecimal128Type* decimal128_type
+ *         const CDurationType* duration_type
  */
 
 #line 178 "pyarrow/lib.pxd"
 
 
 #line 178 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Type {
+struct __pyx_vtabstruct_7pyarrow_3lib_DurationType {
 
 #line 178 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 178 "pyarrow/lib.pxd"
 };
 
 #line 178 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Type *__pyx_vtabptr_7pyarrow_3lib_Decimal128Type;
+static struct __pyx_vtabstruct_7pyarrow_3lib_DurationType *__pyx_vtabptr_7pyarrow_3lib_DurationType;
 
 #line 178 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":183
  * 
  * 
- * cdef class Decimal256Type(FixedSizeBinaryType):             # <<<<<<<<<<<<<<
+ * cdef class FixedSizeBinaryType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CDecimal256Type* decimal256_type
+ *         const CFixedSizeBinaryType* fixed_size_binary_type
  */
 
 #line 183 "pyarrow/lib.pxd"
 
 
 #line 183 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Type {
+struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType {
 
 #line 183 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 183 "pyarrow/lib.pxd"
 };
 
 #line 183 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Type *__pyx_vtabptr_7pyarrow_3lib_Decimal256Type;
+static struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType *__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryType;
 
 #line 183 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":188
  * 
  * 
- * cdef class RunEndEncodedType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class Decimal128Type(FixedSizeBinaryType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CRunEndEncodedType* run_end_encoded_type
+ *         const CDecimal128Type* decimal128_type
  */
 
 #line 188 "pyarrow/lib.pxd"
 
 
 #line 188 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_RunEndEncodedType {
+struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Type {
 
 #line 188 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType __pyx_base;
 
 #line 188 "pyarrow/lib.pxd"
 };
 
 #line 188 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_RunEndEncodedType *__pyx_vtabptr_7pyarrow_3lib_RunEndEncodedType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Type *__pyx_vtabptr_7pyarrow_3lib_Decimal128Type;
 
 #line 188 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":193
  * 
  * 
- * cdef class BaseExtensionType(DataType):             # <<<<<<<<<<<<<<
+ * cdef class Decimal256Type(FixedSizeBinaryType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CExtensionType* ext_type
+ *         const CDecimal256Type* decimal256_type
  */
 
 #line 193 "pyarrow/lib.pxd"
 
 
 #line 193 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType {
+struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Type {
 
 #line 193 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType __pyx_base;
 
 #line 193 "pyarrow/lib.pxd"
 };
 
 #line 193 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType *__pyx_vtabptr_7pyarrow_3lib_BaseExtensionType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Type *__pyx_vtabptr_7pyarrow_3lib_Decimal256Type;
 
 #line 193 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":198
  * 
  * 
- * cdef class ExtensionType(BaseExtensionType):             # <<<<<<<<<<<<<<
+ * cdef class RunEndEncodedType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CPyExtensionType* cpy_ext_type
+ *         const CRunEndEncodedType* run_end_encoded_type
  */
 
 #line 198 "pyarrow/lib.pxd"
 
 
 #line 198 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionType {
+struct __pyx_vtabstruct_7pyarrow_3lib_RunEndEncodedType {
 
 #line 198 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 198 "pyarrow/lib.pxd"
 };
 
 #line 198 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionType *__pyx_vtabptr_7pyarrow_3lib_ExtensionType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_RunEndEncodedType *__pyx_vtabptr_7pyarrow_3lib_RunEndEncodedType;
 
 #line 198 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":203
  * 
  * 
- * cdef class FixedShapeTensorType(BaseExtensionType):             # <<<<<<<<<<<<<<
+ * cdef class BaseExtensionType(DataType):             # <<<<<<<<<<<<<<
  *     cdef:
- *         const CFixedShapeTensorType* tensor_ext_type
+ *         const CExtensionType* ext_type
  */
 
 #line 203 "pyarrow/lib.pxd"
 
 
 #line 203 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_FixedShapeTensorType {
+struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType {
 
 #line 203 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_DataType __pyx_base;
 
 #line 203 "pyarrow/lib.pxd"
 };
 
 #line 203 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_FixedShapeTensorType *__pyx_vtabptr_7pyarrow_3lib_FixedShapeTensorType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType *__pyx_vtabptr_7pyarrow_3lib_BaseExtensionType;
 
 #line 203 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":208
  * 
  * 
- * cdef class PyExtensionType(ExtensionType):             # <<<<<<<<<<<<<<
- *     pass
- * 
+ * cdef class ExtensionType(BaseExtensionType):             # <<<<<<<<<<<<<<
+ *     cdef:
+ *         const CPyExtensionType* cpy_ext_type
  */
 
 #line 208 "pyarrow/lib.pxd"
 
 
 #line 208 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_PyExtensionType {
+struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionType {
 
 #line 208 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionType __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType __pyx_base;
 
 #line 208 "pyarrow/lib.pxd"
 };
 
 #line 208 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_PyExtensionType *__pyx_vtabptr_7pyarrow_3lib_PyExtensionType;
+static struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionType *__pyx_vtabptr_7pyarrow_3lib_ExtensionType;
 
 #line 208 "pyarrow/lib.pxd"
 
 
+/* "pyarrow/lib.pxd":213
+ * 
+ * 
+ * cdef class FixedShapeTensorType(BaseExtensionType):             # <<<<<<<<<<<<<<
+ *     cdef:
+ *         const CFixedShapeTensorType* tensor_ext_type
+ */
+
+#line 213 "pyarrow/lib.pxd"
+
+
+#line 213 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_FixedShapeTensorType {
+
+#line 213 "pyarrow/lib.pxd"
+  struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType __pyx_base;
+
+#line 213 "pyarrow/lib.pxd"
+};
+
+#line 213 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_FixedShapeTensorType *__pyx_vtabptr_7pyarrow_3lib_FixedShapeTensorType;
+
+#line 213 "pyarrow/lib.pxd"
+
+
 /* "pyarrow/lib.pxd":218
  * 
  * 
+ * cdef class PyExtensionType(ExtensionType):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 218 "pyarrow/lib.pxd"
+
+
+#line 218 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_PyExtensionType {
+
+#line 218 "pyarrow/lib.pxd"
+  struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionType __pyx_base;
+
+#line 218 "pyarrow/lib.pxd"
+};
+
+#line 218 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_PyExtensionType *__pyx_vtabptr_7pyarrow_3lib_PyExtensionType;
+
+#line 218 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":228
+ * 
+ * 
  * cdef class KeyValueMetadata(_Metadata):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[const CKeyValueMetadata] wrapped
  */
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
 
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_KeyValueMetadata {
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata *, std::shared_ptr< arrow::KeyValueMetadata const >  const &);
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
   PyObject *(*wrap)(std::shared_ptr< arrow::KeyValueMetadata const >  const &);
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::KeyValueMetadata const >  (*unwrap)(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata *);
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
 };
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_KeyValueMetadata *__pyx_vtabptr_7pyarrow_3lib_KeyValueMetadata;
 
-#line 218 "pyarrow/lib.pxd"
+#line 228 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":230
+/* "pyarrow/lib.pxd":240
  * 
  * 
  * cdef class Field(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CField] sp_field
  */
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
 
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_Field {
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_Field *, std::shared_ptr< arrow::Field>  const &);
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
 };
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_Field *__pyx_vtabptr_7pyarrow_3lib_Field;
 
-#line 230 "pyarrow/lib.pxd"
+#line 240 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":241
+/* "pyarrow/lib.pxd":251
  * 
  * 
  * cdef class Schema(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSchema] sp_schema
  */
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
 
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_Schema {
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_Schema *, std::vector<std::shared_ptr< arrow::Field> >  const &);
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
   void (*init_schema)(struct __pyx_obj_7pyarrow_3lib_Schema *, std::shared_ptr< arrow::Schema>  const &);
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
 };
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_Schema *__pyx_vtabptr_7pyarrow_3lib_Schema;
 
-#line 241 "pyarrow/lib.pxd"
+#line 251 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":250
+/* "pyarrow/lib.pxd":260
  * 
  * 
  * cdef class Scalar(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CScalar] wrapped
  */
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
 
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_Scalar {
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_Scalar *, std::shared_ptr< arrow::Scalar>  const &);
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
   PyObject *(*wrap)(std::shared_ptr< arrow::Scalar>  const &);
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::Scalar>  (*unwrap)(struct __pyx_obj_7pyarrow_3lib_Scalar *);
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
 };
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_Scalar *__pyx_vtabptr_7pyarrow_3lib_Scalar;
 
-#line 250 "pyarrow/lib.pxd"
+#line 260 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":266
+/* "pyarrow/lib.pxd":276
  * 
  * 
  * cdef class Array(_PandasConvertible):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CArray] sp_array
  */
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
 
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_Array {
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_Array *, std::shared_ptr< arrow::Array>  const &);
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
   PyObject *(*getitem)(struct __pyx_obj_7pyarrow_3lib_Array *, int64_t);
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
   int64_t (*length)(struct __pyx_obj_7pyarrow_3lib_Array *);
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
 };
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_Array *__pyx_vtabptr_7pyarrow_3lib_Array;
 
-#line 266 "pyarrow/lib.pxd"
+#line 276 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":281
+/* "pyarrow/lib.pxd":291
  * 
  * 
  * cdef class Tensor(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CTensor] sp_tensor
  */
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
 
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_Tensor {
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_Tensor *, std::shared_ptr< arrow::Tensor>  const &);
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
 };
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_Tensor *__pyx_vtabptr_7pyarrow_3lib_Tensor;
 
-#line 281 "pyarrow/lib.pxd"
+#line 291 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":292
+/* "pyarrow/lib.pxd":304
  * 
  * 
  * cdef class SparseCSRMatrix(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSparseCSRMatrix] sp_sparse_tensor
  */
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
 
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSRMatrix {
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix *, std::shared_ptr< arrow::SparseCSRMatrix>  const &);
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
 };
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSRMatrix *__pyx_vtabptr_7pyarrow_3lib_SparseCSRMatrix;
 
-#line 292 "pyarrow/lib.pxd"
+#line 304 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":303
+/* "pyarrow/lib.pxd":315
  * 
  * 
  * cdef class SparseCSCMatrix(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSparseCSCMatrix] sp_sparse_tensor
  */
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
 
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSCMatrix {
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix *, std::shared_ptr< arrow::SparseCSCMatrix>  const &);
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
 };
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSCMatrix *__pyx_vtabptr_7pyarrow_3lib_SparseCSCMatrix;
 
-#line 303 "pyarrow/lib.pxd"
+#line 315 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":314
+/* "pyarrow/lib.pxd":326
  * 
  * 
  * cdef class SparseCOOTensor(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSparseCOOTensor] sp_sparse_tensor
  */
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
 
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_SparseCOOTensor {
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor *, std::shared_ptr< arrow::SparseCOOTensor>  const &);
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
 };
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_SparseCOOTensor *__pyx_vtabptr_7pyarrow_3lib_SparseCOOTensor;
 
-#line 314 "pyarrow/lib.pxd"
+#line 326 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":325
+/* "pyarrow/lib.pxd":337
  * 
  * 
  * cdef class SparseCSFTensor(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CSparseCSFTensor] sp_sparse_tensor
  */
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
 
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSFTensor {
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor *, std::shared_ptr< arrow::SparseCSFTensor>  const &);
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
 };
 
-#line 325 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSFTensor *__pyx_vtabptr_7pyarrow_3lib_SparseCSFTensor;
 
-#line 325 "pyarrow/lib.pxd"
-
-
-/* "pyarrow/lib.pxd":336
- * 
- * 
- * cdef class NullArray(Array):             # <<<<<<<<<<<<<<
- *     pass
- * 
- */
-
-#line 336 "pyarrow/lib.pxd"
-
-
-#line 336 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_NullArray {
-
-#line 336 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
-
-#line 336 "pyarrow/lib.pxd"
-};
-
-#line 336 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_NullArray *__pyx_vtabptr_7pyarrow_3lib_NullArray;
-
-#line 336 "pyarrow/lib.pxd"
-
-
-/* "pyarrow/lib.pxd":340
- * 
- * 
- * cdef class BooleanArray(Array):             # <<<<<<<<<<<<<<
- *     pass
- * 
- */
-
-#line 340 "pyarrow/lib.pxd"
-
-
-#line 340 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_BooleanArray {
-
-#line 340 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
-
-#line 340 "pyarrow/lib.pxd"
-};
-
-#line 340 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_BooleanArray *__pyx_vtabptr_7pyarrow_3lib_BooleanArray;
-
-#line 340 "pyarrow/lib.pxd"
-
-
-/* "pyarrow/lib.pxd":344
- * 
- * 
- * cdef class NumericArray(Array):             # <<<<<<<<<<<<<<
- *     pass
- * 
- */
-
-#line 344 "pyarrow/lib.pxd"
-
-
-#line 344 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray {
-
-#line 344 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
-
-#line 344 "pyarrow/lib.pxd"
-};
-
-#line 344 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray *__pyx_vtabptr_7pyarrow_3lib_NumericArray;
-
-#line 344 "pyarrow/lib.pxd"
+#line 337 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":348
  * 
  * 
- * cdef class IntegerArray(NumericArray):             # <<<<<<<<<<<<<<
+ * cdef class NullArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 348 "pyarrow/lib.pxd"
 
 
 #line 348 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_NullArray {
 
 #line 348 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
 #line 348 "pyarrow/lib.pxd"
 };
 
 #line 348 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray *__pyx_vtabptr_7pyarrow_3lib_IntegerArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_NullArray *__pyx_vtabptr_7pyarrow_3lib_NullArray;
 
 #line 348 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":352
  * 
  * 
- * cdef class FloatingPointArray(NumericArray):             # <<<<<<<<<<<<<<
+ * cdef class BooleanArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 352 "pyarrow/lib.pxd"
 
 
 #line 352 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_BooleanArray {
 
 #line 352 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
 #line 352 "pyarrow/lib.pxd"
 };
 
 #line 352 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray *__pyx_vtabptr_7pyarrow_3lib_FloatingPointArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_BooleanArray *__pyx_vtabptr_7pyarrow_3lib_BooleanArray;
 
 #line 352 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":356
  * 
  * 
- * cdef class Int8Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class NumericArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 356 "pyarrow/lib.pxd"
 
 
 #line 356 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Int8Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray {
 
 #line 356 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
 #line 356 "pyarrow/lib.pxd"
 };
 
 #line 356 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Int8Array *__pyx_vtabptr_7pyarrow_3lib_Int8Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray *__pyx_vtabptr_7pyarrow_3lib_NumericArray;
 
 #line 356 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":360
  * 
  * 
- * cdef class UInt8Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class IntegerArray(NumericArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 360 "pyarrow/lib.pxd"
 
 
 #line 360 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_UInt8Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray {
 
 #line 360 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray __pyx_base;
 
 #line 360 "pyarrow/lib.pxd"
 };
 
 #line 360 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_UInt8Array *__pyx_vtabptr_7pyarrow_3lib_UInt8Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray *__pyx_vtabptr_7pyarrow_3lib_IntegerArray;
 
 #line 360 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":364
  * 
  * 
- * cdef class Int16Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class FloatingPointArray(NumericArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 364 "pyarrow/lib.pxd"
 
 
 #line 364 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Int16Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray {
 
 #line 364 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray __pyx_base;
 
 #line 364 "pyarrow/lib.pxd"
 };
 
 #line 364 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Int16Array *__pyx_vtabptr_7pyarrow_3lib_Int16Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray *__pyx_vtabptr_7pyarrow_3lib_FloatingPointArray;
 
 #line 364 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":368
  * 
  * 
- * cdef class UInt16Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class Int8Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 368 "pyarrow/lib.pxd"
 
 
 #line 368 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_UInt16Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_Int8Array {
 
 #line 368 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 368 "pyarrow/lib.pxd"
 };
 
 #line 368 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_UInt16Array *__pyx_vtabptr_7pyarrow_3lib_UInt16Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Int8Array *__pyx_vtabptr_7pyarrow_3lib_Int8Array;
 
 #line 368 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":372
  * 
  * 
- * cdef class Int32Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class UInt8Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 372 "pyarrow/lib.pxd"
 
 
 #line 372 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Int32Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_UInt8Array {
 
 #line 372 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 372 "pyarrow/lib.pxd"
 };
 
 #line 372 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Int32Array *__pyx_vtabptr_7pyarrow_3lib_Int32Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_UInt8Array *__pyx_vtabptr_7pyarrow_3lib_UInt8Array;
 
 #line 372 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":376
  * 
  * 
- * cdef class UInt32Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class Int16Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 376 "pyarrow/lib.pxd"
 
 
 #line 376 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_UInt32Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_Int16Array {
 
 #line 376 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 376 "pyarrow/lib.pxd"
 };
 
 #line 376 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_UInt32Array *__pyx_vtabptr_7pyarrow_3lib_UInt32Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Int16Array *__pyx_vtabptr_7pyarrow_3lib_Int16Array;
 
 #line 376 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":380
  * 
  * 
- * cdef class Int64Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class UInt16Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 380 "pyarrow/lib.pxd"
 
 
 #line 380 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Int64Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_UInt16Array {
 
 #line 380 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 380 "pyarrow/lib.pxd"
 };
 
 #line 380 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Int64Array *__pyx_vtabptr_7pyarrow_3lib_Int64Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_UInt16Array *__pyx_vtabptr_7pyarrow_3lib_UInt16Array;
 
 #line 380 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":384
  * 
  * 
- * cdef class UInt64Array(IntegerArray):             # <<<<<<<<<<<<<<
+ * cdef class Int32Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 384 "pyarrow/lib.pxd"
 
 
 #line 384 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_UInt64Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_Int32Array {
 
 #line 384 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 384 "pyarrow/lib.pxd"
 };
 
 #line 384 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_UInt64Array *__pyx_vtabptr_7pyarrow_3lib_UInt64Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Int32Array *__pyx_vtabptr_7pyarrow_3lib_Int32Array;
 
 #line 384 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":388
  * 
  * 
- * cdef class HalfFloatArray(FloatingPointArray):             # <<<<<<<<<<<<<<
+ * cdef class UInt32Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 388 "pyarrow/lib.pxd"
 
 
 #line 388 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_HalfFloatArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_UInt32Array {
 
 #line 388 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 388 "pyarrow/lib.pxd"
 };
 
 #line 388 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_HalfFloatArray *__pyx_vtabptr_7pyarrow_3lib_HalfFloatArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_UInt32Array *__pyx_vtabptr_7pyarrow_3lib_UInt32Array;
 
 #line 388 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":392
  * 
  * 
- * cdef class FloatArray(FloatingPointArray):             # <<<<<<<<<<<<<<
+ * cdef class Int64Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 392 "pyarrow/lib.pxd"
 
 
 #line 392 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_FloatArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_Int64Array {
 
 #line 392 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 392 "pyarrow/lib.pxd"
 };
 
 #line 392 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_FloatArray *__pyx_vtabptr_7pyarrow_3lib_FloatArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Int64Array *__pyx_vtabptr_7pyarrow_3lib_Int64Array;
 
 #line 392 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":396
  * 
  * 
- * cdef class DoubleArray(FloatingPointArray):             # <<<<<<<<<<<<<<
+ * cdef class UInt64Array(IntegerArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 396 "pyarrow/lib.pxd"
 
 
 #line 396 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_DoubleArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_UInt64Array {
 
 #line 396 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray __pyx_base;
 
 #line 396 "pyarrow/lib.pxd"
 };
 
 #line 396 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_DoubleArray *__pyx_vtabptr_7pyarrow_3lib_DoubleArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_UInt64Array *__pyx_vtabptr_7pyarrow_3lib_UInt64Array;
 
 #line 396 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":400
  * 
  * 
- * cdef class FixedSizeBinaryArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class HalfFloatArray(FloatingPointArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 400 "pyarrow/lib.pxd"
 
 
 #line 400 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_HalfFloatArray {
 
 #line 400 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray __pyx_base;
 
 #line 400 "pyarrow/lib.pxd"
 };
 
 #line 400 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray *__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_HalfFloatArray *__pyx_vtabptr_7pyarrow_3lib_HalfFloatArray;
 
 #line 400 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":404
  * 
  * 
- * cdef class Decimal128Array(FixedSizeBinaryArray):             # <<<<<<<<<<<<<<
+ * cdef class FloatArray(FloatingPointArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 404 "pyarrow/lib.pxd"
 
 
 #line 404 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_FloatArray {
 
 #line 404 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray __pyx_base;
 
 #line 404 "pyarrow/lib.pxd"
 };
 
 #line 404 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Array *__pyx_vtabptr_7pyarrow_3lib_Decimal128Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_FloatArray *__pyx_vtabptr_7pyarrow_3lib_FloatArray;
 
 #line 404 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":408
  * 
  * 
- * cdef class Decimal256Array(FixedSizeBinaryArray):             # <<<<<<<<<<<<<<
+ * cdef class DoubleArray(FloatingPointArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 408 "pyarrow/lib.pxd"
 
 
 #line 408 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Array {
+struct __pyx_vtabstruct_7pyarrow_3lib_DoubleArray {
 
 #line 408 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray __pyx_base;
 
 #line 408 "pyarrow/lib.pxd"
 };
 
 #line 408 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Array *__pyx_vtabptr_7pyarrow_3lib_Decimal256Array;
+static struct __pyx_vtabstruct_7pyarrow_3lib_DoubleArray *__pyx_vtabptr_7pyarrow_3lib_DoubleArray;
 
 #line 408 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":412
  * 
  * 
- * cdef class StructArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class FixedSizeBinaryArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 412 "pyarrow/lib.pxd"
 
 
 #line 412 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_StructArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray {
 
 #line 412 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
 #line 412 "pyarrow/lib.pxd"
 };
 
 #line 412 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_StructArray *__pyx_vtabptr_7pyarrow_3lib_StructArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray *__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryArray;
 
 #line 412 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":416
  * 
  * 
- * cdef class BaseListArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class Decimal128Array(FixedSizeBinaryArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 416 "pyarrow/lib.pxd"
 
 
 #line 416 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Array {
 
 #line 416 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray __pyx_base;
 
 #line 416 "pyarrow/lib.pxd"
 };
 
 #line 416 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray *__pyx_vtabptr_7pyarrow_3lib_BaseListArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Array *__pyx_vtabptr_7pyarrow_3lib_Decimal128Array;
 
 #line 416 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":420
  * 
  * 
- * cdef class ListArray(BaseListArray):             # <<<<<<<<<<<<<<
+ * cdef class Decimal256Array(FixedSizeBinaryArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 420 "pyarrow/lib.pxd"
 
 
 #line 420 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_ListArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Array {
 
 #line 420 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray __pyx_base;
 
 #line 420 "pyarrow/lib.pxd"
 };
 
 #line 420 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_ListArray *__pyx_vtabptr_7pyarrow_3lib_ListArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Array *__pyx_vtabptr_7pyarrow_3lib_Decimal256Array;
 
 #line 420 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":424
  * 
  * 
- * cdef class LargeListArray(BaseListArray):             # <<<<<<<<<<<<<<
+ * cdef class StructArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 424 "pyarrow/lib.pxd"
 
 
 #line 424 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_LargeListArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_StructArray {
 
 #line 424 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
 #line 424 "pyarrow/lib.pxd"
 };
 
 #line 424 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_LargeListArray *__pyx_vtabptr_7pyarrow_3lib_LargeListArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_StructArray *__pyx_vtabptr_7pyarrow_3lib_StructArray;
 
 #line 424 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":428
  * 
  * 
- * cdef class MapArray(ListArray):             # <<<<<<<<<<<<<<
+ * cdef class BaseListArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 428 "pyarrow/lib.pxd"
 
 
 #line 428 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_MapArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray {
 
 #line 428 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_ListArray __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
 #line 428 "pyarrow/lib.pxd"
 };
 
 #line 428 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_MapArray *__pyx_vtabptr_7pyarrow_3lib_MapArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray *__pyx_vtabptr_7pyarrow_3lib_BaseListArray;
 
 #line 428 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":432
  * 
  * 
- * cdef class FixedSizeListArray(BaseListArray):             # <<<<<<<<<<<<<<
+ * cdef class ListArray(BaseListArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 432 "pyarrow/lib.pxd"
 
 
 #line 432 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_ListArray {
 
 #line 432 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray __pyx_base;
 
 #line 432 "pyarrow/lib.pxd"
 };
 
 #line 432 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListArray *__pyx_vtabptr_7pyarrow_3lib_FixedSizeListArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_ListArray *__pyx_vtabptr_7pyarrow_3lib_ListArray;
 
 #line 432 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":436
  * 
  * 
- * cdef class UnionArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class LargeListArray(BaseListArray):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 436 "pyarrow/lib.pxd"
 
 
 #line 436 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_UnionArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_LargeListArray {
 
 #line 436 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray __pyx_base;
 
 #line 436 "pyarrow/lib.pxd"
 };
 
 #line 436 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_UnionArray *__pyx_vtabptr_7pyarrow_3lib_UnionArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_LargeListArray *__pyx_vtabptr_7pyarrow_3lib_LargeListArray;
 
 #line 436 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":440
  * 
  * 
- * cdef class StringArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class ListViewArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 440 "pyarrow/lib.pxd"
 
 
 #line 440 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_StringArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_ListViewArray {
 
 #line 440 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
 #line 440 "pyarrow/lib.pxd"
 };
 
 #line 440 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_StringArray *__pyx_vtabptr_7pyarrow_3lib_StringArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_ListViewArray *__pyx_vtabptr_7pyarrow_3lib_ListViewArray;
 
 #line 440 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":444
  * 
  * 
- * cdef class BinaryArray(Array):             # <<<<<<<<<<<<<<
+ * cdef class LargeListViewArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 #line 444 "pyarrow/lib.pxd"
 
 
 #line 444 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_BinaryArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_LargeListViewArray {
 
 #line 444 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
 #line 444 "pyarrow/lib.pxd"
 };
 
 #line 444 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_BinaryArray *__pyx_vtabptr_7pyarrow_3lib_BinaryArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_LargeListViewArray *__pyx_vtabptr_7pyarrow_3lib_LargeListViewArray;
 
 #line 444 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/lib.pxd":448
  * 
  * 
- * cdef class DictionaryArray(Array):             # <<<<<<<<<<<<<<
- *     cdef:
- *         object _indices, _dictionary
+ * cdef class MapArray(ListArray):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
  */
 
 #line 448 "pyarrow/lib.pxd"
 
 
 #line 448 "pyarrow/lib.pxd"
-struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryArray {
+struct __pyx_vtabstruct_7pyarrow_3lib_MapArray {
 
 #line 448 "pyarrow/lib.pxd"
-  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+  struct __pyx_vtabstruct_7pyarrow_3lib_ListArray __pyx_base;
 
 #line 448 "pyarrow/lib.pxd"
 };
 
 #line 448 "pyarrow/lib.pxd"
-static struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryArray *__pyx_vtabptr_7pyarrow_3lib_DictionaryArray;
+static struct __pyx_vtabstruct_7pyarrow_3lib_MapArray *__pyx_vtabptr_7pyarrow_3lib_MapArray;
 
 #line 448 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":453
+/* "pyarrow/lib.pxd":452
+ * 
+ * 
+ * cdef class FixedSizeListArray(BaseListArray):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 452 "pyarrow/lib.pxd"
+
+
+#line 452 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListArray {
+
+#line 452 "pyarrow/lib.pxd"
+  struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray __pyx_base;
+
+#line 452 "pyarrow/lib.pxd"
+};
+
+#line 452 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListArray *__pyx_vtabptr_7pyarrow_3lib_FixedSizeListArray;
+
+#line 452 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":456
+ * 
+ * 
+ * cdef class UnionArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 456 "pyarrow/lib.pxd"
+
+
+#line 456 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_UnionArray {
+
+#line 456 "pyarrow/lib.pxd"
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+
+#line 456 "pyarrow/lib.pxd"
+};
+
+#line 456 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_UnionArray *__pyx_vtabptr_7pyarrow_3lib_UnionArray;
+
+#line 456 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":460
+ * 
+ * 
+ * cdef class StringArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 460 "pyarrow/lib.pxd"
+
+
+#line 460 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_StringArray {
+
+#line 460 "pyarrow/lib.pxd"
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+
+#line 460 "pyarrow/lib.pxd"
+};
+
+#line 460 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_StringArray *__pyx_vtabptr_7pyarrow_3lib_StringArray;
+
+#line 460 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":464
+ * 
+ * 
+ * cdef class BinaryArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 464 "pyarrow/lib.pxd"
+
+
+#line 464 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_BinaryArray {
+
+#line 464 "pyarrow/lib.pxd"
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+
+#line 464 "pyarrow/lib.pxd"
+};
+
+#line 464 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_BinaryArray *__pyx_vtabptr_7pyarrow_3lib_BinaryArray;
+
+#line 464 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":468
+ * 
+ * 
+ * cdef class StringViewArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 468 "pyarrow/lib.pxd"
+
+
+#line 468 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_StringViewArray {
+
+#line 468 "pyarrow/lib.pxd"
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+
+#line 468 "pyarrow/lib.pxd"
+};
+
+#line 468 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_StringViewArray *__pyx_vtabptr_7pyarrow_3lib_StringViewArray;
+
+#line 468 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":472
+ * 
+ * 
+ * cdef class BinaryViewArray(Array):             # <<<<<<<<<<<<<<
+ *     pass
+ * 
+ */
+
+#line 472 "pyarrow/lib.pxd"
+
+
+#line 472 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_BinaryViewArray {
+
+#line 472 "pyarrow/lib.pxd"
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+
+#line 472 "pyarrow/lib.pxd"
+};
+
+#line 472 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_BinaryViewArray *__pyx_vtabptr_7pyarrow_3lib_BinaryViewArray;
+
+#line 472 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":476
+ * 
+ * 
+ * cdef class DictionaryArray(Array):             # <<<<<<<<<<<<<<
+ *     cdef:
+ *         object _indices, _dictionary
+ */
+
+#line 476 "pyarrow/lib.pxd"
+
+
+#line 476 "pyarrow/lib.pxd"
+struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryArray {
+
+#line 476 "pyarrow/lib.pxd"
+  struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
+
+#line 476 "pyarrow/lib.pxd"
+};
+
+#line 476 "pyarrow/lib.pxd"
+static struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryArray *__pyx_vtabptr_7pyarrow_3lib_DictionaryArray;
+
+#line 476 "pyarrow/lib.pxd"
+
+
+/* "pyarrow/lib.pxd":481
  * 
  * 
  * cdef class ExtensionArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
 
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionArray {
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
 };
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionArray *__pyx_vtabptr_7pyarrow_3lib_ExtensionArray;
 
-#line 453 "pyarrow/lib.pxd"
+#line 481 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":457
+/* "pyarrow/lib.pxd":485
  * 
  * 
  * cdef class MonthDayNanoIntervalArray(Array):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
 
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_MonthDayNanoIntervalArray {
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Array __pyx_base;
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
 };
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_MonthDayNanoIntervalArray *__pyx_vtabptr_7pyarrow_3lib_MonthDayNanoIntervalArray;
 
-#line 457 "pyarrow/lib.pxd"
+#line 485 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":465
+/* "pyarrow/lib.pxd":493
  * 
  * 
  * cdef class ChunkedArray(_PandasConvertible):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CChunkedArray] sp_chunked_array
  */
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
 
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_ChunkedArray {
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_ChunkedArray *, std::shared_ptr< arrow::ChunkedArray>  const &);
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
   PyObject *(*getitem)(struct __pyx_obj_7pyarrow_3lib_ChunkedArray *, int64_t);
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
 };
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_ChunkedArray *__pyx_vtabptr_7pyarrow_3lib_ChunkedArray;
 
-#line 465 "pyarrow/lib.pxd"
+#line 493 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":482
+/* "pyarrow/lib.pxd":510
  * 
  * 
  * cdef class Table(_Tabular):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CTable] sp_table
  */
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
 
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_Table {
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_Table *, std::shared_ptr< arrow::Table>  const &);
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
 };
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_Table *__pyx_vtabptr_7pyarrow_3lib_Table;
 
-#line 482 "pyarrow/lib.pxd"
+#line 510 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":490
+/* "pyarrow/lib.pxd":518
  * 
  * 
  * cdef class RecordBatch(_Tabular):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CRecordBatch] sp_batch
  */
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
 
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_RecordBatch {
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_RecordBatch *, std::shared_ptr< arrow::RecordBatch>  const &);
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
 };
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_RecordBatch *__pyx_vtabptr_7pyarrow_3lib_RecordBatch;
 
-#line 490 "pyarrow/lib.pxd"
+#line 518 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":499
+/* "pyarrow/lib.pxd":527
  * 
  * 
  * cdef class Buffer(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CBuffer] buffer
  */
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
 
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_Buffer {
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_Buffer *, std::shared_ptr< arrow::Buffer>  const &);
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
   PyObject *(*getitem)(struct __pyx_obj_7pyarrow_3lib_Buffer *, int64_t);
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
 };
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_Buffer *__pyx_vtabptr_7pyarrow_3lib_Buffer;
 
-#line 499 "pyarrow/lib.pxd"
+#line 527 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":509
+/* "pyarrow/lib.pxd":537
  * 
  * 
  * cdef class ResizableBuffer(Buffer):             # <<<<<<<<<<<<<<
  * 
  *     cdef void init_rz(self, const shared_ptr[CResizableBuffer]& buffer)
  */
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
 
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_ResizableBuffer {
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_Buffer __pyx_base;
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
   void (*init_rz)(struct __pyx_obj_7pyarrow_3lib_ResizableBuffer *, std::shared_ptr< arrow::ResizableBuffer>  const &);
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
 };
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_ResizableBuffer *__pyx_vtabptr_7pyarrow_3lib_ResizableBuffer;
 
-#line 509 "pyarrow/lib.pxd"
+#line 537 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":514
+/* "pyarrow/lib.pxd":542
  * 
  * 
  * cdef class NativeFile(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CInputStream] input_stream
  */
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
 
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile {
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   PyObject *(*set_random_access_file)(struct __pyx_obj_7pyarrow_3lib_NativeFile *, std::shared_ptr< arrow::io::RandomAccessFile> );
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   PyObject *(*set_input_stream)(struct __pyx_obj_7pyarrow_3lib_NativeFile *, std::shared_ptr< arrow::io::InputStream> );
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   PyObject *(*set_output_stream)(struct __pyx_obj_7pyarrow_3lib_NativeFile *, std::shared_ptr< arrow::io::OutputStream> );
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::io::RandomAccessFile>  (*get_random_access_file)(struct __pyx_obj_7pyarrow_3lib_NativeFile *);
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::io::InputStream>  (*get_input_stream)(struct __pyx_obj_7pyarrow_3lib_NativeFile *);
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
   std::shared_ptr< arrow::io::OutputStream>  (*get_output_stream)(struct __pyx_obj_7pyarrow_3lib_NativeFile *);
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
 };
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile *__pyx_vtabptr_7pyarrow_3lib_NativeFile;
 
-#line 514 "pyarrow/lib.pxd"
+#line 542 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":538
+/* "pyarrow/lib.pxd":566
  * 
  * 
  * cdef class BufferedInputStream(NativeFile):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
 
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_BufferedInputStream {
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile __pyx_base;
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
 };
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_BufferedInputStream *__pyx_vtabptr_7pyarrow_3lib_BufferedInputStream;
 
-#line 538 "pyarrow/lib.pxd"
+#line 566 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":542
+/* "pyarrow/lib.pxd":570
  * 
  * 
  * cdef class BufferedOutputStream(NativeFile):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
 
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_BufferedOutputStream {
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile __pyx_base;
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
 };
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_BufferedOutputStream *__pyx_vtabptr_7pyarrow_3lib_BufferedOutputStream;
 
-#line 542 "pyarrow/lib.pxd"
+#line 570 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":546
+/* "pyarrow/lib.pxd":574
  * 
  * 
  * cdef class CompressedInputStream(NativeFile):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
 
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_CompressedInputStream {
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile __pyx_base;
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
 };
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_CompressedInputStream *__pyx_vtabptr_7pyarrow_3lib_CompressedInputStream;
 
-#line 546 "pyarrow/lib.pxd"
+#line 574 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":550
+/* "pyarrow/lib.pxd":578
  * 
  * 
  * cdef class CompressedOutputStream(NativeFile):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
 
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_CompressedOutputStream {
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
   struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile __pyx_base;
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
 };
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_CompressedOutputStream *__pyx_vtabptr_7pyarrow_3lib_CompressedOutputStream;
 
-#line 550 "pyarrow/lib.pxd"
+#line 578 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":564
+/* "pyarrow/lib.pxd":592
  * 
  * 
  * cdef class CacheOptions(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         CCacheOptions wrapped
  */
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
 
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_CacheOptions {
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_CacheOptions *, arrow::io::CacheOptions);
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
   arrow::io::CacheOptions (*unwrap)(struct __pyx_obj_7pyarrow_3lib_CacheOptions *);
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
   PyObject *(*wrap)(arrow::io::CacheOptions const );
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
 };
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_CacheOptions *__pyx_vtabptr_7pyarrow_3lib_CacheOptions;
 
-#line 564 "pyarrow/lib.pxd"
+#line 592 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":576
+/* "pyarrow/lib.pxd":604
  * 
  * 
  * cdef class Codec(_Weakrefable):             # <<<<<<<<<<<<<<
  *     cdef:
  *         shared_ptr[CCodec] wrapped
  */
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
 
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_Codec {
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
    arrow::util::Codec *(*unwrap)(struct __pyx_obj_7pyarrow_3lib_Codec *);
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
 };
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_Codec *__pyx_vtabptr_7pyarrow_3lib_Codec;
 
-#line 576 "pyarrow/lib.pxd"
+#line 604 "pyarrow/lib.pxd"
 
 
-/* "pyarrow/lib.pxd":584
+/* "pyarrow/lib.pxd":612
  * 
  * # This class is only used internally for now
  * cdef class StopToken:             # <<<<<<<<<<<<<<
  *     cdef:
  *         CStopToken stop_token
  */
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
 
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
 struct __pyx_vtabstruct_7pyarrow_3lib_StopToken {
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
   void (*init)(struct __pyx_obj_7pyarrow_3lib_StopToken *, arrow::StopToken);
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
 };
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
 static struct __pyx_vtabstruct_7pyarrow_3lib_StopToken *__pyx_vtabptr_7pyarrow_3lib_StopToken;
 
-#line 584 "pyarrow/lib.pxd"
+#line 612 "pyarrow/lib.pxd"
 
 
 /* "pyarrow/_parquet.pxd":564
  *         const COutputStream* sink)
  * 
  * cdef class FileEncryptionProperties:             # <<<<<<<<<<<<<<
  *     """File-level encryption properties for the low-level API"""
@@ -8681,14 +8977,16 @@
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_IpcWriteOptions;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_IpcReadOptions;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_Message;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_MemoryPool;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_DataType;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_ListType;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_LargeListType;
+  PyTypeObject *__pyx_ptype_7pyarrow_3lib_ListViewType;
+  PyTypeObject *__pyx_ptype_7pyarrow_3lib_LargeListViewType;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_MapType;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_FixedSizeListType;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_StructType;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_DictionaryMemo;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_DictionaryType;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_TimestampType;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_Time32Type;
@@ -8733,19 +9031,23 @@
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_Decimal128Array;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_Decimal256Array;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_StructArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_BaseListArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_ListArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_LargeListArray;
+  PyTypeObject *__pyx_ptype_7pyarrow_3lib_ListViewArray;
+  PyTypeObject *__pyx_ptype_7pyarrow_3lib_LargeListViewArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_MapArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_FixedSizeListArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_UnionArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_StringArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_BinaryArray;
+  PyTypeObject *__pyx_ptype_7pyarrow_3lib_StringViewArray;
+  PyTypeObject *__pyx_ptype_7pyarrow_3lib_BinaryViewArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_DictionaryArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_ExtensionArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_ChunkedArray;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib__Tabular;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_Table;
   PyTypeObject *__pyx_ptype_7pyarrow_3lib_RecordBatch;
@@ -9010,14 +9312,16 @@
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_IpcWriteOptions);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_IpcReadOptions);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_Message);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_MemoryPool);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_DataType);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_ListType);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_LargeListType);
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_ListViewType);
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_LargeListViewType);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_MapType);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_FixedSizeListType);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_StructType);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_DictionaryMemo);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_DictionaryType);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_TimestampType);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_Time32Type);
@@ -9062,19 +9366,23 @@
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_Decimal128Array);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_Decimal256Array);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_StructArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_BaseListArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_ListArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_LargeListArray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_ListViewArray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_LargeListViewArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_MapArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_FixedSizeListArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_UnionArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_StringArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_BinaryArray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_StringViewArray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_BinaryViewArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_DictionaryArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_ExtensionArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_ChunkedArray);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib__Tabular);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_Table);
   Py_CLEAR(clear_module_state->__pyx_ptype_7pyarrow_3lib_RecordBatch);
@@ -9311,14 +9619,16 @@
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_IpcWriteOptions);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_IpcReadOptions);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_Message);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_MemoryPool);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_DataType);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_ListType);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_LargeListType);
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_ListViewType);
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_LargeListViewType);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_MapType);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_FixedSizeListType);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_StructType);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_DictionaryMemo);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_DictionaryType);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_TimestampType);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_Time32Type);
@@ -9363,19 +9673,23 @@
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_Decimal128Array);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_Decimal256Array);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_StructArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_BaseListArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_ListArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_LargeListArray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_ListViewArray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_LargeListViewArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_MapArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_FixedSizeListArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_UnionArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_StringArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_BinaryArray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_StringViewArray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_BinaryViewArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_DictionaryArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_ExtensionArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_ChunkedArray);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib__Tabular);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_Table);
   Py_VISIT(traverse_module_state->__pyx_ptype_7pyarrow_3lib_RecordBatch);
@@ -9746,14 +10060,16 @@
 #define __pyx_ptype_7pyarrow_3lib_IpcWriteOptions __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_IpcWriteOptions
 #define __pyx_ptype_7pyarrow_3lib_IpcReadOptions __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_IpcReadOptions
 #define __pyx_ptype_7pyarrow_3lib_Message __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_Message
 #define __pyx_ptype_7pyarrow_3lib_MemoryPool __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_MemoryPool
 #define __pyx_ptype_7pyarrow_3lib_DataType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_DataType
 #define __pyx_ptype_7pyarrow_3lib_ListType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_ListType
 #define __pyx_ptype_7pyarrow_3lib_LargeListType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_LargeListType
+#define __pyx_ptype_7pyarrow_3lib_ListViewType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_ListViewType
+#define __pyx_ptype_7pyarrow_3lib_LargeListViewType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_LargeListViewType
 #define __pyx_ptype_7pyarrow_3lib_MapType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_MapType
 #define __pyx_ptype_7pyarrow_3lib_FixedSizeListType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_FixedSizeListType
 #define __pyx_ptype_7pyarrow_3lib_StructType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_StructType
 #define __pyx_ptype_7pyarrow_3lib_DictionaryMemo __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_DictionaryMemo
 #define __pyx_ptype_7pyarrow_3lib_DictionaryType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_DictionaryType
 #define __pyx_ptype_7pyarrow_3lib_TimestampType __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_TimestampType
 #define __pyx_ptype_7pyarrow_3lib_Time32Type __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_Time32Type
@@ -9798,19 +10114,23 @@
 #define __pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray
 #define __pyx_ptype_7pyarrow_3lib_Decimal128Array __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_Decimal128Array
 #define __pyx_ptype_7pyarrow_3lib_Decimal256Array __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_Decimal256Array
 #define __pyx_ptype_7pyarrow_3lib_StructArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_StructArray
 #define __pyx_ptype_7pyarrow_3lib_BaseListArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_BaseListArray
 #define __pyx_ptype_7pyarrow_3lib_ListArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_ListArray
 #define __pyx_ptype_7pyarrow_3lib_LargeListArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_LargeListArray
+#define __pyx_ptype_7pyarrow_3lib_ListViewArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_ListViewArray
+#define __pyx_ptype_7pyarrow_3lib_LargeListViewArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_LargeListViewArray
 #define __pyx_ptype_7pyarrow_3lib_MapArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_MapArray
 #define __pyx_ptype_7pyarrow_3lib_FixedSizeListArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_FixedSizeListArray
 #define __pyx_ptype_7pyarrow_3lib_UnionArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_UnionArray
 #define __pyx_ptype_7pyarrow_3lib_StringArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_StringArray
 #define __pyx_ptype_7pyarrow_3lib_BinaryArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_BinaryArray
+#define __pyx_ptype_7pyarrow_3lib_StringViewArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_StringViewArray
+#define __pyx_ptype_7pyarrow_3lib_BinaryViewArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_BinaryViewArray
 #define __pyx_ptype_7pyarrow_3lib_DictionaryArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_DictionaryArray
 #define __pyx_ptype_7pyarrow_3lib_ExtensionArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_ExtensionArray
 #define __pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray
 #define __pyx_ptype_7pyarrow_3lib_ChunkedArray __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_ChunkedArray
 #define __pyx_ptype_7pyarrow_3lib__Tabular __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib__Tabular
 #define __pyx_ptype_7pyarrow_3lib_Table __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_Table
 #define __pyx_ptype_7pyarrow_3lib_RecordBatch __pyx_mstate_global->__pyx_ptype_7pyarrow_3lib_RecordBatch
@@ -48702,160 +49022,172 @@
   __pyx_vtabptr_7pyarrow_3lib_MemoryPool = (struct __pyx_vtabstruct_7pyarrow_3lib_MemoryPool*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MemoryPool); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MemoryPool)) __PYX_ERR(8, 90, __pyx_L1_error)
   __pyx_ptype_7pyarrow_3lib_DataType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DataType", sizeof(struct __pyx_obj_7pyarrow_3lib_DataType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DataType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DataType) __PYX_ERR(8, 103, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_DataType = (struct __pyx_vtabstruct_7pyarrow_3lib_DataType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DataType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DataType)) __PYX_ERR(8, 103, __pyx_L1_error)
   __pyx_ptype_7pyarrow_3lib_ListType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ListType", sizeof(struct __pyx_obj_7pyarrow_3lib_ListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ListType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ListType) __PYX_ERR(8, 113, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_ListType = (struct __pyx_vtabstruct_7pyarrow_3lib_ListType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ListType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ListType)) __PYX_ERR(8, 113, __pyx_L1_error)
   __pyx_ptype_7pyarrow_3lib_LargeListType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "LargeListType", sizeof(struct __pyx_obj_7pyarrow_3lib_LargeListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_LargeListType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_LargeListType) __PYX_ERR(8, 118, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_3lib_LargeListType = (struct __pyx_vtabstruct_7pyarrow_3lib_LargeListType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_LargeListType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_LargeListType)) __PYX_ERR(8, 118, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_MapType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MapType", sizeof(struct __pyx_obj_7pyarrow_3lib_MapType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MapType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MapType) __PYX_ERR(8, 123, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_MapType = (struct __pyx_vtabstruct_7pyarrow_3lib_MapType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MapType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MapType)) __PYX_ERR(8, 123, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedSizeListType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeListType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeListType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeListType) __PYX_ERR(8, 128, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_FixedSizeListType = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeListType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeListType)) __PYX_ERR(8, 128, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_StructType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StructType", sizeof(struct __pyx_obj_7pyarrow_3lib_StructType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StructType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StructType) __PYX_ERR(8, 133, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_StructType = (struct __pyx_vtabstruct_7pyarrow_3lib_StructType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StructType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StructType)) __PYX_ERR(8, 133, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DictionaryMemo = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DictionaryMemo", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryMemo), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DictionaryMemo),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DictionaryMemo) __PYX_ERR(8, 140, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DictionaryType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DictionaryType", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DictionaryType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DictionaryType) __PYX_ERR(8, 148, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_DictionaryType = (struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DictionaryType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DictionaryType)) __PYX_ERR(8, 148, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_TimestampType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "TimestampType", sizeof(struct __pyx_obj_7pyarrow_3lib_TimestampType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_TimestampType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_TimestampType) __PYX_ERR(8, 153, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_TimestampType = (struct __pyx_vtabstruct_7pyarrow_3lib_TimestampType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_TimestampType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_TimestampType)) __PYX_ERR(8, 153, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Time32Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Time32Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Time32Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Time32Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Time32Type) __PYX_ERR(8, 158, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Time32Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Time32Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Time32Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Time32Type)) __PYX_ERR(8, 158, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Time64Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Time64Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Time64Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Time64Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Time64Type) __PYX_ERR(8, 163, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Time64Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Time64Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Time64Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Time64Type)) __PYX_ERR(8, 163, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DurationType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DurationType", sizeof(struct __pyx_obj_7pyarrow_3lib_DurationType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DurationType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DurationType) __PYX_ERR(8, 168, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_DurationType = (struct __pyx_vtabstruct_7pyarrow_3lib_DurationType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DurationType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DurationType)) __PYX_ERR(8, 168, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeBinaryType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType) __PYX_ERR(8, 173, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryType = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryType)) __PYX_ERR(8, 173, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Decimal128Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal128Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal128Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal128Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal128Type) __PYX_ERR(8, 178, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Decimal128Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal128Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal128Type)) __PYX_ERR(8, 178, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Decimal256Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal256Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal256Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal256Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal256Type) __PYX_ERR(8, 183, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Decimal256Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal256Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal256Type)) __PYX_ERR(8, 183, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_RunEndEncodedType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "RunEndEncodedType", sizeof(struct __pyx_obj_7pyarrow_3lib_RunEndEncodedType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_RunEndEncodedType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_RunEndEncodedType) __PYX_ERR(8, 188, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_RunEndEncodedType = (struct __pyx_vtabstruct_7pyarrow_3lib_RunEndEncodedType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_RunEndEncodedType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_RunEndEncodedType)) __PYX_ERR(8, 188, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BaseExtensionType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BaseExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_BaseExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BaseExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BaseExtensionType) __PYX_ERR(8, 193, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_BaseExtensionType = (struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BaseExtensionType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BaseExtensionType)) __PYX_ERR(8, 193, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ExtensionType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_ExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ExtensionType) __PYX_ERR(8, 198, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_ExtensionType = (struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ExtensionType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ExtensionType)) __PYX_ERR(8, 198, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedShapeTensorType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedShapeTensorType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedShapeTensorType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedShapeTensorType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedShapeTensorType) __PYX_ERR(8, 203, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_FixedShapeTensorType = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedShapeTensorType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedShapeTensorType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedShapeTensorType)) __PYX_ERR(8, 203, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_PyExtensionType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "PyExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_PyExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_PyExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_PyExtensionType) __PYX_ERR(8, 208, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_PyExtensionType = (struct __pyx_vtabstruct_7pyarrow_3lib_PyExtensionType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_PyExtensionType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_PyExtensionType)) __PYX_ERR(8, 208, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib__Metadata = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_Metadata", sizeof(struct __pyx_obj_7pyarrow_3lib__Metadata), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__Metadata),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__Metadata) __PYX_ERR(8, 212, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_KeyValueMetadata = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "KeyValueMetadata", sizeof(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_KeyValueMetadata) __PYX_ERR(8, 218, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_KeyValueMetadata = (struct __pyx_vtabstruct_7pyarrow_3lib_KeyValueMetadata*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_KeyValueMetadata); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_KeyValueMetadata)) __PYX_ERR(8, 218, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Field = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Field", sizeof(struct __pyx_obj_7pyarrow_3lib_Field), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Field),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Field) __PYX_ERR(8, 230, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Field = (struct __pyx_vtabstruct_7pyarrow_3lib_Field*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Field); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Field)) __PYX_ERR(8, 230, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Schema = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Schema", sizeof(struct __pyx_obj_7pyarrow_3lib_Schema), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Schema),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Schema) __PYX_ERR(8, 241, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Schema = (struct __pyx_vtabstruct_7pyarrow_3lib_Schema*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Schema); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Schema)) __PYX_ERR(8, 241, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Scalar = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Scalar", sizeof(struct __pyx_obj_7pyarrow_3lib_Scalar), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Scalar),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Scalar) __PYX_ERR(8, 250, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Scalar = (struct __pyx_vtabstruct_7pyarrow_3lib_Scalar*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Scalar); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Scalar)) __PYX_ERR(8, 250, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib__PandasConvertible = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_PandasConvertible", sizeof(struct __pyx_obj_7pyarrow_3lib__PandasConvertible), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__PandasConvertible),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__PandasConvertible) __PYX_ERR(8, 262, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Array) __PYX_ERR(8, 266, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Array)) __PYX_ERR(8, 266, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Tensor = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Tensor", sizeof(struct __pyx_obj_7pyarrow_3lib_Tensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Tensor),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Tensor) __PYX_ERR(8, 281, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Tensor = (struct __pyx_vtabstruct_7pyarrow_3lib_Tensor*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Tensor); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Tensor)) __PYX_ERR(8, 281, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_SparseCSRMatrix = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCSRMatrix", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCSRMatrix) __PYX_ERR(8, 292, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_SparseCSRMatrix = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSRMatrix*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCSRMatrix); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCSRMatrix)) __PYX_ERR(8, 292, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_SparseCSCMatrix = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCSCMatrix", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCSCMatrix) __PYX_ERR(8, 303, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_SparseCSCMatrix = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSCMatrix*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCSCMatrix); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCSCMatrix)) __PYX_ERR(8, 303, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_SparseCOOTensor = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCOOTensor", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCOOTensor) __PYX_ERR(8, 314, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_SparseCOOTensor = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCOOTensor*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCOOTensor); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCOOTensor)) __PYX_ERR(8, 314, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_SparseCSFTensor = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCSFTensor", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCSFTensor) __PYX_ERR(8, 325, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_SparseCSFTensor = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSFTensor*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCSFTensor); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCSFTensor)) __PYX_ERR(8, 325, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_NullArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "NullArray", sizeof(struct __pyx_obj_7pyarrow_3lib_NullArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_NullArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_NullArray) __PYX_ERR(8, 336, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_NullArray = (struct __pyx_vtabstruct_7pyarrow_3lib_NullArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_NullArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_NullArray)) __PYX_ERR(8, 336, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BooleanArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BooleanArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BooleanArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BooleanArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BooleanArray) __PYX_ERR(8, 340, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_BooleanArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BooleanArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BooleanArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BooleanArray)) __PYX_ERR(8, 340, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_NumericArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "NumericArray", sizeof(struct __pyx_obj_7pyarrow_3lib_NumericArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_NumericArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_NumericArray) __PYX_ERR(8, 344, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_NumericArray = (struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_NumericArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_NumericArray)) __PYX_ERR(8, 344, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_IntegerArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "IntegerArray", sizeof(struct __pyx_obj_7pyarrow_3lib_IntegerArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_IntegerArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_IntegerArray) __PYX_ERR(8, 348, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_IntegerArray = (struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_IntegerArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_IntegerArray)) __PYX_ERR(8, 348, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FloatingPointArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FloatingPointArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FloatingPointArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FloatingPointArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FloatingPointArray) __PYX_ERR(8, 352, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_FloatingPointArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FloatingPointArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FloatingPointArray)) __PYX_ERR(8, 352, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Int8Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int8Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int8Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int8Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int8Array) __PYX_ERR(8, 356, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Int8Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int8Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int8Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int8Array)) __PYX_ERR(8, 356, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UInt8Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt8Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt8Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt8Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt8Array) __PYX_ERR(8, 360, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_UInt8Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt8Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt8Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt8Array)) __PYX_ERR(8, 360, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Int16Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int16Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int16Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int16Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int16Array) __PYX_ERR(8, 364, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Int16Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int16Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int16Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int16Array)) __PYX_ERR(8, 364, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UInt16Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt16Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt16Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt16Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt16Array) __PYX_ERR(8, 368, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_UInt16Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt16Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt16Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt16Array)) __PYX_ERR(8, 368, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Int32Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int32Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int32Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int32Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int32Array) __PYX_ERR(8, 372, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Int32Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int32Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int32Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int32Array)) __PYX_ERR(8, 372, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UInt32Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt32Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt32Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt32Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt32Array) __PYX_ERR(8, 376, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_UInt32Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt32Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt32Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt32Array)) __PYX_ERR(8, 376, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Int64Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int64Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int64Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int64Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int64Array) __PYX_ERR(8, 380, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Int64Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int64Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int64Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int64Array)) __PYX_ERR(8, 380, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UInt64Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt64Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt64Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt64Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt64Array) __PYX_ERR(8, 384, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_UInt64Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt64Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt64Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt64Array)) __PYX_ERR(8, 384, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_HalfFloatArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "HalfFloatArray", sizeof(struct __pyx_obj_7pyarrow_3lib_HalfFloatArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_HalfFloatArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_HalfFloatArray) __PYX_ERR(8, 388, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_HalfFloatArray = (struct __pyx_vtabstruct_7pyarrow_3lib_HalfFloatArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_HalfFloatArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_HalfFloatArray)) __PYX_ERR(8, 388, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FloatArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FloatArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FloatArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FloatArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FloatArray) __PYX_ERR(8, 392, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_FloatArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FloatArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FloatArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FloatArray)) __PYX_ERR(8, 392, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DoubleArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DoubleArray", sizeof(struct __pyx_obj_7pyarrow_3lib_DoubleArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DoubleArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DoubleArray) __PYX_ERR(8, 396, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_DoubleArray = (struct __pyx_vtabstruct_7pyarrow_3lib_DoubleArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DoubleArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DoubleArray)) __PYX_ERR(8, 396, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeBinaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray) __PYX_ERR(8, 400, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryArray)) __PYX_ERR(8, 400, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Decimal128Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal128Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal128Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal128Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal128Array) __PYX_ERR(8, 404, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Decimal128Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal128Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal128Array)) __PYX_ERR(8, 404, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Decimal256Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal256Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal256Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal256Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal256Array) __PYX_ERR(8, 408, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Decimal256Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal256Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal256Array)) __PYX_ERR(8, 408, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_StructArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StructArray", sizeof(struct __pyx_obj_7pyarrow_3lib_StructArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StructArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StructArray) __PYX_ERR(8, 412, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_StructArray = (struct __pyx_vtabstruct_7pyarrow_3lib_StructArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StructArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StructArray)) __PYX_ERR(8, 412, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BaseListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BaseListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BaseListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BaseListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BaseListArray) __PYX_ERR(8, 416, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_BaseListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BaseListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BaseListArray)) __PYX_ERR(8, 416, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ListArray) __PYX_ERR(8, 420, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_ListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ListArray)) __PYX_ERR(8, 420, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_LargeListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "LargeListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_LargeListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_LargeListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_LargeListArray) __PYX_ERR(8, 424, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_LargeListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_LargeListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_LargeListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_LargeListArray)) __PYX_ERR(8, 424, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_MapArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MapArray", sizeof(struct __pyx_obj_7pyarrow_3lib_MapArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MapArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MapArray) __PYX_ERR(8, 428, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_MapArray = (struct __pyx_vtabstruct_7pyarrow_3lib_MapArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MapArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MapArray)) __PYX_ERR(8, 428, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_FixedSizeListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeListArray) __PYX_ERR(8, 432, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_FixedSizeListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeListArray)) __PYX_ERR(8, 432, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_UnionArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UnionArray", sizeof(struct __pyx_obj_7pyarrow_3lib_UnionArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UnionArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UnionArray) __PYX_ERR(8, 436, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_UnionArray = (struct __pyx_vtabstruct_7pyarrow_3lib_UnionArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UnionArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UnionArray)) __PYX_ERR(8, 436, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_StringArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StringArray", sizeof(struct __pyx_obj_7pyarrow_3lib_StringArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StringArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StringArray) __PYX_ERR(8, 440, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_StringArray = (struct __pyx_vtabstruct_7pyarrow_3lib_StringArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StringArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StringArray)) __PYX_ERR(8, 440, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BinaryArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BinaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BinaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BinaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BinaryArray) __PYX_ERR(8, 444, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_BinaryArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BinaryArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BinaryArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BinaryArray)) __PYX_ERR(8, 444, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_DictionaryArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DictionaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DictionaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DictionaryArray) __PYX_ERR(8, 448, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_DictionaryArray = (struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DictionaryArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DictionaryArray)) __PYX_ERR(8, 448, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ExtensionArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ExtensionArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ExtensionArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ExtensionArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ExtensionArray) __PYX_ERR(8, 453, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_ExtensionArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ExtensionArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ExtensionArray)) __PYX_ERR(8, 453, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MonthDayNanoIntervalArray", sizeof(struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray) __PYX_ERR(8, 457, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_MonthDayNanoIntervalArray = (struct __pyx_vtabstruct_7pyarrow_3lib_MonthDayNanoIntervalArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MonthDayNanoIntervalArray)) __PYX_ERR(8, 457, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ChunkedArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ChunkedArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ChunkedArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ChunkedArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ChunkedArray) __PYX_ERR(8, 465, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_ChunkedArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ChunkedArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ChunkedArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ChunkedArray)) __PYX_ERR(8, 465, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib__Tabular = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_Tabular", sizeof(struct __pyx_obj_7pyarrow_3lib__Tabular), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__Tabular),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__Tabular) __PYX_ERR(8, 478, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Table = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Table", sizeof(struct __pyx_obj_7pyarrow_3lib_Table), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Table),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Table) __PYX_ERR(8, 482, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Table = (struct __pyx_vtabstruct_7pyarrow_3lib_Table*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Table); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Table)) __PYX_ERR(8, 482, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_RecordBatch = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "RecordBatch", sizeof(struct __pyx_obj_7pyarrow_3lib_RecordBatch), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_RecordBatch),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_RecordBatch) __PYX_ERR(8, 490, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_RecordBatch = (struct __pyx_vtabstruct_7pyarrow_3lib_RecordBatch*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_RecordBatch); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_RecordBatch)) __PYX_ERR(8, 490, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Buffer = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Buffer", sizeof(struct __pyx_obj_7pyarrow_3lib_Buffer), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Buffer),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Buffer) __PYX_ERR(8, 499, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Buffer = (struct __pyx_vtabstruct_7pyarrow_3lib_Buffer*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Buffer); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Buffer)) __PYX_ERR(8, 499, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_ResizableBuffer = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ResizableBuffer", sizeof(struct __pyx_obj_7pyarrow_3lib_ResizableBuffer), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ResizableBuffer),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ResizableBuffer) __PYX_ERR(8, 509, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_ResizableBuffer = (struct __pyx_vtabstruct_7pyarrow_3lib_ResizableBuffer*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ResizableBuffer); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ResizableBuffer)) __PYX_ERR(8, 509, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_NativeFile = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "NativeFile", sizeof(struct __pyx_obj_7pyarrow_3lib_NativeFile), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_NativeFile),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_NativeFile) __PYX_ERR(8, 514, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_NativeFile = (struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_NativeFile); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_NativeFile)) __PYX_ERR(8, 514, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BufferedInputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BufferedInputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_BufferedInputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BufferedInputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BufferedInputStream) __PYX_ERR(8, 538, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_BufferedInputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_BufferedInputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BufferedInputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BufferedInputStream)) __PYX_ERR(8, 538, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_BufferedOutputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BufferedOutputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_BufferedOutputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BufferedOutputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BufferedOutputStream) __PYX_ERR(8, 542, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_BufferedOutputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_BufferedOutputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BufferedOutputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BufferedOutputStream)) __PYX_ERR(8, 542, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_CompressedInputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "CompressedInputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_CompressedInputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_CompressedInputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_CompressedInputStream) __PYX_ERR(8, 546, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_CompressedInputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_CompressedInputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_CompressedInputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_CompressedInputStream)) __PYX_ERR(8, 546, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_CompressedOutputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "CompressedOutputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_CompressedOutputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_CompressedOutputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_CompressedOutputStream) __PYX_ERR(8, 550, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_CompressedOutputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_CompressedOutputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_CompressedOutputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_CompressedOutputStream)) __PYX_ERR(8, 550, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib__CRecordBatchWriter = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_CRecordBatchWriter", sizeof(struct __pyx_obj_7pyarrow_3lib__CRecordBatchWriter), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__CRecordBatchWriter),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__CRecordBatchWriter) __PYX_ERR(8, 554, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_RecordBatchReader = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "RecordBatchReader", sizeof(struct __pyx_obj_7pyarrow_3lib_RecordBatchReader), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_RecordBatchReader),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_RecordBatchReader) __PYX_ERR(8, 559, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_CacheOptions = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "CacheOptions", sizeof(struct __pyx_obj_7pyarrow_3lib_CacheOptions), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_CacheOptions),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_CacheOptions) __PYX_ERR(8, 564, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_CacheOptions = (struct __pyx_vtabstruct_7pyarrow_3lib_CacheOptions*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_CacheOptions); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_CacheOptions)) __PYX_ERR(8, 564, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_Codec = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Codec", sizeof(struct __pyx_obj_7pyarrow_3lib_Codec), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Codec),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Codec) __PYX_ERR(8, 576, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_Codec = (struct __pyx_vtabstruct_7pyarrow_3lib_Codec*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Codec); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Codec)) __PYX_ERR(8, 576, __pyx_L1_error)
-  __pyx_ptype_7pyarrow_3lib_StopToken = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StopToken", sizeof(struct __pyx_obj_7pyarrow_3lib_StopToken), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StopToken),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StopToken) __PYX_ERR(8, 584, __pyx_L1_error)
-  __pyx_vtabptr_7pyarrow_3lib_StopToken = (struct __pyx_vtabstruct_7pyarrow_3lib_StopToken*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StopToken); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StopToken)) __PYX_ERR(8, 584, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ListViewType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ListViewType", sizeof(struct __pyx_obj_7pyarrow_3lib_ListViewType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ListViewType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ListViewType) __PYX_ERR(8, 123, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_ListViewType = (struct __pyx_vtabstruct_7pyarrow_3lib_ListViewType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ListViewType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ListViewType)) __PYX_ERR(8, 123, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_LargeListViewType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "LargeListViewType", sizeof(struct __pyx_obj_7pyarrow_3lib_LargeListViewType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_LargeListViewType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_LargeListViewType) __PYX_ERR(8, 128, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_LargeListViewType = (struct __pyx_vtabstruct_7pyarrow_3lib_LargeListViewType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_LargeListViewType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_LargeListViewType)) __PYX_ERR(8, 128, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_MapType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MapType", sizeof(struct __pyx_obj_7pyarrow_3lib_MapType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MapType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MapType) __PYX_ERR(8, 133, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_MapType = (struct __pyx_vtabstruct_7pyarrow_3lib_MapType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MapType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MapType)) __PYX_ERR(8, 133, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedSizeListType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeListType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeListType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeListType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeListType) __PYX_ERR(8, 138, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_FixedSizeListType = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeListType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeListType)) __PYX_ERR(8, 138, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_StructType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StructType", sizeof(struct __pyx_obj_7pyarrow_3lib_StructType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StructType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StructType) __PYX_ERR(8, 143, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_StructType = (struct __pyx_vtabstruct_7pyarrow_3lib_StructType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StructType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StructType)) __PYX_ERR(8, 143, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DictionaryMemo = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DictionaryMemo", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryMemo), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DictionaryMemo),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DictionaryMemo) __PYX_ERR(8, 150, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DictionaryType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DictionaryType", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DictionaryType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DictionaryType) __PYX_ERR(8, 158, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_DictionaryType = (struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DictionaryType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DictionaryType)) __PYX_ERR(8, 158, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_TimestampType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "TimestampType", sizeof(struct __pyx_obj_7pyarrow_3lib_TimestampType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_TimestampType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_TimestampType) __PYX_ERR(8, 163, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_TimestampType = (struct __pyx_vtabstruct_7pyarrow_3lib_TimestampType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_TimestampType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_TimestampType)) __PYX_ERR(8, 163, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Time32Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Time32Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Time32Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Time32Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Time32Type) __PYX_ERR(8, 168, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Time32Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Time32Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Time32Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Time32Type)) __PYX_ERR(8, 168, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Time64Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Time64Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Time64Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Time64Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Time64Type) __PYX_ERR(8, 173, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Time64Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Time64Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Time64Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Time64Type)) __PYX_ERR(8, 173, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DurationType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DurationType", sizeof(struct __pyx_obj_7pyarrow_3lib_DurationType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DurationType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DurationType) __PYX_ERR(8, 178, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_DurationType = (struct __pyx_vtabstruct_7pyarrow_3lib_DurationType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DurationType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DurationType)) __PYX_ERR(8, 178, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeBinaryType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType) __PYX_ERR(8, 183, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryType = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryType)) __PYX_ERR(8, 183, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Decimal128Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal128Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal128Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal128Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal128Type) __PYX_ERR(8, 188, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Decimal128Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal128Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal128Type)) __PYX_ERR(8, 188, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Decimal256Type = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal256Type", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal256Type), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal256Type),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal256Type) __PYX_ERR(8, 193, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Decimal256Type = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Type*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal256Type); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal256Type)) __PYX_ERR(8, 193, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_RunEndEncodedType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "RunEndEncodedType", sizeof(struct __pyx_obj_7pyarrow_3lib_RunEndEncodedType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_RunEndEncodedType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_RunEndEncodedType) __PYX_ERR(8, 198, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_RunEndEncodedType = (struct __pyx_vtabstruct_7pyarrow_3lib_RunEndEncodedType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_RunEndEncodedType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_RunEndEncodedType)) __PYX_ERR(8, 198, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BaseExtensionType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BaseExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_BaseExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BaseExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BaseExtensionType) __PYX_ERR(8, 203, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_BaseExtensionType = (struct __pyx_vtabstruct_7pyarrow_3lib_BaseExtensionType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BaseExtensionType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BaseExtensionType)) __PYX_ERR(8, 203, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ExtensionType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_ExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ExtensionType) __PYX_ERR(8, 208, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_ExtensionType = (struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ExtensionType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ExtensionType)) __PYX_ERR(8, 208, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedShapeTensorType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedShapeTensorType", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedShapeTensorType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedShapeTensorType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedShapeTensorType) __PYX_ERR(8, 213, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_FixedShapeTensorType = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedShapeTensorType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedShapeTensorType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedShapeTensorType)) __PYX_ERR(8, 213, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_PyExtensionType = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "PyExtensionType", sizeof(struct __pyx_obj_7pyarrow_3lib_PyExtensionType), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_PyExtensionType),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_PyExtensionType) __PYX_ERR(8, 218, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_PyExtensionType = (struct __pyx_vtabstruct_7pyarrow_3lib_PyExtensionType*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_PyExtensionType); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_PyExtensionType)) __PYX_ERR(8, 218, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib__Metadata = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_Metadata", sizeof(struct __pyx_obj_7pyarrow_3lib__Metadata), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__Metadata),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__Metadata) __PYX_ERR(8, 222, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_KeyValueMetadata = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "KeyValueMetadata", sizeof(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_KeyValueMetadata),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_KeyValueMetadata) __PYX_ERR(8, 228, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_KeyValueMetadata = (struct __pyx_vtabstruct_7pyarrow_3lib_KeyValueMetadata*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_KeyValueMetadata); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_KeyValueMetadata)) __PYX_ERR(8, 228, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Field = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Field", sizeof(struct __pyx_obj_7pyarrow_3lib_Field), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Field),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Field) __PYX_ERR(8, 240, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Field = (struct __pyx_vtabstruct_7pyarrow_3lib_Field*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Field); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Field)) __PYX_ERR(8, 240, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Schema = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Schema", sizeof(struct __pyx_obj_7pyarrow_3lib_Schema), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Schema),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Schema) __PYX_ERR(8, 251, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Schema = (struct __pyx_vtabstruct_7pyarrow_3lib_Schema*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Schema); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Schema)) __PYX_ERR(8, 251, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Scalar = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Scalar", sizeof(struct __pyx_obj_7pyarrow_3lib_Scalar), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Scalar),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Scalar) __PYX_ERR(8, 260, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Scalar = (struct __pyx_vtabstruct_7pyarrow_3lib_Scalar*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Scalar); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Scalar)) __PYX_ERR(8, 260, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib__PandasConvertible = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_PandasConvertible", sizeof(struct __pyx_obj_7pyarrow_3lib__PandasConvertible), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__PandasConvertible),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__PandasConvertible) __PYX_ERR(8, 272, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Array) __PYX_ERR(8, 276, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Array)) __PYX_ERR(8, 276, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Tensor = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Tensor", sizeof(struct __pyx_obj_7pyarrow_3lib_Tensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Tensor),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Tensor) __PYX_ERR(8, 291, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Tensor = (struct __pyx_vtabstruct_7pyarrow_3lib_Tensor*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Tensor); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Tensor)) __PYX_ERR(8, 291, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_SparseCSRMatrix = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCSRMatrix", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCSRMatrix),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCSRMatrix) __PYX_ERR(8, 304, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_SparseCSRMatrix = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSRMatrix*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCSRMatrix); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCSRMatrix)) __PYX_ERR(8, 304, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_SparseCSCMatrix = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCSCMatrix", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCSCMatrix),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCSCMatrix) __PYX_ERR(8, 315, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_SparseCSCMatrix = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSCMatrix*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCSCMatrix); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCSCMatrix)) __PYX_ERR(8, 315, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_SparseCOOTensor = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCOOTensor", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCOOTensor),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCOOTensor) __PYX_ERR(8, 326, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_SparseCOOTensor = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCOOTensor*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCOOTensor); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCOOTensor)) __PYX_ERR(8, 326, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_SparseCSFTensor = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "SparseCSFTensor", sizeof(struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_SparseCSFTensor),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_SparseCSFTensor) __PYX_ERR(8, 337, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_SparseCSFTensor = (struct __pyx_vtabstruct_7pyarrow_3lib_SparseCSFTensor*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_SparseCSFTensor); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_SparseCSFTensor)) __PYX_ERR(8, 337, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_NullArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "NullArray", sizeof(struct __pyx_obj_7pyarrow_3lib_NullArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_NullArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_NullArray) __PYX_ERR(8, 348, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_NullArray = (struct __pyx_vtabstruct_7pyarrow_3lib_NullArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_NullArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_NullArray)) __PYX_ERR(8, 348, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BooleanArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BooleanArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BooleanArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BooleanArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BooleanArray) __PYX_ERR(8, 352, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_BooleanArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BooleanArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BooleanArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BooleanArray)) __PYX_ERR(8, 352, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_NumericArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "NumericArray", sizeof(struct __pyx_obj_7pyarrow_3lib_NumericArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_NumericArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_NumericArray) __PYX_ERR(8, 356, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_NumericArray = (struct __pyx_vtabstruct_7pyarrow_3lib_NumericArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_NumericArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_NumericArray)) __PYX_ERR(8, 356, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_IntegerArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "IntegerArray", sizeof(struct __pyx_obj_7pyarrow_3lib_IntegerArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_IntegerArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_IntegerArray) __PYX_ERR(8, 360, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_IntegerArray = (struct __pyx_vtabstruct_7pyarrow_3lib_IntegerArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_IntegerArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_IntegerArray)) __PYX_ERR(8, 360, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FloatingPointArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FloatingPointArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FloatingPointArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FloatingPointArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FloatingPointArray) __PYX_ERR(8, 364, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_FloatingPointArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FloatingPointArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FloatingPointArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FloatingPointArray)) __PYX_ERR(8, 364, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Int8Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int8Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int8Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int8Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int8Array) __PYX_ERR(8, 368, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Int8Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int8Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int8Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int8Array)) __PYX_ERR(8, 368, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UInt8Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt8Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt8Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt8Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt8Array) __PYX_ERR(8, 372, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_UInt8Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt8Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt8Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt8Array)) __PYX_ERR(8, 372, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Int16Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int16Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int16Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int16Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int16Array) __PYX_ERR(8, 376, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Int16Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int16Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int16Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int16Array)) __PYX_ERR(8, 376, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UInt16Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt16Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt16Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt16Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt16Array) __PYX_ERR(8, 380, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_UInt16Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt16Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt16Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt16Array)) __PYX_ERR(8, 380, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Int32Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int32Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int32Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int32Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int32Array) __PYX_ERR(8, 384, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Int32Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int32Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int32Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int32Array)) __PYX_ERR(8, 384, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UInt32Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt32Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt32Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt32Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt32Array) __PYX_ERR(8, 388, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_UInt32Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt32Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt32Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt32Array)) __PYX_ERR(8, 388, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Int64Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Int64Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Int64Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Int64Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Int64Array) __PYX_ERR(8, 392, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Int64Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Int64Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Int64Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Int64Array)) __PYX_ERR(8, 392, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UInt64Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UInt64Array", sizeof(struct __pyx_obj_7pyarrow_3lib_UInt64Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UInt64Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UInt64Array) __PYX_ERR(8, 396, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_UInt64Array = (struct __pyx_vtabstruct_7pyarrow_3lib_UInt64Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UInt64Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UInt64Array)) __PYX_ERR(8, 396, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_HalfFloatArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "HalfFloatArray", sizeof(struct __pyx_obj_7pyarrow_3lib_HalfFloatArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_HalfFloatArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_HalfFloatArray) __PYX_ERR(8, 400, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_HalfFloatArray = (struct __pyx_vtabstruct_7pyarrow_3lib_HalfFloatArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_HalfFloatArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_HalfFloatArray)) __PYX_ERR(8, 400, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FloatArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FloatArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FloatArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FloatArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FloatArray) __PYX_ERR(8, 404, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_FloatArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FloatArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FloatArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FloatArray)) __PYX_ERR(8, 404, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DoubleArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DoubleArray", sizeof(struct __pyx_obj_7pyarrow_3lib_DoubleArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DoubleArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DoubleArray) __PYX_ERR(8, 408, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_DoubleArray = (struct __pyx_vtabstruct_7pyarrow_3lib_DoubleArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DoubleArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DoubleArray)) __PYX_ERR(8, 408, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeBinaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeBinaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray) __PYX_ERR(8, 412, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeBinaryArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeBinaryArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeBinaryArray)) __PYX_ERR(8, 412, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Decimal128Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal128Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal128Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal128Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal128Array) __PYX_ERR(8, 416, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Decimal128Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal128Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal128Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal128Array)) __PYX_ERR(8, 416, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Decimal256Array = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Decimal256Array", sizeof(struct __pyx_obj_7pyarrow_3lib_Decimal256Array), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Decimal256Array),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Decimal256Array) __PYX_ERR(8, 420, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Decimal256Array = (struct __pyx_vtabstruct_7pyarrow_3lib_Decimal256Array*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Decimal256Array); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Decimal256Array)) __PYX_ERR(8, 420, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_StructArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StructArray", sizeof(struct __pyx_obj_7pyarrow_3lib_StructArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StructArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StructArray) __PYX_ERR(8, 424, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_StructArray = (struct __pyx_vtabstruct_7pyarrow_3lib_StructArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StructArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StructArray)) __PYX_ERR(8, 424, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BaseListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BaseListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BaseListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BaseListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BaseListArray) __PYX_ERR(8, 428, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_BaseListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BaseListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BaseListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BaseListArray)) __PYX_ERR(8, 428, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ListArray) __PYX_ERR(8, 432, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_ListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ListArray)) __PYX_ERR(8, 432, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_LargeListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "LargeListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_LargeListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_LargeListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_LargeListArray) __PYX_ERR(8, 436, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_LargeListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_LargeListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_LargeListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_LargeListArray)) __PYX_ERR(8, 436, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ListViewArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ListViewArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ListViewArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ListViewArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ListViewArray) __PYX_ERR(8, 440, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_ListViewArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ListViewArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ListViewArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ListViewArray)) __PYX_ERR(8, 440, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_LargeListViewArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "LargeListViewArray", sizeof(struct __pyx_obj_7pyarrow_3lib_LargeListViewArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_LargeListViewArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_LargeListViewArray) __PYX_ERR(8, 444, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_LargeListViewArray = (struct __pyx_vtabstruct_7pyarrow_3lib_LargeListViewArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_LargeListViewArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_LargeListViewArray)) __PYX_ERR(8, 444, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_MapArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MapArray", sizeof(struct __pyx_obj_7pyarrow_3lib_MapArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MapArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MapArray) __PYX_ERR(8, 448, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_MapArray = (struct __pyx_vtabstruct_7pyarrow_3lib_MapArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MapArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MapArray)) __PYX_ERR(8, 448, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_FixedSizeListArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "FixedSizeListArray", sizeof(struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_FixedSizeListArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_FixedSizeListArray) __PYX_ERR(8, 452, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_FixedSizeListArray = (struct __pyx_vtabstruct_7pyarrow_3lib_FixedSizeListArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_FixedSizeListArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_FixedSizeListArray)) __PYX_ERR(8, 452, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_UnionArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "UnionArray", sizeof(struct __pyx_obj_7pyarrow_3lib_UnionArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_UnionArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_UnionArray) __PYX_ERR(8, 456, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_UnionArray = (struct __pyx_vtabstruct_7pyarrow_3lib_UnionArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_UnionArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_UnionArray)) __PYX_ERR(8, 456, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_StringArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StringArray", sizeof(struct __pyx_obj_7pyarrow_3lib_StringArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StringArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StringArray) __PYX_ERR(8, 460, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_StringArray = (struct __pyx_vtabstruct_7pyarrow_3lib_StringArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StringArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StringArray)) __PYX_ERR(8, 460, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BinaryArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BinaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BinaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BinaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BinaryArray) __PYX_ERR(8, 464, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_BinaryArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BinaryArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BinaryArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BinaryArray)) __PYX_ERR(8, 464, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_StringViewArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StringViewArray", sizeof(struct __pyx_obj_7pyarrow_3lib_StringViewArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StringViewArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StringViewArray) __PYX_ERR(8, 468, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_StringViewArray = (struct __pyx_vtabstruct_7pyarrow_3lib_StringViewArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StringViewArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StringViewArray)) __PYX_ERR(8, 468, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BinaryViewArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BinaryViewArray", sizeof(struct __pyx_obj_7pyarrow_3lib_BinaryViewArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BinaryViewArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BinaryViewArray) __PYX_ERR(8, 472, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_BinaryViewArray = (struct __pyx_vtabstruct_7pyarrow_3lib_BinaryViewArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BinaryViewArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BinaryViewArray)) __PYX_ERR(8, 472, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_DictionaryArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "DictionaryArray", sizeof(struct __pyx_obj_7pyarrow_3lib_DictionaryArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_DictionaryArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_DictionaryArray) __PYX_ERR(8, 476, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_DictionaryArray = (struct __pyx_vtabstruct_7pyarrow_3lib_DictionaryArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_DictionaryArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_DictionaryArray)) __PYX_ERR(8, 476, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ExtensionArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ExtensionArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ExtensionArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ExtensionArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ExtensionArray) __PYX_ERR(8, 481, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_ExtensionArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ExtensionArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ExtensionArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ExtensionArray)) __PYX_ERR(8, 481, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "MonthDayNanoIntervalArray", sizeof(struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_MonthDayNanoIntervalArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray) __PYX_ERR(8, 485, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_MonthDayNanoIntervalArray = (struct __pyx_vtabstruct_7pyarrow_3lib_MonthDayNanoIntervalArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_MonthDayNanoIntervalArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_MonthDayNanoIntervalArray)) __PYX_ERR(8, 485, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ChunkedArray = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ChunkedArray", sizeof(struct __pyx_obj_7pyarrow_3lib_ChunkedArray), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ChunkedArray),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ChunkedArray) __PYX_ERR(8, 493, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_ChunkedArray = (struct __pyx_vtabstruct_7pyarrow_3lib_ChunkedArray*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ChunkedArray); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ChunkedArray)) __PYX_ERR(8, 493, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib__Tabular = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_Tabular", sizeof(struct __pyx_obj_7pyarrow_3lib__Tabular), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__Tabular),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__Tabular) __PYX_ERR(8, 506, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Table = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Table", sizeof(struct __pyx_obj_7pyarrow_3lib_Table), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Table),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Table) __PYX_ERR(8, 510, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Table = (struct __pyx_vtabstruct_7pyarrow_3lib_Table*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Table); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Table)) __PYX_ERR(8, 510, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_RecordBatch = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "RecordBatch", sizeof(struct __pyx_obj_7pyarrow_3lib_RecordBatch), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_RecordBatch),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_RecordBatch) __PYX_ERR(8, 518, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_RecordBatch = (struct __pyx_vtabstruct_7pyarrow_3lib_RecordBatch*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_RecordBatch); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_RecordBatch)) __PYX_ERR(8, 518, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Buffer = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Buffer", sizeof(struct __pyx_obj_7pyarrow_3lib_Buffer), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Buffer),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Buffer) __PYX_ERR(8, 527, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Buffer = (struct __pyx_vtabstruct_7pyarrow_3lib_Buffer*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Buffer); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Buffer)) __PYX_ERR(8, 527, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_ResizableBuffer = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "ResizableBuffer", sizeof(struct __pyx_obj_7pyarrow_3lib_ResizableBuffer), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_ResizableBuffer),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_ResizableBuffer) __PYX_ERR(8, 537, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_ResizableBuffer = (struct __pyx_vtabstruct_7pyarrow_3lib_ResizableBuffer*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_ResizableBuffer); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_ResizableBuffer)) __PYX_ERR(8, 537, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_NativeFile = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "NativeFile", sizeof(struct __pyx_obj_7pyarrow_3lib_NativeFile), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_NativeFile),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_NativeFile) __PYX_ERR(8, 542, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_NativeFile = (struct __pyx_vtabstruct_7pyarrow_3lib_NativeFile*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_NativeFile); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_NativeFile)) __PYX_ERR(8, 542, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BufferedInputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BufferedInputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_BufferedInputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BufferedInputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BufferedInputStream) __PYX_ERR(8, 566, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_BufferedInputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_BufferedInputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BufferedInputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BufferedInputStream)) __PYX_ERR(8, 566, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_BufferedOutputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "BufferedOutputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_BufferedOutputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_BufferedOutputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_BufferedOutputStream) __PYX_ERR(8, 570, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_BufferedOutputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_BufferedOutputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_BufferedOutputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_BufferedOutputStream)) __PYX_ERR(8, 570, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_CompressedInputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "CompressedInputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_CompressedInputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_CompressedInputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_CompressedInputStream) __PYX_ERR(8, 574, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_CompressedInputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_CompressedInputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_CompressedInputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_CompressedInputStream)) __PYX_ERR(8, 574, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_CompressedOutputStream = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "CompressedOutputStream", sizeof(struct __pyx_obj_7pyarrow_3lib_CompressedOutputStream), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_CompressedOutputStream),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_CompressedOutputStream) __PYX_ERR(8, 578, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_CompressedOutputStream = (struct __pyx_vtabstruct_7pyarrow_3lib_CompressedOutputStream*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_CompressedOutputStream); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_CompressedOutputStream)) __PYX_ERR(8, 578, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib__CRecordBatchWriter = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "_CRecordBatchWriter", sizeof(struct __pyx_obj_7pyarrow_3lib__CRecordBatchWriter), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib__CRecordBatchWriter),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib__CRecordBatchWriter) __PYX_ERR(8, 582, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_RecordBatchReader = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "RecordBatchReader", sizeof(struct __pyx_obj_7pyarrow_3lib_RecordBatchReader), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_RecordBatchReader),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_RecordBatchReader) __PYX_ERR(8, 587, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_CacheOptions = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "CacheOptions", sizeof(struct __pyx_obj_7pyarrow_3lib_CacheOptions), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_CacheOptions),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_CacheOptions) __PYX_ERR(8, 592, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_CacheOptions = (struct __pyx_vtabstruct_7pyarrow_3lib_CacheOptions*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_CacheOptions); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_CacheOptions)) __PYX_ERR(8, 592, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_Codec = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "Codec", sizeof(struct __pyx_obj_7pyarrow_3lib_Codec), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_Codec),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_Codec) __PYX_ERR(8, 604, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_Codec = (struct __pyx_vtabstruct_7pyarrow_3lib_Codec*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_Codec); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_Codec)) __PYX_ERR(8, 604, __pyx_L1_error)
+  __pyx_ptype_7pyarrow_3lib_StopToken = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow.lib", "StopToken", sizeof(struct __pyx_obj_7pyarrow_3lib_StopToken), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_3lib_StopToken),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_3lib_StopToken) __PYX_ERR(8, 612, __pyx_L1_error)
+  __pyx_vtabptr_7pyarrow_3lib_StopToken = (struct __pyx_vtabstruct_7pyarrow_3lib_StopToken*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_3lib_StopToken); if (unlikely(!__pyx_vtabptr_7pyarrow_3lib_StopToken)) __PYX_ERR(8, 612, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("pyarrow._parquet"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7pyarrow_8_parquet_FileEncryptionProperties = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "FileEncryptionProperties", sizeof(struct __pyx_obj_7pyarrow_8_parquet_FileEncryptionProperties), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_FileEncryptionProperties),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_FileEncryptionProperties) __PYX_ERR(4, 564, __pyx_L1_error)
   __pyx_vtabptr_7pyarrow_8_parquet_FileEncryptionProperties = (struct __pyx_vtabstruct_7pyarrow_8_parquet_FileEncryptionProperties*)__Pyx_GetVtable(__pyx_ptype_7pyarrow_8_parquet_FileEncryptionProperties); if (unlikely(!__pyx_vtabptr_7pyarrow_8_parquet_FileEncryptionProperties)) __PYX_ERR(4, 564, __pyx_L1_error)
   __pyx_ptype_7pyarrow_8_parquet_ParquetSchema = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "ParquetSchema", sizeof(struct __pyx_obj_7pyarrow_8_parquet_ParquetSchema), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_ParquetSchema),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_ParquetSchema) __PYX_ERR(4, 608, __pyx_L1_error)
   __pyx_ptype_7pyarrow_8_parquet_FileMetaData = __Pyx_ImportType_3_0_10(__pyx_t_1, "pyarrow._parquet", "FileMetaData", sizeof(struct __pyx_obj_7pyarrow_8_parquet_FileMetaData), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_7pyarrow_8_parquet_FileMetaData),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7pyarrow_8_parquet_FileMetaData) __PYX_ERR(4, 613, __pyx_L1_error)
```

### Comparing `palletjack-2.1.2/palletjack/palletjack_cython.pyx` & `palletjack-2.2.0/palletjack/palletjack_cython.pyx`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/palletjack/parquet_types_palletjack.cpp` & `palletjack-2.2.0/palletjack/parquet_types_palletjack.cpp`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/palletjack/parquet_types_palletjack.h` & `palletjack-2.2.0/palletjack/parquet_types_palletjack.h`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/palletjack.egg-info/PKG-INFO` & `palletjack-2.2.0/palletjack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: palletjack
-Version: 2.1.2
+Version: 2.2.0
 Summary: Faster parquet metadata reading
 Author-email: Marcin Krystianc <marcin.krystianc@gmail.com>
 Project-URL: Homepage, https://github.com/marcin-krystianc/PalletJack
 Project-URL: Issues, https://github.com/marcin-krystianc/PalletJack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyarrow~=15.0
+Requires-Dist: pyarrow~=16.0
 
 # PalletJack
 PalletJack was created as a workaround for apache/arrow#38149. The standard parquet reader is not efficient for files with numerous columns and row groups, as it requires parsing the entire metadata section each time the file is opened. The size of this metadata section is proportional to the number of columns and row groups in the file.
 
 PalletJack reduces the amount of metadata bytes that need to be read and decoded by storing metadata in a different format. This approach enables reading only the essential subset of metadata as required.
 
 ## Features
 
 - Storing parquet metadata in an indexed format
 - Reading parquet metadata for a subset of row groups and columns
 
 ## Required:
 
-- pyarrow  ~= 15.0
+- pyarrow  ~= 16.0
  
 PalletJack operates on top of pyarrow, making it an essential requirement for both building and using PalletJack. While our source package is compatible with recent versions of pyarrow, the binary distribution package specifically requires the latest major version of pyarrow.
 
 ##  Installation
 
 ```
 pip install palletjack
```

### Comparing `palletjack-2.1.2/palletjack.egg-info/SOURCES.txt` & `palletjack-2.2.0/palletjack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/pyproject.toml` & `palletjack-2.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = [
   "setuptools>=55.0",
   "Cython>=3",
-  "pyarrow~=15.0",
+  "pyarrow~=16.0",
   "thrift",
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "palletjack"
-version = "2.1.2"
+version = "2.2.0"
 authors = [
   { name="Marcin Krystianc", email="marcin.krystianc@gmail.com" },
 ]
 description = "Faster parquet metadata reading"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "pyarrow~=15.0",
+  "pyarrow~=16.0",
 ]
 
 [tool.setuptools.packages.find]
 include = ['palletjack*']
 
 [tool.setuptools.package-data]
 "*" = ["*.pxd", "*.h", "*.pyx"]
```

### Comparing `palletjack-2.1.2/setup.py` & `palletjack-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/test/test_palletjack.py` & `palletjack-2.2.0/test/test_palletjack.py`

 * *Files identical despite different names*

### Comparing `palletjack-2.1.2/test/test_readme.py` & `palletjack-2.2.0/test/test_readme.py`

 * *Files identical despite different names*


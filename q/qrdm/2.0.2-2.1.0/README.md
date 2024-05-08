# Comparing `tmp/qrdm-2.0.2.tar.gz` & `tmp/qrdm-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrdm-2.0.2.tar", last modified: Fri Apr 19 14:40:51 2024, max compression
+gzip compressed data, was "qrdm-2.1.0.tar", last modified: Wed May  8 14:33:16 2024, max compression
```

## Comparing `qrdm-2.0.2.tar` & `qrdm-2.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.840281 qrdm-2.0.2/
--rw-r--r--   0 er27743    (501) staff       (20)     1093 2024-02-01 15:51:39.000000 qrdm-2.0.2/LICENSE.txt
--rw-r--r--   0 er27743    (501) staff       (20)      165 2024-02-01 20:42:07.000000 qrdm-2.0.2/MANIFEST.in
--rw-r--r--   0 er27743    (501) staff       (20)     5231 2024-04-19 14:40:51.840073 qrdm-2.0.2/PKG-INFO
--rw-r--r--   0 er27743    (501) staff       (20)     3146 2024-03-20 18:50:58.000000 qrdm-2.0.2/README.md
--rw-r--r--   0 er27743    (501) staff       (20)     2377 2024-03-20 18:17:25.000000 qrdm-2.0.2/pyproject.toml
--rw-r--r--   0 er27743    (501) staff       (20)       38 2024-04-19 14:40:51.840318 qrdm-2.0.2/setup.cfg
--rw-r--r--   0 er27743    (501) staff       (20)      405 2024-03-19 18:31:04.000000 qrdm-2.0.2/setup.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.831039 qrdm-2.0.2/src/
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.833181 qrdm-2.0.2/src/qrdm/
--rw-r--r--   0 er27743    (501) staff       (20)      410 2024-04-18 18:52:12.000000 qrdm-2.0.2/src/qrdm/__init__.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.835103 qrdm-2.0.2/src/qrdm/backend/
--rw-r--r--   0 er27743    (501) staff       (20)      582 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)     5110 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/config.py
--rw-r--r--   0 er27743    (501) staff       (20)     2274 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/main.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.835811 qrdm-2.0.2/src/qrdm/backend/routers/
--rw-r--r--   0 er27743    (501) staff       (20)       49 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/routers/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)     5650 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/backend/routers/qr.py
--rw-r--r--   0 er27743    (501) staff       (20)      485 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/exceptions.py
--rw-r--r--   0 er27743    (501) staff       (20)     4430 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/models.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.837021 qrdm-2.0.2/src/qrdm/qr/
--rw-r--r--   0 er27743    (501) staff       (20)       45 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/qr/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)     1234 2024-02-01 20:42:07.000000 qrdm-2.0.2/src/qrdm/qr/_const.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.837776 qrdm-2.0.2/src/qrdm/qr/data/
--rw-r--r--   0 er27743    (501) staff       (20)       50 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/qr/data/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)      789 2024-02-01 20:42:07.000000 qrdm-2.0.2/src/qrdm/qr/data/qr_capacity.csv
--rw-r--r--   0 er27743    (501) staff       (20)    35444 2024-02-01 20:42:07.000000 qrdm-2.0.2/src/qrdm/qr/data/qrdm_logo_red.png
--rw-r--r--   0 er27743    (501) staff       (20)    12725 2024-04-18 18:49:43.000000 qrdm-2.0.2/src/qrdm/qr/decode.py
--rw-r--r--   0 er27743    (501) staff       (20)    11089 2024-04-18 18:49:43.000000 qrdm-2.0.2/src/qrdm/qr/encode.py
--rw-r--r--   0 er27743    (501) staff       (20)     9598 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/qr/pdf_writer.py
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.838950 qrdm-2.0.2/src/qrdm/qr/protobuf/
--rw-r--r--   0 er27743    (501) staff       (20)      823 2024-03-19 18:31:04.000000 qrdm-2.0.2/src/qrdm/qr/protobuf/__init__.py
--rw-r--r--   0 er27743    (501) staff       (20)      383 2024-02-05 20:55:14.000000 qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm.proto
--rw-r--r--   0 er27743    (501) staff       (20)     2046 2024-02-05 20:56:25.000000 qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm_pb2.py
--rw-r--r--   0 er27743    (501) staff       (20)     2310 2024-02-09 16:48:01.000000 qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm_pb2.pyi
-drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-04-19 14:40:51.839160 qrdm-2.0.2/src/qrdm.egg-info/
--rw-r--r--   0 er27743    (501) staff       (20)     5231 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/PKG-INFO
--rw-r--r--   0 er27743    (501) staff       (20)      773 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/SOURCES.txt
--rw-r--r--   0 er27743    (501) staff       (20)        1 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/dependency_links.txt
--rw-r--r--   0 er27743    (501) staff       (20)      439 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/requires.txt
--rw-r--r--   0 er27743    (501) staff       (20)        5 2024-04-19 14:40:51.000000 qrdm-2.0.2/src/qrdm.egg-info/top_level.txt
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-05-08 14:33:16.748841 qrdm-2.1.0/
+-rw-r--r--   0 er27743    (501) staff       (20)     1093 2024-02-01 15:51:39.000000 qrdm-2.1.0/LICENSE.txt
+-rw-r--r--   0 er27743    (501) staff       (20)      165 2024-02-01 20:42:07.000000 qrdm-2.1.0/MANIFEST.in
+-rw-r--r--   0 er27743    (501) staff       (20)     5231 2024-05-08 14:33:16.748600 qrdm-2.1.0/PKG-INFO
+-rw-r--r--   0 er27743    (501) staff       (20)     3146 2024-04-11 15:56:42.000000 qrdm-2.1.0/README.md
+-rw-r--r--   0 er27743    (501) staff       (20)     2377 2024-03-20 18:17:25.000000 qrdm-2.1.0/pyproject.toml
+-rw-r--r--   0 er27743    (501) staff       (20)       38 2024-05-08 14:33:16.748891 qrdm-2.1.0/setup.cfg
+-rw-r--r--   0 er27743    (501) staff       (20)      405 2024-03-19 18:31:04.000000 qrdm-2.1.0/setup.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-05-08 14:33:16.735365 qrdm-2.1.0/src/
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-05-08 14:33:16.742161 qrdm-2.1.0/src/qrdm/
+-rw-r--r--   0 er27743    (501) staff       (20)      410 2024-05-08 14:28:21.000000 qrdm-2.1.0/src/qrdm/__init__.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-05-08 14:33:16.743777 qrdm-2.1.0/src/qrdm/backend/
+-rw-r--r--   0 er27743    (501) staff       (20)      582 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/backend/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)     5110 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/backend/config.py
+-rw-r--r--   0 er27743    (501) staff       (20)     2274 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/backend/main.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-05-08 14:33:16.744310 qrdm-2.1.0/src/qrdm/backend/routers/
+-rw-r--r--   0 er27743    (501) staff       (20)       49 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/backend/routers/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)     5650 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/backend/routers/qr.py
+-rw-r--r--   0 er27743    (501) staff       (20)      485 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/exceptions.py
+-rw-r--r--   0 er27743    (501) staff       (20)     4430 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/models.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-05-08 14:33:16.745307 qrdm-2.1.0/src/qrdm/qr/
+-rw-r--r--   0 er27743    (501) staff       (20)       45 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/qr/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)     1234 2024-02-01 20:42:07.000000 qrdm-2.1.0/src/qrdm/qr/_const.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-05-08 14:33:16.745973 qrdm-2.1.0/src/qrdm/qr/data/
+-rw-r--r--   0 er27743    (501) staff       (20)       50 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/qr/data/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)      789 2024-02-01 20:42:07.000000 qrdm-2.1.0/src/qrdm/qr/data/qr_capacity.csv
+-rw-r--r--   0 er27743    (501) staff       (20)    35444 2024-02-01 20:42:07.000000 qrdm-2.1.0/src/qrdm/qr/data/qrdm_logo_red.png
+-rw-r--r--   0 er27743    (501) staff       (20)    12725 2024-04-19 14:53:52.000000 qrdm-2.1.0/src/qrdm/qr/decode.py
+-rw-r--r--   0 er27743    (501) staff       (20)    11775 2024-05-08 14:18:24.000000 qrdm-2.1.0/src/qrdm/qr/encode.py
+-rw-r--r--   0 er27743    (501) staff       (20)     9598 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/qr/pdf_writer.py
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-05-08 14:33:16.747174 qrdm-2.1.0/src/qrdm/qr/protobuf/
+-rw-r--r--   0 er27743    (501) staff       (20)      823 2024-03-19 18:31:04.000000 qrdm-2.1.0/src/qrdm/qr/protobuf/__init__.py
+-rw-r--r--   0 er27743    (501) staff       (20)      383 2024-02-05 20:55:14.000000 qrdm-2.1.0/src/qrdm/qr/protobuf/qrdm.proto
+-rw-r--r--   0 er27743    (501) staff       (20)     2046 2024-02-05 20:56:25.000000 qrdm-2.1.0/src/qrdm/qr/protobuf/qrdm_pb2.py
+-rw-r--r--   0 er27743    (501) staff       (20)     2310 2024-02-09 16:48:01.000000 qrdm-2.1.0/src/qrdm/qr/protobuf/qrdm_pb2.pyi
+drwxr-xr-x   0 er27743    (501) staff       (20)        0 2024-05-08 14:33:16.747522 qrdm-2.1.0/src/qrdm.egg-info/
+-rw-r--r--   0 er27743    (501) staff       (20)     5231 2024-05-08 14:33:16.000000 qrdm-2.1.0/src/qrdm.egg-info/PKG-INFO
+-rw-r--r--   0 er27743    (501) staff       (20)      773 2024-05-08 14:33:16.000000 qrdm-2.1.0/src/qrdm.egg-info/SOURCES.txt
+-rw-r--r--   0 er27743    (501) staff       (20)        1 2024-05-08 14:33:16.000000 qrdm-2.1.0/src/qrdm.egg-info/dependency_links.txt
+-rw-r--r--   0 er27743    (501) staff       (20)      439 2024-05-08 14:33:16.000000 qrdm-2.1.0/src/qrdm.egg-info/requires.txt
+-rw-r--r--   0 er27743    (501) staff       (20)        5 2024-05-08 14:33:16.000000 qrdm-2.1.0/src/qrdm.egg-info/top_level.txt
```

### Comparing `qrdm-2.0.2/LICENSE.txt` & `qrdm-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/PKG-INFO` & `qrdm-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrdm
-Version: 2.0.2
+Version: 2.1.0
 Summary: QR Data Manager
 Author: MIT Lincoln Laboratory
 Author-email: "Cuyler D. O'Brien" <cuyler.obrien@ll.mit.edu>, "Eric A. Quintero" <Eric.Quintero@ll.mit.edu>, Tod Shannon <tod@ll.mit.edu>, "Michael J. Snyder" <michael.snyder@ll.mit.edu>
 License: MIT License
 Project-URL: Documentation, https://mit-ll.github.io/qrdm
 Project-URL: Repository, https://github.com/mit-ll/qrdm
 Keywords: QR,QR code
```

### Comparing `qrdm-2.0.2/README.md` & `qrdm-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/pyproject.toml` & `qrdm-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/backend/__init__.py` & `qrdm-2.1.0/src/qrdm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/backend/config.py` & `qrdm-2.1.0/src/qrdm/backend/config.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/backend/main.py` & `qrdm-2.1.0/src/qrdm/backend/main.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/backend/routers/qr.py` & `qrdm-2.1.0/src/qrdm/backend/routers/qr.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/models.py` & `qrdm-2.1.0/src/qrdm/models.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/qr/_const.py` & `qrdm-2.1.0/src/qrdm/qr/_const.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/qr/data/qr_capacity.csv` & `qrdm-2.1.0/src/qrdm/qr/data/qr_capacity.csv`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/qr/data/qrdm_logo_red.png` & `qrdm-2.1.0/src/qrdm/qr/data/qrdm_logo_red.png`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/qr/decode.py` & `qrdm-2.1.0/src/qrdm/qr/decode.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/qr/encode.py` & `qrdm-2.1.0/src/qrdm/qr/encode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Copyright 2024, Massachusetts Institute of Technology
 # Subject to FAR 52.227-11 - Patent Rights - Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 """Generate QRDM PDFs from source documents."""
+
 from __future__ import annotations
 
 import hashlib
 import io
 import logging
 import shutil
+import warnings
 from collections.abc import Iterator
 from math import ceil
 from pathlib import Path
 from typing import Optional, Union, overload
 
 import qrcode.image.svg as qr_svg
 import reedsolo
@@ -208,28 +210,45 @@
     else:
         payload_fragments = list(
             _split_file_content(
                 total_payload_bytes, maximum_length=single_qr_payload_size
             )
         )
 
+    n_raw_fragments = len(payload_fragments)
     if encode_ec_codes:
-        num_ecc = ceil(len(payload_fragments) * qr_const.EC_CODE_PROPORTION)
-        payload_fragments = _generate_ec_fragments(payload_fragments, num_ecc=num_ecc)
+        # Reed-Solomon encoder chunks at ~256, so we just want this fraction _per 256_
+        # at most
+        e = qr_const.EC_CODE_PROPORTION
+        max_ecc = ceil(256 * e / (1 + e))
+        num_ecc = min(max_ecc, ceil(n_raw_fragments * e))
+        n_qr_expected = n_raw_fragments + (
+            1 + (n_raw_fragments // (256 - num_ecc)) * num_ecc
+        )
+        if n_raw_fragments * (1 + e) >= 256:
+            warnings.warn(
+                f"Input data requires {n_qr_expected} QR codes to encode. "
+                "Error-correction requires significantly longer processing above 256 codes."
+            )
     else:
         num_ecc = 0
+        n_qr_expected = n_raw_fragments
 
-    total_qr_codes = len(payload_fragments)
-    if total_qr_codes >= N_MAX_QRS:
+    if n_qr_expected >= N_MAX_QRS:
         msg = (
-            f"The total number of QR codes: {total_qr_codes} exceeds the maximum of "
-            f"{N_MAX_QRS}, consider breaking the file into smaller pieces."
+            f"The provided input requires {n_qr_expected} QR codes to encode, which "
+            f"exceeds the maximum of {N_MAX_QRS}, consider breaking the file into smaller pieces."
         )
         raise QREncodeError(msg)
 
+    if num_ecc > 0:
+        payload_fragments = _generate_ec_fragments(payload_fragments, num_ecc=num_ecc)
+
+    total_qr_codes = len(payload_fragments)
+
     qr_contents: list[bytes] = []
     for sequence_number, fragment in enumerate(payload_fragments):
         qr_meta = QRMeta(
             document_hash=document_hash,
             sequence_number=sequence_number,
             total_qr_codes=total_qr_codes,
             num_ecc=num_ecc,
```

### Comparing `qrdm-2.0.2/src/qrdm/qr/pdf_writer.py` & `qrdm-2.1.0/src/qrdm/qr/pdf_writer.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/qr/protobuf/__init__.py` & `qrdm-2.1.0/src/qrdm/qr/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm_pb2.py` & `qrdm-2.1.0/src/qrdm/qr/protobuf/qrdm_pb2.py`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm/qr/protobuf/qrdm_pb2.pyi` & `qrdm-2.1.0/src/qrdm/qr/protobuf/qrdm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qrdm-2.0.2/src/qrdm.egg-info/PKG-INFO` & `qrdm-2.1.0/src/qrdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrdm
-Version: 2.0.2
+Version: 2.1.0
 Summary: QR Data Manager
 Author: MIT Lincoln Laboratory
 Author-email: "Cuyler D. O'Brien" <cuyler.obrien@ll.mit.edu>, "Eric A. Quintero" <Eric.Quintero@ll.mit.edu>, Tod Shannon <tod@ll.mit.edu>, "Michael J. Snyder" <michael.snyder@ll.mit.edu>
 License: MIT License
 Project-URL: Documentation, https://mit-ll.github.io/qrdm
 Project-URL: Repository, https://github.com/mit-ll/qrdm
 Keywords: QR,QR code
```

### Comparing `qrdm-2.0.2/src/qrdm.egg-info/SOURCES.txt` & `qrdm-2.1.0/src/qrdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


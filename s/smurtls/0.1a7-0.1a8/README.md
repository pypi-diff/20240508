# Comparing `tmp/smurtls-0.1a7-py3-none-any.whl.zip` & `tmp/smurtls-0.1a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 3743 bytes, number of entries: 7
--rwxrwxrwx  2.0 unx       19 b- defN 24-Apr-30 11:12 smurtls/__init__.py
--rwxrwxrwx  2.0 unx      162 b- defN 24-Apr-30 08:28 smurtls/config.py
--rwxrwxrwx  2.0 unx     7188 b- defN 24-Apr-30 09:19 smurtls/data.py
--rwxrwxrwx  2.0 unx      444 b- defN 24-Apr-30 13:10 smurtls-0.1a7.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 24-Apr-30 13:10 smurtls-0.1a7.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 24-Apr-30 13:10 smurtls-0.1a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      515 b- defN 24-Apr-30 13:10 smurtls-0.1a7.dist-info/RECORD
-7 files, 8428 bytes uncompressed, 2831 bytes compressed:  66.4%
+Zip file size: 3567 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       19 b- defN 24-May-08 20:07 smurtls/__init__.py
+-rw-r--r--  2.0 unx     7331 b- defN 24-May-08 20:07 smurtls/data.py
+-rw-r--r--  2.0 unx      474 b- defN 24-May-08 20:07 smurtls-0.1a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 20:07 smurtls-0.1a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-08 20:07 smurtls-0.1a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      442 b- defN 24-May-08 20:07 smurtls-0.1a8.dist-info/RECORD
+6 files, 8366 bytes uncompressed, 2765 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
 Filename: smurtls/__init__.py
 Comment: 
 
-Filename: smurtls/config.py
-Comment: 
-
 Filename: smurtls/data.py
 Comment: 
 
-Filename: smurtls-0.1a7.dist-info/METADATA
+Filename: smurtls-0.1a8.dist-info/METADATA
 Comment: 
 
-Filename: smurtls-0.1a7.dist-info/WHEEL
+Filename: smurtls-0.1a8.dist-info/WHEEL
 Comment: 
 
-Filename: smurtls-0.1a7.dist-info/top_level.txt
+Filename: smurtls-0.1a8.dist-info/top_level.txt
 Comment: 
 
-Filename: smurtls-0.1a7.dist-info/RECORD
+Filename: smurtls-0.1a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smurtls/data.py

```diff
@@ -1,8 +1,13 @@
-from config import *
+import numpy as np
+import pandas as pd
+from sklearn.preprocessing import MinMaxScaler
+from lifelines.utils import  concordance_index
+from datetime import datetime
+
 class Reader:
     @staticmethod 
     def read_csv(dataSetPath, columns = [], **params):
         df = pd.read_csv(dataSetPath)
         if len(columns) != 0:
             df = df[columns]
         # --------------------
```


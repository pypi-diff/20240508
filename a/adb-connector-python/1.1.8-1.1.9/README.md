# Comparing `tmp/adb_connector_python-1.1.8-py3-none-any.whl.zip` & `tmp/adb_connector_python-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11570 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    39235 b- defN 24-Apr-10 20:15 adb_connector_python/connector.py
--rwxrwxrwx  2.0 unx     1088 b- defN 24-Apr-10 20:15 adb_connector_python-1.1.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5452 b- defN 24-Apr-10 20:15 adb_connector_python-1.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 20:15 adb_connector_python-1.1.8.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       21 b- defN 24-Apr-10 20:15 adb_connector_python-1.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      542 b- defN 24-Apr-10 20:15 adb_connector_python-1.1.8.dist-info/RECORD
-6 files, 46430 bytes uncompressed, 10578 bytes compressed:  77.2%
+Zip file size: 11565 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    39197 b- defN 24-May-08 07:33 adb_connector_python/connector.py
+-rwxr-xr-x  2.0 unx     1088 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5452 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       21 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      542 b- defN 24-May-08 07:34 adb_connector_python-1.1.9.dist-info/RECORD
+6 files, 46392 bytes uncompressed, 10573 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: adb_connector_python/connector.py
 Comment: 
 
-Filename: adb_connector_python-1.1.8.dist-info/LICENSE
+Filename: adb_connector_python-1.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: adb_connector_python-1.1.8.dist-info/METADATA
+Filename: adb_connector_python-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: adb_connector_python-1.1.8.dist-info/WHEEL
+Filename: adb_connector_python-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: adb_connector_python-1.1.8.dist-info/top_level.txt
+Filename: adb_connector_python-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: adb_connector_python-1.1.8.dist-info/RECORD
+Filename: adb_connector_python-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adb_connector_python/connector.py

```diff
@@ -105,15 +105,14 @@
     match platform:
         case "win32":
             system("cls")
         case "linux" | "darwin":
             system("clear")
 
 try:
-    check_output("adb start-server")
     check_output("adb --version", shell=True)
 except:
     raise CalledProcessError(127,"You have not adb installed on this pc")
```

## Comparing `adb_connector_python-1.1.8.dist-info/LICENSE` & `adb_connector_python-1.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `adb_connector_python-1.1.8.dist-info/METADATA` & `adb_connector_python-1.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-connector-python
-Version: 1.1.8
+Version: 1.1.9
 Summary: A simple python package to interface with adb
 Author: Giuseppe Gravante
 License: MIT License
         
         Copyright (c) 2023 Giuseppe7887
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


# Comparing `tmp/xlineparse-0.0.3-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip` & `tmp/xlineparse-0.0.4-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 645330 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 14:06 xlineparse/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 14:06 xlineparse-0.0.3.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 14:06 xlineparse.libs/
--rw-r--r--  2.0 unx        0 b- defN 24-May-08 14:06 xlineparse/py.typed
--rw-r--r--  2.0 unx     7541 b- defN 24-May-08 14:06 xlineparse/__init__.py
--rwxr-xr-x  2.0 unx  2324012 b- defN 24-May-08 14:06 xlineparse/xlineparse.cpython-312-i386-linux-gnu.so
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 14:06 xlineparse-0.0.3.dist-info/license_files/
--rw-r--r--  2.0 unx     2674 b- defN 24-May-08 14:06 xlineparse-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx      690 b- defN 24-May-08 14:06 xlineparse-0.0.3.dist-info/RECORD
--rw-r--r--  2.0 unx       49 b- defN 24-May-08 14:06 xlineparse-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx      212 b- defN 24-May-08 14:06 xlineparse-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx     1071 b- defN 24-May-08 14:06 xlineparse-0.0.3.dist-info/license_files/LICENSE
-12 files, 2336249 bytes uncompressed, 643640 bytes compressed:  72.5%
+Zip file size: 645353 bytes, number of entries: 12
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 16:46 xlineparse/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 16:46 xlineparse-0.0.4.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 16:46 xlineparse.libs/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-08 16:46 xlineparse/py.typed
+-rw-r--r--  2.0 unx     7641 b- defN 24-May-08 16:46 xlineparse/__init__.py
+-rwxr-xr-x  2.0 unx  2324012 b- defN 24-May-08 16:46 xlineparse/xlineparse.cpython-312-i386-linux-gnu.so
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-08 16:46 xlineparse-0.0.4.dist-info/license_files/
+-rw-r--r--  2.0 unx     2674 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      690 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/RECORD
+-rw-r--r--  2.0 unx       49 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx      212 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1071 b- defN 24-May-08 16:46 xlineparse-0.0.4.dist-info/license_files/LICENSE
+12 files, 2336349 bytes uncompressed, 643663 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -1,37 +1,37 @@
 Filename: xlineparse/
 Comment: 
 
-Filename: xlineparse-0.0.3.dist-info/
+Filename: xlineparse-0.0.4.dist-info/
 Comment: 
 
 Filename: xlineparse.libs/
 Comment: 
 
 Filename: xlineparse/py.typed
 Comment: 
 
 Filename: xlineparse/__init__.py
 Comment: 
 
 Filename: xlineparse/xlineparse.cpython-312-i386-linux-gnu.so
 Comment: 
 
-Filename: xlineparse-0.0.3.dist-info/license_files/
+Filename: xlineparse-0.0.4.dist-info/license_files/
 Comment: 
 
-Filename: xlineparse-0.0.3.dist-info/METADATA
+Filename: xlineparse-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xlineparse-0.0.3.dist-info/RECORD
+Filename: xlineparse-0.0.4.dist-info/RECORD
 Comment: 
 
-Filename: xlineparse-0.0.3.dist-info/entry_points.txt
+Filename: xlineparse-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: xlineparse-0.0.3.dist-info/WHEEL
+Filename: xlineparse-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xlineparse-0.0.3.dist-info/license_files/LICENSE
+Filename: xlineparse-0.0.4.dist-info/license_files/LICENSE
 Comment: 
 
 Zip file comment:
```

## xlineparse/__init__.py

```diff
@@ -262,11 +262,15 @@
             parsed = self._parser.parse_line(line)
         except ValueError as e:
             raise LineParseError(f"Failed to parse line: '{line}'\n {e.args[0]}")
         if self._enum_conversions:
             first, *_ = parsed
             enum_conversion: dict[int, StrEnumField] = self._enum_conversions[first]
             parsed = tuple(
-                enum_conversion[i].cls(v) if i in enum_conversion else v
+                (
+                    enum_conversion[i].cls(v)
+                    if (v is not None and i in enum_conversion)
+                    else v
+                )
                 for i, v in enumerate(parsed)
             )
         return parsed  # type: ignore
```

## Comparing `xlineparse-0.0.3.dist-info/METADATA` & `xlineparse-0.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xlineparse
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Programming Language :: Python
 Requires-Dist: maturin ==1.4.0 ; extra == 'dev'
 Requires-Dist: pytest ==7.* ; extra == 'dev'
 Requires-Dist: mypy ==1.6.* ; extra == 'dev'
 Requires-Dist: pip ==24.0 ; extra == 'dev'
 Requires-Dist: pytest ==7.* ; extra == 'test'
 Provides-Extra: dev
```

## Comparing `xlineparse-0.0.3.dist-info/RECORD` & `xlineparse-0.0.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 xlineparse/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xlineparse/__init__.py,sha256=VQ2FP1TrW4NvpQXvoQTxXML66PjTIHNFPA5BMTuX0Rs,7541
+xlineparse/__init__.py,sha256=OevPOvXbavzGJu5873ic96OUzU7xqNFpom6VLtNqY5E,7641
 xlineparse/xlineparse.cpython-312-i386-linux-gnu.so,sha256=Z5iCTXEgl1yBonwWMretnIiWqZ3W9EwlQ1zF6CmgVFo,2324012
-xlineparse-0.0.3.dist-info/METADATA,sha256=0QV8FrOR33McrFuMT-XZgpP57yU2I5pSOQPGYcy1eTw,2674
-xlineparse-0.0.3.dist-info/RECORD,,
-xlineparse-0.0.3.dist-info/entry_points.txt,sha256=V5wyMr5vlGqrFnfZFcMHMIIEXq5C7DmJr8rizjOO_s8,49
-xlineparse-0.0.3.dist-info/WHEEL,sha256=Ae3Tfi6BqeCLKeRR5nIV4A0W4paDC7wSiuTKW2pKNx4,212
-xlineparse-0.0.3.dist-info/license_files/LICENSE,sha256=jpcl6JKJdeKotYCJv0d4vXrgrcA0qF9HpZFuHXLeAyE,1071
+xlineparse-0.0.4.dist-info/METADATA,sha256=-I8UyG7Xcebb9RNzQMfP4N3THpqNsFAdRa4cIWfr6t4,2674
+xlineparse-0.0.4.dist-info/RECORD,,
+xlineparse-0.0.4.dist-info/entry_points.txt,sha256=V5wyMr5vlGqrFnfZFcMHMIIEXq5C7DmJr8rizjOO_s8,49
+xlineparse-0.0.4.dist-info/WHEEL,sha256=Ae3Tfi6BqeCLKeRR5nIV4A0W4paDC7wSiuTKW2pKNx4,212
+xlineparse-0.0.4.dist-info/license_files/LICENSE,sha256=jpcl6JKJdeKotYCJv0d4vXrgrcA0qF9HpZFuHXLeAyE,1071
```

## Comparing `xlineparse-0.0.3.dist-info/license_files/LICENSE` & `xlineparse-0.0.4.dist-info/license_files/LICENSE`

 * *Files identical despite different names*


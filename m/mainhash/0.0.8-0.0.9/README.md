# Comparing `tmp/mainhash-0.0.8.tar.gz` & `tmp/mainhash-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainhash-0.0.8.tar", max compression
+gzip compressed data, was "mainhash-0.0.9.tar", max compression
```

## Comparing `mainhash-0.0.8.tar` & `mainhash-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1074 2024-01-28 16:44:22.000000 mainhash-0.0.8/LICENSE
--rwxr-xr-x   0        0        0     1844 2024-01-28 16:44:22.000000 mainhash-0.0.8/README.md
--rwxr-xr-x   0        0        0      616 2024-02-29 12:06:47.000000 mainhash-0.0.8/pyproject.toml
--rwxr-xr-x   0        0        0      173 2024-02-20 10:49:32.000000 mainhash-0.0.8/src/MainHash/__algs.py
--rwxr-xr-x   0        0        0     1103 2024-02-29 12:06:39.000000 mainhash-0.0.8/src/MainHash/__init__.py
--rwxr-xr-x   0        0        0      592 2024-02-20 10:59:00.000000 mainhash-0.0.8/src/MainHash/all.py
--rwxr-xr-x   0        0        0      362 2024-02-29 12:01:14.000000 mainhash-0.0.8/src/MainHash/blake2b.py
--rwxr-xr-x   0        0        0      362 2024-02-29 12:01:17.000000 mainhash-0.0.8/src/MainHash/blake2s.py
--rwxr-xr-x   0        0        0      346 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/md5.py
--rwxr-xr-x   0        0        0    10133 2024-02-29 12:06:28.000000 mainhash-0.0.8/src/MainHash/script.py
--rwxr-xr-x   0        0        0      350 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/sha1.py
--rwxr-xr-x   0        0        0      358 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/sha224.py
--rwxr-xr-x   0        0        0      358 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/sha256.py
--rwxr-xr-x   0        0        0      358 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/sha384.py
--rwxr-xr-x   0        0        0      366 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/sha3_224.py
--rwxr-xr-x   0        0        0      366 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/sha3_256.py
--rwxr-xr-x   0        0        0      366 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/sha3_384.py
--rwxr-xr-x   0        0        0      366 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/sha3_512.py
--rwxr-xr-x   0        0        0      358 2024-02-11 15:54:04.000000 mainhash-0.0.8/src/MainHash/sha512.py
--rw-r--r--   0        0        0     2541 1970-01-01 00:00:00.000000 mainhash-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-01-28 16:44:22.000000 mainhash-0.0.9/LICENSE
+-rwxr-xr-x   0        0        0     1844 2024-01-28 16:44:22.000000 mainhash-0.0.9/README.md
+-rwxr-xr-x   0        0        0      616 2024-02-29 12:30:29.000000 mainhash-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0      173 2024-02-20 10:49:32.000000 mainhash-0.0.9/src/MainHash/__algs.py
+-rwxr-xr-x   0        0        0     1103 2024-02-29 12:30:21.000000 mainhash-0.0.9/src/MainHash/__init__.py
+-rwxr-xr-x   0        0        0      592 2024-02-20 10:59:00.000000 mainhash-0.0.9/src/MainHash/all.py
+-rwxr-xr-x   0        0        0      362 2024-02-29 12:01:14.000000 mainhash-0.0.9/src/MainHash/blake2b.py
+-rwxr-xr-x   0        0        0      362 2024-02-29 12:01:16.000000 mainhash-0.0.9/src/MainHash/blake2s.py
+-rwxr-xr-x   0        0        0      346 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/md5.py
+-rwxr-xr-x   0        0        0    10191 2024-02-29 12:30:11.000000 mainhash-0.0.9/src/MainHash/script.py
+-rwxr-xr-x   0        0        0      350 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/sha1.py
+-rwxr-xr-x   0        0        0      358 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/sha224.py
+-rwxr-xr-x   0        0        0      358 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/sha256.py
+-rwxr-xr-x   0        0        0      358 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/sha384.py
+-rwxr-xr-x   0        0        0      366 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/sha3_224.py
+-rwxr-xr-x   0        0        0      366 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/sha3_256.py
+-rwxr-xr-x   0        0        0      366 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/sha3_384.py
+-rwxr-xr-x   0        0        0      366 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/sha3_512.py
+-rwxr-xr-x   0        0        0      358 2024-02-11 15:54:04.000000 mainhash-0.0.9/src/MainHash/sha512.py
+-rw-r--r--   0        0        0     2541 1970-01-01 00:00:00.000000 mainhash-0.0.9/PKG-INFO
```

### Comparing `mainhash-0.0.8/LICENSE` & `mainhash-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mainhash-0.0.8/README.md` & `mainhash-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mainhash-0.0.8/pyproject.toml` & `mainhash-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mainhash"
-version = "0.0.8"
+version = "0.0.9"
 description = "Simplifying checksum generation"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainHash.py"
 packages = [
     { include = "MainHash", from = "src" },
 ]
```

### Comparing `mainhash-0.0.8/src/MainHash/__init__.py` & `mainhash-0.0.9/src/MainHash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version_tuple__=(0,0,8)
+__version_tuple__=(0,0,9)
 import MainHash.all as all
 import MainHash.blake2b as blake2b
 import MainHash.blake2s as blake2s
 import MainHash.md5 as md5
 import MainHash.sha1 as sha1
 import MainHash.sha224 as sha224
 import MainHash.sha256 as sha256
```

### Comparing `mainhash-0.0.8/src/MainHash/all.py` & `mainhash-0.0.9/src/MainHash/all.py`

 * *Files identical despite different names*

### Comparing `mainhash-0.0.8/src/MainHash/script.py` & `mainhash-0.0.9/src/MainHash/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,18 @@
   os.chdir(path)
   path=os.getcwd()
   info=ms.path.info(path,listdir=True,listlinks=False)
   files=info["files"]
   d={}
   for i in files:
     if not i.lower().endswith(".mainhash"):
-      d[os.path.relpath(i,path)]=_genFile(i,**kwargs)
+      try:
+        d[os.path.relpath(i,path).replace("\\","/")]=_genFile(i,**kwargs)
+      except:
+        pass
   os.chdir(root)
   return d
 def _genAuto(path,**kwargs):
   type=ms.path.info(path)["type"]
   if type=="file":
     return _genFile(path,**kwargs)
   elif type=="dir":
```

### Comparing `mainhash-0.0.8/PKG-INFO` & `mainhash-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mainhash
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simplifying checksum generation
 Home-page: https://github.com/MainPlay-TG/MainHash.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


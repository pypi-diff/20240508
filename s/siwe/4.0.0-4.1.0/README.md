# Comparing `tmp/siwe-4.0.0.tar.gz` & `tmp/siwe-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siwe-4.0.0.tar", max compression
+gzip compressed data, was "siwe-4.1.0.tar", max compression
```

## Comparing `siwe-4.0.0.tar` & `siwe-4.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11355 2022-04-22 10:09:49.867220 siwe-4.0.0/LICENSE-APACHE
--rw-r--r--   0        0        0     1064 2022-04-22 10:09:49.867290 siwe-4.0.0/LICENSE-MIT
--rw-r--r--   0        0        0     2783 2024-04-29 16:35:59.509274 siwe-4.0.0/README.md
--rw-r--r--   0        0        0     1495 2024-04-29 16:35:59.514434 siwe-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      281 2023-08-23 08:06:58.068654 siwe-4.0.0/siwe/__init__.py
--rw-r--r--   0        0        0     1209 2024-04-29 16:01:00.647319 siwe-4.0.0/siwe/defs.py
--rw-r--r--   0        0        0       24 2023-08-23 08:06:58.069054 siwe-4.0.0/siwe/grammars/__init__.py
--rw-r--r--   0        0        0     1855 2024-04-29 16:01:00.647997 siwe-4.0.0/siwe/grammars/eip4361.py
--rw-r--r--   0        0        0      949 2023-08-23 08:06:58.069570 siwe-4.0.0/siwe/grammars/rfc3339.py
--rw-r--r--   0        0        0      510 2023-08-23 08:06:58.069813 siwe-4.0.0/siwe/grammars/rfc5234.py
--rw-r--r--   0        0        0     2553 2024-04-29 16:01:00.648379 siwe-4.0.0/siwe/parsed.py
--rw-r--r--   0        0        0    12065 2024-04-29 16:35:59.509902 siwe-4.0.0/siwe/siwe.py
--rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 siwe-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2022-04-22 10:09:49.867220 siwe-4.1.0/LICENSE-APACHE
+-rw-r--r--   0        0        0     1064 2022-04-22 10:09:49.867290 siwe-4.1.0/LICENSE-MIT
+-rw-r--r--   0        0        0     2783 2024-04-29 16:35:59.509274 siwe-4.1.0/README.md
+-rw-r--r--   0        0        0     1495 2024-05-08 14:25:21.041241 siwe-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      302 2024-05-08 14:25:08.100293 siwe-4.1.0/siwe/__init__.py
+-rw-r--r--   0        0        0     1209 2024-04-29 16:01:00.647319 siwe-4.1.0/siwe/defs.py
+-rw-r--r--   0        0        0       24 2023-08-23 08:06:58.069054 siwe-4.1.0/siwe/grammars/__init__.py
+-rw-r--r--   0        0        0     1855 2024-04-29 16:01:00.647997 siwe-4.1.0/siwe/grammars/eip4361.py
+-rw-r--r--   0        0        0      949 2023-08-23 08:06:58.069570 siwe-4.1.0/siwe/grammars/rfc3339.py
+-rw-r--r--   0        0        0      510 2023-08-23 08:06:58.069813 siwe-4.1.0/siwe/grammars/rfc5234.py
+-rw-r--r--   0        0        0     2553 2024-04-29 16:01:00.648379 siwe-4.1.0/siwe/parsed.py
+-rw-r--r--   0        0        0    12065 2024-04-29 16:35:59.509902 siwe-4.1.0/siwe/siwe.py
+-rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 siwe-4.1.0/PKG-INFO
```

### Comparing `siwe-4.0.0/LICENSE-APACHE` & `siwe-4.1.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `siwe-4.0.0/LICENSE-MIT` & `siwe-4.1.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `siwe-4.0.0/README.md` & `siwe-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `siwe-4.0.0/pyproject.toml` & `siwe-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "siwe"
-version = "4.0.0"
+version = "4.1.0"
 description = "A Python implementation of Sign-In with Ethereum (EIP-4361)."
 license = "MIT OR Apache-2.0"
 authors = [
   "Spruce Systems, Inc. <hello@spruceid.com>",
   "Payton Garland <payton.r.g@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `siwe-4.0.0/siwe/defs.py` & `siwe-4.1.0/siwe/defs.py`

 * *Files identical despite different names*

### Comparing `siwe-4.0.0/siwe/grammars/eip4361.py` & `siwe-4.1.0/siwe/grammars/eip4361.py`

 * *Files identical despite different names*

### Comparing `siwe-4.0.0/siwe/grammars/rfc3339.py` & `siwe-4.1.0/siwe/grammars/rfc3339.py`

 * *Files identical despite different names*

### Comparing `siwe-4.0.0/siwe/parsed.py` & `siwe-4.1.0/siwe/parsed.py`

 * *Files identical despite different names*

### Comparing `siwe-4.0.0/siwe/siwe.py` & `siwe-4.1.0/siwe/siwe.py`

 * *Files identical despite different names*

### Comparing `siwe-4.0.0/PKG-INFO` & `siwe-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siwe
-Version: 4.0.0
+Version: 4.1.0
 Summary: A Python implementation of Sign-In with Ethereum (EIP-4361).
 Home-page: https://login.xyz
 License: MIT OR Apache-2.0
 Keywords: SIWE,EIP-4361,Sign-In with Ethereum,Spruce ID
 Author: Spruce Systems, Inc.
 Author-email: hello@spruceid.com
 Requires-Python: >=3.8,<4.0
```


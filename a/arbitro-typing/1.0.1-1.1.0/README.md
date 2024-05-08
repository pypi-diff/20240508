# Comparing `tmp/arbitro_typing-1.0.1.tar.gz` & `tmp/arbitro_typing-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arbitro_typing-1.0.1.tar", max compression
+gzip compressed data, was "arbitro_typing-1.1.0.tar", max compression
```

## Comparing `arbitro_typing-1.0.1.tar` & `arbitro_typing-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-08 16:38:06.133912 arbitro_typing-1.0.1/arbitro_typing/__init__.py
--rw-r--r--   0        0        0      921 2024-05-08 16:41:57.827275 arbitro_typing-1.0.1/arbitro_typing/data_types.py
--rw-r--r--   0        0        0     1642 2024-05-08 16:42:41.112323 arbitro_typing-1.0.1/arbitro_typing/models/operations.py
--rw-r--r--   0        0        0     1097 2024-05-08 16:52:49.200238 arbitro_typing-1.0.1/LICENSE
--rw-r--r--   0        0        0      332 2024-05-08 17:06:44.070287 arbitro_typing-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 16:38:06.133912 arbitro_typing-1.0.1/README.md
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 arbitro_typing-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-08 16:38:06.133912 arbitro_typing-1.1.0/arbitro_typing/__init__.py
+-rw-r--r--   0        0        0      921 2024-05-08 16:41:57.827275 arbitro_typing-1.1.0/arbitro_typing/data_types.py
+-rw-r--r--   0        0        0     1642 2024-05-08 16:42:41.112323 arbitro_typing-1.1.0/arbitro_typing/models/operations.py
+-rw-r--r--   0        0        0     1097 2024-05-08 16:52:49.200238 arbitro_typing-1.1.0/LICENSE
+-rw-r--r--   0        0        0      332 2024-05-08 17:23:18.889298 arbitro_typing-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      159 2024-05-08 17:22:18.452296 arbitro_typing-1.1.0/README.md
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 arbitro_typing-1.1.0/PKG-INFO
```

### Comparing `arbitro_typing-1.0.1/arbitro_typing/data_types.py` & `arbitro_typing-1.1.0/arbitro_typing/data_types.py`

 * *Files identical despite different names*

### Comparing `arbitro_typing-1.0.1/arbitro_typing/models/operations.py` & `arbitro_typing-1.1.0/arbitro_typing/models/operations.py`

 * *Files identical despite different names*

### Comparing `arbitro_typing-1.0.1/LICENSE` & `arbitro_typing-1.1.0/LICENSE`

 * *Files identical despite different names*


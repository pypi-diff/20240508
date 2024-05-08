# Comparing `tmp/shitpost-0.1.0.tar.gz` & `tmp/shitpost-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shitpost-0.1.0.tar", max compression
+gzip compressed data, was "shitpost-1.0.0.tar", max compression
```

## Comparing `shitpost-0.1.0.tar` & `shitpost-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-03-25 22:14:16.911728 shitpost-0.1.0/LICENSE
--rw-r--r--   0        0        0       97 2023-03-26 00:53:33.710645 shitpost-0.1.0/README.md
--rw-r--r--   0        0        0      317 2023-03-26 00:55:15.531499 shitpost-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-25 22:21:06.452087 shitpost-0.1.0/shitpost/__init__.py
--rw-r--r--   0        0        0      560 2023-03-26 00:41:22.511464 shitpost-0.1.0/shitpost/callback.py
--rw-r--r--   0        0        0     1896 2023-03-26 00:43:25.169872 shitpost-0.1.0/shitpost/handler.py
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 shitpost-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-08 15:21:15.634178 shitpost-1.0.0/LICENSE
+-rw-r--r--   0        0        0       97 2024-05-08 15:21:15.634178 shitpost-1.0.0/README.md
+-rw-r--r--   0        0        0      317 2024-05-08 15:21:54.368683 shitpost-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 15:21:15.634178 shitpost-1.0.0/shitpost/__init__.py
+-rw-r--r--   0        0        0      560 2024-05-08 15:21:15.634178 shitpost-1.0.0/shitpost/callback.py
+-rw-r--r--   0        0        0     1896 2024-05-08 15:21:15.634178 shitpost-1.0.0/shitpost/handler.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 shitpost-1.0.0/PKG-INFO
```

### Comparing `shitpost-0.1.0/LICENSE` & `shitpost-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shitpost-0.1.0/shitpost/callback.py` & `shitpost-1.0.0/shitpost/callback.py`

 * *Files identical despite different names*

### Comparing `shitpost-0.1.0/shitpost/handler.py` & `shitpost-1.0.0/shitpost/handler.py`

 * *Files identical despite different names*


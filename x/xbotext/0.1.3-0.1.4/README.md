# Comparing `tmp/xbotext-0.1.3.tar.gz` & `tmp/xbotext-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbotext-0.1.3.tar", max compression
+gzip compressed data, was "xbotext-0.1.4.tar", max compression
```

## Comparing `xbotext-0.1.3.tar` & `xbotext-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.3/README.md
--rw-r--r--   0        0        0      255 2024-05-07 12:13:11.059635 xbotext-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.3/xbotext/__init__.py
--rw-r--r--   0        0        0     3336 2024-05-07 12:12:34.225851 xbotext-0.1.3/xbotext/cache.py
--rw-r--r--   0        0        0      522 2024-05-07 11:55:00.763736 xbotext-0.1.3/xbotext/chromium.py
--rw-r--r--   0        0        0      605 2024-05-07 11:55:00.763736 xbotext-0.1.3/xbotext/regedit.py
--rw-r--r--   0        0        0       20 2024-05-07 11:55:00.763736 xbotext-0.1.3/xbotext/sofaware.py
--rw-r--r--   0        0        0      101 2024-05-07 11:55:00.763736 xbotext-0.1.3/xbotext/system.py
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 xbotext-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-05-07 12:19:53.414568 xbotext-0.1.4/README.md
+-rw-r--r--   0        0        0      255 2024-05-07 12:25:04.258412 xbotext-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 11:55:00.752903 xbotext-0.1.4/xbotext/__init__.py
+-rw-r--r--   0        0        0     3336 2024-05-07 12:12:34.225851 xbotext-0.1.4/xbotext/cache.py
+-rw-r--r--   0        0        0      522 2024-05-07 11:55:00.763736 xbotext-0.1.4/xbotext/chromium.py
+-rw-r--r--   0        0        0       76 2024-05-07 12:23:09.391571 xbotext-0.1.4/xbotext/client.py
+-rw-r--r--   0        0        0      605 2024-05-07 11:55:00.763736 xbotext-0.1.4/xbotext/regedit.py
+-rw-r--r--   0        0        0       20 2024-05-07 11:55:00.763736 xbotext-0.1.4/xbotext/sofaware.py
+-rw-r--r--   0        0        0      101 2024-05-07 11:55:00.763736 xbotext-0.1.4/xbotext/system.py
+-rw-r--r--   0        0        0      538 2024-05-07 12:24:54.194157 xbotext-0.1.4/xbotext/web.py
+-rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 xbotext-0.1.4/PKG-INFO
```

### Comparing `xbotext-0.1.3/xbotext/cache.py` & `xbotext-0.1.4/xbotext/cache.py`

 * *Files identical despite different names*

### Comparing `xbotext-0.1.3/xbotext/chromium.py` & `xbotext-0.1.4/xbotext/chromium.py`

 * *Files identical despite different names*

### Comparing `xbotext-0.1.3/xbotext/regedit.py` & `xbotext-0.1.4/xbotext/regedit.py`

 * *Files identical despite different names*


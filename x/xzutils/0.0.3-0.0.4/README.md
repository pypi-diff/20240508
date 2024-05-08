# Comparing `tmp/xzutils-0.0.3.tar.gz` & `tmp/xzutils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xzutils-0.0.3.tar", last modified: Wed May  8 09:00:09 2024, max compression
+gzip compressed data, was "xzutils-0.0.4.tar", last modified: Wed May  8 09:23:00 2024, max compression
```

## Comparing `xzutils-0.0.3.tar` & `xzutils-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-05-08 09:00:09.691825 xzutils-0.0.3/
--rw-r--r--   0 sean      (1000) sean      (1000)      150 2024-05-08 09:00:09.691825 xzutils-0.0.3/PKG-INFO
--rw-rw-r--   0 sean      (1000) sean      (1000)       38 2024-05-08 09:00:09.691825 xzutils-0.0.3/setup.cfg
--rw-rw-r--   0 sean      (1000) sean      (1000)      487 2024-05-08 08:59:44.000000 xzutils-0.0.3/setup.py
-drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-05-08 09:00:09.691825 xzutils-0.0.3/utils/
--rwxr-xr-x   0 sean      (1000) sean      (1000)     3590 2023-11-02 06:31:32.000000 xzutils-0.0.3/utils/EncodeUtils.py
--rw-rw-r--   0 sean      (1000) sean      (1000)        0 2024-05-08 08:57:29.000000 xzutils-0.0.3/utils/__init__.py
--rwxr-xr-x   0 sean      (1000) sean      (1000)    65078 2024-05-08 08:42:29.000000 xzutils-0.0.3/utils/web3Utils.py
-drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-05-08 09:00:09.691825 xzutils-0.0.3/xzutils.egg-info/
--rw-r--r--   0 sean      (1000) sean      (1000)      150 2024-05-08 09:00:09.000000 xzutils-0.0.3/xzutils.egg-info/PKG-INFO
--rw-rw-r--   0 sean      (1000) sean      (1000)      190 2024-05-08 09:00:09.000000 xzutils-0.0.3/xzutils.egg-info/SOURCES.txt
--rw-rw-r--   0 sean      (1000) sean      (1000)        1 2024-05-08 09:00:09.000000 xzutils-0.0.3/xzutils.egg-info/dependency_links.txt
--rw-rw-r--   0 sean      (1000) sean      (1000)        6 2024-05-08 09:00:09.000000 xzutils-0.0.3/xzutils.egg-info/top_level.txt
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-05-08 09:23:00.633906 xzutils-0.0.4/
+-rw-r--r--   0 sean      (1000) sean      (1000)      150 2024-05-08 09:23:00.633906 xzutils-0.0.4/PKG-INFO
+-rw-rw-r--   0 sean      (1000) sean      (1000)       38 2024-05-08 09:23:00.633906 xzutils-0.0.4/setup.cfg
+-rw-rw-r--   0 sean      (1000) sean      (1000)      487 2024-05-08 09:17:09.000000 xzutils-0.0.4/setup.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-05-08 09:23:00.629906 xzutils-0.0.4/utils/
+-rwxr-xr-x   0 sean      (1000) sean      (1000)     3590 2023-11-02 06:31:32.000000 xzutils-0.0.4/utils/EncodeUtils.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)       51 2024-05-08 09:22:39.000000 xzutils-0.0.4/utils/__init__.py
+-rwxr-xr-x   0 sean      (1000) sean      (1000)    65078 2024-05-08 08:42:29.000000 xzutils-0.0.4/utils/web3Utils.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-05-08 09:23:00.629906 xzutils-0.0.4/xzutils.egg-info/
+-rw-r--r--   0 sean      (1000) sean      (1000)      150 2024-05-08 09:23:00.000000 xzutils-0.0.4/xzutils.egg-info/PKG-INFO
+-rw-rw-r--   0 sean      (1000) sean      (1000)      190 2024-05-08 09:23:00.000000 xzutils-0.0.4/xzutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)        1 2024-05-08 09:23:00.000000 xzutils-0.0.4/xzutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)        6 2024-05-08 09:23:00.000000 xzutils-0.0.4/xzutils.egg-info/top_level.txt
```

### Comparing `xzutils-0.0.3/utils/EncodeUtils.py` & `xzutils-0.0.4/utils/EncodeUtils.py`

 * *Files identical despite different names*

### Comparing `xzutils-0.0.3/utils/web3Utils.py` & `xzutils-0.0.4/utils/web3Utils.py`

 * *Files identical despite different names*


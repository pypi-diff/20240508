# Comparing `tmp/xzutils-0.0.1.tar.gz` & `tmp/xzutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xzutils-0.0.1.tar", last modified: Mon Apr 29 04:29:23 2024, max compression
+gzip compressed data, was "xzutils-0.0.2.tar", last modified: Wed May  8 08:44:59 2024, max compression
```

## Comparing `xzutils-0.0.1.tar` & `xzutils-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-04-29 04:29:23.815489 xzutils-0.0.1/
--rw-r--r--   0 sean      (1000) sean      (1000)      150 2024-04-29 04:29:23.815489 xzutils-0.0.1/PKG-INFO
--rw-rw-r--   0 sean      (1000) sean      (1000)       38 2024-04-29 04:29:23.815489 xzutils-0.0.1/setup.cfg
--rw-rw-r--   0 sean      (1000) sean      (1000)      456 2024-04-29 04:21:48.000000 xzutils-0.0.1/setup.py
-drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-04-29 04:29:23.815489 xzutils-0.0.1/xzutils.egg-info/
--rw-r--r--   0 sean      (1000) sean      (1000)      150 2024-04-29 04:29:23.000000 xzutils-0.0.1/xzutils.egg-info/PKG-INFO
--rw-rw-r--   0 sean      (1000) sean      (1000)      132 2024-04-29 04:29:23.000000 xzutils-0.0.1/xzutils.egg-info/SOURCES.txt
--rw-rw-r--   0 sean      (1000) sean      (1000)        1 2024-04-29 04:29:23.000000 xzutils-0.0.1/xzutils.egg-info/dependency_links.txt
--rw-rw-r--   0 sean      (1000) sean      (1000)        1 2024-04-29 04:29:23.000000 xzutils-0.0.1/xzutils.egg-info/top_level.txt
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-05-08 08:44:59.141838 xzutils-0.0.2/
+-rw-r--r--   0 sean      (1000) sean      (1000)      150 2024-05-08 08:44:59.141838 xzutils-0.0.2/PKG-INFO
+-rw-rw-r--   0 sean      (1000) sean      (1000)       38 2024-05-08 08:44:59.141838 xzutils-0.0.2/setup.cfg
+-rw-rw-r--   0 sean      (1000) sean      (1000)      456 2024-05-08 08:44:54.000000 xzutils-0.0.2/setup.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-05-08 08:44:59.141838 xzutils-0.0.2/utils/
+-rwxr-xr-x   0 sean      (1000) sean      (1000)     3590 2023-11-02 06:31:32.000000 xzutils-0.0.2/utils/EncodeUtils.py
+-rw-rw-r--   0 sean      (1000) sean      (1000)        0 2024-05-08 08:41:24.000000 xzutils-0.0.2/utils/__init__.py
+-rwxr-xr-x   0 sean      (1000) sean      (1000)    65078 2024-05-08 08:42:29.000000 xzutils-0.0.2/utils/web3Utils.py
+drwxrwxr-x   0 sean      (1000) sean      (1000)        0 2024-05-08 08:44:59.141838 xzutils-0.0.2/xzutils.egg-info/
+-rw-r--r--   0 sean      (1000) sean      (1000)      150 2024-05-08 08:44:59.000000 xzutils-0.0.2/xzutils.egg-info/PKG-INFO
+-rw-rw-r--   0 sean      (1000) sean      (1000)      190 2024-05-08 08:44:59.000000 xzutils-0.0.2/xzutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)        1 2024-05-08 08:44:59.000000 xzutils-0.0.2/xzutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sean      (1000) sean      (1000)        6 2024-05-08 08:44:59.000000 xzutils-0.0.2/xzutils.egg-info/top_level.txt
```


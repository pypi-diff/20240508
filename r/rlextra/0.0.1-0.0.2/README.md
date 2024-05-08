# Comparing `tmp/rlextra-0.0.1.tar.gz` & `tmp/rlextra-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlextra-0.0.1.tar", last modified: Wed May  8 06:31:59 2024, max compression
+gzip compressed data, was "rlextra-0.0.2.tar", last modified: Wed May  8 21:22:44 2024, max compression
```

## Comparing `rlextra-0.0.1.tar` & `rlextra-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2024-05-08 06:31:59.517454 rlextra-0.0.1/
--rw-r--r--   0 josh       (502) staff       (20)      836 2024-05-08 06:31:59.517233 rlextra-0.0.1/PKG-INFO
--rw-r--r--   0 josh       (502) staff       (20)       14 2024-05-08 06:22:45.000000 rlextra-0.0.1/README.md
--rw-r--r--   0 josh       (502) staff       (20)     1054 2024-05-08 06:28:35.000000 rlextra-0.0.1/pyproject.toml
--rw-r--r--   0 josh       (502) staff       (20)       38 2024-05-08 06:31:59.517497 rlextra-0.0.1/setup.cfg
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2024-05-08 06:31:59.514187 rlextra-0.0.1/src/
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2024-05-08 06:31:59.515296 rlextra-0.0.1/src/rlextra/
--rw-r--r--   0 josh       (502) staff       (20)        0 2024-05-08 06:26:29.000000 rlextra-0.0.1/src/rlextra/__init__.py
--rw-r--r--   0 josh       (502) staff       (20)       47 2024-05-08 06:27:10.000000 rlextra-0.0.1/src/rlextra/main.py
--rw-r--r--   0 josh       (502) staff       (20)        0 2024-05-08 06:22:25.000000 rlextra-0.0.1/src/rlextra/py.typed
-drwxr-xr-x   0 josh       (502) staff       (20)        0 2024-05-08 06:31:59.517006 rlextra-0.0.1/src/rlextra.egg-info/
--rw-r--r--   0 josh       (502) staff       (20)      836 2024-05-08 06:31:59.000000 rlextra-0.0.1/src/rlextra.egg-info/PKG-INFO
--rw-r--r--   0 josh       (502) staff       (20)      263 2024-05-08 06:31:59.000000 rlextra-0.0.1/src/rlextra.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (502) staff       (20)        1 2024-05-08 06:31:59.000000 rlextra-0.0.1/src/rlextra.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (502) staff       (20)       10 2024-05-08 06:31:59.000000 rlextra-0.0.1/src/rlextra.egg-info/requires.txt
--rw-r--r--   0 josh       (502) staff       (20)        8 2024-05-08 06:31:59.000000 rlextra-0.0.1/src/rlextra.egg-info/top_level.txt
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 21:22:44.108762 rlextra-0.0.2/
+-rw-r--r--   0 andy       (501) staff       (20)      381 2024-05-08 21:22:44.108655 rlextra-0.0.2/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-08 21:22:44.108802 rlextra-0.0.2/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)     1738 2024-05-08 21:14:18.000000 rlextra-0.0.2/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 21:22:44.107702 rlextra-0.0.2/src/
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 21:22:44.107896 rlextra-0.0.2/src/rlextra/
+-rw-r--r--   0 andy       (501) staff       (20)      288 2024-05-08 21:14:18.000000 rlextra-0.0.2/src/rlextra/__init__.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-08 21:22:44.108504 rlextra-0.0.2/src/rlextra.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)      381 2024-05-08 21:22:44.000000 rlextra-0.0.2/src/rlextra.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      206 2024-05-08 21:22:44.000000 rlextra-0.0.2/src/rlextra.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-08 21:22:44.000000 rlextra-0.0.2/src/rlextra.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       17 2024-05-08 21:22:44.000000 rlextra-0.0.2/src/rlextra.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)        8 2024-05-08 21:22:44.000000 rlextra-0.0.2/src/rlextra.egg-info/top_level.txt
```


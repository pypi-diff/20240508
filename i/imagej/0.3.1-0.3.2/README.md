# Comparing `tmp/imagej-0.3.1.tar.gz` & `tmp/imagej-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imagej-0.3.1.tar", last modified: Wed Oct 24 16:53:26 2018, max compression
+gzip compressed data, was "imagej-0.3.2.tar", last modified: Wed May  8 19:28:24 2024, max compression
```

## Comparing `imagej-0.3.1.tar` & `imagej-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,11 @@
-drwxr-xr-x   0 curtis     (503) staff       (20)        0 2018-10-24 16:53:26.000000 imagej-0.3.1/
--rw-r--r--   0 curtis     (503) staff       (20)      609 2018-05-18 05:52:55.000000 imagej-0.3.1/LICENSE.txt
--rw-r--r--   0 curtis     (503) staff       (20)       95 2018-05-18 05:52:55.000000 imagej-0.3.1/MANIFEST.in
--rw-r--r--   0 curtis     (503) staff       (20)     2582 2018-10-24 16:53:26.000000 imagej-0.3.1/PKG-INFO
--rw-r--r--   0 curtis     (503) staff       (20)     1791 2018-10-11 19:34:32.000000 imagej-0.3.1/README.md
-drwxr-xr-x   0 curtis     (503) staff       (20)        0 2018-10-24 16:53:26.000000 imagej-0.3.1/imagej/
--rw-r--r--   0 curtis     (503) staff       (20)       23 2018-05-18 05:52:55.000000 imagej-0.3.1/imagej/__init__.py
--rw-r--r--   0 curtis     (503) staff       (20)     2033 2018-10-24 16:52:46.000000 imagej-0.3.1/imagej/imagej.py
-drwxr-xr-x   0 curtis     (503) staff       (20)        0 2018-10-24 16:53:26.000000 imagej-0.3.1/imagej.egg-info/
--rw-r--r--   0 curtis     (503) staff       (20)     2582 2018-10-24 16:53:26.000000 imagej-0.3.1/imagej.egg-info/PKG-INFO
--rw-r--r--   0 curtis     (503) staff       (20)      269 2018-10-24 16:53:26.000000 imagej-0.3.1/imagej.egg-info/SOURCES.txt
--rw-r--r--   0 curtis     (503) staff       (20)        1 2018-10-24 16:53:26.000000 imagej-0.3.1/imagej.egg-info/dependency_links.txt
--rw-r--r--   0 curtis     (503) staff       (20)        7 2018-10-24 16:53:26.000000 imagej-0.3.1/imagej.egg-info/top_level.txt
--rw-r--r--   0 curtis     (503) staff       (20)       29 2018-10-11 19:03:09.000000 imagej-0.3.1/requirements.txt
--rw-r--r--   0 curtis     (503) staff       (20)       34 2018-05-18 05:52:55.000000 imagej-0.3.1/server_requirements.txt
--rw-r--r--   0 curtis     (503) staff       (20)       79 2018-10-24 16:53:26.000000 imagej-0.3.1/setup.cfg
--rw-r--r--   0 curtis     (503) staff       (20)      581 2018-10-24 16:52:49.000000 imagej-0.3.1/setup.py
-drwxr-xr-x   0 curtis     (503) staff       (20)        0 2018-10-24 16:53:26.000000 imagej-0.3.1/test/
--rw-r--r--   0 curtis     (503) staff       (20)     3068 2018-05-18 05:52:55.000000 imagej-0.3.1/test/test_imagej.py
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2024-05-08 19:28:24.396828 imagej-0.3.2/
+-rw-r--r--   0 edward    (1000) edward    (1000)      368 2024-05-08 19:28:24.396828 imagej-0.3.2/PKG-INFO
+-rw-rw-r--   0 edward    (1000) edward    (1000)      174 2024-05-08 19:25:00.000000 imagej-0.3.2/README.md
+drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2024-05-08 19:28:24.396828 imagej-0.3.2/imagej.egg-info/
+-rw-r--r--   0 edward    (1000) edward    (1000)      368 2024-05-08 19:28:24.000000 imagej-0.3.2/imagej.egg-info/PKG-INFO
+-rw-rw-r--   0 edward    (1000) edward    (1000)      167 2024-05-08 19:28:24.000000 imagej-0.3.2/imagej.egg-info/SOURCES.txt
+-rw-rw-r--   0 edward    (1000) edward    (1000)        1 2024-05-08 19:28:24.000000 imagej-0.3.2/imagej.egg-info/dependency_links.txt
+-rw-rw-r--   0 edward    (1000) edward    (1000)        9 2024-05-08 19:28:24.000000 imagej-0.3.2/imagej.egg-info/requires.txt
+-rw-rw-r--   0 edward    (1000) edward    (1000)        1 2024-05-08 19:28:24.000000 imagej-0.3.2/imagej.egg-info/top_level.txt
+-rw-rw-r--   0 edward    (1000) edward    (1000)       38 2024-05-08 19:28:24.396828 imagej-0.3.2/setup.cfg
+-rw-rw-r--   0 edward    (1000) edward    (1000)      525 2024-05-08 19:23:53.000000 imagej-0.3.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```


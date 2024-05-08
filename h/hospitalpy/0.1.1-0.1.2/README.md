# Comparing `tmp/hospitalpy-0.1.1.tar.gz` & `tmp/hospitalpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hospitalpy-0.1.1.tar", last modified: Tue May  7 22:41:57 2024, max compression
+gzip compressed data, was "hospitalpy-0.1.2.tar", last modified: Tue May  7 23:28:43 2024, max compression
```

## Comparing `hospitalpy-0.1.1.tar` & `hospitalpy-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-07 22:41:57.639615 hospitalpy-0.1.1/
--rw-r--r--   0 michaelchary   (501) staff       (20)      316 2024-05-07 22:41:57.639442 hospitalpy-0.1.1/PKG-INFO
--rw-r--r--   0 michaelchary   (501) staff       (20)        5 2024-05-01 20:53:36.000000 hospitalpy-0.1.1/README.md
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-07 22:41:57.639269 hospitalpy-0.1.1/hospitalpy.egg-info/
--rw-r--r--   0 michaelchary   (501) staff       (20)      316 2024-05-07 22:41:57.000000 hospitalpy-0.1.1/hospitalpy.egg-info/PKG-INFO
--rw-r--r--   0 michaelchary   (501) staff       (20)      169 2024-05-07 22:41:57.000000 hospitalpy-0.1.1/hospitalpy.egg-info/SOURCES.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-07 22:41:57.000000 hospitalpy-0.1.1/hospitalpy.egg-info/dependency_links.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-07 22:41:57.000000 hospitalpy-0.1.1/hospitalpy.egg-info/top_level.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)      419 2024-05-07 22:41:54.000000 hospitalpy-0.1.1/pyproject.toml
--rw-r--r--   0 michaelchary   (501) staff       (20)       38 2024-05-07 22:41:57.639655 hospitalpy-0.1.1/setup.cfg
--rw-r--r--   0 michaelchary   (501) staff       (20)      534 2024-05-07 22:39:19.000000 hospitalpy-0.1.1/setup.py
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-07 23:28:43.735771 hospitalpy-0.1.2/
+-rw-r--r--   0 michaelchary   (501) staff       (20)      359 2024-05-07 23:28:43.735570 hospitalpy-0.1.2/PKG-INFO
+-rw-r--r--   0 michaelchary   (501) staff       (20)        5 2024-05-01 20:53:36.000000 hospitalpy-0.1.2/README.md
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-07 23:28:43.735388 hospitalpy-0.1.2/hospitalpy.egg-info/
+-rw-r--r--   0 michaelchary   (501) staff       (20)      359 2024-05-07 23:28:43.000000 hospitalpy-0.1.2/hospitalpy.egg-info/PKG-INFO
+-rw-r--r--   0 michaelchary   (501) staff       (20)      202 2024-05-07 23:28:43.000000 hospitalpy-0.1.2/hospitalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-07 23:28:43.000000 hospitalpy-0.1.2/hospitalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)       13 2024-05-07 23:28:43.000000 hospitalpy-0.1.2/hospitalpy.egg-info/requires.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-07 23:28:43.000000 hospitalpy-0.1.2/hospitalpy.egg-info/top_level.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)      454 2024-05-07 23:28:40.000000 hospitalpy-0.1.2/pyproject.toml
+-rw-r--r--   0 michaelchary   (501) staff       (20)       38 2024-05-07 23:28:43.735808 hospitalpy-0.1.2/setup.cfg
+-rw-r--r--   0 michaelchary   (501) staff       (20)      492 2024-05-07 23:04:38.000000 hospitalpy-0.1.2/setup.py
```


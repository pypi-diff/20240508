# Comparing `tmp/grasp_planning-0.2.tar.gz` & `tmp/grasp_planning-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.2.tar", last modified: Wed May  8 08:15:45 2024, max compression
+gzip compressed data, was "grasp_planning-0.3.tar", last modified: Wed May  8 08:20:04 2024, max compression
```

## Comparing `grasp_planning-0.2.tar` & `grasp_planning-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:15:45.310712 grasp_planning-0.2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2024-05-08 08:15:45.310712 grasp_planning-0.2/PKG-INFO
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:15:45.310712 grasp_planning-0.2/grasp_planning/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2024-05-07 16:34:01.000000 grasp_planning-0.2/grasp_planning/__init__.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:15:45.310712 grasp_planning-0.2/grasp_planning.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      224 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       75 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/top_level.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-08 08:15:45.310712 grasp_planning-0.2/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      676 2024-05-08 08:15:42.000000 grasp_planning-0.2/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:20:04.272701 grasp_planning-0.3/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2024-05-08 08:20:04.272701 grasp_planning-0.3/PKG-INFO
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:20:04.272701 grasp_planning-0.3/grasp_planning/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2024-05-07 16:34:01.000000 grasp_planning-0.3/grasp_planning/__init__.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:20:04.272701 grasp_planning-0.3/grasp_planning.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2024-05-08 08:20:04.000000 grasp_planning-0.3/grasp_planning.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      224 2024-05-08 08:20:04.000000 grasp_planning-0.3/grasp_planning.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-08 08:20:04.000000 grasp_planning-0.3/grasp_planning.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       75 2024-05-08 08:20:04.000000 grasp_planning-0.3/grasp_planning.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2024-05-08 08:20:04.000000 grasp_planning-0.3/grasp_planning.egg-info/top_level.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-08 08:20:04.272701 grasp_planning-0.3/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      684 2024-05-08 08:20:01.000000 grasp_planning-0.3/setup.py
```


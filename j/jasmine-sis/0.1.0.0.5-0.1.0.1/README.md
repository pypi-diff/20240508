# Comparing `tmp/jasmine_sis-0.1.0.0.5.tar.gz` & `tmp/jasmine_sis-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jasmine_sis-0.1.0.0.5.tar", last modified: Tue May  7 21:10:26 2024, max compression
+gzip compressed data, was "jasmine_sis-0.1.0.1.tar", last modified: Tue May  7 20:53:46 2024, max compression
```

## Comparing `jasmine_sis-0.1.0.0.5.tar` & `jasmine_sis-0.1.0.1.tar`

### file list

```diff
@@ -1,21 +1,13 @@
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 21:10:26.499416 jasmine_sis-0.1.0.0.5/
--rw-r--r--   0 sishitan (344948379) staff       (20)     1065 2024-04-17 18:49:24.000000 jasmine_sis-0.1.0.0.5/LICENSE
--rw-r--r--   0 sishitan (344948379) staff       (20)      437 2024-05-07 21:10:26.498656 jasmine_sis-0.1.0.0.5/PKG-INFO
--rw-r--r--   0 sishitan (344948379) staff       (20)     2077 2024-05-01 23:08:17.000000 jasmine_sis-0.1.0.0.5/README.md
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 21:10:26.487858 jasmine_sis-0.1.0.0.5/jasmine/
--rw-r--r--   0 sishitan (344948379) staff       (20)        0 2024-03-22 15:18:25.000000 jasmine_sis-0.1.0.0.5/jasmine/__init__.py
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 21:10:26.492360 jasmine_sis-0.1.0.0.5/jasmine/files_organizer/
--rw-r--r--   0 sishitan (344948379) staff       (20)        0 2024-03-22 15:18:25.000000 jasmine_sis-0.1.0.0.5/jasmine/files_organizer/__init__.py
--rw-r--r--   0 sishitan (344948379) staff       (20)     5001 2024-04-26 17:04:14.000000 jasmine_sis-0.1.0.0.5/jasmine/files_organizer/data_challenge_prep.py
--rw-r--r--   0 sishitan (344948379) staff       (20)     3679 2024-04-26 17:31:20.000000 jasmine_sis-0.1.0.0.5/jasmine/files_organizer/data_challenge_reader.py
--rw-r--r--   0 sishitan (344948379) staff       (20)    15432 2024-05-07 20:44:39.000000 jasmine_sis-0.1.0.0.5/jasmine/files_organizer/lightcurve_cls.py
--rw-r--r--   0 sishitan (344948379) staff       (20)       29 2024-04-17 22:37:22.000000 jasmine_sis-0.1.0.0.5/jasmine/files_organizer/plasticc_files_reader.py
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 21:10:26.497677 jasmine_sis-0.1.0.0.5/jasmine_sis.egg-info/
--rw-r--r--   0 sishitan (344948379) staff       (20)      437 2024-05-07 21:10:26.000000 jasmine_sis-0.1.0.0.5/jasmine_sis.egg-info/PKG-INFO
--rw-r--r--   0 sishitan (344948379) staff       (20)      477 2024-05-07 21:10:26.000000 jasmine_sis-0.1.0.0.5/jasmine_sis.egg-info/SOURCES.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 21:10:26.000000 jasmine_sis-0.1.0.0.5/jasmine_sis.egg-info/dependency_links.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:48:18.000000 jasmine_sis-0.1.0.0.5/jasmine_sis.egg-info/not-zip-safe
--rw-r--r--   0 sishitan (344948379) staff       (20)       81 2024-05-07 21:10:26.000000 jasmine_sis-0.1.0.0.5/jasmine_sis.egg-info/requires.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)        8 2024-05-07 21:10:26.000000 jasmine_sis-0.1.0.0.5/jasmine_sis.egg-info/top_level.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)       38 2024-05-07 21:10:26.499621 jasmine_sis-0.1.0.0.5/setup.cfg
--rw-r--r--   0 sishitan (344948379) staff       (20)      656 2024-05-07 21:10:25.000000 jasmine_sis-0.1.0.0.5/setup.py
+drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 20:53:46.324549 jasmine_sis-0.1.0.1/
+-rw-r--r--   0 sishitan (344948379) staff       (20)     1065 2024-04-17 18:49:24.000000 jasmine_sis-0.1.0.1/LICENSE
+-rw-r--r--   0 sishitan (344948379) staff       (20)      435 2024-05-07 20:53:46.324005 jasmine_sis-0.1.0.1/PKG-INFO
+-rw-r--r--   0 sishitan (344948379) staff       (20)     2077 2024-05-01 23:08:17.000000 jasmine_sis-0.1.0.1/README.md
+drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 20:53:46.323357 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/
+-rw-r--r--   0 sishitan (344948379) staff       (20)      435 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/PKG-INFO
+-rw-r--r--   0 sishitan (344948379) staff       (20)      234 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/SOURCES.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/dependency_links.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:48:18.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/not-zip-safe
+-rw-r--r--   0 sishitan (344948379) staff       (20)       81 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/requires.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)        8 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/top_level.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)       38 2024-05-07 20:53:46.324662 jasmine_sis-0.1.0.1/setup.cfg
+-rw-r--r--   0 sishitan (344948379) staff       (20)      611 2024-05-07 20:53:41.000000 jasmine_sis-0.1.0.1/setup.py
```

### Comparing `jasmine_sis-0.1.0.0.5/LICENSE` & `jasmine_sis-0.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jasmine_sis-0.1.0.0.5/README.md` & `jasmine_sis-0.1.0.1/README.md`

 * *Files identical despite different names*


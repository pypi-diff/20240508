# Comparing `tmp/igc_processor-0.1.0.tar.gz` & `tmp/igc_processor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igc_processor-0.1.0.tar", max compression
+gzip compressed data, was "igc_processor-0.1.1.tar", max compression
```

## Comparing `igc_processor-0.1.0.tar` & `igc_processor-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1067 2024-05-06 14:05:10.286690 igc_processor-0.1.0/LICENSE
--rw-r--r--   0        0        0       15 2024-05-06 14:05:10.286690 igc_processor-0.1.0/README.md
--rw-r--r--   0        0        0      496 2024-05-06 14:05:10.286690 igc_processor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 14:05:10.286690 igc_processor-0.1.0/src/igc_processor/__init__.py
--rw-r--r--   0        0        0     4343 2024-05-06 14:05:10.286690 igc_processor-0.1.0/src/igc_processor/parser.py
--rw-r--r--   0        0        0      290 2024-05-06 14:05:10.286690 igc_processor-0.1.0/src/igc_processor/util.py
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 igc_processor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-08 13:43:02.877505 igc_processor-0.1.1/LICENSE
+-rw-r--r--   0        0        0      803 2024-05-08 13:43:02.877505 igc_processor-0.1.1/README.md
+-rw-r--r--   0        0        0      555 2024-05-08 13:43:02.877505 igc_processor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 13:43:02.877505 igc_processor-0.1.1/src/igc_processor/__init__.py
+-rw-r--r--   0        0        0     2398 2024-05-08 13:43:02.877505 igc_processor-0.1.1/src/igc_processor/circling.py
+-rw-r--r--   0        0        0     4343 2024-05-08 13:43:02.877505 igc_processor-0.1.1/src/igc_processor/parser.py
+-rw-r--r--   0        0        0      290 2024-05-08 13:43:02.877505 igc_processor-0.1.1/src/igc_processor/util.py
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 igc_processor-0.1.1/PKG-INFO
```

### Comparing `igc_processor-0.1.0/LICENSE` & `igc_processor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `igc_processor-0.1.0/src/igc_processor/parser.py` & `igc_processor-0.1.1/src/igc_processor/parser.py`

 * *Files identical despite different names*


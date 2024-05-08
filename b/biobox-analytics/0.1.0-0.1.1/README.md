# Comparing `tmp/biobox_analytics-0.1.0.tar.gz` & `tmp/biobox_analytics-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobox_analytics-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "biobox_analytics-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `biobox_analytics-0.1.0.tar` & `biobox_analytics-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,10 @@
--rw-r--r--   0        0        0     9161 2024-05-06 14:31:32.868808 biobox_analytics-0.1.0/LICENSE
--rw-r--r--   0        0        0       51 2024-05-06 14:39:27.028900 biobox_analytics-0.1.0/biobox_analytics/__init__.py
--rw-r--r--   0        0        0      406 2024-05-06 14:30:24.157072 biobox_analytics-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      277 1970-01-01 00:00:00.000000 biobox_analytics-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     9161 2024-05-06 14:31:32.868808 biobox_analytics-0.1.1/LICENSE
+-rw-r--r--   0        0        0       51 2024-05-08 15:37:10.426554 biobox_analytics-0.1.1/biobox_analytics/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-07 00:33:05.027289 biobox_analytics-0.1.1/biobox_analytics/_setup.py
+-rw-r--r--   0        0        0      116 2024-05-07 14:41:42.381803 biobox_analytics-0.1.1/biobox_analytics/core/__init__.py
+-rw-r--r--   0        0        0      648 2024-05-08 14:46:49.080065 biobox_analytics-0.1.1/biobox_analytics/core/_concept.py
+-rw-r--r--   0        0        0     3690 2024-05-08 15:30:27.110573 biobox_analytics-0.1.1/biobox_analytics/core/_node.py
+-rw-r--r--   0        0        0       48 2024-05-07 02:14:39.211578 biobox_analytics-0.1.1/biobox_analytics/integrations/__init__.py
+-rw-r--r--   0        0        0     2008 2024-05-08 14:47:54.801429 biobox_analytics-0.1.1/biobox_analytics/integrations/_lamindb.py
+-rw-r--r--   0        0        0      406 2024-05-06 14:30:24.157072 biobox_analytics-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      277 1970-01-01 00:00:00.000000 biobox_analytics-0.1.1/PKG-INFO
```

### Comparing `biobox_analytics-0.1.0/LICENSE` & `biobox_analytics-0.1.1/LICENSE`

 * *Files identical despite different names*


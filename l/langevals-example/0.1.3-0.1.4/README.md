# Comparing `tmp/langevals_example-0.1.3.tar.gz` & `tmp/langevals_example-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_example-0.1.3.tar", max compression
+gzip compressed data, was "langevals_example-0.1.4.tar", max compression
```

## Comparing `langevals_example-0.1.3.tar` & `langevals_example-0.1.4.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     2204 2024-05-07 14:19:44.470403 langevals_example-0.1.3/langevals_example/word_count.py
--rw-r--r--   0        0        0      438 2024-05-07 14:20:32.258737 langevals_example-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 langevals_example-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2204 2024-05-08 10:17:41.368534 langevals_example-0.1.4/langevals_example/word_count.py
+-rw-r--r--   0        0        0      438 2024-05-08 10:18:18.964886 langevals_example-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 langevals_example-0.1.4/PKG-INFO
```

### Comparing `langevals_example-0.1.3/langevals_example/word_count.py` & `langevals_example-0.1.4/langevals_example/word_count.py`

 * *Files identical despite different names*


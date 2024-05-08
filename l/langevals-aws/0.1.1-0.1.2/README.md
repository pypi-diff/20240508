# Comparing `tmp/langevals_aws-0.1.1.tar.gz` & `tmp/langevals_aws-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langevals_aws-0.1.1.tar", max compression
+gzip compressed data, was "langevals_aws-0.1.2.tar", max compression
```

## Comparing `langevals_aws-0.1.1.tar` & `langevals_aws-0.1.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     6660 2024-04-28 13:24:54.112394 langevals_aws-0.1.1/langevals_aws/comprehend_pii_detection.py
--rw-r--r--   0        0        0      452 2024-04-28 13:25:21.412479 langevals_aws-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 langevals_aws-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6660 2024-05-07 14:19:44.466403 langevals_aws-0.1.2/langevals_aws/comprehend_pii_detection.py
+-rw-r--r--   0        0        0      452 2024-05-07 14:20:18.550662 langevals_aws-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 langevals_aws-0.1.2/PKG-INFO
```

### Comparing `langevals_aws-0.1.1/langevals_aws/comprehend_pii_detection.py` & `langevals_aws-0.1.2/langevals_aws/comprehend_pii_detection.py`

 * *Files identical despite different names*


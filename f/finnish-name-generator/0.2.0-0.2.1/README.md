# Comparing `tmp/finnish_name_generator-0.2.0.tar.gz` & `tmp/finnish_name_generator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finnish_name_generator-0.2.0.tar", max compression
+gzip compressed data, was "finnish_name_generator-0.2.1.tar", max compression
```

## Comparing `finnish_name_generator-0.2.0.tar` & `finnish_name_generator-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0       25 1970-01-01 00:00:01.000000 finnish_name_generator-0.2.0/README.md
--rw-r--r--   0        0        0      415 1970-01-01 00:00:01.000000 finnish_name_generator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    11921 1970-01-01 00:00:01.000000 finnish_name_generator-0.2.0/src/finnish_name_generator/__init__.py
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 finnish_name_generator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       25 1970-01-01 00:00:01.000000 finnish_name_generator-0.2.1/README.md
+-rw-r--r--   0        0        0      415 1970-01-01 00:00:01.000000 finnish_name_generator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11921 1970-01-01 00:00:01.000000 finnish_name_generator-0.2.1/src/finnish_name_generator/__init__.py
+-rw-r--r--   0        0        0        0 1970-01-01 00:00:01.000000 finnish_name_generator-0.2.1/src/finnish_name_generator/py.typed
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 finnish_name_generator-0.2.1/PKG-INFO
```

### Comparing `finnish_name_generator-0.2.0/src/finnish_name_generator/__init__.py` & `finnish_name_generator-0.2.1/src/finnish_name_generator/__init__.py`

 * *Files identical despite different names*


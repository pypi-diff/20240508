# Comparing `tmp/chyllonge-1.0.5.tar.gz` & `tmp/chyllonge-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyllonge-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "chyllonge-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `chyllonge-1.0.5.tar` & `chyllonge-1.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1683 2024-05-06 20:30:37.317316 chyllonge-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0     2282 2024-05-06 20:30:37.317316 chyllonge-1.0.5/README.md
--rw-r--r--   0        0        0     1140 2024-05-06 20:30:37.813314 chyllonge-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 20:30:37.317316 chyllonge-1.0.5/src/chyllonge/__init__.py
--rw-r--r--   0        0        0    40100 2024-05-06 20:30:37.317316 chyllonge-1.0.5/src/chyllonge/api.py
--rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 chyllonge-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1683 2024-05-08 00:32:31.306919 chyllonge-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     3833 2024-05-08 00:32:31.306919 chyllonge-1.0.6/README.md
+-rw-r--r--   0        0        0     1140 2024-05-08 00:32:31.646918 chyllonge-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 00:32:31.306919 chyllonge-1.0.6/src/chyllonge/__init__.py
+-rw-r--r--   0        0        0    40100 2024-05-08 00:32:31.306919 chyllonge-1.0.6/src/chyllonge/api.py
+-rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 chyllonge-1.0.6/PKG-INFO
```

### Comparing `chyllonge-1.0.5/LICENSE.txt` & `chyllonge-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chyllonge-1.0.5/pyproject.toml` & `chyllonge-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "chyllonge"
-version = "1.0.5"
+version = "1.0.6"
 dependencies = ["tzlocal>=5.2", "requests>=2.31.0"]
 requires-python = ">=3.8"
 authors = [{name = "Alex Fredrickson", email = "alex.q.fredrickson@gmail.com"}]
 maintainers = [{name = "Alex Fredrickson", email = "alex.q.fredrickson@gmail.com"}]
 description = "A Python 3.8+ implementation of the challonge.com API."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
```

### Comparing `chyllonge-1.0.5/src/chyllonge/api.py` & `chyllonge-1.0.6/src/chyllonge/api.py`

 * *Files identical despite different names*


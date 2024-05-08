# Comparing `tmp/slalom_tapdance-1.0.1.dev65.tar.gz` & `tmp/slalom_tapdance-1.0.1.dev67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.1.dev65.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.1.dev67.tar", max compression
```

## Comparing `slalom_tapdance-1.0.1.dev65.tar` & `slalom_tapdance-1.0.1.dev67.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-08 19:41:56.862862 slalom_tapdance-1.0.1.dev65/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-08 19:42:12.583038 slalom_tapdance-1.0.1.dev65/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/install_helper.py
--rw-r--r--   0        0        0    38160 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/states.py
--rw-r--r--   0        0        0    12133 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev65/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-08 20:38:58.029229 slalom_tapdance-1.0.1.dev67/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-08 20:39:23.293231 slalom_tapdance-1.0.1.dev67/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38121 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/states.py
+-rw-r--r--   0        0        0    12133 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev67/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.1.dev65/LICENSE` & `slalom_tapdance-1.0.1.dev67/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev65/pyproject.toml` & `slalom_tapdance-1.0.1.dev67/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.1-dev.65"
+version = "1.0.1-dev.67"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.1.dev65/tapdance/cli.py` & `slalom_tapdance-1.0.1.dev67/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev65/tapdance/config.py` & `slalom_tapdance-1.0.1.dev67/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev65/tapdance/docker.py` & `slalom_tapdance-1.0.1.dev67/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev65/tapdance/install_helper.py` & `slalom_tapdance-1.0.1.dev67/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev65/tapdance/plans.py` & `slalom_tapdance-1.0.1.dev67/tapdance/plans.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,14 @@
                     if metadata.get("valid-replication-keys")
                     else "blank"
                 )
                 + ")"
             )
             metadata["valid-replication-keys"] = table_plan["replication_key"]
             metadata["replication-key"] = table_plan["replication_key"][0]
-            metadata["parent"] = 'yes'
 
 
 def _get_catalog_file_keys(
     key_type: str,
     matches: Dict[str, Dict[str, bool]],
     matched_stream_ids: Dict[str, str],
     catalog_file: str,
```

### Comparing `slalom_tapdance-1.0.1.dev65/tapdance/states.py` & `slalom_tapdance-1.0.1.dev67/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev65/tapdance/syncs.py` & `slalom_tapdance-1.0.1.dev67/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev65/PKG-INFO` & `slalom_tapdance-1.0.1.dev67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.1.dev65
+Version: 1.0.1.dev67
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/slalom_tapdance-1.0.1.dev64.tar.gz` & `tmp/slalom_tapdance-1.0.1.dev65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.1.dev64.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.1.dev65.tar", max compression
```

## Comparing `slalom_tapdance-1.0.1.dev64.tar` & `slalom_tapdance-1.0.1.dev65.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-08 17:43:14.385614 slalom_tapdance-1.0.1.dev64/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/install_helper.py
--rw-r--r--   0        0        0    38145 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/states.py
--rw-r--r--   0        0        0    12133 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev64/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-08 19:41:56.862862 slalom_tapdance-1.0.1.dev65/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-08 19:42:12.583038 slalom_tapdance-1.0.1.dev65/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38160 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/states.py
+-rw-r--r--   0        0        0    12133 2024-05-08 19:41:56.866862 slalom_tapdance-1.0.1.dev65/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev65/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.1.dev64/LICENSE` & `slalom_tapdance-1.0.1.dev65/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev64/pyproject.toml` & `slalom_tapdance-1.0.1.dev65/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.1-dev.64"
+version = "1.0.1-dev.65"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.1.dev64/tapdance/cli.py` & `slalom_tapdance-1.0.1.dev65/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev64/tapdance/config.py` & `slalom_tapdance-1.0.1.dev65/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev64/tapdance/docker.py` & `slalom_tapdance-1.0.1.dev65/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev64/tapdance/install_helper.py` & `slalom_tapdance-1.0.1.dev65/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev64/tapdance/plans.py` & `slalom_tapdance-1.0.1.dev65/tapdance/plans.py`

 * *Files 0% similar despite different names*

```diff
@@ -854,29 +854,29 @@
     full_catalog_file: str = None,
     output_file: str = None,
     all_table_catalog: bool = False
 ) -> None:
     """
     Create an individual catalog for a stream
     """
-    logging.info(f"Creating Catalog. All_table_catalog is {all_table_catalog}")
     taps_dir = config.get_taps_dir()
     catalog_dir = config.get_tap_output_dir(tap_name, taps_dir)
     source_catalog_path = full_catalog_file or os.path.join(
         catalog_dir, "catalog-selected.json"
     )
     output_file = output_file or os.path.join(catalog_dir, f"{table_name}-catalog.json")
     included_table_objects = []
     catalog_full = json.loads(Path(source_catalog_path).read_text())
+    # Loop through all the tables in the catalog until we find the current table
     for tbl in catalog_full["streams"]:
         stream_name = _get_stream_name(tbl)
         # Always add the current table to it's catalog
         if stream_name in table_name:
             _get_stream_metadata_object(tbl)["selected"] = True
-            logging.info(f'Adding {table_name} to catalog.')
+            logging.info(f'Adding current table:{table_name} to catalog.')
             included_table_objects.append(tbl)
         # If all_table_catalog is set, add every table to the current table's catalog.
         elif stream_name not in table_name and all_table_catalog:
             logging.info('All Table Catalogs is selected. Adding all tables to catalog')
             _get_stream_metadata_object(tbl)["selected"] = False
             included_table_objects.append(tbl)
     catalog_new = {"streams": included_table_objects}
```

### Comparing `slalom_tapdance-1.0.1.dev64/tapdance/states.py` & `slalom_tapdance-1.0.1.dev65/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev64/tapdance/syncs.py` & `slalom_tapdance-1.0.1.dev65/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev64/PKG-INFO` & `slalom_tapdance-1.0.1.dev65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.1.dev64
+Version: 1.0.1.dev65
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


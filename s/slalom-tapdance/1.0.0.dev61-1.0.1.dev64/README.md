# Comparing `tmp/slalom_tapdance-1.0.0.dev61.tar.gz` & `tmp/slalom_tapdance-1.0.1.dev64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.0.dev61.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.1.dev64.tar", max compression
```

## Comparing `slalom_tapdance-1.0.0.dev61.tar` & `slalom_tapdance-1.0.1.dev64.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-07 22:48:11.779735 slalom_tapdance-1.0.0.dev61/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-07 22:48:26.527588 slalom_tapdance-1.0.0.dev61/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/install_helper.py
--rw-r--r--   0        0        0    38181 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/states.py
--rw-r--r--   0        0        0    12362 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.0.dev61/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-08 17:43:14.385614 slalom_tapdance-1.0.1.dev64/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38145 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/states.py
+-rw-r--r--   0        0        0    12133 2024-05-08 17:42:53.913342 slalom_tapdance-1.0.1.dev64/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev64/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.0.dev61/LICENSE` & `slalom_tapdance-1.0.1.dev64/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev61/pyproject.toml` & `slalom_tapdance-1.0.1.dev64/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.0-dev.61"
+version = "1.0.1-dev.64"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.0.dev61/tapdance/cli.py` & `slalom_tapdance-1.0.1.dev64/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev61/tapdance/config.py` & `slalom_tapdance-1.0.1.dev64/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev61/tapdance/docker.py` & `slalom_tapdance-1.0.1.dev64/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev61/tapdance/install_helper.py` & `slalom_tapdance-1.0.1.dev64/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev61/tapdance/plans.py` & `slalom_tapdance-1.0.1.dev64/tapdance/plans.py`

 * *Files 1% similar despite different names*

```diff
@@ -801,15 +801,14 @@
             replication_method = "FULL_TABLE"
             basis = f"{replication_strategy} strategy and no valid replication keys"
         logging.debug(
             f"Defaulting to {replication_method} replication based on {basis} "
             f"for '{_get_stream_name(tbl)}'."
         )
         stream_metadata["replication-method"] = replication_method
-        stream_metadata["test"] = "test"
 
 def _remove_senseless_validators(tbl: dict) -> None:
     if "properties" not in tbl["schema"]:
         return
     for col, props in tbl["schema"]["properties"].items():
         for senseless in [
             "multipleOf",
@@ -850,38 +849,38 @@
 )
 def _create_table_catalog(
     #could alter the catalog here
     tap_name: str,
     table_name: str,
     full_catalog_file: str = None,
     output_file: str = None,
-    multiple_table_catalog: bool = False
+    all_table_catalog: bool = False
 ) -> None:
     """
     Create an individual catalog for a stream
     """
-    logging.info(f"Creating Catalog. Multiple_table_catalog is {multiple_table_catalog}")
+    logging.info(f"Creating Catalog. All_table_catalog is {all_table_catalog}")
     taps_dir = config.get_taps_dir()
     catalog_dir = config.get_tap_output_dir(tap_name, taps_dir)
     source_catalog_path = full_catalog_file or os.path.join(
         catalog_dir, "catalog-selected.json"
     )
     output_file = output_file or os.path.join(catalog_dir, f"{table_name}-catalog.json")
     included_table_objects = []
     catalog_full = json.loads(Path(source_catalog_path).read_text())
     for tbl in catalog_full["streams"]:
         stream_name = _get_stream_name(tbl)
-        # if stream_name == table_name:
-        #trying to make a catalog with two streams in it
+        # Always add the current table to it's catalog
         if stream_name in table_name:
             _get_stream_metadata_object(tbl)["selected"] = True
-            logging.info('MTC is not selected. Doing single table catalogs')
+            logging.info(f'Adding {table_name} to catalog.')
             included_table_objects.append(tbl)
-        elif stream_name not in table_name and multiple_table_catalog:
-            logging.info('Multiple Table Catalog is selected. Adding all tables to catalog')
+        # If all_table_catalog is set, add every table to the current table's catalog.
+        elif stream_name not in table_name and all_table_catalog:
+            logging.info('All Table Catalogs is selected. Adding all tables to catalog')
             _get_stream_metadata_object(tbl)["selected"] = False
             included_table_objects.append(tbl)
     catalog_new = {"streams": included_table_objects}
     with open(output_file, "w") as f:
         json.dump(catalog_new, f, indent=2)
```

### Comparing `slalom_tapdance-1.0.0.dev61/tapdance/states.py` & `slalom_tapdance-1.0.1.dev64/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev61/tapdance/syncs.py` & `slalom_tapdance-1.0.1.dev64/tapdance/syncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 
     replication_strategy = replication_strategy or tap_settings.get(
         "REPLICATION_STRATEGY", "INCREMENTAL"
     )
 
     logging.info(tap_settings)
     is_parent_child_tap = tap_settings.get("IS_PARENT_CHILD_TAP", False)
-    logging.info(f'is_parent_child_tap is {is_parent_child_tap}')
 
     config.validate_replication_strategy(replication_strategy)
 
     #could use something here to identify a parent child table
     table_name = table_name or tap_settings.get("TABLE_NAME", None)
     exclude_tables = exclude_tables or tap_settings.get("EXCLUDE_TABLES", None)
     rules_file = config.get_rules_file(taps_dir, tap_name)
@@ -157,32 +156,29 @@
         # Call each tap independently so that table state files are kept separate:
         tmp_catalog_file = f"{catalog_dir}/{tap_name}-{table}-catalog.json"
         table_state_file = (
             state_file
             or config.get_state_file_path()
             or f"{catalog_dir}/{table}-state.json"
         )
-        #TODO- IF PARENT CHILD YES, SEND TO MULTIPLE TABLE CATALOG
-        # ELSE  - SINGLE TABLE CATALOG
         plans._create_table_catalog(
                 tap_name=tap_name,
                 table_name=table,
                 full_catalog_file=full_catalog_file,
                 output_file=tmp_catalog_file,
-                multiple_table_catalog = is_parent_child_tap
+                all_table_catalog = is_parent_child_tap
             )
         _sync_one_table(
             tap_name=tap_name,
             target_name=target_name,
             table_name=table,
             taps_dir=taps_dir,
             config_file=config_file,
             target_config_file=target_config_file,
             table_catalog_file=tmp_catalog_file,
-            # table_catalog_file=full_catalog_file,
             table_state_file=table_state_file,
             log_dir=log_dir,
             dockerized=dockerized,
             tap_exe=tap_exe,
             target_exe=target_exe,
         )
```

### Comparing `slalom_tapdance-1.0.0.dev61/PKG-INFO` & `slalom_tapdance-1.0.1.dev64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.0.dev61
+Version: 1.0.1.dev64
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


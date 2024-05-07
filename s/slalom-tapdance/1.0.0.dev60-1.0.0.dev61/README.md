# Comparing `tmp/slalom_tapdance-1.0.0.dev60.tar.gz` & `tmp/slalom_tapdance-1.0.0.dev61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.0.dev60.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.0.dev61.tar", max compression
```

## Comparing `slalom_tapdance-1.0.0.dev60.tar` & `slalom_tapdance-1.0.0.dev61.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-03 17:40:35.635282 slalom_tapdance-1.0.0.dev60/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-03 17:40:53.399238 slalom_tapdance-1.0.0.dev60/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-03 17:40:35.639283 slalom_tapdance-1.0.0.dev60/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-03 17:40:35.639283 slalom_tapdance-1.0.0.dev60/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-03 17:40:35.639283 slalom_tapdance-1.0.0.dev60/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-03 17:40:35.639283 slalom_tapdance-1.0.0.dev60/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-03 17:40:35.639283 slalom_tapdance-1.0.0.dev60/tapdance/install_helper.py
--rw-r--r--   0        0        0    37840 2024-05-03 17:40:35.639283 slalom_tapdance-1.0.0.dev60/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-03 17:40:35.639283 slalom_tapdance-1.0.0.dev60/tapdance/states.py
--rw-r--r--   0        0        0    11850 2024-05-03 17:40:35.639283 slalom_tapdance-1.0.0.dev60/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.0.dev60/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-07 22:48:11.779735 slalom_tapdance-1.0.0.dev61/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-07 22:48:26.527588 slalom_tapdance-1.0.0.dev61/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38181 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/states.py
+-rw-r--r--   0        0        0    12362 2024-05-07 22:48:11.783735 slalom_tapdance-1.0.0.dev61/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.0.dev61/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.0.dev60/LICENSE` & `slalom_tapdance-1.0.0.dev61/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev60/pyproject.toml` & `slalom_tapdance-1.0.0.dev61/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.0-dev.60"
+version = "1.0.0-dev.61"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.0.dev60/tapdance/cli.py` & `slalom_tapdance-1.0.0.dev61/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev60/tapdance/config.py` & `slalom_tapdance-1.0.0.dev61/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev60/tapdance/docker.py` & `slalom_tapdance-1.0.0.dev61/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev60/tapdance/install_helper.py` & `slalom_tapdance-1.0.0.dev61/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev60/tapdance/plans.py` & `slalom_tapdance-1.0.0.dev61/tapdance/plans.py`

 * *Files 6% similar despite different names*

```diff
@@ -335,14 +335,15 @@
                     if metadata.get("valid-replication-keys")
                     else "blank"
                 )
                 + ")"
             )
             metadata["valid-replication-keys"] = table_plan["replication_key"]
             metadata["replication-key"] = table_plan["replication_key"][0]
+            metadata["parent"] = 'yes'
 
 
 def _get_catalog_file_keys(
     key_type: str,
     matches: Dict[str, Dict[str, bool]],
     matched_stream_ids: Dict[str, str],
     catalog_file: str,
@@ -380,65 +381,51 @@
         )
     return result
 
 
 def _get_rules_file_keys(
     key_type: str, matches: Dict[str, Dict[str, bool]], rules_file: str,
 ) -> Dict[str, List[str]]:
-    """Return a Dictionary of table names and columns that contain an 
-       override in the Rules file that match the provided key type. 
-    
-    """
     result: Dict[str, List[str]] = {}
     if key_type not in ["primary-key", "replication-key"]:
         raise ValueError(
             f"Unexpected key type '{key_type}'. "
             "Expected: 'replication-key' or 'primary-key'"
         )
     # Check rules_file to fill `matches`
     plan_file_lines = uio.get_text_file_contents(rules_file).splitlines()
-    # Loop through the contents of the rules file and check if each line contains an override
+    #Key Overrides
     key_overrides = [
         line.split("->")[0].rstrip()
         for line in plan_file_lines
         if "->" in line and line.split("->")[1].lstrip().rstrip() == key_type
     ]
     for key_spec in key_overrides:
-        # Check to see if the override is formatted correctly
         if len(key_spec.split(".")) != 2 or "*" in key_spec:
             raise ValueError(
                 f"Expected '{key_type}' indicator with exact two-part key, separated "
                 f"by '.'.  Found '{key_spec}'"
             )
         table_name, key_col_name = key_spec.split(".")
-        # Check that the column is on the table
         if table_name not in matches:
             raise ValueError(f"Could not locate table '{table_name}' in selected list.")
         if key_col_name not in matches[table_name]:
             raise ValueError(f"Key column '{key_spec}' is not in column list.")
         elif not matches[table_name][key_col_name]:
             raise ValueError(f"Key column '{key_spec}' is not a selected column.")
-        # Add the column to the table key in the dictionary
-        # If the table is already in the result dictionary, append the new column to the list. 
-        if table_name in result:
-            result[table_name].append(key_col_name)
-        else:
-            result[table_name] = [key_col_name]
+        result[table_name] = [key_col_name]
     return result
 
 
 def _get_table_keys(
     matches: Dict[str, Dict[str, bool]],
     matched_stream_ids: Dict[str, str],
     catalog_file: str,
     rules_file: str,
 ) -> Tuple[Dict[str, List[str]], Dict[str, List[str]]]:
-    """
-    
-    """
     primary_keys: Dict[str, List[str]] = {}
     replication_keys: Dict[str, List[str]] = {}
     stream_name_lookup = {v: k for k, v in matched_stream_ids.items()}
     for key_type, collection in [
         ("primary-key", primary_keys),
         ("replication-key", replication_keys),
     ]:
@@ -446,15 +433,14 @@
             _get_catalog_file_keys(
                 key_type,
                 matches=matches,
                 matched_stream_ids=matched_stream_ids,
                 catalog_file=catalog_file,
             )
         )
-        # Get a dictionary of table names with their overrides from the rules file
         key_overrides = _get_rules_file_keys(
             key_type, matches=matches, rules_file=rules_file
         )
         for table, override in key_overrides.items():
             if table.startswith('"'):
                 table = stream_name_lookup[table.lstrip('"').rstrip('"')]
             collection[table] = override
@@ -646,14 +632,17 @@
 def _make_plan_file_text(
     matches: Dict[str, Dict[str, bool]],
     primary_keys: Dict[str, List[str]],
     replication_keys: Dict[str, List[str]],
     table_stream_ids: Dict[str, str],
     excluded_table_stream_ids: Dict[str, List[str]],
 ) -> str:
+    """
+    Creates the test for the plan file that will be written to the file.
+    """
     sorted_tables = sorted(matches.keys())
     file_text = ""
     file_text += "selected_tables:\n"
     for table in sorted_tables:
         stream_id = table_stream_ids[table]
         primary_key_cols: List[str] = primary_keys[table]
         replication_key_cols: List[str] = replication_keys[table]
@@ -749,20 +738,22 @@
     catalog_full = json.loads(Path(raw_catalog_file).read_text())
     plan_file = plan_file or config.get_plan_file(tap_name)
     plan = yaml.safe_load(uio.get_text_file_contents(plan_file))
     if ("selected_tables" not in plan) or (plan["selected_tables"] is None):
         raise ValueError(f"No selected tables found in plan file '{plan_file}'.")
     included_table_objects = []
     for tbl in sorted(catalog_full["streams"], key=lambda x: _get_stream_name(x)):
+        #loop through the tables in the full catalog, create the catalog selected with the plan file
         stream_name = _get_stream_name(tbl)
         stream_id = _get_stream_id(tbl)
         if stream_name in plan["selected_tables"].keys() and stream_id == plan[
             "selected_tables"
         ][stream_name].get("stream_id", stream_name):
             _set_catalog_file_keys(tbl, plan["selected_tables"][stream_name])
+            # get the metadata from the catalog full
             _select_table(tbl, replication_strategy=replication_strategy)
             for col_name in _get_catalog_table_columns(tbl):
                 col_selected = col_name in (
                     (plan["selected_tables"][stream_name]["selected_columns"] or [])
                     + (plan["selected_tables"][stream_name]["replication_key"] or [])
                     + (plan["selected_tables"][stream_name]["primary_key"] or [])
                 )
@@ -785,14 +776,15 @@
     for tbl in sorted(selected_catalog["streams"], key=lambda x: _get_stream_name(x)):
         _validate_keys(tbl, key_type="primary-key")
     for tbl in sorted(selected_catalog["streams"], key=lambda x: _get_stream_name(x)):
         _validate_keys(tbl, key_type="replication-key")
 
 
 def _select_table(tbl: dict, replication_strategy: str):
+    #Creates the metadata for the Catalog Seleted
     stream_metadata = _get_stream_metadata_object(tbl)
     stream_metadata["selected"] = True
     if (
         "replication-method" not in stream_metadata
         and "forced-replication-method" not in stream_metadata
     ):
         replication_keys = stream_metadata.get("valid-replication-keys", [])
@@ -809,15 +801,15 @@
             replication_method = "FULL_TABLE"
             basis = f"{replication_strategy} strategy and no valid replication keys"
         logging.debug(
             f"Defaulting to {replication_method} replication based on {basis} "
             f"for '{_get_stream_name(tbl)}'."
         )
         stream_metadata["replication-method"] = replication_method
-
+        stream_metadata["test"] = "test"
 
 def _remove_senseless_validators(tbl: dict) -> None:
     if "properties" not in tbl["schema"]:
         return
     for col, props in tbl["schema"]["properties"].items():
         for senseless in [
             "multipleOf",
@@ -852,32 +844,45 @@
     return None
 
 
 @logged(
     "selecting '{table_name}' catalog metadata "
     "from '{tap_name}' source catalog file: {full_catalog_file}"
 )
-def _create_single_table_catalog(
+def _create_table_catalog(
+    #could alter the catalog here
     tap_name: str,
     table_name: str,
     full_catalog_file: str = None,
     output_file: str = None,
+    multiple_table_catalog: bool = False
 ) -> None:
+    """
+    Create an individual catalog for a stream
+    """
+    logging.info(f"Creating Catalog. Multiple_table_catalog is {multiple_table_catalog}")
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
-        if stream_name == table_name:
+        # if stream_name == table_name:
+        #trying to make a catalog with two streams in it
+        if stream_name in table_name:
             _get_stream_metadata_object(tbl)["selected"] = True
+            logging.info('MTC is not selected. Doing single table catalogs')
+            included_table_objects.append(tbl)
+        elif stream_name not in table_name and multiple_table_catalog:
+            logging.info('Multiple Table Catalog is selected. Adding all tables to catalog')
+            _get_stream_metadata_object(tbl)["selected"] = False
             included_table_objects.append(tbl)
     catalog_new = {"streams": included_table_objects}
     with open(output_file, "w") as f:
         json.dump(catalog_new, f, indent=2)
 
 
 def _table_match_check(table_name: str, stream_id: str, select_rules: list) -> bool:
```

### Comparing `slalom_tapdance-1.0.0.dev60/tapdance/states.py` & `slalom_tapdance-1.0.0.dev61/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.0.dev60/tapdance/syncs.py` & `slalom_tapdance-1.0.0.dev61/tapdance/syncs.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,16 +107,22 @@
     target_exe = target_exe or target_settings.get("EXE", f"target-{target_name}")
 
     config.print_plugin_version(tap_exe,target_exe)
 
     replication_strategy = replication_strategy or tap_settings.get(
         "REPLICATION_STRATEGY", "INCREMENTAL"
     )
+
+    logging.info(tap_settings)
+    is_parent_child_tap = tap_settings.get("IS_PARENT_CHILD_TAP", False)
+    logging.info(f'is_parent_child_tap is {is_parent_child_tap}')
+
     config.validate_replication_strategy(replication_strategy)
 
+    #could use something here to identify a parent child table
     table_name = table_name or tap_settings.get("TABLE_NAME", None)
     exclude_tables = exclude_tables or tap_settings.get("EXCLUDE_TABLES", None)
     rules_file = config.get_rules_file(taps_dir, tap_name)
 
     # TODO: Resolve bug in Windows STDERR inclusion when emitting catalog json from
     #       docker run
     # if dockerized is None:
@@ -151,28 +157,32 @@
         # Call each tap independently so that table state files are kept separate:
         tmp_catalog_file = f"{catalog_dir}/{tap_name}-{table}-catalog.json"
         table_state_file = (
             state_file
             or config.get_state_file_path()
             or f"{catalog_dir}/{table}-state.json"
         )
-        plans._create_single_table_catalog(
-            tap_name=tap_name,
-            table_name=table,
-            full_catalog_file=full_catalog_file,
-            output_file=tmp_catalog_file,
-        )
+        #TODO- IF PARENT CHILD YES, SEND TO MULTIPLE TABLE CATALOG
+        # ELSE  - SINGLE TABLE CATALOG
+        plans._create_table_catalog(
+                tap_name=tap_name,
+                table_name=table,
+                full_catalog_file=full_catalog_file,
+                output_file=tmp_catalog_file,
+                multiple_table_catalog = is_parent_child_tap
+            )
         _sync_one_table(
             tap_name=tap_name,
             target_name=target_name,
             table_name=table,
             taps_dir=taps_dir,
             config_file=config_file,
             target_config_file=target_config_file,
             table_catalog_file=tmp_catalog_file,
+            # table_catalog_file=full_catalog_file,
             table_state_file=table_state_file,
             log_dir=log_dir,
             dockerized=dockerized,
             tap_exe=tap_exe,
             target_exe=target_exe,
         )
 
@@ -197,14 +207,15 @@
     pipeline_version_num = config.get_pipeline_version_number()
     table_state_file = config.replace_placeholders(
         {"table_state_file": table_state_file},
         tap_name,
         table_name,
         pipeline_version_num,
     )["table_state_file"]
+    logging.warning(f'{table_catalog_file}')
     tap_args = f"--config {config_file} --catalog {table_catalog_file} "
     if s3_file_exists(table_state_file):
         local_state_file_in = os.path.join(
             config.get_tap_output_dir(tap_name, taps_dir),
             f"{tap_name}-{table_name}-state.json",
         )
         if not uio.get_text_file_contents(table_state_file):
```

### Comparing `slalom_tapdance-1.0.0.dev60/PKG-INFO` & `slalom_tapdance-1.0.0.dev61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.0.dev60
+Version: 1.0.0.dev61
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/tiny_data_warehouse-0.1.3.tar.gz` & `tmp/tiny_data_warehouse-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_data_warehouse-0.1.3.tar", max compression
+gzip compressed data, was "tiny_data_warehouse-0.1.5.tar", max compression
```

## Comparing `tiny_data_warehouse-0.1.3.tar` & `tiny_data_warehouse-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0       55 2024-04-20 14:50:59.621598 tiny_data_warehouse-0.1.3/README.md
--rw-r--r--   0        0        0      482 2024-04-21 05:22:24.539713 tiny_data_warehouse-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2552 2024-04-20 14:48:18.086281 tiny_data_warehouse-0.1.3/tiny_data_warehouse/data_warehouse.py
--rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 tiny_data_warehouse-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       55 2024-04-20 14:50:59.621598 tiny_data_warehouse-0.1.5/README.md
+-rw-r--r--   0        0        0      546 2024-05-08 19:53:31.544718 tiny_data_warehouse-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-26 08:58:36.102348 tiny_data_warehouse-0.1.5/tiny_data_warehouse/__init__.py
+-rw-r--r--   0        0        0     3821 2024-04-26 09:38:13.764963 tiny_data_warehouse-0.1.5/tiny_data_warehouse/data_warehouse.py
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 tiny_data_warehouse-0.1.5/PKG-INFO
```

### Comparing `tiny_data_warehouse-0.1.3/tiny_data_warehouse/data_warehouse.py` & `tiny_data_warehouse-0.1.5/tiny_data_warehouse/data_warehouse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,93 @@
 import os
 
-from typing import Optional, List
+from typing import Optional
 import pandas as pd
 
-
-DEFAULT_FOLDER = os.path.join(os.environ['HOME'], '.tinyws')
-DEFAULT_EVENTS_FOLDER = os.path.join(DEFAULT_FOLDER, 'events')
-
 class DataWarehouse:
-    def __init__(self, events_folder: Optional[str] = None, supported_events: Optional[List[str]]=None) -> None:
+    DEFAULT_FOLDER = os.path.join(os.environ['HOME'], '.tinyws')
+    DEFAULT_EVENTS_FOLDER = os.path.join(DEFAULT_FOLDER, 'events')
+
+    def __init__(self, events_folder: Optional[str] = None, events_config=None) -> None:
         if not events_folder:
-            events_folder = DEFAULT_EVENTS_FOLDER
-            #print("Given that no events_folder was given, the default folder will be used: {}".format(events_folder))
+            events_folder = DataWarehouse.DEFAULT_EVENTS_FOLDER
 
         if not os.path.exists(events_folder):
             os.makedirs(events_folder)
             
-        self.base_folder = DEFAULT_FOLDER
+        self.base_folder = DataWarehouse.DEFAULT_FOLDER
         self.events_folder = events_folder
-        self.supported_events = supported_events
+        self.events_config = events_config
+        if events_config:
+            print("Events config given: ", events_config)
 
-
-    def list_stored_events(self) -> List[str]:
+    def list_stored_events(self):
         os.system("ls -l {}".format(self.events_folder))
 
-    def ls(self):
-        return self.list_stored_events()
-
-    def write_event(self, event_name, event: Optional[str]) -> None:
+    def write_event(self, event_name: str, event_data: dict, verbose=False, dry_run=False) -> None:
         """
         if event is a dict every key will be a column in the parquet file
 
         Adds a column tdw_timestamp to the event
         """
-        if type(event) != dict:
-            raise ValueError('event must be a dictionary got {}'.format(type(event)))
+        self._validate_event_data(event_data)
+
+        event_data['tdw_timestamp'] = pd.Timestamp.now()
+        new_df = pd.DataFrame([event_data])
+
+        if self._exists_data(event_name):
+            existing_data = self.event(event_name)
+
+            if event_name in self.events_config and 'prevent_duplicates_col' in self.events_config[event_name]:
+                check_column_name = self.events_config[event_name]['prevent_duplicates_col']
+                possible_duplicated_value = event_data[check_column_name]
+
+                # test if in existing_data there is a duplicated value
+                if possible_duplicated_value in existing_data[check_column_name].values:
+                    raise ValueError(f"A duplicated value {event_data[check_column_name]} for key {check_column_name} was found in the event {event_name}")
 
-        event['tdw_timestamp'] = pd.Timestamp.now()
-        df = pd.DataFrame([event])
-        if os.path.exists(self._parquet_file(event_name)):
-            df = pd.concat([pd.read_parquet(self._parquet_file(event_name)), df])
+            df = pd.concat([existing_data, new_df])
+
+        if not dry_run:
+            self._write_df(event_name, df)
+        else:
+            print(f"Event {event_name} written successfully")
+
+        if verbose:
+            print(f"Event {event_name} written successfully")
+
+    def _write_df(self, event_name, df):
         df.to_parquet(self._parquet_file(event_name))
-        print(f"Event {event_name} written successfully")
 
+    def _validate_event_data(self, event_data: dict) -> None:
+        if type(event_data) != dict:
+            raise ValueError('event must be a dictionary got {}'.format(type(event_data)))
+
+    def _exists_data(self, event_name: str) -> bool:
+        return os.path.exists(self._parquet_file(event_name))
 
     def event(self, event_name: Optional[str]) -> pd.DataFrame:
         """
         Reads the data from the event returned as a pandas DataFrame
         """
         if not os.path.exists(self._parquet_file(event_name)):
             raise ValueError('Event {} does not exist'.format(event_name))
 
         df = pd.read_parquet(self._parquet_file(event_name))
 
         return df
 
-    def remove_event(self, event_name: str, dry_run=True) -> None:
+    def replace_df(self, event_name: str, df: pd.DataFrame, dry_run=True) -> None:
+        if dry_run:
+            print('Replace of event {}, destructive event! Disable dry run to execute it'.format(event_name))
+        df.to_parquet(self._parquet_file(event_name))
 
+    def remove_event(self, event_name: str, dry_run=True) -> None:
         if dry_run:
-            print('Dry run removal of the the event {}. Disable dry run to execute it'.format(event_name))
+            print('Dry run removal of the the event {}, destructive event! Disable dry run to execute it'.format(event_name))
 
         os.remove(self._parquet_file(event_name))
 
     def print_event(self, event_name: Optional[str]) -> None:
         print(self.event(event_name))
     
     def _parquet_file(self, event_name):
```

### Comparing `tiny_data_warehouse-0.1.3/PKG-INFO` & `tiny_data_warehouse-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: tiny-data-warehouse
-Version: 0.1.3
+Version: 0.1.5
 Summary: 
 Author: Jean Carlo Machado
 Author-email: jean.machado@getyourguide.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fire (>=0.6.0,<0.7.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: pypdf2 (>=3.0.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Installation
 
 ```
 pip install tiny-data-warehouse
 ```
```


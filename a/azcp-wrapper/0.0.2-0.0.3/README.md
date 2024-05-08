# Comparing `tmp/azcp_wrapper-0.0.2.tar.gz` & `tmp/azcp_wrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azcp_wrapper-0.0.2.tar", last modified: Thu Mar 28 20:53:47 2024, max compression
+gzip compressed data, was "azcp_wrapper-0.0.3.tar", last modified: Wed May  8 02:24:06 2024, max compression
```

## Comparing `azcp_wrapper-0.0.2.tar` & `azcp_wrapper-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:53:47.339872 azcp_wrapper-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-28 20:53:47.339872 azcp_wrapper-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:53:47.339872 azcp_wrapper-0.0.2/azcp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/azcp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/azcp_wrapper/azcp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/azcp_wrapper/azcp_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/azcp_wrapper/azcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/azcp_wrapper/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/azcp_wrapper/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:53:47.339872 azcp_wrapper-0.0.2/azcp_wrapper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/azcp_wrapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/azcp_wrapper/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/azcp_wrapper/utils/execute_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:53:47.339872 azcp_wrapper-0.0.2/azcp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-28 20:53:47.000000 azcp_wrapper-0.0.2/azcp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-28 20:53:47.000000 azcp_wrapper-0.0.2/azcp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 20:53:47.000000 azcp_wrapper-0.0.2/azcp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 20:53:47.000000 azcp_wrapper-0.0.2/azcp_wrapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-28 20:53:47.000000 azcp_wrapper-0.0.2/azcp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 20:53:47.000000 azcp_wrapper-0.0.2/azcp_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 20:53:47.339872 azcp_wrapper-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-28 20:53:42.000000 azcp_wrapper-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:24:06.169927 azcp_wrapper-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 02:24:06.169927 azcp_wrapper-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:24:06.169927 azcp_wrapper-0.0.3/azcp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/azcp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/azcp_wrapper/azcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/azcp_wrapper/azcp_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/azcp_wrapper/azcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/azcp_wrapper/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/azcp_wrapper/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:24:06.169927 azcp_wrapper-0.0.3/azcp_wrapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/azcp_wrapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/azcp_wrapper/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/azcp_wrapper/utils/execute_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:24:06.169927 azcp_wrapper-0.0.3/azcp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 02:24:06.000000 azcp_wrapper-0.0.3/azcp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-08 02:24:06.000000 azcp_wrapper-0.0.3/azcp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:24:06.000000 azcp_wrapper-0.0.3/azcp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 02:24:06.000000 azcp_wrapper-0.0.3/azcp_wrapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 02:24:06.000000 azcp_wrapper-0.0.3/azcp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 02:24:06.000000 azcp_wrapper-0.0.3/azcp_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:24:06.169927 azcp_wrapper-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 02:24:02.000000 azcp_wrapper-0.0.3/setup.py
```

### Comparing `azcp_wrapper-0.0.2/LICENSE` & `azcp_wrapper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.2/PKG-INFO` & `azcp_wrapper-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azcp_wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple AzCopy wrapper to transfer data
 Home-page: https://github.com/eabdala/azcp_wrapper
 Author: Erik Alejandro Abdala
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azcp_wrapper-0.0.2/azcp_wrapper/azcp_client.py` & `azcp_wrapper-0.0.3/azcp_wrapper/azcp_client.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.2/azcp_wrapper/azcp_summary.py` & `azcp_wrapper-0.0.3/azcp_wrapper/azcp_summary.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,59 +3,61 @@
 from azcp_wrapper.azcp_utils import AzCopyJobInfo, AzSyncJobInfo
 
 
 def get_property_value(key: str, job_summary: str) -> int:
     property_value = 0
 
     try:
-        property_key_match = re.search(r"{}: \d+\n".format(key), job_summary)
-
+        property_key_match = re.search(r"{}: (\d+(\.\d+)?)".format(re.escape(key)), job_summary)
+        # print(r"{}: (\d+(\.\d+)?)".format(re.escape(key)),property_key_match)
         if property_key_match is not None:
 
             property_key_text = property_key_match.group()
-            property_value_match = re.search(r"\d+", property_key_text)
+            property_value_match = re.search(r"(\d+(\.\d+)?)", property_key_text)
 
             # If the property key text exists in the job summary,
             # the gets the property value
             if property_value_match is not None:
-                property_value = int(property_value_match.group())
+                property_value = str(property_value_match.group())
     except Exception as e:
         print(e)
 
     return property_value
 
 
 def get_transfer_copy_summary_info(
     job_info: AzCopyJobInfo, summary: str
 ) -> AzCopyJobInfo:
     """
     Extract all properties of Job Info from the Azcopy job summary
     """
-
     properties_required = [
         "Number of File Transfers",
         "Number of Folder Property Transfers",
         "Number of File Transfers",
         "Total Number of Transfers",
         "Number of Transfers Completed",
-        "Number of Transfers Failed",
+        "Number of File Transfers Skipped",
         "Number of Transfers Skipped",
     ]
 
     for property_key in properties_required:
 
         # Converting the property key string to attribute form
         property_attribute = property_key.lower().replace(" ", "_")
         property_value = get_property_value(property_key, summary)
 
         # Set the attribute in job_info object
         setattr(job_info, property_attribute, property_value)
 
+    job_info.elapsed_time_minutes = get_property_value(
+        "Elapsed Time (Minutes)", summary
+    )
     job_info.total_bytes_transferred = get_property_value(
-        "TotalBytesTransferred", summary
+        "Total Number of Bytes Transferred", summary
     )
 
     return job_info
 
 
 def get_sync_summary_info(sync_job_info: AzSyncJobInfo, summary: str) -> AzSyncJobInfo:
     """
```

### Comparing `azcp_wrapper-0.0.2/azcp_wrapper/azcp_utils.py` & `azcp_wrapper-0.0.3/azcp_wrapper/azcp_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,51 +202,55 @@
     Created the job info of the Azcopy job executed by the user
     """
 
 
     def __init__(
         self,
         percent_complete: Annotated[float, Doc("")] = float(0),
+        elapsed_time_minutes: Annotated[float, Doc("")] = float(0),
         error_msg: Annotated[str, Doc("")] = "",
         final_job_status_msg: Annotated[str, Doc("")] = "",
         number_of_file_transfers: Annotated[int, Doc("")] = 0,
         number_of_folder_property_transfers: Annotated[int, Doc("")] = 0,
         total_number_of_transfers: Annotated[int, Doc("")] = 0,
         number_of_transfers_completed: Annotated[int, Doc("")] = 0,
         number_of_transfers_failed: Annotated[int , Doc("")]= 0,
-        number_of_transfers_skipped: Annotated[int, Doc("")] = 0,
+        number_of_file_transfers_skipped: Annotated[int, Doc("")] = 0,
         total_bytes_transferred: Annotated[int, Doc("")] = 0,
         completed: Annotated[bool, Doc("")]= False,
     ) -> None:
         # NOTE: Sometimes, azcopy doesn't return value as 100%
         # even if the entire data is transferred.
         # This might be because if the transfer is completed in between
         # the value sent by azcopy, then azcopy fails to send the final
         # percent value and directly sends the job summary
         self.percent_complete = percent_complete
+        self.elapsed_time_minutes = elapsed_time_minutes
         self.error_msg = error_msg
         self.final_job_status_msg = final_job_status_msg
         self.number_of_file_transfers = number_of_file_transfers
         self.number_of_folder_property_transfers = number_of_folder_property_transfers
         self.total_number_of_transfers = total_number_of_transfers
         self.number_of_transfers_completed = number_of_transfers_completed
         self.number_of_transfers_failed = number_of_transfers_failed
-        self.number_of_transfers_skipped = number_of_transfers_skipped
+        self.number_of_file_transfers_skipped = number_of_file_transfers_skipped
         self.total_bytes_transferred = total_bytes_transferred
         self.completed = completed
     def __str__(self) -> str:
         """
         Get a human-readable string representation of the AzCopyJobInfo object.
         """
         return f"AzCopy Job Info:\n" \
+            f"Elapsed Time (Minutes): {self.elapsed_time_minutes}\n" \
                f"Percent Complete: {self.percent_complete}%\n" \
                f"Final Job Status: {self.final_job_status_msg}\n" \
+                f"Number of File Transfers: {self.number_of_file_transfers}\n" \
                f"Transfers Completed: {self.number_of_transfers_completed}\n" \
                f"Transfers Failed: {self.number_of_transfers_failed}\n" \
-               f"Transfers Skipped: {self.number_of_transfers_skipped}\n" \
+               f"Transfers Skipped: {self.number_of_file_transfers_skipped}\n" \
                f"Total Bytes Transferred: {self.total_bytes_transferred}"
 
 
 class AzSyncJobInfo:
     """
     Created the job info of the Azcopy job executed by the user
     """
```

### Comparing `azcp_wrapper-0.0.2/azcp_wrapper/logging_config.py` & `azcp_wrapper-0.0.3/azcp_wrapper/logging_config.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.2/azcp_wrapper/setup.py` & `azcp_wrapper-0.0.3/azcp_wrapper/setup.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.2/azcp_wrapper/utils/execute_command.py` & `azcp_wrapper-0.0.3/azcp_wrapper/utils/execute_command.py`

 * *Files identical despite different names*

### Comparing `azcp_wrapper-0.0.2/azcp_wrapper.egg-info/PKG-INFO` & `azcp_wrapper-0.0.3/azcp_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azcp_wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple AzCopy wrapper to transfer data
 Home-page: https://github.com/eabdala/azcp_wrapper
 Author: Erik Alejandro Abdala
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `azcp_wrapper-0.0.2/setup.py` & `azcp_wrapper-0.0.3/setup.py`

 * *Files identical despite different names*


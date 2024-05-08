# Comparing `tmp/ugrc-sweeper-2.0.1.tar.gz` & `tmp/ugrc-sweeper-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugrc-sweeper-2.0.1.tar", last modified: Tue May  7 20:57:52 2024, max compression
+gzip compressed data, was "ugrc-sweeper-2.0.2.tar", last modified: Wed May  8 17:22:39 2024, max compression
```

## Comparing `ugrc-sweeper-2.0.1.tar` & `ugrc-sweeper-2.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:52.132187 ugrc-sweeper-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-07 20:57:52.132187 ugrc-sweeper-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:57:52.132187 ugrc-sweeper-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:52.128187 ugrc-sweeper-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:52.128187 ugrc-sweeper-2.0.1/src/sweeper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8899 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/address_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/street_types.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:52.132187 ugrc-sweeper-2.0.1/src/sweeper/sweepers/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/sweepers/UseLimitations.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/sweepers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/sweepers/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/sweepers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/sweepers/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/sweepers/empties.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/sweepers/invalids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/sweepers/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-07 20:57:47.000000 ugrc-sweeper-2.0.1/src/sweeper/workspace_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:52.132187 ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-07 20:57:52.000000 ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 20:57:52.000000 ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:57:52.000000 ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 20:57:52.000000 ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:57:52.000000 ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-07 20:57:52.000000 ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 20:57:52.000000 ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:22:38.999432 ugrc-sweeper-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-08 17:22:38.999432 ugrc-sweeper-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:22:38.999432 ugrc-sweeper-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:22:38.991432 ugrc-sweeper-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:22:38.995432 ugrc-sweeper-2.0.2/src/sweeper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8899 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/street_types.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:22:38.995432 ugrc-sweeper-2.0.2/src/sweeper/sweepers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/sweepers/UseLimitations.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/sweepers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/sweepers/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/sweepers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/sweepers/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/sweepers/empties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/sweepers/invalids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/sweepers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-08 17:22:35.000000 ugrc-sweeper-2.0.2/src/sweeper/workspace_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:22:38.995432 ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-08 17:22:38.000000 ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-08 17:22:38.000000 ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:22:38.000000 ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 17:22:38.000000 ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:22:38.000000 ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-08 17:22:38.000000 ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 17:22:38.000000 ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/top_level.txt
```

### Comparing `ugrc-sweeper-2.0.1/LICENSE` & `ugrc-sweeper-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/PKG-INFO` & `ugrc-sweeper-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugrc-sweeper
-Version: 2.0.1
+Version: 2.0.2
 Summary: CLI tool for making good data
 Home-page: https://github.com/agrc/sweeper
 Author: UGRC
 Author-email: ugrc-developers@utah.gov
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ugrc-sweeper-2.0.1/setup.py` & `ugrc-sweeper-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from os.path import basename, splitext
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="ugrc-sweeper",
-    version="2.0.1",
+    version="2.0.2",
     license="MIT",
     description="CLI tool for making good data",
     long_description=(Path(__file__).parent / "readme.md").read_text(),
     long_description_content_type="text/markdown",
     author="UGRC",
     author_email="ugrc-developers@utah.gov",
     url="https://github.com/agrc/sweeper",
```

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/__main__.py` & `ugrc-sweeper-2.0.2/src/sweeper/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 # * coding: utf8 *
 """
 sweeper
 
 Usage:
-  sweeper sweep duplicates  --workspace=<workspace> [--table-name=<table_name> --verbose --try-fix --change-detect --scheduled --save-report=<report_path> --backup-to=<backup_path>]
-  sweeper sweep empties     --workspace=<workspace> [--table-name=<table_name> --verbose --try-fix --change-detect --scheduled --save-report=<report_path> --backup-to=<backup_path>]
-  sweeper sweep invalids    --workspace=<workspace> [--table-name=<table_name> --verbose --try-fix --change-detect --scheduled --save-report=<report_path> --backup-to=<backup_path>]
+  sweeper sweep duplicates  --workspace=<workspace> [--table-name=<table_name> | --change-detect] [--verbose --try-fix --scheduled --save-report=<report_path> --backup-to=<backup_path>]
+  sweeper sweep empties     --workspace=<workspace> [--table-name=<table_name> | --change-detect] [--verbose --try-fix --scheduled --save-report=<report_path> --backup-to=<backup_path>]
+  sweeper sweep invalids    --workspace=<workspace> [--table-name=<table_name> | --change-detect] [--verbose --try-fix --scheduled --save-report=<report_path> --backup-to=<backup_path>]
   sweeper sweep addresses   --workspace=<workspace> --table-name=<table-name> --field-name=<field_name> [--verbose --try-fix --save-report=<report_path> --backup-to=<backup_path>]
-  sweeper sweep metadata    --workspace=<workspace> [--table-name=<table_name> --verbose --try-fix --change-detect --scheduled --save-report=<report_path> --backup-to=<backup_path>]
-  sweeper sweep             --workspace=<workspace> [--table-name=<table_name> --verbose --try-fix --change-detect --scheduled --save-report=<report_path> --backup-to=<backup_path>]
+  sweeper sweep metadata    --workspace=<workspace> [--table-name=<table_name> | --change-detect] [--verbose --try-fix --scheduled --save-report=<report_path> --backup-to=<backup_path>]
+  sweeper sweep             --workspace=<workspace> [--table-name=<table_name> | --change-detect] [--verbose --try-fix --scheduled --save-report=<report_path> --backup-to=<backup_path>]
 
 Arguments:
   workspace     - path to workspace eg: `c:\\my.gdb`
   table_name    - name of feature class or table eg: `Roads` (needs to be fully qualified (eg: `SGID.Transportation.Roads`) for metadata sweeper)
   report_path   - folder to save report to eg: `c:\\temp`
   backup_path   - place to create a temp gdb and import original table
   field_name    - name of the field to check
```

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/address_parser.py` & `ugrc-sweeper-2.0.2/src/sweeper/address_parser.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/backup.py` & `ugrc-sweeper-2.0.2/src/sweeper/backup.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/config.py` & `ugrc-sweeper-2.0.2/src/sweeper/config.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/report.py` & `ugrc-sweeper-2.0.2/src/sweeper/report.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/street_types.json` & `ugrc-sweeper-2.0.2/src/sweeper/street_types.json`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/sweepers/UseLimitations.html` & `ugrc-sweeper-2.0.2/src/sweeper/sweepers/UseLimitations.html`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/sweepers/addresses.py` & `ugrc-sweeper-2.0.2/src/sweeper/sweepers/addresses.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/sweepers/duplicates.py` & `ugrc-sweeper-2.0.2/src/sweeper/sweepers/duplicates.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/sweepers/empties.py` & `ugrc-sweeper-2.0.2/src/sweeper/sweepers/empties.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/sweepers/invalids.py` & `ugrc-sweeper-2.0.2/src/sweeper/sweepers/invalids.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/sweepers/metadata.py` & `ugrc-sweeper-2.0.2/src/sweeper/sweepers/metadata.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/utilities.py` & `ugrc-sweeper-2.0.2/src/sweeper/utilities.py`

 * *Files identical despite different names*

### Comparing `ugrc-sweeper-2.0.1/src/sweeper/workspace_info.py` & `ugrc-sweeper-2.0.2/src/sweeper/workspace_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,20 +72,21 @@
 #: A function to return a list of feature classes based on the change detection table.
 def get_change_detection():
     checked_date = read_last_check_date()
 
     if checked_date:
         checked_string = datetime.datetime.strptime(checked_date, "%Y-%m-%d")
     else:
+        #: this was a deliberate choice so that the first time sweeper is run, it won't processes all tables
         checked_string = datetime.date.today()
 
     last_checked = checked_string.strftime("%m/%d/%Y")
     log.info(f"Last date change detection was checked: {last_checked}")
 
-    egdb = Path(config.get_config("CHANGE_DETECTION_CONNECTION"))
+    egdb = Path(config.get_config("CONNECTIONS_FOLDER")) / config.get_config("CHANGE_DETECTION_CONNECTION")
     cd_table = config.get_config("CHANGE_DETECTION_TABLE")
 
     egdb_conn = arcpy.ArcSDESQLExecute(str(egdb))
     sql = f"SELECT table_name FROM {cd_table} WHERE last_modified >= '{last_checked}'"
 
     #: result will typically be a nested list
     result = egdb_conn.execute(sql)
```

### Comparing `ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/PKG-INFO` & `ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugrc-sweeper
-Version: 2.0.1
+Version: 2.0.2
 Summary: CLI tool for making good data
 Home-page: https://github.com/agrc/sweeper
 Author: UGRC
 Author-email: ugrc-developers@utah.gov
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ugrc-sweeper-2.0.1/src/ugrc_sweeper.egg-info/SOURCES.txt` & `ugrc-sweeper-2.0.2/src/ugrc_sweeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*


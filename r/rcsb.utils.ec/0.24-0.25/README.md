# Comparing `tmp/rcsb.utils.ec-0.24.tar.gz` & `tmp/rcsb_utils_ec-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.ec-0.24.tar", last modified: Tue Jan 10 15:23:39 2023, max compression
+gzip compressed data, was "rcsb_utils_ec-0.25.tar", last modified: Wed May  8 19:30:54 2024, max compression
```

## Comparing `rcsb.utils.ec-0.24.tar` & `rcsb_utils_ec-0.25.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:23:39.112194 rcsb.utils.ec-0.24/
--rw-r--r--   0 vsts      (1001) docker     (122)      869 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1668 2023-01-10 15:23:39.112194 rcsb.utils.ec-0.24/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      968 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:23:39.108194 rcsb.utils.ec-0.24/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:23:39.108194 rcsb.utils.ec-0.24/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:23:39.112194 rcsb.utils.ec-0.24/rcsb/utils/ec/
--rw-r--r--   0 vsts      (1001) docker     (122)    18448 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/rcsb/utils/ec/EnzymeDatabaseProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/rcsb/utils/ec/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:23:39.108194 rcsb.utils.ec-0.24/rcsb.utils.ec.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1668 2023-01-10 15:23:39.000000 rcsb.utils.ec-0.24/rcsb.utils.ec.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      403 2023-01-10 15:23:39.000000 rcsb.utils.ec-0.24/rcsb.utils.ec.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-10 15:23:39.000000 rcsb.utils.ec-0.24/rcsb.utils.ec.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-10 15:23:20.000000 rcsb.utils.ec-0.24/rcsb.utils.ec.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       79 2023-01-10 15:23:39.000000 rcsb.utils.ec-0.24/rcsb.utils.ec.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-01-10 15:23:39.000000 rcsb.utils.ec-0.24/rcsb.utils.ec.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-01-10 15:23:39.112194 rcsb.utils.ec-0.24/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2272 2023-01-10 15:22:43.000000 rcsb.utils.ec-0.24/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 19:30:54.553711 rcsb_utils_ec-0.25/
+-rw-r--r--   0 vsts      (1001) docker     (127)      939 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1840 2024-05-08 19:30:54.553711 rcsb_utils_ec-0.25/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      968 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 19:30:54.553711 rcsb_utils_ec-0.25/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 19:30:54.553711 rcsb_utils_ec-0.25/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 19:30:54.553711 rcsb_utils_ec-0.25/rcsb/utils/ec/
+-rw-r--r--   0 vsts      (1001) docker     (127)    18908 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/rcsb/utils/ec/EnzymeDatabaseProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/rcsb/utils/ec/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-08 19:30:54.553711 rcsb_utils_ec-0.25/rcsb.utils.ec.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1840 2024-05-08 19:30:54.000000 rcsb_utils_ec-0.25/rcsb.utils.ec.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      403 2024-05-08 19:30:54.000000 rcsb_utils_ec-0.25/rcsb.utils.ec.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-08 19:30:54.000000 rcsb_utils_ec-0.25/rcsb.utils.ec.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-08 19:30:31.000000 rcsb_utils_ec-0.25/rcsb.utils.ec.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       79 2024-05-08 19:30:54.000000 rcsb_utils_ec-0.25/rcsb.utils.ec.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-08 19:30:54.000000 rcsb_utils_ec-0.25/rcsb.utils.ec.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-08 19:30:54.553711 rcsb_utils_ec-0.25/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2272 2024-05-08 19:29:44.000000 rcsb_utils_ec-0.25/setup.py
```

### Comparing `rcsb.utils.ec-0.24/HISTORY.txt` & `rcsb_utils_ec-0.25/HISTORY.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,7 +10,8 @@
  24-Nov-2019 V0.18 add normalize() and exists() methods
   8-Dec-2019 V0.19 parse history records looking for EC replacements
  25-Jan-2020 V0.20 add fallback data resource
   3-Feb-2020 V0.21 update dependencies
  25-Jul-2021 V0.22 Make EnzymeDatabaseProvider a subclass of StashableBase, update instal and pipeline
   4-Jan-2022 V0.23 Update list of missing ecIds to reflect latest version of source data
   9-Jan-2023 V0.24 Configuration changes to support tox 4
+  8-May-2024 V0.25 Add additional data quality check to file download
```

### Comparing `rcsb.utils.ec-0.24/LICENSE` & `rcsb_utils_ec-0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.ec-0.24/PKG-INFO` & `rcsb_utils_ec-0.25/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.ec
-Version: 0.24
+Version: 0.25
 Summary: RCSB Python utility classes for processing EC classification data
 Home-page: https://github.com/rcsb/py-rcsb_utils_ec
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rcsb.utils.io>=1.15
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
 
 # RCSB Python Enzyme Classification Data Utilities
 
 [![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_ec?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=3&branchName=master)
 
 ## Introduction
```

### Comparing `rcsb.utils.ec-0.24/README.md` & `rcsb_utils_ec-0.25/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.ec-0.24/rcsb/utils/ec/EnzymeDatabaseProvider.py` & `rcsb_utils_ec-0.25/rcsb/utils/ec/EnzymeDatabaseProvider.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # File:    EnzymeDatabaseProvider.py
 # Author:  J. Westbrook
 # Date:    24-Jan-2019
 # Version: 0.001
 #
 # Update:
 # 21-Jul-2021 jdw  Make this provider a subclass of StashableBase
+#  8-May-2024 dwp  Add additional data quality check to file download (in case data file is empty)
 #
 ##
 """
 Various utilities for extracting data Enzyme database export data files
 and returning lineage details.
 """
 
@@ -123,14 +124,15 @@
                 Returns:
                     dictionary[ec_id] = {'name_list': ... , 'id_list': ... 'depth_list': ... }
         """
         enzD = {}
         #
         mU = MarshalUtil()
         fU = FileUtil()
+        ok, okFetch = False, False
         fn = fU.getFileName(urlTarget)
         xmlFilePath = os.path.join(dirPath, fn)
         enzymeDataPath = os.path.join(dirPath, enzymeDataFileName)
         self.__mU.mkdir(dirPath)
         #
         if not useCache:
             for fp in [xmlFilePath, enzymeDataPath]:
@@ -143,19 +145,22 @@
             enzD = self.__mU.doImport(enzymeDataPath, fmt="json")
         elif not useCache:
             if useCache and fU.exists(xmlFilePath):
                 logger.info("Using an existing resource file %s", xmlFilePath)
                 ok = True
             else:
                 logger.info("Fetching url %s to resource file %s", urlTarget, xmlFilePath)
-                ok = fU.get(urlTarget, xmlFilePath)
-                logger.info("Enzyme data fetch status is %r", ok)
+                okFetch = fU.get(urlTarget, xmlFilePath)
+                ok = fU.size(xmlFilePath) > 10000 and okFetch
+                logger.info("Enzyme data fetch status is %r, data integrity status is %r", okFetch, ok)
                 if not ok:
-                    ok = fU.get(urlTargetFallback, xmlFilePath)
-                    logger.info("Enzyme data fallback fetch status is %r", ok)
+                    logger.info("Fetching fallback url %s to resource file %s", urlTargetFallback, xmlFilePath)
+                    okFetch = fU.get(urlTargetFallback, xmlFilePath)
+                    ok = fU.size(xmlFilePath) > 10000 and okFetch
+                    logger.info("Enzyme data fallback fetch status is %r, data integrity status is %r", okFetch, ok)
             if ok:
                 xrt = mU.doImport(xmlFilePath, fmt="xml")
                 if self.__debug:
                     self.__traverse(xrt, ns="")
                 rD = self.__extract(xrt)
                 enzD = self.__build(rD)
                 ok = self.__mU.doExport(enzymeDataPath, enzD, fmt="json", indent=3)
```

### Comparing `rcsb.utils.ec-0.24/rcsb.utils.ec.egg-info/PKG-INFO` & `rcsb_utils_ec-0.25/rcsb.utils.ec.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.ec
-Version: 0.24
+Version: 0.25
 Summary: RCSB Python utility classes for processing EC classification data
 Home-page: https://github.com/rcsb/py-rcsb_utils_ec
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: rcsb.utils.io>=1.15
+Requires-Dist: beautifulsoup4
+Requires-Dist: lxml
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
 
 # RCSB Python Enzyme Classification Data Utilities
 
 [![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_ec?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=3&branchName=master)
 
 ## Introduction
```

### Comparing `rcsb.utils.ec-0.24/setup.py` & `rcsb_utils_ec-0.25/setup.py`

 * *Files identical despite different names*


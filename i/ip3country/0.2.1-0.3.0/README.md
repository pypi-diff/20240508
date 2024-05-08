# Comparing `tmp/ip3country-0.2.1.tar.gz` & `tmp/ip3country-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ip3country-0.2.1.tar", last modified: Thu Aug 18 22:30:54 2022, max compression
+gzip compressed data, was "ip3country-0.3.0.tar", last modified: Wed May  8 17:34:20 2024, max compression
```

## Comparing `ip3country-0.2.1.tar` & `ip3country-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2022-08-18 22:30:54.375710 ip3country-0.2.1/
--rw-r--r--   0 tore       (501) staff       (20)      750 2022-07-13 18:49:07.000000 ip3country-0.2.1/LICENSE
--rw-r--r--   0 tore       (501) staff       (20)       39 2022-07-13 18:49:07.000000 ip3country-0.2.1/MANIFEST.in
--rw-r--r--   0 tore       (501) staff       (20)      604 2022-08-18 22:30:54.375594 ip3country-0.2.1/PKG-INFO
--rw-r--r--   0 tore       (501) staff       (20)     1714 2022-07-13 18:49:07.000000 ip3country-0.2.1/README.md
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2022-08-18 22:30:54.373995 ip3country-0.2.1/ip3country/
--rw-r--r--   0 tore       (501) staff       (20)       41 2022-07-13 18:49:07.000000 ip3country-0.2.1/ip3country/__init__.py
--rw-r--r--   0 tore       (501) staff       (20)     2336 2022-07-13 18:49:07.000000 ip3country-0.2.1/ip3country/country_lookup.py
--rw-r--r--   0 tore       (501) staff       (20)     2842 2022-07-13 18:49:07.000000 ip3country-0.2.1/ip3country/country_lookup_test.py
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2022-08-18 22:30:54.374515 ip3country-0.2.1/ip3country/data/
--rw-r--r--   0 tore       (501) staff       (20)   417307 2022-07-13 18:49:07.000000 ip3country-0.2.1/ip3country/data/ip_supalite.table
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2022-08-18 22:30:54.374419 ip3country-0.2.1/ip3country.egg-info/
--rw-r--r--   0 tore       (501) staff       (20)      604 2022-08-18 22:30:54.000000 ip3country-0.2.1/ip3country.egg-info/PKG-INFO
--rw-r--r--   0 tore       (501) staff       (20)      294 2022-08-18 22:30:54.000000 ip3country-0.2.1/ip3country.egg-info/SOURCES.txt
--rw-r--r--   0 tore       (501) staff       (20)        1 2022-08-18 22:30:54.000000 ip3country-0.2.1/ip3country.egg-info/dependency_links.txt
--rw-r--r--   0 tore       (501) staff       (20)       11 2022-08-18 22:30:54.000000 ip3country-0.2.1/ip3country.egg-info/top_level.txt
--rw-r--r--   0 tore       (501) staff       (20)       38 2022-08-18 22:30:54.375754 ip3country-0.2.1/setup.cfg
--rw-r--r--   0 tore       (501) staff       (20)      814 2022-08-18 22:30:50.000000 ip3country-0.2.1/setup.py
+drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-05-08 17:34:20.679646 ip3country-0.3.0/
+-rw-r--r--   0 tore       (501) staff       (20)      750 2022-07-13 18:49:07.000000 ip3country-0.3.0/LICENSE
+-rw-r--r--   0 tore       (501) staff       (20)       39 2022-07-13 18:49:07.000000 ip3country-0.3.0/MANIFEST.in
+-rw-r--r--   0 tore       (501) staff       (20)      604 2024-05-08 17:34:20.679435 ip3country-0.3.0/PKG-INFO
+-rw-r--r--   0 tore       (501) staff       (20)     1714 2022-07-13 18:49:07.000000 ip3country-0.3.0/README.md
+drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-05-08 17:34:20.678024 ip3country-0.3.0/ip3country/
+-rw-r--r--   0 tore       (501) staff       (20)       41 2022-07-13 18:49:07.000000 ip3country-0.3.0/ip3country/__init__.py
+-rw-r--r--   0 tore       (501) staff       (20)     2394 2024-05-08 17:34:03.000000 ip3country-0.3.0/ip3country/country_lookup.py
+-rw-r--r--   0 tore       (501) staff       (20)     2842 2022-07-13 18:49:07.000000 ip3country-0.3.0/ip3country/country_lookup_test.py
+drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-05-08 17:34:20.678613 ip3country-0.3.0/ip3country/data/
+-rw-r--r--   0 tore       (501) staff       (20)   417307 2022-07-13 18:49:07.000000 ip3country-0.3.0/ip3country/data/ip_supalite.table
+-rw-r--r--   0 tore       (501) staff       (20)        0 2024-05-08 17:34:03.000000 ip3country-0.3.0/ip3country/py.typed
+drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-05-08 17:34:20.679224 ip3country-0.3.0/ip3country.egg-info/
+-rw-r--r--   0 tore       (501) staff       (20)      604 2024-05-08 17:34:20.000000 ip3country-0.3.0/ip3country.egg-info/PKG-INFO
+-rw-r--r--   0 tore       (501) staff       (20)      314 2024-05-08 17:34:20.000000 ip3country-0.3.0/ip3country.egg-info/SOURCES.txt
+-rw-r--r--   0 tore       (501) staff       (20)        1 2024-05-08 17:34:20.000000 ip3country-0.3.0/ip3country.egg-info/dependency_links.txt
+-rw-r--r--   0 tore       (501) staff       (20)       11 2024-05-08 17:34:20.000000 ip3country-0.3.0/ip3country.egg-info/top_level.txt
+-rw-r--r--   0 tore       (501) staff       (20)       38 2024-05-08 17:34:20.679686 ip3country-0.3.0/setup.cfg
+-rw-r--r--   0 tore       (501) staff       (20)      814 2024-05-08 17:34:03.000000 ip3country-0.3.0/setup.py
```

### Comparing `ip3country-0.2.1/LICENSE` & `ip3country-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ip3country-0.2.1/PKG-INFO` & `ip3country-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ip3country
-Version: 0.2.1
+Version: 0.3.0
 Summary: A zero-dependency, local, fast, tiny ip-address to country lookup
 Home-page: https://github.com/statsig-io/ip3country-py
 Author: Statsig
 Author-email: tore@statsig.com
 License: ISC
 Keywords: ip,country,lookup,statsig
 Classifier: Intended Audience :: Developers
```

### Comparing `ip3country-0.2.1/README.md` & `ip3country-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ip3country-0.2.1/ip3country/country_lookup.py` & `ip3country-0.3.0/ip3country/country_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
+from typing import List
+
 
 class CountryLookup:
-    countryCodes = []
-    countryTable = []
-    ipRanges = []
+    countryCodes: List[str] = []
+    countryTable: List[str] = []
+    ipRanges: List[int] = []
 
     def __init__(self):
         datafile = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'data', 'ip_supalite.table')
         with open(datafile, mode="rb") as file:
             self.ipSupalite = file.read()
         self.processTable()
```

### Comparing `ip3country-0.2.1/ip3country/country_lookup_test.py` & `ip3country-0.3.0/ip3country/country_lookup_test.py`

 * *Files identical despite different names*

### Comparing `ip3country-0.2.1/ip3country/data/ip_supalite.table` & `ip3country-0.3.0/ip3country/data/ip_supalite.table`

 * *Files identical despite different names*

### Comparing `ip3country-0.2.1/ip3country.egg-info/PKG-INFO` & `ip3country-0.3.0/ip3country.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ip3country
-Version: 0.2.1
+Version: 0.3.0
 Summary: A zero-dependency, local, fast, tiny ip-address to country lookup
 Home-page: https://github.com/statsig-io/ip3country-py
 Author: Statsig
 Author-email: tore@statsig.com
 License: ISC
 Keywords: ip,country,lookup,statsig
 Classifier: Intended Audience :: Developers
```

### Comparing `ip3country-0.2.1/setup.py` & `ip3country-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='ip3country',
-    version='0.2.1',
+    version='0.3.0',
     url='https://github.com/statsig-io/ip3country-py',
     author='Statsig',
     author_email='tore@statsig.com',
     description='A zero-dependency, local, fast, tiny ip-address to country lookup',
     long_description="See https://github.com/statsig-io/ip3country-py",
     long_description_content_type="text/markdown",
     keywords=['ip', 'country', 'lookup', 'statsig'],
```


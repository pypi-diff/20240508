# Comparing `tmp/esi_utils_pager-1.1.13.tar.gz` & `tmp/esi_utils_pager-1.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi_utils_pager-1.1.13.tar", last modified: Tue May  7 17:13:47 2024, max compression
+gzip compressed data, was "esi_utils_pager-1.1.14.tar", last modified: Wed May  8 20:27:11 2024, max compression
```

## Comparing `esi_utils_pager-1.1.13.tar` & `esi_utils_pager-1.1.14.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.591933 esi_utils_pager-1.1.13/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/LICENSE.md
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)    10517 2024-05-07 17:13:47.591933 esi_utils_pager-1.1.13/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7377 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1254 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-05-07 17:13:47.591933 esi_utils_pager-1.1.13/setup.cfg
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.575933 esi_utils_pager-1.1.13/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.579933 esi_utils_pager-1.1.13/src/esi_utils_pager/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:12:39.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.583933 esi_utils_pager-1.1.13/src/esi_utils_pager/bin/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    10661 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/bin/pagerlite.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11717 2024-05-07 16:55:36.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/calc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/config.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/country.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.587933 esi_utils_pager-1.1.13/src/esi_utils_pager/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/countries.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    54009 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/economic.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/economy.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    33076 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/fatality.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/fatality.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_casualty.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_casualty.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_collapse_mmi.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_inventory.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_inventory.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_workforce.hdf
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_workforce.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/econexposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24334 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/emploss.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/exposure.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/growth.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/pandas_container.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2467 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/probs.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2024-05-07 15:49:51.000000 esi_utils_pager-1.1.13/src/esi_utils_pager/semimodel.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-07 17:13:47.587933 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)    10517 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1441 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      281 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2024-05-07 17:13:47.000000 esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-08 20:27:11.437611 esi_utils_pager-1.1.14/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/LICENSE.md
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)    13175 2024-05-08 20:27:11.437611 esi_utils_pager-1.1.14/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10035 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1254 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-05-08 20:27:11.437611 esi_utils_pager-1.1.14/setup.cfg
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-08 20:27:11.421610 esi_utils_pager-1.1.14/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-08 20:27:11.425610 esi_utils_pager-1.1.14/src/esi_utils_pager/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-05-08 20:26:03.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-08 20:27:11.425610 esi_utils_pager-1.1.14/src/esi_utils_pager/bin/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    10406 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/bin/pagerlite.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11868 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/calc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2629 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/config.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4444 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/country.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-08 20:27:11.433611 esi_utils_pager-1.1.14/src/esi_utils_pager/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   288256 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   366080 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   974848 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    44597 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/countries.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    54009 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/economic.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/economy.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    33076 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/fatality.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/fatality.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   176744 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_casualty.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   218436 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_casualty.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   260968 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_collapse_mmi.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   198134 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_collapse_mmi.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  1006280 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_inventory.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   290497 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_inventory.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27120 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_workforce.hdf
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14527 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_workforce.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7424 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/econexposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24334 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/emploss.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8367 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/exposure.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7078 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/growth.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      422 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/pandas_container.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2467 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/probs.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27500 2024-05-08 20:13:59.000000 esi_utils_pager-1.1.14/src/esi_utils_pager/semimodel.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-05-08 20:27:11.433611 esi_utils_pager-1.1.14/src/esi_utils_pager.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)    13175 2024-05-08 20:27:11.000000 esi_utils_pager-1.1.14/src/esi_utils_pager.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1441 2024-05-08 20:27:11.000000 esi_utils_pager-1.1.14/src/esi_utils_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-05-08 20:27:11.000000 esi_utils_pager-1.1.14/src/esi_utils_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       65 2024-05-08 20:27:11.000000 esi_utils_pager-1.1.14/src/esi_utils_pager.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      281 2024-05-08 20:27:11.000000 esi_utils_pager-1.1.14/src/esi_utils_pager.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       16 2024-05-08 20:27:11.000000 esi_utils_pager-1.1.14/src/esi_utils_pager.egg-info/top_level.txt
```

### Comparing `esi_utils_pager-1.1.13/LICENSE.md` & `esi_utils_pager-1.1.14/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/PKG-INFO` & `esi_utils_pager-1.1.14/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,7 @@
-Metadata-Version: 2.1
-Name: esi-utils-pager
-Version: 1.1.13
-Summary: USGS PAGER loss modeling functionality
-Author-email: Mike Hearne <mhearne@usgs.gov>
-License: License
-        =======
-        
-        Unless otherwise noted, This project is in the public domain in the United
-        States because it contains materials that originally came from the United
-        States Geological Survey, an agency of the United States Department of
-        Interior. For more information, see the official USGS copyright policy at
-        https://www2.usgs.gov/visual-id/credit_usgs.html#copyright
-        
-        Additionally, we waive copyright and related rights in the work
-        worldwide through the CC0 1.0 Universal public domain dedication.
-        
-        
-        CC0 1.0 Universal Summary
-        -------------------------
-        
-        This is a human-readable summary of the
-        [Legal Code (read the full text)][1].
-        
-        
-        ### No Copyright
-        
-        The person who associated a work with this deed has dedicated the work to
-        the public domain by waiving all of his or her rights to the work worldwide
-        under copyright law, including all related and neighboring rights, to the
-        extent allowed by law.
-        
-        You can copy, modify, distribute and perform the work, even for commercial
-        purposes, all without asking permission.
-        
-        
-        ### Other Information
-        
-        In no way are the patent or trademark rights of any person affected by CC0,
-        nor are the rights that other persons may have in the work or in how the
-        work is used, such as publicity or privacy rights.
-        
-        Unless expressly stated otherwise, the person who associated a work with
-        this deed makes no warranties about the work, and disclaims liability for
-        all uses of the work, to the fullest extent permitted by applicable law.
-        When using or citing the work, you should not imply endorsement by the
-        author or the affirmer.
-        
-        
-        
-        [1]: https://creativecommons.org/publicdomain/zero/1.0/legalcode
-        
-Keywords: losses,earthquake
-Requires-Python: <=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: esi-utils-io
-Requires-Dist: esi-utils-time
-Requires-Dist: fiona
-Requires-Dist: h5py
-Requires-Dist: mapio>=0.8.5
-Requires-Dist: numpy<2.0.0
-Requires-Dist: openpyxl
-Requires-Dist: pandas
-Requires-Dist: PyYAML
-Requires-Dist: rasterio
-Requires-Dist: scipy
-Requires-Dist: shapely
-Requires-Dist: xlrd
-Provides-Extra: dev
-Requires-Dist: build>=0.7.0; extra == "dev"
-Requires-Dist: black>=21; extra == "dev"
-Requires-Dist: flake8>=3.9; extra == "dev"
-Requires-Dist: ipython>=7.26; extra == "dev"
-Requires-Dist: notebook>=6.4.1; extra == "dev"
-Requires-Dist: twine>=3.7.0; extra == "dev"
-Provides-Extra: test
-Requires-Dist: pytest>=6.2; extra == "test"
-Requires-Dist: pytest-cov>=2.12.0; extra == "test"
-Provides-Extra: build
-Requires-Dist: build; extra == "build"
-Requires-Dist: twine; extra == "build"
-Requires-Dist: check-wheel-contents; extra == "build"
-
 # Table of Contents
 - [Table of Contents](#table-of-contents)
 - [Introduction](#introduction)
 - [Installation](#installation)
 - [Upgrading](#upgrading)
 - [Required data](#required-data)
 - [Configuration (for calc\_pager\_event API usage and command line usage)](#configuration-for-calc_pager_event-api-usage-and-command-line-usage)
@@ -241,18 +157,62 @@
 To run the PAGER empirical models on a folder but only for events between 2010 and 2017:
 
 `pagerlite -o output.xlsx batch -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59`
 
 To run PAGER empirical models on a folder but only for events in Japan:
 `pagerlite -o output.xlsx batch -f /data/shakemap_output/ -b 30.844021 44.762578 128.336525  149.031827`
 
+It is possible to provide your own PAGER input files for the empirical fatality and economic models, 
+and for the semi-empirical fatality model. These files can be found in the repository:
+
+ - [Empirical fatality model](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/fatality.xlsx?ref_type=heads):
+ - [Empirical economic model](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/economic.xlsx?ref_type=heads)
+ - Semi-Empirical Model Data:
+   - [Inventory](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/semi_inventory.xlsx?ref_type=heads)
+   - [Workforce](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/semi_workforce.xlsx?ref_type=heads)
+   - [Collapse](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/semi_collapse_mmi.xlsx?ref_type=heads)
+   - [Casualty](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/semi_casualty.xlsx?ref_type=heads)
+
+
+To run pagerlite on the event `us10003re5` with custom empirical data files:
+
+`pagerlite -f ~/custom_fatality.xlsx -e ~/custom_economic.xlsx event us10003re5`
+
+To run the semi-empirical model with custom data files, assuming those files are all in the same folder, 
+and all named as they are in the repository (semi_inventory.xlsx, semi_workforce.xlsx, 
+semi_collapse_mmi.xlsx, semi_casualty.xlsx):
+
+`pagerlite -s --semi-folder ~/test_semi/test1 event us10003re5`
+
+Any custom input files can be used in either `event` or `batch` modes.
+
 See the help for more options (depth and magnitude ranges) on restricting processing of ShakeMap
 grids.
 
+### Running background processes
+
+Running pagerlite over a large number of events can take many minutes or hours
+depending on the number of events being run.  If you have access to a Linux system, you can
+run a batch process in the background and also ensure that the process will continue when you
+disconnect from the remote Linux system. The way to do this is to combine the `nohup` command
+(short for "no hang up") and the ampersand "&" character at the end of the command. 
+Below is an example running on all events inside an Afghanistan bounding box:
+
+`nohup pagerlite  -o ~/afghanistan_text.csv -v batch -f /data/shakedata/ -b 60.271 73.367 29.581 38.795 > ~/afghanistan_log.txt&`
+
+Executing this command with the "&" at the end will start it running in the background. When it is done, you
+can run `tail afghanistan_log.txt` until you see a line that looks like this:
+
+`Saving 1258 rows to afghanistan_text.csv`
+
+If you want to watch the progress of pagerlite, you can run:
+
+`tail -f afghanistan_log.txt`
 
+and see output streaming by as each event is processed.
 
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi_utils_pager-1.1.13/pyproject.toml` & `esi_utils_pager-1.1.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/bin/pagerlite.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/bin/pagerlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,15 @@
                 outtime = datetime.strptime(timestring, DATEFMT)
             except Exception:
                 raise Exception("Could not parse time or date from %s" % timestring)
     return outtime
 
 
 def set_logging(args):
-    if args.verbose:
-        loglevel = logging.INFO
-    else:
-        loglevel = logging.CRITICAL
+    loglevel = logging.INFO
     logging.basicConfig(
         level=loglevel,
         format="%(asctime)s %(message)s",
         handlers=[logging.StreamHandler()],
     )
 
 
@@ -115,23 +112,23 @@
 def run_event(args):
     set_logging(args)
     check_input_files(args)
     config = read_config()
     file_or_url = pathlib.Path(args.file_or_url)
     if file_or_url.exists():
         dataframe = calc_pager_event(
-            args.grid_xml,
+            args.file_or_url,
             config,
-            args.semimodel,
+            args.semi_folder,
             args.fatality_file,
             args.economic_file,
             args.semi_folder,
         )
     else:
-        url = EVENT_TEMPLATE.format(eventid=args.eventid)
+        url = EVENT_TEMPLATE.format(eventid=args.file_or_url)
         with tempfile.TemporaryDirectory() as tempdir:
             with urlopen(url) as fh:
                 data = fh.read().decode("utf8")
                 jdict = json.loads(data)
                 if "shakemap" not in jdict["properties"]["types"]:
                     print(f"No ShakeMap for event {args.eventid}. Exiting.")
                     sys.exit(1)
@@ -143,28 +140,27 @@
                 tmpgridfile = pathlib.Path(tempdir) / "tmp.xml"
                 with open(tmpgridfile, "wt") as fout:
                     fout.write(xdata)
                 config = read_config()
                 dataframe = calc_pager_event(
                     tmpgridfile,
                     config,
-                    args.semimodel,
+                    args.semi_folder,
                     args.fatality_file,
                     args.economic_file,
                     args.semi_folder,
                 )
-        write_output(args, dataframe)
+    write_output(args, dataframe)
 
 
 def run_batch(args):
     set_logging(args)
     check_input_files(args)
     dataframe = calc_pager_events(
         args.folder,
-        args.verbose,
         args.run_semi,
         args.fatality_file,
         args.economic_file,
         args.semi_folder,
         timerange=args.time_range,
         bounds=args.bounds,
         magrange=args.mag_range,
@@ -222,21 +218,15 @@
         help="Calculate semi-empirical model results as well.",
         action="store_true",
         default=False,
     )
     parser.add_argument(
         "-o", "--outfile", help="Specify output file (.xlsx for Excel, .csv for CSV)"
     )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        default=False,
-        action="store_true",
-        help="Print progress output to the screen",
-    )
+
     parser.add_argument(
         "-f", "--fatality-file", default=None, help="Path to custom fatality Excel file"
     )
     parser.add_argument(
         "-e", "--economic-file", default=None, help="Path to custom economic Excel file"
     )
     parser.add_argument(
```

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/calc.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,14 @@
     local_time = get_local_time(
         shake_tuple[1]["event_timestamp"],
         config["model_data"]["timezones_file"],
         shake_tuple[1]["lat"],
         shake_tuple[1]["lon"],
     )
     eventid = shake_tuple[1]["event_id"]
-    print(f"Processing event {eventid}...")
     master_row = {}
     master_row["EventID"] = shake_tuple[1]["event_id"]
     master_row["Time"] = shake_tuple[1]["event_timestamp"]
     master_row["LocalTime"] = local_time
     master_row["Latitude"] = shake_tuple[1]["lat"]
     master_row["Longitude"] = shake_tuple[1]["lon"]
     master_row["Depth"] = shake_tuple[1]["depth"]
@@ -212,15 +211,14 @@
             ecoframe = ecoframe.join(final_frame, on=["CountryCode"])
 
     return ecoframe
 
 
 def calc_pager_events(
     gridfolder,
-    verbose,
     run_semi,
     fatality_file,
     economic_file,
     semi_folder,
     timerange=None,
     bounds=None,
     magrange=None,
@@ -295,19 +293,24 @@
             grid_index["depth"] < depthrange[1]
         )
     if magrange is not None:
         magidx = (grid_index["magnitude"] >= magrange[0]) & (
             grid_index["magnitude"] < magrange[1]
         )
     events = grid_index[timeidx & boundsidx & depthidx & magidx]
+    if not len(events):
+        logging.info(
+            "No events matching criteria in input directory. Returning empty data set."
+        )
+        return pd.DataFrame({})
+    logging.info(f"Processing {len(events)} events...")
     dataframes = []
     for idx, row in events.iterrows():
         gridfile = row["gridfile"]
-        if verbose:
-            logging.info(f"Parsing {gridfile}...")
+        logging.info(f"Parsing {gridfile}...")
         dataframe = calc_pager_event(
             gridfile,
             config,
             run_semi,
             fatality_file,
             economic_file,
             semi_folder,
```

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/config.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/config.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/country.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/country.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2.xls`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/API_NY.GDP.PCAP.CD_DS2_en_excel_v2_4770383.xls`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/WPP2015_POP_F02_POPULATION_GROWTH_RATE.xls`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/countries.xlsx` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/countries.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/economic.xlsx` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/economic.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/economy.xml` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/economy.xml`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/fatality.xlsx` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/fatality.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/fatality.xml` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/fatality.xml`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_casualty.hdf` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_casualty.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_casualty.xlsx` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_casualty.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_collapse_mmi.hdf` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_collapse_mmi.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_collapse_mmi.xlsx` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_collapse_mmi.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_inventory.hdf` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_inventory.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_inventory.xlsx` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_inventory.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_workforce.hdf` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_workforce.hdf`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/data/semi_workforce.xlsx` & `esi_utils_pager-1.1.14/src/esi_utils_pager/data/semi_workforce.xlsx`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/econexposure.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/econexposure.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/emploss.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/emploss.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/exposure.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/exposure.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/growth.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/growth.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/probs.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/probs.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager/semimodel.py` & `esi_utils_pager-1.1.14/src/esi_utils_pager/semimodel.py`

 * *Files identical despite different names*

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/PKG-INFO` & `esi_utils_pager-1.1.14/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-utils-pager
-Version: 1.1.13
+Version: 1.1.14
 Summary: USGS PAGER loss modeling functionality
 Author-email: Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -241,18 +241,62 @@
 To run the PAGER empirical models on a folder but only for events between 2010 and 2017:
 
 `pagerlite -o output.xlsx batch -f /data/shakemap_output/ -t 2010-01-01 2017-12-31T23:59:59`
 
 To run PAGER empirical models on a folder but only for events in Japan:
 `pagerlite -o output.xlsx batch -f /data/shakemap_output/ -b 30.844021 44.762578 128.336525  149.031827`
 
+It is possible to provide your own PAGER input files for the empirical fatality and economic models, 
+and for the semi-empirical fatality model. These files can be found in the repository:
+
+ - [Empirical fatality model](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/fatality.xlsx?ref_type=heads):
+ - [Empirical economic model](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/economic.xlsx?ref_type=heads)
+ - Semi-Empirical Model Data:
+   - [Inventory](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/semi_inventory.xlsx?ref_type=heads)
+   - [Workforce](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/semi_workforce.xlsx?ref_type=heads)
+   - [Collapse](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/semi_collapse_mmi.xlsx?ref_type=heads)
+   - [Casualty](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/raw/main/src/esi_utils_pager/data/semi_casualty.xlsx?ref_type=heads)
+
+
+To run pagerlite on the event `us10003re5` with custom empirical data files:
+
+`pagerlite -f ~/custom_fatality.xlsx -e ~/custom_economic.xlsx event us10003re5`
+
+To run the semi-empirical model with custom data files, assuming those files are all in the same folder, 
+and all named as they are in the repository (semi_inventory.xlsx, semi_workforce.xlsx, 
+semi_collapse_mmi.xlsx, semi_casualty.xlsx):
+
+`pagerlite -s --semi-folder ~/test_semi/test1 event us10003re5`
+
+Any custom input files can be used in either `event` or `batch` modes.
+
 See the help for more options (depth and magnitude ranges) on restricting processing of ShakeMap
 grids.
 
+### Running background processes
+
+Running pagerlite over a large number of events can take many minutes or hours
+depending on the number of events being run.  If you have access to a Linux system, you can
+run a batch process in the background and also ensure that the process will continue when you
+disconnect from the remote Linux system. The way to do this is to combine the `nohup` command
+(short for "no hang up") and the ampersand "&" character at the end of the command. 
+Below is an example running on all events inside an Afghanistan bounding box:
+
+`nohup pagerlite  -o ~/afghanistan_text.csv -v batch -f /data/shakedata/ -b 60.271 73.367 29.581 38.795 > ~/afghanistan_log.txt&`
+
+Executing this command with the "&" at the end will start it running in the background. When it is done, you
+can run `tail afghanistan_log.txt` until you see a line that looks like this:
+
+`Saving 1258 rows to afghanistan_text.csv`
+
+If you want to watch the progress of pagerlite, you can run:
+
+`tail -f afghanistan_log.txt`
 
+and see output streaming by as each event is processed.
 
 
 # Library Usage
 
 Usage of the relevant code modules is detailed in the Jupyter notebooks, most notably in the 
 [Earthquake Losses notebook](https://code.usgs.gov/ghsc/esi/esi-utils-pager/-/blob/main/notebooks/EarthquakeLosses.ipynb)
```

### Comparing `esi_utils_pager-1.1.13/src/esi_utils_pager.egg-info/SOURCES.txt` & `esi_utils_pager-1.1.14/src/esi_utils_pager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


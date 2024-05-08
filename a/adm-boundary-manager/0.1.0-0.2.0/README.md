# Comparing `tmp/adm-boundary-manager-0.1.0.tar.gz` & `tmp/adm_boundary_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adm-boundary-manager-0.1.0.tar", last modified: Tue Nov 28 09:56:12 2023, max compression
+gzip compressed data, was "adm_boundary_manager-0.2.0.tar", last modified: Wed May  8 10:59:14 2024, max compression
```

## Comparing `adm-boundary-manager-0.1.0.tar` & `adm_boundary_manager-0.2.0.tar`

### file list

```diff
@@ -1,42 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:12.627641 adm-boundary-manager-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20856 2023-11-28 09:56:12.627641 adm-boundary-manager-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19707 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:12.627641 adm-boundary-manager-0.1.0/adm_boundary_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20856 2023-11-28 09:56:12.000000 adm-boundary-manager-0.1.0/adm_boundary_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-11-28 09:56:12.000000 adm-boundary-manager-0.1.0/adm_boundary_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 09:56:12.000000 adm-boundary-manager-0.1.0/adm_boundary_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-11-28 09:56:12.000000 adm-boundary-manager-0.1.0/adm_boundary_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-28 09:56:12.000000 adm-boundary-manager-0.1.0/adm_boundary_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:12.623641 adm-boundary-manager-0.1.0/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:12.627641 adm-boundary-manager-0.1.0/adminboundarymanager/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/loaders/cod_abs_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/loaders/gadm_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/loaders/generic_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:12.627641 adm-boundary-manager-0.1.0/adminboundarymanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0005_alter_country_country.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:12.623641 adm-boundary-manager-0.1.0/adminboundarymanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:12.627641 adm-boundary-manager-0.1.0/adminboundarymanager/templates/adminboundarymanager/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/adminboundarymanager/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-28 09:55:57.000000 adm-boundary-manager-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-11-28 09:56:12.627641 adm-boundary-manager-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.774520 adm_boundary_manager-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20897 2024-05-08 10:59:14.774520 adm_boundary_manager-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19707 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.774520 adm_boundary_manager-0.2.0/adm_boundary_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20897 2024-05-08 10:59:14.000000 adm_boundary_manager-0.2.0/adm_boundary_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-08 10:59:14.000000 adm_boundary_manager-0.2.0/adm_boundary_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:59:14.000000 adm_boundary_manager-0.2.0/adm_boundary_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-08 10:59:14.000000 adm_boundary_manager-0.2.0/adm_boundary_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 10:59:14.000000 adm_boundary_manager-0.2.0/adm_boundary_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.770520 adm_boundary_manager-0.2.0/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.770520 adm_boundary_manager-0.2.0/adminboundarymanager/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/loaders/cod_abs_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/loaders/gadm_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/loaders/generic_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.774520 adm_boundary_manager-0.2.0/adminboundarymanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0005_alter_country_country.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.766519 adm_boundary_manager-0.2.0/adminboundarymanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.766519 adm_boundary_manager-0.2.0/adminboundarymanager/static/adminboundarymanager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.774520 adm_boundary_manager-0.2.0/adminboundarymanager/static/adminboundarymanager/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    70412 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/static/adminboundarymanager/css/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.774520 adm_boundary_manager-0.2.0/adminboundarymanager/static/adminboundarymanager/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   745424 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/static/adminboundarymanager/js/maplibre-gl.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.766519 adm_boundary_manager-0.2.0/adminboundarymanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:59:14.774520 adm_boundary_manager-0.2.0/adminboundarymanager/templates/adminboundarymanager/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/adminboundarymanager/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 10:59:10.000000 adm_boundary_manager-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-08 10:59:14.774520 adm_boundary_manager-0.2.0/setup.cfg
```

### Comparing `adm-boundary-manager-0.1.0/PKG-INFO` & `adm_boundary_manager-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adm-boundary-manager
-Version: 0.1.0
+Version: 0.2.0
 Summary: Load, manage and visualize Administrative Boundaries Data in Wagtail
 Home-page: https://github.com/wmo-raf/adm-boundary-manager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -21,14 +21,15 @@
 Requires-Dist: wagtail>=4.2.2
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: geopandas>=0.12.2
 Requires-Dist: django-filter>=22.1
 Requires-Dist: django-countries>=7.5.1
 Requires-Dist: django-countries-geoextent>=0.0.1
 Requires-Dist: wagtail-cache>=2.3.0
+Requires-Dist: wagtail-modeladmin>=1.0.0
 
 # Administrative Boundaries Manager
 
 Load, manage and visualize administrative boundaries for a country or more, in Wagtail Projects.
 
 # Overview
```

### Comparing `adm-boundary-manager-0.1.0/README.md` & `adm_boundary_manager-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adm_boundary_manager.egg-info/PKG-INFO` & `adm_boundary_manager-0.2.0/adm_boundary_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adm-boundary-manager
-Version: 0.1.0
+Version: 0.2.0
 Summary: Load, manage and visualize Administrative Boundaries Data in Wagtail
 Home-page: https://github.com/wmo-raf/adm-boundary-manager
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -21,14 +21,15 @@
 Requires-Dist: wagtail>=4.2.2
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: geopandas>=0.12.2
 Requires-Dist: django-filter>=22.1
 Requires-Dist: django-countries>=7.5.1
 Requires-Dist: django-countries-geoextent>=0.0.1
 Requires-Dist: wagtail-cache>=2.3.0
+Requires-Dist: wagtail-modeladmin>=1.0.0
 
 # Administrative Boundaries Manager
 
 Load, manage and visualize administrative boundaries for a country or more, in Wagtail Projects.
 
 # Overview
```

### Comparing `adm-boundary-manager-0.1.0/adm_boundary_manager.egg-info/SOURCES.txt` & `adm_boundary_manager-0.2.0/adm_boundary_manager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,11 @@
 adminboundarymanager/migrations/0001_initial.py
 adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py
 adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py
 adminboundarymanager/migrations/0004_rename_countries_country_and_more.py
 adminboundarymanager/migrations/0005_alter_country_country.py
 adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py
 adminboundarymanager/migrations/__init__.py
+adminboundarymanager/static/adminboundarymanager/css/maplibre-gl.css
+adminboundarymanager/static/adminboundarymanager/js/maplibre-gl.js
 adminboundarymanager/templates/adminboundarymanager/boundary_loader.html
 adminboundarymanager/templates/adminboundarymanager/boundary_preview.html
```

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/errors.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/errors.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/forms.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/forms.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/loaders/__init__.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/loaders/cod_abs_loader.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/loaders/cod_abs_loader.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/loaders/gadm_loader.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/loaders/gadm_loader.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/loaders/generic_loader.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/loaders/generic_loader.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0001_initial.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0002_adminboundarysettings_data_source.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0003_alter_adminboundarysettings_data_source.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0004_rename_countries_country_and_more.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/migrations/0006_remove_adminboundary_size_and_more.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/models.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/models.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/serializers.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/serializers.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html` & `adm_boundary_manager-0.2.0/adminboundarymanager/templates/adminboundarymanager/boundary_loader.html`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html` & `adm_boundary_manager-0.2.0/adminboundarymanager/templates/adminboundarymanager/boundary_preview.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% load i18n %}
 {% load l10n %}
 {% load wagtailadmin_tags wagtailimages_tags static %}
 {% block titletag %}{% blocktrans with title=page.get_admin_display_title %}Admin Boundary Data{{ title }}
 {% endblocktrans %}{% endblock %}
 {% block extra_css %}
     {{ block.super }}
-    <link href="https://unpkg.com/maplibre-gl@3.1.0/dist/maplibre-gl.css" rel="stylesheet"/>
+    <link rel="stylesheet" href="{% static 'adminboundarymanager/css/maplibre-gl.css' %}">
 {% endblock %}
 
 {% block content %}
     {% trans "Administrative Boundaries Data" as header_str %}
 
     {% if countries %}
         {% include "wagtailadmin/shared/header.html" with title=header_str icon="map" action_url=load_boundary_url action_text="Add Boundary" %}
@@ -54,15 +54,15 @@
             {% endif %}
         </div>
     </div>
 {% endblock %}
 
 {% block extra_js %}
     {{ block.super }}
-    <script src="https://unpkg.com/maplibre-gl@3.1.0/dist/maplibre-gl.js"></script>
+    <script src="{% static 'adminboundarymanager/js/maplibre-gl.js' %}"></script>
     <script>
 
         const mapConfig = {{ mapConfig | safe }};
 
         const {combinedBbox, boundaryTilesUrl} = mapConfig
 
         let bounds
```

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/urls.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/urls.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/utils.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/utils.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/views.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/views.py`

 * *Files identical despite different names*

### Comparing `adm-boundary-manager-0.1.0/adminboundarymanager/wagtail_hooks.py` & `adm_boundary_manager-0.2.0/adminboundarymanager/wagtail_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.urls import path, reverse
 from django.utils.translation import gettext_lazy as _
 from wagtail import hooks
 from wagtail.admin.menu import MenuItem
-from wagtail.contrib.modeladmin.options import ModelAdminGroup, ModelAdmin
+from wagtail_modeladmin.options import ModelAdminGroup, ModelAdmin
 
 from .models import AdminBoundarySettings, AdminBoundary
 from .views import load_boundary, preview_boundary
 
 
 @hooks.register('register_admin_urls')
 def urlconf_boundarymanager():
```

### Comparing `adm-boundary-manager-0.1.0/setup.cfg` & `adm_boundary_manager-0.2.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = adm-boundary-manager
-version = 0.1.0
+version = 0.2.0
 description = Load, manage and visualize Administrative Boundaries Data in Wagtail
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/adm-boundary-manager
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
@@ -28,12 +28,13 @@
 	wagtail>=4.2.2
 	shapely>=2.0.1
 	geopandas>=0.12.2
 	django-filter>=22.1
 	django-countries>=7.5.1
 	django-countries-geoextent>=0.0.1
 	wagtail-cache>=2.3.0
+	wagtail-modeladmin>=1.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


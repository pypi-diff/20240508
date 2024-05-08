# Comparing `tmp/nutrical-0.0.4.tar.gz` & `tmp/nutrical-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutrical-0.0.4.tar", last modified: Wed May  8 03:53:42 2024, max compression
+gzip compressed data, was "nutrical-0.0.5.tar", last modified: Wed May  8 05:04:24 2024, max compression
```

## Comparing `nutrical-0.0.4.tar` & `nutrical-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 03:53:42.356691 nutrical-0.0.4/
--rw-rw-rw-   0        0        0    16887 2024-05-08 03:53:42.355281 nutrical-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    12094 2024-05-08 03:50:00.000000 nutrical-0.0.4/README.md
--rw-rw-rw-   0        0        0        2 2024-05-08 03:53:41.000000 nutrical-0.0.4/VERSION
-drwxrwxrwx   0        0        0        0 2024-05-08 03:53:42.349355 nutrical-0.0.4/data/
--rw-rw-rw-   0        0        0     3509 2024-05-02 05:10:03.000000 nutrical-0.0.4/data/TW_FDA_nutrition_items.csv
-drwxrwxrwx   0        0        0        0 2024-05-08 03:53:42.320999 nutrical-0.0.4/nutrical/
--rw-rw-rw-   0        0        0       42 2024-05-03 05:46:07.000000 nutrical-0.0.4/nutrical/__init__.py
--rw-rw-rw-   0        0        0     1499 2024-05-08 03:45:36.000000 nutrical-0.0.4/nutrical/io.py
--rw-rw-rw-   0        0        0     6202 2024-05-08 03:36:52.000000 nutrical-0.0.4/nutrical/nutrical.py
--rw-rw-rw-   0        0        0       95 2024-05-02 07:08:54.000000 nutrical-0.0.4/nutrical/taiwan-fda.py
--rw-rw-rw-   0        0        0     1840 2024-05-05 23:54:15.000000 nutrical-0.0.4/nutrical/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:53:42.340289 nutrical-0.0.4/nutrical.egg-info/
--rw-rw-rw-   0        0        0    16887 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-08 03:53:42.000000 nutrical-0.0.4/nutrical.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 03:53:42.357687 nutrical-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      949 2024-05-03 02:55:53.000000 nutrical-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:04:24.036908 nutrical-0.0.5/
+-rw-rw-rw-   0        0        0    16903 2024-05-08 05:04:24.033184 nutrical-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12110 2024-05-08 03:55:01.000000 nutrical-0.0.5/README.md
+-rw-rw-rw-   0        0        0        2 2024-05-08 05:04:22.000000 nutrical-0.0.5/VERSION
+drwxrwxrwx   0        0        0        0 2024-05-08 05:04:24.028895 nutrical-0.0.5/data/
+-rw-rw-rw-   0        0        0     3509 2024-05-02 05:10:03.000000 nutrical-0.0.5/data/TW_FDA_nutrition_items.csv
+drwxrwxrwx   0        0        0        0 2024-05-08 05:04:23.965688 nutrical-0.0.5/nutrical/
+-rw-rw-rw-   0        0        0       42 2024-05-03 05:46:07.000000 nutrical-0.0.5/nutrical/__init__.py
+-rw-rw-rw-   0        0        0     1499 2024-05-08 03:45:36.000000 nutrical-0.0.5/nutrical/io.py
+-rw-rw-rw-   0        0        0     6202 2024-05-08 03:36:52.000000 nutrical-0.0.5/nutrical/nutrical.py
+-rw-rw-rw-   0        0        0       95 2024-05-02 07:08:54.000000 nutrical-0.0.5/nutrical/taiwan-fda.py
+-rw-rw-rw-   0        0        0     1840 2024-05-05 23:54:15.000000 nutrical-0.0.5/nutrical/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:04:24.019491 nutrical-0.0.5/nutrical.egg-info/
+-rw-rw-rw-   0        0        0    16903 2024-05-08 05:04:23.000000 nutrical-0.0.5/nutrical.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2024-05-08 05:04:23.000000 nutrical-0.0.5/nutrical.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 05:04:23.000000 nutrical-0.0.5/nutrical.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 05:04:23.000000 nutrical-0.0.5/nutrical.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 05:04:23.000000 nutrical-0.0.5/nutrical.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 05:04:24.037873 nutrical-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      949 2024-05-03 02:55:53.000000 nutrical-0.0.5/setup.py
```

### Comparing `nutrical-0.0.4/PKG-INFO` & `nutrical-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nutrical
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nutrition calculation for recipes and ingredients
 Home-page: https://github.com/liao961120/nutrical
 Author: Yongfu Liao
 Author-email: liao961120@gmail.com
 License: UNKNOWN
-Description: Nutrition calculation for recipes and ingredients
-        =================================================
+Description: Nutritional value calculation for recipes and ingredients
+        =========================================================
         
         `nutrical` provides an object-oriented interface for defining and manipulating the nutritional value of ingredients and recipes.
         
         <!-- pandoc test/test.ipynb --to gfm | xclip/pbcopy -->
         <div class="cell markdown">
         
         ## Installation
```

### Comparing `nutrical-0.0.4/README.md` & `nutrical-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Nutrition calculation for recipes and ingredients
-=================================================
+Nutritional value calculation for recipes and ingredients
+=========================================================
 
 `nutrical` provides an object-oriented interface for defining and manipulating the nutritional value of ingredients and recipes.
 
 <!-- pandoc test/test.ipynb --to gfm | xclip/pbcopy -->
 <div class="cell markdown">
 
 ## Installation
```

### Comparing `nutrical-0.0.4/data/TW_FDA_nutrition_items.csv` & `nutrical-0.0.5/data/TW_FDA_nutrition_items.csv`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.4/nutrical/io.py` & `nutrical-0.0.5/nutrical/io.py`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.4/nutrical/nutrical.py` & `nutrical-0.0.5/nutrical/nutrical.py`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.4/nutrical/utils.py` & `nutrical-0.0.5/nutrical/utils.py`

 * *Files identical despite different names*

### Comparing `nutrical-0.0.4/nutrical.egg-info/PKG-INFO` & `nutrical-0.0.5/nutrical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nutrical
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nutrition calculation for recipes and ingredients
 Home-page: https://github.com/liao961120/nutrical
 Author: Yongfu Liao
 Author-email: liao961120@gmail.com
 License: UNKNOWN
-Description: Nutrition calculation for recipes and ingredients
-        =================================================
+Description: Nutritional value calculation for recipes and ingredients
+        =========================================================
         
         `nutrical` provides an object-oriented interface for defining and manipulating the nutritional value of ingredients and recipes.
         
         <!-- pandoc test/test.ipynb --to gfm | xclip/pbcopy -->
         <div class="cell markdown">
         
         ## Installation
```

### Comparing `nutrical-0.0.4/setup.py` & `nutrical-0.0.5/setup.py`

 * *Files identical despite different names*


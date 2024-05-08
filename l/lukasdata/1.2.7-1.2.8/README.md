# Comparing `tmp/lukasdata-1.2.7.tar.gz` & `tmp/lukasdata-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.2.7.tar", last modified: Mon Apr 29 20:09:36 2024, max compression
+gzip compressed data, was "lukasdata-1.2.8.tar", last modified: Wed May  8 19:00:55 2024, max compression
```

## Comparing `lukasdata-1.2.7.tar` & `lukasdata-1.2.8.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 20:09:36.102980 lukasdata-1.2.7/
--rw-rw-rw-   0        0        0      128 2024-04-29 20:09:36.099981 lukasdata-1.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 20:09:36.079991 lukasdata-1.2.7/lukasdata/
--rw-rw-rw-   0        0        0        0 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/__init__.py
--rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/change_directory.py
--rw-rw-rw-   0        0        0      611 2024-04-29 19:54:20.000000 lukasdata-1.2.7/lukasdata/concat_dfs.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/count_nans.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/create_mask.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/dict_to_json.py
--rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.2.7/lukasdata/drop_column_with_na.py
--rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.2.7/lukasdata/get_list_intersection.py
--rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/get_number_columns.py
--rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/json_to_dict.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/list_to_string.py
--rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.2.7/lukasdata/mean_impute.py
--rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.2.7/lukasdata/na_counts.py
--rw-rw-rw-   0        0        0     1182 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/plot_metric_history.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.2.7/lukasdata/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-04-29 20:09:36.097981 lukasdata-1.2.7/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-04-29 20:09:35.000000 lukasdata-1.2.7/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      640 2024-04-29 20:09:36.000000 lukasdata-1.2.7/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 20:09:35.000000 lukasdata-1.2.7/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-29 20:09:35.000000 lukasdata-1.2.7/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-29 20:09:35.000000 lukasdata-1.2.7/lukasdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 20:09:36.103980 lukasdata-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-04-29 20:09:30.000000 lukasdata-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:00:55.129738 lukasdata-1.2.8/
+-rw-rw-rw-   0        0        0      128 2024-05-08 19:00:55.126741 lukasdata-1.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 19:00:55.096759 lukasdata-1.2.8/lukasdata/
+-rw-rw-rw-   0        0        0        0 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.2.8/lukasdata/analyze_datasets.py
+-rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/change_directory.py
+-rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.2.8/lukasdata/check_for_all_zeroes.py
+-rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.2.8/lukasdata/concat_dfs.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/count_nans.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/create_mask.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/dict_to_json.py
+-rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.2.8/lukasdata/drop_column_with_na.py
+-rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.2.8/lukasdata/drop_columns_permutation_score.py
+-rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.2.8/lukasdata/get_list_intersection.py
+-rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/get_number_columns.py
+-rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/json_to_dict.py
+-rw-rw-rw-   0        0        0     1738 2024-05-08 18:59:59.000000 lukasdata-1.2.8/lukasdata/keras_input.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/list_to_string.py
+-rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.2.8/lukasdata/mean_impute.py
+-rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.2.8/lukasdata/na_counts.py
+-rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.2.8/lukasdata/order_dict.py
+-rw-rw-rw-   0        0        0     2400 2024-05-07 10:05:15.000000 lukasdata-1.2.8/lukasdata/permutation_importance.py
+-rw-rw-rw-   0        0        0     1182 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/plot_metric_history.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.2.8/lukasdata/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-05-08 19:00:55.124741 lukasdata-1.2.8/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-08 19:00:54.000000 lukasdata-1.2.8/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      833 2024-05-08 19:00:55.000000 lukasdata-1.2.8/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 19:00:54.000000 lukasdata-1.2.8/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-08 19:00:54.000000 lukasdata-1.2.8/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 19:00:54.000000 lukasdata-1.2.8/lukasdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 19:00:55.130737 lukasdata-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-05-08 19:00:39.000000 lukasdata-1.2.8/setup.py
```

### Comparing `lukasdata-1.2.7/lukasdata/change_directory.py` & `lukasdata-1.2.8/lukasdata/change_directory.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.2.7/lukasdata/plot_metric_history.py` & `lukasdata-1.2.8/lukasdata/plot_metric_history.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.2.7/lukasdata.egg-info/SOURCES.txt` & `lukasdata-1.2.8/lukasdata.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 setup.py
 lukasdata/__init__.py
+lukasdata/analyze_datasets.py
 lukasdata/change_directory.py
+lukasdata/check_for_all_zeroes.py
 lukasdata/concat_dfs.py
 lukasdata/count_nans.py
 lukasdata/create_mask.py
 lukasdata/del_jpg.py
 lukasdata/determine_file_type.py
 lukasdata/dict_to_json.py
 lukasdata/drop_column_with_na.py
+lukasdata/drop_columns_permutation_score.py
 lukasdata/get_list_intersection.py
 lukasdata/get_number_columns.py
 lukasdata/json_to_dict.py
+lukasdata/keras_input.py
 lukasdata/list_to_string.py
 lukasdata/mean_impute.py
 lukasdata/na_counts.py
+lukasdata/order_dict.py
+lukasdata/permutation_importance.py
 lukasdata/plot_metric_history.py
 lukasdata/string_to_text.py
 lukasdata.egg-info/PKG-INFO
 lukasdata.egg-info/SOURCES.txt
 lukasdata.egg-info/dependency_links.txt
 lukasdata.egg-info/requires.txt
 lukasdata.egg-info/top_level.txt
```


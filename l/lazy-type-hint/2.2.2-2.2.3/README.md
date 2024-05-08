# Comparing `tmp/lazy_type_hint-2.2.2.tar.gz` & `tmp/lazy_type_hint-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.2.2.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.2.3.tar", max compression
```

## Comparing `lazy_type_hint-2.2.2.tar` & `lazy_type_hint-2.2.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.2.2/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0    12413 2024-04-29 13:45:53.508452 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     7793 2024-04-29 13:45:53.517325 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0     1279 2024-04-29 13:45:53.522867 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    17314 2024-04-19 13:25:22.433858 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     2963 2024-04-20 12:20:31.948128 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0      803 2024-04-23 15:02:40.562766 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
--rw-r--r--   0        0        0     1144 2024-04-23 15:02:40.563766 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     5922 2024-04-23 15:02:40.570766 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      601 2024-04-19 13:25:22.452857 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     7814 2024-05-01 13:21:10.135455 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0     1779 2024-04-29 13:45:53.534808 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1309 2024-04-20 12:20:31.951328 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6646 2024-04-29 13:45:53.539888 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1988 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2129 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0     1039 2024-04-29 13:45:53.548265 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     3114 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0     1478 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      396 2024-04-23 15:02:40.591280 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
--rw-r--r--   0        0        0      432 2024-04-23 15:02:40.597509 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
--rw-r--r--   0        0        0      511 2024-04-23 15:02:40.606702 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/numpy_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      794 2024-04-23 15:02:40.615914 lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2340 2024-04-29 13:45:49.656127 lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3137 2024-04-29 13:45:49.662517 lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0    10092 2024-04-29 13:45:49.712316 lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.2.2/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     2222 2024-04-23 15:02:15.663344 lazy_type_hint-2.2.2/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      732 2024-04-19 13:25:22.511264 lazy_type_hint-2.2.2/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.2.2/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5900 2024-04-29 13:45:53.555265 lazy_type_hint-2.2.2/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.2.2/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.2/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.2/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3712 2024-04-20 12:20:31.953328 lazy_type_hint-2.2.2/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2625 2024-05-01 13:21:10.136456 lazy_type_hint-2.2.2/pyproject.toml
--rw-r--r--   0        0        0    12338 2024-04-29 13:45:49.641764 lazy_type_hint-2.2.2/README.md
--rw-r--r--   0        0        0    12602 1970-01-01 00:00:00.000000 lazy_type_hint-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.2.3/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0    12413 2024-04-29 13:45:53.508452 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     7793 2024-05-07 20:41:03.159890 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0     1279 2024-04-29 13:45:53.522867 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    17314 2024-04-19 13:25:22.433858 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     2963 2024-04-20 12:20:31.948128 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0      803 2024-04-23 15:02:40.562766 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
+-rw-r--r--   0        0        0     1144 2024-04-23 15:02:40.563766 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     5922 2024-04-23 15:02:40.570766 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      601 2024-04-19 13:25:22.452857 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     7806 2024-05-08 07:23:27.799663 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0     1779 2024-05-07 20:57:24.444184 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1309 2024-04-20 12:20:31.951328 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6646 2024-04-29 13:45:53.539888 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1988 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2129 2024-04-23 15:02:40.576999 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0     1039 2024-04-29 13:45:53.548265 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     3114 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0     1478 2024-04-23 15:02:40.585280 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      396 2024-04-23 15:02:40.591280 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
+-rw-r--r--   0        0        0      432 2024-04-23 15:02:40.597509 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
+-rw-r--r--   0        0        0      511 2024-04-23 15:02:40.606702 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/numpy_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      794 2024-04-23 15:02:40.615914 lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2340 2024-04-29 13:45:49.656127 lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3137 2024-04-29 13:45:49.662517 lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0    10092 2024-04-29 13:45:49.712316 lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.2.3/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     2222 2024-04-23 15:02:15.663344 lazy_type_hint-2.2.3/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      732 2024-04-19 13:25:22.511264 lazy_type_hint-2.2.3/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.2.3/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5900 2024-04-29 13:45:53.555265 lazy_type_hint-2.2.3/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.2.3/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.3/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.2.3/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3712 2024-04-20 12:20:31.953328 lazy_type_hint-2.2.3/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2664 2024-05-08 07:23:27.800664 lazy_type_hint-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0    12338 2024-04-29 13:45:49.641764 lazy_type_hint-2.2.3/README.md
+-rw-r--r--   0        0        0    12602 1970-01-01 00:00:00.000000 lazy_type_hint-2.2.3/PKG-INFO
```

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/factory.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,21 +144,21 @@
         if not self.are_all_columns_literal_compatible:
             return {}
 
         # Corner case to avoid infinite recursion
         if all(isinstance(column, tuple) and len(column) == 1 for column in self.data.columns):
             return {}
 
+        columns_processed: Set[Union[bool, str, int]] = set()
         for column in data.columns:
             if not self.can_be_accessed_multilevel:  # Here all columns will  be Hashable
                 column = cast(Hashable, column)
                 children[column] = self._create_child(column)
             else:  # Here all columns will be tuple
                 multi_column = cast(Tuple[Hashable, ...], column)
-                columns_processed: Set[Union[bool, str, int]] = set()
                 if multi_column[0] not in columns_processed:
                     if isinstance(multi_column[0], self.literal_compatible_types):
                         columns_processed.add(multi_column[0])
                         children[column[0]] = self._create_child(column[0])
         return children
 
     @override
```

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/pandas_series_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/pandas_series_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.2.3/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.2.3/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.2.3/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/strategies.py` & `lazy_type_hint-2.2.3/lazy_type_hint/strategies.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.2.3/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.2.3/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.2.3/lazy_type_hint/utils/import_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.2.3/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.2.3/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.2.3/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.2.3/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/pyproject.toml` & `lazy_type_hint-2.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.2.2"
+version = "2.2.3"
 description = "Automate type hint generation in a single line."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
 
@@ -69,13 +69,14 @@
 
 [tool.codespell]
 ignore-words-list = "bu"  # Comma separated
 
 [tool.pytest.ini_options]
 markers = "integration"
 # addopts = "-vv"
+# addopts = ["-m", "not integration"]
 # addopts = ["-n", "auto", "-m", "not integration"]
 addopts = ["-n", "auto"]  # All tests
 testpaths = ["tests"]
 
 # Commands:
 # poetry run pytest --benchmark-only
```

### Comparing `lazy_type_hint-2.2.2/README.md` & `lazy_type_hint-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.2.2/PKG-INFO` & `lazy_type_hint-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 2.2.2
+Version: 2.2.3
 Summary: Automate type hint generation in a single line.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


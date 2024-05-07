# Comparing `tmp/freeze_dried_data-2.1.2.tar.gz` & `tmp/freeze_dried_data-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-2.1.2.tar", last modified: Mon May  6 18:07:31 2024, max compression
+gzip compressed data, was "freeze_dried_data-2.1.3.tar", last modified: Tue May  7 17:38:05 2024, max compression
```

## Comparing `freeze_dried_data-2.1.2.tar` & `freeze_dried_data-2.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 18:07:31.659799 freeze_dried_data-2.1.2/
--rw-r--r--   0 root         (0) root         (0)     1072 2024-05-06 18:05:58.000000 freeze_dried_data-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11553 2024-05-06 18:07:31.659799 freeze_dried_data-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10686 2024-05-06 18:05:58.000000 freeze_dried_data-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 18:07:31.659799 freeze_dried_data-2.1.2/freeze_dried_data/
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-06 18:05:58.000000 freeze_dried_data-2.1.2/freeze_dried_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30134 2024-05-06 18:05:58.000000 freeze_dried_data-2.1.2/freeze_dried_data/freeze_dried_data.py
--rw-r--r--   0 root         (0) root         (0)    11613 2024-05-06 18:05:58.000000 freeze_dried_data-2.1.2/freeze_dried_data/freeze_dried_data_old.py
--rw-r--r--   0 root         (0) root         (0)    40064 2024-05-06 18:05:58.000000 freeze_dried_data-2.1.2/freeze_dried_data/test_freeze_dried_data.py
--rw-r--r--   0 root         (0) root         (0)     7982 2024-05-06 18:05:58.000000 freeze_dried_data-2.1.2/freeze_dried_data/test_freeze_dried_data_old.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 18:07:31.659799 freeze_dried_data-2.1.2/freeze_dried_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11553 2024-05-06 18:07:31.000000 freeze_dried_data-2.1.2/freeze_dried_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-06 18:07:31.000000 freeze_dried_data-2.1.2/freeze_dried_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 18:07:31.000000 freeze_dried_data-2.1.2/freeze_dried_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-06 18:07:31.000000 freeze_dried_data-2.1.2/freeze_dried_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 18:07:31.659799 freeze_dried_data-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-06 18:05:58.000000 freeze_dried_data-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:38:05.652715 freeze_dried_data-2.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1072 2024-05-07 17:22:15.000000 freeze_dried_data-2.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11553 2024-05-07 17:38:05.652715 freeze_dried_data-2.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    10686 2024-05-07 17:22:15.000000 freeze_dried_data-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:38:05.652715 freeze_dried_data-2.1.3/freeze_dried_data/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-05-07 17:22:15.000000 freeze_dried_data-2.1.3/freeze_dried_data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    30657 2024-05-07 17:31:41.000000 freeze_dried_data-2.1.3/freeze_dried_data/freeze_dried_data.py
+-rwxrwxrwx   0 root         (0) root         (0)    11613 2024-05-07 17:22:15.000000 freeze_dried_data-2.1.3/freeze_dried_data/freeze_dried_data_old.py
+-rwxrwxrwx   0 root         (0) root         (0)    40245 2024-05-07 17:31:40.000000 freeze_dried_data-2.1.3/freeze_dried_data/test_freeze_dried_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     7982 2024-05-07 17:22:15.000000 freeze_dried_data-2.1.3/freeze_dried_data/test_freeze_dried_data_old.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:38:05.652715 freeze_dried_data-2.1.3/freeze_dried_data.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11553 2024-05-07 17:38:05.000000 freeze_dried_data-2.1.3/freeze_dried_data.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-07 17:38:05.000000 freeze_dried_data-2.1.3/freeze_dried_data.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 17:38:05.000000 freeze_dried_data-2.1.3/freeze_dried_data.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-07 17:38:05.000000 freeze_dried_data-2.1.3/freeze_dried_data.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 17:38:05.652715 freeze_dried_data-2.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1125 2024-05-07 17:37:15.000000 freeze_dried_data-2.1.3/setup.py
```

### Comparing `freeze_dried_data-2.1.2/LICENSE` & `freeze_dried_data-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.2/PKG-INFO` & `freeze_dried_data-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze_dried_data
-Version: 2.1.2
+Version: 2.1.3
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.1.2/README.md` & `freeze_dried_data-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.2/freeze_dried_data/freeze_dried_data.py` & `freeze_dried_data-2.1.3/freeze_dried_data/freeze_dried_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,28 @@
         """
         Gets the row with the specified key.
 
         :param key: The key of the row.
         :return: The row with the specified key. 
         :raises KeyError: If the key is not found.
         """
-
+        
         if key not in self.index:
-            raise KeyError("Key not found.", key)
+            if isinstance(key, tuple):
+                if key in self.index:
+                    return self[key]
+                else:
+                    if key[0] in self.index:
+                        indices = self.index[key[0]]
+                        col_index = self.columns[key[1]]
+                        start, end = indices[col_index:col_index+2]
+                        data = self.read_chunk(start, end)
+                        return self.column_to_deserialize[col_index](data)
+            else:
+                raise KeyError("Key not found.", key)
         
         if self.columns is None:
             
             start, end = self.index[key]
             data = self.read_chunk(start, end)
 
             return self.no_columns_deserialize(data)
```

### Comparing `freeze_dried_data-2.1.2/freeze_dried_data/freeze_dried_data_old.py` & `freeze_dried_data-2.1.3/freeze_dried_data/freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.2/freeze_dried_data/test_freeze_dried_data.py` & `freeze_dried_data-2.1.3/freeze_dried_data/test_freeze_dried_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,17 @@
             self.assertEqual(rfdd['house1'][2], 100000)
             self.assertEqual(rfdd['house2'][0], 'house2')
             self.assertEqual(rfdd['house2'][1], 200)
             self.assertEqual(rfdd['house2'][2], 200000)
             self.assertEqual(rfdd['house3'][0], 'house3')
             self.assertEqual(rfdd['house3'][1], 300)
             self.assertEqual(rfdd['house3'][2], 300000)
+            self.assertEqual(rfdd['house1','name'], 'house1')
+            self.assertEqual(rfdd['house1','area'], 100)
+            self.assertEqual(rfdd['house1','price'], 100000)
 
 
             for k,v in rfdd.items():
                 print(k)
                 print(v)
 
             # prints:
@@ -96,14 +99,15 @@
             # price: 200000
             #
             # house3
             # name: house3
             # area: 300
             # price: 300000
 
+
     def test_file_exists(self):
         with WFDD(self.test_file, overwrite=True) as wfdd:
             wfdd['hello'] = 'world'
             wfdd['number'] = 123
             
 
         with self.assertRaises(FileExistsError):
```

### Comparing `freeze_dried_data-2.1.2/freeze_dried_data/test_freeze_dried_data_old.py` & `freeze_dried_data-2.1.3/freeze_dried_data/test_freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.2/freeze_dried_data.egg-info/PKG-INFO` & `freeze_dried_data-2.1.3/freeze_dried_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze-dried-data
-Version: 2.1.2
+Version: 2.1.3
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.1.2/setup.py` & `freeze_dried_data-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='freeze_dried_data',
-    version='2.1.2',
+    version='2.1.3',
     description='A simple format for machine learning datasets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/tstandley/freeze_dried_data',
     author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
```


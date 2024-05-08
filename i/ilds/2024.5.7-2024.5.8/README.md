# Comparing `tmp/ilds-2024.5.7.tar.gz` & `tmp/ilds-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ilds-2024.5.7.tar", last modified: Tue May  7 09:52:41 2024, max compression
+gzip compressed data, was "dist\ilds-2024.5.8.tar", last modified: Wed May  8 02:02:04 2024, max compression
```

## Comparing `ilds-2024.5.7.tar` & `ilds-2024.5.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:52:41.000000 ilds-2024.5.7/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:52:40.000000 ilds-2024.5.7/ilds/
--rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2024.5.7/ilds/cmd.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:52:40.000000 ilds-2024.5.7/ilds/django/
--rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2024.5.7/ilds/django/admin.py
--rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2024.5.7/ilds/django/import_export.py
--rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2024.5.7/ilds/django/model.py
--rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2024.5.7/ilds/django/user.py
--rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2024.5.7/ilds/django/util.py
--rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2024.5.7/ilds/django/__init__.py
--rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2024.5.7/ilds/everything.py
--rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2024.5.7/ilds/excel_xlrd.py
--rw-rw-rw-   0        0        0     9462 2023-05-16 08:14:48.000000 ilds-2024.5.7/ilds/excel_xlsx.py
--rw-rw-rw-   0        0        0    27737 2024-01-16 03:04:03.000000 ilds-2024.5.7/ilds/file.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:52:40.000000 ilds-2024.5.7/ilds/lib/
--rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2024.5.7/ilds/lib/browsercookie.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:52:41.000000 ilds-2024.5.7/ilds/lib/configobj/
--rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2024.5.7/ilds/lib/configobj/validate.py
--rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2024.5.7/ilds/lib/configobj/_version.py
--rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2024.5.7/ilds/lib/configobj/__init__.py
--rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2024.5.7/ilds/lib/hexdump.py
--rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2024.5.7/ilds/lib/__init__.py
--rw-rw-rw-   0        0        0    18063 2024-03-01 06:06:21.000000 ilds-2024.5.7/ilds/match_data.py
--rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2024.5.7/ilds/md.py
--rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2024.5.7/ilds/md5summer.py
--rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2024.5.7/ilds/mycsv.py
--rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2024.5.7/ilds/net.py
--rw-rw-rw-   0        0        0     9879 2024-05-07 09:51:51.000000 ilds-2024.5.7/ilds/pd.py
--rw-rw-rw-   0        0        0     8238 2024-01-18 09:17:32.000000 ilds-2024.5.7/ilds/spider.py
--rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2024.5.7/ilds/time.py
--rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2024.5.7/ilds/util.py
--rw-rw-rw-   0        0        0      422 2024-05-07 09:51:51.000000 ilds-2024.5.7/ilds/versions.py
--rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2024.5.7/ilds/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:52:40.000000 ilds-2024.5.7/ilds.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-07 09:52:39.000000 ilds-2024.5.7/ilds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1316 2024-05-07 09:52:39.000000 ilds-2024.5.7/ilds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       82 2024-05-07 09:52:39.000000 ilds-2024.5.7/ilds.egg-info/requires.txt
--rw-rw-rw-   0        0        0      695 2024-05-07 09:52:39.000000 ilds-2024.5.7/ilds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2024-05-07 09:52:39.000000 ilds-2024.5.7/ilds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1316 2024-05-07 09:52:41.000000 ilds-2024.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2024.5.7/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-07 09:52:41.000000 ilds-2024.5.7/setup.cfg
--rw-rw-rw-   0        0        0     6481 2024-01-16 03:08:05.000000 ilds-2024.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:02:04.000000 ilds-2024.5.8/
+drwxrwxrwx   0        0        0        0 2024-05-08 02:02:04.000000 ilds-2024.5.8/ilds/
+-rw-rw-rw-   0        0        0     1797 2021-09-26 05:21:21.000000 ilds-2024.5.8/ilds/cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:02:04.000000 ilds-2024.5.8/ilds/django/
+-rw-rw-rw-   0        0        0     3407 2019-10-30 05:10:14.000000 ilds-2024.5.8/ilds/django/admin.py
+-rw-rw-rw-   0        0        0    14906 2019-10-30 03:18:15.000000 ilds-2024.5.8/ilds/django/import_export.py
+-rw-rw-rw-   0        0        0    15417 2019-11-27 09:35:07.000000 ilds-2024.5.8/ilds/django/model.py
+-rw-rw-rw-   0        0        0     1840 2019-04-12 05:15:43.000000 ilds-2024.5.8/ilds/django/user.py
+-rw-rw-rw-   0        0        0     2085 2021-09-28 08:04:39.000000 ilds-2024.5.8/ilds/django/util.py
+-rw-rw-rw-   0        0        0        0 2018-08-07 03:24:52.000000 ilds-2024.5.8/ilds/django/__init__.py
+-rw-rw-rw-   0        0        0     9150 2021-12-06 10:18:15.000000 ilds-2024.5.8/ilds/everything.py
+-rw-rw-rw-   0        0        0     9470 2019-03-29 08:26:49.000000 ilds-2024.5.8/ilds/excel_xlrd.py
+-rw-rw-rw-   0        0        0     9462 2023-05-16 08:14:48.000000 ilds-2024.5.8/ilds/excel_xlsx.py
+-rw-rw-rw-   0        0        0    27737 2024-01-16 03:04:03.000000 ilds-2024.5.8/ilds/file.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:02:04.000000 ilds-2024.5.8/ilds/lib/
+-rw-rw-rw-   0        0        0    13740 2018-11-26 09:16:44.000000 ilds-2024.5.8/ilds/lib/browsercookie.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:02:04.000000 ilds-2024.5.8/ilds/lib/configobj/
+-rw-rw-rw-   0        0        0    46989 2019-05-06 20:45:36.000000 ilds-2024.5.8/ilds/lib/configobj/validate.py
+-rw-rw-rw-   0        0        0       44 2019-05-06 20:45:36.000000 ilds-2024.5.8/ilds/lib/configobj/_version.py
+-rw-rw-rw-   0        0        0    88030 2019-05-06 20:45:36.000000 ilds-2024.5.8/ilds/lib/configobj/__init__.py
+-rw-rw-rw-   0        0        0    13829 2018-10-24 05:15:43.000000 ilds-2024.5.8/ilds/lib/hexdump.py
+-rw-rw-rw-   0        0        0        0 2018-10-24 05:29:38.000000 ilds-2024.5.8/ilds/lib/__init__.py
+-rw-rw-rw-   0        0        0    18063 2024-03-01 06:06:21.000000 ilds-2024.5.8/ilds/match_data.py
+-rw-rw-rw-   0        0        0     7121 2019-11-18 03:49:54.000000 ilds-2024.5.8/ilds/md.py
+-rw-rw-rw-   0        0        0     4832 2022-09-07 09:59:12.000000 ilds-2024.5.8/ilds/md5summer.py
+-rw-rw-rw-   0        0        0     3513 2019-10-11 11:13:36.000000 ilds-2024.5.8/ilds/mycsv.py
+-rw-rw-rw-   0        0        0     5123 2022-12-12 02:45:33.000000 ilds-2024.5.8/ilds/net.py
+-rw-rw-rw-   0        0        0    10237 2024-05-08 01:54:08.000000 ilds-2024.5.8/ilds/pd.py
+-rw-rw-rw-   0        0        0     8238 2024-01-18 09:17:32.000000 ilds-2024.5.8/ilds/spider.py
+-rw-rw-rw-   0        0        0    13238 2021-03-05 07:49:55.000000 ilds-2024.5.8/ilds/time.py
+-rw-rw-rw-   0        0        0     7637 2022-10-08 10:21:44.000000 ilds-2024.5.8/ilds/util.py
+-rw-rw-rw-   0        0        0      422 2024-05-08 02:01:07.000000 ilds-2024.5.8/ilds/versions.py
+-rw-rw-rw-   0        0        0        0 2018-07-04 06:42:08.000000 ilds-2024.5.8/ilds/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:02:04.000000 ilds-2024.5.8/ilds.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-08 02:02:03.000000 ilds-2024.5.8/ilds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1316 2024-05-08 02:02:03.000000 ilds-2024.5.8/ilds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       82 2024-05-08 02:02:03.000000 ilds-2024.5.8/ilds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      695 2024-05-08 02:02:03.000000 ilds-2024.5.8/ilds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        5 2024-05-08 02:02:03.000000 ilds-2024.5.8/ilds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1316 2024-05-08 02:02:04.000000 ilds-2024.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2019-10-24 10:28:45.000000 ilds-2024.5.8/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-08 02:02:04.000000 ilds-2024.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     6481 2024-01-16 03:08:05.000000 ilds-2024.5.8/setup.py
```

### Comparing `ilds-2024.5.7/ilds/cmd.py` & `ilds-2024.5.8/ilds/cmd.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/django/admin.py` & `ilds-2024.5.8/ilds/django/admin.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/django/import_export.py` & `ilds-2024.5.8/ilds/django/import_export.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/django/model.py` & `ilds-2024.5.8/ilds/django/model.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/django/user.py` & `ilds-2024.5.8/ilds/django/user.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/django/util.py` & `ilds-2024.5.8/ilds/django/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/everything.py` & `ilds-2024.5.8/ilds/everything.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/excel_xlrd.py` & `ilds-2024.5.8/ilds/excel_xlrd.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/excel_xlsx.py` & `ilds-2024.5.8/ilds/excel_xlsx.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/file.py` & `ilds-2024.5.8/ilds/file.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/lib/browsercookie.py` & `ilds-2024.5.8/ilds/lib/browsercookie.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/lib/configobj/validate.py` & `ilds-2024.5.8/ilds/lib/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/lib/configobj/__init__.py` & `ilds-2024.5.8/ilds/lib/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/lib/hexdump.py` & `ilds-2024.5.8/ilds/lib/hexdump.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/match_data.py` & `ilds-2024.5.8/ilds/match_data.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/md.py` & `ilds-2024.5.8/ilds/md.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/md5summer.py` & `ilds-2024.5.8/ilds/md5summer.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/mycsv.py` & `ilds-2024.5.8/ilds/mycsv.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/net.py` & `ilds-2024.5.8/ilds/net.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/pd.py` & `ilds-2024.5.8/ilds/pd.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,21 +41,15 @@
     with pd.ExcelFile(file) as excel:
         if sheet_names is None:
             sheet_names = excel.sheet_names
         else:
             # 确保Excel文件中提供的 sheet_names 存在
             invalid_sheets = set(sheet_names) - set(excel.sheet_names)
             if invalid_sheets:
-                raise ValueError(f"Excel 文件中不存在以下标题：{invalid_sheets}")
-
-            # 当严格模式开启时，检查是否有额外的表薄名称在文件中
-            if strict_mode:
-                extra_sheets = set(excel.sheet_names) - set(sheet_names)
-                if extra_sheets:
-                    raise ValueError(f"Excel 文件中包含了未在“{sheet_names}”中的额外标题：{extra_sheets}")
+                raise ValueError(f"Excel 文件中不存在以下表格：{invalid_sheets}")
 
         if is_print:
             print('表薄名称列表：', sheet_names)
         # 通过表薄名字读取表单
         # data['总表'] = pd.read_excel(excel, sheet_name='总表')
         # 读取全部表
         for sheet_name in sheet_names:
@@ -65,15 +59,27 @@
                 print('表薄名称：', sheet_name, '\t', '行数：', len(_df), '\t', '文件：', file)
             # if 'Metadatas' != sheet_name:
             #     print('跳过内容', sheet_name)
             #     continue
             if add_source_column:
                 _df['本行来自'] = f"{os.path.split(file)[1]} - {sheet_name}"
             # 是否指定要合并的列
+            # 严格模式下检查工作表列是否与concat_columns完全匹配
             if concat_columns is not None:
+                # 检查指定列是否都在DataFrame中
+                missing_columns = set(concat_columns) - set(_df.columns)
+                if missing_columns:
+                    raise ValueError(f"工作表 '{sheet_name}' 中缺少以下指定列：{missing_columns}")
+
+                # 严格模式：检查是否有额外的列
+                if strict_mode:
+                    extra_columns = set(_df.columns) - set(concat_columns)
+                    if extra_columns:
+                        raise ValueError(f"工作表 '{sheet_name}' 包含未在指定标题中声明的额外列：{extra_columns}")
+
                 _df = _df[concat_columns]
             df_list.append(_df)
     return df_list
 
 
 def get_excel_data(file, columns=None, add_source_column=True, only_read_first_table=False, read_sheet_state=False,
                    is_print=True):
```

### Comparing `ilds-2024.5.7/ilds/spider.py` & `ilds-2024.5.8/ilds/spider.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/time.py` & `ilds-2024.5.8/ilds/time.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds/util.py` & `ilds-2024.5.8/ilds/util.py`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/ilds.egg-info/PKG-INFO` & `ilds-2024.5.8/ilds.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2024.5.7
+Version: 2024.5.8
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2024.5.7/ilds.egg-info/SOURCES.txt` & `ilds-2024.5.8/ilds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ilds-2024.5.7/PKG-INFO` & `ilds-2024.5.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ilds
-Version: 2024.5.7
+Version: 2024.5.8
 Summary: 常用模块的集合，为了多平台，多电脑调用方便!
 Home-page: https://github.com/ldsxp/ilds
 Author: lds
 Author-email: 85176878@qq.com
 License: GNU GPL 3
 Download-URL: https://pypi.org/project/ilds
 Description: ====================
```

### Comparing `ilds-2024.5.7/setup.py` & `ilds-2024.5.8/setup.py`

 * *Files identical despite different names*


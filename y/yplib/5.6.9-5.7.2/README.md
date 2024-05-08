# Comparing `tmp/yplib-5.6.9.tar.gz` & `tmp/yplib-5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.6.9.tar", last modified: Tue May  7 07:15:19 2024, max compression
+gzip compressed data, was "yplib-5.7.2.tar", last modified: Wed May  8 06:56:19 2024, max compression
```

## Comparing `yplib-5.6.9.tar` & `yplib-5.7.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 07:15:19.862524 yplib-5.6.9/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.6.9/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-07 07:15:19.862524 yplib-5.6.9/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 07:15:19.862524 yplib-5.6.9/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-07 07:15:13.000000 yplib-5.6.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:15:19.847524 yplib-5.6.9/yplib/
--rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.6.9/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.9/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.9/yplib/chart_html.py
--rw-rw-rw-   0        0        0    11759 2024-05-07 07:03:32.000000 yplib-5.6.9/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.9/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.9/yplib/http_util.py
--rw-rw-rw-   0        0        0    41365 2024-05-07 07:14:26.000000 yplib-5.6.9/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.9/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.9/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.9/yplib/markdown.py
--rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.6.9/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.9/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-07 07:15:19.862524 yplib-5.6.9/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-07 07:15:19.000000 yplib-5.6.9/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-07 07:15:19.000000 yplib-5.6.9/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 07:15:19.000000 yplib-5.6.9/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-07 07:15:19.000000 yplib-5.6.9/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 06:56:19.150186 yplib-5.7.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.7.2/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-08 06:56:19.150186 yplib-5.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.7.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:56:19.150186 yplib-5.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-08 06:56:00.000000 yplib-5.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:56:19.135190 yplib-5.7.2/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.7.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.7.2/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.7.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    12004 2024-05-08 06:55:43.000000 yplib-5.7.2/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.7.2/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.7.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.7.2/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.7.2/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.7.2/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.7.2/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-07 06:14:17.000000 yplib-5.7.2/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.7.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-08 06:56:19.150186 yplib-5.7.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-08 06:56:18.000000 yplib-5.7.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-08 06:56:18.000000 yplib-5.7.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 06:56:18.000000 yplib-5.7.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 06:56:18.000000 yplib-5.7.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.6.9/LICENSE` & `yplib-5.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.6.9/setup.py` & `yplib-5.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.6.9",
+    version="5.7.2",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.6.9/yplib/__init__.py` & `yplib-5.7.2/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.9/yplib/chart.py` & `yplib-5.7.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.9/yplib/chart_html.py` & `yplib-5.7.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.9/yplib/db.py` & `yplib-5.7.2/yplib/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 
 from yplib.index import *
 from yplib.http_util import *
 import pymysql
 import adbc_driver_manager
 import adbc_driver_flightsql.dbapi as flight_sql
+import warnings
+
+warnings.filterwarnings("ignore", message="Cannot disable autocommit", category=Warning)
 
 
 # 有关数据库操作的类
 def get_connect(database=None, user=None, password=None, charset='utf8mb4', port=3306, host=None):
     return pymysql.connect(database=database, user=user, password=password, charset=charset, port=port, host=host)
 
 
@@ -38,34 +41,37 @@
             db_cursor.execute(s)
     else:
         if is_log:
             to_log_file(sql)
         db_cursor.execute(str(sql))
     if commit:
         db_conn.commit()
+    db_cursor.close()
+    db_conn.close()
 
 
 def get_doris_conn(db_config='doris'):
     config_db = get_config_data(db_config)
     my_uri = config_db['uri']
     my_db_kwargs = {
         adbc_driver_manager.DatabaseOptions.USERNAME.value: config_db['username'],
         adbc_driver_manager.DatabaseOptions.PASSWORD.value: config_db['password'],
     }
     conn = flight_sql.connect(uri=my_uri, db_kwargs=my_db_kwargs)
     return conn
 
 
 # 执行 sql 语句, 并且提交, 默认值提交的了
-def exec_doris_sql(sql='', db_config='doris'):
-    conn = get_doris_conn(db_config)
-    cursor = conn.cursor()
-    cursor.execute(sql)
-    cursor.close()
-    conn.close()
+def exec_doris_sql(sql='', db_config='wh_doris', database='mx_risk'):
+    exec_sql(sql, db_config=db_config, database=database)
+    # conn = get_doris_conn(db_config)
+    # cursor = conn.cursor()
+    # cursor.execute(sql)
+    # cursor.close()
+    # conn.close()
 
 
 def get_data_from_doris(sql='', db_config='doris'):
     conn = get_doris_conn(db_config)
     cursor = conn.cursor()
     cursor.execute(sql)
     arrow_data = cursor.fetchallarrow()
```

### Comparing `yplib-5.6.9/yplib/file.py` & `yplib-5.7.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.9/yplib/http_util.py` & `yplib-5.7.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.9/yplib/index.py` & `yplib-5.7.2/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,14 +378,16 @@
         file_name = get_file_name(file_name, suffix, is_date=file_name_is_date)
     # 文件路径
     file_name_path = file_name
     if file_path != '':
         file_name_path = file_path + '/' + file_name
     # 写入文件
     text_file = open(file_name_path, 'a', encoding='utf-8')
+    if isinstance(data_list, set):
+        data_list = list(data_list)
     if not isinstance(data_list, list):
         text_file.write(to_str(data_list) + '\n')
     else:
         for one in data_list:
             if (isinstance(one, list) or isinstance(one, tuple) or isinstance(one, set)) and sep_list is not None:
                 text_file.write(str(sep_list).join(list(map(lambda x: to_str(x), one))) + '\n')
             else:
```

### Comparing `yplib-5.6.9/yplib/mail.py` & `yplib-5.7.2/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.9/yplib/mail_html.py` & `yplib-5.7.2/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.9/yplib/markdown.py` & `yplib-5.7.2/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.9/yplib/multi_thread.py` & `yplib-5.7.2/yplib/multi_thread.py`

 * *Files identical despite different names*


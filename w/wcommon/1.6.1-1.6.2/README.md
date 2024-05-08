# Comparing `tmp/wcommon-1.6.1.tar.gz` & `tmp/wcommon-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcommon-1.6.1.tar", last modified: Sun Apr 28 09:52:12 2024, max compression
+gzip compressed data, was "wcommon-1.6.2.tar", last modified: Wed May  8 09:31:56 2024, max compression
```

## Comparing `wcommon-1.6.1.tar` & `wcommon-1.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-04-28 09:52:12.283061 wcommon-1.6.1/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1776 2024-04-28 09:52:12.281528 wcommon-1.6.1/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1382 2024-04-28 09:51:36.000000 wcommon-1.6.1/README.md
--rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2024-04-28 09:52:12.283478 wcommon-1.6.1/setup.cfg
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2024-01-26 07:38:05.000000 wcommon-1.6.1/setup.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-04-28 09:52:12.268898 wcommon-1.6.1/wcommon/
--rw-r--r--   0 wangjunbo   (502) staff       (20)    31043 2024-01-26 07:37:04.000000 wcommon-1.6.1/wcommon/__init__.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-04-28 09:52:12.279104 wcommon-1.6.1/wcommon.egg-info/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1776 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/SOURCES.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/dependency_links.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/requires.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2024-04-28 09:52:11.000000 wcommon-1.6.1/wcommon.egg-info/top_level.txt
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-05-08 09:31:56.518342 wcommon-1.6.2/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1701 2024-05-08 09:31:56.517930 wcommon-1.6.2/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1307 2024-04-28 09:53:34.000000 wcommon-1.6.2/README.md
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2024-05-08 09:31:56.518502 wcommon-1.6.2/setup.cfg
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2024-05-08 09:30:29.000000 wcommon-1.6.2/setup.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-05-08 09:31:56.514907 wcommon-1.6.2/wcommon/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)    31270 2024-05-08 09:29:58.000000 wcommon-1.6.2/wcommon/__init__.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2024-05-08 09:31:56.517305 wcommon-1.6.2/wcommon.egg-info/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1701 2024-05-08 09:31:56.000000 wcommon-1.6.2/wcommon.egg-info/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2024-05-08 09:31:56.000000 wcommon-1.6.2/wcommon.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2024-05-08 09:31:56.000000 wcommon-1.6.2/wcommon.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2024-05-08 09:31:56.000000 wcommon-1.6.2/wcommon.egg-info/requires.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2024-05-08 09:31:56.000000 wcommon-1.6.2/wcommon.egg-info/top_level.txt
```

### Comparing `wcommon-1.6.1/PKG-INFO` & `wcommon-1.6.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.6.1
+Version: 1.6.2
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -72,13 +72,11 @@
 ```python
 # bulk_insert
 mysql.bulk_insert2("test.person",[{"name":"ma2","age":40},{"name":"liyanhong2","age":39},{"name":"ren"}] )
 ```
 
 
 ## Feature
-### 1.3.5
-Mysql insert语句执行的时候，忽略值为None的字段。
 
 ### 1.3.8
 可以通过check_requirement方法检测依赖包是否已经安装，如果没有安装，则提示安装。
```

### Comparing `wcommon-1.6.1/README.md` & `wcommon-1.6.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -58,12 +58,10 @@
 ```python
 # bulk_insert
 mysql.bulk_insert2("test.person",[{"name":"ma2","age":40},{"name":"liyanhong2","age":39},{"name":"ren"}] )
 ```
 
 
 ## Feature
-### 1.3.5
-Mysql insert语句执行的时候，忽略值为None的字段。
 
 ### 1.3.8
 可以通过check_requirement方法检测依赖包是否已经安装，如果没有安装，则提示安装。
```

### Comparing `wcommon-1.6.1/setup.py` & `wcommon-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     # 项目的名称 一般在同级目录中有个同名的文件夹
     name="wcommon",
     # 项目的版本
-    version="1.6.1",
+    version="1.6.2",
     # 项目的作者
     author="WangJunbo",
     # 作者的邮箱
     author_email="wjbhnu@gmail.com",
     # 项目描述
     description="常用工具类方法集合",
     # 项目的长描述
```

### Comparing `wcommon-1.6.1/wcommon/__init__.py` & `wcommon-1.6.2/wcommon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -520,40 +520,41 @@
 
 
 # reconnecting mysql , 参考 https://www.kingname.info/2017/04/17/decorate-for-method/
 def pingmysql(original_function):
     def wrapper(self, *args, **kwargs):
         try:
             self.database.ping()
-            if self.columns_dict is None:
+            if self.columns_dict is None or timetool.time() - self.meta_update_time > 300:
                 cursor = self.database.cursor()
                 self.columns_dict = {}
                 sql = "select TABLE_SCHEMA,TABLE_NAME,COLUMN_NAME,DATA_TYPE from information_schema.columns where 1 =1 and TABLE_SCHEMA not in ('information_schema','performance_schema','mysql','sys') "
                 cursor.execute(sql)
                 for row in cursor:
                     table_schema = row.get("TABLE_SCHEMA")
                     table_name = row.get("TABLE_NAME")
                     column_name = row.get("COLUMN_NAME")
                     k = '{}.{}.{}'.format(table_schema, table_name, column_name)
                     self.columns_dict[k] = row
+                self.meta_update_time = timetool.time()
             result = original_function(self, *args, **kwargs)
             return result
         except Exception as e:
             traceback.print_exc()
             return 'an Exception raised.'
-
     return wrapper
 
 
 class Mysql():
 
     def __init__(self, configuraion_file=configuration_file, section="mysql"):
         self.default_database_name = ''
         self.database = None
         self.columns_dict = None
+        self.meta_update_time = 0 #self.columns_dict数据的更新时间，self.columns_dict 每5分钟左右更新一次
         try:
             config = configparser.ConfigParser()
             config.read(configuraion_file)
             host = config.get(section, "host")
             port = int(config.get(section, "port"))
             user = config.get(section, "user")
             password = config.get(section, "passwd")
```

### Comparing `wcommon-1.6.1/wcommon.egg-info/PKG-INFO` & `wcommon-1.6.2/wcommon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.6.1
+Version: 1.6.2
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -72,13 +72,11 @@
 ```python
 # bulk_insert
 mysql.bulk_insert2("test.person",[{"name":"ma2","age":40},{"name":"liyanhong2","age":39},{"name":"ren"}] )
 ```
 
 
 ## Feature
-### 1.3.5
-Mysql insert语句执行的时候，忽略值为None的字段。
 
 ### 1.3.8
 可以通过check_requirement方法检测依赖包是否已经安装，如果没有安装，则提示安装。
```


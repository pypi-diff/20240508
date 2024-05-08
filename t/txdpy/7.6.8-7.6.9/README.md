# Comparing `tmp/txdpy-7.6.8.tar.gz` & `tmp/txdpy-7.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-hgmkh_o3\txdpy-7.6.8.tar", last modified: Tue Apr 30 09:31:44 2024, max compression
+gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-w8i3yfpv\txdpy-7.6.9.tar", last modified: Tue May  7 06:59:05 2024, max compression
```

## Comparing `txdpy-7.6.8.tar` & `txdpy-7.6.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 09:31:44.000000 txdpy-7.6.8/
--rw-rw-rw-   0        0        0       71 2024-04-30 09:31:44.000000 txdpy-7.6.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-30 09:31:44.000000 txdpy-7.6.8/setup.cfg
--rw-rw-rw-   0        0        0      371 2024-04-30 09:29:46.000000 txdpy-7.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy/
--rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/URLjoin.py
--rw-rw-rw-   0        0        0     2851 2024-04-29 03:32:28.000000 txdpy-7.6.8/txdpy/__init__.py
--rw-rw-rw-   0        0        0    28068 2024-04-30 09:29:05.000000 txdpy-7.6.8/txdpy/bk_179.py
--rw-rw-rw-   0        0        0     3855 2024-04-30 03:54:19.000000 txdpy-7.6.8/txdpy/easyreq.py
--rw-rw-rw-   0        0        0     3247 2024-04-03 01:19:42.000000 txdpy-7.6.8/txdpy/excel_easy.py
--rw-rw-rw-   0        0        0     2472 2024-04-10 04:32:34.000000 txdpy-7.6.8/txdpy/get_key.py
--rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/list_processing.py
--rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/lookup.py
--rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.6.8/txdpy/progress_display.py
--rw-rw-rw-   0        0        0     6469 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/pytmysql.py
--rw-rw-rw-   0        0        0    11855 2024-04-07 07:33:20.000000 txdpy-7.6.8/txdpy/read_data.py
--rw-rw-rw-   0        0        0     3049 2024-04-16 09:49:08.000000 txdpy-7.6.8/txdpy/requests_operation.py
--rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/selenium_Firefox.py
--rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/str_category.py
--rw-rw-rw-   0        0        0     1042 2024-04-03 08:33:24.000000 txdpy-7.6.8/txdpy/text_similar.py
--rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.6.8/txdpy/translate.py
-drwxrwxrwx   0        0        0        0 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/
--rw-rw-rw-   0        0        0       71 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-30 09:31:44.000000 txdpy-7.6.8/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 06:59:05.000000 txdpy-7.6.9/
+-rw-rw-rw-   0        0        0       71 2024-05-07 06:59:05.000000 txdpy-7.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 06:59:05.000000 txdpy-7.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-05-07 06:58:42.000000 txdpy-7.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:59:05.000000 txdpy-7.6.9/txdpy/
+-rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.6.9/txdpy/URLjoin.py
+-rw-rw-rw-   0        0        0     2851 2024-04-29 03:32:28.000000 txdpy-7.6.9/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    28068 2024-04-30 09:29:05.000000 txdpy-7.6.9/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0     3855 2024-04-30 03:54:19.000000 txdpy-7.6.9/txdpy/easyreq.py
+-rw-rw-rw-   0        0        0     5977 2024-05-07 06:57:21.000000 txdpy-7.6.9/txdpy/excel_easy.py
+-rw-rw-rw-   0        0        0     2472 2024-04-10 04:32:34.000000 txdpy-7.6.9/txdpy/get_key.py
+-rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.6.9/txdpy/list_processing.py
+-rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.6.9/txdpy/lookup.py
+-rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.6.9/txdpy/progress_display.py
+-rw-rw-rw-   0        0        0     6469 2024-03-21 05:24:55.000000 txdpy-7.6.9/txdpy/pytmysql.py
+-rw-rw-rw-   0        0        0    11855 2024-04-07 07:33:20.000000 txdpy-7.6.9/txdpy/read_data.py
+-rw-rw-rw-   0        0        0     3049 2024-04-16 09:49:08.000000 txdpy-7.6.9/txdpy/requests_operation.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.6.9/txdpy/selenium_Firefox.py
+-rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.6.9/txdpy/str_category.py
+-rw-rw-rw-   0        0        0     1042 2024-04-03 08:33:24.000000 txdpy-7.6.9/txdpy/text_similar.py
+-rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.6.9/txdpy/translate.py
+drwxrwxrwx   0        0        0        0 2024-05-07 06:59:05.000000 txdpy-7.6.9/txdpy.egg-info/
+-rw-rw-rw-   0        0        0       71 2024-05-07 06:59:05.000000 txdpy-7.6.9/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2024-05-07 06:59:05.000000 txdpy-7.6.9/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 06:59:05.000000 txdpy-7.6.9/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2024-05-07 06:59:05.000000 txdpy-7.6.9/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-07 06:59:05.000000 txdpy-7.6.9/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-7.6.8/txdpy/URLjoin.py` & `txdpy-7.6.9/txdpy/URLjoin.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/__init__.py` & `txdpy-7.6.9/txdpy/__init__.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/bk_179.py` & `txdpy-7.6.9/txdpy/bk_179.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/easyreq.py` & `txdpy-7.6.9/txdpy/easyreq.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/excel_easy.py` & `txdpy-7.6.9/txdpy/excel_easy.py`

 * *Files 26% similar despite different names*

```diff
@@ -66,26 +66,103 @@
         if '.' in num:
             num = float(num)
         else:
             num = int(num)
     return num
 
 #读取execl数据
+import os.path
+from .pytmysql import PyMySQL
+import xlrd,xlsxwriter,zipfile
+from .bk_179 import optstr
+from file_ls import ls
+from tqdm import tqdm
+
+def excel_into_mysql(file:str,host:str, password:str, database:str,bm:str,th_a=1,stat:int=0,port:int=3306, user:str='root',auto_add_key:bool=True):
+    """
+    :param file: 文件路径
+    :param host: mysql地址
+    :param password: mysql密码
+    :param database: mysql数据库名称
+    :param bm: 数据库表名称
+    :param th_a: 插入数据表表头，可传入excel对应行或列表
+    :param stat: 插入数据库数据行，有默认规则，可自定义
+    :param port: mysql端口号
+    :param user: mysql用户名
+    :param auto_add_key: 是否自动添加表头字段
+    :return:
+    """
+    data = xlrd.open_workbook(file)
+    table = data.sheets()[0]  #通过工作表索引顺序获取
+    nrows = table.nrows #有效行数
+    ncols = table.ncols #有效列数
+    data=[]
+    for r in range(nrows):
+        l=[]
+        for c in range(ncols):
+            l.append(table.cell_value(r, c))
+        data.append(l)
+    mysql = PyMySQL(host=host,port=3306, user='root', password=password, database=database,auto_add_key=auto_add_key)
+    th=[]
+    if type(th_a) is int:
+        th=data[th_a-1]
+        stat=th_a
+    elif type(th) is list:
+        th = th_a
+    for v in data[stat:]:
+        mysql.insert_into(bm,th,v)
+    mysql.close()
+
+def gen_excel(data:list,save_path,header=None,is_optstr=True):
+    """
+    :param data:列表数据
+    :param save_path:保存excel路径
+    :param header:表头
+    """
+    if header:
+        data = list(data)
+        data.insert(0,header)
+    workbook = xlsxwriter.Workbook(save_path if save_path.endswith('.xlsx') else f'{save_path}.xlsx')
+    sheet = workbook.add_worksheet()
+    for row_num, row_data in enumerate(tqdm(data,desc=f'{os.path.basename(save_path)}')):
+        for col_num, col_value in enumerate(row_data):
+            if is_optstr:
+                sheet.write(row_num, col_num, optstr(col_value if col_value is None else str(col_value)))
+            else:
+                sheet.write(row_num, col_num, col_value)
+    workbook.close()
+
+#保留有效的小数位
+def prvadepl(num):
+    if type(num)==float or type(num)==numpy.float64:
+        num = str(num).rstrip('0').rstrip('.')
+        if '.' in num:
+            num = float(num)
+        else:
+            num = int(num)
+    return num
+
+#读取execl数据
 def read_excel(file_path,sheet_index=0):
     """
     :param file_path:文件路径或路径下第一个文件
     :param sheet_index:工作表索引默认第一个
     return:表格数据
     """
     if not file_path.endswith('.xlsx'):
         file_paths=ls(file_path)
         for path in file_paths:
             if path.endswith('.xlsx'):
                 file_path=path
                 break
     from openpyxl import load_workbook
-    workbook = load_workbook(filename=file_path,read_only=True)
-    worksheet = workbook.worksheets[sheet_index]
-    datas = []
-    for row in worksheet.iter_rows():
-        datas.append([prvadepl(cell.value) if isinstance(cell.value, float) else cell.value for cell in row])
-    return datas
+    try:
+        workbook = load_workbook(filename=file_path,read_only=True)
+        worksheet = workbook.worksheets[sheet_index]
+        datas = []
+        for row in worksheet.iter_rows():
+            datas.append([prvadepl(cell.value) if isinstance(cell.value, float) else cell.value for cell in row])
+        return datas
+    except zipfile.BadZipFile:
+        from txdpy import webptablesl
+        with open(file_path, 'r', encoding='utf-8') as f:
+            return webptablesl(f.read(), '//table')
```

### Comparing `txdpy-7.6.8/txdpy/get_key.py` & `txdpy-7.6.9/txdpy/get_key.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/list_processing.py` & `txdpy-7.6.9/txdpy/list_processing.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/lookup.py` & `txdpy-7.6.9/txdpy/lookup.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/progress_display.py` & `txdpy-7.6.9/txdpy/progress_display.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/pytmysql.py` & `txdpy-7.6.9/txdpy/pytmysql.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/read_data.py` & `txdpy-7.6.9/txdpy/read_data.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/requests_operation.py` & `txdpy-7.6.9/txdpy/requests_operation.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/selenium_Firefox.py` & `txdpy-7.6.9/txdpy/selenium_Firefox.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/str_category.py` & `txdpy-7.6.9/txdpy/str_category.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/text_similar.py` & `txdpy-7.6.9/txdpy/text_similar.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.6.8/txdpy/translate.py` & `txdpy-7.6.9/txdpy/translate.py`

 * *Files identical despite different names*


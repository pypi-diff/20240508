# Comparing `tmp/robotframework-xlibrary-11.0.7.tar.gz` & `tmp/robotframework-xlibrary-11.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-xlibrary-11.0.7.tar", last modified: Tue May  7 09:50:01 2024, max compression
+gzip compressed data, was "dist\robotframework-xlibrary-11.0.8.tar", last modified: Wed May  8 07:21:37 2024, max compression
```

## Comparing `robotframework-xlibrary-11.0.7.tar` & `robotframework-xlibrary-11.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/
--rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-11.0.7/LICENSE
--rw-rw-rw-   0        0        0     2269 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2024-04-22 17:31:21.000000 robotframework-xlibrary-11.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/setup.cfg
--rw-rw-rw-   0        0        0      818 2024-05-07 09:41:25.000000 robotframework-xlibrary-11.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/XLibrary/
--rw-rw-rw-   0        0        0     1114 2024-04-25 02:20:02.000000 robotframework-xlibrary-11.0.7/src/XLibrary/__init__.py
--rw-rw-rw-   0        0        0      235 2024-04-25 02:20:03.000000 robotframework-xlibrary-11.0.7/src/XLibrary/main.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/XLibrary/submodule1/
--rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.7/src/XLibrary/submodule1/__init__.py
--rw-rw-rw-   0        0        0     4870 2024-04-24 03:28:43.000000 robotframework-xlibrary-11.0.7/src/XLibrary/submodule1/module1.py
--rw-rw-rw-   0        0        0     6471 2024-05-07 09:24:36.000000 robotframework-xlibrary-11.0.7/src/XLibrary/submodule1/module2.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/XLibrary/submodule2/
--rw-rw-rw-   0        0        0      114 2024-04-25 02:19:59.000000 robotframework-xlibrary-11.0.7/src/XLibrary/submodule2/__init__.py
--rw-rw-rw-   0        0        0     2570 2024-05-07 09:10:53.000000 robotframework-xlibrary-11.0.7/src/XLibrary/submodule2/module1.py
--rw-rw-rw-   0        0        0      261 2024-04-25 02:20:02.000000 robotframework-xlibrary-11.0.7/src/XLibrary/submodule2/module2.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/robotframework_xlibrary.egg-info/
--rw-rw-rw-   0        0        0     2269 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/robotframework_xlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/robotframework_xlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/robotframework_xlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/robotframework_xlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 09:50:01.000000 robotframework-xlibrary-11.0.7/src/robotframework_xlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/
+-rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-11.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2269 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2024-04-22 17:31:21.000000 robotframework-xlibrary-11.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      818 2024-05-08 07:18:44.000000 robotframework-xlibrary-11.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/XLibrary/
+-rw-rw-rw-   0        0        0     1114 2024-04-25 02:20:02.000000 robotframework-xlibrary-11.0.8/src/XLibrary/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-04-25 02:20:03.000000 robotframework-xlibrary-11.0.8/src/XLibrary/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/XLibrary/submodule1/
+-rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.8/src/XLibrary/submodule1/__init__.py
+-rw-rw-rw-   0        0        0     4870 2024-04-24 03:28:43.000000 robotframework-xlibrary-11.0.8/src/XLibrary/submodule1/module1.py
+-rw-rw-rw-   0        0        0     9324 2024-05-08 07:17:54.000000 robotframework-xlibrary-11.0.8/src/XLibrary/submodule1/module2.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/XLibrary/submodule2/
+-rw-rw-rw-   0        0        0      114 2024-04-25 02:19:59.000000 robotframework-xlibrary-11.0.8/src/XLibrary/submodule2/__init__.py
+-rw-rw-rw-   0        0        0     2570 2024-05-07 09:10:53.000000 robotframework-xlibrary-11.0.8/src/XLibrary/submodule2/module1.py
+-rw-rw-rw-   0        0        0      261 2024-04-25 02:20:02.000000 robotframework-xlibrary-11.0.8/src/XLibrary/submodule2/module2.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/robotframework_xlibrary.egg-info/
+-rw-rw-rw-   0        0        0     2269 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/robotframework_xlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/robotframework_xlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/robotframework_xlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/robotframework_xlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 07:21:37.000000 robotframework-xlibrary-11.0.8/src/robotframework_xlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-xlibrary-11.0.7/PKG-INFO` & `robotframework-xlibrary-11.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 11.0.7
+Version: 11.0.8
 Summary: Custom Library for MyAIS 2.0 Automation
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-11.0.7/README.md` & `robotframework-xlibrary-11.0.8/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.7/setup.py` & `robotframework-xlibrary-11.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="robotframework-xlibrary",
-    version="11.0.7",
+    version="11.0.8",
     author="Tassana Khrueawan",
     author_email="tassana.khr@gmail.com",
     description="Custom Library for MyAIS 2.0 Automation",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Khrx1999/robotframework-xlibrary.git",
     package_dir={'': 'src'},
```

### Comparing `robotframework-xlibrary-11.0.7/src/XLibrary/__init__.py` & `robotframework-xlibrary-11.0.8/src/XLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.7/src/XLibrary/submodule1/module1.py` & `robotframework-xlibrary-11.0.8/src/XLibrary/submodule1/module1.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.7/src/XLibrary/submodule1/module2.py` & `robotframework-xlibrary-11.0.8/src/XLibrary/submodule1/module2.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,14 +77,78 @@
             cursor = cursor.sort(sort)
         if limit:
             cursor = cursor.limit(limit)
 
         results = list(cursor)
         return results
       
+      
+    @keyword("XQuery Dynamic Value")
+    def query_dynamic_value(self, result, field='None', value='None', expect=None):
+        """
+        ***|    Description     |***
+        |   *`XQuery Dynamic Value`*   |   เป็น Keyword สำหรับ Query ข้อมูลใน Collection แบบเจาะลงไป |
+ 
+       
+        ***|    Example     |***
+        | *`${arpu_value}`* | *`XQuery Dynamic Value`* | *`result`* | *`productCharacteristic`* | *`name`* | *`arpu`* |
+        | *`Log`* | *`${arpu_value}`* |
+ 
+       
+        ***|    Parameters     |***
+        - **`result`**  ผลลัพธ์ของการ Query ที่เป็นรายการข้อมูลจาก MongoDB.
+        - **`field`**   ชื่อฟิลด์ในข้อมูลที่ต้องการเจาะลงไป.
+        - **`value`**   ชื่อคีย์ภายในฟิลด์ที่ต้องการเข้าถึง.
+        - **`expect`**  ค่าที่ต้องการเทียบเพื่อหาข้อมูลที่ตรงกับเงื่อนไข.
+ 
+ 
+        *`Create By Tassana Khrueawan`*
+        """
+        for item in result:
+            if field in item and isinstance(item[field], list):
+                if expect:
+                    for char in item[field]:
+                        if char.get(value) == expect:
+                            return char.get('value')
+                else:
+                    return item[field]
+        return None
+ 
+ 
+    @keyword("XQuery Specific Value")
+    def query_specific_value(self, result, field_name=None):
+        """
+        ***|    Description     |***
+        |   XQuery Specific Value   |   Keyword สำหรับ Query ข้อมูลใน Collection แบบไม่เจาะลงไป |
+ 
+       
+        ***|    Example     |***
+        | *`${name}`* | *`XQuery Specific Value`* | *`result`* | *`name`* |
+        | *`Log`* | *`${name}`* |
+ 
+ 
+        ***|    Parameters     |***
+        - **`result`**  ผลลัพธ์ของการ Query ที่เป็นรายการข้อมูลจาก MongoDB.
+        - **`field_name`**   ชื่อฟิลด์ที่ต้องการเข้าถึงเพื่อค้นหาค่าภายใน.
+ 
+ 
+        *`Create By Tassana Khrueawan`*
+        """
+        if not field_name:
+            return result
+ 
+        results = []
+        if isinstance(result, list):
+            for doc in result:
+                if isinstance(doc, dict) and field_name in doc:
+                    results.append(doc[field_name])
+        else:
+            results = result.get(field_name, None)
+ 
+        return results  
 
     @keyword("XConvert BSON Document to JSON Object")
     def bson_to_json_object(self, bson_data):
         """
         แปลงข้อมูล BSON เป็นอ็อบเจกต์ Python (dictionary หรือ list) โดยไม่ต้องแปลงเป็นสตริง JSON
 
         พารามิเตอร์:
```

### Comparing `robotframework-xlibrary-11.0.7/src/XLibrary/submodule2/module1.py` & `robotframework-xlibrary-11.0.8/src/XLibrary/submodule2/module1.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.7/src/robotframework_xlibrary.egg-info/PKG-INFO` & `robotframework-xlibrary-11.0.8/src/robotframework_xlibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 11.0.7
+Version: 11.0.8
 Summary: Custom Library for MyAIS 2.0 Automation
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-11.0.7/src/robotframework_xlibrary.egg-info/SOURCES.txt` & `robotframework-xlibrary-11.0.8/src/robotframework_xlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*


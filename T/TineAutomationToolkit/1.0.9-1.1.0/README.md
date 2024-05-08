# Comparing `tmp/TineAutomationToolkit-1.0.9.tar.gz` & `tmp/TineAutomationToolkit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TineAutomationToolkit-1.0.9.tar", last modified: Fri May  3 10:14:55 2024, max compression
+gzip compressed data, was "dist\TineAutomationToolkit-1.1.0.tar", last modified: Wed May  8 04:00:40 2024, max compression
```

## Comparing `TineAutomationToolkit-1.0.9.tar` & `TineAutomationToolkit-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/
--rw-rw-rw-   0        0        0     2280 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/
--rw-rw-rw-   0        0        0      403 2024-04-25 03:30:22.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/detect/
--rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/detect/__init__.py
--rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/detect/detectelement.py
-drwxrwxrwx   0        0        0        0 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/
--rw-rw-rw-   0        0        0      812 2024-04-25 03:30:23.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/__init__.py
--rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/capturescreenshot.py
--rw-rw-rw-   0        0        0     4726 2024-04-11 09:59:28.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/connectionmanagement.py
--rw-rw-rw-   0        0        0    18183 2024-04-19 08:45:03.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/controlelement.py
--rw-rw-rw-   0        0        0     4187 2024-05-03 10:12:43.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/convertobject.py
--rw-rw-rw-   0        0        0     2495 2024-04-17 15:53:57.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/keyevent.py
--rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/scroll.py
--rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/toolkitstest.py
--rw-rw-rw-   0        0        0     2444 2024-04-17 15:25:52.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/touch.py
--rw-rw-rw-   0        0        0     8386 2024-04-19 09:32:00.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/waitingelement.py
-drwxrwxrwx   0        0        0        0 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit.egg-info/
--rw-rw-rw-   0        0        0     2280 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      830 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/TineAutomationToolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 10:14:55.000000 TineAutomationToolkit-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      755 2024-05-03 09:51:13.000000 TineAutomationToolkit-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:00:40.000000 TineAutomationToolkit-1.1.0/
+-rw-rw-rw-   0        0        0     2280 2024-05-08 04:00:40.000000 TineAutomationToolkit-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 04:00:40.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/
+-rw-rw-rw-   0        0        0      403 2024-04-25 03:30:22.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:00:40.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/detect/
+-rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/detect/__init__.py
+-rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/detect/detectelement.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:00:40.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/
+-rw-rw-rw-   0        0        0      812 2024-04-25 03:30:23.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/capturescreenshot.py
+-rw-rw-rw-   0        0        0     4726 2024-04-11 09:59:28.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/connectionmanagement.py
+-rw-rw-rw-   0        0        0    18183 2024-04-19 08:45:03.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/controlelement.py
+-rw-rw-rw-   0        0        0     4388 2024-05-08 03:58:42.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/convertobject.py
+-rw-rw-rw-   0        0        0     2495 2024-04-17 15:53:57.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/keyevent.py
+-rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/scroll.py
+-rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/toolkitstest.py
+-rw-rw-rw-   0        0        0     2444 2024-04-17 15:25:52.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/touch.py
+-rw-rw-rw-   0        0        0    10151 2024-05-08 03:55:50.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/waitingelement.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:00:40.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit.egg-info/
+-rw-rw-rw-   0        0        0     2280 2024-05-08 04:00:39.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      830 2024-05-08 04:00:39.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 04:00:39.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-08 04:00:39.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-08 04:00:39.000000 TineAutomationToolkit-1.1.0/TineAutomationToolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 04:00:40.000000 TineAutomationToolkit-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-05-08 03:53:15.000000 TineAutomationToolkit-1.1.0/setup.py
```

### Comparing `TineAutomationToolkit-1.0.9/PKG-INFO` & `TineAutomationToolkit-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.9
+Version: 1.1.0
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.9/README.md` & `TineAutomationToolkit-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/detect/detectelement.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/detect/detectelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/__init__.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/capturescreenshot.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/capturescreenshot.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/connectionmanagement.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/connectionmanagement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/controlelement.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/controlelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/convertobject.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/convertobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,16 @@
             - **`data`**  ข้อมูล Json.
         """
         self._tree_structure(data)
 
     def convert_time_to_local_timezone(self,date,timezone='Asia/Bangkok'):
         """ Owner : suthasinee.k@arcadiaapm.com
         ***|    Description     |***
-        | 
+        |   มีไว้สำหรับรับเวลาที่ได้มาแล้วแปลงเป็นเวลาของ TimeZone 
+        |   โดย Default คือ Asia/Bangkok
         """
         # กำหนด timezone เป็น UTC
         utc_timezone = pytz.timezone('UTC')
         # แปลง timezone จาก UTC เป็น local timezone
         local_timezone = pytz.timezone(timezone)  
         # ตรวจสอบว่าข้อมูลนำเข้าเป็น datetime object หรือไม่
         if isinstance(date, datetime):
```

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/keyevent.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/keyevent.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/scroll.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/scroll.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/touch.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/touch.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit/keywords/waitingelement.py` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit/keywords/waitingelement.py`

 * *Files 12% similar despite different names*

```diff
@@ -147,14 +147,49 @@
             if not present:
                 return
             else:
                 return error or "Text '%s' did not disappear in %s" % (text, self._format_timeout(timeout))
 
         self._wait_until_no_error(timeout, check_present)    
 
+    def native_wait_until_page_does_not_contain_element(self, locator, timeout=None, error=None):
+        """Waits until element specified with `locator` disappears from current page.
+
+        Fails if `timeout` expires before the element disappears. See
+        `introduction` for more information about `timeout` and its
+        default value.
+
+        `error` can be used to override the default error message.
+
+         See also `Wait Until Page Contains`,
+        `Wait Until Page Does Not Contain`,
+        `Wait Until Page Contains Element` and
+        BuiltIn keyword `Wait Until Keyword Succeeds`.
+
+        ===================================================
+
+        จะล้มเหลวถ้า `timeout` หมดก่อนที่ `element` จะหายไป ดู
+        `introduction` เพื่อข้อมูลเพิ่มเติมเกี่ยวกับ `timeout` และค่าเริ่มต้นของมัน
+
+        `error` สามารถใช้เพื่อแทนที่ข้อความแสดงข้อผิดพลาดเริ่มต้น
+
+        ดูเพิ่มเติมที่ `Wait Until Page Contains`,
+        `Wait Until Page Contains Element`,
+        `Wait Until Page Does Not Contain Element` และคำสั่ง BuiltIn `Wait Until Keyword Succeeds`.
+        """
+
+        def check_present():
+            present = conelement._is_element_present(locator)
+            if not present:
+                return
+            else:
+                return error or "Text '%s' did not disappear in %s" % (locator, self._format_timeout(timeout))
+
+        self._wait_until_no_error(timeout, check_present)   
+
     
     #PRIVATE_FUNCTION
         
     def _format_timeout(self, timeout):
         timeout = robot.utils.timestr_to_secs(timeout) if timeout is not None else timeout_in_secs
         return robot.utils.secs_to_timestr(timeout)
```

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit.egg-info/PKG-INFO` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.0.9
+Version: 1.1.0
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.0.9/TineAutomationToolkit.egg-info/SOURCES.txt` & `TineAutomationToolkit-1.1.0/TineAutomationToolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.0.9/setup.py` & `TineAutomationToolkit-1.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="TineAutomationToolkit",
-    version="1.0.9",
+    version="1.1.0",
     author="Pornpawit Suttha",
     author_email="pornpawit14suttha@gmail.com",
     description="Test Library for TineAutomationToolkit",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/pornpawit08/TineAutomationToolkit.git",
     packages=find_packages(),
```


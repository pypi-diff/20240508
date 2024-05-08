# Comparing `tmp/testplans-0.2.7.tar.gz` & `tmp/testplans-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.2.7.tar", last modified: Wed May  8 09:48:26 2024, max compression
+gzip compressed data, was "testplans-0.2.8.tar", last modified: Wed May  8 10:13:28 2024, max compression
```

## Comparing `testplans-0.2.7.tar` & `testplans-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 09:48:26.932843 testplans-0.2.7/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-05-08 09:48:26.932385 testplans-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-05-08 08:21:08.000000 testplans-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 09:48:26.935775 testplans-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 09:48:26.922497 testplans-0.2.7/testplans/
--rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.7/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.7/testplans/_results.py
--rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.2.7/testplans/api.py
--rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.7/testplans/devices.py
--rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.7/testplans/gui.py
--rw-rw-rw-   0        0        0    11908 2024-05-08 07:37:04.000000 testplans-0.2.7/testplans/main.py
--rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.7/testplans/models.py
--rw-rw-rw-   0        0        0    12181 2024-05-08 09:39:24.000000 testplans-0.2.7/testplans/tc.py
--rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.7/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-05-08 09:48:26.930488 testplans-0.2.7/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-05-08 09:48:26.000000 testplans-0.2.7/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-08 09:48:26.000000 testplans-0.2.7/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 09:48:26.000000 testplans-0.2.7/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 09:48:26.000000 testplans-0.2.7/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 10:13:28.027063 testplans-0.2.8/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     5494 2024-05-08 10:13:28.027063 testplans-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4584 2024-05-08 10:12:56.000000 testplans-0.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 10:13:28.028061 testplans-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:13:28.019610 testplans-0.2.8/testplans/
+-rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.8/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.8/testplans/_results.py
+-rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.2.8/testplans/api.py
+-rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.8/testplans/devices.py
+-rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.8/testplans/gui.py
+-rw-rw-rw-   0        0        0    11908 2024-05-08 07:37:04.000000 testplans-0.2.8/testplans/main.py
+-rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.8/testplans/models.py
+-rw-rw-rw-   0        0        0    12244 2024-05-08 10:11:05.000000 testplans-0.2.8/testplans/tc.py
+-rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.8/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-05-08 10:13:28.026038 testplans-0.2.8/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5494 2024-05-08 10:13:27.000000 testplans-0.2.8/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-08 10:13:28.000000 testplans-0.2.8/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 10:13:27.000000 testplans-0.2.8/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 10:13:27.000000 testplans-0.2.8/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.2.7/LICENSE` & `testplans-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `testplans-0.2.7/PKG-INFO` & `testplans-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.7
+Version: 0.2.8
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.2.7)
+# testplans (v0.2.8)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.7/README.md` & `testplans-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# testplans (v0.2.7)
+# testplans (v0.2.8)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.7/setup.py` & `testplans-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.7/testplans/_results.py` & `testplans-0.2.8/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.7/testplans/api.py` & `testplans-0.2.8/testplans/api.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.7/testplans/devices.py` & `testplans-0.2.8/testplans/devices.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.7/testplans/gui.py` & `testplans-0.2.8/testplans/gui.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.7/testplans/main.py` & `testplans-0.2.8/testplans/main.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.7/testplans/models.py` & `testplans-0.2.8/testplans/models.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.7/testplans/tc.py` & `testplans-0.2.8/testplans/tc.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
     exx: Optional[Exception]
     progress: int
 
     # =================================================================================================================
     # def __init__(self, dut: Any, _settings_files: Union[None, pathlib.Path, List[pathlib.Path]] = None):
     def __init__(self, index: int = 0):
         super().__init__()
-
         self.LOGGER.debug("init tc")
 
         self.INDEX = index
 
         if self.DEVICES__CLS:
             self.DEVICES__BY_INDEX = self.DEVICES__CLS(self.INDEX)
 
@@ -251,15 +250,18 @@
         progress = self.progress
         self.teardown()
         self.progress = progress
 
     @classmethod
     def terminate__cls(cls) -> None:
         for tc_inst in cls.TCS__INST:
-            tc_inst.terminate()
+            try:
+                tc_inst.terminate()
+            except:
+                pass
 
         cls.teardown__cls()
 
     # =================================================================================================================
     def run(self) -> None:
         self.LOGGER.debug("run")
```

### Comparing `testplans-0.2.7/testplans/tm.py` & `testplans-0.2.8/testplans/tm.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.7/testplans.egg-info/PKG-INFO` & `testplans-0.2.8/testplans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.7
+Version: 0.2.8
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.2.7)
+# testplans (v0.2.8)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```


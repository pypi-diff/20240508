# Comparing `tmp/testplans-0.2.6.tar.gz` & `tmp/testplans-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.2.6.tar", last modified: Thu May  2 10:00:48 2024, max compression
+gzip compressed data, was "testplans-0.2.7.tar", last modified: Wed May  8 09:48:26 2024, max compression
```

## Comparing `testplans-0.2.6.tar` & `testplans-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 10:00:48.459642 testplans-0.2.6/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-05-02 10:00:48.459642 testplans-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-05-02 10:00:30.000000 testplans-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 10:00:48.461071 testplans-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:00:48.454643 testplans-0.2.6/testplans/
--rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.6/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.6/testplans/_results.py
--rw-rw-rw-   0        0        0     3974 2024-04-26 14:17:18.000000 testplans-0.2.6/testplans/api.py
--rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.6/testplans/devices.py
--rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.6/testplans/gui.py
--rw-rw-rw-   0        0        0    11908 2024-05-02 10:00:30.000000 testplans-0.2.6/testplans/main.py
--rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.6/testplans/models.py
--rw-rw-rw-   0        0        0    11272 2024-04-26 14:26:56.000000 testplans-0.2.6/testplans/tc.py
--rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.6/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:00:48.459642 testplans-0.2.6/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-05-02 10:00:48.000000 testplans-0.2.6/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-02 10:00:48.000000 testplans-0.2.6/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 10:00:48.000000 testplans-0.2.6/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-02 10:00:48.000000 testplans-0.2.6/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 09:48:26.932843 testplans-0.2.7/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     5494 2024-05-08 09:48:26.932385 testplans-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4584 2024-05-08 08:21:08.000000 testplans-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 09:48:26.935775 testplans-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:48:26.922497 testplans-0.2.7/testplans/
+-rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.7/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.7/testplans/_results.py
+-rw-rw-rw-   0        0        0     3974 2024-05-08 07:37:04.000000 testplans-0.2.7/testplans/api.py
+-rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.7/testplans/devices.py
+-rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.7/testplans/gui.py
+-rw-rw-rw-   0        0        0    11908 2024-05-08 07:37:04.000000 testplans-0.2.7/testplans/main.py
+-rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.7/testplans/models.py
+-rw-rw-rw-   0        0        0    12181 2024-05-08 09:39:24.000000 testplans-0.2.7/testplans/tc.py
+-rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.7/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-05-08 09:48:26.930488 testplans-0.2.7/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5494 2024-05-08 09:48:26.000000 testplans-0.2.7/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-08 09:48:26.000000 testplans-0.2.7/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 09:48:26.000000 testplans-0.2.7/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 09:48:26.000000 testplans-0.2.7/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.2.6/LICENSE` & `testplans-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `testplans-0.2.6/PKG-INFO` & `testplans-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.6
+Version: 0.2.7
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
 
-# testplans (v0.2.6)
+# testplans (v0.2.7)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.6/README.md` & `testplans-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# testplans (v0.2.6)
+# testplans (v0.2.7)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.6/setup.py` & `testplans-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.6/testplans/_results.py` & `testplans-0.2.7/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.6/testplans/api.py` & `testplans-0.2.7/testplans/api.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.6/testplans/devices.py` & `testplans-0.2.7/testplans/devices.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.6/testplans/gui.py` & `testplans-0.2.7/testplans/gui.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.6/testplans/main.py` & `testplans-0.2.7/testplans/main.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.6/testplans/models.py` & `testplans-0.2.7/testplans/models.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.6/testplans/tc.py` & `testplans-0.2.7/testplans/tc.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 # =====================================================================================================================
 class Signals(SignalsTemplate):
     signal__tc_state_changed = pyqtSignal(_TestCaseBase)
 
 
 # =====================================================================================================================
 class TestCaseBase(_TestCaseBase, QThread):
+    LOG_ENABLE = True
+    LOG_USE_FILE = False
+
     # SETTINGS ------------------------------------
     NAME: str = ""      # set auto!
     DESCRIPTION: str = ""
     SKIP: Optional[bool] = None     # access only over CLASS attribute! not instance!!!
     skip_tc_dut: Optional[bool] = None
     ASYNC: Optional[bool] = True
     # STOP_IF_FALSE_RESULT: Optional[bool] = None     # NOT USED NOW! MAYBE NOT IMPORTANT!!!
@@ -57,14 +60,17 @@
     exx: Optional[Exception]
     progress: int
 
     # =================================================================================================================
     # def __init__(self, dut: Any, _settings_files: Union[None, pathlib.Path, List[pathlib.Path]] = None):
     def __init__(self, index: int = 0):
         super().__init__()
+
+        self.LOGGER.debug("init tc")
+
         self.INDEX = index
 
         if self.DEVICES__CLS:
             self.DEVICES__BY_INDEX = self.DEVICES__CLS(self.INDEX)
 
         self.clear()
 
@@ -115,14 +121,16 @@
                 for file in _settings_files:
                     if file.exists():
                         file_data = json.loads(file.read_text())
                         result.update(file_data)
         return result
 
     def clear(self) -> None:
+        self.LOGGER.debug("clear")
+
         self.result = None
         self.details = {}
         self.exx = None
         self.progress = 0
 
     @classmethod
     def clear__cls(cls):
@@ -156,19 +164,23 @@
     # @result__cls_startup.setter
     # def result__cls_startup(cls, value: Optional[bool]) -> None:
     #     cls.__result__cls_startup = value
     #     # cls.signals.signal__tc_state_changed.emit(cls)
 
     # DETAILS ---------------------------------------------------------------------------------------------------------
     def details_update(self, details: Dict[str, Any]) -> None:
+        self.LOGGER.debug("")
+
         self.details.update(details)
         # self.signals.signal__tc_state_changed.emit(self)
 
     # =================================================================================================================
     def info_pretty(self) -> str:
+        self.LOGGER.debug("")
+
         # fixme: ref from info_get
         result = ""
 
         result += f"NAME={self.NAME}\n"
         result += f"DESCRIPTION={self.DESCRIPTION}\n"
         result += f"SKIP={self.SKIP}\n"
         result += f"skip_tc_dut={self.skip_tc_dut}\n"
@@ -201,14 +213,16 @@
             "settings": cls.settings_read(),
         }
 
         return ModelTcClsInfo(**result)
 
     # =================================================================================================================
     def get__results(self) -> ModelTcInstResult:
+        self.LOGGER.debug("")
+
         result = {
             **self.get__info().dict(),
 
             "DEVICE": self.DUT.get__info(),
 
             # RESULTS
             "is_active": self.isRunning(),
@@ -226,14 +240,16 @@
         results = []
         for tc_inst in cls.TCS__INST:
             results.append(tc_inst.get__results().dict())
         return results
 
     # =================================================================================================================
     def terminate(self) -> None:
+        self.LOGGER.debug("")
+
         super().terminate()
 
         progress = self.progress
         self.teardown()
         self.progress = progress
 
     @classmethod
@@ -241,66 +257,76 @@
         for tc_inst in cls.TCS__INST:
             tc_inst.terminate()
 
         cls.teardown__cls()
 
     # =================================================================================================================
     def run(self) -> None:
-        # self.LOGGER.debug("run clear")
+        self.LOGGER.debug("run")
 
         # PREPARE --------
         self.clear()
         if not self.DEVICES__BY_INDEX.DUT or not self.DEVICES__BY_INDEX.DUT.connect() or self.DEVICES__BY_INDEX.DUT.SKIP:
             return
 
         # WORK --------
-        # self.LOGGER.debug("run startup")
+        self.LOGGER.debug("run-startup")
         if self.startup():
             try:
-                # self.LOGGER.debug("run run_wrapped")
+                self.LOGGER.debug("run-run_wrapped START")
                 self.result = self.run_wrapped()
-                # self.LOGGER.debug(f"{self.result=}")
+                self.LOGGER.debug(f"run-run_wrapped FINISHED WITH {self.result=}")
             except Exception as exx:
                 self.exx = exx
-        # self.LOGGER.debug("run teardown")
+        self.LOGGER.debug("run-teardown")
         self.teardown()
 
     @classmethod
     def run__cls(cls) -> None:
         """run TC on batch duts(??? may be INDEXES???)
         prefered using in thread on upper level!
         """
         # if not cls.DEVICES__CLS.LIST__DUT:
         #     return
 
+        print(f"run__cls=START={cls.NAME=}={'='*50}")
         if cls.SKIP:
+            print(f"run__cls=SKIP={cls.NAME=}={'='*50}")
             return
 
         # ---------------------------------
+        print(f"run__cls=clear__cls")
         cls.clear__cls()
 
+        print(f"run__cls=startup__cls")
         cls.result__cls_startup = cls.startup__cls()
+        print(f"run__cls={cls.result__cls_startup=}")
         if not cls.result__cls_startup:
             return
 
         # BATCH --------------------------
         for tc_inst in cls.TCS__INST:
             if tc_inst.skip_tc_dut:
                 continue
 
+            print(f"run__cls=tc_inst.start({tc_inst.INDEX=})")
             tc_inst.start()
             if not cls.ASYNC:
+                print(f"run__cls=tc_inst.wait({tc_inst.INDEX=})inONEBYONE")
                 tc_inst.wait()
 
         # FINISH --------------------------
         if cls.ASYNC:
             for tc_inst in cls.TCS__INST:
+                print(f"run__cls=tc_inst.wait({tc_inst.INDEX=})inPARALLEL")
                 tc_inst.wait()
 
+        print(f"run__cls=teardown__cls")
         cls.teardown__cls()
+        print(f"run__cls=FINISH={cls.NAME=}={'='*50}")
 
     # REDEFINE ========================================================================================================
     pass
     pass
     pass
     pass
     pass
@@ -310,18 +336,20 @@
     @classmethod
     def startup__cls(cls) -> bool:
         """before batch work
         """
         return True
 
     def startup(self) -> bool:
+        self.LOGGER.debug("")
         self.progress = 1
         return True
 
     def teardown(self):
+        self.LOGGER.debug("")
         self.progress = 100
 
     @classmethod
     def teardown__cls(cls):
         pass
 
     # RUN -------------------------------------------------------------------------------------------------------------
```

### Comparing `testplans-0.2.6/testplans/tm.py` & `testplans-0.2.7/testplans/tm.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.6/testplans.egg-info/PKG-INFO` & `testplans-0.2.7/testplans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.6
+Version: 0.2.7
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
 
-# testplans (v0.2.6)
+# testplans (v0.2.7)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```


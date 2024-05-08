# Comparing `tmp/SleepHarmonizer-0.1.5.tar.gz` & `tmp/SleepHarmonizer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SleepHarmonizer-0.1.5.tar", last modified: Tue Apr 30 07:14:23 2024, max compression
+gzip compressed data, was "SleepHarmonizer-0.2.1.tar", last modified: Wed May  8 07:52:42 2024, max compression
```

## Comparing `SleepHarmonizer-0.1.5.tar` & `SleepHarmonizer-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.352892 SleepHarmonizer-0.1.5/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9049 2024-04-30 07:14:23.352892 SleepHarmonizer-0.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8562 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.347894 SleepHarmonizer-0.1.5/SleepHarmonizer/
--rw-rw-rw-   0 root         (0) root         (0)     4184 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/EDFWriter.py
--rw-rw-rw-   0 root         (0) root         (0)     3961 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/PSGEventManager.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6744 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.349893 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/
--rw-rw-rw-   0 root         (0) root         (0)     4077 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/Export.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/LoadData.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/Setup.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/phases/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.350893 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/
--rwxrwxrwx   0 root         (0) root         (0)    12683 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/AliceRMLLoader.py
--rw-rw-rw-   0 root         (0) root         (0)    11246 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/AliceTextReportLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     4568 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     8335 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py
--rw-rw-rw-   0 root         (0) root         (0)     8269 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoErgLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     7126 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderAlice.py
--rw-rw-rw-   0 root         (0) root         (0)     5374 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderDomino.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderTest.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.348894 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9049 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1217 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      153 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-30 07:14:23.000000 SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 07:14:23.352892 SleepHarmonizer-0.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-04-30 07:13:50.000000 SleepHarmonizer-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.351893 SleepHarmonizer-0.1.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 07:14:23.352892 SleepHarmonizer-0.1.5/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_Export.py
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_LoadData.py
--rwxrwxrwx   0 root         (0) root         (0)     1016 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_Setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-30 07:13:49.000000 SleepHarmonizer-0.1.5/tests/unit/test_SignalPreprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:52:42.623904 SleepHarmonizer-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9049 2024-05-08 07:52:42.622904 SleepHarmonizer-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8562 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:52:42.618904 SleepHarmonizer-0.2.1/SleepHarmonizer/
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/PSGEventManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6744 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      542 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:52:42.619904 SleepHarmonizer-0.2.1/SleepHarmonizer/phases/
+-rw-rw-rw-   0 root         (0) root         (0)     4077 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/phases/Export.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/phases/LoadData.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/phases/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:52:42.621904 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/
+-rwxrwxrwx   0 root         (0) root         (0)    12683 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/AliceRMLLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)    11246 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/AliceTextReportLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     4568 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     8335 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py
+-rw-rw-rw-   0 root         (0) root         (0)     8269 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/DominoErgLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7126 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/RecordLoaderAlice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5374 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/RecordLoaderDomino.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/RecordLoaderTest.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:52:42.621904 SleepHarmonizer-0.2.1/SleepHarmonizer/recordwriter/
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordwriter/RecordWriter.py
+-rw-rw-rw-   0 root         (0) root         (0)     4589 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordwriter/RecordWriterDICOM.py
+-rw-rw-rw-   0 root         (0) root         (0)     2297 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordwriter/RecordWriterEDF.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/SleepHarmonizer/recordwriter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:52:42.619904 SleepHarmonizer-0.2.1/SleepHarmonizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9049 2024-05-08 07:52:42.000000 SleepHarmonizer-0.2.1/SleepHarmonizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1315 2024-05-08 07:52:42.000000 SleepHarmonizer-0.2.1/SleepHarmonizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 07:52:42.000000 SleepHarmonizer-0.2.1/SleepHarmonizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      153 2024-05-08 07:52:42.000000 SleepHarmonizer-0.2.1/SleepHarmonizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-08 07:52:42.000000 SleepHarmonizer-0.2.1/SleepHarmonizer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 07:52:42.623904 SleepHarmonizer-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-05-08 07:52:07.000000 SleepHarmonizer-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:52:42.621904 SleepHarmonizer-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 07:52:42.622904 SleepHarmonizer-0.2.1/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1961 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/tests/unit/test_Export.py
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/tests/unit/test_LoadData.py
+-rwxrwxrwx   0 root         (0) root         (0)     1028 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/tests/unit/test_Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-05-08 07:52:05.000000 SleepHarmonizer-0.2.1/tests/unit/test_SignalPreprocessing.py
```

### Comparing `SleepHarmonizer-0.1.5/LICENSE` & `SleepHarmonizer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/PKG-INFO` & `SleepHarmonizer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SleepHarmonizer
-Version: 0.1.5
+Version: 0.2.1
 Summary: A Plugin and stand alone tool to harmonize sleep related data
 Home-page: https://gitlab.com/sleep-is-all-you-need/sleep-harmonizer
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SleepHarmonizer-0.1.5/README.md` & `SleepHarmonizer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/PSGEventManager.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/PSGEventManager.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/SignalPreprocessing.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/config.yaml` & `SleepHarmonizer-0.2.1/SleepHarmonizer/config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dataversion:
   version: init
   recordIds: null
   groupBy: null
   minimalSamplingRate: {}
 
 export-path: data/export/
+useWriter: RecordWriterEDF
 export:
   annotations:
     - apnea
     - arousal
     - limb
     - sleepStage
     - light
```

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/phases/Export.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/phases/Export.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from pathlib import Path
 import shutil
-from SleepHarmonizer.EDFWriter import EDFWriter
-from SleepHarmonizer.PSGEventManager import PSGEventManager
-from SleepHarmonizer.SignalPreprocessing import SignalPreprocessing
+from pathlib import Path
+
 from pyPhases import Phase
 from pyPhases.util import BatchProgress
-from pyPhasesRecordloader import AnnotationNotFound, ChannelsNotPresent, RecordLoader, Event
+from pyPhasesRecordloader import AnnotationNotFound, ChannelsNotPresent, Event, RecordLoader
+
+from SleepHarmonizer.PSGEventManager import PSGEventManager
+from SleepHarmonizer.recordwriter.RecordWriter import RecordWriter
+from SleepHarmonizer.SignalPreprocessing import SignalPreprocessing
+
 
 class Export(Phase):
-    skipExisting = False
+    skipExisting = True
     useMultiThreading = True
     useDigitalSignals = True
     prepareEventsFor = None
 
     def getAnnotationsFromDf(self, df):
         return df.T.to_dict().values()
 
@@ -22,83 +25,84 @@
             lightEvents.append(Event.fromdict({"start": lightOn, "duration": 0, "name": "Licht An"}))
         if lightOff > 0:
             lightEvents.append(Event.fromdict({"start": lightOff, "duration": 0, "name": "Licht Aus"}))
 
         return lightEvents
 
     def exportRecord(self, recordName):
-        exportFilename = self.exportPath + "/" + recordName
-        path = Path(exportFilename  + ".edf")
-        if path.is_file() and self.skipExisting:
+        rw = self.recordWriter
+        rl = self.recordLoader
+
+        if rw.exist(recordName) and self.skipExisting:
             self.log(f"Record {recordName} skipped because it already exists")
             return
-
-        rl = self.recordLoader
+        
 
         try:
-            psgSignal, events = self.recordLoader.loadRecord(recordName)
+            psgSignal, events = rl.loadRecord(recordName)
             em = PSGEventManager()
 
             events += self.getLightEvents(rl.lightOff, rl.lightOn)
             events = em.getDataframeFromEvents(events)
 
             # tailor psg signal
             keepSignals = self.getConfig("export.channels", None)
             psgSignal.reduceSignals(keepSignals)
 
             allowEventsConfig = self.getConfig("export.annotations", None)
             allowEvents = []
             if allowEventsConfig is not None:
                 for ev in allowEventsConfig:
-                    if ev in em.eventGroups and ev :
+                    if ev in em.eventGroups and ev:
                         allowEvents += em.eventGroups[ev]
                     else:
                         allowEvents.append(ev)
-                        
+
                 events = events.query("name in @allowEvents")
 
             annotations = self.getAnnotationsFromDf(events)
 
             # signal preprocessing / harmonizing
             targetFrequency = self.preProcessingConfig["targetFrequency"]
             signalProcessor = SignalPreprocessing(self.preProcessingConfig)
             psgSignal.targetFrequency = targetFrequency
             signalProcessor.preprocessingSignal(psgSignal)
 
             # write the harmonized signal into an edf
-            rw = EDFWriter()
-            tmpFilename = exportFilename + "_tmp"
-            rw.writeSignals(tmpFilename, psgSignal.signals, annotations, signalIsDigital=self.useDigitalSignals)
-            shutil.move(tmpFilename, exportFilename + ".edf")
+            rw.createFolderStructure()
+            tmpRecordName = recordName + "-tmp"
+
+            rw.writeSignals(tmpRecordName, psgSignal.signals, annotations, signalIsDigital=self.useDigitalSignals)
+            shutil.move(rw.getFilePath(tmpRecordName), rw.getFilePath(recordName)) 
 
         except AnnotationNotFound as e:
             self.logError(f"not all required annotation exist for {recordName}")
         except ChannelsNotPresent as e:
             self.logError(f"not all required channels exist for {recordName}: {e.channels}")
 
     def main(self):
         self.events = None
         self.annotations = []
 
         self.exportPath = self.getConfig("export-path")
         if not Path(self.exportPath).exists():
             Path(self.exportPath).mkdir(parents=True, exist_ok=True)
 
-
         recordId = self.getConfig("recordId", False)
         if not recordId:
             recordIds = self.project.getData("allDBRecordIds", list)
             # flatten grouped record ids
             recordIds = [recordId for groupedRecords in recordIds.values() for recordId in groupedRecords]
         else:
             self.useMultiThreading = False
             recordIds = [recordId]
 
         bp = BatchProgress()
         bp.asynchronous = True
         bp.useMultiThreading = self.useMultiThreading
 
         self.recordLoader = RecordLoader.get()
+        self.recordWriter = RecordWriter.get()
         self.recordLoader.useDigitalSignals = self.useDigitalSignals
 
         self.preProcessingConfig = self.getConfig("preprocessing")
         bp.start(self.exportRecord, batchList=recordIds)
```

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/phases/LoadData.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/phases/LoadData.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/AliceRMLLoader.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/AliceRMLLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/AliceTextReportLoader.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/AliceTextReportLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/DominoErgLoader.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/DominoErgLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderAlice.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/RecordLoaderAlice.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderDomino.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/RecordLoaderDomino.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer/recordloaders/RecordLoaderTest.py` & `SleepHarmonizer-0.2.1/SleepHarmonizer/recordloaders/RecordLoaderTest.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/PKG-INFO` & `SleepHarmonizer-0.2.1/SleepHarmonizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SleepHarmonizer
-Version: 0.1.5
+Version: 0.2.1
 Summary: A Plugin and stand alone tool to harmonize sleep related data
 Home-page: https://gitlab.com/sleep-is-all-you-need/sleep-harmonizer
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SleepHarmonizer-0.1.5/SleepHarmonizer.egg-info/SOURCES.txt` & `SleepHarmonizer-0.2.1/SleepHarmonizer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-SleepHarmonizer/EDFWriter.py
 SleepHarmonizer/PSGEventManager.py
 SleepHarmonizer/Plugin.py
 SleepHarmonizer/SignalPreprocessing.py
 SleepHarmonizer/__init__.py
 SleepHarmonizer/config.yaml
 SleepHarmonizer.egg-info/PKG-INFO
 SleepHarmonizer.egg-info/SOURCES.txt
 SleepHarmonizer.egg-info/dependency_links.txt
 SleepHarmonizer.egg-info/requires.txt
 SleepHarmonizer.egg-info/top_level.txt
 SleepHarmonizer/phases/Export.py
 SleepHarmonizer/phases/LoadData.py
-SleepHarmonizer/phases/Setup.py
 SleepHarmonizer/phases/__init__.py
 SleepHarmonizer/recordloaders/AliceRMLLoader.py
 SleepHarmonizer/recordloaders/AliceTextReportLoader.py
 SleepHarmonizer/recordloaders/DominoAnnotationLoader.py
 SleepHarmonizer/recordloaders/DominoAnnotationWriter.py
 SleepHarmonizer/recordloaders/DominoErgLoader.py
 SleepHarmonizer/recordloaders/RecordLoaderAlice.py
 SleepHarmonizer/recordloaders/RecordLoaderDomino.py
 SleepHarmonizer/recordloaders/RecordLoaderTest.py
 SleepHarmonizer/recordloaders/__init__.py
+SleepHarmonizer/recordwriter/RecordWriter.py
+SleepHarmonizer/recordwriter/RecordWriterDICOM.py
+SleepHarmonizer/recordwriter/RecordWriterEDF.py
+SleepHarmonizer/recordwriter/__init__.py
 tests/__init__.py
 tests/conftest.py
 tests/unit/__init__.py
 tests/unit/test_Export.py
 tests/unit/test_LoadData.py
 tests/unit/test_Plugin.py
-tests/unit/test_Setup.py
 tests/unit/test_SignalPreprocessing.py
```

### Comparing `SleepHarmonizer-0.1.5/setup.py` & `SleepHarmonizer-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SleepHarmonizer",
-    version="v0.1.5"[1:],
+    version="v0.2.1"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Plugin and stand alone tool to harmonize sleep related data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/sleep-is-all-you-need/sleep-harmonizer",
     packages=setuptools.find_packages(),
```

### Comparing `SleepHarmonizer-0.1.5/tests/unit/test_Export.py` & `SleepHarmonizer-0.2.1/tests/unit/test_Export.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 
 
 class TestLoadData(TestCase):
     phase = Export()
 
     @patch("shutil.move", return_value=None)
     @patch("pyPhasesRecordloaderSHHS.recordLoaders.RecordLoaderSHHS.RecordLoaderSHHS.loadRecord", side_effect=getTestSignalData)
-    @patch("SleepHarmonizer.EDFWriter.EDFWriter.writeSignals", return_value=None)
+    @patch("SleepHarmonizer.recordwriter.RecordWriterEDF.RecordWriterEDF.writeSignals", return_value=None)
     @OverwriteConfig({"recordId": "myId"})
     def testExport(self, mock_writeSignals, mock_loadRecord, mock_move):
         self.phase.run()
 
         self.assertTrue(mock_writeSignals.called)
         self.assertTrue(mock_loadRecord.called)
 
         file = mock_writeSignals.call_args[0][0]
         signals = mock_writeSignals.call_args[0][1]
         recordEvents = list(mock_writeSignals.call_args[0][2])
 
-        self.assertEqual(file, "data/export//myId_tmp")
+        self.assertEqual(file, "myId-tmp")
         self.assertEqual(len(signals), 1)
         self.assertEqual(len(recordEvents), 1)
         self.assertEqual(signals[0].name, "testsignal")
         self.assertEqual(recordEvents[0]["name"], "arousal")
         self.assertEqual(recordEvents[0]["start"], 1)
         self.assertEqual(recordEvents[0]["duration"], 1)
         self.assertEqual(signals[0].signal.tolist(), [1, 2, 3])
```

### Comparing `SleepHarmonizer-0.1.5/tests/unit/test_LoadData.py` & `SleepHarmonizer-0.2.1/tests/unit/test_LoadData.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.5/tests/unit/test_Plugin.py` & `SleepHarmonizer-0.2.1/tests/unit/test_Plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from unittest import TestCase
 
-from pyPhases import ConfigNotFoundException, Project, pdict
+from pyPhases import Project
+
 from pyPhasesRecordloader import RecordLoader
 from SleepHarmonizer.Plugin import Plugin
 
 
 class TestPlugin(TestCase):
     def setUp(self):
         self.options = {}
         self.project = Project()
-        # self.project.config = pdict({})
+        self.project.config = self.project.loadConfig("SleepHarmonizer/config.yaml")
         self.plugin = Plugin(self.project, self.options)
 
     def test_project_is_extended(self):
         self.assertIn("Export", self.project.phaseMap)
         self.assertIn("LoadData", self.project.phaseMap)
 
         loadDataPhase = self.project.getPhase("LoadData")
```

### Comparing `SleepHarmonizer-0.1.5/tests/unit/test_SignalPreprocessing.py` & `SleepHarmonizer-0.2.1/tests/unit/test_SignalPreprocessing.py`

 * *Files identical despite different names*


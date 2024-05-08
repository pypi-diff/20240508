# Comparing `tmp/hitips-1.0.5.tar.gz` & `tmp/hitips-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hitips-1.0.5.tar", last modified: Fri Apr 26 13:33:54 2024, max compression
+gzip compressed data, was "hitips-1.0.6.tar", last modified: Wed May  8 14:13:23 2024, max compression
```

## Comparing `hitips-1.0.5.tar` & `hitips-1.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-04-26 13:33:54.197115 hitips-1.0.5/
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     1068 2023-11-24 15:47:05.000000 hitips-1.0.5/LICENSE.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)     3843 2024-04-26 13:33:54.197115 hitips-1.0.5/PKG-INFO
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     3138 2024-01-17 17:21:47.000000 hitips-1.0.5/README.md
-drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-04-26 13:33:54.197115 hitips-1.0.5/hitips/
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    50780 2024-03-15 19:28:27.000000 hitips-1.0.5/hitips/Analysis.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    53624 2024-03-15 19:00:28.000000 hitips-1.0.5/hitips/AnalysisGUI.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)   107390 2024-04-22 14:42:35.000000 hitips-1.0.5/hitips/BatchAnalyzer.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    21745 2024-03-11 02:56:27.000000 hitips-1.0.5/hitips/Cell_Spot_Tracker.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    21332 2024-03-15 19:28:11.000000 hitips-1.0.5/hitips/Display.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    19739 2023-10-27 02:34:12.000000 hitips-1.0.5/hitips/DisplayGUI.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    27989 2024-03-11 02:56:27.000000 hitips-1.0.5/hitips/GUI_parameters.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    12590 2023-10-30 16:18:43.000000 hitips-1.0.5/hitips/GridLayout.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     7077 2024-03-11 02:56:27.000000 hitips-1.0.5/hitips/HiTIPS.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    10429 2023-11-28 19:29:52.000000 hitips-1.0.5/hitips/IO_ResourceGUI.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     2053 2023-11-24 18:39:45.000000 hitips-1.0.5/hitips/InputOutput.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)    21275 2024-03-11 02:16:59.000000 hitips-1.0.5/hitips/MetaData_Reader.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)   167336 2022-09-22 05:27:10.000000 hitips-1.0.5/hitips/Roboto-Bold.ttf
--rw-------   0 nciadmin  (1001) nciadmin  (1001)   167000 2022-09-22 05:27:10.000000 hitips-1.0.5/hitips/Roboto-Light.ttf
--rw-------   0 nciadmin  (1001) nciadmin  (1001)        0 2023-11-24 18:59:44.000000 hitips-1.0.5/hitips/__init__.py
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     1773 2021-07-19 16:28:45.000000 hitips-1.0.5/hitips/cell_config.json
--rw-------   0 nciadmin  (1001) nciadmin  (1001)      451 2024-01-09 19:58:56.000000 hitips-1.0.5/hitips/logging_decorator.py
-drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-04-26 13:33:54.197115 hitips-1.0.5/hitips.egg-info/
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)     3843 2024-04-26 13:33:53.000000 hitips-1.0.5/hitips.egg-info/PKG-INFO
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)      598 2024-04-26 13:33:54.000000 hitips-1.0.5/hitips.egg-info/SOURCES.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)        1 2024-04-26 13:33:53.000000 hitips-1.0.5/hitips.egg-info/dependency_links.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)       46 2024-04-26 13:33:54.000000 hitips-1.0.5/hitips.egg-info/entry_points.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)      290 2024-04-26 13:33:54.000000 hitips-1.0.5/hitips.egg-info/requires.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)        7 2024-04-26 13:33:54.000000 hitips-1.0.5/hitips.egg-info/top_level.txt
--rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)       38 2024-04-26 13:33:54.197115 hitips-1.0.5/setup.cfg
--rw-------   0 nciadmin  (1001) nciadmin  (1001)     1728 2024-04-26 13:33:42.000000 hitips-1.0.5/setup.py
+drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-05-08 14:13:23.814766 hitips-1.0.6/
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     1068 2023-11-24 15:47:05.000000 hitips-1.0.6/LICENSE.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)     3843 2024-05-08 14:13:23.814766 hitips-1.0.6/PKG-INFO
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     3138 2024-01-17 17:21:47.000000 hitips-1.0.6/README.md
+drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-05-08 14:13:23.814766 hitips-1.0.6/hitips/
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    50780 2024-03-15 19:28:27.000000 hitips-1.0.6/hitips/Analysis.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    53623 2024-05-06 21:13:43.000000 hitips-1.0.6/hitips/AnalysisGUI.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)   107390 2024-04-22 14:42:35.000000 hitips-1.0.6/hitips/BatchAnalyzer.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    21745 2024-03-11 02:56:27.000000 hitips-1.0.6/hitips/Cell_Spot_Tracker.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    21332 2024-03-15 19:28:11.000000 hitips-1.0.6/hitips/Display.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    19739 2023-10-27 02:34:12.000000 hitips-1.0.6/hitips/DisplayGUI.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    27966 2024-05-07 00:58:49.000000 hitips-1.0.6/hitips/GUI_parameters.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    12501 2024-05-08 14:10:39.000000 hitips-1.0.6/hitips/GridLayout.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     7077 2024-03-11 02:56:27.000000 hitips-1.0.6/hitips/HiTIPS.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    10429 2023-11-28 19:29:52.000000 hitips-1.0.6/hitips/IO_ResourceGUI.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     2053 2023-11-24 18:39:45.000000 hitips-1.0.6/hitips/InputOutput.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)    21275 2024-03-11 02:16:59.000000 hitips-1.0.6/hitips/MetaData_Reader.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)   167336 2022-09-22 05:27:10.000000 hitips-1.0.6/hitips/Roboto-Bold.ttf
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)   167000 2022-09-22 05:27:10.000000 hitips-1.0.6/hitips/Roboto-Light.ttf
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)        0 2023-11-24 18:59:44.000000 hitips-1.0.6/hitips/__init__.py
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     1773 2021-07-19 16:28:45.000000 hitips-1.0.6/hitips/cell_config.json
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)      451 2024-01-09 19:58:56.000000 hitips-1.0.6/hitips/logging_decorator.py
+drwxrwxr-x   0 nciadmin  (1001) nciadmin  (1001)        0 2024-05-08 14:13:23.814766 hitips-1.0.6/hitips.egg-info/
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)     3843 2024-05-08 14:13:23.000000 hitips-1.0.6/hitips.egg-info/PKG-INFO
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)      598 2024-05-08 14:13:23.000000 hitips-1.0.6/hitips.egg-info/SOURCES.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)        1 2024-05-08 14:13:23.000000 hitips-1.0.6/hitips.egg-info/dependency_links.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)       46 2024-05-08 14:13:23.000000 hitips-1.0.6/hitips.egg-info/entry_points.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)      290 2024-05-08 14:13:23.000000 hitips-1.0.6/hitips.egg-info/requires.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)        7 2024-05-08 14:13:23.000000 hitips-1.0.6/hitips.egg-info/top_level.txt
+-rw-rw-r--   0 nciadmin  (1001) nciadmin  (1001)       38 2024-05-08 14:13:23.814766 hitips-1.0.6/setup.cfg
+-rw-------   0 nciadmin  (1001) nciadmin  (1001)     1728 2024-05-08 14:12:47.000000 hitips-1.0.6/setup.py
```

### Comparing `hitips-1.0.5/LICENSE.txt` & `hitips-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/PKG-INFO` & `hitips-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hitips
-Version: 1.0.5
+Version: 1.0.6
 Summary: HiTIPS: High-Throughput Image Processing Software for FISH data analysis
 Home-page: https://github.com/CBIIT/HiTIPS
 Author: keikhosravi
 Author-email: adib.keikhosravi@nih.gov
 License: MIT
 Keywords: high-throughput imaging FISH analysis cell segmentation signal quantification
 Platform: UNKNOWN
```

### Comparing `hitips-1.0.5/README.md` & `hitips-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/Analysis.py` & `hitips-1.0.6/hitips/Analysis.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/AnalysisGUI.py` & `hitips-1.0.6/hitips/AnalysisGUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 if hasattr(QtCore.Qt, 'AA_EnableHighDpiScaling'):
     QtWidgets.QApplication.setAttribute(QtCore.Qt.AA_EnableHighDpiScaling, True)
 
 if hasattr(QtCore.Qt, 'AA_UseHighDpiPixmaps'):
     QtWidgets.QApplication.setAttribute(QtCore.Qt.AA_UseHighDpiPixmaps, True)
 
 
-
 class analyzer(QWidget):
 
     def __init__(self, centralwidget, gridLayout_centralwidget, displaygui=None, ImDisplay=None, image_analyzer=None, gui_params=None):
         super().__init__(centralwidget)
         self.gridLayout_centralwidget = gridLayout_centralwidget
         self.displaygui = displaygui
         self.AnalysisLbl = QtWidgets.QLabel(centralwidget)
```

### Comparing `hitips-1.0.5/hitips/BatchAnalyzer.py` & `hitips-1.0.6/hitips/BatchAnalyzer.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/Cell_Spot_Tracker.py` & `hitips-1.0.6/hitips/Cell_Spot_Tracker.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/Display.py` & `hitips-1.0.6/hitips/Display.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/DisplayGUI.py` & `hitips-1.0.6/hitips/DisplayGUI.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/GUI_parameters.py` & `hitips-1.0.6/hitips/GUI_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,20 @@
         self.IntegratedIntensityCbox_currentIndex = self.AnalysisGui.IntegratedIntensityCbox.currentIndex()
         self.SpotareaminSpinBox_value = self.AnalysisGui.SpotareaminSpinBox.value()
         self.SpotareamaxSpinBox_value = self.AnalysisGui.SpotareamaxSpinBox.value()
         self.SpotIntegratedIntensitySpinBox_value = self.AnalysisGui.SpotIntegratedIntensitySpinBox.value()
         self.PSFsizeSpinBox_value = self.AnalysisGui.PSFsizeSpinBox.value()
         
         self.params_dict = self.gather_analysis_params()
+        # self.UPDATE_SPOT_ANALYSIS_PARAMS()
         
     def gather_analysis_params(self):
-        
+        self.UPDATE_SPOT_ANALYSIS_PARAMS()
         params_dict = {
-            "spot_params_dict": self.INITIALIZE_SPOT_ANALYSIS_PARAMS(),
+            "spot_params_dict": self.spot_params_dict,
             "NucInfoChkBox_check_status": self.AnalysisGui.NucInfoChkBox.isChecked(),
             "SpotsLocation_check_status": self.AnalysisGui.SpotsLocation.isChecked(),
             "Spot_Tracking_check_status": self.AnalysisGui.Spot_Tracking.isChecked(),
             "SpotLocationCbox_currentText": self.AnalysisGui.SpotLocationCbox.currentText(),
             "SpotsDistance_check_status": self.AnalysisGui.SpotsDistance.isChecked(),
             "NucMaskCheckBox_status_check": self.AnalysisGui.NucMaskCheckBox.isChecked(),
             "NucMaxZprojectCheckBox_status_check": self.AnalysisGui.NucMaxZprojectCheckBox.isChecked(),
@@ -205,30 +206,31 @@
 
         if current_channel == 'All':
             self.spot_params_dict = {
                 f"Ch{i}": get_channel_params() for i in range(1, 6)
             }
         elif current_channel in ['Ch1', 'Ch2', 'Ch3', 'Ch4', 'Ch5']:
             self.spot_params_dict[current_channel] = get_channel_params()
+        
             
     def UPDATE_SPOT_ANALYSIS_GUI_PARAMS(self):
 
         current_channel = self.AnalysisGui.spotchannelselect.currentText()
 
         if current_channel in ['Ch1', 'Ch2', 'Ch3', 'Ch4', 'Ch5']:
 
             gui_elements = [
-                self.AnalysisGui.spotanalysismethod,  # QComboBox
-                self.AnalysisGui.thresholdmethod,     # QComboBox
-                self.AnalysisGui.ThresholdSlider,     # QSlider or QSpinBox
-                self.AnalysisGui.SensitivitySpinBox,  # QSpinBox
-                self.AnalysisGui.ResizeFactor,    # QSpinBox
-                self.AnalysisGui.SpotareaminSpinBox,  # QSpinBox
-                self.AnalysisGui.SpotareamaxSpinBox,  # QSpinBox
-                self.AnalysisGui.SpotIntegratedIntensitySpinBox  # QSpinBox
+                self.AnalysisGui.spotanalysismethod,  
+                self.AnalysisGui.thresholdmethod,     
+                self.AnalysisGui.ThresholdSlider,     
+                self.AnalysisGui.SensitivitySpinBox,  
+                self.AnalysisGui.ResizeFactor,    
+                self.AnalysisGui.SpotareaminSpinBox,  
+                self.AnalysisGui.SpotareamaxSpinBox,  
+                self.AnalysisGui.SpotIntegratedIntensitySpinBox 
             ]
 
             for i, gui_element in enumerate(gui_elements):
                 value = np.array(self.spot_params_dict[current_channel][i]).astype(int)
     
                 try:
                     # Attempt to disconnect the signal
```

### Comparing `hitips-1.0.5/hitips/GridLayout.py` & `hitips-1.0.6/hitips/GridLayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         font.setBold(False)
         font.setWeight(10)
         self.tableWidget.setFont(font)
         self.tableWidget.setColumnCount(WELL_PLATE_LENGTH)
         self.tableWidget.setRowCount(WELL_PLATE_WIDTH)
         self.tableWidget.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         
-        # Rest of your code, initializing headers and other widgets...
         for i in range(WELL_PLATE_WIDTH):
             item = QtWidgets.QTableWidgetItem()
             self.tableWidget.setVerticalHeaderItem(i, item)
 
         for i in range(WELL_PLATE_LENGTH):
             item = QtWidgets.QTableWidgetItem()
             self.tableWidget.setHorizontalHeaderItem(i, item)
@@ -97,16 +96,15 @@
         font.setPointSize(8)
         self.Zlist.setFont(font)
         self.Zlist.setVerticalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOn)
         self.Zlist.setBatchSize(80)
         self.Zlist.setObjectName("Zlist")
         self.Zlist.itemClicked.connect(lambda: self.on_click_list(self.ControlPanel.Meta_Data_df,self.ImDisplay, self.displaygui))
         
-        
-        
+
         self.Zlabel = QtWidgets.QLabel(self.groupBox1)
         self.gridLayout_grdigroupbox1.addWidget(self.Zlabel, 1, 2, 1, 1)
         font = QtGui.QFont()
         font.setPointSize(11)
         self.Zlabel.setFont(font)
         self.Zlabel.setObjectName("Zlabel")
         
@@ -277,8 +275,7 @@
     import sys
     app = QtWidgets.QApplication(sys.argv)
     MainWindow = QtWidgets.QMainWindow()
     ui = Ui_MainWindow()
     ui.setupUi(MainWindow)
     MainWindow.show()
     sys.exit(app.exec_())
-
```

### Comparing `hitips-1.0.5/hitips/HiTIPS.py` & `hitips-1.0.6/hitips/HiTIPS.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/IO_ResourceGUI.py` & `hitips-1.0.6/hitips/IO_ResourceGUI.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/InputOutput.py` & `hitips-1.0.6/hitips/InputOutput.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/MetaData_Reader.py` & `hitips-1.0.6/hitips/MetaData_Reader.py`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/Roboto-Bold.ttf` & `hitips-1.0.6/hitips/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/Roboto-Light.ttf` & `hitips-1.0.6/hitips/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips/cell_config.json` & `hitips-1.0.6/hitips/cell_config.json`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/hitips.egg-info/PKG-INFO` & `hitips-1.0.6/hitips.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hitips
-Version: 1.0.5
+Version: 1.0.6
 Summary: HiTIPS: High-Throughput Image Processing Software for FISH data analysis
 Home-page: https://github.com/CBIIT/HiTIPS
 Author: keikhosravi
 Author-email: adib.keikhosravi@nih.gov
 License: MIT
 Keywords: high-throughput imaging FISH analysis cell segmentation signal quantification
 Platform: UNKNOWN
```

### Comparing `hitips-1.0.5/hitips.egg-info/SOURCES.txt` & `hitips-1.0.6/hitips.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hitips-1.0.5/setup.py` & `hitips-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="hitips",
-    version="1.0.5",
+    version="1.0.6",
     author="keikhosravi",
     author_email="adib.keikhosravi@nih.gov",
     description="HiTIPS: High-Throughput Image Processing Software for FISH data analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CBIIT/HiTIPS",
     packages=find_packages(),
```


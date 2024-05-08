# Comparing `tmp/pyqtgraph_ext-1.2.0.tar.gz` & `tmp/pyqtgraph_ext-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqtgraph_ext-1.2.0.tar", last modified: Tue Apr 30 21:46:36 2024, max compression
+gzip compressed data, was "pyqtgraph_ext-1.2.6.tar", last modified: Wed May  8 17:11:29 2024, max compression
```

## Comparing `pyqtgraph_ext-1.2.0.tar` & `pyqtgraph_ext-1.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1077 2024-01-29 19:12:56.810546 pyqtgraph_ext-1.2.0/LICENSE
--rw-r--r--   0        0        0      760 2024-04-24 22:10:53.577243 pyqtgraph_ext-1.2.0/README.md
--rw-r--r--   0        0        0     1202 2024-04-30 21:46:36.453400 pyqtgraph_ext-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     9304 2024-04-30 14:22:23.759075 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegion.py
--rw-r--r--   0        0        0     6764 2024-04-30 14:22:23.759456 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegionTreeItem.py
--rw-r--r--   0        0        0     2579 2024-04-30 14:22:23.759796 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegionTreeModel.py
--rw-r--r--   0        0        0    17198 2024-04-30 14:22:23.760185 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegionTreeView.py
--rw-r--r--   0        0        0     1577 2024-02-19 16:35:28.155322 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Figure.py
--rw-r--r--   0        0        0     6567 2024-04-26 20:37:41.001643 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Graph.py
--rw-r--r--   0        0        0      830 2024-04-26 15:12:20.979202 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Plot.py
--rw-r--r--   0        0        0     6117 2024-04-24 22:09:55.723207 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/PlotGrid.py
--rw-r--r--   0        0        0     6555 2024-04-24 22:10:53.578129 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/View.py
--rw-r--r--   0        0        0      573 2024-04-30 14:22:23.760679 pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/__init__.py
--rw-r--r--   0        0        0        0 2024-01-29 19:12:56.812918 pyqtgraph_ext-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 pyqtgraph_ext-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-29 19:12:56.810546 pyqtgraph_ext-1.2.6/LICENSE
+-rw-r--r--   0        0        0      760 2024-04-24 22:10:53.577243 pyqtgraph_ext-1.2.6/README.md
+-rw-r--r--   0        0        0     1202 2024-05-08 17:11:29.973497 pyqtgraph_ext-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     9304 2024-04-30 14:22:23.759075 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/AxisRegion.py
+-rw-r--r--   0        0        0     6764 2024-04-30 14:22:23.759456 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/AxisRegionTreeItem.py
+-rw-r--r--   0        0        0     2579 2024-04-30 14:22:23.759796 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/AxisRegionTreeModel.py
+-rw-r--r--   0        0        0    17198 2024-04-30 14:22:23.760185 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/AxisRegionTreeView.py
+-rw-r--r--   0        0        0     1577 2024-02-19 16:35:28.155322 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/Figure.py
+-rw-r--r--   0        0        0     7892 2024-05-08 17:01:24.583558 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/Graph.py
+-rw-r--r--   0        0        0      830 2024-04-26 15:12:20.979202 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/Plot.py
+-rw-r--r--   0        0        0     6117 2024-04-24 22:09:55.723207 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/PlotGrid.py
+-rw-r--r--   0        0        0     6555 2024-04-24 22:10:53.578129 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/View.py
+-rw-r--r--   0        0        0      573 2024-04-30 14:22:23.760679 pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-29 19:12:56.812918 pyqtgraph_ext-1.2.6/tests/__init__.py
+-rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 pyqtgraph_ext-1.2.6/PKG-INFO
```

### Comparing `pyqtgraph_ext-1.2.0/LICENSE` & `pyqtgraph_ext-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/README.md` & `pyqtgraph_ext-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/pyproject.toml` & `pyqtgraph_ext-1.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 requires-python = ">=3.9"
 dependencies = [
     "numpy>=1.26.2",
     "qtpy>=2.4.1",
     "qtawesome>=1.3.0",
     "pyqtgraph>=0.13.3",
-    "pyqt-ext>=1.1.0",
+    "pyqt-ext>=1.2.5",
 ]
 readme = "README.md"
 keywords = [
     "PyQt",
     "PySide",
     "pyqtgraph",
 ]
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "1.2.0"
+version = "1.2.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/pyqtgraph-ext"
 repository = "https://github.com/marcel-goldschen-ohm/pyqtgraph-ext"
```

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegion.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/AxisRegion.py`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegionTreeItem.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/AxisRegionTreeItem.py`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegionTreeModel.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/AxisRegionTreeModel.py`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/AxisRegionTreeView.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/AxisRegionTreeView.py`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Figure.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/Figure.py`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Graph.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/Graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 from qtpy.QtCore import *
 from qtpy.QtGui import *
 from qtpy.QtWidgets import *
 import pyqtgraph as pg
 from pyqt_ext.utils import toQColor
 from pyqt_ext.graph import GraphStyle, editGraphStyle
+from pyqt_ext.widgets import TableWidgetWithCopyPaste
 
 
 class Graph(pg.PlotDataItem):
     """ PlotDataItem with custom context menu and style dialog. """
 
     sigNameChanged = Signal(str)
 
@@ -67,14 +68,16 @@
     def getContextMenus(self, event=None):
         name = self.name()
         if name is None:
             name = self.__class__.__name__
         self._thisItemMenu = QMenu(name)
         # self._thisItemMenu.addAction('Rename')
         # self._thisItemMenu.addSeparator()
+        self._thisItemMenu.addAction('Data table', self.dataDialog)
+        self._thisItemMenu.addSeparator()
         self._thisItemMenu.addAction('Style', self.styleDialog)
         # self._thisItemMenu.addSeparator()
         # self._thisItemMenu.addAction('Hide', lambda: self.setVisible(False))
         # self._thisItemMenu.addSeparator()
         # self._thisItemMenu.addAction('Delete', lambda: self.getViewBox().deleteItem(self))
 
         self.menu = QMenu()
@@ -175,7 +178,36 @@
         if name is None:
             name = self.__class__.__name__
         old_style: GraphStyle = self.graphStyle()
         new_style: GraphStyle | None = editGraphStyle(old_style, parent = self.getViewBox().getViewWidget(), title = name)
         if new_style is None:
             return
         self.setGraphStyle(new_style)
+    
+    def dataDialog(self):
+        dlg = QDialog()
+        dlg.setWindowTitle(self.name())
+        vbox = QVBoxLayout(dlg)
+        vbox.setContentsMargins(0, 0, 0, 0)
+        vbox.setSpacing(0)
+        xdata, ydata = self.getOriginalDataset()
+        n_rows = len(ydata)
+        n_cols = 2
+        table = TableWidgetWithCopyPaste(n_rows, n_cols)
+        for row in range(n_rows):
+            table.setItem(row, 0, QTableWidgetItem(str(xdata[row])))
+            table.setItem(row, 1, QTableWidgetItem(str(ydata[row])))
+        table.setEditTriggers(QAbstractItemView.NoEditTriggers)
+        xaxis = self.getViewBox().parentWidget().getAxis('bottom')
+        yaxis = self.getViewBox().parentWidget().getAxis('left')
+        xlabel = xaxis.labelText
+        if xaxis.labelUnits:
+            xlabel += f' ({xaxis.labelUnits})'
+        ylabel = yaxis.labelText
+        if yaxis.labelUnits:
+            ylabel += f' ({yaxis.labelUnits})'
+        table.setHorizontalHeaderLabels([xlabel, ylabel])
+        for col in range(n_cols):
+            table.resizeColumnToContents(col)
+        table.resizeRowsToContents()
+        vbox.addWidget(table)
+        dlg.exec()
```

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/Plot.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/Plot.py`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/PlotGrid.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/PlotGrid.py`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/View.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/View.py`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/src/pyqtgraph_ext/__init__.py` & `pyqtgraph_ext-1.2.6/src/pyqtgraph_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtgraph_ext-1.2.0/PKG-INFO` & `pyqtgraph_ext-1.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtgraph-ext
-Version: 1.2.0
+Version: 1.2.6
 Summary: Collection of PyQtGraph widgets/tools.
 Keywords: PyQt,PySide,pyqtgraph
 Home-page: https://github.com/marcel-goldschen-ohm/pyqtgraph-ext
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Project-URL: Homepage, https://github.com/marcel-goldschen-ohm/pyqtgraph-ext
 Project-URL: Repository, https://github.com/marcel-goldschen-ohm/pyqtgraph-ext
 Requires-Python: >=3.9
 Requires-Dist: numpy>=1.26.2
 Requires-Dist: qtpy>=2.4.1
 Requires-Dist: qtawesome>=1.3.0
 Requires-Dist: pyqtgraph>=0.13.3
-Requires-Dist: pyqt-ext>=1.1.0
+Requires-Dist: pyqt-ext>=1.2.5
 Description-Content-Type: text/markdown
 
 # pyqtgraph-ext
 Collection of [PyQtGraph](https://www.pyqtgraph.org) widgets/tools with custom styling or behavior.
 
 - [Install](#install)
 - [AxisRegion](#axisregion)
```


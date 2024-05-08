# Comparing `tmp/pyqt_ext-1.2.3.tar.gz` & `tmp/pyqt_ext-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt_ext-1.2.3.tar", last modified: Tue May  7 19:57:30 2024, max compression
+gzip compressed data, was "pyqt_ext-1.2.5.tar", last modified: Wed May  8 17:11:06 2024, max compression
```

## Comparing `pyqt_ext-1.2.3.tar` & `pyqt_ext-1.2.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1077 2024-01-29 19:11:38.968151 pyqt_ext-1.2.3/LICENSE
--rw-r--r--   0        0        0      637 2024-05-07 14:26:09.378718 pyqt_ext-1.2.3/README.md
--rw-r--r--   0        0        0     1123 2024-05-07 19:57:30.241316 pyqt_ext-1.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 18:05:49.614382 pyqt_ext-1.2.3/src/pyqt_ext/__init__.py
--rw-r--r--   0        0        0    15661 2024-04-30 21:40:30.459705 pyqt_ext-1.2.3/src/pyqt_ext/graph/GraphStyle.py
--rw-r--r--   0        0        0       81 2024-02-26 18:05:49.615491 pyqt_ext-1.2.3/src/pyqt_ext/graph/__init__.py
--rw-r--r--   0        0        0     4933 2024-02-26 18:05:49.616028 pyqt_ext-1.2.3/src/pyqt_ext/tmp/Chart.py
--rw-r--r--   0        0        0    14436 2024-04-23 20:40:53.301852 pyqt_ext-1.2.3/src/pyqt_ext/tree/AbstractTreeItem.py
--rw-r--r--   0        0        0    14629 2024-04-22 17:42:52.732350 pyqt_ext-1.2.3/src/pyqt_ext/tree/AbstractTreeModel.py
--rw-r--r--   0        0        0     6553 2024-03-04 20:57:48.587337 pyqt_ext-1.2.3/src/pyqt_ext/tree/KeyValueTreeItem.py
--rw-r--r--   0        0        0     2896 2024-02-26 18:33:33.713144 pyqt_ext-1.2.3/src/pyqt_ext/tree/KeyValueTreeModel.py
--rw-r--r--   0        0        0     3501 2024-03-04 20:57:48.587786 pyqt_ext-1.2.3/src/pyqt_ext/tree/KeyValueTreeView.py
--rw-r--r--   0        0        0    11058 2024-05-07 15:42:00.614650 pyqt_ext-1.2.3/src/pyqt_ext/tree/TreeView.py
--rw-r--r--   0        0        0      392 2024-02-26 18:05:49.619082 pyqt_ext-1.2.3/src/pyqt_ext/tree/__init__.py
--rw-r--r--   0        0        0     1624 2024-04-25 15:58:28.549088 pyqt_ext-1.2.3/src/pyqt_ext/utils/Color.py
--rw-r--r--   0        0        0       64 2024-02-26 18:05:49.619812 pyqt_ext-1.2.3/src/pyqt_ext/utils/__init__.py
--rw-r--r--   0        0        0     5452 2024-04-23 18:11:10.293878 pyqt_ext-1.2.3/src/pyqt_ext/widgets/CollapsibleSection.py
--rw-r--r--   0        0        0     2415 2024-02-29 22:56:53.609934 pyqt_ext-1.2.3/src/pyqt_ext/widgets/ColorButton.py
--rw-r--r--   0        0        0    11804 2024-05-03 14:12:30.627760 pyqt_ext-1.2.3/src/pyqt_ext/widgets/MultiValueSpinBox.py
--rw-r--r--   0        0        0      184 2024-03-05 15:06:04.507342 pyqt_ext-1.2.3/src/pyqt_ext/widgets/__init__.py
--rw-r--r--   0        0        0        0 2024-01-29 19:11:38.971696 pyqt_ext-1.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1642 1970-01-01 00:00:00.000000 pyqt_ext-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-29 19:11:38.968151 pyqt_ext-1.2.5/LICENSE
+-rw-r--r--   0        0        0      637 2024-05-07 14:26:09.378718 pyqt_ext-1.2.5/README.md
+-rw-r--r--   0        0        0     1123 2024-05-08 17:11:06.810464 pyqt_ext-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-26 18:05:49.614382 pyqt_ext-1.2.5/src/pyqt_ext/__init__.py
+-rw-r--r--   0        0        0    15661 2024-04-30 21:40:30.459705 pyqt_ext-1.2.5/src/pyqt_ext/graph/GraphStyle.py
+-rw-r--r--   0        0        0       81 2024-02-26 18:05:49.615491 pyqt_ext-1.2.5/src/pyqt_ext/graph/__init__.py
+-rw-r--r--   0        0        0     4933 2024-02-26 18:05:49.616028 pyqt_ext-1.2.5/src/pyqt_ext/tmp/Chart.py
+-rw-r--r--   0        0        0    14436 2024-04-23 20:40:53.301852 pyqt_ext-1.2.5/src/pyqt_ext/tree/AbstractTreeItem.py
+-rw-r--r--   0        0        0    14629 2024-04-22 17:42:52.732350 pyqt_ext-1.2.5/src/pyqt_ext/tree/AbstractTreeModel.py
+-rw-r--r--   0        0        0     6553 2024-03-04 20:57:48.587337 pyqt_ext-1.2.5/src/pyqt_ext/tree/KeyValueTreeItem.py
+-rw-r--r--   0        0        0     2896 2024-02-26 18:33:33.713144 pyqt_ext-1.2.5/src/pyqt_ext/tree/KeyValueTreeModel.py
+-rw-r--r--   0        0        0     3501 2024-03-04 20:57:48.587786 pyqt_ext-1.2.5/src/pyqt_ext/tree/KeyValueTreeView.py
+-rw-r--r--   0        0        0    11058 2024-05-07 15:42:00.614650 pyqt_ext-1.2.5/src/pyqt_ext/tree/TreeView.py
+-rw-r--r--   0        0        0      392 2024-02-26 18:05:49.619082 pyqt_ext-1.2.5/src/pyqt_ext/tree/__init__.py
+-rw-r--r--   0        0        0     1624 2024-04-25 15:58:28.549088 pyqt_ext-1.2.5/src/pyqt_ext/utils/Color.py
+-rw-r--r--   0        0        0       64 2024-02-26 18:05:49.619812 pyqt_ext-1.2.5/src/pyqt_ext/utils/__init__.py
+-rw-r--r--   0        0        0     5452 2024-04-23 18:11:10.293878 pyqt_ext-1.2.5/src/pyqt_ext/widgets/CollapsibleSection.py
+-rw-r--r--   0        0        0     2415 2024-02-29 22:56:53.609934 pyqt_ext-1.2.5/src/pyqt_ext/widgets/ColorButton.py
+-rw-r--r--   0        0        0    11804 2024-05-03 14:12:30.627760 pyqt_ext-1.2.5/src/pyqt_ext/widgets/MultiValueSpinBox.py
+-rw-r--r--   0        0        0     2240 2024-05-08 16:52:37.320968 pyqt_ext-1.2.5/src/pyqt_ext/widgets/TableWidgetWithCopyPaste.py
+-rw-r--r--   0        0        0      263 2024-05-08 16:52:58.378411 pyqt_ext-1.2.5/src/pyqt_ext/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-29 19:11:38.971696 pyqt_ext-1.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     1642 1970-01-01 00:00:00.000000 pyqt_ext-1.2.5/PKG-INFO
```

### Comparing `pyqt_ext-1.2.3/LICENSE` & `pyqt_ext-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/README.md` & `pyqt_ext-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/pyproject.toml` & `pyqt_ext-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "1.2.3"
+version = "1.2.5"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/pyqt-ext"
 repository = "https://github.com/marcel-goldschen-ohm/pyqt-ext"
```

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/graph/GraphStyle.py` & `pyqt_ext-1.2.5/src/pyqt_ext/graph/GraphStyle.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/tmp/Chart.py` & `pyqt_ext-1.2.5/src/pyqt_ext/tmp/Chart.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/tree/AbstractTreeItem.py` & `pyqt_ext-1.2.5/src/pyqt_ext/tree/AbstractTreeItem.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/tree/AbstractTreeModel.py` & `pyqt_ext-1.2.5/src/pyqt_ext/tree/AbstractTreeModel.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/tree/KeyValueTreeItem.py` & `pyqt_ext-1.2.5/src/pyqt_ext/tree/KeyValueTreeItem.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/tree/KeyValueTreeModel.py` & `pyqt_ext-1.2.5/src/pyqt_ext/tree/KeyValueTreeModel.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/tree/KeyValueTreeView.py` & `pyqt_ext-1.2.5/src/pyqt_ext/tree/KeyValueTreeView.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/tree/TreeView.py` & `pyqt_ext-1.2.5/src/pyqt_ext/tree/TreeView.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/utils/Color.py` & `pyqt_ext-1.2.5/src/pyqt_ext/utils/Color.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/widgets/CollapsibleSection.py` & `pyqt_ext-1.2.5/src/pyqt_ext/widgets/CollapsibleSection.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/widgets/ColorButton.py` & `pyqt_ext-1.2.5/src/pyqt_ext/widgets/ColorButton.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/src/pyqt_ext/widgets/MultiValueSpinBox.py` & `pyqt_ext-1.2.5/src/pyqt_ext/widgets/MultiValueSpinBox.py`

 * *Files identical despite different names*

### Comparing `pyqt_ext-1.2.3/PKG-INFO` & `pyqt_ext-1.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqt-ext
-Version: 1.2.3
+Version: 1.2.5
 Summary: Collection of PyQt/PySide widgets/tools
 Keywords: PyQt,PySide
 Home-page: https://github.com/marcel-goldschen-ohm/pyqt-ext
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


# Comparing `tmp/xarray_treeview-1.2.2.tar.gz` & `tmp/xarray_treeview-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_treeview-1.2.2.tar", last modified: Mon May  6 21:12:49 2024, max compression
+gzip compressed data, was "xarray_treeview-1.2.3.tar", last modified: Tue May  7 19:57:48 2024, max compression
```

## Comparing `xarray_treeview-1.2.2.tar` & `xarray_treeview-1.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2024-01-11 16:04:45.274505 xarray_treeview-1.2.2/LICENSE
--rw-r--r--   0        0        0      210 2024-01-29 19:36:00.736104 xarray_treeview-1.2.2/README.md
--rw-r--r--   0        0        0     1261 2024-05-06 21:12:49.447039 xarray_treeview-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     7781 2024-05-02 17:20:29.148732 xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeItem.py
--rw-r--r--   0        0        0     5999 2024-05-02 18:10:19.300488 xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeModel.py
--rw-r--r--   0        0        0    10751 2024-05-02 18:19:08.766975 xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeView.py
--rw-r--r--   0        0        0     3977 2024-05-02 18:19:50.460886 xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeViewer.py
--rw-r--r--   0        0        0      257 2024-05-02 18:13:58.486880 xarray_treeview-1.2.2/src/xarray_treeview/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 16:04:45.276303 xarray_treeview-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 xarray_treeview-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-11 16:04:45.274505 xarray_treeview-1.2.3/LICENSE
+-rw-r--r--   0        0        0      210 2024-01-29 19:36:00.736104 xarray_treeview-1.2.3/README.md
+-rw-r--r--   0        0        0     1261 2024-05-07 19:57:48.301854 xarray_treeview-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7711 2024-05-07 19:08:47.993454 xarray_treeview-1.2.3/src/xarray_treeview/XarrayTreeItem.py
+-rw-r--r--   0        0        0     6066 2024-05-07 19:08:53.403187 xarray_treeview-1.2.3/src/xarray_treeview/XarrayTreeModel.py
+-rw-r--r--   0        0        0     7709 2024-05-07 15:43:52.040405 xarray_treeview-1.2.3/src/xarray_treeview/XarrayTreeView.py
+-rw-r--r--   0        0        0     3977 2024-05-02 18:19:50.460886 xarray_treeview-1.2.3/src/xarray_treeview/XarrayTreeViewer.py
+-rw-r--r--   0        0        0      257 2024-05-02 18:13:58.486880 xarray_treeview-1.2.3/src/xarray_treeview/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 16:04:45.276303 xarray_treeview-1.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 xarray_treeview-1.2.3/PKG-INFO
```

### Comparing `xarray_treeview-1.2.2/LICENSE` & `xarray_treeview-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_treeview-1.2.2/pyproject.toml` & `xarray_treeview-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "1.2.2"
+version = "1.2.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/xarray-treeview"
 repository = "https://github.com/marcel-goldschen-ohm/xarray-treeview"
```

### Comparing `xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeItem.py` & `xarray_treeview-1.2.3/src/xarray_treeview/XarrayTreeItem.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,14 @@
                 new_parent_node: DataTree | None = parent.node if parent is not None else None
                 if self.node.parent is not new_parent_node:
                     self.node.orphan()
             if parent is not None:
                 if self.node.parent is not parent.node:
                     self.node.parent = parent.node
         elif self.is_var() or self.is_coord():
-            # if parent is None:
-            #     # delete var/coord
             old_node: DataTree = self.node
             new_node: DataTree = parent.node if parent is not None else DataTree(name=self.name)
             if new_node is not old_node:
                 if self.is_var():
                     new_node.ds = new_node.to_dataset().assign({self.key: old_node[self.key]})
                 elif self.is_coord():
                     new_node.ds = new_node.to_dataset().assign_coords({self.key: old_node[self.key]})
```

### Comparing `xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeModel.py` & `xarray_treeview-1.2.3/src/xarray_treeview/XarrayTreeModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,18 @@
             flags |= Qt.ItemFlag.ItemIsSelectable
         elif item.is_var() and 'var' in self.allowedSelections():
             flags |= Qt.ItemFlag.ItemIsSelectable
         elif item.is_coord() and 'coord' in self.allowedSelections():
             flags |= Qt.ItemFlag.ItemIsSelectable
         # drag and drop
         if self.supportedDropActions() != Qt.DropAction.IgnoreAction:
-            # if item.is_node():
-            flags |= Qt.ItemFlag.ItemIsDragEnabled | Qt.ItemFlag.ItemIsDropEnabled
+            flags |= Qt.ItemFlag.ItemIsDragEnabled
+            if item.is_node():
+                # can only drop on node items
+                flags |= Qt.ItemFlag.ItemIsDropEnabled
         return flags
 
     def data(self, index: QModelIndex, role: int):
         if not index.isValid():
             return
         item: XarrayTreeItem = self.itemFromIndex(index)
         if role == Qt.ItemDataRole.DisplayRole or role == Qt.ItemDataRole.EditRole:
```

### Comparing `xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeView.py` & `xarray_treeview-1.2.3/src/xarray_treeview/XarrayTreeView.py`

 * *Files 26% similar despite different names*

```diff
@@ -167,84 +167,14 @@
 
         dlg = QDialog(self)
         dlg.setWindowTitle(item.path)
         layout = QVBoxLayout(dlg)
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(textEdit)
         dlg.exec()
-    
-    def dropEvent(self, event: QDropEvent):
-        src_index: QModelIndex = getattr(self, '_src_index', None)
-        if (src_index is None) or (not src_index.isValid()) or (src_index == QModelIndex()):
-            event.ignore()
-            return
-        dst_index: QModelIndex = self.indexAt(event.pos())
-        
-        model: XarrayTreeModel = self.model()
-        src_parent_index: QModelIndex = model.parent(src_index)
-        src_row = src_index.row()
-        dst_parent_index: QModelIndex = model.parent(dst_index)
-        dst_row = dst_index.row()
-
-        drop_pos = self.dropIndicatorPosition()
-        if drop_pos == QAbstractItemView.DropIndicatorPosition.OnViewport:
-            dst_parent_index = QModelIndex()
-            dst_row = model.rowCount(dst_parent_index)
-        elif drop_pos == QAbstractItemView.DropIndicatorPosition.OnItem:
-            dst_item = model.itemFromIndex(dst_index)
-            if dst_item.is_node():
-                dst_parent_index = dst_index
-                dst_row = model.rowCount(dst_parent_index)
-            elif dst_item.is_var():
-                pass # handle drops on vars?
-            elif dst_item.is_coord():
-                pass # handle drops on coords?
-        elif drop_pos == QAbstractItemView.DropIndicatorPosition.AboveItem:
-            pass
-        elif drop_pos == QAbstractItemView.DropIndicatorPosition.BelowItem:
-            dst_row += 1
-        
-        # organize child order: vars, coords, nodes
-        src_item = model.itemFromIndex(model.index(src_row, 0, src_parent_index))
-        if src_item.is_var():
-            while dst_row > 0:
-                dst_prev_item = model.itemFromIndex(model.index(dst_row - 1, 0, dst_parent_index))
-                if dst_prev_item.is_var():
-                    break
-                dst_row -= 1
-        elif src_item.is_coord():
-            while dst_row > 0:
-                dst_prev_item = model.itemFromIndex(model.index(dst_row - 1, 0, dst_parent_index))
-                if dst_prev_item.is_var() or dst_prev_item.is_coord():
-                    break
-                dst_row -= 1
-            while dst_row < model.rowCount(dst_parent_index):
-                dst_next_item = model.itemFromIndex(model.index(dst_row, 0, dst_parent_index))
-                if dst_next_item.is_coord() or dst_next_item.is_node():
-                    break
-                dst_row += 1
-        elif src_item.is_node():
-            while dst_row < model.rowCount(dst_parent_index):
-                dst_next_item = model.itemFromIndex(model.index(dst_row, 0, dst_parent_index))
-                if dst_next_item.is_node():
-                    break
-                dst_row += 1
-        
-        if event.dropAction() == Qt.DropAction.MoveAction:
-            model.moveRow(src_parent_index, src_row, dst_parent_index, dst_row)
-        else:
-            event.ignore()
-            return
-
-        # We already handled the drop event, so ignore the default implementation.
-        event.setDropAction(Qt.DropAction.IgnoreAction)
-        event.accept()
-
-        # debug
-        # print(model.root().dumps())
 
 
 def test_live():
     import numpy as np
     from xarray_treeview import XarrayDndTreeModel
     app = QApplication()
 
@@ -282,14 +212,15 @@
     baselined_node = DataTree(name='baselined', data=baselined_ds, parent=raw_node)
     scaled_node = DataTree(name='scaled', data=scaled_ds, parent=baselined_node)
     # print('-----\n', root_node.to_datatree())
 
     root_item = XarrayTreeItem(root_node)
     model = XarrayDndTreeModel(root_item)
     view = XarrayTreeView()
+    view.setSelectionMode(QAbstractItemView.ExtendedSelection)
     view.setModel(model)
     view.show()
     view.resize(QSize(600, 600))
     view.expandAll()
     view.resizeAllColumnsToContents()
 
     app.exec()
```

### Comparing `xarray_treeview-1.2.2/src/xarray_treeview/XarrayTreeViewer.py` & `xarray_treeview-1.2.3/src/xarray_treeview/XarrayTreeViewer.py`

 * *Files identical despite different names*

### Comparing `xarray_treeview-1.2.2/PKG-INFO` & `xarray_treeview-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-treeview
-Version: 1.2.2
+Version: 1.2.3
 Summary: PyQt/PySide model/view for tree of Xarray datasets.
 Keywords: PyQt,PySide,xarray,tree
 Home-page: https://github.com/marcel-goldschen-ohm/xarray-treeview
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


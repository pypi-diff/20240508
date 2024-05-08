# Comparing `tmp/xarray_graph-0.2.3.tar.gz` & `tmp/xarray_graph-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_graph-0.2.3.tar", last modified: Tue May  7 19:58:05 2024, max compression
+gzip compressed data, was "xarray_graph-0.2.4.tar", last modified: Tue May  7 21:51:04 2024, max compression
```

## Comparing `xarray_graph-0.2.3.tar` & `xarray_graph-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-01-11 15:44:26.780358 xarray_graph-0.2.3/LICENSE
--rw-r--r--   0        0        0      238 2024-04-30 22:54:33.783557 xarray_graph-0.2.3/README.md
--rw-r--r--   0        0        0     1393 2024-05-07 19:58:05.303616 xarray_graph-0.2.3/pyproject.toml
--rw-r--r--   0        0        0   102020 2024-05-07 19:50:51.521706 xarray_graph-0.2.3/src/xarray_graph/XarrayGraph.py
--rw-r--r--   0        0        0       48 2024-01-11 15:44:26.782449 xarray_graph-0.2.3/src/xarray_graph/__init__.py
--rw-r--r--   0        0        0     2274 2024-04-30 22:51:19.174738 xarray_graph-0.2.3/src/xarray_graph/__main__.py
--rw-r--r--   0        0        0     1841 2024-04-30 14:22:30.897258 xarray_graph-0.2.3/src/xarray_graph/tmp/RegionsManager.py
--rw-r--r--   0        0        0        0 2024-01-11 15:44:26.782628 xarray_graph-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 xarray_graph-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-01-11 15:44:26.780358 xarray_graph-0.2.4/LICENSE
+-rw-r--r--   0        0        0      238 2024-04-30 22:54:33.783557 xarray_graph-0.2.4/README.md
+-rw-r--r--   0        0        0     1393 2024-05-07 21:51:04.746069 xarray_graph-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0   101400 2024-05-07 21:49:38.144618 xarray_graph-0.2.4/src/xarray_graph/XarrayGraph.py
+-rw-r--r--   0        0        0       48 2024-01-11 15:44:26.782449 xarray_graph-0.2.4/src/xarray_graph/__init__.py
+-rw-r--r--   0        0        0     2274 2024-04-30 22:51:19.174738 xarray_graph-0.2.4/src/xarray_graph/__main__.py
+-rw-r--r--   0        0        0     1841 2024-04-30 14:22:30.897258 xarray_graph-0.2.4/src/xarray_graph/tmp/RegionsManager.py
+-rw-r--r--   0        0        0        0 2024-01-11 15:44:26.782628 xarray_graph-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 xarray_graph-0.2.4/PKG-INFO
```

### Comparing `xarray_graph-0.2.3/LICENSE` & `xarray_graph-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.2.3/pyproject.toml` & `xarray_graph-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
 ]
-version = "0.2.3"
+version = "0.2.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/marcel-goldschen-ohm/xarray-graph"
 repository = "https://github.com/marcel-goldschen-ohm/xarray-graph"
```

### Comparing `xarray_graph-0.2.3/src/xarray_graph/XarrayGraph.py` & `xarray_graph-0.2.4/src/xarray_graph/XarrayGraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         # regions tree view
         self._region_treeview.model().setRoot(AxisRegionTreeItem(self.regions))
 
         # notes
         self._notes_edit.setPlainText(self.attrs.get('notes', ''))
 
         # populate array math selections
-        # self._update_array_math_comboboxes()
+        self._update_array_math_comboboxes()
     
     @property
     def dims(self) -> list[str]:
         dims = []
         for node in self.data.subtree:
             for dim in node.dims:
                 if dim not in dims:
@@ -1187,15 +1187,15 @@
         self._math_rhs_combobox.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred)
 
         self._math_operator_combobox = QComboBox()
         self._math_operator_combobox.addItems(['+', '-', '*', '/'])
         self._math_operator_combobox.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Preferred)
 
         self._math_eval_button = QPushButton('Evaluate')
-        # self._math_eval_button.clicked.connect(self.eval_array_math)
+        self._math_eval_button.pressed.connect(self.eval_array_math)
 
         math_group = QGroupBox('Array math')
         grid = QGridLayout(math_group)
         grid.setContentsMargins(3, 3, 3, 3)
         grid.setSpacing(5)
         grid.addWidget(self._math_result_name_edit, 0, 0, 1, 2)
         equals_label = QLabel('=')
@@ -1508,21 +1508,14 @@
         scroll_area = QScrollArea()
         scroll_area.setFrameShape(QFrame.NoFrame)
         scroll_area.setWidget(panel)
         scroll_area.setWidgetResizable(True)
 
         self._control_panel.addWidget(scroll_area)
     
-    # def _show_region_context_menu(self, pos: QPoint) -> None:
-    #     if not hasattr(self, '_region_button_menu'):
-    #         self._region_button_menu = QMenu()
-    #     menu = QMenu()
-    #     menu.addAction('Draw X-axis regions until unchecked', self.clear_regions)
-    #     menu.exec(self.sender().mapToGlobal(pos))
-    
     def _set_region_drawing_mode(self, draw: bool | None = None) -> None:
         if draw is None:
             draw = self._region_button.isChecked()
         self._region_button.setChecked(draw)
         
         try:
             rowmin, rowmax = self._grid_rowlim
@@ -1663,65 +1656,56 @@
     def _update_item_font(self):
         for plot in self.plots():
             view: View = plot.getViewBox()
             for item in view.allChildren():
                 if isinstance(item, XAxisRegion):
                     item.setFontSize(self._textitem_fontsize_spinbox.value())
 
-    # def _update_array_math_comboboxes(self) -> None:
-    #     var_items = []
-    #     item = self._data_treeview.model().root
-    #     while item is not None:
-    #         if item.is_var():
-    #             var_items += [item.name_from_path(maxchar=100)]
-    #         item = item.next_depth_first()
-    #     self._math_lhs_combobox.clear()
-    #     self._math_rhs_combobox.clear()
-    #     self._math_lhs_combobox.addItems(var_items)
-    #     self._math_rhs_combobox.addItems(var_items)
-    
-    # def eval_array_math(self) -> None:
-    #     var_items = []
-    #     item = self._data_treeview.model().root
-    #     while item is not None:
-    #         if item.is_var():
-    #             var_items += [item]
-    #         item = item.next_depth_first()
-    #     lhs_item = var_items[self._math_lhs_combobox.currentIndex()]
-    #     rhs_item = var_items[self._math_rhs_combobox.currentIndex()]
-    #     lhs: xr.DataArray = lhs_item.node.inherited_data(lhs_item.key)
-    #     rhs: xr.DataArray = rhs_item.node.inherited_data(rhs_item.key)
-    #     op = self._math_operator_combobox.currentText()
-    #     # TODO: limit vars to the intersection of their coords
-    #     if op == '+':
-    #         result = lhs + rhs
-    #     elif op == '-':
-    #         result = lhs - rhs
-    #     elif op == '*':
-    #         result = lhs * rhs
-    #     elif op == '/':
-    #         result = lhs / rhs
-    #     # append result as child of lhs_item
-    #     # TODO: handle result name collisions
-    #     result_name = self._math_result_name_edit.text().strip()
-    #     ds = xr.Dataset(data_vars={result.name: result})
-    #     result_node = XarrayTreeNode(name=result_name, dataset=ds, parent=lhs_item.node)
-        
-    #     # update data tree
-    #     self.data = self.data
-
-    #     # make sure newly added node is selected and expanded
-    #     model: XarrayTreeModel = self._data_treeview.model()
-    #     item: XarrayTreeItem = model.root
-    #     while item is not None:
-    #         if item.node is result_node and item.is_var():
-    #             index: QModelIndex = model.createIndex(item.row(), 0, item)
-    #             self._data_treeview.selectionModel().select(index, QItemSelectionModel.SelectionFlag.Select | QItemSelectionModel.SelectionFlag.Rows)
-    #             self._data_treeview.setExpanded(model.parent(index), True)
-    #         item = item.next_depth_first()
+    def _update_array_math_comboboxes(self) -> None:
+        var_paths = [item.path for item in self._data_treeview.model().root().depth_first() if item.is_var()]
+        for i in range(len(var_paths)):
+            if len(var_paths[i]) > 100:
+                var_paths[i] = '...' + var_paths[i][-97:]
+        self._math_lhs_combobox.clear()
+        self._math_rhs_combobox.clear()
+        self._math_lhs_combobox.addItems(var_paths)
+        self._math_rhs_combobox.addItems(var_paths)
+    
+    def eval_array_math(self) -> None:
+        var_items = [item for item in self._data_treeview.model().root().depth_first() if item.is_var()]
+        lhs_item = var_items[self._math_lhs_combobox.currentIndex()]
+        rhs_item = var_items[self._math_rhs_combobox.currentIndex()]
+        lhs: xr.DataArray = lhs_item.node[lhs_item.key]
+        rhs: xr.DataArray = rhs_item.node[rhs_item.key]
+        op = self._math_operator_combobox.currentText()
+        if op == '+':
+            result = lhs + rhs
+        elif op == '-':
+            result = lhs - rhs
+        elif op == '*':
+            result = lhs * rhs
+        elif op == '/':
+            result = lhs / rhs
+        # append result as child of lhs_item
+        result_name = self._math_result_name_edit.text().strip()
+        if result_name == '':
+            result_name = self._math_result_name_edit.placeholderText()
+        result_ds = xr.Dataset(data_vars={result.name: result})
+        result_node = DataTree(name=result_name, data=result_ds, parent=lhs_item.node)
+        
+        # update data tree
+        self.data = self.data
+
+        # make sure newly added fit nodes are selected and expanded
+        model: XarrayTreeModel = self._data_treeview.model()
+        for item in model.root().depth_first():
+            if item.node is result_node and item.is_var():
+                index: QModelIndex = model.createIndex(item.sibling_index, 0, item)
+                self._data_treeview.selectionModel().select(index, QItemSelectionModel.SelectionFlag.Select | QItemSelectionModel.SelectionFlag.Rows)
+                self._data_treeview.setExpanded(model.parent(index), True)
     
     # # @Slot()
     # # def on_axes_item_changed(self):
     # #     item = self.sender()
     # #     if isinstance(item, XAxisRegion):
     # #         item._data['group'] = item.group()
     # #         item._data['region'] = list(item.getRegion())
```

### Comparing `xarray_graph-0.2.3/src/xarray_graph/__main__.py` & `xarray_graph-0.2.4/src/xarray_graph/__main__.py`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.2.3/src/xarray_graph/tmp/RegionsManager.py` & `xarray_graph-0.2.4/src/xarray_graph/tmp/RegionsManager.py`

 * *Files identical despite different names*

### Comparing `xarray_graph-0.2.3/PKG-INFO` & `xarray_graph-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-graph
-Version: 0.2.3
+Version: 0.2.4
 Summary: PyQt/PySide UI for graphing (x,y) slices of Xarray datasets.
 Keywords: PyQt,PySide,xarray,graph
 Home-page: https://github.com/marcel-goldschen-ohm/xarray-graph
 Author-Email: Marcel Goldschen-Ohm <goldschen-ohm@utexas.edu>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


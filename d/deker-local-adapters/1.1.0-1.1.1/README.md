# Comparing `tmp/deker_local_adapters-1.1.0.tar.gz` & `tmp/deker_local_adapters-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deker_local_adapters-1.1.0.tar", max compression
+gzip compressed data, was "deker_local_adapters-1.1.1.tar", max compression
```

## Comparing `deker_local_adapters-1.1.0.tar` & `deker_local_adapters-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/LICENSE
--rw-r--r--   0        0        0      322 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/README.md
--rw-r--r--   0        0        0     1126 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/__init__.py
--rw-r--r--   0        0        0     8100 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/array_adapter.py
--rw-r--r--   0        0        0     5311 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/collection_adapter.py
--rw-r--r--   0        0        0     1002 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/errors.py
--rw-r--r--   0        0        0     3461 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/factory.py
--rw-r--r--   0        0        0     8302 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/mixin.py
--rw-r--r--   0        0        0      905 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/__init__.py
--rw-r--r--   0        0        0     1166 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/enums.py
--rw-r--r--   0        0        0      921 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/hdf5/__init__.py
--rw-r--r--   0        0        0    12120 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py
--rw-r--r--   0        0        0    11113 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py
--rw-r--r--   0        0        0     4512 2023-12-28 13:48:29.676326 deker_local_adapters-1.1.0/deker_local_adapters/varray_adapter.py
--rw-r--r--   0        0        0     8854 2023-12-28 13:48:37.132331 deker_local_adapters-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 deker_local_adapters-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-08 08:30:01.253028 deker_local_adapters-1.1.1/LICENSE
+-rw-r--r--   0        0        0      322 2024-05-08 08:30:01.253028 deker_local_adapters-1.1.1/README.md
+-rw-r--r--   0        0        0     1126 2024-05-08 08:30:01.253028 deker_local_adapters-1.1.1/deker_local_adapters/__init__.py
+-rw-r--r--   0        0        0     8054 2024-05-08 08:30:01.253028 deker_local_adapters-1.1.1/deker_local_adapters/array_adapter.py
+-rw-r--r--   0        0        0     5311 2024-05-08 08:30:01.253028 deker_local_adapters-1.1.1/deker_local_adapters/collection_adapter.py
+-rw-r--r--   0        0        0     1002 2024-05-08 08:30:01.253028 deker_local_adapters-1.1.1/deker_local_adapters/errors.py
+-rw-r--r--   0        0        0     3461 2024-05-08 08:30:01.257029 deker_local_adapters-1.1.1/deker_local_adapters/factory.py
+-rw-r--r--   0        0        0     8345 2024-05-08 08:30:01.257029 deker_local_adapters-1.1.1/deker_local_adapters/mixin.py
+-rw-r--r--   0        0        0      905 2024-05-08 08:30:01.257029 deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/__init__.py
+-rw-r--r--   0        0        0     1166 2024-05-08 08:30:01.257029 deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/enums.py
+-rw-r--r--   0        0        0      921 2024-05-08 08:30:01.257029 deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/hdf5/__init__.py
+-rw-r--r--   0        0        0    12120 2024-05-08 08:30:01.257029 deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py
+-rw-r--r--   0        0        0    11115 2024-05-08 08:30:01.257029 deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py
+-rw-r--r--   0        0        0     4478 2024-05-08 08:30:01.257029 deker_local_adapters-1.1.1/deker_local_adapters/varray_adapter.py
+-rw-r--r--   0        0        0     8856 2024-05-08 08:30:11.693065 deker_local_adapters-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 deker_local_adapters-1.1.1/PKG-INFO
```

### Comparing `deker_local_adapters-1.1.0/LICENSE` & `deker_local_adapters-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/__init__.py` & `deker_local_adapters-1.1.1/deker_local_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/array_adapter.py` & `deker_local_adapters-1.1.1/deker_local_adapters/array_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Generator, Optional, Tuple, Type, Union
 
 from deker.ABC.base_adapters import BaseArrayAdapter
 from deker.arrays import Array
 from deker.ctx import CTX
 from deker.errors import DekerArrayError
-from deker.locks import CreateArrayLock, ReadArrayLock, WriteArrayLock
+from deker.locks import ReadArrayLock, WriteArrayLock
 from deker.log import SelfLoggerMixin
 from deker.schemas import AttributeSchema
 from deker.tools import get_main_path, get_symlink_path
 from deker.tools.decorators import check_ctx_state
 from deker.types import ArrayMeta, Numeric, Slice
 from numpy import ndarray
 
@@ -78,17 +78,16 @@
             if files:
                 # just one file is expected inside the list
                 return files[0]
         except FileNotFoundError:
             return None
 
     @check_ctx_state
-    @CreateArrayLock()
-    def create(self, array: Array) -> Array:
-        """Create a new array.
+    def create(self, array: Array) -> None:
+        """Create a new array on disk storage.
 
         :param array: Array instance
         """
         main_filename, sym_filename = self.get_filenames_for_create_methods(array)
         self.check_array_file_existence(main_filename)
 
         # If the array is part of a varray, check that such varray exists
@@ -107,15 +106,14 @@
         self.storage_adapter.create(
             main_filename,
             array.shape,
             array_meta,
         )
         # Create symlink
         os.symlink(main_filename, sym_filename)
-        return array
 
     @check_ctx_state
     @ReadArrayLock()
     def read_data(self, array: Array, bounds: Slice) -> Union[Numeric, ndarray]:
         """Read data from the existing array.
 
         :param array: Array instance
```

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/collection_adapter.py` & `deker_local_adapters-1.1.1/deker_local_adapters/collection_adapter.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/errors.py` & `deker_local_adapters-1.1.1/deker_local_adapters/errors.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/factory.py` & `deker_local_adapters-1.1.1/deker_local_adapters/factory.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/mixin.py` & `deker_local_adapters-1.1.1/deker_local_adapters/mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from deker.types import ArrayMeta
 from deker_tools.path import is_empty
 
 from deker_local_adapters.errors import DekerBrokenSymlinkError
 
 
 if TYPE_CHECKING:
-    from deker.ABC import BaseArray, BaseArraysSchema
+    from deker.ABC import BaseArraysSchema
     from deker.ABC.base_adapters import BaseArrayAdapter, BaseVArrayAdapter
     from deker.collection import Collection
 
 
 class LocalAdapterMixin(object):
     """Mixin for local adapters.
 
@@ -67,15 +67,15 @@
                         break
                     if folder.exists():
                         os.rmdir(folder)
         except FileNotFoundError:
             pass
 
     @check_ctx_state
-    def delete(self, array: "BaseArray") -> None:
+    def delete(self, array: Union[Array, VArray]) -> None:
         """Delete the existing array.
 
         :param array: array instance
         """
         try:
             paths = get_paths(array, self.collection_path)
             filename = array.id + self.file_ext
@@ -83,30 +83,30 @@
             for file in files:
                 self._delete(file)
 
         except Exception as e:
             self.logger.exception(e)
             raise e
 
-    def is_deleted(self, array: "BaseArray") -> bool:
+    def is_deleted(self, array: Union[Array, VArray]) -> bool:
         """Check if the array was deleted.
 
         :param array: Array to check
         """
         path = get_main_path(array.id, self.collection_path / self.data_dir)
         # If it does not exist, then it's not created or deleted
         return not os.path.exists(path)
 
     @check_ctx_state
-    def _get_main_path_to_file(self, array: "BaseArray") -> Path:
+    def _get_main_path_to_file(self, array: Union[Array, VArray]) -> Path:
         paths = get_paths(array, self.collection_path)
         file = array.id + self.file_ext
         return paths.main / file
 
-    def get_filenames_for_create_methods(self, array: "BaseArray") -> Tuple[Path, Path]:
+    def get_filenames_for_create_methods(self, array: Union[Array, VArray]) -> Tuple[Path, Path]:
         """Return paths to the main file and symlink.
 
         !!! DO NOT USE THIS METHOD ANYWHERE EXCEPT adapter.create !!!!
 
         :param array: Array or VArray
         """
         paths = get_paths(array, self.collection_path)
@@ -160,15 +160,15 @@
     def get_by_primary_attributes(
         self,
         primary_attributes: dict,
         schema: "BaseArraysSchema",
         collection: "Collection",
         array_adapter: "BaseArrayAdapter",
         varray_adapter: "BaseVArrayAdapter",
-    ) -> Optional["BaseArray"]:
+    ) -> Optional[Union[Array, VArray]]:
         """Find (V)Array by given primary attributes.
 
         :param primary_attributes: Key attributes
         :param schema: (V)Array schema
         :param collection: Collection instance
         :param array_adapter: Arrays' adapter
         :param varray_adapter: VArrays' adapter
@@ -196,15 +196,15 @@
 
     def get_by_id(
         self,
         id_: str,
         collection: "Collection",
         array_adapter: "BaseArrayAdapter",
         varray_adapter: "BaseVArrayAdapter",
-    ) -> Optional["BaseArray"]:
+    ) -> Optional[Union[Array, VArray]]:
         """Find (V)Array by id.
 
         :param id_: Array id
         :param collection: Collection
         :param array_adapter: Arrays' adapter
         :param varray_adapter: VArrays' adapter
         """
```

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/__init__.py` & `deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/enums.py` & `deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/enums.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/hdf5/__init__.py` & `deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py` & `deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/hdf5/hdf5_options.py`

 * *Files identical despite different names*

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py` & `deker_local_adapters-1.1.1/deker_local_adapters/storage_adapters/hdf5/hdf5_storage_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from h5py import Dataset
 from numpy import ndarray
 
 from deker_local_adapters.storage_adapters.hdf5.hdf5_options import HDF5Options
 
 
 os.environ["HDF5_PLUGIN_PATH"] = hdf5plugin.PLUGIN_PATH
-os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"
+# os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"
 
 
 class HDF5StorageAdapter(SelfLoggerMixin, BaseStorageAdapter):
     """Local HDF5 storage adapter.
 
     Wraps `h5py` files managing logic.
     """
```

### Comparing `deker_local_adapters-1.1.0/deker_local_adapters/varray_adapter.py` & `deker_local_adapters-1.1.1/deker_local_adapters/varray_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from typing import Any, Type, Union
 
 from deker.ABC import BaseStorageAdapter
 from deker.ABC.base_adapters import BaseVArrayAdapter
 from deker.arrays import VArray
 from deker.ctx import CTX
 from deker.errors import DekerArrayError
-from deker.locks import CreateArrayLock, UpdateMetaAttributeLock
+from deker.locks import UpdateMetaAttributeLock
 from deker.log import SelfLoggerMixin
 from deker.tools.decorators import check_ctx_state
 from deker.types import ArrayMeta, Numeric, Slice
 from numpy import ndarray
 
 from deker_local_adapters.mixin import LocalAdapterMixin
 
@@ -65,32 +65,30 @@
 
     @check_ctx_state
     def clear(self, array: "VArray", bounds: Slice) -> None:
         """Not implemented."""
         raise NotImplementedError
 
     @check_ctx_state
-    @CreateArrayLock()
-    def create(self, array: VArray) -> VArray:
-        """Create varray.
+    def create(self, array: VArray) -> None:
+        """Create a new virtual array on disk storage.
 
         :param array: VArray instance
         """
         main_filename, sym_filename = self.get_filenames_for_create_methods(array)
         self.check_array_file_existence(main_filename)
 
         if array.primary_attributes:
             self.check_symlink_existence(sym_filename)
 
         os.makedirs(main_filename.parent, exist_ok=True)
         varray_meta = array._create_meta()
         with open(main_filename, "w", encoding="utf-8") as f:
             f.write(varray_meta)
         os.symlink(main_filename, sym_filename)
-        return array
 
     @check_ctx_state
     def read_meta(self, array: Union[VArray, Path]) -> ArrayMeta:
         """Read VArray metadata.
 
         :param array:  VArray instance
         """
```

### Comparing `deker_local_adapters-1.1.0/pyproject.toml` & `deker_local_adapters-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
                                 ###############
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
-version = "1.1.0"  # a placeholder for poetry CI dynamic versionning plugin
+version = "1.1.1"  # a placeholder for poetry CI dynamic versionning plugin
 name = "deker_local_adapters"
 packages = [{ include = "deker_local_adapters" }]
 description = "Plugin with local adapters for deker"
 authors = ["OpenWeather <info@openweathermap.org>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 documentation = 'https://docs.deker.io/'
@@ -55,15 +55,16 @@
                                 ####################
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.18"
 h5py = "^3.8.0"
 hdf5plugin = "^4.0.1"
-deker-tools= "^1.0.0"
+deker-tools = "^1.0.0"
+
 
 [tool.poetry.group.dev.dependencies]
 black = "23.1.0"
 darglint = "1.8.1"
 Flake8-pyproject = "1.2.3"
 flake8 = "5.0.4"
 flake8-bugbear = "23.1.20"
```

### Comparing `deker_local_adapters-1.1.0/PKG-INFO` & `deker_local_adapters-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deker_local_adapters
-Version: 1.1.0
+Version: 1.1.1
 Summary: Plugin with local adapters for deker
 Home-page: https://deker.io/
 License: GPL-3.0-only
 Author: OpenWeather
 Author-email: info@openweathermap.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```


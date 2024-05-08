# Comparing `tmp/deker-1.1.5.tar.gz` & `tmp/deker-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deker-1.1.5.tar", max compression
+gzip compressed data, was "deker-1.1.6.tar", max compression
```

## Comparing `deker-1.1.5.tar` & `deker-1.1.6.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0    35149 2024-04-03 11:51:51.083068 deker-1.1.5/LICENSE
--rw-r--r--   0        0        0     4264 2024-04-03 11:51:51.083068 deker-1.1.5/README.md
--rw-r--r--   0        0        0     1141 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/__init__.py
--rw-r--r--   0        0        0    17166 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_adapters.py
--rw-r--r--   0        0        0    21663 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_array.py
--rw-r--r--   0        0        0     1595 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_collection.py
--rw-r--r--   0        0        0     2254 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_dimension.py
--rw-r--r--   0        0        0     2900 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_factory.py
--rw-r--r--   0        0        0     2471 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_integrity.py
--rw-r--r--   0        0        0     5216 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_locks.py
--rw-r--r--   0        0        0     3266 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_managers.py
--rw-r--r--   0        0        0     6487 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_schemas.py
--rw-r--r--   0        0        0    12459 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ABC/base_subset.py
--rw-r--r--   0        0        0     1746 2024-04-03 11:51:51.083068 deker-1.1.5/deker/__init__.py
--rw-r--r--   0        0        0    12506 2024-04-03 11:51:51.083068 deker-1.1.5/deker/arrays.py
--rw-r--r--   0        0        0    25520 2024-04-03 11:51:51.083068 deker-1.1.5/deker/client.py
--rw-r--r--   0        0        0    13687 2024-04-03 11:51:51.083068 deker-1.1.5/deker/collection.py
--rw-r--r--   0        0        0     2134 2024-04-03 11:51:51.083068 deker-1.1.5/deker/config.py
--rw-r--r--   0        0        0     1527 2024-04-03 11:51:51.083068 deker-1.1.5/deker/ctx.py
--rw-r--r--   0        0        0    13257 2024-04-03 11:51:51.083068 deker-1.1.5/deker/dimensions.py
--rw-r--r--   0        0        0     2868 2024-04-03 11:51:51.083068 deker-1.1.5/deker/errors.py
--rw-r--r--   0        0        0     3054 2024-04-03 11:51:51.083068 deker-1.1.5/deker/flock.py
--rw-r--r--   0        0        0    11575 2024-04-03 11:51:51.083068 deker-1.1.5/deker/integrity.py
--rw-r--r--   0        0        0    19347 2024-04-03 11:51:51.083068 deker-1.1.5/deker/locks.py
--rw-r--r--   0        0        0     1848 2024-04-03 11:51:51.083068 deker-1.1.5/deker/log.py
--rw-r--r--   0        0        0     8640 2024-04-03 11:51:51.083068 deker-1.1.5/deker/managers.py
--rw-r--r--   0        0        0    18705 2024-04-03 11:51:51.083068 deker-1.1.5/deker/schemas.py
--rw-r--r--   0        0        0    26932 2024-04-03 11:51:51.083068 deker-1.1.5/deker/subset.py
--rw-r--r--   0        0        0     1193 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/__init__.py
--rw-r--r--   0        0        0     4241 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/array.py
--rw-r--r--   0        0        0     2063 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/decorators.py
--rw-r--r--   0        0        0     5351 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/path.py
--rw-r--r--   0        0        0     5157 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/schema.py
--rw-r--r--   0        0        0     2013 2024-04-03 11:51:51.083068 deker-1.1.5/deker/tools/time.py
--rw-r--r--   0        0        0      902 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/__init__.py
--rw-r--r--   0        0        0      720 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/__init__.py
--rw-r--r--   0        0        0     3281 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/classes.py
--rw-r--r--   0        0        0     2923 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/enums.py
--rw-r--r--   0        0        0     1339 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/shell.py
--rw-r--r--   0        0        0     3388 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/private/typings.py
--rw-r--r--   0        0        0        0 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/public/__init__.py
--rw-r--r--   0        0        0     5274 2024-04-03 11:51:51.083068 deker-1.1.5/deker/types/public/classes.py
--rw-r--r--   0        0        0     6339 2024-04-03 11:51:51.083068 deker-1.1.5/deker/uri.py
--rw-r--r--   0        0        0     7766 2024-04-03 11:51:51.087068 deker-1.1.5/deker/validators.py
--rw-r--r--   0        0        0      787 2024-04-03 11:51:51.087068 deker-1.1.5/deker/warnings.py
--rw-r--r--   0        0        0     9525 2024-04-03 11:51:59.215157 deker-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     6008 1970-01-01 00:00:00.000000 deker-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-08 09:57:02.251088 deker-1.1.6/LICENSE
+-rw-r--r--   0        0        0     4264 2024-05-08 09:57:02.251088 deker-1.1.6/README.md
+-rw-r--r--   0        0        0     1141 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/__init__.py
+-rw-r--r--   0        0        0    17166 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_adapters.py
+-rw-r--r--   0        0        0    20390 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_array.py
+-rw-r--r--   0        0        0     1595 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_collection.py
+-rw-r--r--   0        0        0     2254 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_dimension.py
+-rw-r--r--   0        0        0     2900 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_factory.py
+-rw-r--r--   0        0        0     2471 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_integrity.py
+-rw-r--r--   0        0        0     5182 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_locks.py
+-rw-r--r--   0        0        0     3266 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_managers.py
+-rw-r--r--   0        0        0     6487 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_schemas.py
+-rw-r--r--   0        0        0    12459 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ABC/base_subset.py
+-rw-r--r--   0        0        0     1745 2024-05-08 09:57:02.251088 deker-1.1.6/deker/__init__.py
+-rw-r--r--   0        0        0    12506 2024-05-08 09:57:02.251088 deker-1.1.6/deker/arrays.py
+-rw-r--r--   0        0        0    25520 2024-05-08 09:57:02.251088 deker-1.1.6/deker/client.py
+-rw-r--r--   0        0        0    13687 2024-05-08 09:57:02.251088 deker-1.1.6/deker/collection.py
+-rw-r--r--   0        0        0     2134 2024-05-08 09:57:02.251088 deker-1.1.6/deker/config.py
+-rw-r--r--   0        0        0     1527 2024-05-08 09:57:02.251088 deker-1.1.6/deker/ctx.py
+-rw-r--r--   0        0        0    13257 2024-05-08 09:57:02.251088 deker-1.1.6/deker/dimensions.py
+-rw-r--r--   0        0        0     4016 2024-05-08 09:57:02.251088 deker-1.1.6/deker/errors.py
+-rw-r--r--   0        0        0     3054 2024-05-08 09:57:02.251088 deker-1.1.6/deker/flock.py
+-rw-r--r--   0        0        0    11576 2024-05-08 09:57:02.251088 deker-1.1.6/deker/integrity.py
+-rw-r--r--   0        0        0    15932 2024-05-08 09:57:02.251088 deker-1.1.6/deker/locks.py
+-rw-r--r--   0        0        0     1848 2024-05-08 09:57:02.251088 deker-1.1.6/deker/log.py
+-rw-r--r--   0        0        0     8760 2024-05-08 09:57:02.251088 deker-1.1.6/deker/managers.py
+-rw-r--r--   0        0        0    18705 2024-05-08 09:57:02.251088 deker-1.1.6/deker/schemas.py
+-rw-r--r--   0        0        0    27092 2024-05-08 09:57:02.251088 deker-1.1.6/deker/subset.py
+-rw-r--r--   0        0        0     1193 2024-05-08 09:57:02.251088 deker-1.1.6/deker/tools/__init__.py
+-rw-r--r--   0        0        0     4241 2024-05-08 09:57:02.251088 deker-1.1.6/deker/tools/array.py
+-rw-r--r--   0        0        0     5491 2024-05-08 09:57:02.251088 deker-1.1.6/deker/tools/attributes.py
+-rw-r--r--   0        0        0     2063 2024-05-08 09:57:02.251088 deker-1.1.6/deker/tools/decorators.py
+-rw-r--r--   0        0        0     5351 2024-05-08 09:57:02.251088 deker-1.1.6/deker/tools/path.py
+-rw-r--r--   0        0        0     5157 2024-05-08 09:57:02.251088 deker-1.1.6/deker/tools/schema.py
+-rw-r--r--   0        0        0     2013 2024-05-08 09:57:02.251088 deker-1.1.6/deker/tools/time.py
+-rw-r--r--   0        0        0      902 2024-05-08 09:57:02.251088 deker-1.1.6/deker/types/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-08 09:57:02.251088 deker-1.1.6/deker/types/private/__init__.py
+-rw-r--r--   0        0        0     3281 2024-05-08 09:57:02.251088 deker-1.1.6/deker/types/private/classes.py
+-rw-r--r--   0        0        0     2923 2024-05-08 09:57:02.251088 deker-1.1.6/deker/types/private/enums.py
+-rw-r--r--   0        0        0     1339 2024-05-08 09:57:02.251088 deker-1.1.6/deker/types/private/shell.py
+-rw-r--r--   0        0        0     3388 2024-05-08 09:57:02.251088 deker-1.1.6/deker/types/private/typings.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:57:02.251088 deker-1.1.6/deker/types/public/__init__.py
+-rw-r--r--   0        0        0     5274 2024-05-08 09:57:02.251088 deker-1.1.6/deker/types/public/classes.py
+-rw-r--r--   0        0        0     6339 2024-05-08 09:57:02.251088 deker-1.1.6/deker/uri.py
+-rw-r--r--   0        0        0     9245 2024-05-08 09:57:02.255088 deker-1.1.6/deker/validators.py
+-rw-r--r--   0        0        0      787 2024-05-08 09:57:02.255088 deker-1.1.6/deker/warnings.py
+-rw-r--r--   0        0        0     9566 2024-05-08 09:57:10.099133 deker-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6008 1970-01-01 00:00:00.000000 deker-1.1.6/PKG-INFO
```

### Comparing `deker-1.1.5/LICENSE` & `deker-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/README.md` & `deker-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ABC/__init__.py` & `deker-1.1.6/deker/ABC/__init__.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ABC/base_adapters.py` & `deker-1.1.6/deker/ABC/base_adapters.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ABC/base_array.py` & `deker-1.1.6/deker/ABC/base_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """Abstract interfaces for array and virtual array."""
 
 import json
 
 from abc import ABC, abstractmethod
-from collections import OrderedDict
 from copy import deepcopy
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any, List, Optional, Tuple, Type, Union
 
 import numpy as np
 
 from deker_tools.slices import create_shape_from_slice
@@ -31,18 +30,19 @@
 
 from deker.dimensions import Dimension, TimeDimension
 from deker.errors import DekerMetaDataError, DekerValidationError
 from deker.log import SelfLoggerMixin
 from deker.schemas import ArraySchema, VArraySchema
 from deker.subset import Subset, VSubset
 from deker.tools.array import check_memory, get_id
+from deker.tools.attributes import make_ordered_dict, serialize_attribute_value
 from deker.tools.schema import create_dimensions
 from deker.types.private.classes import ArrayMeta, Serializer
 from deker.types.private.typings import FancySlice, Numeric, Slice
-from deker.validators import process_attributes, is_valid_uuid, validate_custom_attributes_update
+from deker.validators import is_valid_uuid, process_attributes, validate_custom_attributes_update
 
 
 if TYPE_CHECKING:
     from deker.ABC.base_adapters import BaseArrayAdapter, BaseVArrayAdapter, IArrayAdapter
     from deker.arrays import Array, VArray
     from deker.collection import Collection
 
@@ -291,18 +291,17 @@
         self.__adapter = adapter
         self.__array_adapter = array_adapter
 
         primary_attributes, custom_attributes = process_attributes(
             self.schema, primary_attributes, custom_attributes
         )
 
-        self.primary_attributes: OrderedDict = (
-            OrderedDict({**primary_attributes}) if primary_attributes else OrderedDict()
+        self.primary_attributes, self.custom_attributes = make_ordered_dict(
+            primary_attributes, custom_attributes, self.schema.attributes  # type: ignore[arg-type]
         )
-        self.custom_attributes: dict = custom_attributes if custom_attributes else {}
 
     def __del__(self) -> None:
         del self.__adapter
         del self.__array_adapter
         del self.__collection
 
     @property
@@ -388,34 +387,22 @@
             attributes,
         )
         self._adapter.update_meta_custom_attributes(self, attributes)
         self.custom_attributes = attributes
         self.logger.info(f"{self!s} custom attributes updated: {attributes}")
 
     def _create_meta(self) -> str:
-        """Serialize array into metadata string."""
+        """Serialize array into metadata JSON string."""
         primary_attrs, custom_attrs = deepcopy(self.primary_attributes), deepcopy(
             self.custom_attributes
         )
         for attrs in (primary_attrs, custom_attrs):
             for key, value in attrs.items():
-                if isinstance(value, datetime):
-                    attrs[key] = value.isoformat()
-                elif isinstance(value, np.ndarray):
-                    attrs[key] = value.tolist()
-                elif isinstance(value, (list, tuple)):
-                    elements = []
-                    for element in value:
-                        if isinstance(element, np.integer):
-                            elements.append(int(element))
-                        else:
-                            elements.append(element)
-                    attrs[key] = tuple(elements)
-                else:
-                    attrs[key] = value
+                attrs[key] = serialize_attribute_value(value)
+
         return json.dumps(
             {
                 "id": self.id,
                 "primary_attributes": primary_attrs,
                 "custom_attributes": custom_attrs,
             }
         )
@@ -466,42 +453,29 @@
         :param array_adapter: Array adapter instance
         :param varray_adapter: VArray adapter instance
         """
         if varray_adapter:
             attrs_schema = collection.varray_schema.attributes
         else:
             attrs_schema = collection.array_schema.attributes
-        try:
-            for attr in attrs_schema:
-                attributes = (
-                    meta["primary_attributes"] if attr.primary else meta["custom_attributes"]
-                )
 
-                value = attributes[attr.name]
-
-                if attr.dtype == datetime:
-                    attributes[attr.name] = get_utc(value)
-                if attr.dtype == tuple:
-                    if (
-                        attr.primary or (not attr.primary and value is not None)
-                    ) and not isinstance(value, list):
-                        raise DekerMetaDataError(
-                            f"Collection '{collection.name}' metadata is corrupted: "
-                            f"attribute '{attr.name}' has invalid type '{type(value)}'; '{attr.dtype}' expected"
-                        )
-
-                    if attr.primary or (not attr.primary and value is not None):
-                        attributes[attr.name] = tuple(value)
+        try:
+            # To ensure the order of attributes
+            primary_attributes, custom_attributes = make_ordered_dict(
+                meta["primary_attributes"],
+                meta["custom_attributes"],
+                attrs_schema,  # type: ignore[arg-type]
+            )
 
             arr_params = {
                 "collection": collection,
                 "adapter": array_adapter,
                 "id_": meta["id"],
-                "primary_attributes": meta.get("primary_attributes"),
-                "custom_attributes": meta.get("custom_attributes"),
+                "primary_attributes": primary_attributes,
+                "custom_attributes": custom_attributes,
             }
             if varray_adapter:
                 arr_params.update({"adapter": varray_adapter, "array_adapter": array_adapter})
             return cls(**arr_params)  # type: ignore[arg-type,return-value]
         except (KeyError, ValueError) as e:
             raise DekerMetaDataError(f"{cls} metadata invalid/corrupted: {e}")
```

### Comparing `deker-1.1.5/deker/ABC/base_collection.py` & `deker-1.1.6/deker/ABC/base_collection.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ABC/base_dimension.py` & `deker-1.1.6/deker/ABC/base_dimension.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ABC/base_factory.py` & `deker-1.1.6/deker/ABC/base_factory.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ABC/base_integrity.py` & `deker-1.1.6/deker/ABC/base_integrity.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ABC/base_locks.py` & `deker-1.1.6/deker/ABC/base_locks.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """Abstract interfaces for locks."""
-
 from abc import ABC, abstractmethod
 from functools import wraps
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 from deker.flock import Flock
 from deker.log import SelfLoggerMixin
@@ -27,24 +26,23 @@
 
 class BaseLock(SelfLoggerMixin, ABC):
     """Base class for read/write locks."""
 
     ALLOWED_TYPES: List[str] = []
     lock: Optional[Union[Flock, Path]] = None
     instance: Optional[Any] = None
+    args: Optional[List[Any]] = None
+    kwargs: Optional[Dict] = None
 
     @abstractmethod
-    def get_path(self, func_args: Sequence, func_kwargs: Dict) -> Optional[Path]:
+    def get_path(self) -> Optional[Path]:
         """Get path to the lock file.
 
         For Arrays it shall be .arrlock (array read lock) or path to the file (array write lock)
         For VArrays there are no specific locks for reading, for writing - lock on .json
-
-        :param func_args: Arguments of method call
-        :param func_kwargs: Keyword arguments of method call
         """
         pass
 
     def check_existing_lock(self, func_args: Sequence, func_kwargs: Dict) -> None:
         """Check if there is lock for given method.
 
         :param func_args: Arguments for function that has been called
@@ -94,15 +92,15 @@
 
         :param lock: lock to be acquired
         :param func: decorated function
         :param args: Arguments of decorated function
         :param kwargs: Keyword arguments of decorated function
         """
         lock.check_existing_lock(args, kwargs)
-        path = lock.get_path(args, kwargs)
+        path = lock.get_path()
         lock.acquire(path)
         try:
             # Logic is in the separate method, so we can override its behavior
             # E.g., CreateArray lock has specific instructions for array attribute
             result = lock.get_result(func, args, kwargs)
         except Exception as e:
             lock.release(e)
@@ -125,15 +123,16 @@
             :param args: Arguments of decorated function
             :param kwargs: Keyword arguments of decorated function
             """
             # To keep different references for locks
             lock = self.__class__()
             # as we wrap methods, we should have access to 'self' objects
             lock.instance = kwargs.get("self") or args[0]
-
+            lock.args = args
+            lock.kwargs = kwargs
             # Check that we don't have lock on anything that besides methods that require lock
             lock.check_type()
 
             # Logic is in the separate method, so we can override its behavior
             # E.g., in WriteVArrayLock, where we should skip the whole lock logic
             return lock._inner_method_logic(lock, args, kwargs, func)
```

### Comparing `deker-1.1.5/deker/ABC/base_managers.py` & `deker-1.1.6/deker/ABC/base_managers.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ABC/base_schemas.py` & `deker-1.1.6/deker/ABC/base_schemas.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ABC/base_subset.py` & `deker-1.1.6/deker/ABC/base_subset.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/__init__.py` & `deker-1.1.6/deker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,33 +13,32 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 # nopycln: file
 # isort: skip_file
 
-from deker_local_adapters.storage_adapters.hdf5.hdf5_options import (
-    HDF5Options,
-    HDF5CompressionOpts,
-)
-
 from deker.arrays import Array, VArray
 from deker.client import Client
 from deker.collection import Collection
 from deker.dimensions import Dimension, TimeDimension
 from deker.managers import FilteredManager
 from deker.schemas import (
     ArraySchema,
     AttributeSchema,
     DimensionSchema,
     TimeDimensionSchema,
     VArraySchema,
 )
 from deker.subset import Subset, VSubset
 from deker.types.public.classes import Scale
+from deker_local_adapters.storage_adapters.hdf5.hdf5_options import (
+    HDF5Options,
+    HDF5CompressionOpts,
+)
 
 __all__ = (
     # deker.adapters.hdf5
     "HDF5CompressionOpts",
     "HDF5Options",
     # deker.arrays
     "Array",
```

### Comparing `deker-1.1.5/deker/arrays.py` & `deker-1.1.6/deker/arrays.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/client.py` & `deker-1.1.6/deker/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,31 +23,31 @@
 
 from datetime import datetime
 from multiprocessing import cpu_count
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple, Type, Union
 
 from deker_tools.data import convert_size_to_human
-from deker_tools.path import is_path_valid
 from deker_tools.log import set_logger
+from deker_tools.path import is_path_valid
 from psutil import swap_memory, virtual_memory
 from tqdm import tqdm
 
 from deker.collection import Collection
 from deker.config import DekerConfig
 from deker.ctx import CTX
 from deker.errors import (
     DekerClientError,
     DekerCollectionNotExistsError,
     DekerMetaDataError,
     DekerValidationError,
 )
 from deker.integrity import IntegrityChecker
 from deker.locks import META_DIVIDER
-from deker.log import SelfLoggerMixin, set_logging_level, format_string
+from deker.log import SelfLoggerMixin, format_string, set_logging_level
 from deker.schemas import ArraySchema, VArraySchema
 from deker.tools import convert_human_memory_to_bytes
 from deker.types import ArrayLockMeta, CollectionLockMeta, LocksExtensions, LocksTypes, StorageSize
 from deker.uri import Uri
 from deker.warnings import DekerWarning
```

### Comparing `deker-1.1.5/deker/collection.py` & `deker-1.1.6/deker/collection.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/config.py` & `deker-1.1.6/deker/config.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/ctx.py` & `deker-1.1.6/deker/ctx.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/dimensions.py` & `deker-1.1.6/deker/dimensions.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/flock.py` & `deker-1.1.6/deker/flock.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/integrity.py` & `deker-1.1.6/deker/integrity.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     DekerIntegrityError,
     DekerMetaDataError,
 )
 from deker.managers import ArrayManager, VArrayManager
 from deker.tools import get_main_path, get_symlink_path
 from deker.types.private.enums import LocksExtensions
 
+
 if TYPE_CHECKING:
     from deker.client import Client
 
 
 class DataChecker(BaseChecker):
     """Checks Array's single number data from subset."""
 
@@ -183,23 +184,23 @@
             for array in data_manager:
                 try:
                     if self.next_checker:
                         self.next_checker.check(array, collection)
                 except DekerBaseApplicationError as e:
                     if self.stop_on_error:
                         raise DekerIntegrityError(str(e))
-                    self.errors[
-                        f"Collection {collection.name} arrays integrity errors:"
-                    ].append(str(e))
+                    self.errors[f"Collection {collection.name} arrays integrity errors:"].append(
+                        str(e)
+                    )
         except DekerMetaDataError as e:
             if self.stop_on_error:
                 raise e
-            self.errors[
-                f"Collection {collection.name} (V)Arrays initialization errors:"
-            ].append(str(e))
+            self.errors[f"Collection {collection.name} (V)Arrays initialization errors:"].append(
+                str(e)
+            )
 
     def check(self, collection: Collection) -> None:
         """Check if Arrays or VArrays and their locks in Collection are valid.
 
         :param collection: Collection to be checked
         """
         if self.level < self.CHECKER_LEVEL:
```

### Comparing `deker-1.1.5/deker/locks.py` & `deker-1.1.6/deker/locks.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,179 +19,227 @@
 import fcntl
 import os
 import time
 
 from pathlib import Path
 from threading import get_native_id
 from time import sleep
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Sequence, Union, Tuple
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+)
 from uuid import uuid4
 
 from deker.ABC.base_locks import BaseLock
 from deker.errors import DekerLockError, DekerMemoryError
 from deker.flock import Flock
 from deker.tools.path import get_main_path
 from deker.types.private.enums import LocksExtensions
 
 
 if TYPE_CHECKING:
     from deker_local_adapters import LocalArrayAdapter
 
     from deker.arrays import Array, VArray
-    from deker.types.private.classes import ArrayPositionedData
 
 META_DIVIDER = ":"
+ArrayFromArgs = Union[Path, Union["Array", "VArray"]]
+T = TypeVar("T")
 
 
-class ReadArrayLock(BaseLock):
+def _get_lock_filename(id_: str, lock_ext: LocksExtensions) -> str:
+    """Get filename for lockfile.
+
+    :param id_: ID of array
+    :param lock_ext: Extension of lock
+    :return:
+    """
+    name = META_DIVIDER.join([f"{id_}", f"{uuid4()}", f"{os.getpid()}", f"{get_native_id()}"])
+    return str(name + lock_ext.value)
+
+
+def _check_write_locks(dir_path: Path, id_: str) -> bool:
+    """Checks write locks from VArrays that differs from current.
+
+    :param dir_path: Dir where locks are stored (the one with hdf file)
+    :param id_: Id of array
+    """
+    for file in dir_path.iterdir():
+        # Skip lock from current process.
+        # Used when you have to read meta inside .update operation of varray
+        if file.name.endswith(f"{os.getpid()}{LocksExtensions.varray_lock.value}"):
+            return True
+        # If we've found another varray lock, that not from current process.
+        if file.name.endswith(LocksExtensions.varray_lock.value):  # type: ignore
+            raise DekerLockError(f"Array {id_} is locked with {file.name}")
+    return False
+
+
+class LockWithArrayMixin(Generic[T]):
+    """Base class with getter of array."""
+
+    args: Optional[List[Any]]
+    kwargs: Optional[Dict]
+    instance: Optional[Any]
+    is_locked_with_varray: bool = False
+
+    @property
+    def array_id(self) -> str:
+        """Get if from Array, or Path to the array."""
+        # Get instance of the array
+        if isinstance(self.array, Path):
+            path = self.array
+            id_ = path.name.split(".")[0]
+        else:
+            id_ = self.array.id  # type: ignore[attr-defined]
+        return id_
+
+    @property
+    def array(self) -> T:
+        """Parse array from args and save ref to it."""
+        array = self.kwargs.get("array") or self.args[1]  # zero arg is 'self'
+        return array
+
+    @property
+    def dir_path(self) -> Path:
+        """Path to directory with main file."""
+        return get_main_path(self.array_id, self.instance.collection_path / self.instance.data_dir)
+
+
+def wait_for_unlock(
+    check_func: Callable, check_func_args: tuple, timeout: int, interval: float
+) -> bool:
+    """Waiting while there is no locks.
+
+    :param check_func: Func that check if lock has been releases
+    :param check_func_args: Args for func
+    :param timeout: For how long we should wait lock release
+    :param interval: How often we check locks
+    :return:
+    """
+    start_time = time.monotonic()
+    while (time.monotonic() - start_time) <= timeout:
+        if check_func(*check_func_args):
+            return True
+        sleep(interval)
+    return False
+
+
+class ReadArrayLock(LockWithArrayMixin[ArrayFromArgs], BaseLock):
     """Read lock for Array."""
 
     ALLOWED_TYPES = ["LocalArrayAdapter"]
 
-    def get_path(self, func_args: Sequence, func_kwargs: Dict) -> Path:
+    def get_path(self) -> Path:
         """Get path to read-lock file.
 
         It's only the case for arrays, varrays don't have read locks.
-        :param func_args: arguments of method call
-        :param func_kwargs: keyword arguments of method call
         """
-        # Get instance of the array
-        array: Union[Path, Union[Array, VArray]] = (
-            func_kwargs.get("array") or func_args[1]
-        )  # zero arg is 'self'
-        if isinstance(array, Path):
-            path = array
-            id_ = path.name.split(".")[0]
-        else:
-            id_ = array.id
-
         # Get file directory
-        dir_path = get_main_path(id_, self.instance.collection_path / self.instance.data_dir)
-        filename = (
-            META_DIVIDER.join([f"{id_}", f"{uuid4()}", f"{os.getpid()}", f"{get_native_id()}"])
-            + LocksExtensions.array_read_lock.value
-        )
+        filename = _get_lock_filename(self.array_id, LocksExtensions.array_read_lock)
+
         # Create read lock file path
-        path = dir_path / f"{filename}"
+        path = self.dir_path / f"{filename}"
 
-        self.logger.debug(f"Got path for array.id {id_} lock file: {path}")
+        self.logger.debug(f"Got path for array.id {self.array_id} lock file: {path}")
         return path
 
     def check_existing_lock(self, func_args: Sequence, func_kwargs: Dict) -> None:
         """Read operations are not performed in case there are any WRITE locks.
 
         Array file would be Flocked for writing / updating, so we just need to try flock it once more
         :param func_args: arguments for called function.
         :param func_kwargs: keyword arguments for called function.
         """
-        array: Union[Path, Union[Array, VArray]] = (
-            func_kwargs.get("array") or func_args[1]
-        )  # zero arg is 'self'
-        if isinstance(array, Path):
-            path = array
-            id_ = path.name.split(".")[0]
-        else:
-            id_ = array.id
-
-        dir_path = get_main_path(id_, self.instance.collection_path / self.instance.data_dir)
-        path = dir_path / (id_ + self.instance.file_ext)
-        for file in dir_path.iterdir():
-            # Skip lock from current process.
-            if file.name.endswith(f"{os.getpid()}{LocksExtensions.varray_lock.value}"):
-                self.is_locked_with_varray = True
-                return
-            # If we've found another varray lock, that not from current process.
-            if file.name.endswith(LocksExtensions.varray_lock.value):  # type: ignore
-                raise DekerLockError(f"Array {array} is locked with {file.name}")
+        # Check write locks
+        if _check_write_locks(self.dir_path, self.array_id):
+            self.is_locked_with_varray = True
+            # File was locked with VArray from current process.
+            return
+        # No write locks found
+        path = self.dir_path / (self.array_id + self.instance.file_ext)
         try:
             with open(path, "r") as f:
                 fcntl.flock(f, fcntl.LOCK_SH | fcntl.LOCK_NB)
                 self.logger.debug(f"Set shared flock for {path}")
 
         except BlockingIOError:
-            raise DekerLockError(f"Array {id_} is locked for update operation, cannot be read.")
+            raise DekerLockError(
+                f"Array {self.array_id} is locked for update operation, cannot be read."
+            )
 
     def acquire(self, path: Union[str, Path]) -> Any:
         """Read files will not be flocked - only created.
 
         :param path: Path to file which should be locked
         """
         # Create lock file
         self.lock = path
         open(path, "a").close()
-        self.logger.debug(f"Acquired lock for {self.lock}")
+        self.logger.debug(f"Acquired read lock for {self.lock}")
 
     def release(self, e: Optional[Exception] = None) -> None:  # noqa[ARG002]
         """Release lock by deleting file.
 
         :param e: Exception that may have been raised.
         """
         if self.lock and self.lock.exists():
             self.lock.unlink()
+            self.logger.debug(f"Releasing read lock for {self.lock}")
             self.lock = None
-            self.logger.debug(f"Released lock for {self.lock}")
 
 
-class WriteArrayLock(BaseLock):
+class WriteArrayLock(LockWithArrayMixin["Array"], BaseLock):
     """Write lock for arrays."""
 
     ALLOWED_TYPES = ["LocalArrayAdapter"]
 
-    is_locked_with_varray: bool = False
-
-    def get_path(self, func_args: Sequence, func_kwargs: Dict) -> Path:
-        """Get path to the file for locking.
-
-        :param func_args: arguments of method call
-        :param func_kwargs: keyword arguments of method call
-        """
-        array = func_kwargs.get("array") or func_args[1]  # zero arg is 'self'
-        dir_path = get_main_path(array.id, self.instance.collection_path / self.instance.data_dir)
-        path = dir_path / (array.id + self.instance.file_ext)
-        self.logger.debug(f"Got path for array.id {array.id} lock file: {path}")
+    def get_path(self) -> Path:
+        """Get path to the file for locking."""
+        path = self.dir_path / (self.array_id + self.instance.file_ext)
+        self.logger.debug(f"Got path for array.id {self.array.id} lock file: {path}")
         return path
 
     def check_existing_lock(self, func_args: Sequence, func_kwargs: Dict) -> None:
         """Check read locks before write execution.
 
         :param func_args: arguments of method call
         :param func_kwargs: keyword arguments of method call
         """
-        # Check current read locks
-        array = func_kwargs.get("array") or func_args[1]  # zero arg is 'self'
-        dir_path = get_main_path(array.id, self.instance.collection_path / self.instance.data_dir)
-
         # If array belongs to varray, we should check if varray is also locked
-        if array._vid:
-            for file in dir_path.iterdir():
-                # Skip lock from current process.
-                if file.name.endswith(f"{os.getpid()}{LocksExtensions.varray_lock.value}"):
-                    self.is_locked_with_varray = True
-                    return
-                # If we've found another varray lock, that not from current process.
-                if file.name.endswith(LocksExtensions.varray_lock.value):  # type: ignore
-                    raise DekerLockError(f"Array {array} is locked with {file.name}")
+        self.is_locked_with_varray = _check_write_locks(self.dir_path, self.array_id)
 
         # Increment write lock, to prevent more read locks coming.
-        self.acquire(self.get_path(func_args, func_kwargs))
+        self.acquire(self.get_path())
 
         # Pattern that has to find any read locks
-        glob_pattern = f"{array.id}:*{LocksExtensions.array_read_lock.value}"
+        glob_pattern = f"{self.array.id}:*{LocksExtensions.array_read_lock.value}"
 
         # Wait till there are no more read locks
-        start_time = time.monotonic()
-        while (time.monotonic() - start_time) <= self.instance.ctx.config.write_lock_timeout:
-            if not list(dir_path.rglob(glob_pattern)):
-                return
-
-            sleep(self.instance.ctx.config.write_lock_check_interval)
+        if wait_for_unlock(
+            lambda path, pattern: not list(path.rglob(pattern)),
+            (self.dir_path, glob_pattern),
+            self.instance.ctx.config.write_lock_timeout,
+            self.instance.ctx.config.write_lock_check_interval,
+        ):
+            # If all locks are released, go further
+            return
 
         # If we hit the timeout, release write lock and raise DekerLockError
         self.release()
-        raise DekerLockError(f"Array {array} is locked with read locks")
+        raise DekerLockError(f"Array {self.array} is locked with read locks")
 
     def release(self, e: Optional[Exception] = None) -> None:
         """Release Flock.
 
         If array is locked from Varary from current Process, do nothing
         :param e: exception that might have been raised
         """
@@ -233,33 +281,28 @@
 
         super().check_type()
         adapter = self.instance._VSubset__adapter
         is_running_on_local = isinstance(adapter, LocalVArrayAdapter)
         if not is_running_on_local:
             self.skip_lock = True
 
-    def get_path(self, func_args: Sequence, func_kwargs: Dict) -> Optional[Path]:  # noqa[ARG002]
-        """Path of json Varray file.
-
-        :param func_args: arguments of the function that has been called.
-        :param func_kwargs: keyword arguments of the function that has been called.
-        """
+    def get_path(self) -> Optional[Path]:  # noqa[ARG002]
+        """Path of json Varray file."""
         array = self.instance._VSubset__array
         adapter = self.instance._VSubset__adapter
         path = get_main_path(
             array.id, self.instance._VSubset__collection.path / adapter.data_dir
         ) / (array.id + adapter.file_ext)
         self.logger.debug(f"Got path for array.id {array.id} lock file: {path}")
         return path
 
     def check_locks_for_array_and_set_flock(self, filename: Path) -> Flock:
         """Check if there is no read lock.
 
         :param filename: Path to file that should be flocked
-        :return:
         """
         # Check read lock first
         array_id = filename.name.split(".")[0]
         glob_pattern = f"{array_id}:*"
         for _ in filename.parent.rglob(glob_pattern):
             raise DekerLockError(f"Array {array_id} is locked")
 
@@ -269,28 +312,26 @@
 
         # Add flag that this array is locked by varray
         open(f"{filename}:{os.getpid()}{LocksExtensions.varray_lock.value}", "w").close()
         return lock
 
     def check_arrays_locks(
         self,
-        arrays_positions: List[ArrayPositionedData],
         adapter: LocalArrayAdapter,
         varray: VArray,
     ) -> List[Path]:
         """Check all Arrays that are in current VArray.
 
-        :param arrays_positions: Arrays' positions in VArray
         :param adapter: Array Adapter instance
         :param varray: VArray
         """
         currently_locked = []
 
         collection = varray._VArray__collection  # type: ignore[attr-defined]
-        for array_position in arrays_positions:
+        for array_position in self.instance._VSubset__arrays:
             filename = adapter._get_symlink_filename(
                 varray.id,
                 array_position.vposition,
                 collection.array_schema.primary_attributes,  # type: ignore[arg-type]
             )
             if not filename:
                 continue
@@ -310,33 +351,33 @@
 
         :param func_args: arguments of the function that has been called.
         :param func_kwargs: keyword arguments of the function that has been called.
         """
         adapter = self.instance._VSubset__array_adapter
         varray = self.instance._VSubset__array
 
-        arrays_positions: List[ArrayPositionedData] = self.instance._VSubset__arrays
-
         # Clear links to locks
         self.locks = []
         # Locks that have been acquired by third party process
 
         # Iterate over Arrays in VArray and try to lock them. If locking fails - wait.
         # If it fails again - release all locks.
-        currently_locked = self.check_arrays_locks(arrays_positions, adapter, varray)
+        currently_locked = self.check_arrays_locks(adapter, varray)
         if not currently_locked:
             # Release array locks
             return
 
         # Wait till there are no more read locks
-        start_time = time.monotonic()
-        while (time.monotonic() - start_time) <= adapter.ctx.config.write_lock_timeout:
-            if not self.check_arrays_locks(arrays_positions, adapter, varray):
-                return
-            sleep(adapter.ctx.config.write_lock_check_interval)
+        if wait_for_unlock(
+            check_func=lambda: not self.check_arrays_locks(adapter, varray),
+            check_func_args=tuple(),
+            timeout=adapter.ctx.config.write_lock_timeout,
+            interval=adapter.ctx.config.write_lock_check_interval,
+        ):
+            return
         # Release all locks
         self.release()
         raise DekerLockError(f"VArray {varray} is locked")
 
     def release(self, e: Optional[Exception] = None) -> None:  # noqa[ARG002]
         """Release all locks.
 
@@ -372,135 +413,38 @@
         """
         # If we want to skip logic of lock (e.g. when we use server adapters)
         if lock.skip_lock:
             return lock.get_result(func, args, kwargs)
         return super()._inner_method_logic(lock, args, kwargs, func)
 
 
-class CreateArrayLock(BaseLock):
-    """Lock that we set when we want to create an array."""
-
-    ALLOWED_TYPES = ["LocalArrayAdapter", "LocalVArrayAdapter"]
-
-    path: Optional[Path] = None
-
-    def get_path(self, func_args: Sequence, func_kwargs: Dict) -> Path:
-        """Return path to the file that should be locked.
-
-        :param func_args: arguments for called method
-        :param func_kwargs: keyword arguments for called method
-        :return:
-        """
-        array = func_kwargs.get("array") or func_args[1]  # zero arg is 'self'
-
-        # Get file directory path
-        dir_path = self.instance.collection_path
-        filename = META_DIVIDER.join(
-            [
-                f"{array.id}",
-                f"{uuid4()}",
-                f"{os.getpid()}",
-                f"{get_native_id()}",
-            ]
-        )
-        # Create lock file
-        path = dir_path / f"{filename}{LocksExtensions.array_lock.value}"
-        if not path.exists():
-            path.open("w").close()
-
-        self.path = path
-        self.logger.debug(f"got path for array.id {array.id} lock file: {path}")
-        return path
-
-    def check_existing_lock(self, func_args: Sequence, func_kwargs: Dict) -> None:
-        """Check if there is currently lock for array creating.
-
-        :param func_args: arguments for called method
-        :param func_kwargs: keyword arguments for called method
-        """
-        from deker.arrays import Array, VArray
-
-        # Check current read locks
-        array = func_kwargs.get("array") or func_args[1]  # zero arg is 'self'
-        if isinstance(array, dict):
-            adapter = array["adapter"].__class__.__name__
-            if adapter not in self.ALLOWED_TYPES:
-                raise DekerLockError(f"Adapter {adapter} is not allowed to create locks for arrays")
-
-            # TODO: figure out a way to avoid constructing Array object here
-            array_type = Array if adapter == self.ALLOWED_TYPES[0] else VArray
-            array = array_type(**array)
-
-        dir_path = self.instance.collection_path
-
-        # Pattern that has to find any create locks
-        glob_pattern = f"{array.id}:*{LocksExtensions.array_lock.value}"
-        for _ in dir_path.rglob(glob_pattern):
-            raise DekerLockError(f"Array {array} is locked for creating")
-
-        func_kwargs["array"] = array
-
-    def get_result(self, func: Callable, args: Any, kwargs: Any) -> Any:
-        """Call func, and get its result.
-
-        :param func: decorated function
-        :param args: arguments of decorated function
-        :param kwargs: keyword arguments of decorated function
-        """
-        if kw_array := kwargs.pop("array"):
-            args = list(args)
-            # First elem is self, so for functions with array, set array as next arg.
-            args[1] = kw_array
-            result = func(*tuple(args), **kwargs)
-        else:
-            result = func(*args, **kwargs)
-        return result
-
-    def release(self, e: Optional[Exception] = None) -> None:
-        """Release Flock.
-
-        :param e: exception that might have been raised
-        """
-        self.path.unlink(missing_ok=True)
-        super().release(e)
-
-
-class UpdateMetaAttributeLock(BaseLock):
+class UpdateMetaAttributeLock(LockWithArrayMixin[Union["Array", "VArray"]], BaseLock):
     """Lock for updating meta."""
 
     ALLOWED_TYPES = ["LocalArrayAdapter", "LocalVArrayAdapter"]
 
-    def get_path(self, func_args: Sequence, func_kwargs: Dict) -> Path:
-        """Return path to the file that should be locked.
-
-        :param func_args: arguments for called method
-        :param func_kwargs: keyword arguments for called method
-        :return:
-        """
-        array = func_kwargs.get("array") or func_args[1]  # zero arg is 'self'
-
+    def get_path(self) -> Path:
+        """Return path to the file that should be locked."""
         # Get directory where file locates
-        dir_path = get_main_path(array.id, self.instance.collection_path / self.instance.data_dir)
-        path = dir_path / f"{array.id}{self.instance.file_ext}"
-        self.logger.debug(f"Got path for array.id {array.id} lock file: {path}")
+        dir_path = get_main_path(
+            self.array.id, self.instance.collection_path / self.instance.data_dir
+        )
+        path = dir_path / f"{self.array.id}{self.instance.file_ext}"
+        self.logger.debug(f"Got path for array.id {self.array.id} lock file: {path}")
         return path
 
 
 class CollectionLock(BaseLock):
     """Lock for collection creation."""
 
     ALLOWED_TYPES = ["LocalCollectionAdapter"]
 
-    def get_path(self, func_args: Sequence, func_kwargs: Dict) -> Path:  # noqa[ARG002]
-        """Return path to collection lock file.
-
-        :param func_args: arguments for called method
-        :param func_kwargs: keyword arguments for called method
-        """
-        collection = func_args[1]
+    def get_path(self) -> Path:  # noqa[ARG002]
+        """Return path to collection lock file."""
+        collection = self.args[1]
         path = self.instance.collections_resource / (collection.name + ".lock")
         self.logger.debug(f"Got path for collection {collection.name} lock file: {path}")
         return path
 
     def release(self, e: Optional[Exception] = None) -> None:
         """Release Collection Lock.
```

### Comparing `deker-1.1.5/deker/log.py` & `deker-1.1.6/deker/log.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/managers.py` & `deker-1.1.6/deker/managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,17 +128,19 @@
         if isinstance(schema, VArraySchema):
             arr_params.update(
                 {
                     "adapter": self.__varray_adapter,  # type: ignore[dict-item]
                     "array_adapter": self.__array_adapter,  # type: ignore[dict-item]
                 }
             )
+            array = VArray(**arr_params)  # type: ignore[arg-type]
         else:
             arr_params.update({"adapter": self.__array_adapter})  # type: ignore[dict-item]
-        array = self._adapter.create(arr_params)
+            array = Array(**arr_params)  # type: ignore[arg-type]
+        self._adapter.create(array)
         return array
 
     def create(
         self,
         primary_attributes: Optional[dict] = None,
         custom_attributes: Optional[dict] = None,
         id_: Optional[str] = None,
```

### Comparing `deker-1.1.5/deker/schemas.py` & `deker-1.1.6/deker/schemas.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/subset.py` & `deker-1.1.6/deker/subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,25 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import builtins
+import traceback
 
 from typing import TYPE_CHECKING, Iterator, List, Optional, Tuple, Union
 
 import numpy as np
 
 from deker_tools.slices import create_shape_from_slice, match_slice_size, slice_converter
 from numpy import ndarray
 
 from deker.ABC.base_subset import BaseSubset
-from deker.errors import DekerArrayError, DekerLockError, DekerVSubsetError
+from deker.errors import DekerArrayError, DekerVSubsetError
 from deker.locks import WriteVarrayLock
 from deker.schemas import TimeDimensionSchema
 from deker.tools import not_deleted
 from deker.types.private.classes import (
     ArrayOffset,
     ArrayPosition,
     ArrayPositionedData,
@@ -573,14 +574,15 @@
 
         * Data cannot be ``None``
         * Data ``shape`` should be equal to the ``VSubset.shape``
         * Data ``dtype`` should be equal to the ``VArray.dtype``
 
         :param data: new data which shall match subset slicing
         """
+        from deker.arrays import Array
 
         def _update(array_data: ArrayPositionedData) -> None:
             """If there is a need in the future to calculate Array's time dimension start value.  # noqa: DAR101, D400
 
             ATD - Array time dimension
             VATD - VArray time dimension
             vpos - v_position
@@ -595,46 +597,49 @@
                         dim_schema.start_value, str
                     ):
                         attr_name = dim_schema.start_value[1:]
                         dim: TimeDimension = self.__array.dimensions[n]
                         pos = array_data.vposition[n]
                         custom_attributes[attr_name] = dim.start_value + dim.step * pos  # type: ignore[operator]
 
-                array = self.__array_adapter.create(
-                    {
-                        "collection": self.__collection,
-                        "adapter": self.__array_adapter,
-                        "primary_attributes": {
-                            "vid": self.__array.id,
-                            "v_position": array_data.vposition,
-                        },
-                        "custom_attributes": custom_attributes,
-                    }
-                )
+                kwargs = {
+                    "collection": self.__collection,
+                    "adapter": self.__array_adapter,
+                    "primary_attributes": {
+                        "vid": self.__array.id,
+                        "v_position": array_data.vposition,
+                    },
+                    "custom_attributes": custom_attributes,
+                }
+                array = Array(**kwargs)  # type: ignore[arg-type]
+                self.__array_adapter.create(array)
             subset = array[array_data.bounds]
             subset.update(array_data.data)
 
         self.logger.debug(f"Trying to update data for {self!s}")
         if data is None:
             raise DekerArrayError("Updating data shall not be None")
 
         data = self.__array_adapter._process_data(
             self.__array.dtype, self.__array.shape, data, self.__bounds
         )
 
-        results = self.__adapter.executor.map(
-            _update,
-            [
-                ArrayPositionedData(vpos, array_bounds, data[data_bounds])
-                for vpos, array_bounds, data_bounds in self.__arrays
-            ],
-        )
-        try:
-            list(results)
-        except Exception as e:
-            if isinstance(e, DekerLockError):
-                raise e
-            else:
-                raise DekerVSubsetError(
-                    f"ATTENTION: Data in {self!s} IS NOW CORRUPTED due to the exception above"
-                ).with_traceback(e.__traceback__)
+        positions = [
+            ArrayPositionedData(vpos, array_bounds, data[data_bounds])
+            for vpos, array_bounds, data_bounds in self.__arrays
+        ]
+        futures = [self.__adapter.executor.submit(_update, position) for position in positions]
+
+        exceptions = []
+        for future in futures:
+            try:
+                future.result()
+            except Exception as e:
+                exceptions.append(repr(e) + "\n" + traceback.format_exc(-1))
+
+        if exceptions:
+            raise DekerVSubsetError(
+                f"ATTENTION: Data in {self!s} MAY BE NOW CORRUPTED due to the exceptions occurred in threads",
+                exceptions,
+            )
+
         self.logger.info(f"{self!s} data updated OK")
```

### Comparing `deker-1.1.5/deker/tools/__init__.py` & `deker-1.1.6/deker/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/tools/array.py` & `deker-1.1.6/deker/tools/array.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/tools/decorators.py` & `deker-1.1.6/deker/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/tools/path.py` & `deker-1.1.6/deker/tools/path.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/tools/schema.py` & `deker-1.1.6/deker/tools/schema.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/tools/time.py` & `deker-1.1.6/deker/tools/time.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/types/__init__.py` & `deker-1.1.6/deker/types/__init__.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/types/private/__init__.py` & `deker-1.1.6/deker/types/private/__init__.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/types/private/classes.py` & `deker-1.1.6/deker/types/private/classes.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/types/private/enums.py` & `deker-1.1.6/deker/types/private/enums.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/types/private/shell.py` & `deker-1.1.6/deker/types/private/shell.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/types/private/typings.py` & `deker-1.1.6/deker/types/private/typings.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/types/public/classes.py` & `deker-1.1.6/deker/types/public/classes.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/uri.py` & `deker-1.1.6/deker/uri.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/deker/validators.py` & `deker-1.1.6/deker/validators.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 from typing import TYPE_CHECKING, Optional, Tuple, Union
 
 from deker_tools.time import get_utc
 
 from deker.dimensions import Dimension, TimeDimension
 from deker.errors import DekerValidationError
+from deker.types import DTypeEnum
+
 
 if TYPE_CHECKING:
     from deker.schemas import ArraySchema, AttributeSchema, VArraySchema
 
 
 def process_time_dimension_attrs(attributes: dict, attr_name: str) -> datetime.datetime:
     """Validate time attribute and return its value.
@@ -38,53 +40,94 @@
     if time_attribute is None:
         raise DekerValidationError("No start value provided for time dimension")
     if time_attribute.tzinfo is None or time_attribute.tzinfo != datetime.timezone.utc:
         time_attribute = get_utc(time_attribute)
     return time_attribute
 
 
+def __validate_attribute_type(attribute: object) -> None:
+    """Validate attribute type over allowed types.
+
+    :param attribute: attribute object
+    """
+    if isinstance(attribute, tuple):
+        for attr in attribute:
+            __validate_attribute_type(attr)
+
+    dtype = type(attribute)
+    if attribute is not None:
+        try:
+            DTypeEnum(dtype).value
+        except (ValueError, KeyError):
+            raise DekerValidationError(f"Invalid dtype value {dtype}")
+
+
 def __process_attributes_types(
     attrs_schema: Tuple["AttributeSchema", ...],
     primary_attributes: dict,
     custom_attributes: dict,
+    dimensions: list,
 ) -> None:
     """Validate attributes types over schema and update dicts if needed.
 
     :param attrs_schema: attributes schema
     :param primary_attributes: primary attributes to validate
     :param custom_attributes: custom attributes to validate
+    :param dimensions: list of dimensions
     """
+    from deker.schemas import TimeDimensionSchema
+
     attributes = {**primary_attributes, **custom_attributes}
     for attr in attrs_schema:
         if attr.primary:
             # check if primary attribute is not missing and its type
             if attr.name not in attributes:
                 raise DekerValidationError(f"Key attribute missing: {attr.name}")
             if not isinstance(primary_attributes[attr.name], attr.dtype):
                 raise DekerValidationError(
                     f'Key attribute "{attr.name}" invalid type: {type(primary_attributes[attr.name])}; '
                     f"expected {attr.dtype}"
                 )
 
+            # validate tuples contents type
+            if isinstance(primary_attributes[attr.name], tuple):
+                __validate_attribute_type(primary_attributes[attr.name])
+
         else:
             # check if custom attribute is not missing and its type
             custom_attribute = custom_attributes.get(attr.name)
             if custom_attribute is not None and not isinstance(custom_attribute, attr.dtype):
                 raise DekerValidationError(
                     f'Custom attribute "{attr.name}" invalid type {type(custom_attributes[attr.name])}; '
                     f"expected {attr.dtype}"
                 )
 
             if custom_attribute is None:
                 if attr.dtype == datetime.datetime:
-                    raise DekerValidationError(f'Custom attribute "{attr.name}" cannot be None')
+                    for d in dimensions:
+                        if (
+                            isinstance(d, TimeDimensionSchema)
+                            and isinstance(d.start_value, str)
+                            and d.start_value.startswith("$" + attr.name)
+                        ):
+                            raise DekerValidationError(
+                                f'Custom attribute "{attr.name}" cannot be None'
+                            )
                 custom_attributes[attr.name] = None
 
-        # convert attribute with datetime to utc if needed
-        if attr.dtype == datetime.datetime and attr.name in attributes:
+            # validate tuples
+            if isinstance(custom_attributes[attr.name], tuple):
+                __validate_attribute_type(custom_attributes[attr.name])
+
+        # convert datetime attribute with set datetime value to utc if needed
+        if (
+            attr.dtype == datetime.datetime
+            and attr.name in attributes
+            and attributes[attr.name] is not None
+        ):
             try:
                 utc = get_utc(attributes[attr.name])
                 if attr.primary:
                     primary_attributes[attr.name] = utc
                 else:
                     custom_attributes[attr.name] = utc
             except (ValueError, TypeError) as e:
@@ -134,15 +177,15 @@
     extra_names = set(attributes.keys()).difference(schema_attrs_names)
     if extra_names:
         raise DekerValidationError(
             f"Setting additional attributes not listed in schema is not allowed. "
             f"Invalid attributes: {sorted(extra_names)}"
         )
     __process_attributes_types(
-        attrs_schema, primary_attributes, custom_attributes  # type: ignore[arg-type]
+        attrs_schema, primary_attributes, custom_attributes, schema.dimensions  # type: ignore[arg-type]
     )
     return primary_attributes, custom_attributes
 
 
 def validate_custom_attributes_update(
     schema: Union["ArraySchema", "VArraySchema"],
     dimensions: Tuple[Union[Dimension, TimeDimension], ...],
```

### Comparing `deker-1.1.5/deker/warnings.py` & `deker-1.1.6/deker/warnings.py`

 * *Files identical despite different names*

### Comparing `deker-1.1.5/pyproject.toml` & `deker-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
                                 ###############
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
-version = "1.1.5"  # a placeholder for poetry CI dynamic versionning plugin
+version = "1.1.6"  # a placeholder for poetry CI dynamic versionning plugin
 name = "deker"
 packages = [{ include = "deker" }]
 description = "Multidimensional arrays storage engine"
 authors = ["OpenWeather <info@openweathermap.org>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 documentation = 'https://docs.deker.io/'
@@ -58,15 +58,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 attrs = "^23.1.0"
 typing-extensions = "^4.4.0"
 tqdm = "^4.64.1"
 psutil = "^5.9.5"
-deker-local-adapters = "^1.0.1"
+deker-local-adapters = "^1.1.1"
 deker-server-adapters = {version = "^1.0.0", optional = true}
 deker-shell = { version = "^1.0.0", optional = true }
 xarray = {version = "^2023.5.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "23.1.0"
 coverage = "7.1.0"
@@ -170,15 +170,15 @@
 # https://flake8.pycqa.org/en/latest/
 # https://pypi.org/project/flake8-bugbear
 # https://pypi.org/project/flake8-docstrings/
 # https://pypi.org/project/flake8-import-order/
 # https://pypi.org/project/flake8-pytest-style/
 # https://pypi.org/project/pep8-naming/
 min_python_version = 3.9
-max-complexity = 15
+max-complexity = 16
 max-doc-length = 120
 max-line-length = 120
 strictness = "full"
 docstring_style = "sphinx"
 docstring-convention = "pep257"
 application_import_names = "deker"
 import-order-style = "pycharm"
@@ -199,14 +199,15 @@
 extend-select = ["D417"]
 per-file-ignores = [
     "__init__.py: D104, F401, F403, F405, I100",
     "deker/integrity.py: E501",
     "deker/private/types/shell.py: D205, D400",
     "deker/collection.py: D401",
     "deker/subset.py: DAR101, E203",
+    "deker/errors.py: D301",
 ]
 ignore = [
     "B012",
     "B019",
     "D100",
     "D104",
     "D105",
@@ -225,14 +226,15 @@
     "DAR401",
     "DAR501",
     "I101",
     "I201",
     "I202",
     "N807",
     "N813",
+    "N818",
     "W503",
     "W504",
 ]
 
 [tool.pycln]  # imports linter
 # https://hadialqattan.github.io/pycln/#/README
 all = true
```

### Comparing `deker-1.1.5/PKG-INFO` & `deker-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deker
-Version: 1.1.5
+Version: 1.1.6
 Summary: Multidimensional arrays storage engine
 Home-page: https://deker.io/
 License: GPL-3.0-only
 Author: OpenWeather
 Author-email: info@openweathermap.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: server-adapters
 Provides-Extra: shell
 Provides-Extra: xarray
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
-Requires-Dist: deker-local-adapters (>=1.0.1,<2.0.0)
+Requires-Dist: deker-local-adapters (>=1.1.1,<2.0.0)
 Requires-Dist: deker-server-adapters (>=1.0.0,<2.0.0) ; extra == "server-adapters" or extra == "all"
 Requires-Dist: deker-shell (>=1.0.0,<2.0.0) ; extra == "shell" or extra == "all"
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: xarray (>=2023.5.0,<2024.0.0) ; extra == "xarray" or extra == "all"
 Project-URL: Documentation, https://docs.deker.io/
```


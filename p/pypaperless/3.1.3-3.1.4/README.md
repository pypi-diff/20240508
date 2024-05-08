# Comparing `tmp/pypaperless-3.1.3.tar.gz` & `tmp/pypaperless-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaperless-3.1.3.tar", max compression
+gzip compressed data, was "pypaperless-3.1.4.tar", max compression
```

## Comparing `pypaperless-3.1.3.tar` & `pypaperless-3.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1070 2024-04-29 08:17:32.149712 pypaperless-3.1.3/LICENSE.md
--rw-r--r--   0        0        0     2605 2024-04-29 08:17:32.149712 pypaperless-3.1.3/README.md
--rw-r--r--   0        0        0     3720 2024-04-29 08:17:45.489933 pypaperless-3.1.3/pyproject.toml
--rw-r--r--   0        0        0       73 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/__init__.py
--rw-r--r--   0        0        0    11483 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/api.py
--rw-r--r--   0        0        0     3876 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/const.py
--rw-r--r--   0        0        0     1741 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/exceptions.py
--rw-r--r--   0        0        0      899 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/helpers.py
--rw-r--r--   0        0        0     1260 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/__init__.py
--rw-r--r--   0        0        0     3724 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/base.py
--rw-r--r--   0        0        0     6788 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/classifiers.py
--rw-r--r--   0        0        0     5891 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/common.py
--rw-r--r--   0        0        0     1500 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/config.py
--rw-r--r--   0        0        0     1654 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/custom_fields.py
--rw-r--r--   0        0        0    19742 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/documents.py
--rw-r--r--   0        0        0       93 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/generators/__init__.py
--rw-r--r--   0        0        0     2112 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/generators/page.py
--rw-r--r--   0        0        0     3041 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mails.py
--rw-r--r--   0        0        0       37 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/__init__.py
--rw-r--r--   0        0        0      288 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/helpers/__init__.py
--rw-r--r--   0        0        0     1091 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/helpers/callable.py
--rw-r--r--   0        0        0      916 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/helpers/draftable.py
--rw-r--r--   0        0        0     2744 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/helpers/iterable.py
--rw-r--r--   0        0        0      765 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/helpers/securable.py
--rw-r--r--   0        0        0      413 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/models/__init__.py
--rw-r--r--   0        0        0     2169 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/models/creatable.py
--rw-r--r--   0        0        0      382 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/models/data_fields.py
--rw-r--r--   0        0        0      755 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/models/deletable.py
--rw-r--r--   0        0        0      742 2024-04-29 08:17:32.153712 pypaperless-3.1.3/src/pypaperless/models/mixins/models/securable.py
--rw-r--r--   0        0        0     2641 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/models/mixins/models/updatable.py
--rw-r--r--   0        0        0     2660 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/models/pages.py
--rw-r--r--   0        0        0     2201 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/models/permissions.py
--rw-r--r--   0        0        0     1390 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/models/saved_views.py
--rw-r--r--   0        0        0     1856 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/models/share_links.py
--rw-r--r--   0        0        0     1773 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/models/status.py
--rw-r--r--   0        0        0     2735 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/models/tasks.py
--rw-r--r--   0        0        0     7330 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/models/utils/__init__.py
--rw-r--r--   0        0        0     4564 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/models/workflows.py
--rw-r--r--   0        0        0        0 2024-04-29 08:17:32.157712 pypaperless-3.1.3/src/pypaperless/py.typed
--rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 pypaperless-3.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-08 16:11:43.847977 pypaperless-3.1.4/LICENSE.md
+-rw-r--r--   0        0        0     2605 2024-05-08 16:11:43.847977 pypaperless-3.1.4/README.md
+-rw-r--r--   0        0        0     3720 2024-05-08 16:11:56.340014 pypaperless-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/__init__.py
+-rw-r--r--   0        0        0    11483 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/api.py
+-rw-r--r--   0        0        0     3876 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/const.py
+-rw-r--r--   0        0        0     1741 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/exceptions.py
+-rw-r--r--   0        0        0      899 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/helpers.py
+-rw-r--r--   0        0        0     1260 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/models/__init__.py
+-rw-r--r--   0        0        0     3724 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/models/base.py
+-rw-r--r--   0        0        0     6788 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/models/classifiers.py
+-rw-r--r--   0        0        0     5891 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/models/common.py
+-rw-r--r--   0        0        0     1500 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/models/config.py
+-rw-r--r--   0        0        0     1654 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/models/custom_fields.py
+-rw-r--r--   0        0        0    19726 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/models/documents.py
+-rw-r--r--   0        0        0       93 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/models/generators/__init__.py
+-rw-r--r--   0        0        0     2112 2024-05-08 16:11:43.847977 pypaperless-3.1.4/src/pypaperless/models/generators/page.py
+-rw-r--r--   0        0        0     3041 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mails.py
+-rw-r--r--   0        0        0       37 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/helpers/__init__.py
+-rw-r--r--   0        0        0     1009 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/helpers/callable.py
+-rw-r--r--   0        0        0      916 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/helpers/draftable.py
+-rw-r--r--   0        0        0     2893 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/helpers/iterable.py
+-rw-r--r--   0        0        0      765 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/helpers/securable.py
+-rw-r--r--   0        0        0      413 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/models/__init__.py
+-rw-r--r--   0        0        0     2169 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/models/creatable.py
+-rw-r--r--   0        0        0      382 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/models/data_fields.py
+-rw-r--r--   0        0        0      755 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/models/deletable.py
+-rw-r--r--   0        0        0      742 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/models/securable.py
+-rw-r--r--   0        0        0     2641 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/mixins/models/updatable.py
+-rw-r--r--   0        0        0     2660 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/pages.py
+-rw-r--r--   0        0        0     2201 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/permissions.py
+-rw-r--r--   0        0        0     1390 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/saved_views.py
+-rw-r--r--   0        0        0     1856 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/share_links.py
+-rw-r--r--   0        0        0     1773 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/status.py
+-rw-r--r--   0        0        0     2735 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/tasks.py
+-rw-r--r--   0        0        0     7307 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/utils/__init__.py
+-rw-r--r--   0        0        0     4564 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/models/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-08 16:11:43.851978 pypaperless-3.1.4/src/pypaperless/py.typed
+-rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 pypaperless-3.1.4/PKG-INFO
```

### Comparing `pypaperless-3.1.3/LICENSE.md` & `pypaperless-3.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/README.md` & `pypaperless-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/pyproject.toml` & `pypaperless-3.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.poetry]
 name = "pypaperless"
-version = "3.1.3"
+version = "3.1.4"
 description = "Little api client for paperless(-ngx)."
 authors = ["Tobias Schulz <public.dev@tbsch.de>"]
 maintainers = ["Tobias Schulz <public.dev@tbsch.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tb1337/paperless-api"
 repository = "https://github.com/tb1337/paperless-api"
```

### Comparing `pypaperless-3.1.3/src/pypaperless/api.py` & `pypaperless-3.1.4/src/pypaperless/api.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/const.py` & `pypaperless-3.1.4/src/pypaperless/const.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/exceptions.py` & `pypaperless-3.1.4/src/pypaperless/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/helpers.py` & `pypaperless-3.1.4/src/pypaperless/helpers.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/__init__.py` & `pypaperless-3.1.4/src/pypaperless/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/base.py` & `pypaperless-3.1.4/src/pypaperless/models/base.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/classifiers.py` & `pypaperless-3.1.4/src/pypaperless/models/classifiers.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/common.py` & `pypaperless-3.1.4/src/pypaperless/models/common.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/config.py` & `pypaperless-3.1.4/src/pypaperless/models/config.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/custom_fields.py` & `pypaperless-3.1.4/src/pypaperless/models/custom_fields.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/documents.py` & `pypaperless-3.1.4/src/pypaperless/models/documents.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,15 +607,15 @@
 
     async def get_next_asn(self) -> int:
         """Request the next archive serial number from DRF."""
         async with self._api.request("get", API_PATH["documents_next_asn"]) as res:
             try:
                 res.raise_for_status()
                 return int(await res.text())
-            except Exception as exc:  # noqa: BLE001
+            except Exception as exc:
                 raise AsnRequestError from exc
 
     async def more_like(self, pk: int) -> AsyncGenerator[Document, None]:
         """Lookup documents similar to the given document pk.
 
         Shortcut function. Same behaviour is possible using `reduce()`.
```

### Comparing `pypaperless-3.1.3/src/pypaperless/models/generators/page.py` & `pypaperless-3.1.4/src/pypaperless/models/generators/page.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/mails.py` & `pypaperless-3.1.4/src/pypaperless/models/mails.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/mixins/helpers/callable.py` & `pypaperless-3.1.4/src/pypaperless/models/mixins/helpers/callable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """CallableMixin for PyPaperless helpers."""
 
 from pypaperless.models.base import HelperProtocol, ResourceT
 
-from .securable import SecurableMixin
-
 
 class CallableMixin(HelperProtocol[ResourceT]):
     """Provide methods for calling a specific resource item."""
 
     async def __call__(
         self,
         pk: int,
@@ -29,13 +27,13 @@
         """
         data = {
             "id": pk,
         }
         item = self._resource_cls.create_with_data(self._api, data)
 
         # set requesting full permissions
-        if SecurableMixin in type(self).__bases__ and getattr(self, "_request_full_perms", False):
+        if getattr(self, "_request_full_perms", False):
             item._params.update({"full_perms": "true"})  # noqa: SLF001
 
         if not lazy:
             await item.load()
         return item
```

### Comparing `pypaperless-3.1.3/src/pypaperless/models/mixins/helpers/draftable.py` & `pypaperless-3.1.4/src/pypaperless/models/mixins/helpers/draftable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/mixins/helpers/iterable.py` & `pypaperless-3.1.4/src/pypaperless/models/mixins/helpers/iterable.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,8 +90,12 @@
         ```
 
         """
         params = getattr(self, "_aiter_filters", None) or {}
         params.setdefault("page", page)
         params.setdefault("page_size", page_size)
 
+        # set requesting full permissions
+        if getattr(self, "_request_full_perms", False):
+            params.update({"full_perms": "true"})
+
         return PageGenerator(self._api, self._api_path, self._resource_cls, params=params)
```

### Comparing `pypaperless-3.1.3/src/pypaperless/models/mixins/helpers/securable.py` & `pypaperless-3.1.4/src/pypaperless/models/mixins/helpers/securable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/mixins/models/creatable.py` & `pypaperless-3.1.4/src/pypaperless/models/mixins/models/creatable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/mixins/models/deletable.py` & `pypaperless-3.1.4/src/pypaperless/models/mixins/models/deletable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/mixins/models/securable.py` & `pypaperless-3.1.4/src/pypaperless/models/mixins/models/securable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/mixins/models/updatable.py` & `pypaperless-3.1.4/src/pypaperless/models/mixins/models/updatable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/pages.py` & `pypaperless-3.1.4/src/pypaperless/models/pages.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/permissions.py` & `pypaperless-3.1.4/src/pypaperless/models/permissions.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/saved_views.py` & `pypaperless-3.1.4/src/pypaperless/models/saved_views.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/share_links.py` & `pypaperless-3.1.4/src/pypaperless/models/share_links.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/status.py` & `pypaperless-3.1.4/src/pypaperless/models/status.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/tasks.py` & `pypaperless-3.1.4/src/pypaperless/models/tasks.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/src/pypaperless/models/utils/__init__.py` & `pypaperless-3.1.4/src/pypaperless/models/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 def _str_to_date(datestr: str) -> date:
     """Parse date from string."""
     return date.fromisoformat(datestr)
 
 
 def _dateobj_to_str(value: date | datetime) -> str:
     """Parse string from date objects."""
-    return value.isoformat().replace("+00:00", "Z")
+    return value.isoformat()
 
 
 def object_to_dict_value(value: Any) -> Any:
     """Convert object values to their correspondending json values."""
 
     def _clean_value(_value_obj: Any) -> Any:
         if isinstance(_value_obj, dict):
```

### Comparing `pypaperless-3.1.3/src/pypaperless/models/workflows.py` & `pypaperless-3.1.4/src/pypaperless/models/workflows.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.3/PKG-INFO` & `pypaperless-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypaperless
-Version: 3.1.3
+Version: 3.1.4
 Summary: Little api client for paperless(-ngx).
 Home-page: https://github.com/tb1337/paperless-api
 License: MIT
 Keywords: library,async,api-client,python3,paperless-ngx
 Author: Tobias Schulz
 Author-email: public.dev@tbsch.de
 Maintainer: Tobias Schulz
```


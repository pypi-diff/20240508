# Comparing `tmp/akatosh-3.0.5.tar.gz` & `tmp/akatosh-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akatosh-3.0.5.tar", max compression
+gzip compressed data, was "akatosh-3.0.6.tar", max compression
```

## Comparing `akatosh-3.0.5.tar` & `akatosh-3.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      544 2024-05-05 12:01:25.677659 akatosh-3.0.5/Akatosh/__init__.py
--rw-r--r--   0        0        0     5333 2024-05-01 06:18:14.039666 akatosh-3.0.5/Akatosh/entity.py
--rw-r--r--   0        0        0     6273 2024-05-01 06:22:47.670314 akatosh-3.0.5/Akatosh/event.py
--rw-r--r--   0        0        0     5230 2024-05-01 01:03:37.391211 akatosh-3.0.5/Akatosh/resource.py
--rw-r--r--   0        0        0     6052 2024-05-01 08:00:36.765790 akatosh-3.0.5/Akatosh/universe.py
--rw-r--r--   0        0        0      321 2024-05-05 12:01:19.437729 akatosh-3.0.5/pyproject.toml
--rw-r--r--   0        0        0     2324 2024-05-01 01:03:37.392209 akatosh-3.0.5/README.md
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 akatosh-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0      544 2024-05-08 01:04:21.582527 akatosh-3.0.6/Akatosh/__init__.py
+-rw-r--r--   0        0        0     5333 2024-05-08 01:04:21.583527 akatosh-3.0.6/Akatosh/entity.py
+-rw-r--r--   0        0        0     6273 2024-05-08 01:05:22.105174 akatosh-3.0.6/Akatosh/event.py
+-rw-r--r--   0        0        0     5230 2024-04-22 03:53:18.056982 akatosh-3.0.6/Akatosh/resource.py
+-rw-r--r--   0        0        0     6052 2024-05-08 01:04:21.585530 akatosh-3.0.6/Akatosh/universe.py
+-rw-r--r--   0        0        0      321 2024-05-08 01:06:10.955605 akatosh-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2324 2024-04-19 03:36:27.289023 akatosh-3.0.6/README.md
+-rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 akatosh-3.0.6/PKG-INFO
```

### Comparing `akatosh-3.0.5/Akatosh/__init__.py` & `akatosh-3.0.6/Akatosh/__init__.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.5/Akatosh/entity.py` & `akatosh-3.0.6/Akatosh/entity.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.5/Akatosh/event.py` & `akatosh-3.0.6/Akatosh/event.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,21 +74,21 @@
 
             if (
                 self.started == True
                 and self.ended == False
                 and self.paused == False
                 and self.next == Mundus.time
             ):
-                self._next += max(Mundus.time_step, self.step)
-                self._next = round(self._next, Mundus.time_resolution)
                 if asyncio.iscoroutinefunction(self._action):
                     await self._action()
                 else:
                     self._action()
                 self._acted = True
+                self._next += max(Mundus.time_step, self.step)
+                self._next = round(self._next, Mundus.time_resolution)
                 logger.debug(f"Event {self} acted.")
                 if self._once == True:
                     self._ended = True
                     logger.debug(f"Event {self} ended.")
                     return
 
             if self.ended == False:
```

### Comparing `akatosh-3.0.5/Akatosh/resource.py` & `akatosh-3.0.6/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.5/Akatosh/universe.py` & `akatosh-3.0.6/Akatosh/universe.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.5/README.md` & `akatosh-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.5/PKG-INFO` & `akatosh-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 3.0.5
+Version: 3.0.6
 Summary: 
 Author: Innovation Central Perth Maintainer
 Author-email: ryf0510@live.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


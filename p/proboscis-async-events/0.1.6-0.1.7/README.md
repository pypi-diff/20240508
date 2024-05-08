# Comparing `tmp/proboscis_async_events-0.1.6.tar.gz` & `tmp/proboscis_async_events-0.1.7.tar.gz`

## Comparing `proboscis_async_events-0.1.6.tar` & `proboscis_async_events-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.python-version
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/requirements-dev.lock
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/requirements.lock
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/.gitignore
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/modules.xml
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/proboscis-async-events.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/vcs.xml
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/workspace.xml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/codeStyles/Project.xml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/src/proboscis_async_events/__init__.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/src/proboscis_async_events/messaging.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/test/test_messaging.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/.gitignore
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/README.md
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.python-version
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/requirements-dev.lock
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/requirements.lock
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.idea/.gitignore
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.idea/modules.xml
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.idea/proboscis-async-events.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.idea/vcs.xml
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.idea/workspace.xml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.idea/codeStyles/Project.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/src/proboscis_async_events/__init__.py
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/src/proboscis_async_events/messaging.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/test/test_messaging.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/.gitignore
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/README.md
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 proboscis_async_events-0.1.7/PKG-INFO
```

### Comparing `proboscis_async_events-0.1.6/.idea/proboscis-async-events.iml` & `proboscis_async_events-0.1.7/.idea/proboscis-async-events.iml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.6/.idea/workspace.xml` & `proboscis_async_events-0.1.7/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.6/.idea/inspectionProfiles/Project_Default.xml` & `proboscis_async_events-0.1.7/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.6/src/proboscis_async_events/messaging.py` & `proboscis_async_events-0.1.7/src/proboscis_async_events/messaging.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self.value_empty = Event()
         self.value_empty.set()
         self.entered = Event()
         self.message = _Item("waiting", None)
 
     async def __aenter__(self):
         self.entered.set()
+        return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.unsubscribe()
         self.entered.clear()
 
 
     async def tell(self, message: _Item):
```

### Comparing `proboscis_async_events-0.1.6/test/test_messaging.py` & `proboscis_async_events-0.1.7/test/test_messaging.py`

 * *Files identical despite different names*

### Comparing `proboscis_async_events-0.1.6/pyproject.toml` & `proboscis_async_events-0.1.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "proboscis-async-events"
-version = "0.1.6"
+version = "0.1.7"
 description = "Add your description here"
 authors = [
     { name = "proboscis", email = "nameissoap@gmail.com" }
 ]
 dependencies = [
     "pampy>=0.3.0",
     "pytest>=8.2.0",
```


# Comparing `tmp/ptsqld-0.1.1.tar.gz` & `tmp/ptsqld-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsqld-0.1.1.tar", max compression
+gzip compressed data, was "ptsqld-0.1.2.tar", max compression
```

## Comparing `ptsqld-0.1.1.tar` & `ptsqld-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      810 2024-04-26 05:49:16.395339 ptsqld-0.1.1/README.md
--rw-r--r--   0        0        0     2072 2024-04-26 18:40:36.240506 ptsqld-0.1.1/ptsqld/__init__.py
--rw-r--r--   0        0        0     1462 2024-03-12 09:17:42.025413 ptsqld-0.1.1/ptsqld/__init__.py~
--rw-r--r--   0        0        0      487 2024-03-13 20:19:06.329725 ptsqld-0.1.1/ptsqld/__main__.py~
--rw-r--r--   0        0        0      459 2024-04-26 18:40:55.420907 ptsqld-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 ptsqld-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      810 2024-04-26 05:49:16.395339 ptsqld-0.1.2/README.md
+-rw-r--r--   0        0        0     3934 2024-05-08 20:05:04.861387 ptsqld-0.1.2/ptsqld/__init__.py
+-rw-r--r--   0        0        0     1462 2024-03-12 09:17:42.025413 ptsqld-0.1.2/ptsqld/__init__.py~
+-rw-r--r--   0        0        0      487 2024-03-13 20:19:06.329725 ptsqld-0.1.2/ptsqld/__main__.py~
+-rw-r--r--   0        0        0      515 2024-05-08 19:46:15.927359 ptsqld-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 ptsqld-0.1.2/PKG-INFO
```

### Comparing `ptsqld-0.1.1/README.md` & `ptsqld-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ptsqld-0.1.1/ptsqld/__init__.py` & `ptsqld-0.1.2/ptsqld/__init__.py~`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,56 @@
-from os.path import exists
-from datetime import datetime
 from sqlton import parse
 from sqlton.ast import Select
 from sqletic import Engine
+from pickle import load, dump
 from functools import partialmethod
-from echovault import Vault 
-from dulwich.object_store import DiskObjectStore
-from dulwich.refs import DiskRefsContainer
-    
+from readerwriterlock.rwlock import RWLockRead
+
 def __forward(self, method_name, *args, **kwargs):
     if method_name.startswith('execute'):
         statement, = parse(args[0])
         
-        return getattr(self._engine, method_name)(*args, *kwargs)
+        if statement is Select:
+            lock = self.lock.gen_rlock()
+        else:
+            lock = self.lock.gen_wlock()
+        
+        with lock:
+            return getattr(self._engine, method_name)(*args, *kwargs)
+            
     else:
         return getattr(self._engine, method_name)(*args, *kwargs)
 
+
 class Cursor:
-    def __init__(self, tables, engine):
+    def __init__(engine, lock):
         self._engine = engine
-        self._tables = tables
-
-    def __iter__(self):
-        yield from iter(self._engine)
+        self._lock = lock
 
-    @property
-    def description(self):
-        return self._engine.description
-
-    def close(self):
-        ...
+    __iter__ = partialmethod(forward, '__iter__')
 
 class Connection:
-    def __init__(self, path, branch='main'):
+    def __init__(self, path):
         self.__path = path
-
-        if exists(path + '/.git'):
-            path += '/.git/'
-
-        self.__tables = Vault(DiskObjectStore(path + '/objects/'),
-                              DiskRefsContainer(path + '/'),
-                              ref=branch)
+        
+        with open(self.__path, 'rb') as file: 
+            self.__tables = load(file)
 
         self._engine = Engine(self.__tables)
+        self._lock = RWLockRead()
 
     def close(self):
-        ...
-
-    def commit(self):
-        if self.__tables.tree.id == self.__tables.object_store[self.__tables.refs[self.__tables.ref]].tree:
-            # nothing to commit as the hash of the tree did not change
-            return
-        
-        self.__tables.commit(message=f'update at {datetime.now().isoformat()}')
-
-    def rollback(self):
-        self.__tables.rollback()
+        with open(self.path, 'wb') as file:
+            dumps(self.tables)
 
-    def cursor(self):
-        return Cursor(self.__tables, self._engine)
+    __del__ = close
 
-    @property
-    def description(self):
-        return self._engine.description
+    def cursor():
+        return Cursor(self._engine, self._lock)
 
 for method_name in {'execute', 'fetchone', 'fetchmany', 'fetchall'}:
-    setattr(Cursor, method_name, partialmethod(__forward, method_name))
-    setattr(Connection, method_name, partialmethod(__forward, method_name))
+    setattr(Cursor, partialmethod(__forward, method_name))
+    setattr(Connection, partialmethod(__forward, method_name))
 
 def connect(path):
-    return Connection(path)
+    
+
```

### Comparing `ptsqld-0.1.1/PKG-INFO` & `ptsqld-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptsqld
-Version: 0.1.1
+Version: 0.1.2
 Summary: An SQL Database which shall avoid any further PTSD associated to other SQL Database setup (understand flexible, simple)
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


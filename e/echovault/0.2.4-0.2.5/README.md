# Comparing `tmp/echovault-0.2.4.tar.gz` & `tmp/echovault-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echovault-0.2.4.tar", max compression
+gzip compressed data, was "echovault-0.2.5.tar", max compression
```

## Comparing `echovault-0.2.4.tar` & `echovault-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.4/README.md
--rw-r--r--   0        0        0       34 2024-04-25 18:14:25.800920 echovault-0.2.4/echovault/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.4/echovault/__init__.py~
--rw-r--r--   0        0        0     1028 2024-04-28 19:08:59.099761 echovault-0.2.4/echovault/_container.py
--rw-r--r--   0        0        0     1030 2024-04-24 19:49:03.244111 echovault-0.2.4/echovault/_container.py~
--rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.4/echovault/db.py~
--rw-r--r--   0        0        0     2733 2024-04-30 18:15:33.064347 echovault-0.2.4/echovault/dict.py
--rw-r--r--   0        0        0     2283 2024-04-23 18:43:20.644733 echovault-0.2.4/echovault/dict.py~
--rw-r--r--   0        0        0     2305 2024-04-30 19:41:38.740513 echovault-0.2.4/echovault/list.py
--rw-r--r--   0        0        0     1176 2024-04-24 19:49:34.034385 echovault-0.2.4/echovault/list.py~
--rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.4/echovault/table.py~
--rw-r--r--   0        0        0     6912 2024-05-05 18:15:23.514138 echovault-0.2.4/echovault/vault.py
--rw-r--r--   0        0        0     8070 2024-05-05 18:08:25.266920 echovault-0.2.4/echovault/vault.py.bck
--rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.4/echovault/vault.py~
--rw-r--r--   0        0        0      380 2024-05-05 18:21:21.324123 echovault-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.5/README.md
+-rw-r--r--   0        0        0       34 2024-04-25 18:14:25.800920 echovault-0.2.5/echovault/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.5/echovault/__init__.py~
+-rw-r--r--   0        0        0     1028 2024-04-28 19:08:59.099761 echovault-0.2.5/echovault/_container.py
+-rw-r--r--   0        0        0     1030 2024-04-24 19:49:03.244111 echovault-0.2.5/echovault/_container.py~
+-rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.5/echovault/db.py~
+-rw-r--r--   0        0        0     2733 2024-04-30 18:15:33.064347 echovault-0.2.5/echovault/dict.py
+-rw-r--r--   0        0        0     2283 2024-04-23 18:43:20.644733 echovault-0.2.5/echovault/dict.py~
+-rw-r--r--   0        0        0     2305 2024-04-30 19:41:38.740513 echovault-0.2.5/echovault/list.py
+-rw-r--r--   0        0        0     1176 2024-04-24 19:49:34.034385 echovault-0.2.5/echovault/list.py~
+-rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.5/echovault/table.py~
+-rw-r--r--   0        0        0     7210 2024-05-08 19:07:16.968735 echovault-0.2.5/echovault/vault.py
+-rw-r--r--   0        0        0     8070 2024-05-05 18:08:25.266920 echovault-0.2.5/echovault/vault.py.bck
+-rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.5/echovault/vault.py~
+-rw-r--r--   0        0        0      380 2024-05-08 19:11:10.643977 echovault-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.5/PKG-INFO
```

### Comparing `echovault-0.2.4/README.md` & `echovault-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/echovault/_container.py` & `echovault-0.2.5/echovault/_container.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/echovault/_container.py~` & `echovault-0.2.5/echovault/_container.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/echovault/dict.py` & `echovault-0.2.5/echovault/dict.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/echovault/dict.py~` & `echovault-0.2.5/echovault/dict.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/echovault/list.py` & `echovault-0.2.5/echovault/list.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/echovault/list.py~` & `echovault-0.2.5/echovault/list.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/echovault/table.py~` & `echovault-0.2.5/echovault/table.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/echovault/vault.py` & `echovault-0.2.5/echovault/vault.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 except:
     def getuid():
         return None
 
     def getgid():
         return None
 
+ref_head = b'refs/heads/'
+    
 def walk_ancestor(object_store, commit):
     for identifier in commit.parents:
         yield identifier
 
     for identifier in commit.parents:
         yield from walk(object_store, object_store[identifier])
     
@@ -61,16 +63,20 @@
     
     def __init__(self, object_store, refs, *, tree:Tree=None, ref=None):
         super().__init__(object_store, None, None, tree)
         self.refs = refs
         if ref is not None:
             self.checkout(ref)
         else:
-            self.ref = None
+            self._ref = None
 
+    @property
+    def ref(self):
+        return self._ref[len(ref_head):].decode('utf-8')
+            
     def __getitem__(self, name:str):
         identifier = self.encode(name)
         _, oid = self.tree[identifier]
         tree = self.object_store[oid]
         return List(self.object_store,
                      self,
                      identifier,
@@ -105,43 +111,47 @@
 
     def __repr__(self):
         return repr({key: value
                      for key, value
                      in self.items()})
             
     def rollback(self):
-        if self.ref is None:
+        if self._ref is None:
             self.tree = Tree()
         else:
             self.tree = self.object_store[self.object_store[self.refs[ref]].tree]
 
-    def checkout(self, ref):
-        tree = Tree()
+    def checkout(self, ref, branch=False):
+        tree = self.tree
         
-        ref = b'refs/heads/' + ref.encode('utf-8')
+        ref = ref_head + ref.encode('utf-8')
         
         if ref in self.refs:
             tree = self.object_store[self.object_store[self.refs[ref]].tree]
-        
-        self.ref = ref
+        elif branch:
+            self.refs[ref] = self.refs[self._ref]
+        else:
+            raise ValueError(f"No {ref} branch is existing !")
+            
+        self._ref = ref
         self.tree = tree
         
             
     def commit(self,
                ref:Optional[str]=None,
                message:Optional[str]='',
                author:Optional[str]=None,
                committer:Optional[str]=None,
                time_:Optional[int]=None,
                timezone:Optional[int]=None,
                ):
         if ref is None:
-            ref = self.ref
+            ref = self._ref
         else:
-            ref = b'refs/heads/' + ref.encode('utf-8')
+            ref = ref_head + ref.encode('utf-8')
             
         commit = Commit()
         
         commit.message = message.encode('utf-8')
         commit.tree = self.tree
 
         if committer is None:
@@ -168,16 +178,16 @@
         commit.commit_time = time_
         commit.commit_timezone = timezone
         commit.author_time = time_
         commit.author_timezone = timezone
 
         if ref in self.refs:
             parents = (self.refs[ref],)
-        elif self.ref in self.refs:
-            parents = (self.refs[self.ref],)
+        elif self._ref in self.refs:
+            parents = (self.refs[self._ref],)
         else:
             parents = ()
             
         commit.parents = parents
         
         if not commit.id in self.object_store:
             self.object_store.add_object(commit)
@@ -218,14 +228,14 @@
                         self[key] = entries
                 case ('!=', name, *difference):
                     self[name].patch((difference,))
 
     def merge(self, others, *, without_conflict=True):
         ancestor = last_common_ancestor(self.object_store,
                                         self.refs,
-                                        (vault.ref for vault in (self, *others)))
+                                        (vault._ref for vault in (self, *others)))
 
         base_vault = Vault(self.object_store, self.refs,
                            tree=self.object_store[self.object_store[ancestor].tree])
 
         for child in others:
             self.patch(child.diff(base_vault))
```

### Comparing `echovault-0.2.4/echovault/vault.py.bck` & `echovault-0.2.5/echovault/vault.py.bck`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/echovault/vault.py~` & `echovault-0.2.5/echovault/vault.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.4/PKG-INFO` & `echovault-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echovault
-Version: 0.2.4
+Version: 0.2.5
 Summary: echovault is git data storage
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


# Comparing `tmp/typedmongo-1.3.0.tar.gz` & `tmp/typedmongo-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.3.0.tar", last modified: Tue May  7 08:45:25 2024, max compression
+gzip compressed data, was "typedmongo-1.4.0.tar", last modified: Tue May  7 09:28:45 2024, max compression
```

## Comparing `typedmongo-1.3.0.tar` & `typedmongo-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-05-07 08:45:14.284598 typedmongo-1.3.0/LICENSE
--rw-r--r--   0        0        0     3808 2024-05-07 08:45:14.284598 typedmongo-1.3.0/README.md
--rw-r--r--   0        0        0     1441 2024-05-07 08:45:25.828545 typedmongo-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5575 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     4229 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/sync.py
--rw-r--r--   0        0        0     5335 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/test_client.py
--rw-r--r--   0        0        0     2930 2024-05-07 08:45:14.284598 typedmongo-1.3.0/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-05-07 08:45:14.288598 typedmongo-1.3.0/tests/test_marshamallow.py
--rw-r--r--   0        0        0     4221 2024-05-07 08:45:14.288598 typedmongo-1.3.0/tests/test_table.py
--rw-r--r--   0        0        0      811 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/__init__.py
--rw-r--r--   0        0        0      811 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    10328 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     9999 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     8494 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    10122 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5452 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/expressions.py
--rw-r--r--   0        0        0     9999 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/fields.py
--rw-r--r--   0        0        0      849 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/sync.py
--rw-r--r--   0        0        0     8494 2024-05-07 08:45:14.288598 typedmongo-1.3.0/typedmongo/table.py
--rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 typedmongo-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-07 09:28:32.689580 typedmongo-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3808 2024-05-07 09:28:32.689580 typedmongo-1.4.0/README.md
+-rw-r--r--   0        0        0     1441 2024-05-07 09:28:45.517577 typedmongo-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5575 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     4229 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/sync.py
+-rw-r--r--   0        0        0     5335 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/test_client.py
+-rw-r--r--   0        0        0     3031 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     4221 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/test_table.py
+-rw-r--r--   0        0        0      811 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/__init__.py
+-rw-r--r--   0        0        0      811 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    10328 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     9999 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     8494 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    10122 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5468 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/expressions.py
+-rw-r--r--   0        0        0     9999 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/fields.py
+-rw-r--r--   0        0        0      849 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/sync.py
+-rw-r--r--   0        0        0     8494 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/table.py
+-rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 typedmongo-1.4.0/PKG-INFO
```

### Comparing `typedmongo-1.3.0/LICENSE` & `typedmongo-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/README.md` & `typedmongo-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/pyproject.toml` & `typedmongo-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.3.0"
+version = "1.4.0"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.3.0/tests/asyncio/test_client.py` & `typedmongo-1.4.0/tests/asyncio/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/tests/asyncio/test_table.py` & `typedmongo-1.4.0/tests/asyncio/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/tests/sync.py` & `typedmongo-1.4.0/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/tests/test_client.py` & `typedmongo-1.4.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/tests/test_expressions.py` & `typedmongo-1.4.0/tests/test_expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,11 +88,15 @@
             ~~((field > 18) & (field < 35)),
             CombineExpression(
                 "AND",
                 CompareExpression(field, ">", 18),
                 CompareExpression(field, "<", 35),
             ),
         ),
+        (
+            None & (field > 18),
+            CompareExpression(field, ">", 18),
+        ),
     ],
 )
 def test_compile_expressions(expression, expected):
     assert expression == expected
```

### Comparing `typedmongo-1.3.0/tests/test_marshamallow.py` & `typedmongo-1.4.0/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/tests/test_table.py` & `typedmongo-1.4.0/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/__init__.py` & `typedmongo-1.4.0/typedmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/asyncio/__init__.py` & `typedmongo-1.4.0/typedmongo/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/asyncio/client.py` & `typedmongo-1.4.0/typedmongo/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/asyncio/fields.py` & `typedmongo-1.4.0/typedmongo/asyncio/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/asyncio/table.py` & `typedmongo-1.4.0/typedmongo/asyncio/table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/client.py` & `typedmongo-1.4.0/typedmongo/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/expressions.py` & `typedmongo-1.4.0/typedmongo/expressions.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,39 +38,41 @@
         """
         self & other
         """
         if not isinstance(other, Expression):
             return NotImplemented
         return CombineExpression("AND", self, other)
 
-    # Should we support it?
-    # def __rand__(self, other: Expression) -> CombineExpression:
-    #     """
-    #     other & self
-    #     """
-    #     if not isinstance(other, Expression):
-    #         return NotImplemented
-    #     return CombineExpression("AND", other, self)
+    def __rand__(self, other: Expression | None) -> Expression:
+        """
+        other & self
+        """
+        if other is None:
+            return self
+        if not isinstance(other, Expression):
+            return NotImplemented
+        return CombineExpression("AND", other, self)
 
     def __or__(self, other: Expression) -> CombineExpression:
         """
         self | other
         """
         if not isinstance(other, Expression):
             return NotImplemented
         return CombineExpression("OR", self, other)
 
-    # Should we support it?
-    # def __ror__(self, other: Expression) -> CombineExpression:
-    #     """
-    #     other | self
-    #     """
-    #     if not isinstance(other, Expression):
-    #         return NotImplemented
-    #     return CombineExpression("OR", other, self)
+    def __ror__(self, other: Expression | None) -> Expression:
+        """
+        other | self
+        """
+        if other is None:
+            return self
+        if not isinstance(other, Expression):
+            return NotImplemented
+        return CombineExpression("OR", other, self)
 
 
 class CompareMixin(HasFieldName):
     def __eq__(self, other: Any) -> CompareExpression:
         """
         self == other
         """
```

### Comparing `typedmongo-1.3.0/typedmongo/fields.py` & `typedmongo-1.4.0/typedmongo/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/marshamallow.py` & `typedmongo-1.4.0/typedmongo/marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/sync.py` & `typedmongo-1.4.0/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/typedmongo/table.py` & `typedmongo-1.4.0/typedmongo/table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.3.0/PKG-INFO` & `typedmongo-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedmongo
-Version: 1.3.0
+Version: 1.4.0
 Summary: A production-ready modern Python MongoDB ODM
 Author-Email: abersheeran <me@abersheeran.com>
 License: Apache2.0
 Requires-Python: >=3.10
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: motor>=3.4.0
 Requires-Dist: marshmallow>=3.21.1
```


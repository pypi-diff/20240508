# Comparing `tmp/edgegap_database-1.7.0.tar.gz` & `tmp/edgegap_database-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_database-1.7.0.tar", max compression
+gzip compressed data, was "edgegap_database-1.7.1.tar", max compression
```

## Comparing `edgegap_database-1.7.0.tar` & `edgegap_database-1.7.1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
--rw-r--r--   0        0        0     1993 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/LICENSE
--rw-r--r--   0        0        0     2180 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/README.md
--rw-r--r--   0        0        0       17 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/edgegap_database/BUILD
--rw-r--r--   0        0        0      445 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/edgegap_database/__init__.py
--rw-r--r--   0        0        0      754 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/edgegap_database/_base.py
--rw-r--r--   0        0        0      580 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/edgegap_database/_configuration.py
--rw-r--r--   0        0        0     1072 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/edgegap_database/_engine.py
--rw-r--r--   0        0        0      796 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/edgegap_database/_factory.py
--rw-r--r--   0        0        0      271 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/edgegap_database/_model.py
--rw-r--r--   0        0        0     2282 2024-05-07 13:27:48.723497 edgegap_database-1.7.0/edgegap_database/_operator.py
--rw-r--r--   0        0        0      509 2024-05-07 13:27:48.727497 edgegap_database-1.7.0/edgegap_database/_session.py
--rw-r--r--   0        0        0       17 2024-05-07 13:27:48.727497 edgegap_database-1.7.0/edgegap_database/errors/BUILD
--rw-r--r--   0        0        0      327 2024-05-07 13:27:48.727497 edgegap_database-1.7.0/edgegap_database/errors/__init__.py
--rw-r--r--   0        0        0      698 2024-05-07 13:27:48.727497 edgegap_database-1.7.0/edgegap_database/errors/_exceptions.py
--rw-r--r--   0        0        0      484 2024-05-07 13:27:48.727497 edgegap_database-1.7.0/edgegap_database/errors/_factory.py
--rw-r--r--   0        0        0      766 2024-05-07 13:29:10.252192 edgegap_database-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 edgegap_database-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-08 03:08:51.667389 edgegap_database-1.7.1/LICENSE
+-rw-r--r--   0        0        0     2180 2024-05-08 03:08:51.667602 edgegap_database-1.7.1/README.md
+-rw-r--r--   0        0        0      445 2024-05-08 03:08:51.668076 edgegap_database-1.7.1/edgegap_database/__init__.py
+-rw-r--r--   0        0        0      754 2024-05-08 03:08:51.668280 edgegap_database-1.7.1/edgegap_database/_base.py
+-rw-r--r--   0        0        0      580 2024-05-08 03:08:51.668450 edgegap_database-1.7.1/edgegap_database/_configuration.py
+-rw-r--r--   0        0        0     1072 2024-05-08 03:08:51.668630 edgegap_database-1.7.1/edgegap_database/_engine.py
+-rw-r--r--   0        0        0      796 2024-05-08 03:08:51.668821 edgegap_database-1.7.1/edgegap_database/_factory.py
+-rw-r--r--   0        0        0      271 2024-05-08 03:08:51.669000 edgegap_database-1.7.1/edgegap_database/_model.py
+-rw-r--r--   0        0        0     2252 2024-05-08 03:09:28.557443 edgegap_database-1.7.1/edgegap_database/_operator.py
+-rw-r--r--   0        0        0      509 2024-05-08 03:08:51.669671 edgegap_database-1.7.1/edgegap_database/_session.py
+-rw-r--r--   0        0        0      327 2024-05-08 03:08:51.669940 edgegap_database-1.7.1/edgegap_database/errors/__init__.py
+-rw-r--r--   0        0        0      698 2024-05-08 03:08:51.670181 edgegap_database-1.7.1/edgegap_database/errors/_exceptions.py
+-rw-r--r--   0        0        0      484 2024-05-08 03:08:51.670363 edgegap_database-1.7.1/edgegap_database/errors/_factory.py
+-rw-r--r--   0        0        0      766 2024-05-08 03:10:32.464708 edgegap_database-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2994 1970-01-01 00:00:00.000000 edgegap_database-1.7.1/PKG-INFO
```

### Comparing `edgegap_database-1.7.0/LICENSE` & `edgegap_database-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.0/README.md` & `edgegap_database-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.0/edgegap_database/_base.py` & `edgegap_database-1.7.1/edgegap_database/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.0/edgegap_database/_configuration.py` & `edgegap_database-1.7.1/edgegap_database/_configuration.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.0/edgegap_database/_engine.py` & `edgegap_database-1.7.1/edgegap_database/_engine.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.0/edgegap_database/_factory.py` & `edgegap_database-1.7.1/edgegap_database/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.0/edgegap_database/_operator.py` & `edgegap_database-1.7.1/edgegap_database/_operator.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,50 +32,50 @@
 
     def exec(self, statement: expression.Select | expression.SelectOfScalar) -> TupleResult | ScalarResult:
         result = self.__session.exec(statement)
         self.__session.commit()
 
         return result
 
-    def create(self, model: type[T]) -> T:
+    def create(self, model: T) -> T:
         with self.handle_exception():
             self.__session.add(model)
             self.__session.commit()
             self.__session.refresh(model)
 
             return model
 
-    def update(self, model: type[T]) -> T:
+    def update(self, model: T) -> T:
         with self.handle_exception():
             self.__session.add(model)
             self.__session.commit()
             self.__session.refresh(model)
 
             return model
 
-    def update_many(self, models: list[type[T]]) -> list[T]:
+    def update_many(self, models: list[T]) -> list[T]:
         with self.handle_exception():
             for model in models:
                 self.__session.add(model)
 
             self.__session.commit()
 
             for model in models:
                 self.__session.refresh(model)
 
             return models
 
-    def delete(self, model: type[T]) -> T:
+    def delete(self, model: T) -> T:
         with self.handle_exception():
             self.__session.delete(model)
             self.__session.commit()
 
             return model
 
-    def delete_many(self, models: list[type[T]]) -> list[T]:
+    def delete_many(self, models: list[T]) -> list[T]:
         with self.handle_exception():
             for model in models:
                 self.__session.delete(model)
 
             self.__session.commit()
 
             return models
```

### Comparing `edgegap_database-1.7.0/edgegap_database/errors/_exceptions.py` & `edgegap_database-1.7.1/edgegap_database/errors/_exceptions.py`

 * *Files identical despite different names*

### Comparing `edgegap_database-1.7.0/pyproject.toml` & `edgegap_database-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-database"
-version = "1.7.0"
+version = "1.7.1"
 description = "The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 psycopg-c = "^3.1.18"
```

### Comparing `edgegap_database-1.7.0/PKG-INFO` & `edgegap_database-1.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edgegap-database
-Version: 1.7.0
+Version: 1.7.1
 Summary: The Edgegap Database library includes various tools and helpers for interacting with Database and Migrations. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: psycopg-c (>=3.1.18,<4.0.0)
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: sqlmodel (>=0.0.18,<0.0.19)
 Description-Content-Type: text/markdown
```


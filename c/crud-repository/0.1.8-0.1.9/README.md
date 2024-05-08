# Comparing `tmp/crud_repository-0.1.8.tar.gz` & `tmp/crud_repository-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crud_repository-0.1.8.tar", last modified: Tue May  7 16:10:41 2024, max compression
+gzip compressed data, was "crud_repository-0.1.9.tar", last modified: Tue May  7 16:39:58 2024, max compression
```

## Comparing `crud_repository-0.1.8.tar` & `crud_repository-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 16:10:33.000000 crud_repository-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 16:10:33.000000 crud_repository-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-07 16:10:41.661715 crud_repository-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-07 16:10:33.000000 crud_repository-0.1.8/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    15987 2024-05-07 16:10:33.000000 crud_repository-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.657715 crud_repository-0.1.8/crud_repository/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/__config__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/crud_repository/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/db/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/db/idatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/crud_repository/db/mariadb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/db/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/db/mariadb/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/crud_repository/db/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/db/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/db/mysql/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/crud_repository/db/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/db/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/db/postgres/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/crud_repository/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/crud_repository/my_logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/my_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/my_logger/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/my_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/my_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/my_logger/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/crud_repository/repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/repo/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/crud_repository/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 16:10:33.000000 crud_repository-0.1.8/crud_repository/utils/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:10:41.661715 crud_repository-0.1.8/crud_repository.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-07 16:10:41.000000 crud_repository-0.1.8/crud_repository.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-07 16:10:41.000000 crud_repository-0.1.8/crud_repository.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:10:41.000000 crud_repository-0.1.8/crud_repository.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:10:41.000000 crud_repository-0.1.8/crud_repository.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 16:10:41.000000 crud_repository-0.1.8/crud_repository.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 16:10:41.000000 crud_repository-0.1.8/crud_repository.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 16:10:39.000000 crud_repository-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 16:10:41.665715 crud_repository-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 16:10:33.000000 crud_repository-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.510638 crud_repository-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 16:39:50.000000 crud_repository-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 16:39:50.000000 crud_repository-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-07 16:39:58.510638 crud_repository-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-07 16:39:50.000000 crud_repository-0.1.9/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16044 2024-05-07 16:39:50.000000 crud_repository-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.502638 crud_repository-0.1.9/crud_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/idatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/db/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/mariadb/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/db/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/mysql/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/db/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/postgres/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/my_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/repo/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/utils/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 16:39:56.000000 crud_repository-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 16:39:58.510638 crud_repository-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 16:39:50.000000 crud_repository-0.1.9/setup.py
```

### Comparing `crud_repository-0.1.8/LICENSE` & `crud_repository-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/PKG-INFO` & `crud_repository-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.8
+Version: 0.1.9
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
```

### Comparing `crud_repository-0.1.8/PYPI.md` & `crud_repository-0.1.9/PYPI.md`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/README.md` & `crud_repository-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -45,42 +45,44 @@
           +id: int
           +username: str
           +password: str
       }
     }
     namespace Databases { 
         class IDatabase {
+            << interface >>
           +connect(): Connection
           +get_session(): scoped_session
         }
         class PostgreSQLDatabase {
-            #session: scoped_session
+            +session: scoped_session
             #engine: Engine
             +connect(): Connection
             +get_session(): scoped_session
         }
         class MySQLDatabase {
-            #session: scoped_session
+            +session: scoped_session
             #engine: Engine
             +connect(): Connection
             +get_session(): scoped_session
         }
         class MariaDBDatabase {
-            #session: scoped_session
+            +session: scoped_session
             #engine: Engine
             +connect(): Connection
             +get_session(): scoped_session
         }
         class DatabaseFactory {
             +create(config: dict): IDatabase
         }
     }
 
     namespace Repositories { 
         class IRepository ~Base as T~ {
+            << interface >>
           +create(entity: T) : T
           +read(id) : T
           +update(entity: T): T
           +delete(entity: T): None
       }
         class Repository {
           #database: IDatabase
@@ -208,15 +210,15 @@
 * The `Repository` returns the newly formed `User Repository` object back to the `Client`.
 
 ---
 
 ### Perform CRUD Operation on User model
 
 ```mermaid
-sequenceDiagram
+sequenceDiagram 
     box Perform CRUD Operation
     participant Client
     participant UserRepository
     participant Repository
     participant User as User Model
     end
     Client->>UserRepository: performOperation(operation: string, user_repo: UserRepository)
```

### Comparing `crud_repository-0.1.8/crud_repository/__config__.py` & `crud_repository-0.1.9/crud_repository/__config__.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/db/factory.py` & `crud_repository-0.1.9/crud_repository/db/factory.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/db/idatabase.py` & `crud_repository-0.1.9/crud_repository/db/idatabase.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/db/mariadb/db.py` & `crud_repository-0.1.9/crud_repository/db/mariadb/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/db/mysql/db.py` & `crud_repository-0.1.9/crud_repository/db/mysql/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/db/postgres/db.py` & `crud_repository-0.1.9/crud_repository/db/postgres/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/my_logger/formatters.py` & `crud_repository-0.1.9/crud_repository/my_logger/formatters.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/my_logger/handlers.py` & `crud_repository-0.1.9/crud_repository/my_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/my_logger/logger.py` & `crud_repository-0.1.9/crud_repository/my_logger/logger.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/my_logger/monitor.py` & `crud_repository-0.1.9/crud_repository/my_logger/monitor.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository/repo/repository.py` & `crud_repository-0.1.9/crud_repository/repo/repository.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/crud_repository.egg-info/PKG-INFO` & `crud_repository-0.1.9/crud_repository.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.8
+Version: 0.1.9
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
```

### Comparing `crud_repository-0.1.8/crud_repository.egg-info/SOURCES.txt` & `crud_repository-0.1.9/crud_repository.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.8/pyproject.toml` & `crud_repository-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crud_repository"
-version = "0.1.8"
+version = "0.1.9"
 description = "The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases."
 authors = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"},
   {email = "info@hyfisolutions.com"},
 ]
 maintainers = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"}
```

### Comparing `crud_repository-0.1.8/setup.py` & `crud_repository-0.1.9/setup.py`

 * *Files identical despite different names*


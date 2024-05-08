# Comparing `tmp/crud_repository-0.1.9.tar.gz` & `tmp/crud_repository-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crud_repository-0.1.9.tar", last modified: Tue May  7 16:39:58 2024, max compression
+gzip compressed data, was "crud_repository-0.2.0.tar", last modified: Wed May  8 07:46:40 2024, max compression
```

## Comparing `crud_repository-0.1.9.tar` & `crud_repository-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.510638 crud_repository-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 16:39:50.000000 crud_repository-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 16:39:50.000000 crud_repository-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-07 16:39:58.510638 crud_repository-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-07 16:39:50.000000 crud_repository-0.1.9/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    16044 2024-05-07 16:39:50.000000 crud_repository-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.502638 crud_repository-0.1.9/crud_repository/
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/__config__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/idatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/db/mariadb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/mariadb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/mariadb/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/db/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/mysql/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/db/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/db/postgres/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/my_logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/my_logger/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/repo/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 16:39:50.000000 crud_repository-0.1.9/crud_repository/utils/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:39:58.506638 crud_repository-0.1.9/crud_repository.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 16:39:58.000000 crud_repository-0.1.9/crud_repository.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-07 16:39:56.000000 crud_repository-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-07 16:39:58.510638 crud_repository-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 16:39:50.000000 crud_repository-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.535001 crud_repository-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 07:46:33.000000 crud_repository-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-08 07:46:33.000000 crud_repository-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-08 07:46:40.535001 crud_repository-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-08 07:46:33.000000 crud_repository-0.2.0/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-05-08 07:46:33.000000 crud_repository-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.531001 crud_repository-0.2.0/crud_repository/
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/__config__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.531001 crud_repository-0.2.0/crud_repository/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/db/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/db/idatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.531001 crud_repository-0.2.0/crud_repository/db/mariadb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/db/mariadb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/db/mariadb/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.535001 crud_repository-0.2.0/crud_repository/db/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/db/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/db/mysql/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.535001 crud_repository-0.2.0/crud_repository/db/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/db/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/db/postgres/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.535001 crud_repository-0.2.0/crud_repository/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.535001 crud_repository-0.2.0/crud_repository/my_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/my_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/my_logger/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/my_logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/my_logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/my_logger/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.535001 crud_repository-0.2.0/crud_repository/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-08 07:46:33.000000 crud_repository-0.2.0/crud_repository/repo/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:46:40.535001 crud_repository-0.2.0/crud_repository.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-08 07:46:40.000000 crud_repository-0.2.0/crud_repository.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-08 07:46:40.000000 crud_repository-0.2.0/crud_repository.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:46:40.000000 crud_repository-0.2.0/crud_repository.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:46:40.000000 crud_repository-0.2.0/crud_repository.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-08 07:46:40.000000 crud_repository-0.2.0/crud_repository.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 07:46:40.000000 crud_repository-0.2.0/crud_repository.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 07:46:38.000000 crud_repository-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 07:46:40.535001 crud_repository-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 07:46:33.000000 crud_repository-0.2.0/setup.py
```

### Comparing `crud_repository-0.1.9/LICENSE` & `crud_repository-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/PKG-INFO` & `crud_repository-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.9
+Version: 0.2.0
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
```

### Comparing `crud_repository-0.1.9/PYPI.md` & `crud_repository-0.2.0/PYPI.md`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/README.md` & `crud_repository-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,55 +3,56 @@
 ---
 
 # CRUD Repository
 
 ---
 ## Description
 
-The CRUDRepository is a Python project designed to provide a 
-generic implementation of Create, Read, Update, and Delete (CRUD) 
-operations for various databases. It uses the Repository design pattern 
-to abstract the data access layer, allowing for easy switching between 
-different databases using the Factory pattern in which each database 
-object implements a Singleton object.  
-
-The project includes classes for handling different types of databases 
-such as PostgreSQL, MySQL, and MariaDB. Each of these classes implements 
-a common Interface, ensuring a consistent method of interaction 
-regardless of the underlying database.  
-
-The CRUDRepository also includes a Repository class that provides generic 
-CRUD operations. This class can be used as a base for creating more specific 
-repositories, like the test Repository UserRepository included in the project, which is 
-designed to manage User instances.  
-
-The project uses SQLAlchemy for ORM, providing a high-level, Pythonic 
-interface for database operations. It also includes a DatabaseFactory for 
-creating instances of the appropriate database class based on provided 
-configuration.  
-
-In summary, CRUDRepository is a flexible and extensible 
-foundation for Python applications that require database interactions, 
-abstracting the complexities of direct database access and providing a 
+The CRUDRepository is a Python project designed to provide a
+generic implementation of Create, Read, Update, and Delete (CRUD)
+operations for various databases. It uses the Repository design pattern
+to abstract the data access layer, allowing for easy switching between
+different databases using the Factory pattern in which each database
+object implements a Singleton object.
+
+The project includes classes for handling different types of databases
+such as PostgreSQL, MySQL, and MariaDB. Each of these classes implements
+a common Interface, ensuring a consistent method of interaction
+regardless of the underlying database.
+
+The CRUDRepository also includes a Repository class that provides generic
+CRUD operations. This class can be used as a base for creating more specific
+repositories, like the test Repository UserRepository included in the project, which is
+designed to manage User instances.
+
+The project uses SQLAlchemy for ORM, providing a high-level, Pythonic
+interface for database operations. It also includes a DatabaseFactory for
+creating instances of the appropriate database class based on provided
+configuration. The DatabaseFactory implements the Singleton design pattern, 
+ensuring that only one instance of each database type is created.
+
+In summary, CRUDRepository is a flexible and extensible
+foundation for Python applications that require database interactions,
+abstracting the complexities of direct database access and providing a
 clear and simple interface for performing CRUD operations.
 
 ## Class Diagram
 
 ```mermaid
 classDiagram
-    namespace Models { 
+    namespace Models {
         class Base {
         }
       class User {
           +id: int
           +username: str
           +password: str
       }
     }
-    namespace Databases { 
+    namespace Databases {
         class IDatabase {
             << interface >>
           +connect(): Connection
           +get_session(): scoped_session
         }
         class PostgreSQLDatabase {
             +session: scoped_session
@@ -68,19 +69,20 @@
         class MariaDBDatabase {
             +session: scoped_session
             #engine: Engine
             +connect(): Connection
             +get_session(): scoped_session
         }
         class DatabaseFactory {
-            +create(config: dict): IDatabase
+            _instances: Dict$
+            +create(config: dict) : IDatabase$
         }
     }
 
-    namespace Repositories { 
+    namespace Repositories {
         class IRepository ~Base as T~ {
             << interface >>
           +create(entity: T) : T
           +read(id) : T
           +update(entity: T): T
           +delete(entity: T): None
       }
@@ -94,20 +96,20 @@
       }
         class UserRepository {
             +__init__(database: IDatabase)
         }
     }
 
 
-    
+
     IDatabase <|-- PostgreSQLDatabase: Implements
     IDatabase <|-- MySQLDatabase: Implements
     IDatabase <|-- MariaDBDatabase: Implements
 
-    
+
     IRepository ~Base as T~ <|-- Repository : Implements
     Repository <|-- UserRepository: Implements
     PostgreSQLDatabase "1" -- "1" Repository: Uses
     MySQLDatabase "1" -- "1" Repository: Uses
     MariaDBDatabase "1" -- "1" Repository: Uses
     UserRepository "1" -- "1" User: Manages
     Base <|-- User: Implements
@@ -116,15 +118,15 @@
     DatabaseFactory --> MariaDBDatabase: << create >>
 ```
 
 ### In this diagram (Class Diagram):
 
 * `Base` is a base class for all models, and `User` is a specific model that extends `Base`.
 * `IDatabase` is an abstract base class that defines the interface for a database. `PostgreSQLDatabase`, `MySQLDatabase`, and `MariaDBDatabase` are concrete implementations of this interface.
-* `DatabaseFactory` is a factory class that creates instances of `PostgreSQLDatabase`, `MySQLDatabase`, or `MariaDBDatabase` based on the provided configuration.
+* `DatabaseFactory` is a factory class that creates instances of `PostgreSQLDatabase`, `MySQLDatabase`, or `MariaDBDatabase` based on the provided configuration. It ensures that only one instance of each database type is created, implementing the Singleton design pattern.
 * `IRepository ~T~` is an abstract base class that defines the interface for a repository, and `Repository ~Base~` is a generic implementation of this interface that is bound to the `Base` model class.
 * `UserRepository` is a specific repository that manages `User` instances.
 * `PostgreSQLDatabase`, `MySQLDatabase`, and `MariaDBDatabase` are used by `Repository ~Base~`, and `UserRepository` manages `User` instances.
 
 ---
 
 ## Sequence Diagrams
```

### Comparing `crud_repository-0.1.9/crud_repository/__config__.py` & `crud_repository-0.2.0/crud_repository/__config__.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository/db/factory.py` & `crud_repository-0.2.0/crud_repository/db/factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,78 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 This module provides classes for managing databases.
 """
+from typing import Dict
+
 from crud_repository.db.idatabase import IDatabase
 from crud_repository.db.mariadb.db import MariaDBDatabase
 from crud_repository.db.mysql.db import MySQLDatabase
 from crud_repository.db.postgres.db import PostgreSQLDatabase
 from crud_repository.my_logger.logger import CustomLogger
 
 log = CustomLogger(__name__).get_logger("DEBUG")
 
 
 # ---------------------------------------------------------
 class DatabaseFactory:
     """
     This class provides a factory for creating database instances.
     """
+    _instances: Dict = {}
+
     @staticmethod
     def create(config: dict) -> IDatabase:
         """
         Create a database instance based on the provided configuration.
 
         :param config: The configuration for the database.
         :return: (IDatabase) The created database instance.
         """
         try:
+            # Check if an instance of this type already exists
+            if config["type"] in DatabaseFactory._instances:
+                return DatabaseFactory._instances[config["type"]]
+
             # Create the appropriate database instance based on the configuration
             # (e.g., PostgreSQL, MySQL, MariaDB, etc.)
-            if config["type"] == "postgresql":
-                return PostgreSQLDatabase(
+            if config["type"].lower() == "postgresql":
+                instance = PostgreSQLDatabase(
                     **{
                         "db_name": config["db_name"],
                         "user": config["user"],
                         "password": config["password"],
                         "host": config["host"],
                         "port": config["port"],
                     }
                 )
-            if config["type"] == "mysql":
-                return MySQLDatabase(
+            elif config["type"].lower() == "mysql":
+                instance = MySQLDatabase(
                     **{
                         "db_name": config["db_name"],
                         "user": config["user"],
                         "password": config["password"],
                         "host": config["host"],
                         "port": config["port"],
                     }
                 )
-            if config["type"] == "mariadb":
-                return MariaDBDatabase(
+            elif config["type"].lower() == "mariadb":
+                instance = MariaDBDatabase(
                     **{
                         "db_name": config["db_name"],
                         "user": config["user"],
                         "password": config["password"],
                         "host": config["host"],
                         "port": config["port"],
                     }
                 )
-            # ... other database types
-            raise ValueError("Invalid database type")
+            else:
+                raise ValueError("Invalid database type")
+
+            # Store the new instance in the dictionary
+            DatabaseFactory._instances[config["type"]] = instance
+
+            return instance
         except Exception as e:
             log.debug(f"Error creating database instance: {e}")
-            raise e
+            raise e
```

### Comparing `crud_repository-0.1.9/crud_repository/db/idatabase.py` & `crud_repository-0.2.0/crud_repository/db/idatabase.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository/db/mariadb/db.py` & `crud_repository-0.2.0/crud_repository/db/mariadb/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository/db/mysql/db.py` & `crud_repository-0.2.0/crud_repository/db/mysql/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository/db/postgres/db.py` & `crud_repository-0.2.0/crud_repository/db/postgres/db.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository/my_logger/formatters.py` & `crud_repository-0.2.0/crud_repository/my_logger/formatters.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository/my_logger/handlers.py` & `crud_repository-0.2.0/crud_repository/my_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository/my_logger/logger.py` & `crud_repository-0.2.0/crud_repository/my_logger/logger.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository/my_logger/monitor.py` & `crud_repository-0.2.0/crud_repository/my_logger/monitor.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository/repo/repository.py` & `crud_repository-0.2.0/crud_repository/repo/repository.py`

 * *Files identical despite different names*

### Comparing `crud_repository-0.1.9/crud_repository.egg-info/PKG-INFO` & `crud_repository-0.2.0/crud_repository.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crud_repository
-Version: 0.1.9
+Version: 0.2.0
 Summary: The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases.
 Home-page: https://github.com/dellius-alexander/CRUDRepository.git
 Author: Dellius Alexander
 Author-email: Dellius Alexander <dalexander@hyfisolutions.com>, info@hyfisolutions.com
 Maintainer-email: Dellius Alexander <dalexander@hyfisolutions.com>
 License: MIT License
```

### Comparing `crud_repository-0.1.9/crud_repository.egg-info/SOURCES.txt` & `crud_repository-0.2.0/crud_repository.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,10 +26,8 @@
 crud_repository/model/base.py
 crud_repository/my_logger/__init__.py
 crud_repository/my_logger/formatters.py
 crud_repository/my_logger/handlers.py
 crud_repository/my_logger/logger.py
 crud_repository/my_logger/monitor.py
 crud_repository/repo/__init__.py
-crud_repository/repo/repository.py
-crud_repository/utils/__init__.py
-crud_repository/utils/crypto.py
+crud_repository/repo/repository.py
```

### Comparing `crud_repository-0.1.9/pyproject.toml` & `crud_repository-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crud_repository"
-version = "0.1.9"
+version = "0.2.0"
 description = "The CRUDRepository is a Python project designed to provide a generic implementation of Create, Read, Update, and Delete (CRUD) operations for various databases."
 authors = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"},
   {email = "info@hyfisolutions.com"},
 ]
 maintainers = [
   {name = "Dellius Alexander", email = "dalexander@hyfisolutions.com"}
```

### Comparing `crud_repository-0.1.9/setup.py` & `crud_repository-0.2.0/setup.py`

 * *Files identical despite different names*


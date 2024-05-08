# Comparing `tmp/mongodb_orm-0.0.129a5.tar.gz` & `tmp/mongodb_orm-0.0.130.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_orm-0.0.129a5.tar", last modified: Wed May  8 14:08:42 2024, max compression
+gzip compressed data, was "mongodb_orm-0.0.130.tar", last modified: Fri May  3 12:50:20 2024, max compression
```

## Comparing `mongodb_orm-0.0.129a5.tar` & `mongodb_orm-0.0.130.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:42.756541 mongodb_orm-0.0.129a5/
--rw-rw-rw-   0        0        0      348 2024-05-08 14:08:42.753523 mongodb_orm-0.0.129a5/PKG-INFO
--rw-rw-rw-   0        0        0      593 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:41.251724 mongodb_orm-0.0.129a5/mongodb_orm/
--rw-rw-rw-   0        0        0       95 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/__init__.py
--rw-rw-rw-   0        0        0      489 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:41.383703 mongodb_orm-0.0.129a5/mongodb_orm/custom_urls/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/custom_urls/__init__.py
--rw-rw-rw-   0        0        0     1543 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a5/mongodb_orm/custom_urls/bread_urls.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:41.494711 mongodb_orm-0.0.129a5/mongodb_orm/decorators/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/decorators/__init__.py
--rw-rw-rw-   0        0        0      483 2024-05-01 09:35:34.000000 mongodb_orm-0.0.129a5/mongodb_orm/decorators/chained.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:41.603703 mongodb_orm-0.0.129a5/mongodb_orm/exceptions/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/exceptions/__init__.py
--rw-rw-rw-   0        0        0      142 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/exceptions/syntax_exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:41.868703 mongodb_orm-0.0.129a5/mongodb_orm/interfaces/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/interfaces/__init__.py
--rw-rw-rw-   0        0        0     2671 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/interfaces/base_mongodb_model.py
--rw-rw-rw-   0        0        0     7835 2024-05-01 14:26:45.000000 mongodb_orm-0.0.129a5/mongodb_orm/interfaces/mongodb_model.py
--rw-rw-rw-   0        0        0      826 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/interfaces/mongodb_model_events.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:41.931704 mongodb_orm-0.0.129a5/mongodb_orm/management/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:42.020703 mongodb_orm-0.0.129a5/mongodb_orm/management/commands/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/management/commands/__init__.py
--rw-rw-rw-   0        0        0     4650 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/management/commands/update_schema.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:42.091713 mongodb_orm-0.0.129a5/mongodb_orm/models/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:42.203703 mongodb_orm-0.0.129a5/mongodb_orm/singletons/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/singletons/__init__.py
--rw-rw-rw-   0        0        0      392 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/singletons/mongodb_singleton_client.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:42.519523 mongodb_orm-0.0.129a5/mongodb_orm/types/
--rw-rw-rw-   0        0        0      530 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/types/Relation.py
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/types/__init__.py
--rw-rw-rw-   0        0        0      136 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/types/index.py
--rw-rw-rw-   0        0        0      440 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a5/mongodb_orm/types/logger_object.py
--rw-rw-rw-   0        0        0      797 2024-05-01 12:31:08.000000 mongodb_orm-0.0.129a5/mongodb_orm/types/model_schema.py
--rw-rw-rw-   0        0        0      382 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/types/options.py
--rw-rw-rw-   0        0        0      196 2024-05-01 09:42:29.000000 mongodb_orm-0.0.129a5/mongodb_orm/urls.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:42.584525 mongodb_orm-0.0.129a5/mongodb_orm/utils/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/utils/__init__.py
--rw-rw-rw-   0        0        0     1752 2024-05-08 14:07:56.000000 mongodb_orm-0.0.129a5/mongodb_orm/utils/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:42.689534 mongodb_orm-0.0.129a5/mongodb_orm/views/
--rw-rw-rw-   0        0        0        0 2024-05-01 09:27:04.000000 mongodb_orm-0.0.129a5/mongodb_orm/views/__init__.py
--rw-rw-rw-   0        0        0     4088 2024-05-08 14:06:36.000000 mongodb_orm-0.0.129a5/mongodb_orm/views/mongodb_api_model_view.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:08:41.337708 mongodb_orm-0.0.129a5/mongodb_orm.egg-info/
--rw-rw-rw-   0        0        0      348 2024-05-08 14:08:40.000000 mongodb_orm-0.0.129a5/mongodb_orm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1208 2024-05-08 14:08:41.000000 mongodb_orm-0.0.129a5/mongodb_orm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 14:08:40.000000 mongodb_orm-0.0.129a5/mongodb_orm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-08 14:08:40.000000 mongodb_orm-0.0.129a5/mongodb_orm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-08 14:08:40.000000 mongodb_orm-0.0.129a5/mongodb_orm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 14:08:42.756541 mongodb_orm-0.0.129a5/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-05-08 14:08:12.000000 mongodb_orm-0.0.129a5/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.011392 mongodb_orm-0.0.130/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-05-03 12:50:20.010628 mongodb_orm-0.0.130/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      565 2024-04-23 13:57:27.000000 mongodb_orm-0.0.130/README.md
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.987397 mongodb_orm-0.0.130/mongodb_orm/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       91 2024-04-23 14:47:25.000000 mongodb_orm-0.0.130/mongodb_orm/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      475 2024-04-23 14:25:35.000000 mongodb_orm-0.0.130/mongodb_orm/apps.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.991405 mongodb_orm-0.0.130/mongodb_orm/custom_urls/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-18 11:23:58.000000 mongodb_orm-0.0.130/mongodb_orm/custom_urls/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1507 2024-05-03 12:46:06.000000 mongodb_orm-0.0.130/mongodb_orm/custom_urls/bread_urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.992785 mongodb_orm-0.0.130/mongodb_orm/decorators/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/decorators/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      433 2024-04-04 10:34:42.000000 mongodb_orm-0.0.130/mongodb_orm/decorators/chained.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.994312 mongodb_orm-0.0.130/mongodb_orm/exceptions/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/exceptions/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      138 2024-04-04 10:34:42.000000 mongodb_orm-0.0.130/mongodb_orm/exceptions/syntax_exceptions.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.998052 mongodb_orm-0.0.130/mongodb_orm/interfaces/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:42.000000 mongodb_orm-0.0.130/mongodb_orm/interfaces/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2619 2024-04-29 14:42:33.000000 mongodb_orm-0.0.130/mongodb_orm/interfaces/base_mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     7653 2024-05-03 12:47:26.000000 mongodb_orm-0.0.130/mongodb_orm/interfaces/mongodb_model.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      801 2024-04-29 09:28:59.000000 mongodb_orm-0.0.130/mongodb_orm/interfaces/mongodb_model_events.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:19.999053 mongodb_orm-0.0.130/mongodb_orm/management/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.130/mongodb_orm/management/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.000015 mongodb_orm-0.0.130/mongodb_orm/management/commands/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/management/commands/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4559 2024-04-23 15:18:03.000000 mongodb_orm-0.0.130/mongodb_orm/management/commands/update_schema.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.000897 mongodb_orm-0.0.130/mongodb_orm/models/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-04 10:34:43.000000 mongodb_orm-0.0.130/mongodb_orm/models/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.001907 mongodb_orm-0.0.130/mongodb_orm/singletons/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/singletons/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-04-04 10:34:44.000000 mongodb_orm-0.0.130/mongodb_orm/singletons/mongodb_singleton_client.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.006272 mongodb_orm-0.0.130/mongodb_orm/types/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      508 2024-04-04 10:34:44.000000 mongodb_orm-0.0.130/mongodb_orm/types/Relation.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/types/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      128 2024-04-04 10:34:44.000000 mongodb_orm-0.0.130/mongodb_orm/types/index.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      406 2024-04-04 10:34:44.000000 mongodb_orm-0.0.130/mongodb_orm/types/logger_object.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      766 2024-05-03 12:47:26.000000 mongodb_orm-0.0.130/mongodb_orm/types/model_schema.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      368 2024-04-23 15:18:03.000000 mongodb_orm-0.0.130/mongodb_orm/types/options.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      189 2024-05-03 12:47:26.000000 mongodb_orm-0.0.130/mongodb_orm/urls.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.007400 mongodb_orm-0.0.130/mongodb_orm/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 15:11:55.000000 mongodb_orm-0.0.130/mongodb_orm/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1163 2024-04-26 10:44:00.000000 mongodb_orm-0.0.130/mongodb_orm/utils/helpers.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.008773 mongodb_orm-0.0.130/mongodb_orm/views/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        0 2024-04-23 14:15:07.000000 mongodb_orm-0.0.130/mongodb_orm/views/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3901 2024-04-23 14:28:47.000000 mongodb_orm-0.0.130/mongodb_orm/views/mongodb_api_model_view.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-05-03 12:50:20.009786 mongodb_orm-0.0.130/mongodb_orm.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      333 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1208 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       35 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       12 2024-05-03 12:50:19.000000 mongodb_orm-0.0.130/mongodb_orm.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-05-03 12:50:20.011546 mongodb_orm-0.0.130/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      594 2024-05-03 12:50:10.000000 mongodb_orm-0.0.130/setup.py
```

### Comparing `mongodb_orm-0.0.129a5/mongodb_orm/custom_urls/bread_urls.py` & `mongodb_orm-0.0.130/mongodb_orm/custom_urls/bread_urls.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import os
-import sys
-import importlib.util
-from django.conf import settings
-from rest_framework import routers
-from django.urls import path, include
-from mongodb_orm.interfaces.mongodb_model import MongoDBModel
-from mongodb_orm.views.mongodb_api_model_view import MongoDBAPIModelView
-
-current_directory = os.path.dirname(os.path.abspath(__file__))
-BASE_DIR = settings.BASE_DIR
-if hasattr(settings, 'MONGODB_ORM_MODELS_FOLDER'):
-    MONGODB_MODELS_PATH = settings.MONGODB_ORM_MODELS_FOLDER
-else:
-    MONGODB_MODELS_PATH = "app/models"
-
-models_directory = os.path.join(current_directory, BASE_DIR, MONGODB_MODELS_PATH)
-sys.path.insert(0, os.path.abspath(os.path.join(current_directory, "..")))
-
-router = routers.SimpleRouter()
-
-for filename in os.listdir(str(models_directory)):
-    if filename.endswith(".py") and filename != "__init__.py":
-        module_name = os.path.splitext(filename)[0]
-        try:
-            module = importlib.import_module(f"{MONGODB_MODELS_PATH.replace('/', '.')}.{module_name}")
-            for name, obj in vars(module).items():
-                if (isinstance(obj, type) and issubclass(obj, MongoDBAPIModelView)
-                        and issubclass(obj, MongoDBModel) and obj != MongoDBAPIModelView and obj != MongoDBModel):
-                    router.register(rf"{obj.collection_name}", obj, basename=f"{obj.collection_name}")
-        except Exception as e:
-            print(f"Error loading module {module_name}: {e}")
-
-BREAD_URLS = [
-    path('', include(router.urls)),
-]
+import os
+import sys
+import importlib.util
+from django.conf import settings
+from rest_framework import routers
+from django.urls import path, include
+from mongodb_orm.interfaces.mongodb_model import MongoDBModel
+from mongodb_orm.views.mongodb_api_model_view import MongoDBAPIModelView
+
+current_directory = os.path.dirname(os.path.abspath(__file__))
+BASE_DIR = settings.BASE_DIR
+if hasattr(settings, 'MONGODB_ORM_MODELS_FOLDER'):
+    MONGODB_MODELS_PATH = settings.MONGODB_ORM_MODELS_FOLDER
+else:
+    MONGODB_MODELS_PATH = "app/models"
+
+models_directory = os.path.join(current_directory, BASE_DIR, MONGODB_MODELS_PATH)
+sys.path.insert(0, os.path.abspath(os.path.join(current_directory, "..")))
+
+router = routers.SimpleRouter()
+
+for filename in os.listdir(str(models_directory)):
+    if filename.endswith(".py") and filename != "__init__.py":
+        module_name = os.path.splitext(filename)[0]
+        try:
+            module = importlib.import_module(f"{MONGODB_MODELS_PATH.replace('/', '.')}.{module_name}")
+            for name, obj in vars(module).items():
+                if (isinstance(obj, type) and issubclass(obj, MongoDBAPIModelView)
+                        and issubclass(obj, MongoDBModel) and obj != MongoDBAPIModelView and obj != MongoDBModel):
+                    router.register(rf"{obj.collection_name}", obj, basename=f"{obj.collection_name}")
+        except Exception as e:
+            print(f"Error loading module {module_name}: {e}")
+
+BREAD_URLS = [
+    path('', include(router.urls)),
+]
```

### Comparing `mongodb_orm-0.0.129a5/mongodb_orm/interfaces/base_mongodb_model.py` & `mongodb_orm-0.0.130/mongodb_orm/interfaces/base_mongodb_model.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from typing import List
-from pymongo.database import Database
-from pymongo.collection import Collection
-from mongodb_orm.types.index import Index
-from mongodb_orm.types.options import Options
-from mongodb_orm.types.Relation import Relation
-from mongodb_orm.singletons.mongodb_singleton_client import MongoDBClient
-
-
-class BaseMongoDBModel:
-    """
-        Preventing direct Instantiation of this class
-    """
-
-    def __new__(cls, *args, **kwargs):
-        if cls is BaseMongoDBModel:
-            raise TypeError(f"only children of '{cls.__name__}' may be instantiated")
-        return object.__new__(cls)
-
-    def connect(self, tenant: str, collection: str, options: Options = None, indexes: List[Index] = None,
-                relations: List[Relation] = None) -> Collection:
-        client = MongoDBClient().get_database(f'{tenant}')
-        if collection not in client.list_collection_names():
-            self._create_collection(client, collection, options, indexes, relations)
-        return client.get_collection(collection)
-
-    """
-        Creating the collection if not exists and if there are indexes they will be created
-    """
-
-    @staticmethod
-    def _create_collection(client: Database, collection: str, options: Options = None,
-                           indexes: List[Index] = None, relations: List[Relation] = None) -> None:
-        schema: dict = {}
-        if options is not None:
-            schema = {'$jsonSchema': options['schema']}
-        collection_instance = client.create_collection(collection,
-                                                       timeseries={'timeField': 'created_at',
-                                                                   'metaField': 'consumed'} if options and options.get(
-                                                           'time_series') else None,
-                                                       validator=schema if options and not options.get(
-                                                           'time_series') else None,
-                                                       expireAfterSeconds=30 if options and options.get(
-                                                           'time_series') else None)
-        if indexes:
-            for index in indexes:
-                collection_instance.create_index([
-                    (index['name'], 1 if index['asc'] else -1)
-                ],
-                    unique=index['unique'] if options and not options.get('time_series') else None,
-                    expireAfterSeconds=index['expireAfterSeconds'] if index['expireAfterSeconds'] else None
-                )
+from typing import List
+from pymongo.database import Database
+from pymongo.collection import Collection
+from mongodb_orm.types.index import Index
+from mongodb_orm.types.options import Options
+from mongodb_orm.types.Relation import Relation
+from mongodb_orm.singletons.mongodb_singleton_client import MongoDBClient
+
+
+class BaseMongoDBModel:
+    """
+        Preventing direct Instantiation of this class
+    """
+
+    def __new__(cls, *args, **kwargs):
+        if cls is BaseMongoDBModel:
+            raise TypeError(f"only children of '{cls.__name__}' may be instantiated")
+        return object.__new__(cls)
+
+    def connect(self, tenant: str, collection: str, options: Options = None, indexes: List[Index] = None,
+                relations: List[Relation] = None) -> Collection:
+        client = MongoDBClient().get_database(f'{tenant}')
+        if collection not in client.list_collection_names():
+            self._create_collection(client, collection, options, indexes, relations)
+        return client.get_collection(collection)
+
+    """
+        Creating the collection if not exists and if there are indexes they will be created
+    """
+
+    @staticmethod
+    def _create_collection(client: Database, collection: str, options: Options = None,
+                           indexes: List[Index] = None, relations: List[Relation] = None) -> None:
+        schema: dict = {}
+        if options is not None:
+            schema = {'$jsonSchema': options['schema']}
+        collection_instance = client.create_collection(collection,
+                                                       timeseries={'timeField': 'created_at',
+                                                                   'metaField': 'consumed'} if options and options.get(
+                                                           'time_series') else None,
+                                                       validator=schema if options and not options.get(
+                                                           'time_series') else None,
+                                                       expireAfterSeconds=30 if options and options.get(
+                                                           'time_series') else None)
+        if indexes:
+            for index in indexes:
+                collection_instance.create_index([
+                    (index['name'], 1 if index['asc'] else -1)
+                ],
+                    unique=index['unique'] if options and not options.get('time_series') else None,
+                    expireAfterSeconds=index['expireAfterSeconds'] if index['expireAfterSeconds'] else None
+                )
```

### Comparing `mongodb_orm-0.0.129a5/mongodb_orm/interfaces/mongodb_model.py` & `mongodb_orm-0.0.130/mongodb_orm/interfaces/mongodb_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-import math
-import pymongo
-from bson import ObjectId
-from datetime import datetime
-from typing import List, Union, Sequence
-from pymongo.cursor import Cursor
-from pymongo.collection import Collection
-from pymongo.results import InsertOneResult
-
-from mongodb_orm.interfaces.mongodb_model_events import MongoDBModelEvents
-from mongodb_orm.types.index import Index
-from mongodb_orm.utils.helpers import Helper
-from mongodb_orm.types.options import Options
-from mongodb_orm.types.Relation import Relation
-from mongodb_orm.decorators.chained import chained
-from mongodb_orm.exceptions.syntax_exceptions import ChainingError
-from mongodb_orm.interfaces.base_mongodb_model import BaseMongoDBModel
-
-
-class MongoDBModel(BaseMongoDBModel, MongoDBModelEvents):
-    """
-        Public class variables to be overridden by the model
-    """
-    collection_name: str = ''
-    # Check the following link to check what are the possible valid options for collection creation
-    # https://www.mongodb.com/docs/manual/reference/method/db.createCollection/
-    options: Options = None
-    timestamp: bool = True
-    # List[index] of the indexes for a
-    indexes: List[Index] = None
-    # List of the attributes allowed to be returned per query
-    attributes: List[str] = ['*']
-    # List of the attributes guarded against returned per query
-    guarded: List[str] = []
-    # List of the relationship to a model
-    relations: List[Relation] = None
-
-    """
-        Preventing direct Instantiation of this class 
-    """
-
-    def __new__(cls, *args, **kwargs):
-        if cls is MongoDBModel:
-            raise TypeError(f"only children of '{cls.__name__}' may be instantiated")
-        return object.__new__(cls)
-
-    """
-        The logic behind all the crud of a model
-    """
-
-    _collection: Collection = None
-
-    def set_tenant(self, tenant_name: str):
-        self.__init__(tenant=tenant_name)
-
-    def __init__(self, tenant: str = 'public', **kwargs):
-        self._collection = self.connect(tenant, self.collection_name, self.options, self.indexes, self.relations)
-        self._projection = {k: 1 for k in self.attributes if k != '*' and k not in self.guarded}
-        self._result: Cursor | InsertOneResult | dict | None = None
-        self.chained = True
-
-    def query(self) -> 'MongoDBModel':
-        self.chained = False
-        return self
-
-    def json(self) -> Union[List[dict], dict]:
-        if self._result is None:
-            raise ChainingError(message='you can not call json directly, it needs to be chained')
-        if isinstance(self._result, Cursor):
-            return [Helper.standardize_dict(item, underscore=True) for item in list(self._result)]
-        else:
-            return Helper.standardize_dict(self._result, underscore=True)
-
-    @chained
-    def get(self, pk: str) -> Union[dict, 'MongoDBModel']:
-        return self._collection.find_one({'_id': ObjectId(pk)}, projection=self._projection)
-
-    @chained
-    def get_all(self,
-                filters: dict = None,
-                page: int = 1,
-                per_page: int = 10,
-                sort_by: tuple = None) -> Union[dict, 'MongoDBModel']:
-        sort_criteria: Sequence = [('_id', pymongo.ASCENDING)]
-
-        if sort_by is not None:
-            sort_criteria: Sequence = [sort_by]
-        cursor: Cursor = self._collection.find(
-            filters, projection=self._projection
-        ).sort(sort_criteria).skip(
-            (page * per_page) - per_page
-        ).limit(per_page)
-        # Convert cursor to list of dictionaries
-        data = [Helper.standardize_dict(item, underscore=True) for item in list(cursor)]
-        # Get total documents count
-        total_documents = self.count()
-        # Calculate total pages
-        total_pages = math.ceil(total_documents / per_page)
-
-        query_result: dict = {
-            'data': data,
-            'filters': filters,
-            'page': page,
-            'per_page': per_page,
-            'total_pages': total_pages,
-            'sort_by': [{sort_tuple[0]: sort_tuple[1]} for sort_tuple in sort_criteria],
-            'matches': len(data),
-            'total_documents': self.count()
-        }
-        return query_result
-
-    @chained
-    def find_one(self, filters: dict, sort_criteria: List[tuple] = None) -> Union[dict, 'MongoDBModel']:
-        return self._collection.find_one(filters, sort=sort_criteria, projection=self._projection)
-
-    @chained
-    def put(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
-        query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
-                                                     {'$set': {**record, **({
-                                                                                'updated_at': datetime.utcnow()
-                                                                            } if self.timestamp else {})}},
-                                                     projection=self._projection)
-        self.on_partial_update(self.get(pk).json(), record)
-        return query
-
-    @chained
-    def patch(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
-        query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
-                                                     {'$push': record,
-                                                      '$set':
-                                                          {**({
-                                                                  'updated_at': datetime.utcnow()
-                                                              } if self.timestamp else {})}
-                                                      },
-                                                     projection=self._projection)
-        self.on_partial_update(record, self.get(pk).json())
-        return query
-
-    @chained
-    def put_patch(self, pk: str, put_record: dict, patch_record: dict) -> Union[dict, 'MongoDBModel']:
-        return self._collection.find_one_and_update({'_id': ObjectId(pk)},
-                                                    {'$set': {**put_record, **({
-                                                                                   'updated_at': datetime.utcnow()
-                                                                               } if self.timestamp else {})},
-                                                     '$push': patch_record},
-                                                    projection=self._projection)
-
-    def post(self, record: dict) -> Union[InsertOneResult, 'MongoDBModel']:
-        self.on_save(record)
-        return self._collection.insert_one({**record, **({
-                                                             'created_at': datetime.utcnow(),
-                                                             'updated_at': datetime.utcnow()
-                                                         } if self.timestamp else {})})
-
-    # def mass_patch(self):
-    #     return self._collection.update_many(
-    #         {},
-    #         [
-    #             {
-    #                 '$set': {
-    #                     'created_at': {'$toDate': '$created_at'},
-    #                     'updated_at': datetime.utcnow()
-    #                 }
-    #             }
-    #         ]
-    #     )
-
-    def delete(self, pk: str) -> bool:
-        self.on_delete(self.get(pk).json())
-        return bool(self._collection.find_one_and_delete({'_id': ObjectId(pk)}, projection=self._projection))
-
-    def count(self, filters: dict = None) -> int:
-        return self._collection.count_documents(filters if filters else {})
-
-    def distinct_values(self, key: str) -> list:
-        return self._collection.distinct(key)
+import math
+import pymongo
+from bson import ObjectId
+from datetime import datetime
+from typing import List, Union, Sequence
+from pymongo.cursor import Cursor
+from pymongo.collection import Collection
+from pymongo.results import InsertOneResult
+
+from mongodb_orm.interfaces.mongodb_model_events import MongoDBModelEvents
+from mongodb_orm.types.index import Index
+from mongodb_orm.utils.helpers import Helper
+from mongodb_orm.types.options import Options
+from mongodb_orm.types.Relation import Relation
+from mongodb_orm.decorators.chained import chained
+from mongodb_orm.exceptions.syntax_exceptions import ChainingError
+from mongodb_orm.interfaces.base_mongodb_model import BaseMongoDBModel
+
+
+class MongoDBModel(BaseMongoDBModel, MongoDBModelEvents):
+    """
+        Public class variables to be overridden by the model
+    """
+    collection_name: str = ''
+    # Check the following link to check what are the possible valid options for collection creation
+    # https://www.mongodb.com/docs/manual/reference/method/db.createCollection/
+    options: Options = None
+    timestamp: bool = True
+    # List[index] of the indexes for a
+    indexes: List[Index] = None
+    # List of the attributes allowed to be returned per query
+    attributes: List[str] = ['*']
+    # List of the attributes guarded against returned per query
+    guarded: List[str] = []
+    # List of the relationship to a model
+    relations: List[Relation] = None
+
+    """
+        Preventing direct Instantiation of this class 
+    """
+
+    def __new__(cls, *args, **kwargs):
+        if cls is MongoDBModel:
+            raise TypeError(f"only children of '{cls.__name__}' may be instantiated")
+        return object.__new__(cls)
+
+    """
+        The logic behind all the crud of a model
+    """
+
+    _collection: Collection = None
+
+    def set_tenant(self, tenant_name: str):
+        self.__init__(tenant=tenant_name)
+
+    def __init__(self, tenant: str = 'public', **kwargs):
+        self._collection = self.connect(tenant, self.collection_name, self.options, self.indexes, self.relations)
+        self._projection = {k: 1 for k in self.attributes if k != '*' and k not in self.guarded}
+        self._result: Cursor | InsertOneResult | dict | None = None
+        self.chained = True
+
+    def query(self) -> 'MongoDBModel':
+        self.chained = False
+        return self
+
+    def json(self) -> List[dict] | dict:
+        if self._result is None:
+            raise ChainingError(message='you can not call json directly, it needs to be chained')
+        if isinstance(self._result, Cursor):
+            return [Helper.standardize_dict(item, underscore=True) for item in list(self._result)]
+        else:
+            return Helper.standardize_dict(self._result, underscore=True)
+
+    @chained
+    def get(self, pk: str) -> Union[dict, 'MongoDBModel']:
+        return self._collection.find_one({'_id': ObjectId(pk)}, projection=self._projection)
+
+    @chained
+    def get_all(self,
+                filters: dict = None,
+                page: int = 1,
+                per_page: int = 10,
+                sort_by: tuple = None) -> Union[dict, 'MongoDBModel']:
+        sort_criteria: Sequence = [('_id', pymongo.ASCENDING)]
+
+        if sort_by is not None:
+            sort_criteria: Sequence = [sort_by]
+        cursor: Cursor = self._collection.find(
+            filters, projection=self._projection
+        ).sort(sort_criteria).skip(
+            (page * per_page) - per_page
+        ).limit(per_page)
+        # Convert cursor to list of dictionaries
+        data = [Helper.standardize_dict(item, underscore=True) for item in list(cursor)]
+        # Get total documents count
+        total_documents = self.count()
+        # Calculate total pages
+        total_pages = math.ceil(total_documents / per_page)
+
+        query_result: dict = {
+            'data': data,
+            'filters': filters,
+            'page': page,
+            'per_page': per_page,
+            'total_pages': total_pages,
+            'sort_by': [{sort_tuple[0]: sort_tuple[1]} for sort_tuple in sort_criteria],
+            'matches': len(data),
+            'total_documents': self.count()
+        }
+        return query_result
+
+    @chained
+    def find_one(self, filters: dict, sort_criteria: List[tuple] = None) -> Union[dict, 'MongoDBModel']:
+        return self._collection.find_one(filters, sort=sort_criteria, projection=self._projection)
+
+    @chained
+    def put(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
+        query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
+                                                     {'$set': {**record, **({
+                                                                                'updated_at': datetime.utcnow()
+                                                                            } if self.timestamp else {})}},
+                                                     projection=self._projection)
+        self.on_partial_update(self.get(pk).json(), record)
+        return query
+
+    @chained
+    def patch(self, pk: str, record: dict) -> Union[dict, 'MongoDBModel']:
+        query = self._collection.find_one_and_update({'_id': ObjectId(pk)},
+                                                     {'$push': record,
+                                                      '$set':
+                                                          {**({
+                                                                  'updated_at': datetime.utcnow()
+                                                              } if self.timestamp else {})}
+                                                      },
+                                                     projection=self._projection)
+        self.on_partial_update(record, self.get(pk).json())
+        return query
+
+    @chained
+    def put_patch(self, pk: str, put_record: dict, patch_record: dict) -> Union[dict, 'MongoDBModel']:
+        return self._collection.find_one_and_update({'_id': ObjectId(pk)},
+                                                    {'$set': {**put_record, **({
+                                                                                   'updated_at': datetime.utcnow()
+                                                                               } if self.timestamp else {})},
+                                                     '$push': patch_record},
+                                                    projection=self._projection)
+
+    def post(self, record: dict) -> Union[InsertOneResult, 'MongoDBModel']:
+        self.on_save(record)
+        return self._collection.insert_one({**record, **({
+                                                             'created_at': datetime.utcnow(),
+                                                             'updated_at': datetime.utcnow()
+                                                         } if self.timestamp else {})})
+
+    # def mass_patch(self):
+    #     return self._collection.update_many(
+    #         {},
+    #         [
+    #             {
+    #                 '$set': {
+    #                     'created_at': {'$toDate': '$created_at'},
+    #                     'updated_at': datetime.utcnow()
+    #                 }
+    #             }
+    #         ]
+    #     )
+
+    def delete(self, pk: str) -> bool:
+        self.on_delete(self.get(pk).json())
+        return bool(self._collection.find_one_and_delete({'_id': ObjectId(pk)}, projection=self._projection))
+
+    def count(self, filters: dict = None) -> int:
+        return self._collection.count_documents(filters if filters else {})
+
+    def distinct_values(self, key: str) -> list:
+        return self._collection.distinct(key)
```

### Comparing `mongodb_orm-0.0.129a5/mongodb_orm/types/model_schema.py` & `mongodb_orm-0.0.130/mongodb_orm/types/model_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from enum import Enum
-from typing import TypedDict, List, Dict, Optional, Union, Final
-
-
-class GeoJsonType(Enum):
-    POINT: Final[str] = 'Point'
-    LINESTRING: Final[str] = 'LineString'
-    POLYGON: Final[str] = 'Polygon'
-    MULTIPOINT: Final[str] = 'MultiPoint'
-    MULTILINESTRING: Final[str] = 'MultiLineString'
-    MULTIPOLYGON: Final[str] = 'MultiPolygon'
-
-
-class PropertySchema(TypedDict):
-    bsonType: str
-    description: Optional[str]  # Optional
-    required: Optional[List[str]]  # Optional
-    properties: Optional[Dict[str, 'PropertySchema']]  # Optional
-
-
-class ModelSchema(TypedDict):
-    bsonType: str
-    title: Optional[str]  # Optional
-    required: Optional[List[str]]  # Optional
-    properties: Dict[str, Union[PropertySchema, dict]]  # Optional
+from enum import Enum
+from typing import TypedDict, List, Dict, Optional, Union, Final
+
+
+class GeoJsonType(Enum):
+    POINT: Final[str] = 'Point'
+    LINESTRING: Final[str] = 'LineString'
+    POLYGON: Final[str] = 'Polygon'
+    MULTIPOINT: Final[str] = 'MultiPoint'
+    MULTILINESTRING: Final[str] = 'MultiLineString'
+    MULTIPOLYGON: Final[str] = 'MultiPolygon'
+
+
+class PropertySchema(TypedDict):
+    bsonType: str
+    description: Optional[str]  # Optional
+    required: Optional[List[str]]  # Optional
+    properties: Optional[Dict[str, 'PropertySchema']]  # Optional
+
+
+class ModelSchema(TypedDict):
+    bsonType: str
+    title: Optional[str]  # Optional
+    required: Optional[List[str]]  # Optional
+    properties: Dict[str, PropertySchema | dict]  # Optional
```

### Comparing `mongodb_orm-0.0.129a5/mongodb_orm/views/mongodb_api_model_view.py` & `mongodb_orm-0.0.130/mongodb_orm/views/mongodb_api_model_view.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,77 @@
-import json
-from pymongo.results import InsertOneResult
-from rest_framework.response import Response
-from rest_framework.decorators import action
-from rest_framework.viewsets import ViewSet
-from ..interfaces.mongodb_model import MongoDBModel
-from ..utils.helpers import Helper
-
-
-class MongoDBAPIModelView(MongoDBModel, ViewSet):
-
-
-    def list(self: MongoDBModel, request, *args, **kwargs) -> Response:
-        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
-        page: int = request.query_params.get('page', 1)
-        per_page: int = request.query_params.get('per_page', 5)
-        order_by: str = request.query_params.get('order_by', None)
-        order_mode: int = request.query_params.get('order_mode', 1)
-        filters: str = request.query_params.get('filters', {})
-        sort_by = None
-        if order_by:
-            sort_by = (order_by, int(order_mode))
-        query = MongoDBModel.get_all(self, filters=json.loads(filters) if filters else None, page=int(page),
-                                     per_page=int(per_page),
-                                     sort_by=sort_by)
-        return Response({'success': True, 'result': query.json()})
-
-    def retrieve(self, request, *args, **kwargs) -> Response:
-        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
-        try:
-            result = MongoDBModel.get(self, pk=str(kwargs.get('pk')))
-        except Exception as e:
-            return Response({'success': False, 'error': str(e)})
-        return Response({'success': True, 'result': result.json()})
-
-    @action(methods=['get'], detail=False)
-    def get_record_by_filters(self, request, *args, **kwargs) -> Response:
-        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
-        filters: str = request.query_params.get('filters', None)
-        if not filters:
-            return Response({'success': False, 'error': 'you need to provide at least one filter'})
-        try:
-            result = MongoDBModel.find_one(self, filters=json.loads(filters))
-        except Exception as e:
-            return Response({'success': False, 'error': str(e)})
-        return Response({'success': True, 'result': result.json()})
-
-    def create(self, request, *args, **kwargs) -> Response:
-        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
-        try:
-            new_record: InsertOneResult = MongoDBModel.post(self, Helper.standard_record(request.data))
-            retrieve_record: dict = MongoDBModel.get(self, pk=str(new_record.inserted_id)).json()
-        except Exception as e:
-            return Response({'success': False, 'error': str(e)})
-        return Response({'success': True, 'record': retrieve_record})
-
-    def update(self, request, *args, **kwargs) -> Response:
-        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
-        try:
-            MongoDBModel.put(self, pk=str(kwargs.get('pk')), record=Helper.standard_record(request.data))
-        except Exception as e:
-            return Response({'success': False, 'error': str(e)})
-        return Response({'success': True})
-
-    def partial_update(self, request, *args, **kwargs) -> Response:
-        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
-        try:
-            MongoDBModel.patch(self, pk=str(kwargs.get('pk')), record=Helper.standard_record(request.data))
-        except Exception as e:
-            return Response({'success': False, 'error': str(e)})
-        return Response({'success': True})
-
-    def destroy(self, request, *args, **kwargs) -> Response:
-        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
-        try:
-            result = MongoDBModel.delete(self, pk=str(kwargs.get('pk')))
-        except Exception as e:
-            return Response({'success': False, 'error': str(e)})
-        return Response({'success': result})
+import json
+from pymongo.results import InsertOneResult
+from rest_framework.response import Response
+from rest_framework.decorators import action
+from rest_framework.viewsets import ViewSet
+from ..interfaces.mongodb_model import MongoDBModel
+
+
+class MongoDBAPIModelView(MongoDBModel, ViewSet):
+
+    def list(self: MongoDBModel, request, *args, **kwargs) -> Response:
+        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
+        page: int = request.query_params.get('page', 1)
+        per_page: int = request.query_params.get('per_page', 5)
+        order_by: str = request.query_params.get('order_by', None)
+        order_mode: int = request.query_params.get('order_mode', 1)
+        filters: str = request.query_params.get('filters', {})
+        sort_by = None
+        if order_by:
+            sort_by = (order_by, int(order_mode))
+        query = MongoDBModel.get_all(self, filters=json.loads(filters) if filters else None, page=int(page),
+                                     per_page=int(per_page),
+                                     sort_by=sort_by)
+        return Response({'success': True, 'result': query.json()})
+
+    def retrieve(self, request, *args, **kwargs) -> Response:
+        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
+        try:
+            result = MongoDBModel.get(self, pk=str(kwargs.get('pk')))
+        except Exception as e:
+            return Response({'success': False, 'error': str(e)})
+        return Response({'success': True, 'result': result.json()})
+
+    @action(methods=['get'], detail=False)
+    def get_record_by_filters(self, request, *args, **kwargs) -> Response:
+        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
+        filters: str = request.query_params.get('filters', None)
+        if not filters:
+            return Response({'success': False, 'error': 'you need to provide at least one filter'})
+        try:
+            result = MongoDBModel.find_one(self, filters=json.loads(filters))
+        except Exception as e:
+            return Response({'success': False, 'error': str(e)})
+        return Response({'success': True, 'result': result.json()})
+
+    def create(self, request, *args, **kwargs) -> Response:
+        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
+        try:
+            new_record: InsertOneResult = MongoDBModel.post(self, request.data)
+            retrieve_record: dict = MongoDBModel.get(self, pk=str(new_record.inserted_id)).json()
+        except Exception as e:
+            return Response({'success': False, 'error': str(e)})
+        return Response({'success': True, 'record': retrieve_record})
+
+    def update(self, request, *args, **kwargs) -> Response:
+        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
+        try:
+            MongoDBModel.put(self, pk=str(kwargs.get('pk')), record=request.data)
+        except Exception as e:
+            return Response({'success': False, 'error': str(e)})
+        return Response({'success': True})
+
+    def partial_update(self, request, *args, **kwargs) -> Response:
+        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
+        try:
+            MongoDBModel.patch(self, pk=str(kwargs.get('pk')), record=request.data)
+        except Exception as e:
+            return Response({'success': False, 'error': str(e)})
+        return Response({'success': True})
+
+    def destroy(self, request, *args, **kwargs) -> Response:
+        MongoDBModel.set_tenant(self, tenant_name=request.headers.get('database', 'public'))
+        try:
+            result = MongoDBModel.delete(self, pk=str(kwargs.get('pk')))
+        except Exception as e:
+            return Response({'success': False, 'error': str(e)})
+        return Response({'success': result})
```

### Comparing `mongodb_orm-0.0.129a5/mongodb_orm.egg-info/SOURCES.txt` & `mongodb_orm-0.0.130/mongodb_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


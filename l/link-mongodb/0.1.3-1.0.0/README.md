# Comparing `tmp/link_mongodb-0.1.3.tar.gz` & `tmp/link_mongodb-1.0.0.tar.gz`

## Comparing `link_mongodb-0.1.3.tar` & `link_mongodb-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 link_mongodb-0.1.3/mkdocs.yml
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 link_mongodb-0.1.3/src/link_mongodb/__init__.py
--rw-r--r--   0        0        0    17828 2020-02-02 00:00:00.000000 link_mongodb-0.1.3/src/link_mongodb/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 link_mongodb-0.1.3/src/link_mongodb/py.typed
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 link_mongodb-0.1.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 link_mongodb-0.1.3/LICENSE
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 link_mongodb-0.1.3/README.md
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 link_mongodb-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 link_mongodb-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/mkdocs.yml
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/src/link_mongodb/__init__.py
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/src/link_mongodb/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/src/link_mongodb/py.typed
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/README.md
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 link_mongodb-1.0.0/PKG-INFO
```

### Comparing `link_mongodb-0.1.3/mkdocs.yml` & `link_mongodb-1.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `link_mongodb-0.1.3/src/link_mongodb/core.py` & `link_mongodb-1.0.0/src/link_mongodb/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,17 @@
     print("Connecting to MongoDB server...")
     with MongoClient(mongodb_uri) as client:
         collection = client[database_name][collection_name]
 
         try:
             print(f"Executing insert_one query with document: {document}")
             result = collection.insert_one(document)
-            result_dict = collection.find_one({"_id": result.inserted_id})
-            print(f"result: {result_dict}")
-            return result_dict
+            # result_dict = collection.find_one({"_id": result.inserted_id})
+            # print(f"result: {result_dict}")
+            return result
         except errors.PyMongoError as e:
             raise Exception(f"An error occurred while querying the MongoDB collection: {str(e)}")
         
 def insert_many(mongodb_uri: str, database_name: str, collection_name: str, documents: List[Dict]) -> Optional[List]:
     """
     Inserts multiple documents into a MongoDB collection.
 
@@ -107,15 +107,15 @@
     with MongoClient(mongodb_uri) as client:
         collection = client[database_name][collection_name]
 
         try:
             print(f"Executing insert_many query with documents: {documents}")
             result = collection.insert_many(documents)
             print(f"ids of the inserted document: {result.inserted_ids}")
-            return result.inserted_ids
+            return result
         except errors.PyMongoError as e:
             raise Exception(f"An error occurred while querying the MongoDB collection: {str(e)}")
         
 
 def update_one(mongodb_uri: str, database_name: str, collection_name: str, filter: Dict, update: Dict) -> Optional[Dict]:
     """
     Updates a document in a MongoDB collection based on the provided filter and update parameters.
@@ -138,14 +138,15 @@
         collection = client[database_name][collection_name]
 
         try:
             print(f"Executing update_one query with filter: {filter} and update: {update}")
             result = collection.update_one(filter=filter, update=update)
             result_dict = result.raw_result
             print(f"result: {result_dict}")
+            return result
         except errors.PyMongoError as e:
             raise Exception(f"An error occurred while querying the MongoDB collection: {str(e)}")
 
 def update_many(mongodb_uri: str, database_name: str, collection_name: str, filter: Dict, update: Dict) -> Optional[Dict]:
     """
     Updates multiple documents in a MongoDB collection that match the specified filter with the given update.
 
@@ -166,15 +167,15 @@
     with MongoClient(mongodb_uri) as client:
         collection = client[database_name][collection_name]
 
         try:
             print(f"Executing update_many query with filter: {filter} and update: {update}")
             result = collection.update_many(filter=filter, update=update)
             print(f"matched count: {result.matched_count} modified count: {result.modified_count}")
-            return result.raw_result
+            return result
         except errors.PyMongoError as e:
             raise Exception(f"An error occurred while querying the MongoDB collection: {str(e)}")
         
 def delete_one(mongodb_uri: str, database_name: str, collection_name: str, filter: Dict) -> Optional[Dict]:
     """
     Deletes a single document from a MongoDB collection that matches the specified filter.
 
@@ -194,15 +195,15 @@
     with MongoClient(mongodb_uri) as client:
         collection = client[database_name][collection_name]
 
         try:
             print(f"Executing delete_one query with filter: {filter}")
             result = collection.delete_one(filter=filter)
             print(f"Query result: {result.raw_result}")
-            return result.raw_result
+            return result
         except errors.PyMongoError as e:
             raise Exception(f"An error occurred while querying the MongoDB collection: {str(e)}")
         
 def delete_many(mongodb_uri: str, database_name: str, collection_name: str, filter: Dict) -> Optional[Dict]:
     """
     Deletes multiple documents from a MongoDB collection based on the provided filter.
     
@@ -222,15 +223,15 @@
     with MongoClient(mongodb_uri) as client:
         collection = client[database_name][collection_name]
 
         try:
             print(f"Executing delete_many query with filter: {filter}")
             result = collection.delete_many(filter=filter)
             print(f"Query result: {result.raw_result}")
-            return result.raw_result
+            return result
         except errors.PyMongoError as e:
             raise Exception(f"An error occurred while querying the MongoDB collection: {str(e)}")
         
 def count(mongodb_uri: str, database_name: str, collection_name: str, filter: Dict) -> Optional[Dict]:
     """
     Counts the number of documents in a MongoDB collection that match the specified filter.
```

### Comparing `link_mongodb-0.1.3/.gitignore` & `link_mongodb-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `link_mongodb-0.1.3/LICENSE` & `link_mongodb-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `link_mongodb-0.1.3/README.md` & `link_mongodb-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `link_mongodb-0.1.3/pyproject.toml` & `link_mongodb-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "pymongo == 4.6.1",
+  "pymongo == 4.5.0",
 ]
 description = "link mongo database"
 dynamic = ["version"]
 keywords = []
 license = "MIT"
 name = "link_mongodb"
 readme = "README.md"
```

### Comparing `link_mongodb-0.1.3/PKG-INFO` & `link_mongodb-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: link_mongodb
-Version: 0.1.3
+Version: 1.0.0
 Summary: link mongo database
 Project-URL: Documentation, https://asmitul.github.io/link-mongodb
 Project-URL: Issues, https://github.com/asmitul/link-mongodb/issues
 Project-URL: Source, https://github.com/asmitul/link-mongodb
 Author: asmitul
 License-Expression: MIT
 License-File: LICENSE
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.12,>=3.8
-Requires-Dist: pymongo==4.6.1
+Requires-Dist: pymongo==4.5.0
 Provides-Extra: docs
 Requires-Dist: mkdocs-git-revision-date-localized-plugin~=1.1.0; extra == 'docs'
 Requires-Dist: mkdocs-material~=8.5.4; extra == 'docs'
 Requires-Dist: mkdocstrings[python]~=0.19.0; extra == 'docs'
 Requires-Dist: mkdocs~=1.4.0; extra == 'docs'
 Provides-Extra: quality
 Requires-Dist: black~=22.10.0; extra == 'quality'
```


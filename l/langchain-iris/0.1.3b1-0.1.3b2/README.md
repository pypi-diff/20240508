# Comparing `tmp/langchain_iris-0.1.3b1.tar.gz` & `tmp/langchain_iris-0.1.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_iris-0.1.3b1.tar", last modified: Tue Apr 16 10:32:45 2024, max compression
+gzip compressed data, was "langchain_iris-0.1.3b2.tar", last modified: Wed May  8 10:53:37 2024, max compression
```

## Comparing `langchain_iris-0.1.3b1.tar` & `langchain_iris-0.1.3b2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:32:45.730961 langchain_iris-0.1.3b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-16 10:32:25.000000 langchain_iris-0.1.3b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-16 10:32:45.730961 langchain_iris-0.1.3b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-16 10:32:25.000000 langchain_iris-0.1.3b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:32:45.730961 langchain_iris-0.1.3b1/langchain_iris/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 10:32:25.000000 langchain_iris-0.1.3b1/langchain_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19669 2024-04-16 10:32:25.000000 langchain_iris-0.1.3b1/langchain_iris/vectorstores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:32:45.730961 langchain_iris-0.1.3b1/langchain_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-16 10:32:45.000000 langchain_iris-0.1.3b1/langchain_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-16 10:32:45.000000 langchain_iris-0.1.3b1/langchain_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:32:45.000000 langchain_iris-0.1.3b1/langchain_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 10:32:45.000000 langchain_iris-0.1.3b1/langchain_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 10:32:45.000000 langchain_iris-0.1.3b1/langchain_iris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-16 10:32:45.730961 langchain_iris-0.1.3b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 10:32:25.000000 langchain_iris-0.1.3b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:32:45.730961 langchain_iris-0.1.3b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-04-16 10:32:25.000000 langchain_iris-0.1.3b1/tests/test_vectorstores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/langchain_iris/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/langchain_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19886 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/langchain_iris/vectorstores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/langchain_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/tests/test_vectorstores.py
```

### Comparing `langchain_iris-0.1.3b1/LICENSE` & `langchain_iris-0.1.3b2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_iris-0.1.3b1/PKG-INFO` & `langchain_iris-0.1.3b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-iris
-Version: 0.1.3b1
+Version: 0.1.3b2
 Summary: The InterSystems IRIS adoption for Langchain
 Home-page: https://github.com/caretdev/langchain-iris
 Project-URL: Source, https://github.com/caretdev/langchain-iris
 Project-URL: Tracker, https://github.com/caretdev/langchain-iris/issues
 Keywords: "InterSystems IRIS"
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langchain_iris-0.1.3b1/README.md` & `langchain_iris-0.1.3b2/README.md`

 * *Files identical despite different names*

### Comparing `langchain_iris-0.1.3b1/langchain_iris/vectorstores.py` & `langchain_iris-0.1.3b2/langchain_iris/vectorstores.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,23 @@
         self.collection_name = collection_name
         self.pre_delete_collection = pre_delete_collection
         self.collection_metadata = collection_metadata
         self._distance_strategy = distance_strategy
         self.logger = logger or logging.getLogger(__name__)
         self.override_relevance_score_fn = relevance_score_fn
         self.engine_args = engine_args or {}
-        self._conn = connection if connection else self.connect()
+        if connection:
+            self._conn = connection 
+            try:
+                if connection.dialect.supports_vectors:
+                    self.native_vector = True
+            except:  # noqa
+                pass
+        else: 
+            self._conn = self.connect()
 
         self.__post_init__()
 
     def __post_init__(
         self,
     ) -> None:
         """
```

### Comparing `langchain_iris-0.1.3b1/langchain_iris.egg-info/PKG-INFO` & `langchain_iris-0.1.3b2/langchain_iris.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-iris
-Version: 0.1.3b1
+Version: 0.1.3b2
 Summary: The InterSystems IRIS adoption for Langchain
 Home-page: https://github.com/caretdev/langchain-iris
 Project-URL: Source, https://github.com/caretdev/langchain-iris
 Project-URL: Tracker, https://github.com/caretdev/langchain-iris/issues
 Keywords: "InterSystems IRIS"
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langchain_iris-0.1.3b1/setup.cfg` & `langchain_iris-0.1.3b2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = langchain-iris
-version = 0.1.3b1
+version = 0.1.3b2
 description = The InterSystems IRIS adoption for Langchain
 long_description = file: README.md
 url = https://github.com/caretdev/langchain-iris
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
```

### Comparing `langchain_iris-0.1.3b1/tests/test_vectorstores.py` & `langchain_iris-0.1.3b2/tests/test_vectorstores.py`

 * *Files identical despite different names*


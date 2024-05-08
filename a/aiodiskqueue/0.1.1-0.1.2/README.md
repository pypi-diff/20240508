# Comparing `tmp/aiodiskqueue-0.1.1.tar.gz` & `tmp/aiodiskqueue-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.1.tar` & `aiodiskqueue-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1080 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/LICENSE
--rw-r--r--   0        0        0     2982 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/README.rst
--rw-r--r--   0        0        0     1053 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      256 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0      230 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/__init__.py
--rw-r--r--   0        0        0     1172 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/base.py
--rw-r--r--   0        0        0     3121 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/dbm.py
--rw-r--r--   0        0        0     3476 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/simple.py
--rw-r--r--   0        0        0     2166 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/engines/sqlite.py
--rw-r--r--   0        0        0      268 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0     7934 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/queues.py
--rw-r--r--   0        0        0      714 2023-06-09 11:23:48.665306 aiodiskqueue-0.1.1/src/aiodiskqueue/utils.py
--rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2982 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/README.rst
+-rw-r--r--   0        0        0     1053 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      256 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/src/aiodiskqueue/engines/__init__.py
+-rw-r--r--   0        0        0     1172 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/src/aiodiskqueue/engines/base.py
+-rw-r--r--   0        0        0     3121 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/src/aiodiskqueue/engines/dbm.py
+-rw-r--r--   0        0        0     3476 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/src/aiodiskqueue/engines/simple.py
+-rw-r--r--   0        0        0     2321 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/src/aiodiskqueue/engines/sqlite.py
+-rw-r--r--   0        0        0      268 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0     7934 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/src/aiodiskqueue/queues.py
+-rw-r--r--   0        0        0      714 2024-05-08 20:51:13.430605 aiodiskqueue-0.1.2/src/aiodiskqueue/utils.py
+-rw-r--r--   0        0        0     3942 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.2/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.1/LICENSE` & `aiodiskqueue-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.1/README.rst` & `aiodiskqueue-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.1/pyproject.toml` & `aiodiskqueue-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.1/src/aiodiskqueue/engines/base.py` & `aiodiskqueue-0.1.2/src/aiodiskqueue/engines/base.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.1/src/aiodiskqueue/engines/dbm.py` & `aiodiskqueue-0.1.2/src/aiodiskqueue/engines/dbm.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.1/src/aiodiskqueue/engines/simple.py` & `aiodiskqueue-0.1.2/src/aiodiskqueue/engines/simple.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.1/src/aiodiskqueue/engines/sqlite.py` & `aiodiskqueue-0.1.2/src/aiodiskqueue/engines/sqlite.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,11 +62,15 @@
                 )
 
         async def remove_item(self):
             async with aiosqlite.connect(self._data_path, isolation_level=None) as db:
                 await db.execute(
                     """
                         DELETE FROM queue
-                        ORDER BY rowid
-                        LIMIT 1;
+                        WHERE rowid IN (
+                            SELECT rowid
+                            FROM queue
+                            ORDER BY rowid
+                            LIMIT 1
+                        );
                     """
                 )
```

### Comparing `aiodiskqueue-0.1.1/src/aiodiskqueue/queues.py` & `aiodiskqueue-0.1.2/src/aiodiskqueue/queues.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.1/src/aiodiskqueue/utils.py` & `aiodiskqueue-0.1.2/src/aiodiskqueue/utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.1/PKG-INFO` & `aiodiskqueue-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.1
+Version: 0.1.2
 Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```


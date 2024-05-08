# Comparing `tmp/elasticsearch_pii_redacter-1.9.1.tar.gz` & `tmp/elasticsearch_pii_redacter-1.9.2.tar.gz`

## Comparing `elasticsearch_pii_redacter-1.9.1.tar` & `elasticsearch_pii_redacter-1.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/__init__.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/cli.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/defaults.py
--rw-r--r--   0        0        0    24416 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/elastic_api.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/exceptions.py
--rw-r--r--   0        0        0    10535 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/helpers.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/logtools.py
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/main.py
--rw-r--r--   0        0        0    20892 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/redacters.py
--rw-r--r--   0        0        0    19177 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/tracking.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/version.py
--rw-r--r--   0        0        0    12956 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/app/waiters.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/.gitignore
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/README.rst
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/__init__.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/cli.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/defaults.py
+-rw-r--r--   0        0        0    24416 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/elastic_api.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/exceptions.py
+-rw-r--r--   0        0        0    10535 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/helpers.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/logtools.py
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/main.py
+-rw-r--r--   0        0        0    20892 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/redacters.py
+-rw-r--r--   0        0        0    19177 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/tracking.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/version.py
+-rw-r--r--   0        0        0    12956 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/app/waiters.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/.gitignore
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/README.rst
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 elasticsearch_pii_redacter-1.9.2/PKG-INFO
```

### Comparing `elasticsearch_pii_redacter-1.9.1/app/cli.py` & `elasticsearch_pii_redacter-1.9.2/app/cli.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/app/defaults.py` & `elasticsearch_pii_redacter-1.9.2/app/defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/app/elastic_api.py` & `elasticsearch_pii_redacter-1.9.2/app/elastic_api.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/app/exceptions.py` & `elasticsearch_pii_redacter-1.9.2/app/exceptions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/app/helpers.py` & `elasticsearch_pii_redacter-1.9.2/app/helpers.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/app/logtools.py` & `elasticsearch_pii_redacter-1.9.2/app/logtools.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/app/main.py` & `elasticsearch_pii_redacter-1.9.2/app/main.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/app/redacters.py` & `elasticsearch_pii_redacter-1.9.2/app/redacters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/app/tracking.py` & `elasticsearch_pii_redacter-1.9.2/app/tracking.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/app/waiters.py` & `elasticsearch_pii_redacter-1.9.2/app/waiters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/README.rst` & `elasticsearch_pii_redacter-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/pyproject.toml` & `elasticsearch_pii_redacter-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `elasticsearch_pii_redacter-1.9.1/PKG-INFO` & `elasticsearch_pii_redacter-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-pii-redacter
-Version: 1.9.1
+Version: 1.9.2
 Summary: Redacting field data from your Elasticsearch indices and Searchable Snapshots
 Project-URL: Homepage, https://github.com/elastic/elastic-pii-redacter
 Project-URL: Bug Tracker, https://github.com/elastic/elastic-pii-redacter/issues
 Author-email: Elastic <info@elastic.co>
 License: Apache-2.0
 Keywords: elasticsearch,index,pii,redact
 Classifier: Intended Audience :: Developers
```


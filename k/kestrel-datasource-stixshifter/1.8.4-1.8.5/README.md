# Comparing `tmp/kestrel_datasource_stixshifter-1.8.4.tar.gz` & `tmp/kestrel_datasource_stixshifter-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kestrel_datasource_stixshifter-1.8.4.tar", last modified: Thu May  2 15:44:20 2024, max compression
+gzip compressed data, was "kestrel_datasource_stixshifter-1.8.5.tar", last modified: Wed May  8 15:12:11 2024, max compression
```

## Comparing `kestrel_datasource_stixshifter-1.8.4.tar` & `kestrel_datasource_stixshifter-1.8.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:44:20.009048 kestrel_datasource_stixshifter-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-02 15:44:20.009048 kestrel_datasource_stixshifter-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:44:20.009048 kestrel_datasource_stixshifter-1.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:44:20.001047 kestrel_datasource_stixshifter-1.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:44:20.005047 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/subquery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:44:20.005047 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/worker/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/worker/transmitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:44:20.009048 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-02 15:44:19.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-02 15:44:20.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:44:19.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 15:44:19.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 15:44:19.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 15:44:19.000000 kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:44:20.005047 kestrel_datasource_stixshifter-1.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/tests/test_command_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/tests/test_stixshifter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/tests/test_stixshifter_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-02 15:44:08.000000 kestrel_datasource_stixshifter-1.8.4/tests/test_stixshifter_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:12:11.732315 kestrel_datasource_stixshifter-1.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-08 15:12:11.732315 kestrel_datasource_stixshifter-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:12:11.732315 kestrel_datasource_stixshifter-1.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:12:11.724315 kestrel_datasource_stixshifter-1.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:12:11.728315 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/subquery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:12:11.728315 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/worker/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/worker/transmitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:12:11.732315 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-08 15:12:11.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-08 15:12:11.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:12:11.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 15:12:11.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:12:11.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 15:12:11.000000 kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:12:11.728315 kestrel_datasource_stixshifter-1.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/tests/test_command_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/tests/test_stixshifter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/tests/test_stixshifter_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-08 15:11:59.000000 kestrel_datasource_stixshifter-1.8.5/tests/test_stixshifter_translator.py
```

### Comparing `kestrel_datasource_stixshifter-1.8.4/PKG-INFO` & `kestrel_datasource_stixshifter-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: kestrel_datasource_stixshifter
-Version: 1.8.4
+Version: 1.8.5
 Summary: Kestrel STIX-shifter Datasource Interface
 Maintainer-email: Xiaokui Shu <xiaokui.shu@ibm.com>, Paul Coccoli <pcoccoli@us.ibm.com>
 License: Apache 2.0 License
 Project-URL: Homepage, https://github.com/opencybersecurityalliance/kestrel-lang
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Project-URL: Repository, https://github.com/opencybersecurityalliance/kestrel-lang.git
 Keywords: kestrel,datasource,interface,STIX-shifter
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: kestrel_core>=1.8.1
+Requires-Dist: kestrel_core>=1.8.2
 Requires-Dist: lxml==4.9.4
 Requires-Dist: requests>=2.31.0
 Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: stix-shifter==7.0.6
-Requires-Dist: stix-shifter-utils==7.0.6
+Requires-Dist: stix-shifter==7.0.7
+Requires-Dist: stix-shifter-utils==7.0.7
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: stix-shifter-modules-elastic-ecs; extra == "test"
 
 .. image:: https://github.com/opencybersecurityalliance/kestrel-lang/raw/develop/logo/logo_w_text.png
    :width: 460
    :alt: Kestrel Threat Hunting Language
```

### Comparing `kestrel_datasource_stixshifter-1.8.4/README.rst` & `kestrel_datasource_stixshifter-1.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/pyproject.toml` & `kestrel_datasource_stixshifter-1.8.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 68.2.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kestrel_datasource_stixshifter"
-version = "1.8.4"
+version = "1.8.5"
 description = "Kestrel STIX-shifter Datasource Interface"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "Apache 2.0 License"}
 maintainers = [
     {name = "Xiaokui Shu", email = "xiaokui.shu@ibm.com"},
     {name = "Paul Coccoli", email = "pcoccoli@us.ibm.com"},
@@ -23,20 +23,20 @@
     "Topic :: Security",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
 ]
 
 dependencies = [
-    "kestrel_core>=1.8.1",
+    "kestrel_core>=1.8.2",
     "lxml==4.9.4", # Python 3.8 on mac error >5.0.0; stackoverflow #75442675
     "requests>=2.31.0",
     "nest-asyncio>=1.6.0",
-    "stix-shifter==7.0.6",
-    "stix-shifter-utils==7.0.6",
+    "stix-shifter==7.0.7",
+    "stix-shifter-utils==7.0.7",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "stix-shifter-modules-elastic-ecs",
 ]
```

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/cli.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/cli.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/config.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/config.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/connector.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/connector.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/diagnosis.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/diagnosis.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/interface.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         profiles:
             host101:
                 connector: elastic_ecs
                 connection:
                     host: elastic.securitylog.company.com
                     port: 9200
                     indices: host101
+                    pagination: false # disable pagination (only <10k results) to have better performance; Kestrel default: true
                     options:  # use any of this section when needed
                         verify_cert: false  # allow invalid/expired/self-signed certificate
                         retrieval_batch_size: 10000  # set to 10000 to match default Elasticsearch page size; Kestrel default across connectors: 2000
                         single_batch_timeout: 120  # increase it if hit 60 seconds (Kestrel default) timeout error for each batch of retrieval
                         cool_down_after_transmission: 2  # seconds to cool down between data source API calls, required by some API such as sentinelone; Kestrel default: 0
                         subquery_time_window: 3600 # split each query into multiple subqueries with smaller time windows specified here in seconds; Kestrel default: 0 (not split query)
                         allow_dev_connector: True  # do not check version of a connector to allow custom/testing connector installed with any version; Kestrel default: False
```

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/multiproc.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/multiproc.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/query.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/query.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/subquery.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/subquery.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/worker/translator.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/worker/translator.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/worker/transmitter.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/worker/transmitter.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter/worker/utils.py` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter/worker/utils.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter.egg-info/PKG-INFO` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: kestrel_datasource_stixshifter
-Version: 1.8.4
+Version: 1.8.5
 Summary: Kestrel STIX-shifter Datasource Interface
 Maintainer-email: Xiaokui Shu <xiaokui.shu@ibm.com>, Paul Coccoli <pcoccoli@us.ibm.com>
 License: Apache 2.0 License
 Project-URL: Homepage, https://github.com/opencybersecurityalliance/kestrel-lang
 Project-URL: Documentation, https://kestrel.readthedocs.io/
 Project-URL: Repository, https://github.com/opencybersecurityalliance/kestrel-lang.git
 Keywords: kestrel,datasource,interface,STIX-shifter
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Requires-Dist: kestrel_core>=1.8.1
+Requires-Dist: kestrel_core>=1.8.2
 Requires-Dist: lxml==4.9.4
 Requires-Dist: requests>=2.31.0
 Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: stix-shifter==7.0.6
-Requires-Dist: stix-shifter-utils==7.0.6
+Requires-Dist: stix-shifter==7.0.7
+Requires-Dist: stix-shifter-utils==7.0.7
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: stix-shifter-modules-elastic-ecs; extra == "test"
 
 .. image:: https://github.com/opencybersecurityalliance/kestrel-lang/raw/develop/logo/logo_w_text.png
    :width: 460
    :alt: Kestrel Threat Hunting Language
```

### Comparing `kestrel_datasource_stixshifter-1.8.4/src/kestrel_datasource_stixshifter.egg-info/SOURCES.txt` & `kestrel_datasource_stixshifter-1.8.5/src/kestrel_datasource_stixshifter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/tests/test_command_get.py` & `kestrel_datasource_stixshifter-1.8.5/tests/test_command_get.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/tests/test_stixshifter.py` & `kestrel_datasource_stixshifter-1.8.5/tests/test_stixshifter.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/tests/test_stixshifter_diagnosis.py` & `kestrel_datasource_stixshifter-1.8.5/tests/test_stixshifter_diagnosis.py`

 * *Files identical despite different names*

### Comparing `kestrel_datasource_stixshifter-1.8.4/tests/test_stixshifter_translator.py` & `kestrel_datasource_stixshifter-1.8.5/tests/test_stixshifter_translator.py`

 * *Files identical despite different names*


# Comparing `tmp/confhub-0.0.3.2a0.tar.gz` & `tmp/confhub-0.0.3a0.tar.gz`

## Comparing `confhub-0.0.3.2a0.tar` & `confhub-0.0.3a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/CHANGELOG.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/__main__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/__meta__.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/commands.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/enums.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/exceptions.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/models.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/reader.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/setup_logger.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/confhub/templates.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/tests/.secrets.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/tests/example__secrets.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/tests/settings.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/tests/test_confhub.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/LICENSE
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/README.md
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/pyproject.toml
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 confhub-0.0.3.2a0/PKG-INFO
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 confhub-0.0.3a0/CHANGELOG.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 confhub-0.0.3a0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/__init__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/__meta__.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/commands.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/enums.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/exceptions.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/models.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/reader.py
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/setup_logger.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/templates.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 confhub-0.0.3a0/tests/.secrets.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 confhub-0.0.3a0/tests/example__secrets.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 confhub-0.0.3a0/tests/settings.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 confhub-0.0.3a0/tests/test_confhub.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 confhub-0.0.3a0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 confhub-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 confhub-0.0.3a0/README.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 confhub-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 confhub-0.0.3a0/PKG-INFO
```

### Comparing `confhub-0.0.3.2a0/confhub/__main__.py` & `confhub-0.0.3a0/confhub/__main__.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/confhub/commands.py` & `confhub-0.0.3a0/confhub/commands.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/confhub/enums.py` & `confhub-0.0.3a0/confhub/enums.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/confhub/exceptions.py` & `confhub-0.0.3a0/confhub/exceptions.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/confhub/models.py` & `confhub-0.0.3a0/confhub/models.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/confhub/reader.py` & `confhub-0.0.3a0/confhub/reader.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/confhub/setup_logger.py` & `confhub-0.0.3a0/confhub/setup_logger.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/confhub/templates.py` & `confhub-0.0.3a0/confhub/templates.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/tests/test_confhub.py` & `confhub-0.0.3a0/tests/test_confhub.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/.gitignore` & `confhub-0.0.3a0/.gitignore`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/LICENSE` & `confhub-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/README.md` & `confhub-0.0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3.2a0/pyproject.toml` & `confhub-0.0.3a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,11 +40,8 @@
 ]
 dynamic = ["version"]
 
 [tool.hatch.version]
 path = "confhub/__meta__.py"
 
 [project.urls]
-Repository = "https://github.com/morington/confhub/"
-
-[project.scripts]
-hello-world = "confhub:confhub"
+Repository = "https://github.com/morington/confhub/"
```

### Comparing `confhub-0.0.3.2a0/PKG-INFO` & `confhub-0.0.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: confhub
-Version: 0.0.3.2a0
+Version: 0.0.3a0
 Summary: Configuration add-on to Dynaconf
 Project-URL: Repository, https://github.com/morington/confhub/
 Author-email: Adam Morington <morington.mail@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: cfg,confhub,config,configuration,dynaconf,setting,settings
 Classifier: Development Status :: 3 - Alpha
```


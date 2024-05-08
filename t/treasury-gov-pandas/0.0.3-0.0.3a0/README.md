# Comparing `tmp/treasury_gov_pandas-0.0.3.tar.gz` & `tmp/treasury_gov_pandas-0.0.3a0.tar.gz`

## Comparing `treasury_gov_pandas-0.0.3.tar` & `treasury_gov_pandas-0.0.3a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3/src/treasury_gov_pandas/__init__.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3/src/treasury_gov_pandas/load.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3/LICENSE
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3a0/src/treasury_gov_pandas/__init__.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3a0/src/treasury_gov_pandas/load.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3a0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3a0/LICENSE
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3a0/README.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 treasury_gov_pandas-0.0.3a0/PKG-INFO
```

### Comparing `treasury_gov_pandas-0.0.3/src/treasury_gov_pandas/load.py` & `treasury_gov_pandas-0.0.3a0/src/treasury_gov_pandas/load.py`

 * *Files identical despite different names*

### Comparing `treasury_gov_pandas-0.0.3/LICENSE` & `treasury_gov_pandas-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `treasury_gov_pandas-0.0.3/pyproject.toml` & `treasury_gov_pandas-0.0.3a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "treasury_gov_pandas"
-version = "0.0.3"
+version = "0.0.3a0"
 authors = [
   { name="Eduardo Cavazos", email="wayo.cavazos@gmail.com" },
 ]
 description = "Library for downloading treasury.gov datasets."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `treasury_gov_pandas-0.0.3/PKG-INFO` & `treasury_gov_pandas-0.0.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: treasury_gov_pandas
-Version: 0.0.3
+Version: 0.0.3a0
 Summary: Library for downloading treasury.gov datasets.
 Project-URL: Homepage, https://github.com/dharmatech/treasury_gov_pandas.py
 Project-URL: Issues, https://github.com/dharmatech/treasury_gov_pandas.py/issues
 Author-email: Eduardo Cavazos <wayo.cavazos@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/aiondata-0.4.3.tar.gz` & `tmp/aiondata-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiondata-0.4.3.tar", max compression
+gzip compressed data, was "aiondata-0.4.4.tar", max compression
```

## Comparing `aiondata-0.4.3.tar` & `aiondata-0.4.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11372 2024-05-05 08:08:35.202989 aiondata-0.4.3/LICENSE
--rw-r--r--   0        0        0     4606 2024-05-05 08:08:35.202989 aiondata-0.4.3/README.md
--rw-r--r--   0        0        0      419 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/__init__.py
--rw-r--r--   0        0        0     5289 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/bindingdb.py
--rw-r--r--   0        0        0     2118 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/datasets.py
--rw-r--r--   0        0        0     4714 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/moleculenet.py
--rw-r--r--   0        0        0     8692 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/protein_structure.py
--rw-r--r--   0        0        0     5413 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/weizmann_ccca.py
--rw-r--r--   0        0        0     1505 2024-05-05 08:08:35.206989 aiondata-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11372 2024-05-08 08:27:22.469074 aiondata-0.4.4/LICENSE
+-rw-r--r--   0        0        0     4606 2024-05-08 08:27:22.469074 aiondata-0.4.4/README.md
+-rw-r--r--   0        0        0      419 2024-05-08 08:27:22.469074 aiondata-0.4.4/aiondata/__init__.py
+-rw-r--r--   0        0        0     5360 2024-05-08 08:27:22.469074 aiondata-0.4.4/aiondata/bindingdb.py
+-rw-r--r--   0        0        0     2118 2024-05-08 08:27:22.469074 aiondata-0.4.4/aiondata/datasets.py
+-rw-r--r--   0        0        0     4714 2024-05-08 08:27:22.469074 aiondata-0.4.4/aiondata/moleculenet.py
+-rw-r--r--   0        0        0     8692 2024-05-08 08:27:22.469074 aiondata-0.4.4/aiondata/protein_structure.py
+-rw-r--r--   0        0        0     5413 2024-05-08 08:27:22.469074 aiondata-0.4.4/aiondata/weizmann_ccca.py
+-rw-r--r--   0        0        0     1505 2024-05-08 08:27:22.469074 aiondata-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.4.4/PKG-INFO
```

### Comparing `aiondata-0.4.3/LICENSE` & `aiondata-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.3/README.md` & `aiondata-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.3/aiondata/bindingdb.py` & `aiondata-0.4.4/aiondata/bindingdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,17 @@
             if cached_sdf.exists():
                 self.fd = self.from_compressed_file(cached_sdf)
             else:
                 self.fd = self.from_url(self.SOURCE)
         else:
             self.fd = fd
 
-    @staticmethod
-    def _convert_to_numeric(prop_name: str, value: str) -> Union[int, float, str, None]:
+    def _convert_to_numeric(
+        self, prop_name: str, value: str
+    ) -> Union[int, float, str, None]:
         """
         Converts a property value to numeric type.
 
         Args:
             prop_name (str): The name of the property.
             value (str): The value of the property.
 
@@ -68,60 +69,60 @@
                     return int(float_value)
                 else:
                     return float_value
             except ValueError:
                 return value
 
     @staticmethod
-    def from_url(url: str) -> "BindingDB":
+    def from_url(url: str) -> io.BufferedReader:
         """
         Creates a BindingDB instance from a URL containing a compressed SDF file, using streaming.
 
         Args:
             url (str): The URL of the dataset.
 
         Returns:
-            A BindingDB instance.
+            A BufferedReader instance containing the content of the SDF file.
         """
         with urllib.request.urlopen(url) as response:
             with zipfile.ZipFile(io.BytesIO(response.read())) as z:
                 sdf_name = z.namelist()[0]
                 with z.open(sdf_name) as sdf_file:
                     sdf_content = io.BufferedReader(sdf_file)
-        return BindingDB(sdf_content)
+        return sdf_content
 
     @staticmethod
-    def from_compressed_file(file_path: str) -> "BindingDB":
+    def from_compressed_file(file_path: str) -> io.BufferedReader:
         """
         Creates a BindingDB instance from a compressed SDF file.
 
         Args:
             file_path (str): The path to the compressed file.
 
         Returns:
-            A BindingDB instance.
+            A BufferedReader instance containing the content of the SDF file.
         """
         with zipfile.ZipFile(file_path) as z:
             sdf_name = z.namelist()[0]
             with z.open(sdf_name) as sdf_file:
                 sdf_content = io.BufferedReader(sdf_file)
-        return BindingDB(sdf_content)
+        return sdf_content
 
     @staticmethod
-    def from_uncompressed_file(file_path: str) -> "BindingDB":
+    def from_uncompressed_file(file_path: str) -> io.BufferedReader:
         """
         Creates a BindingDB instance from an uncompressed SDF file.
 
         Args:
             file_path (str): The path to the uncompressed file.
 
         Returns:
-            A BindingDB instance.
+            A BufferedReader instance containing the content of the SDF file.
         """
-        return BindingDB(open(file_path, "rb"))
+        return open(file_path, "rb")
 
     def to_generator(self, progress_bar: bool = True) -> Generator[dict, None, None]:
         """
         Converts the dataset to a generator.
 
         Args:
             progress_bar (bool): Whether to display a progress bar.
@@ -151,13 +152,11 @@
                     if "PubChem SID" in record:
                         record["PubChem SID of Ligand"] = record.pop("PubChem SID")
                     if "PubChem CID" in record:
                         record["PubChem CID of Ligand"] = record.pop("PubChem CID")
 
                     record["SMILES"] = Chem.MolToSmiles(mol)
                     yield record
-                else:
-                    break
 
         # Re-enable logging
         RDLogger.EnableLog("rdApp.error")
         RDLogger.EnableLog("rdApp.warning")
```

### Comparing `aiondata-0.4.3/aiondata/datasets.py` & `aiondata-0.4.4/aiondata/datasets.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.3/aiondata/moleculenet.py` & `aiondata-0.4.4/aiondata/moleculenet.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.3/aiondata/protein_structure.py` & `aiondata-0.4.4/aiondata/protein_structure.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.3/aiondata/weizmann_ccca.py` & `aiondata-0.4.4/aiondata/weizmann_ccca.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.3/pyproject.toml` & `aiondata-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiondata"
-version = "0.4.3"
+version = "0.4.4"
 description = "A common data access layer for AI-driven drug discovery."
 authors = ["JJ Ben-Joseph <jj@tensorspace.ai>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://www.github.com/aion-labs/aiondata"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `aiondata-0.4.3/PKG-INFO` & `aiondata-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiondata
-Version: 0.4.3
+Version: 0.4.4
 Summary: A common data access layer for AI-driven drug discovery.
 Home-page: https://www.github.com/aion-labs/aiondata
 License: Apache
 Author: JJ Ben-Joseph
 Author-email: jj@tensorspace.ai
 Requires-Python: >=3.10
 Classifier: Development Status :: 3 - Alpha
```


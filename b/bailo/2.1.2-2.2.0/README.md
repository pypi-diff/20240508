# Comparing `tmp/bailo-2.1.2.tar.gz` & `tmp/bailo-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bailo-2.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bailo-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bailo-2.1.2.tar` & `bailo-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2241 2024-04-24 14:35:49.087870 bailo-2.1.2/README.md
--rw-r--r--   0        0        0     4869 2024-04-24 14:35:49.087870 bailo-2.1.2/pyproject.toml
--rw-r--r--   0        0        0      616 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/__init__.py
--rw-r--r--   0        0        0      153 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/__init__.py
--rw-r--r--   0        0        0     3458 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/agent.py
--rw-r--r--   0        0        0    19238 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/client.py
--rw-r--r--   0        0        0      672 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/enums.py
--rw-r--r--   0        0        0      221 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/exceptions.py
--rw-r--r--   0        0        0     1057 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/core/utils.py
--rw-r--r--   0        0        0      521 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/access_request.py
--rw-r--r--   0        0        0    15468 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/model.py
--rw-r--r--   0        0        0     7043 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/release.py
--rw-r--r--   0        0        0     2976 2024-04-24 14:35:49.087870 bailo-2.1.2/src/bailo/helper/schema.py
--rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 bailo-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2241 2024-05-08 10:58:38.690190 bailo-2.2.0/README.md
+-rw-r--r--   0        0        0     4889 2024-05-08 10:58:38.694190 bailo-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      636 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/core/__init__.py
+-rw-r--r--   0        0        0     3458 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/core/agent.py
+-rw-r--r--   0        0        0    19238 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/core/client.py
+-rw-r--r--   0        0        0      672 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/core/enums.py
+-rw-r--r--   0        0        0      221 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/core/exceptions.py
+-rw-r--r--   0        0        0     1072 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/core/utils.py
+-rw-r--r--   0        0        0      521 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/helper/__init__.py
+-rw-r--r--   0        0        0     3923 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/helper/access_request.py
+-rw-r--r--   0        0        0    15468 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/helper/model.py
+-rw-r--r--   0        0        0     9816 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/helper/release.py
+-rw-r--r--   0        0        0     2976 2024-05-08 10:58:38.694190 bailo-2.2.0/src/bailo/helper/schema.py
+-rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 bailo-2.2.0/PKG-INFO
```

### Comparing `bailo-2.1.2/README.md` & `bailo-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bailo-2.1.2/pyproject.toml` & `bailo-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.8.1"
 dynamic = ["version"]
 dependencies = [
     "semantic-version==2.10.0",
-    "requests>=2.22"
+    "requests>=2.22",
+    "tqdm>=4.66.2"
 ]
 
 [project.optional-dependencies]
 test = [
     "black==23.3.0",
     "check-manifest==0.49",
     "mlflow>2.11.0",
```

### Comparing `bailo-2.1.2/src/bailo/__init__.py` & `bailo-2.2.0/src/bailo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 Bailo Python Client
 ===================
 
 Bailo is a ecosystem for managing the lifecycle of managing machine learning models. This package provides support for interacting with models within Bailo.
 """
 from __future__ import annotations
 
-__version__ = "2.1.2"
+
+# Package Version
+__version__ = "2.2.0"
+
 
 from bailo.core.agent import Agent, PkiAgent, TokenAgent
 from bailo.core.client import Client
 from bailo.core.enums import EntryKind, ModelVisibility, Role, SchemaKind
 from bailo.helper.access_request import AccessRequest
 from bailo.helper.model import Experiment, Model
 from bailo.helper.release import Release
```

### Comparing `bailo-2.1.2/src/bailo/core/agent.py` & `bailo-2.2.0/src/bailo/core/agent.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.2/src/bailo/core/client.py` & `bailo-2.2.0/src/bailo/core/client.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.2/src/bailo/core/enums.py` & `bailo-2.2.0/src/bailo/core/enums.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.2/src/bailo/core/utils.py` & `bailo-2.2.0/src/bailo/core/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import annotations
 
+import os
 from typing import Any
 
+NO_COLOR = "NO_COLOR" in os.environ
+
 
 def filter_none(json: dict[str, Any]) -> dict[str, Any]:
     """Remove None attributes from a dictionary.
 
     :param json: Dictionary to filter
     :return: Dictionary with removed Nonetypes
     """
@@ -13,23 +16,23 @@
     return res
 
 
 class NestedDict(dict):
     def __getitem__(self, keytuple):
         # if key is not a tuple then access as normal
         if not isinstance(keytuple, tuple):
-            return super(NestedDict, self).__getitem__(keytuple)
+            return super().__getitem__(keytuple)
         d = self
         for key in keytuple:
             d = d[key]
         return d
 
     def __setitem__(self, keytuple, item):
         # if key is not a tuple then access as normal
         if not isinstance(keytuple, tuple):
-            return super(NestedDict, self).__setitem__(keytuple, item)
+            return super().__setitem__(keytuple, item)
         d = self
         for index, key in enumerate(keytuple):
             if index != len(keytuple) - 1:
                 d = d.setdefault(key, {})
             else:
                 d[key] = item
```

### Comparing `bailo-2.1.2/src/bailo/helper/__init__.py` & `bailo-2.2.0/src/bailo/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.2/src/bailo/helper/access_request.py` & `bailo-2.2.0/src/bailo/helper/access_request.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.2/src/bailo/helper/model.py` & `bailo-2.2.0/src/bailo/helper/model.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.2/src/bailo/helper/release.py` & `bailo-2.2.0/src/bailo/helper/release.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from __future__ import annotations
 
 import os
+import fnmatch
 import shutil
 from io import BytesIO
-from typing import Any
+from typing import Any, Union
+from tqdm import tqdm
+from tqdm.utils import CallbackIOWrapper
 
 from bailo.core.client import Client
+from bailo.core.exceptions import BailoException
+from bailo.core.utils import NO_COLOR
 from semantic_version import Version
 
+BLOCK_SIZE = 1024
+
 
 class Release:
     def __init__(
         self,
         client: Client,
         model_id: str,
         version: Version | str,
@@ -131,59 +138,123 @@
             files,
             images,
             minor,
             draft,
         )
 
     def download(self, filename: str, write: bool = True, path: str | None = None) -> Any:
-        """Give returns a Reading object given the file id.
+        """Returns a response object given the file name and optionally writes file to disk.
 
         :param filename: The name of the file to retrieve
         :param write: Bool to determine if writing file to disk, defaults to True
         :param path: Local path to write file to (if write set to True)
 
         :return: A JSON response object
         """
         res = self.client.get_download_by_filename(self.model_id, str(self.version), filename)
 
         if write:
             if path is None:
                 path = filename
-            with open(path, "wb") as f:
-                f.write(res.content)
+            total_size = int(res.headers.get("content-length", 0))
+
+            if NO_COLOR:
+                colour = "white"
+            else:
+                colour = "green"
+
+            with tqdm(
+                total=total_size,
+                unit="B",
+                unit_scale=True,
+                unit_divisor=BLOCK_SIZE,
+                postfix=f"downloading {filename} as {path}",
+                colour=colour,
+            ) as t:
+                with open(path, "wb") as f:
+                    for data in res.iter_content(BLOCK_SIZE):
+                        t.update(len(data))
+                        f.write(data)
 
         return res
 
+    def download_all(self, path: str = os.getcwd(), include: list | str = None, exclude: list | str = None):
+        """Writes all files to disk given a local directory.
+
+        :param include: List or string of fnmatch statements for file names to include, defaults to None
+        :param exclude: List or string of fnmatch statements for file names to exclude, defaults to None
+        :param path: Local directory to write files to
+        :raises BailoException: If the release has no files assigned to it
+        ..note:: Fnmatch statements support Unix shell-style wildcards.
+        """
+        files_metadata = self.client.get_release(self.model_id, str(self.version))["release"]["files"]
+        if files_metadata == []:
+            raise BailoException("Release has no associated files.")
+        file_names = [file_metadata["name"] for file_metadata in files_metadata]
+
+        if isinstance(include, str):
+            include = [include]
+        if isinstance(exclude, str):
+            exclude = [exclude]
+
+        if include is not None:
+            file_names = [file for file in file_names if any([fnmatch.fnmatch(file, pattern) for pattern in include])]
+
+        if exclude is not None:
+            file_names = [
+                file for file in file_names if not any([fnmatch.fnmatch(file, pattern) for pattern in exclude])
+            ]
+
+        os.makedirs(path, exist_ok=True)
+        for file in file_names:
+            file_path = os.path.join(path, file)
+            self.download(filename=file, path=file_path)
+
     def upload(self, path: str, data: BytesIO | None = None) -> str:
         """Upload a file to the release.
 
         :param path: The path, or name of file or directory to be uploaded
         :param data: A BytesIO object if not loading from disk
 
         :return: The unique file ID of the file uploaded
         ..note:: If path provided is a directory, it will be uploaded as a zip
         """
-        name = os.path.split(path)[1]
+        name = os.path.split(path)[-1]
 
         if data is None:
             if is_zip := os.path.isdir(path):
                 shutil.make_archive(name, "zip", path)
                 path = f"{name}.zip"
                 name = path
 
-            with open(path, "rb") as f:
-                res = self.client.simple_upload(self.model_id, name, f).json()
+            data = open(path, "rb")
 
             if is_zip:
                 os.remove(path)
+
+        old_file_position = data.tell()
+        data.seek(0, os.SEEK_END)
+        size = data.tell()
+        data.seek(old_file_position, os.SEEK_SET)
+
+        if NO_COLOR:
+            colour = "white"
         else:
-            res = self.client.simple_upload(self.model_id, name, data).json()
+            colour = "blue"
+
+        with tqdm(
+            total=size, unit="B", unit_scale=True, unit_divisor=BLOCK_SIZE, postfix=f"uploading {name}", colour=colour
+        ) as t:
+            wrapped_buffer = CallbackIOWrapper(t.update, data, "read")
+            res = self.client.simple_upload(self.model_id, name, wrapped_buffer).json()
 
         self.files.append(res["file"]["id"])
         self.update()
+        if not isinstance(data, BytesIO):
+            data.close()
         return res["file"]["id"]
 
     def update(self) -> Any:
         """Update the any changes to this release on Bailo.
 
         :return: JSON Response object
         """
```

### Comparing `bailo-2.1.2/src/bailo/helper/schema.py` & `bailo-2.2.0/src/bailo/helper/schema.py`

 * *Files identical despite different names*

### Comparing `bailo-2.1.2/PKG-INFO` & `bailo-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: bailo
-Version: 2.1.2
+Version: 2.2.0
 Summary: Simplifies interacting with Bailo
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: semantic-version==2.10.0
 Requires-Dist: requests>=2.22
+Requires-Dist: tqdm>=4.66.2
 Requires-Dist: black==23.3.0 ; extra == "test"
 Requires-Dist: check-manifest==0.49 ; extra == "test"
 Requires-Dist: mlflow>2.11.0 ; extra == "test"
 Requires-Dist: pre-commit==3.3.1 ; extra == "test"
 Requires-Dist: pylint==2.17.4 ; extra == "test"
 Requires-Dist: pylint_junit ; extra == "test"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: bailo Version: 2.1.2 Summary: Simplifies
+Metadata-Version: 2.1 Name: bailo Version: 2.2.0 Summary: Simplifies
 interacting with Bailo Requires-Python: >=3.8.1 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: semantic-version==2.10.0 Requires-Dist: requests>=2.22 Requires-
-Dist: black==23.3.0 ; extra == "test" Requires-Dist: check-manifest==0.49 ;
-extra == "test" Requires-Dist: mlflow>2.11.0 ; extra == "test" Requires-Dist:
-pre-commit==3.3.1 ; extra == "test" Requires-Dist: pylint==2.17.4 ; extra ==
-"test" Requires-Dist: pylint_junit ; extra == "test" Requires-Dist: pytest-
-cov==4.0.0 ; extra == "test" Requires-Dist: pytest-mock<3.10.1 ; extra ==
-"test" Requires-Dist: pytest-runner ; extra == "test" Requires-Dist:
-pytest==7.3.1 ; extra == "test" Requires-Dist: pytest-github-actions-annotate-
-failures ; extra == "test" Requires-Dist: requests_mock==1.11.0 ; extra ==
-"test" Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test" Project-URL:
-Documentation, https://github.com/gchq/bailo/tree/main#readme Project-URL:
-Source, https://github.com/gchq/bailo Project-URL: Tracker, https://github.com/
-gchq/bailo/issues Provides-Extra: test # Bailo Python Client A simple Python
-API Wrapper for Bailo
+Dist: tqdm>=4.66.2 Requires-Dist: black==23.3.0 ; extra == "test" Requires-
+Dist: check-manifest==0.49 ; extra == "test" Requires-Dist: mlflow>2.11.0 ;
+extra == "test" Requires-Dist: pre-commit==3.3.1 ; extra == "test" Requires-
+Dist: pylint==2.17.4 ; extra == "test" Requires-Dist: pylint_junit ; extra ==
+"test" Requires-Dist: pytest-cov==4.0.0 ; extra == "test" Requires-Dist:
+pytest-mock<3.10.1 ; extra == "test" Requires-Dist: pytest-runner ; extra ==
+"test" Requires-Dist: pytest==7.3.1 ; extra == "test" Requires-Dist: pytest-
+github-actions-annotate-failures ; extra == "test" Requires-Dist:
+requests_mock==1.11.0 ; extra == "test" Requires-Dist: shellcheck-py==0.9.0.2 ;
+extra == "test" Project-URL: Documentation, https://github.com/gchq/bailo/tree/
+main#readme Project-URL: Source, https://github.com/gchq/bailo Project-URL:
+Tracker, https://github.com/gchq/bailo/issues Provides-Extra: test # Bailo
+Python Client A simple Python API Wrapper for Bailo
 Table of Contents
    1. _K_e_y_ _F_e_a_t_u_r_e_s
    2. _I_n_s_t_a_l_l_i_n_g
    3. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
    4. _D_e_v_e_l_o_p_m_e_n_t
           o _P_r_e_c_o_m_m_i_t_s
           o _T_e_s_t_i_n_g
```


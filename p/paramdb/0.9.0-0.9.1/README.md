# Comparing `tmp/paramdb-0.9.0.tar.gz` & `tmp/paramdb-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paramdb-0.9.0.tar", max compression
+gzip compressed data, was "paramdb-0.9.1.tar", max compression
```

## Comparing `paramdb-0.9.0.tar` & `paramdb-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1521 2023-06-29 19:01:15.627857 paramdb-0.9.0/LICENSE
--rw-r--r--   0        0        0     1861 2023-06-29 19:01:15.627857 paramdb-0.9.0/README.md
--rw-r--r--   0        0        0      706 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/__init__.py
--rw-r--r--   0        0        0    10274 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_database.py
--rw-r--r--   0        0        0      571 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_keys.py
--rw-r--r--   0        0        0        0 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/__init__.py
--rw-r--r--   0        0        0     6622 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/_collections.py
--rw-r--r--   0        0        0     3498 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/_dataclasses.py
--rw-r--r--   0        0        0     4343 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/_param_data.py
--rw-r--r--   0        0        0     1177 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/_param_data/_type_mixins.py
--rw-r--r--   0        0        0        0 2023-06-29 19:01:15.627857 paramdb-0.9.0/paramdb/py.typed
--rw-r--r--   0        0        0     1213 2023-06-29 19:01:15.627857 paramdb-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 paramdb-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-08-09 18:25:10.364345 paramdb-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1861 2023-08-09 18:25:10.364345 paramdb-0.9.1/README.md
+-rw-r--r--   0        0        0      706 2023-08-09 18:25:10.364345 paramdb-0.9.1/paramdb/__init__.py
+-rw-r--r--   0        0        0    10274 2023-08-09 18:25:10.364345 paramdb-0.9.1/paramdb/_database.py
+-rw-r--r--   0        0        0      571 2023-08-09 18:25:10.364345 paramdb-0.9.1/paramdb/_keys.py
+-rw-r--r--   0        0        0        0 2023-08-09 18:25:10.364345 paramdb-0.9.1/paramdb/_param_data/__init__.py
+-rw-r--r--   0        0        0     6622 2023-08-09 18:25:10.364345 paramdb-0.9.1/paramdb/_param_data/_collections.py
+-rw-r--r--   0        0        0     3657 2023-08-09 18:25:10.364345 paramdb-0.9.1/paramdb/_param_data/_dataclasses.py
+-rw-r--r--   0        0        0     4369 2023-08-09 18:25:10.364345 paramdb-0.9.1/paramdb/_param_data/_param_data.py
+-rw-r--r--   0        0        0     1177 2023-08-09 18:25:10.364345 paramdb-0.9.1/paramdb/_param_data/_type_mixins.py
+-rw-r--r--   0        0        0        0 2023-08-09 18:25:10.364345 paramdb-0.9.1/paramdb/py.typed
+-rw-r--r--   0        0        0     1237 2023-08-09 18:25:10.364345 paramdb-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 paramdb-0.9.1/PKG-INFO
```

### Comparing `paramdb-0.9.0/LICENSE` & `paramdb-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paramdb-0.9.0/README.md` & `paramdb-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `paramdb-0.9.0/paramdb/__init__.py` & `paramdb-0.9.1/paramdb/__init__.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.9.0/paramdb/_database.py` & `paramdb-0.9.1/paramdb/_database.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.9.0/paramdb/_keys.py` & `paramdb-0.9.1/paramdb/_keys.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.9.0/paramdb/_param_data/_collections.py` & `paramdb-0.9.1/paramdb/_param_data/_collections.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.9.0/paramdb/_param_data/_dataclasses.py` & `paramdb-0.9.1/paramdb/_param_data/_dataclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,24 @@
 from typing_extensions import Self, dataclass_transform
 from paramdb._keys import LAST_UPDATED_KEY
 from paramdb._param_data._param_data import ParamData
 
 
 @dataclass_transform(kw_only_default=True)
 class _ParamDataclass(ParamData):
-    """Base class for parameter dataclasses."""
+    """
+    Base class for parameter dataclasses.
+
+    Any keyword arguments given when creating a subclass are passed to the dataclass
+    constructor.
+    """
 
     def __init_subclass__(cls, /, kw_only: bool = True, **kwargs: Any) -> None:
         # Convert subclasses into dataclasses
-        super().__init_subclass__()
+        super().__init_subclass__()  # kwargs are passed to dataclass constructor
         dataclass(kw_only=kw_only, **kwargs)(cls)
 
     def __getitem__(self, name: str) -> Any:
         # Enable getting attributes via indexing
         return getattr(self, name)
 
     def __setitem__(self, name: str, value: Any) -> None:
```

### Comparing `paramdb-0.9.0/paramdb/_param_data/_param_data.py` & `paramdb-0.9.1/paramdb/_param_data/_param_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 class ParamData(ABC):
     """Abstract base class for all parameter data."""
 
     # Most recently initialized structure that contains this parameter data
     _parent: ParamData | None = None
 
-    def __init_subclass__(cls) -> None:
+    def __init_subclass__(cls, /, **kwargs: Any) -> None:
         # Add subclass to dictionary of parameter data classes
+        super().__init_subclass__(**kwargs)
         _param_classes[cls.__name__] = cls
-        super().__init_subclass__()
 
     def _add_child(self, child: Any) -> None:
         """Add the given object as a child, if it is ``ParamData``."""
 
         if isinstance(child, ParamData):
             # Use ParamData __setattr__ to avoid updating _last_updated
             ParamData.__setattr__(child, "_parent", self)
```

### Comparing `paramdb-0.9.0/paramdb/_param_data/_type_mixins.py` & `paramdb-0.9.1/paramdb/_param_data/_type_mixins.py`

 * *Files identical despite different names*

### Comparing `paramdb-0.9.0/pyproject.toml` & `paramdb-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 [tool.poetry]
 name = "paramdb"
-version = "0.9.0"
+version = "0.9.1"
 description = "Python package for storing and retrieving experiment parameters."
 authors = ["Alex Hadley <alexhad6@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/PainterQubits/paramdb"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typing-extensions = "^4.7.0"
-sqlalchemy = "^2.0.17"
+typing-extensions = "^4.7.1"
+sqlalchemy = "^2.0.19"
 zstandard = "^0.21.0"
-astropy = {version = "^5.3", optional = true}
+astropy = {version = "^5.3.1", optional = true}
 
 [tool.poetry.extras]
 astropy = ["astropy"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
-flake8 = "^6.0.0"
-pylint = "^2.17.4"
+flake8 = "^6.1.0"
+pylint = "^2.17.5"
 mypy = "^1.4.1"
-black = "^23.3.0"
+black = "^23.7.0"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^7.0.1"
+sphinx = "^7.1.2"
 myst-parser = "^2.0.0"
-furo = "^2023.5.20"
+furo = "^2023.7.26"
 sphinx-copybutton = "^0.5.2"
 jupyter-sphinx = "^0.4.0"
+ipykernel = "^6.25.1"
 sphinx-autobuild = "^2021.3.14"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 
 [tool.pylint.basic]
 good-names-rgxs = ["^[a-z][a-z0-9]?$"]
```

### Comparing `paramdb-0.9.0/PKG-INFO` & `paramdb-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: paramdb
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python package for storing and retrieving experiment parameters.
 Home-page: https://github.com/PainterQubits/paramdb
 License: BSD-3-Clause
 Author: Alex Hadley
 Author-email: alexhad6@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: astropy
-Requires-Dist: astropy (>=5.3,<6.0) ; extra == "astropy"
-Requires-Dist: sqlalchemy (>=2.0.17,<3.0.0)
-Requires-Dist: typing-extensions (>=4.7.0,<5.0.0)
+Requires-Dist: astropy (>=5.3.1,<6.0.0) ; extra == "astropy"
+Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Requires-Dist: zstandard (>=0.21.0,<0.22.0)
 Project-URL: Repository, https://github.com/PainterQubits/paramdb
 Description-Content-Type: text/markdown
 
 # ParamDB
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/paramdb)](https://pypi.org/project/paramdb/)
```


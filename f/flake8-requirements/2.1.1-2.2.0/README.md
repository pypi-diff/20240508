# Comparing `tmp/flake8_requirements-2.1.1-py3-none-any.whl.zip` & `tmp/flake8_requirements-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 15585 bytes, number of entries: 9
--rw-r--r--  2.0 unx       71 b- defN 24-Mar-27 06:49 flake8_requirements/__init__.py
--rw-r--r--  2.0 unx    27214 b- defN 24-Mar-27 06:49 flake8_requirements/checker.py
--rw-r--r--  2.0 unx    11332 b- defN 24-Mar-27 06:49 flake8_requirements/modules.py
--rw-r--r--  2.0 unx     1111 b- defN 24-Mar-27 06:49 flake8_requirements-2.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6021 b- defN 24-Mar-27 06:49 flake8_requirements-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 06:49 flake8_requirements-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 24-Mar-27 06:49 flake8_requirements-2.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-Mar-27 06:49 flake8_requirements-2.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      819 b- defN 24-Mar-27 06:49 flake8_requirements-2.1.1.dist-info/RECORD
-9 files, 46739 bytes uncompressed, 14147 bytes compressed:  69.7%
+Zip file size: 15814 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       71 b- defN 24-May-08 11:57 flake8_requirements/__init__.py
+-rw-r--r--  2.0 unx    28425 b- defN 24-May-08 11:57 flake8_requirements/checker.py
+-rw-r--r--  2.0 unx    11332 b- defN 24-May-08 11:57 flake8_requirements/modules.py
+-rw-r--r--  2.0 unx     1111 b- defN 24-May-08 11:57 flake8_requirements-2.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6021 b- defN 24-May-08 11:57 flake8_requirements-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 11:57 flake8_requirements-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 24-May-08 11:57 flake8_requirements-2.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-08 11:57 flake8_requirements-2.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      819 b- defN 24-May-08 11:57 flake8_requirements-2.2.0.dist-info/RECORD
+9 files, 47950 bytes uncompressed, 14376 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: flake8_requirements/checker.py
 Comment: 
 
 Filename: flake8_requirements/modules.py
 Comment: 
 
-Filename: flake8_requirements-2.1.1.dist-info/LICENSE.txt
+Filename: flake8_requirements-2.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: flake8_requirements-2.1.1.dist-info/METADATA
+Filename: flake8_requirements-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: flake8_requirements-2.1.1.dist-info/WHEEL
+Filename: flake8_requirements-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: flake8_requirements-2.1.1.dist-info/entry_points.txt
+Filename: flake8_requirements-2.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: flake8_requirements-2.1.1.dist-info/top_level.txt
+Filename: flake8_requirements-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: flake8_requirements-2.1.1.dist-info/RECORD
+Filename: flake8_requirements-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flake8_requirements/checker.py

```diff
@@ -16,15 +16,15 @@
 else:
     import tomli as tomllib
 
 from .modules import KNOWN_3RD_PARTIES
 from .modules import STDLIB_PY3
 
 # NOTE: Changing this number will alter package version as well.
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 __license__ = "MIT"
 
 LOG = getLogger('flake8.plugin.requirements')
 
 ERRORS = {
     'I900': "I900 '{pkg}' not listed as a requirement",
     'I901': "I901 '{pkg}' required but not used",
@@ -557,22 +557,51 @@
     @classmethod
     def get_pyproject_toml_pep621(cls):
         """Try to get PEP 621 metadata."""
         cfg_pep518 = cls.get_pyproject_toml()
         return cfg_pep518.get('project', {})
 
     @classmethod
+    def get_setuptools_dynamic_requirements(cls):
+        """Retrieve dynamic requirements defined in setuptools config."""
+        cfg = cls.get_pyproject_toml()
+        dynamic_keys = cfg.get('project', {}).get('dynamic', [])
+        dynamic_config = (
+            cfg.get('tool', {}).get('setuptools', {}).get('dynamic', {})
+        )
+        requirements = []
+        files_to_parse = []
+        if 'dependencies' in dynamic_keys:
+            files_to_parse.extend(
+                dynamic_config.get('dependencies', {}).get('file', [])
+            )
+        if 'optional-dependencies' in dynamic_keys:
+            for element in dynamic_config.get(
+                'optional-dependencies', {}
+            ).values():
+                files_to_parse.extend(element.get('file', []))
+        for file_path in files_to_parse:
+            try:
+                with open(file_path, 'r') as file:
+                    requirements.extend(parse_requirements(file))
+            except IOError as e:
+                LOG.debug("Couldn't open requirements file: %s", e)
+        return requirements
+
+    @classmethod
     def get_pyproject_toml_pep621_requirements(cls):
         """Try to get PEP 621 metadata requirements."""
         pep621 = cls.get_pyproject_toml_pep621()
         requirements = []
         requirements.extend(parse_requirements(
             pep621.get("dependencies", ())))
         for r in pep621.get("optional-dependencies", {}).values():
             requirements.extend(parse_requirements(r))
+        if len(requirements) == 0:
+            requirements = cls.get_setuptools_dynamic_requirements()
         return requirements
 
     @classmethod
     def get_pyproject_toml_poetry(cls):
         """Try to get poetry configuration."""
         cfg_pep518 = cls.get_pyproject_toml()
         return cfg_pep518.get('tool', {}).get('poetry', {})
```

## Comparing `flake8_requirements-2.1.1.dist-info/LICENSE.txt` & `flake8_requirements-2.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `flake8_requirements-2.1.1.dist-info/METADATA` & `flake8_requirements-2.2.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-requirements
-Version: 2.1.1
+Version: 2.2.0
 Summary: Package requirements checker, plugin for flake8
 Home-page: https://github.com/Arkq/flake8-requirements
 Author: Arkadiusz Bokowy
 Author-email: arkadiusz.bokowy@gmail.com
 License: MIT
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
```


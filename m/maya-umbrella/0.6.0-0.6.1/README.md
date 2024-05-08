# Comparing `tmp/maya_umbrella-0.6.0.tar.gz` & `tmp/maya_umbrella-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maya_umbrella-0.6.0.tar", max compression
+gzip compressed data, was "maya_umbrella-0.6.1.tar", max compression
```

## Comparing `maya_umbrella-0.6.0.tar` & `maya_umbrella-0.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1060 2024-05-08 16:17:57.631673 maya_umbrella-0.6.0/LICENSE
--rw-r--r--   0        0        0     8127 2024-05-08 16:17:57.631673 maya_umbrella-0.6.0/README.md
--rw-r--r--   0        0        0      401 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/__init__.py
--rw-r--r--   0        0        0       22 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/__version__.py
--rw-r--r--   0        0        0     5044 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/cleaner.py
--rw-r--r--   0        0        0    13111 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/collector.py
--rw-r--r--   0        0        0      539 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/constants.py
--rw-r--r--   0        0        0     5601 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/defender.py
--rw-r--r--   0        0        0     8333 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/filesystem.py
--rw-r--r--   0        0        0        0 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/__init__.py
--rw-r--r--   0        0        0      761 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/delete_turtle.py
--rw-r--r--   0        0        0     1281 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/delete_unknown_plugin_node.py
--rw-r--r--   0        0        0      556 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/fix_model_panel.py
--rw-r--r--   0        0        0      484 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/hooks/fix_on_model_change_3dc.py
--rw-r--r--   0        0        0     2683 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/i18n.py
--rw-r--r--   0        0        0      962 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/locales/en_US.json
--rw-r--r--   0        0        0     1006 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/locales/zh_CN.json
--rw-r--r--   0        0        0     1338 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/log.py
--rw-r--r--   0        0        0     3394 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/maya_funs.py
--rw-r--r--   0        0        0     3710 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/scanner.py
--rw-r--r--   0        0        0      354 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/signatures.py
--rw-r--r--   0        0        0     1022 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccine.py
--rw-r--r--   0        0        0        0 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccines/__init__.py
--rw-r--r--   0        0        0      489 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccines/vaccine1.py
--rw-r--r--   0        0        0     2123 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccines/vaccine2.py
--rw-r--r--   0        0        0     3493 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/maya_umbrella/vaccines/vaccine3.py
--rw-r--r--   0        0        0     5284 2024-05-08 16:17:57.655673 maya_umbrella-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     9178 1970-01-01 00:00:00.000000 maya_umbrella-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-08 16:49:34.049419 maya_umbrella-0.6.1/LICENSE
+-rw-r--r--   0        0        0     8127 2024-05-08 16:49:34.049419 maya_umbrella-0.6.1/README.md
+-rw-r--r--   0        0        0      401 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/__version__.py
+-rw-r--r--   0        0        0     5044 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/cleaner.py
+-rw-r--r--   0        0        0    13111 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/collector.py
+-rw-r--r--   0        0        0      539 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/constants.py
+-rw-r--r--   0        0        0     5601 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/defender.py
+-rw-r--r--   0        0        0     8333 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/filesystem.py
+-rw-r--r--   0        0        0        0 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/hooks/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/hooks/delete_turtle.py
+-rw-r--r--   0        0        0     1281 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/hooks/delete_unknown_plugin_node.py
+-rw-r--r--   0        0        0      556 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/hooks/fix_model_panel.py
+-rw-r--r--   0        0        0      484 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/hooks/fix_on_model_change_3dc.py
+-rw-r--r--   0        0        0     2683 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/i18n.py
+-rw-r--r--   0        0        0      962 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/locales/en_US.json
+-rw-r--r--   0        0        0     1006 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/locales/zh_CN.json
+-rw-r--r--   0        0        0     1338 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/log.py
+-rw-r--r--   0        0        0     3394 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/maya_funs.py
+-rw-r--r--   0        0        0     3970 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/scanner.py
+-rw-r--r--   0        0        0      354 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/signatures.py
+-rw-r--r--   0        0        0     1022 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/vaccine.py
+-rw-r--r--   0        0        0        0 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/vaccines/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/vaccines/vaccine1.py
+-rw-r--r--   0        0        0     2123 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/vaccines/vaccine2.py
+-rw-r--r--   0        0        0     3493 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/maya_umbrella/vaccines/vaccine3.py
+-rw-r--r--   0        0        0     5284 2024-05-08 16:49:34.073419 maya_umbrella-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     9178 1970-01-01 00:00:00.000000 maya_umbrella-0.6.1/PKG-INFO
```

### Comparing `maya_umbrella-0.6.0/LICENSE` & `maya_umbrella-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/README.md` & `maya_umbrella-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/cleaner.py` & `maya_umbrella-0.6.1/maya_umbrella/cleaner.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/collector.py` & `maya_umbrella-0.6.1/maya_umbrella/collector.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/constants.py` & `maya_umbrella-0.6.1/maya_umbrella/constants.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/defender.py` & `maya_umbrella-0.6.1/maya_umbrella/defender.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/filesystem.py` & `maya_umbrella-0.6.1/maya_umbrella/filesystem.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/hooks/delete_turtle.py` & `maya_umbrella-0.6.1/maya_umbrella/hooks/delete_turtle.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/hooks/delete_unknown_plugin_node.py` & `maya_umbrella-0.6.1/maya_umbrella/hooks/delete_unknown_plugin_node.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/hooks/fix_model_panel.py` & `maya_umbrella-0.6.1/maya_umbrella/hooks/fix_model_panel.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/i18n.py` & `maya_umbrella-0.6.1/maya_umbrella/i18n.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/locales/en_US.json` & `maya_umbrella-0.6.1/maya_umbrella/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/locales/zh_CN.json` & `maya_umbrella-0.6.1/maya_umbrella/locales/zh_CN.json`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/log.py` & `maya_umbrella-0.6.1/maya_umbrella/log.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/maya_funs.py` & `maya_umbrella-0.6.1/maya_umbrella/maya_funs.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/scanner.py` & `maya_umbrella-0.6.1/maya_umbrella/scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             env (dict, optional): Custom environment variables. Defaults to None,
             which sets the 'MAYA_COLOR_MANAGEMENT_SYNCOLOR' variable to '1'.
         """
         self.logger = logging.getLogger(__name__)
         self.defender = None
         self.output_path = output_path
         self._failed_files = []
+        self._reference_files = []
         self._fixed_files = []
         # Custom env.
         self._env = env or {
             "MAYA_COLOR_MANAGEMENT_SYNCOLOR": "1"
         }
 
     def scan_files_from_pattern(self, pattern):
@@ -59,14 +60,17 @@
         Args:
             files (list): List of file paths to scan and fix.
         """
         with context_defender() as defender:
             self.defender = defender
             for maya_file in files:
                 self._fix(maya_file)
+            while len(self._reference_files) > 0:
+                for ref in self._reference_files:
+                    self._fix(ref)
         return self._fixed_files
 
     def scan_files_from_file(self, text_file):
         """Scan and fix Maya files from a given text file containing a list of file paths.
 
         Args:
             text_file (str): Path to the text file containing the list of file paths.
@@ -92,10 +96,11 @@
         if self.defender.have_issues:
             self.defender.fix()
             backup_path = get_backup_path(maya_file, root_path=self.output_path)
             self.logger.debug("Backup saved to: {backup_path}".format(backup_path=backup_path))
             shutil.copy2(maya_file, backup_path)
             cmds.file(s=True, f=True)
             self._fixed_files.append(maya_file)
-            cmds.file(new=True, force=True)
-        for ref in self.defender.collector.infected_reference_files:
-            self._fix(ref)
+            self._reference_files.extend(self.defender.collector.infected_reference_files)
+        if maya_file in self._reference_files:
+            self._reference_files.remove(maya_file)
+        cmds.file(new=True, force=True)
```

### Comparing `maya_umbrella-0.6.0/maya_umbrella/vaccine.py` & `maya_umbrella-0.6.1/maya_umbrella/vaccine.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/vaccines/vaccine2.py` & `maya_umbrella-0.6.1/maya_umbrella/vaccines/vaccine2.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/maya_umbrella/vaccines/vaccine3.py` & `maya_umbrella-0.6.1/maya_umbrella/vaccines/vaccine3.py`

 * *Files identical despite different names*

### Comparing `maya_umbrella-0.6.0/pyproject.toml` & `maya_umbrella-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maya_umbrella"
-version = "0.6.0"
+version = "0.6.1"
 description = "Check and fix maya virus."
 homepage = "https://github.com/loonghao/maya_umbrella"
 repository = "https://github.com/loonghao/maya_umbrella"
 documentation = "https://github.com/loonghao/maya_umbrella"
 keywords = ["notifiers", "python", "Maya", "dcc"]
 authors = ["longhao <hal.long@outlook.com>"]
 license = "MIT"
@@ -32,15 +32,15 @@
 python = ">=2.7,<2.8 || >=3.6.0"
 
 [tool.poetry.dev-dependencies]
 nox = { version = "^2024.3.2", python = ">=3.8.1,<3.11" }
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.0"
+version = "0.6.1"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "maya_umbrella/__version__.py"
 ]
 
 [build-system]
```

### Comparing `maya_umbrella-0.6.0/PKG-INFO` & `maya_umbrella-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya_umbrella
-Version: 0.6.0
+Version: 0.6.1
 Summary: Check and fix maya virus.
 Home-page: https://github.com/loonghao/maya_umbrella
 License: MIT
 Keywords: notifiers,python,Maya,dcc
 Author: longhao
 Author-email: hal.long@outlook.com
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
```


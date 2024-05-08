# Comparing `tmp/ascender-0.1.9.tar.gz` & `tmp/ascender-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascender-0.1.9.tar", max compression
+gzip compressed data, was "ascender-0.2.0.tar", max compression
```

## Comparing `ascender-0.1.9.tar` & `ascender-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35148 2023-12-19 19:36:15.353783 ascender-0.1.9/LICENSE
--rw-r--r--   0        0        0      953 2023-12-19 20:05:30.701956 ascender-0.1.9/README.md
--rw-r--r--   0        0        0      146 2024-04-28 15:55:58.332495 ascender-0.1.9/ascender/app.py
--rw-r--r--   0        0        0     3239 2024-04-28 15:02:31.682934 ascender-0.1.9/ascender/commands/projects.py
--rw-r--r--   0        0        0     1840 2023-12-19 21:08:03.713265 ascender-0.1.9/ascender/commands/runner.py
--rw-r--r--   0        0        0      132 2023-12-19 20:00:44.526193 ascender-0.1.9/ascender/launch.py
--rw-r--r--   0        0        0     7730 2024-04-29 17:15:34.992137 ascender-0.1.9/ascender/logic/projects.py
--rw-r--r--   0        0        0     2573 2024-04-29 17:17:21.628820 ascender-0.1.9/ascender/logic/runner.py
--rw-r--r--   0        0        0     2630 2024-04-29 17:08:02.073555 ascender-0.1.9/ascender/logic/versions.py
--rw-r--r--   0        0        0      179 2024-01-04 18:50:06.046792 ascender-0.1.9/ascender/settings.py
--rw-r--r--   0        0        0      655 2024-04-29 17:17:30.025286 ascender-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ascender-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-12-19 19:36:15.353783 ascender-0.2.0/LICENSE
+-rw-r--r--   0        0        0      953 2023-12-19 20:05:30.701956 ascender-0.2.0/README.md
+-rw-r--r--   0        0        0      146 2024-04-28 15:55:58.332495 ascender-0.2.0/ascender/app.py
+-rw-r--r--   0        0        0     3239 2024-04-28 15:02:31.682934 ascender-0.2.0/ascender/commands/projects.py
+-rw-r--r--   0        0        0     1840 2023-12-19 21:08:03.713265 ascender-0.2.0/ascender/commands/runner.py
+-rw-r--r--   0        0        0      132 2023-12-19 20:00:44.526193 ascender-0.2.0/ascender/launch.py
+-rw-r--r--   0        0        0     7792 2024-05-08 11:32:58.790380 ascender-0.2.0/ascender/logic/projects.py
+-rw-r--r--   0        0        0     2573 2024-04-29 17:17:21.628820 ascender-0.2.0/ascender/logic/runner.py
+-rw-r--r--   0        0        0     2630 2024-04-29 17:08:02.073555 ascender-0.2.0/ascender/logic/versions.py
+-rw-r--r--   0        0        0      179 2024-01-04 18:50:06.046792 ascender-0.2.0/ascender/settings.py
+-rw-r--r--   0        0        0      655 2024-05-08 11:33:16.596318 ascender-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 ascender-0.2.0/PKG-INFO
```

### Comparing `ascender-0.1.9/LICENSE` & `ascender-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ascender-0.1.9/README.md` & `ascender-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ascender-0.1.9/ascender/commands/projects.py` & `ascender-0.2.0/ascender/commands/projects.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.9/ascender/commands/runner.py` & `ascender-0.2.0/ascender/commands/runner.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.9/ascender/logic/projects.py` & `ascender-0.2.0/ascender/logic/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         shutil.copyfile(f"{self.base_path}/.asc_temp/pyproject.toml", f"{self.base_path}/pyproject.toml")
 
         # Apply last custom updates set in update.txt
         update_dir = f"{self.base_path}/core/update.txt"
         if os.path.exists(update_dir):
             with open(update_dir, "r") as u:
                 _update_contents = u.read()
-                _update_contents = _update_contents.replace("[BASE_PATH]", self.base_path)
+                _update_contents = _update_contents.replace("[BASE_PATH]", self.base_path).replace("[INSTALLATION_PATH]", f"{self.base_path}/.asc_temp")
                 print(_update_contents)
                 exec(_update_contents)
             os.remove(update_dir)
         
         # Delete .asc_temp directory
         shutil.rmtree(f"{self.base_path}/.asc_temp")
```

### Comparing `ascender-0.1.9/ascender/logic/runner.py` & `ascender-0.2.0/ascender/logic/runner.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.9/ascender/logic/versions.py` & `ascender-0.2.0/ascender/logic/versions.py`

 * *Files identical despite different names*

### Comparing `ascender-0.1.9/pyproject.toml` & `ascender-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ascender"
-version = "0.1.9"
+version = "0.2.0"
 description = "The CLI tool for working with AscenderFramework: Installation, command execution and version management"
 authors = ["AscenderTeam"]
 repository = "https://github.com/AscenderTeam/AscenderCLI"
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `ascender-0.1.9/PKG-INFO` & `ascender-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascender
-Version: 0.1.9
+Version: 0.2.0
 Summary: The CLI tool for working with AscenderFramework: Installation, command execution and version management
 Home-page: https://github.com/AscenderTeam/AscenderCLI
 License: GPL-3.0
 Author: AscenderTeam
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```


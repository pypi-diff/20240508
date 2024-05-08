# Comparing `tmp/confhub-0.0.2a0.tar.gz` & `tmp/confhub-0.0.3a0.tar.gz`

## Comparing `confhub-0.0.2a0.tar` & `confhub-0.0.3a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 confhub-0.0.2a0/CHANGELOG.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 confhub-0.0.2a0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/__meta__.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/commands.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/enums.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/exceptions.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/models.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/reader.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/setup_logger.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 confhub-0.0.2a0/confhub/templates.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 confhub-0.0.2a0/tests/.secrets.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 confhub-0.0.2a0/tests/example__secrets.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 confhub-0.0.2a0/tests/settings.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 confhub-0.0.2a0/tests/test_confhub.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 confhub-0.0.2a0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 confhub-0.0.2a0/LICENSE
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 confhub-0.0.2a0/README.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 confhub-0.0.2a0/pyproject.toml
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 confhub-0.0.2a0/PKG-INFO
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

### Comparing `confhub-0.0.2a0/confhub/__main__.py` & `confhub-0.0.3a0/confhub/__main__.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.2a0/confhub/commands.py` & `confhub-0.0.3a0/confhub/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,23 +32,23 @@
         logger.info('Loading configuration files', secret_file=secret_file, secret_file__example=secret_file__example, settings=settings_file)
 
     current_dir = Path(os.getcwd())
     folder_path = current_dir / Path(folder)
     logger.debug('`create` function called', folder=folder_path, current_dir=current_dir)
 
     if not folder_path.exists():
-        folder_path.mkdir(parents=True, exist_ok=True)
         _q = True
         while _q:
             confirmation_creation_folder = input(f'\nDo you want to create a new folder at ({folder_path})? [Y/n]\n: ')
             if not confirmation_creation_folder:
                 confirmation_creation_folder = 'y'
 
             if confirmation_creation_folder.lower() in ['y', 'yes', 'д', 'да']:
                 _q = False
+                folder_path.mkdir(parents=True, exist_ok=True)
                 generate_configurations_files(select_folder=folder_path)
             elif confirmation_creation_folder.lower() in ['n', 'no', 'н', 'нет']:
                 _q = False
                 logger.info('Generation canceled')
     else:
         generate_configurations_files(select_folder=folder_path)
         logger.debug('Folder exists')
```

### Comparing `confhub-0.0.2a0/confhub/enums.py` & `confhub-0.0.3a0/confhub/enums.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.2a0/confhub/exceptions.py` & `confhub-0.0.3a0/confhub/exceptions.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.2a0/confhub/models.py` & `confhub-0.0.3a0/confhub/models.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.2a0/confhub/reader.py` & `confhub-0.0.3a0/confhub/reader.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.2a0/confhub/setup_logger.py` & `confhub-0.0.3a0/confhub/setup_logger.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.2a0/confhub/templates.py` & `confhub-0.0.3a0/confhub/templates.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.2a0/tests/test_confhub.py` & `confhub-0.0.3a0/tests/test_confhub.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.2a0/.gitignore` & `confhub-0.0.3a0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
+
+.pypirc
```

### Comparing `confhub-0.0.2a0/LICENSE` & `confhub-0.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `confhub-0.0.2a0/pyproject.toml` & `confhub-0.0.3a0/pyproject.toml`

 * *Files identical despite different names*


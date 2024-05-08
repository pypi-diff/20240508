# Comparing `tmp/pypa_make_easy-0.2.tar.gz` & `tmp/pypa_make_easy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypa_make_easy-0.2.tar", last modified: Sun May  5 16:14:28 2024, max compression
+gzip compressed data, was "pypa_make_easy-0.3.tar", last modified: Wed May  8 09:41:04 2024, max compression
```

## Comparing `pypa_make_easy-0.2.tar` & `pypa_make_easy-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-05 16:14:28.215109 pypa_make_easy-0.2/
--rw-r--r--   0 alex      (1000) alex      (1000)    11325 2024-05-05 16:09:42.000000 pypa_make_easy-0.2/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     2133 2024-05-05 16:14:28.215109 pypa_make_easy-0.2/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     1669 2024-05-05 16:09:42.000000 pypa_make_easy-0.2/README.rst
--rwxr-xr-x   0 alex      (1000) alex      (1000)    15873 2024-05-05 16:09:42.000000 pypa_make_easy-0.2/pypa
--rwxr-xr-x   0 alex      (1000) alex      (1000)    15873 2024-05-05 16:09:42.000000 pypa_make_easy-0.2/pypa-make-easy
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-05 16:14:28.215109 pypa_make_easy-0.2/pypa_make_easy.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     2133 2024-05-05 16:14:28.000000 pypa_make_easy-0.2/pypa_make_easy.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      236 2024-05-05 16:14:28.000000 pypa_make_easy-0.2/pypa_make_easy.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-05-05 16:14:28.000000 pypa_make_easy-0.2/pypa_make_easy.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       12 2024-05-05 16:14:28.000000 pypa_make_easy-0.2/pypa_make_easy.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-05-05 16:14:28.000000 pypa_make_easy-0.2/pypa_make_easy.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2024-05-05 16:14:28.215109 pypa_make_easy-0.2/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)      673 2024-05-05 16:09:42.000000 pypa_make_easy-0.2/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 09:41:04.126583 pypa_make_easy-0.3/
+-rw-r--r--   0 alex      (1000) alex      (1000)    11325 2024-05-08 09:31:01.000000 pypa_make_easy-0.3/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     2383 2024-05-08 09:41:04.126583 pypa_make_easy-0.3/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     1919 2024-05-08 09:31:01.000000 pypa_make_easy-0.3/README.rst
+-rwxr-xr-x   0 alex      (1000) alex      (1000)    17443 2024-05-08 09:31:01.000000 pypa_make_easy-0.3/pypa
+-rwxr-xr-x   0 alex      (1000) alex      (1000)    17443 2024-05-08 09:31:01.000000 pypa_make_easy-0.3/pypa-make-easy
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-08 09:41:04.126583 pypa_make_easy-0.3/pypa_make_easy.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2383 2024-05-08 09:41:04.000000 pypa_make_easy-0.3/pypa_make_easy.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      236 2024-05-08 09:41:04.000000 pypa_make_easy-0.3/pypa_make_easy.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-05-08 09:41:04.000000 pypa_make_easy-0.3/pypa_make_easy.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       12 2024-05-08 09:41:04.000000 pypa_make_easy-0.3/pypa_make_easy.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-05-08 09:41:04.000000 pypa_make_easy-0.3/pypa_make_easy.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2024-05-08 09:41:04.126583 pypa_make_easy-0.3/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)      673 2024-05-08 09:40:58.000000 pypa_make_easy-0.3/setup.py
```

### Comparing `pypa_make_easy-0.2/LICENSE` & `pypa_make_easy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypa_make_easy-0.2/PKG-INFO` & `pypa_make_easy-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypa-make-easy
-Version: 0.2
+Version: 0.3
 Summary: Script to Create PyPi projects, but in easy
 Home-page: https://github.com/DevMasterLinux/pypa-make-easy
 Author: Kevin Alexander Krefting
 Author-email: kakrefting@gmail.com
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -77,7 +77,24 @@
 
 Install
 -------
 
 .. code-block:: bash
 
     python3 -m pip install pypa-make-easy
+
+Docker
+======
+
+You can with Docker Create your own PyPi packages Safe
+
+Build on Device
+
+.. code-block:: bash
+
+   ./scripts/run-docker.sh
+
+Download
+
+.. code-block:: bash
+
+   docker pull ghcr.io/devmasterlinux/pypa-make-easy/pypa-make-easy:1714930262
```

### Comparing `pypa_make_easy-0.2/README.rst` & `pypa_make_easy-0.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -63,7 +63,24 @@
 
 Install
 -------
 
 .. code-block:: bash
 
     python3 -m pip install pypa-make-easy
+
+Docker
+======
+
+You can with Docker Create your own PyPi packages Safe
+
+Build on Device
+
+.. code-block:: bash
+
+   ./scripts/run-docker.sh
+
+Download
+
+.. code-block:: bash
+
+   docker pull ghcr.io/devmasterlinux/pypa-make-easy/pypa-make-easy:1714930262
```

### Comparing `pypa_make_easy-0.2/pypa` & `pypa_make_easy-0.3/pypa`

 * *Files 18% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         
         if 'Moduls' in data:
             moduls = data['Moduls']
             for modul_key, modul_data in moduls.items():
                 modul_name = modul_data.get('name')
                 modul_type = modul_data['source']['Type']
                 if not modul_type:
-                    Create.Modul(projectname, modul_name)
+                    Create.Modul(Create, projectname, modul_name)
                 else:
                     modul_path = modul_data['source']['Path']
                     src_path = f"{PYPA_PATH}/{projectname}/src/{projectname}"
                     modul_file = f"{src_path}/{modul_name}"
                     shutil.copy(modul_path, modul_file)
         else:
             echo("Moduls not Found, Read Failed, YAML invalid")
@@ -295,15 +295,15 @@
             submoduls = data['SubModuls']
             for submodul_key, submodul_data in submoduls.items():
                 submodul_name = submodul_data.get('name')
                 submodul_type = submodul_data['source']['Type']
                 submodul_files = submodul_data['source']['Files']
                 if not submodul_type:
                     for file in submodul_files:
-                        Create.Submodul(projectname, submodul_name, file)
+                        Create.Submodul(Create, projectname, submodul_name, file)
                 else:
                     base_path = submodul_data['source']['Path']
                     src_path = f"{PYPA_PATH}/{projectname}/src/{projectname}"
                     for file in submodul_files:
                         file_path = f"{base_path}/{file}"
                         target_path = f"{src_path}/{submodul_name}/{file}"
                         shutil.copy(file_path, target_path)
@@ -311,28 +311,28 @@
             echo("Submoduls not Found, but is not Important, SKIP")
 
         if 'Readme' in data:
             readme = data['Readme']
             readme_status = readme.get('Exist')
             readme_path = readme.get('Path')
             if not readme_status:
-                Init.Readme(projectname)
+                Init.Readme(Init, projectname)
             else:
                 project_path = f"{PYPA_PATH}/{projectname}"
                 readme_project = f"{project_path}/README.rst"
                 shutil.copy(readme_path, readme_project)
         else:
             echo("Readme not Found, but is not Important, SKIP")
 
         if 'Setup' in data:
             setup = data['Setup']
             setup_status = setup.get('Exist')
             setup_path = setup.get('Path')
             if not setup_status:
-                Init.Setup(projectname)
+                Init.Setup(Init, projectname)
             else:
                 project_path = f"{PYPA_PATH}/{projectname}"
                 setup_project = f"{project_path}/setup.py"
                 shutil.copy(setup_path, setup_project)
         else:
             echo("Setup not Found, but is not Important, SKIP")
 
@@ -340,71 +340,71 @@
     if len(sys.argv) < 2:
         show_help("error")
         sys.exit(1)
 
     CMD = sys.argv[1]
     if CMD in ["--create", "create", "-c"]:
         if len(sys.argv) < 3:
-            show_help("error")
+            show_help("create")
             sys.exit(1)
 
         OPTION = sys.argv[2]
         if OPTION in ["--project", "project", "-p"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("create")
                 sys.exit(1)
             Create.Project(Create, sys.argv[3])
         elif OPTION in ["--modul", "modul", "-m"]:
             if len(sys.argv) < 5:
-                show_help("error")
+                show_help("create")
                 sys.exit(1)
             Create.Modul(Create, sys.argv[3], sys.argv[4])
         elif OPTION in ["--submodul", "submodul", "-sm"]:
             if len(sys.argv) < 6:
-                show_help("error")
+                show_help("create")
                 sys.exit(1)
             Create.Submodul(Create, sys.argv[3], sys.argv[4], sys.argv[5:-1])
         elif OPTION in ["--script", "script", "-sc"]:
             if len(sys.argv) < 6:
-                show_help("error")
+                show_help("create")
                 sys.exit(1)
             Create.Script(Create, sys.argv[3], sys.argv[4], sys.argv[5])
         elif OPTION in ["--help", "help", "-h"]:
             show_help("create")
         else:
             show_help("create")
     elif CMD in ["--init", "init", "-i"]:
         if len(sys.argv) < 3:
-            show_help("error")
+            show_help("init")
             sys.exit(1)
 
         OPTION = sys.argv[2]
         if OPTION in ["--modul", "modul", "-m"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             Init.Modul(Init, sys.argv[3])
         elif OPTION in ["--submodul", "submodul", "-sm"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             Init.Submodul(Init, sys.argv[3])
         elif OPTION in ["--readme", "readme", "-r"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             Init.Readme(Init, sys.argv[3])
         elif OPTION in ["--setup", "setup", "-s"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             Init.Setup(Init, sys.argv[3])
         elif OPTION in ["--full", "full", "-f"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             NAME = sys.argv[3]
             Init.Modul(Init, NAME)
             Init.Submodul(Init, NAME)
             Init.Readme(Init, NAME)
             Init.Setup(Init, NAME)
         elif OPTION in ["--help", "help", "-h"]:
@@ -427,9 +427,58 @@
         if OPTION in ["--help", "help", "-h"]:
             show_help("yaml")
         else:
             FILE = OPTION
             Yaml.read(Yaml, FILE)
     elif CMD in ["--help", "help", "-h"]:
         show_help("help")
+    elif CMD in ["-cp"]:
+        if len(sys.argv) < 3:
+            show_help("create")
+            sys.exit(1)
+        Create.Project(Create, sys.argv[2])
+    elif CMD in ["-cm"]:
+        if len(sys.argv) < 4:
+            show_help("create")
+            sys.exit(1)
+        Create.Modul(Create, sys.argv[2], sys.argv[3])
+    elif CMD in ["-csm"]:
+        if len(sys.argv) < 5:
+            show_help("error")
+            sys.exit(1)
+        Create.Submodul(Create, sys.argv[2], sys.argv[3], sys.argv[4:-1])
+    elif CMD in ["-csc"]:
+        if len(sys.argv) < 5:
+            show_help("error")
+            sys.exit(1)
+        Create.Script(Create, sys.argv[2], sys.argv[3], sys.argv[4])
+    elif CMD in ["-im"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        Init.Modul(Init, sys.argv[2])
+    elif CMD in ["-ism"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        Init.Submodul(Init, sys.argv[2])
+    elif CMD in ["-ir"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        Init.Readme(Init, sys.argv[2])
+    elif CMD in ["-is"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        Init.Setup(Init, sys.argv[2])
+    elif CMD in ["-if"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        NAME = sys.argv[2]
+        Init.Modul(Init, NAME)
+        Init.Submodul(Init, NAME)
+        Init.Readme(Init, NAME)
+        Init.Setup(Init, NAME)
     else:
         show_help("error")
```

### Comparing `pypa_make_easy-0.2/pypa-make-easy` & `pypa_make_easy-0.3/pypa-make-easy`

 * *Files 18% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         
         if 'Moduls' in data:
             moduls = data['Moduls']
             for modul_key, modul_data in moduls.items():
                 modul_name = modul_data.get('name')
                 modul_type = modul_data['source']['Type']
                 if not modul_type:
-                    Create.Modul(projectname, modul_name)
+                    Create.Modul(Create, projectname, modul_name)
                 else:
                     modul_path = modul_data['source']['Path']
                     src_path = f"{PYPA_PATH}/{projectname}/src/{projectname}"
                     modul_file = f"{src_path}/{modul_name}"
                     shutil.copy(modul_path, modul_file)
         else:
             echo("Moduls not Found, Read Failed, YAML invalid")
@@ -295,15 +295,15 @@
             submoduls = data['SubModuls']
             for submodul_key, submodul_data in submoduls.items():
                 submodul_name = submodul_data.get('name')
                 submodul_type = submodul_data['source']['Type']
                 submodul_files = submodul_data['source']['Files']
                 if not submodul_type:
                     for file in submodul_files:
-                        Create.Submodul(projectname, submodul_name, file)
+                        Create.Submodul(Create, projectname, submodul_name, file)
                 else:
                     base_path = submodul_data['source']['Path']
                     src_path = f"{PYPA_PATH}/{projectname}/src/{projectname}"
                     for file in submodul_files:
                         file_path = f"{base_path}/{file}"
                         target_path = f"{src_path}/{submodul_name}/{file}"
                         shutil.copy(file_path, target_path)
@@ -311,28 +311,28 @@
             echo("Submoduls not Found, but is not Important, SKIP")
 
         if 'Readme' in data:
             readme = data['Readme']
             readme_status = readme.get('Exist')
             readme_path = readme.get('Path')
             if not readme_status:
-                Init.Readme(projectname)
+                Init.Readme(Init, projectname)
             else:
                 project_path = f"{PYPA_PATH}/{projectname}"
                 readme_project = f"{project_path}/README.rst"
                 shutil.copy(readme_path, readme_project)
         else:
             echo("Readme not Found, but is not Important, SKIP")
 
         if 'Setup' in data:
             setup = data['Setup']
             setup_status = setup.get('Exist')
             setup_path = setup.get('Path')
             if not setup_status:
-                Init.Setup(projectname)
+                Init.Setup(Init, projectname)
             else:
                 project_path = f"{PYPA_PATH}/{projectname}"
                 setup_project = f"{project_path}/setup.py"
                 shutil.copy(setup_path, setup_project)
         else:
             echo("Setup not Found, but is not Important, SKIP")
 
@@ -340,71 +340,71 @@
     if len(sys.argv) < 2:
         show_help("error")
         sys.exit(1)
 
     CMD = sys.argv[1]
     if CMD in ["--create", "create", "-c"]:
         if len(sys.argv) < 3:
-            show_help("error")
+            show_help("create")
             sys.exit(1)
 
         OPTION = sys.argv[2]
         if OPTION in ["--project", "project", "-p"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("create")
                 sys.exit(1)
             Create.Project(Create, sys.argv[3])
         elif OPTION in ["--modul", "modul", "-m"]:
             if len(sys.argv) < 5:
-                show_help("error")
+                show_help("create")
                 sys.exit(1)
             Create.Modul(Create, sys.argv[3], sys.argv[4])
         elif OPTION in ["--submodul", "submodul", "-sm"]:
             if len(sys.argv) < 6:
-                show_help("error")
+                show_help("create")
                 sys.exit(1)
             Create.Submodul(Create, sys.argv[3], sys.argv[4], sys.argv[5:-1])
         elif OPTION in ["--script", "script", "-sc"]:
             if len(sys.argv) < 6:
-                show_help("error")
+                show_help("create")
                 sys.exit(1)
             Create.Script(Create, sys.argv[3], sys.argv[4], sys.argv[5])
         elif OPTION in ["--help", "help", "-h"]:
             show_help("create")
         else:
             show_help("create")
     elif CMD in ["--init", "init", "-i"]:
         if len(sys.argv) < 3:
-            show_help("error")
+            show_help("init")
             sys.exit(1)
 
         OPTION = sys.argv[2]
         if OPTION in ["--modul", "modul", "-m"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             Init.Modul(Init, sys.argv[3])
         elif OPTION in ["--submodul", "submodul", "-sm"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             Init.Submodul(Init, sys.argv[3])
         elif OPTION in ["--readme", "readme", "-r"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             Init.Readme(Init, sys.argv[3])
         elif OPTION in ["--setup", "setup", "-s"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             Init.Setup(Init, sys.argv[3])
         elif OPTION in ["--full", "full", "-f"]:
             if len(sys.argv) < 4:
-                show_help("error")
+                show_help("init")
                 sys.exit(1)
             NAME = sys.argv[3]
             Init.Modul(Init, NAME)
             Init.Submodul(Init, NAME)
             Init.Readme(Init, NAME)
             Init.Setup(Init, NAME)
         elif OPTION in ["--help", "help", "-h"]:
@@ -427,9 +427,58 @@
         if OPTION in ["--help", "help", "-h"]:
             show_help("yaml")
         else:
             FILE = OPTION
             Yaml.read(Yaml, FILE)
     elif CMD in ["--help", "help", "-h"]:
         show_help("help")
+    elif CMD in ["-cp"]:
+        if len(sys.argv) < 3:
+            show_help("create")
+            sys.exit(1)
+        Create.Project(Create, sys.argv[2])
+    elif CMD in ["-cm"]:
+        if len(sys.argv) < 4:
+            show_help("create")
+            sys.exit(1)
+        Create.Modul(Create, sys.argv[2], sys.argv[3])
+    elif CMD in ["-csm"]:
+        if len(sys.argv) < 5:
+            show_help("error")
+            sys.exit(1)
+        Create.Submodul(Create, sys.argv[2], sys.argv[3], sys.argv[4:-1])
+    elif CMD in ["-csc"]:
+        if len(sys.argv) < 5:
+            show_help("error")
+            sys.exit(1)
+        Create.Script(Create, sys.argv[2], sys.argv[3], sys.argv[4])
+    elif CMD in ["-im"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        Init.Modul(Init, sys.argv[2])
+    elif CMD in ["-ism"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        Init.Submodul(Init, sys.argv[2])
+    elif CMD in ["-ir"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        Init.Readme(Init, sys.argv[2])
+    elif CMD in ["-is"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        Init.Setup(Init, sys.argv[2])
+    elif CMD in ["-if"]:
+        if len(sys.argv) < 3:
+            show_help("init")
+            sys.exit(1)
+        NAME = sys.argv[2]
+        Init.Modul(Init, NAME)
+        Init.Submodul(Init, NAME)
+        Init.Readme(Init, NAME)
+        Init.Setup(Init, NAME)
     else:
         show_help("error")
```

### Comparing `pypa_make_easy-0.2/pypa_make_easy.egg-info/PKG-INFO` & `pypa_make_easy-0.3/pypa_make_easy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypa-make-easy
-Version: 0.2
+Version: 0.3
 Summary: Script to Create PyPi projects, but in easy
 Home-page: https://github.com/DevMasterLinux/pypa-make-easy
 Author: Kevin Alexander Krefting
 Author-email: kakrefting@gmail.com
 License: Apache License 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -77,7 +77,24 @@
 
 Install
 -------
 
 .. code-block:: bash
 
     python3 -m pip install pypa-make-easy
+
+Docker
+======
+
+You can with Docker Create your own PyPi packages Safe
+
+Build on Device
+
+.. code-block:: bash
+
+   ./scripts/run-docker.sh
+
+Download
+
+.. code-block:: bash
+
+   docker pull ghcr.io/devmasterlinux/pypa-make-easy/pypa-make-easy:1714930262
```

### Comparing `pypa_make_easy-0.2/setup.py` & `pypa_make_easy-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='pypa-make-easy',
-    version='0.2',
+    version='0.3',
     license='Apache License 2.0',
     description='Script to Create PyPi projects, but in easy',
     long_description=readme(),
     author='Kevin Alexander Krefting',
     author_email='kakrefting@gmail.com',
     url='https://github.com/DevMasterLinux/pypa-make-easy',
     scripts=['pypa-make-easy', 'pypa'],
```


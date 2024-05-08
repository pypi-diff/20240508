# Comparing `tmp/pisa_ssh-0.0.2.tar.gz` & `tmp/pisa_ssh-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisa_ssh-0.0.2.tar", last modified: Mon Apr 29 20:07:58 2024, max compression
+gzip compressed data, was "pisa_ssh-0.1.0.tar", last modified: Wed May  8 10:47:01 2024, max compression
```

## Comparing `pisa_ssh-0.0.2.tar` & `pisa_ssh-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 20:07:40.000000 pisa_ssh-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-29 20:07:40.000000 pisa_ssh-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-29 20:07:40.000000 pisa_ssh-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:58.186134 pisa_ssh-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/src/pisa/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 20:07:40.000000 pisa_ssh-0.0.2/src/pisa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.152060 pisa_ssh-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/dispatcher/cluster_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/dispatcher/task_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/runner/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-08 10:46:45.000000 pisa_ssh-0.1.0/src/pisa/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:47:01.156060 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 10:47:01.000000 pisa_ssh-0.1.0/src/pisa_ssh.egg-info/top_level.txt
```

### Comparing `pisa_ssh-0.0.2/LICENSE` & `pisa_ssh-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.0.2/PKG-INFO` & `pisa_ssh-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.0.2
-Summary: Python SSH Infrastructure for Scalable Applications (PISA)
+Version: 0.1.0
+Summary: Pseudo Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
 Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # pisa
-Python SSH Infrastructure for Scalable Applications (PISA)
+Pseudo Infrastructure for Scalable Applications (PISA)
 
 PISA is a simple but powerful program that allows to combine the computational power of multiple computers and turn them into a batch system using only the SSH access. It is designed to be simple and therefore only runs on a some machines from the computer pool of the physics department at KIT. It is not designed to be a general purpose batch system and is only maintained for this environment. Furthermore it is not designed to be used by many users at the same time because there is no limit provided for the allocated resources (our estimation is that only one person at the time will be using it). The large benefit of PISA is that it runs completely within the userspace and requires neither root access or higher privileges for installation nor to run the program.
 
 PISA connects to all the available machines using SSH. This only works when the authentication via an SSH key was set up before. Otherwise the connection cannot be established. Furthermore it requires the working directory (usually the home directory of all the users) to be the same on all machines. This is usual for our environment because the user home directories are mounted via NFS. The user interface is kept as simple as possible: Everything is dome from the command line. PISA gets a list of all the available machines and starts to connect to every one of them.
 
 TODO: Write more about the architecture.
```

### Comparing `pisa_ssh-0.0.2/README.md` & `pisa_ssh-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # pisa
-Python SSH Infrastructure for Scalable Applications (PISA)
+Pseudo Infrastructure for Scalable Applications (PISA)
 
 PISA is a simple but powerful program that allows to combine the computational power of multiple computers and turn them into a batch system using only the SSH access. It is designed to be simple and therefore only runs on a some machines from the computer pool of the physics department at KIT. It is not designed to be a general purpose batch system and is only maintained for this environment. Furthermore it is not designed to be used by many users at the same time because there is no limit provided for the allocated resources (our estimation is that only one person at the time will be using it). The large benefit of PISA is that it runs completely within the userspace and requires neither root access or higher privileges for installation nor to run the program.
 
 PISA connects to all the available machines using SSH. This only works when the authentication via an SSH key was set up before. Otherwise the connection cannot be established. Furthermore it requires the working directory (usually the home directory of all the users) to be the same on all machines. This is usual for our environment because the user home directories are mounted via NFS. The user interface is kept as simple as possible: Everything is dome from the command line. PISA gets a list of all the available machines and starts to connect to every one of them.
 
 TODO: Write more about the architecture.
```

### Comparing `pisa_ssh-0.0.2/pyproject.toml` & `pisa_ssh-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pisa-ssh"
-description = "Python SSH Infrastructure for Scalable Applications (PISA)"
+description = "Pseudo Infrastructure for Scalable Applications (PISA)"
 authors = [
 	{ name="Michael Hohenstein", email="michael@hohenste.in" },
 ]
 readme = "README.md"
-requires-python= ">=3.9"
+requires-python= ">=3.11"
 keywords = ["data", "analysis", "education", "university", "students", "physics"]
 
 license = {text = "MIT"}
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Topic :: Education",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     # currently no dependencies
 ]
 dynamic = ["version"]
@@ -50,16 +48,16 @@
     "twine", 
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/MitchiLaser/pisa/blob/main/docs/README.md" # TODO: Maybe provide github pages build and HTML page
 "Repository" = "https://github.com/MitchiLaser/pisa"
 
-#[project.scripts]
-#kafe2go = "kafe2.fit.tools.kafe2go:kafe2go" # TODO: Update for pisa dispatcher
+[project.scripts]
+pisa = "pisa.__main__:main"
 
 ########## TODO ???? ##############
 
 #[tool.pytest.ini_options]
 #testpaths = "kafe2/test"
 #python_files = "test*.py"
```

### Comparing `pisa_ssh-0.0.2/src/pisa_ssh.egg-info/PKG-INFO` & `pisa_ssh-0.1.0/src/pisa_ssh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.0.2
-Summary: Python SSH Infrastructure for Scalable Applications (PISA)
+Version: 0.1.0
+Summary: Pseudo Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
 Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # pisa
-Python SSH Infrastructure for Scalable Applications (PISA)
+Pseudo Infrastructure for Scalable Applications (PISA)
 
 PISA is a simple but powerful program that allows to combine the computational power of multiple computers and turn them into a batch system using only the SSH access. It is designed to be simple and therefore only runs on a some machines from the computer pool of the physics department at KIT. It is not designed to be a general purpose batch system and is only maintained for this environment. Furthermore it is not designed to be used by many users at the same time because there is no limit provided for the allocated resources (our estimation is that only one person at the time will be using it). The large benefit of PISA is that it runs completely within the userspace and requires neither root access or higher privileges for installation nor to run the program.
 
 PISA connects to all the available machines using SSH. This only works when the authentication via an SSH key was set up before. Otherwise the connection cannot be established. Furthermore it requires the working directory (usually the home directory of all the users) to be the same on all machines. This is usual for our environment because the user home directories are mounted via NFS. The user interface is kept as simple as possible: Everything is dome from the command line. PISA gets a list of all the available machines and starts to connect to every one of them.
 
 TODO: Write more about the architecture.
```


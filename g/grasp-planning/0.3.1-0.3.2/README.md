# Comparing `tmp/grasp_planning-0.3.1.tar.gz` & `tmp/grasp_planning-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.3.1.tar", last modified: Wed May  8 08:27:33 2024, max compression
+gzip compressed data, was "grasp_planning-0.3.2.tar", last modified: Wed May  8 08:29:28 2024, max compression
```

## Comparing `grasp_planning-0.3.1.tar` & `grasp_planning-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:27:33.975582 grasp_planning-0.3.1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      268 2024-05-08 08:27:33.975582 grasp_planning-0.3.1/PKG-INFO
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:27:33.975582 grasp_planning-0.3.1/grasp_planning/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2024-05-07 16:34:01.000000 grasp_planning-0.3.1/grasp_planning/__init__.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:27:33.975582 grasp_planning-0.3.1/grasp_planning.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      268 2024-05-08 08:27:33.000000 grasp_planning-0.3.1/grasp_planning.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      224 2024-05-08 08:27:33.000000 grasp_planning-0.3.1/grasp_planning.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-08 08:27:33.000000 grasp_planning-0.3.1/grasp_planning.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       75 2024-05-08 08:27:33.000000 grasp_planning-0.3.1/grasp_planning.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2024-05-08 08:27:33.000000 grasp_planning-0.3.1/grasp_planning.egg-info/top_level.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-08 08:27:33.975582 grasp_planning-0.3.1/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      686 2024-05-08 08:27:29.000000 grasp_planning-0.3.1/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:29:28.724439 grasp_planning-0.3.2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      268 2024-05-08 08:29:28.724439 grasp_planning-0.3.2/PKG-INFO
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:29:28.724439 grasp_planning-0.3.2/grasp_planning/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2024-05-07 16:34:01.000000 grasp_planning-0.3.2/grasp_planning/__init__.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:29:28.724439 grasp_planning-0.3.2/grasp_planning.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      268 2024-05-08 08:29:28.000000 grasp_planning-0.3.2/grasp_planning.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      224 2024-05-08 08:29:28.000000 grasp_planning-0.3.2/grasp_planning.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-08 08:29:28.000000 grasp_planning-0.3.2/grasp_planning.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       75 2024-05-08 08:29:28.000000 grasp_planning-0.3.2/grasp_planning.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2024-05-08 08:29:28.000000 grasp_planning-0.3.2/grasp_planning.egg-info/top_level.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-08 08:29:28.724439 grasp_planning-0.3.2/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      689 2024-05-08 08:29:27.000000 grasp_planning-0.3.2/setup.py
```

### Comparing `grasp_planning-0.3.1/setup.py` & `grasp_planning-0.3.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = [] # Here we'll add: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirement_path):
     with open(requirement_path) as f:
         install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="grasp_planning",
-    version="0.3.1", 
+    version="0.3.2", 
     author="Tomas Merva", 
     author_email="tmerva7@gmail.com",
     description="Grasp and Motion Planning Python Package",
     long_description="Grasp and Motion Planning Python Package",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages('.'),
     install_requires=install_requires
 )
```


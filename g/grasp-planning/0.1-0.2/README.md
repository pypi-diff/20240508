# Comparing `tmp/grasp_planning-0.1.tar.gz` & `tmp/grasp_planning-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.1.tar", last modified: Tue May  7 16:37:18 2024, max compression
+gzip compressed data, was "grasp_planning-0.2.tar", last modified: Wed May  8 08:15:45 2024, max compression
```

## Comparing `grasp_planning-0.1.tar` & `grasp_planning-0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-07 16:37:18.871979 grasp_planning-0.1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2024-05-07 16:37:18.871979 grasp_planning-0.1/PKG-INFO
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-07 16:37:18.871979 grasp_planning-0.1/grasp_planning.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2024-05-07 16:37:18.000000 grasp_planning-0.1/grasp_planning.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      197 2024-05-07 16:37:18.000000 grasp_planning-0.1/grasp_planning.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-07 16:37:18.000000 grasp_planning-0.1/grasp_planning.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       75 2024-05-07 16:37:18.000000 grasp_planning-0.1/grasp_planning.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-07 16:37:18.000000 grasp_planning-0.1/grasp_planning.egg-info/top_level.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-07 16:37:18.871979 grasp_planning-0.1/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      645 2024-05-07 16:32:34.000000 grasp_planning-0.1/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:15:45.310712 grasp_planning-0.2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2024-05-08 08:15:45.310712 grasp_planning-0.2/PKG-INFO
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:15:45.310712 grasp_planning-0.2/grasp_planning/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2024-05-07 16:34:01.000000 grasp_planning-0.2/grasp_planning/__init__.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:15:45.310712 grasp_planning-0.2/grasp_planning.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      266 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      224 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       75 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2024-05-08 08:15:45.000000 grasp_planning-0.2/grasp_planning.egg-info/top_level.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-08 08:15:45.310712 grasp_planning-0.2/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      676 2024-05-08 08:15:42.000000 grasp_planning-0.2/setup.py
```

### Comparing `grasp_planning-0.1/setup.py` & `grasp_planning-0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 requirement_path = f"{lib_folder}/requirements.txt"
 install_requires = [] # Here we'll add: ["gunicorn", "docutils>=0.3", "lxml==0.5a7"]
 if os.path.isfile(requirement_path):
     with open(requirement_path) as f:
         install_requires = f.read().splitlines()
 
 setuptools.setup(
-    name="grasp_planning", 
-    version  = '0.1',
+    name="grasp_planning",
+    version="0.2", 
     author="Tomas Merva", 
-    author_email='tmerva7@gmail.com',
-    description='Grasp and Motion Planning Python Package',
-    long_description='Grasp and Motion Planning Python Package',
+    author_email="tmerva7@gmail.com",
+    description="Grasp and Motion Planning Python Package",
+    long_description="Grasp and Motion Planning Python Package",
+    packages=["grasp_planning"],
     install_requires=install_requires
-)
+)
```


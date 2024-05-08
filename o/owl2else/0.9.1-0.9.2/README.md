# Comparing `tmp/owl2else-0.9.1.tar.gz` & `tmp/owl2else-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owl2else-0.9.1.tar", last modified: Tue Oct  3 07:59:19 2023, max compression
+gzip compressed data, was "owl2else-0.9.2.tar", last modified: Wed May  8 14:06:12 2024, max compression
```

## Comparing `owl2else-0.9.1.tar` & `owl2else-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-10-03 07:59:19.463874 owl2else-0.9.1/
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     3228 2022-05-13 09:13:03.000000 owl2else-0.9.1/.gitignore
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)    35149 2022-05-13 09:13:03.000000 owl2else-0.9.1/LICENSE
--rw-r--r--   0 bejar     (1000) bejar     (1000)      868 2023-10-03 07:59:19.463874 owl2else-0.9.1/PKG-INFO
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)      345 2022-05-13 09:13:03.000000 owl2else-0.9.1/README.md
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-10-03 07:59:19.461874 owl2else-0.9.1/bin/
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     4803 2022-05-13 09:13:03.000000 owl2else-0.9.1/bin/owl2clips
--rw-r--r--   0 bejar     (1000) bejar     (1000)       35 2023-10-03 07:38:02.000000 owl2else-0.9.1/bin/owl2clips.bat
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     4711 2022-05-13 09:13:03.000000 owl2else-0.9.1/bin/owl2plot
--rw-r--r--   0 bejar     (1000) bejar     (1000)       34 2023-10-03 07:54:33.000000 owl2else-0.9.1/bin/owl2plot.bat
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     3013 2022-05-13 09:13:03.000000 owl2else-0.9.1/bin/owl2rdflib
--rw-r--r--   0 bejar     (1000) bejar     (1000)       36 2023-10-03 07:54:52.000000 owl2else-0.9.1/bin/owl2rdflib.bat
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-10-03 07:59:19.461874 owl2else-0.9.1/owl2conv/
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)      217 2022-05-13 09:13:03.000000 owl2else-0.9.1/owl2conv/__init__.py
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)    11761 2022-05-13 09:36:35.000000 owl2else-0.9.1/owl2conv/owlobjects.py
-drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2023-10-03 07:59:19.463874 owl2else-0.9.1/owl2else.egg-info/
--rw-r--r--   0 bejar     (1000) bejar     (1000)      868 2023-10-03 07:59:19.000000 owl2else-0.9.1/owl2else.egg-info/PKG-INFO
--rw-rw-r--   0 bejar     (1000) bejar     (1000)      351 2023-10-03 07:59:19.000000 owl2else-0.9.1/owl2else.egg-info/SOURCES.txt
--rw-rw-r--   0 bejar     (1000) bejar     (1000)        1 2023-10-03 07:59:19.000000 owl2else-0.9.1/owl2else.egg-info/dependency_links.txt
--rw-rw-r--   0 bejar     (1000) bejar     (1000)       27 2023-10-03 07:59:19.000000 owl2else-0.9.1/owl2else.egg-info/requires.txt
--rw-rw-r--   0 bejar     (1000) bejar     (1000)        9 2023-10-03 07:59:19.000000 owl2else-0.9.1/owl2else.egg-info/top_level.txt
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)      203 2023-10-03 07:45:56.000000 owl2else-0.9.1/pack
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)       79 2023-10-03 07:59:19.464874 owl2else-0.9.1/setup.cfg
--rwxrwxr-x   0 bejar     (1000) bejar     (1000)     1073 2023-10-03 07:55:47.000000 owl2else-0.9.1/setup.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-08 14:06:12.001621 owl2else-0.9.2/
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     3228 2022-05-13 09:13:03.000000 owl2else-0.9.2/.gitignore
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)    35149 2022-05-13 09:13:03.000000 owl2else-0.9.2/LICENSE
+-rw-r--r--   0 bejar     (1000) bejar     (1000)      868 2024-05-08 14:06:12.001621 owl2else-0.9.2/PKG-INFO
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)      345 2022-05-13 09:13:03.000000 owl2else-0.9.2/README.md
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-08 14:06:11.964621 owl2else-0.9.2/bin/
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     4803 2022-05-13 09:13:03.000000 owl2else-0.9.2/bin/owl2clips
+-rw-r--r--   0 bejar     (1000) bejar     (1000)       35 2023-10-03 07:38:02.000000 owl2else-0.9.2/bin/owl2clips.bat
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     4711 2022-05-13 09:13:03.000000 owl2else-0.9.2/bin/owl2plot
+-rw-r--r--   0 bejar     (1000) bejar     (1000)       34 2023-10-03 07:54:33.000000 owl2else-0.9.2/bin/owl2plot.bat
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     3691 2024-05-08 14:01:42.000000 owl2else-0.9.2/bin/owl2rdflib
+-rw-r--r--   0 bejar     (1000) bejar     (1000)       36 2023-10-03 07:54:52.000000 owl2else-0.9.2/bin/owl2rdflib.bat
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-08 14:06:11.998621 owl2else-0.9.2/owl2conv/
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)      217 2022-05-13 09:13:03.000000 owl2else-0.9.2/owl2conv/__init__.py
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)    11874 2023-10-19 04:34:55.000000 owl2else-0.9.2/owl2conv/owlobjects.py
+drwxrwxr-x   0 bejar     (1000) bejar     (1000)        0 2024-05-08 14:06:12.000621 owl2else-0.9.2/owl2else.egg-info/
+-rw-r--r--   0 bejar     (1000) bejar     (1000)      868 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/PKG-INFO
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)      351 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/SOURCES.txt
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)        1 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/dependency_links.txt
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)       27 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/requires.txt
+-rw-rw-r--   0 bejar     (1000) bejar     (1000)        9 2024-05-08 14:06:11.000000 owl2else-0.9.2/owl2else.egg-info/top_level.txt
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)      203 2023-10-03 07:45:56.000000 owl2else-0.9.2/pack
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)       79 2024-05-08 14:06:12.002621 owl2else-0.9.2/setup.cfg
+-rwxrwxr-x   0 bejar     (1000) bejar     (1000)     1073 2024-05-08 14:05:46.000000 owl2else-0.9.2/setup.py
```

### Comparing `owl2else-0.9.1/.gitignore` & `owl2else-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `owl2else-0.9.1/LICENSE` & `owl2else-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `owl2else-0.9.1/PKG-INFO` & `owl2else-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owl2else
-Version: 0.9.1
+Version: 0.9.2
 Summary: Utilities to transform ontology OWL2 files to other formats
 Home-page: https://github.com/bejar/owl2else
 Author: Javier Bejar
 Author-email: bejar@cs.upc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `owl2else-0.9.1/bin/owl2clips` & `owl2else-0.9.2/bin/owl2clips`

 * *Files identical despite different names*

### Comparing `owl2else-0.9.1/bin/owl2plot` & `owl2else-0.9.2/bin/owl2plot`

 * *Files identical despite different names*

### Comparing `owl2else-0.9.1/owl2conv/owlobjects.py` & `owl2else-0.9.2/owl2conv/owlobjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,22 +287,24 @@
         :param graph:
         :param cdict:
         :return:
         """
         iclass = graph.objects(self.uriref, RDF.type)
 
         # Selects the class for the instance skipping OWL.NamedIndividual
+        curi = None
         for c in iclass:
             if c != OWL.NamedIndividual:
                 self.iclass = self.chop(c)
                 curi = c
 
+        if curi is None:
+            raise NameError(f'Instance {self.name} has no class!!!')
         iclass_name = graph.objects(curi, RDFS.label)
 
-
         for n in iclass_name:
             self.iclass_label = n.replace(' ', '_') 
         if self.iclass_label is None:
             self.iclass_label = self.chop(curi)
 
         # If individual has no class something is wrong
         if self.iclass is None:
```

### Comparing `owl2else-0.9.1/owl2else.egg-info/PKG-INFO` & `owl2else-0.9.2/owl2else.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owl2else
-Version: 0.9.1
+Version: 0.9.2
 Summary: Utilities to transform ontology OWL2 files to other formats
 Home-page: https://github.com/bejar/owl2else
 Author: Javier Bejar
 Author-email: bejar@cs.upc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `owl2else-0.9.1/setup.py` & `owl2else-0.9.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="owl2else", # Replace with your own username
-    version="0.9.1",
+    version="0.9.2",
     author="Javier Bejar",
     author_email="bejar@cs.upc.edu",
     description="Utilities to transform ontology OWL2 files to other formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bejar/owl2else",
     packages=['owl2conv'],
```


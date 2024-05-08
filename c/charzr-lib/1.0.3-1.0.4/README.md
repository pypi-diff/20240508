# Comparing `tmp/charzr_lib-1.0.3.tar.gz` & `tmp/charzr_lib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charzr_lib-1.0.3.tar", last modified: Wed May  8 02:25:56 2024, max compression
+gzip compressed data, was "charzr_lib-1.0.4.tar", last modified: Wed May  8 03:06:25 2024, max compression
```

## Comparing `charzr_lib-1.0.3.tar` & `charzr_lib-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 02:25:56.454942 charzr_lib-1.0.3/
--rw-rw-rw-   0        0        0      316 2024-05-08 02:25:56.450061 charzr_lib-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 02:25:56.291902 charzr_lib-1.0.3/charzr_lib/
--rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.3/charzr_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.3/charzr_lib/pokemon.csv
--rw-rw-rw-   0        0        0      743 2024-05-08 00:26:00.000000 charzr_lib-1.0.3/charzr_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 02:25:56.447133 charzr_lib-1.0.3/charzr_lib.egg-info/
--rw-rw-rw-   0        0        0      316 2024-05-08 02:25:53.000000 charzr_lib-1.0.3/charzr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-08 02:25:53.000000 charzr_lib-1.0.3/charzr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 02:25:53.000000 charzr_lib-1.0.3/charzr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 02:25:53.000000 charzr_lib-1.0.3/charzr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 02:25:53.000000 charzr_lib-1.0.3/charzr_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 02:25:56.454942 charzr_lib-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      454 2024-05-08 01:13:44.000000 charzr_lib-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:25.138156 charzr_lib-1.0.4/
+-rw-rw-rw-   0        0        0      316 2024-05-08 03:06:25.135228 charzr_lib-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:24.984878 charzr_lib-1.0.4/charzr_lib/
+-rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.4/charzr_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.4/charzr_lib/pokemon.csv
+-rw-rw-rw-   0        0        0      812 2024-05-08 03:05:58.000000 charzr_lib-1.0.4/charzr_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:06:25.131323 charzr_lib-1.0.4/charzr_lib.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-08 03:06:23.000000 charzr_lib-1.0.4/charzr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-08 03:06:24.000000 charzr_lib-1.0.4/charzr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:06:23.000000 charzr_lib-1.0.4/charzr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 03:06:23.000000 charzr_lib-1.0.4/charzr_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 03:06:23.000000 charzr_lib-1.0.4/charzr_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:06:25.138156 charzr_lib-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      454 2024-05-08 03:05:58.000000 charzr_lib-1.0.4/setup.py
```

### Comparing `charzr_lib-1.0.3/README.md` & `charzr_lib-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.3/charzr_lib/pokemon.csv` & `charzr_lib-1.0.4/charzr_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.3/charzr_lib/random_pokemon.py` & `charzr_lib-1.0.4/charzr_lib/random_pokemon.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import pkg_resources
 import pandas as pd
 
 class RandomPokemon:
     FILE_PATH = pkg_resources.resource_filename(__name__, 'pokemon.csv')
 
-def __init__(self):
-    self._file = pd.read_csv(RandomPokemon.FILE_PATH)
-    self._pokemon = None
-    self._number = None
-    self._name = None
-    self._type1 = None
-
-def generate_random (self):
-    self._pokemon = self._file. sample()
-    self._number = self._pokemon["#"]. values[0]
-    self._name = self._pokemon["Name"]. values[0]
-    self._type1 = self._pokemon["Type 1"]. values[0]
-
-def getPokemon(self):
-    return self._pokemon
+    def __init__(self):
+        self._file = pd.read_csv(RandomPokemon.FILE_PATH)
+        self._pokemon = None
+        self._number = None
+        self._name = None
+        self._type1 = None
+
+    def generate_random(self):
+       self._pokemon = self._file. sample()
+       self._number = self._pokemon["#"]. values[0]
+       self._name = self._pokemon["Name"]. values[0]
+       self._type1 = self._pokemon["Type 1"]. values[0]
+
+    def getPokemon(self):
+       return self._pokemon
 
-def getNumber(self):
-    return self._number
+    def getNumber(self):
+       return self._number
 
-def getName(self):
-    return self._name
+    def getName(self):
+        return self._name
 
-def getType1(self):
-    return self._type1
+    def getType1(self):
+        return self._type1
```


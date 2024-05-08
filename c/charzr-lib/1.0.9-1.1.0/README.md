# Comparing `tmp/charzr_lib-1.0.9.tar.gz` & `tmp/charzr_lib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charzr_lib-1.0.9.tar", last modified: Wed May  8 04:23:34 2024, max compression
+gzip compressed data, was "charzr_lib-1.1.0.tar", last modified: Wed May  8 04:27:45 2024, max compression
```

## Comparing `charzr_lib-1.0.9.tar` & `charzr_lib-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 04:23:34.880801 charzr_lib-1.0.9/
--rw-rw-rw-   0        0        0      316 2024-05-08 04:23:34.877873 charzr_lib-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 04:23:34.817343 charzr_lib-1.0.9/charzr_lib/
--rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.9/charzr_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.9/charzr_lib/pokemon.csv
--rw-rw-rw-   0        0        0     2272 2024-05-08 04:23:16.000000 charzr_lib-1.0.9/charzr_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:23:34.874944 charzr_lib-1.0.9/charzr_lib.egg-info/
--rw-rw-rw-   0        0        0      316 2024-05-08 04:23:33.000000 charzr_lib-1.0.9/charzr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-08 04:23:33.000000 charzr_lib-1.0.9/charzr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 04:23:33.000000 charzr_lib-1.0.9/charzr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 04:23:33.000000 charzr_lib-1.0.9/charzr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 04:23:33.000000 charzr_lib-1.0.9/charzr_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 04:23:34.880801 charzr_lib-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      454 2024-05-08 04:23:16.000000 charzr_lib-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:27:45.639587 charzr_lib-1.1.0/
+-rw-rw-rw-   0        0        0      316 2024-05-08 04:27:45.635682 charzr_lib-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 04:27:45.491190 charzr_lib-1.1.0/charzr_lib/
+-rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.1.0/charzr_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.1.0/charzr_lib/pokemon.csv
+-rw-rw-rw-   0        0        0     2270 2024-05-08 04:26:41.000000 charzr_lib-1.1.0/charzr_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:27:45.632754 charzr_lib-1.1.0/charzr_lib.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-08 04:27:43.000000 charzr_lib-1.1.0/charzr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-08 04:27:43.000000 charzr_lib-1.1.0/charzr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 04:27:43.000000 charzr_lib-1.1.0/charzr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 04:27:43.000000 charzr_lib-1.1.0/charzr_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 04:27:43.000000 charzr_lib-1.1.0/charzr_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 04:27:45.640563 charzr_lib-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      454 2024-05-08 04:27:31.000000 charzr_lib-1.1.0/setup.py
```

### Comparing `charzr_lib-1.0.9/README.md` & `charzr_lib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.9/charzr_lib/pokemon.csv` & `charzr_lib-1.1.0/charzr_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.9/charzr_lib/random_pokemon.py` & `charzr_lib-1.1.0/charzr_lib/random_pokemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         self._name = self._pokemon["Name"]. values[0]
         self._type1 = self._pokemon["Type 1"]. values[0]
         self._type2 = self._pokemon["Type 2"].values[0]
         self._total = self._pokemon["Total"].values[0]
         self._hp = self._pokemon["HP"].values[0]
         self._attack = self._pokemon["Attack"].values[0]
         self._defense = self._pokemon["Defense"].values[0]
-        self._spatk = self._pokemon["Sp.Atk"].values[0]
-        self._spdef = self._pokemon["Sp.Def"].values[0]
+        self._spatk = self._pokemon["SpAtk"].values[0]
+        self._spdef = self._pokemon["SpDef"].values[0]
         self._speed = self._pokemon["Speed"].values[0]
         self._generation = self._pokemon["Generation"].values[0]
         self._legendary = self._pokemon["Legendary"].values[0]
 
     def getPokemon(self):
        return self._pokemon
 
@@ -66,15 +66,15 @@
 
     def getDefense(self):
         return self._defense
 
     def getSpAtk(self):
         return self._spatk
 
-    def getSpdef(self):
+    def getSpDef(self):
         return self._spdef
 
     def getSpeed(self):
         return self._speed
 
     def getGeneration(self):
         return self._generation
```


# Comparing `tmp/charzr_lib-1.1.1.tar.gz` & `tmp/charzr_lib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charzr_lib-1.1.1.tar", last modified: Wed May  8 04:34:41 2024, max compression
+gzip compressed data, was "charzr_lib-1.1.2.tar", last modified: Wed May  8 04:41:18 2024, max compression
```

## Comparing `charzr_lib-1.1.1.tar` & `charzr_lib-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 04:34:41.468294 charzr_lib-1.1.1/
--rw-rw-rw-   0        0        0      316 2024-05-08 04:34:41.465364 charzr_lib-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 04:34:41.331612 charzr_lib-1.1.1/charzr_lib/
--rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.1.1/charzr_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.1.1/charzr_lib/pokemon.csv
--rw-rw-rw-   0        0        0     2274 2024-05-08 04:34:23.000000 charzr_lib-1.1.1/charzr_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:34:41.462437 charzr_lib-1.1.1/charzr_lib.egg-info/
--rw-rw-rw-   0        0        0      316 2024-05-08 04:34:39.000000 charzr_lib-1.1.1/charzr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-08 04:34:39.000000 charzr_lib-1.1.1/charzr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 04:34:39.000000 charzr_lib-1.1.1/charzr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 04:34:39.000000 charzr_lib-1.1.1/charzr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 04:34:39.000000 charzr_lib-1.1.1/charzr_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 04:34:41.468294 charzr_lib-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      454 2024-05-08 04:34:22.000000 charzr_lib-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:41:18.670389 charzr_lib-1.1.2/
+-rw-rw-rw-   0        0        0      316 2024-05-08 04:41:18.666483 charzr_lib-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 04:41:18.513205 charzr_lib-1.1.2/charzr_lib/
+-rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.1.2/charzr_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.1.2/charzr_lib/pokemon.csv
+-rw-rw-rw-   0        0        0     2245 2024-05-08 04:40:26.000000 charzr_lib-1.1.2/charzr_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:41:18.663553 charzr_lib-1.1.2/charzr_lib.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-08 04:41:17.000000 charzr_lib-1.1.2/charzr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-08 04:41:17.000000 charzr_lib-1.1.2/charzr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 04:41:17.000000 charzr_lib-1.1.2/charzr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 04:41:17.000000 charzr_lib-1.1.2/charzr_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 04:41:17.000000 charzr_lib-1.1.2/charzr_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 04:41:18.670389 charzr_lib-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      464 2024-05-08 04:41:02.000000 charzr_lib-1.1.2/setup.py
```

### Comparing `charzr_lib-1.1.1/README.md` & `charzr_lib-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.1.1/charzr_lib/pokemon.csv` & `charzr_lib-1.1.2/charzr_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.1.1/charzr_lib/random_pokemon.py` & `charzr_lib-1.1.2/charzr_lib/random_pokemon.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 
     def generate_random(self):
         self._pokemon = self._file. sample()
         self._number = self._pokemon["#"]. values[0]
         self._name = self._pokemon["Name"]. values[0]
         self._type1 = self._pokemon["Type 1"]. values[0]
         self._type2 = self._pokemon["Type 2"].values[0]
-        self._total = self._pokemon["Total"].values[0]
-        self._hp = self._pokemon["HP"].values[0]
-        self._attack = self._pokemon["Attack"].values[0]
-        self._defense = self._pokemon["Defense"].values[0]
-        self._spatk = self._pokemon["SpAtk"].values[0]
-        self._spdef = self._pokemon["SpDef"].values[0]
-        self._speed = self._pokemon["Speed"].values[0]
-        self._generation = self._pokemon["Generation"].values[0]
+        self._total = self._pokemon["#1"].values[0]
+        self._hp = self._pokemon["#2"].values[0]
+        self._attack = self._pokemon["#3"].values[0]
+        self._defense = self._pokemon["#4"].values[0]
+        self._spatk = self._pokemon["#5"].values[0]
+        self._spdef = self._pokemon["#6"].values[0]
+        self._speed = self._pokemon["#7"].values[0]
+        self._generation = self._pokemon["#8"].values[0]
         self._legendary = self._pokemon["Legendary"].values[0]
 
     def getPokemon(self):
 
         return self._pokemon
 
     def getNumber(self):
```


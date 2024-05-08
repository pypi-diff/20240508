# Comparing `tmp/charzr_lib-1.0.7.tar.gz` & `tmp/charzr_lib-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charzr_lib-1.0.7.tar", last modified: Wed May  8 04:08:44 2024, max compression
+gzip compressed data, was "charzr_lib-1.0.8.tar", last modified: Wed May  8 04:17:56 2024, max compression
```

## Comparing `charzr_lib-1.0.7.tar` & `charzr_lib-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 04:08:44.834489 charzr_lib-1.0.7/
--rw-rw-rw-   0        0        0      316 2024-05-08 04:08:44.818868 charzr_lib-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 04:08:44.497669 charzr_lib-1.0.7/charzr_lib/
--rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.7/charzr_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.7/charzr_lib/pokemon.csv
--rw-rw-rw-   0        0        0     2272 2024-05-08 04:07:06.000000 charzr_lib-1.0.7/charzr_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:08:44.814962 charzr_lib-1.0.7/charzr_lib.egg-info/
--rw-rw-rw-   0        0        0      316 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 04:08:44.836443 charzr_lib-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      454 2024-05-08 04:08:14.000000 charzr_lib-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:17:56.191597 charzr_lib-1.0.8/
+-rw-rw-rw-   0        0        0      316 2024-05-08 04:17:56.188670 charzr_lib-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 04:17:56.085181 charzr_lib-1.0.8/charzr_lib/
+-rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.8/charzr_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.8/charzr_lib/pokemon.csv
+-rw-rw-rw-   0        0        0     2233 2024-05-08 04:16:31.000000 charzr_lib-1.0.8/charzr_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:17:56.185739 charzr_lib-1.0.8/charzr_lib.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-08 04:17:55.000000 charzr_lib-1.0.8/charzr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-08 04:17:55.000000 charzr_lib-1.0.8/charzr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 04:17:55.000000 charzr_lib-1.0.8/charzr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 04:17:55.000000 charzr_lib-1.0.8/charzr_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 04:17:55.000000 charzr_lib-1.0.8/charzr_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 04:17:56.191597 charzr_lib-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      454 2024-05-08 04:17:47.000000 charzr_lib-1.0.8/setup.py
```

### Comparing `charzr_lib-1.0.7/README.md` & `charzr_lib-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.7/charzr_lib/pokemon.csv` & `charzr_lib-1.0.8/charzr_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.7/charzr_lib/random_pokemon.py` & `charzr_lib-1.0.8/charzr_lib/random_pokemon.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 
     def generate_random(self):
         self._pokemon = self._file. sample()
         self._number = self._pokemon["#"]. values[0]
         self._name = self._pokemon["Name"]. values[0]
         self._type1 = self._pokemon["Type 1"]. values[0]
         self._type2 = self._pokemon["Type 2"].values[0]
-        self._total = self._pokemon["Total"].values[0]
-        self._hp = self._pokemon["hp"].values[0]
-        self._attack = self._pokemon["Attack"].values[0]
-        self._defense = self._pokemon["Defense"].values[0]
-        self._spatk = self._pokemon["Sp.Atk"].values[0]
-        self._spdef = self._pokemon["Sp.Def"].values[0]
-        self._speed = self._pokemon["Speed"].values[0]
-        self._generation = self._pokemon["Generation"].values[0]
+        self._total = self._pokemon["#"].values[0]
+        self._hp = self._pokemon["#"].values[0]
+        self._attack = self._pokemon["#"].values[0]
+        self._defense = self._pokemon["#"].values[0]
+        self._spatk = self._pokemon["#"].values[0]
+        self._spdef = self._pokemon["#"].values[0]
+        self._speed = self._pokemon["#"].values[0]
+        self._generation = self._pokemon["#"].values[0]
         self._legendary = self._pokemon["Legendary"].values[0]
 
     def getPokemon(self):
        return self._pokemon
 
     def getNumber(self):
        return self._number
```


# Comparing `tmp/charzr_lib-1.1.3.tar.gz` & `tmp/charzr_lib-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charzr_lib-1.1.3.tar", last modified: Wed May  8 04:50:01 2024, max compression
+gzip compressed data, was "charzr_lib-1.1.4.tar", last modified: Wed May  8 05:02:45 2024, max compression
```

## Comparing `charzr_lib-1.1.3.tar` & `charzr_lib-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 04:50:01.179140 charzr_lib-1.1.3/
--rw-rw-rw-   0        0        0      316 2024-05-08 04:50:01.176212 charzr_lib-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 04:50:01.050270 charzr_lib-1.1.3/charzr_lib/
--rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.1.3/charzr_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.1.3/charzr_lib/pokemon.csv
--rw-rw-rw-   0        0        0     2237 2024-05-08 04:49:39.000000 charzr_lib-1.1.3/charzr_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:50:01.172306 charzr_lib-1.1.3/charzr_lib.egg-info/
--rw-rw-rw-   0        0        0      316 2024-05-08 04:49:59.000000 charzr_lib-1.1.3/charzr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-08 04:50:00.000000 charzr_lib-1.1.3/charzr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 04:49:59.000000 charzr_lib-1.1.3/charzr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 04:49:59.000000 charzr_lib-1.1.3/charzr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 04:49:59.000000 charzr_lib-1.1.3/charzr_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 04:50:01.179140 charzr_lib-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      464 2024-05-08 04:49:39.000000 charzr_lib-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:02:45.105100 charzr_lib-1.1.4/
+-rw-rw-rw-   0        0        0      316 2024-05-08 05:02:45.102172 charzr_lib-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 05:02:44.952800 charzr_lib-1.1.4/charzr_lib/
+-rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.1.4/charzr_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.1.4/charzr_lib/pokemon.csv
+-rw-rw-rw-   0        0        0     2276 2024-05-08 05:02:16.000000 charzr_lib-1.1.4/charzr_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:02:45.100220 charzr_lib-1.1.4/charzr_lib.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-08 05:02:43.000000 charzr_lib-1.1.4/charzr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-08 05:02:43.000000 charzr_lib-1.1.4/charzr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 05:02:43.000000 charzr_lib-1.1.4/charzr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 05:02:43.000000 charzr_lib-1.1.4/charzr_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 05:02:43.000000 charzr_lib-1.1.4/charzr_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 05:02:45.105100 charzr_lib-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      464 2024-05-08 05:02:31.000000 charzr_lib-1.1.4/setup.py
```

### Comparing `charzr_lib-1.1.3/README.md` & `charzr_lib-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.1.3/charzr_lib/pokemon.csv` & `charzr_lib-1.1.4/charzr_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.1.3/charzr_lib/random_pokemon.py` & `charzr_lib-1.1.4/charzr_lib/random_pokemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 
     def generate_random(self):
         self._pokemon = self._file. sample()
         self._number = self._pokemon["#"]. values[0]
         self._name = self._pokemon["Name"]. values[0]
         self._type1 = self._pokemon["Type 1"]. values[0]
         self._type2 = self._pokemon["Type 2"].values[0]
-        self._total = self._pokemon[int].values[0]
-        self._hp = self._pokemon[int].values[0]
-        self._attack = self._pokemon[int].values[0]
-        self._defense = self._pokemon[int].values[0]
-        self._spatk = self._pokemon[int].values[0]
-        self._spdef = self._pokemon[int].values[0]
-        self._speed = self._pokemon[int].values[0]
-        self._generation = self._pokemon[int].values[0]
+        self._total = self._pokemon["Total"].values[0]
+        self._hp = self._pokemon["HP"].values[0]
+        self._attack = self._pokemon["Attack"].values[0]
+        self._defense = self._pokemon["Defense"].values[0]
+        self._spatk = self._pokemon["Sp.Atk"].values[0]
+        self._spdef = self._pokemon["Sp.Def"].values[0]
+        self._speed = self._pokemon["Speed"].values[0]
+        self._generation = self._pokemon["Generation"].values[0]
         self._legendary = self._pokemon["Legendary"].values[0]
 
     def getPokemon(self):
 
         return self._pokemon
 
     def getNumber(self):
```


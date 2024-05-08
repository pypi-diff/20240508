# Comparing `tmp/charzr_lib-1.0.6.tar.gz` & `tmp/charzr_lib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charzr_lib-1.0.6.tar", last modified: Wed May  8 03:44:45 2024, max compression
+gzip compressed data, was "charzr_lib-1.0.7.tar", last modified: Wed May  8 04:08:44 2024, max compression
```

## Comparing `charzr_lib-1.0.6.tar` & `charzr_lib-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 03:44:45.920518 charzr_lib-1.0.6/
--rw-rw-rw-   0        0        0      316 2024-05-08 03:44:45.914660 charzr_lib-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 03:44:45.793600 charzr_lib-1.0.6/charzr_lib/
--rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.6/charzr_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.6/charzr_lib/pokemon.csv
--rw-rw-rw-   0        0        0     2258 2024-05-08 03:42:57.000000 charzr_lib-1.0.6/charzr_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:44:45.909779 charzr_lib-1.0.6/charzr_lib.egg-info/
--rw-rw-rw-   0        0        0      316 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 03:44:45.921495 charzr_lib-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      454 2024-05-08 03:42:57.000000 charzr_lib-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:08:44.834489 charzr_lib-1.0.7/
+-rw-rw-rw-   0        0        0      316 2024-05-08 04:08:44.818868 charzr_lib-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 04:08:44.497669 charzr_lib-1.0.7/charzr_lib/
+-rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.7/charzr_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.7/charzr_lib/pokemon.csv
+-rw-rw-rw-   0        0        0     2272 2024-05-08 04:07:06.000000 charzr_lib-1.0.7/charzr_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:08:44.814962 charzr_lib-1.0.7/charzr_lib.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 04:08:42.000000 charzr_lib-1.0.7/charzr_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 04:08:44.836443 charzr_lib-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      454 2024-05-08 04:08:14.000000 charzr_lib-1.0.7/setup.py
```

### Comparing `charzr_lib-1.0.6/README.md` & `charzr_lib-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.6/charzr_lib/pokemon.csv` & `charzr_lib-1.0.7/charzr_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.6/charzr_lib/random_pokemon.py` & `charzr_lib-1.0.7/charzr_lib/random_pokemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,28 +18,28 @@
         self._spatk = None
         self._spdef = None
         self._speed = None
         self._generation = None
         self._legendary = None
 
     def generate_random(self):
-       self._pokemon = self._file. sample()
-       self._number = self._pokemon["#"]. values[0]
-       self._name = self._pokemon["Name"]. values[0]
-       self._type1 = self._pokemon["Type 1"]. values[0]
-       self._type2 = self._pokemon["Type 2"].values[0]
-       self._total = self._pokemon["Total"].values[0]
-       self._hp = self._pokemon["hp"].values[0]
-       self._attack = self._pokemon["Attack"].values[0]
-       self._defense = self._pokemon["Defense"].values[0]
-       self._spatk = self._pokemon["sp.Atk"].values[0]
-       self._spdef = self._pokemon["Sp.Def"].values[0]
-       self._speed = self._pokemon["Speed"].values[0]
-       self._generation = self._pokemon["Generation"].values[0]
-       self._legendary = self._pokemon["Legendary"].values[0]
+        self._pokemon = self._file. sample()
+        self._number = self._pokemon["#"]. values[0]
+        self._name = self._pokemon["Name"]. values[0]
+        self._type1 = self._pokemon["Type 1"]. values[0]
+        self._type2 = self._pokemon["Type 2"].values[0]
+        self._total = self._pokemon["Total"].values[0]
+        self._hp = self._pokemon["hp"].values[0]
+        self._attack = self._pokemon["Attack"].values[0]
+        self._defense = self._pokemon["Defense"].values[0]
+        self._spatk = self._pokemon["Sp.Atk"].values[0]
+        self._spdef = self._pokemon["Sp.Def"].values[0]
+        self._speed = self._pokemon["Speed"].values[0]
+        self._generation = self._pokemon["Generation"].values[0]
+        self._legendary = self._pokemon["Legendary"].values[0]
 
     def getPokemon(self):
        return self._pokemon
 
     def getNumber(self):
        return self._number
 
@@ -66,15 +66,15 @@
 
     def getDefense(self):
         return self._defense
 
     def getSpAtk(self):
         return self._spatk
 
-    def getspdef(self):
+    def getSpdef(self):
         return self._spdef
 
     def getSpeed(self):
         return self._speed
 
     def getGeneration(self):
         return self._generation
```


# Comparing `tmp/charzr_lib-1.0.4.tar.gz` & `tmp/charzr_lib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charzr_lib-1.0.4.tar", last modified: Wed May  8 03:06:25 2024, max compression
+gzip compressed data, was "charzr_lib-1.0.5.tar", last modified: Wed May  8 03:27:19 2024, max compression
```

## Comparing `charzr_lib-1.0.4.tar` & `charzr_lib-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:25.138156 charzr_lib-1.0.4/
--rw-rw-rw-   0        0        0      316 2024-05-08 03:06:25.135228 charzr_lib-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:24.984878 charzr_lib-1.0.4/charzr_lib/
--rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.4/charzr_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.4/charzr_lib/pokemon.csv
--rw-rw-rw-   0        0        0      812 2024-05-08 03:05:58.000000 charzr_lib-1.0.4/charzr_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:06:25.131323 charzr_lib-1.0.4/charzr_lib.egg-info/
--rw-rw-rw-   0        0        0      316 2024-05-08 03:06:23.000000 charzr_lib-1.0.4/charzr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-08 03:06:24.000000 charzr_lib-1.0.4/charzr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 03:06:23.000000 charzr_lib-1.0.4/charzr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 03:06:23.000000 charzr_lib-1.0.4/charzr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 03:06:23.000000 charzr_lib-1.0.4/charzr_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 03:06:25.138156 charzr_lib-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      454 2024-05-08 03:05:58.000000 charzr_lib-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:27:19.215009 charzr_lib-1.0.5/
+-rw-rw-rw-   0        0        0      316 2024-05-08 03:27:19.212078 charzr_lib-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 03:27:19.108591 charzr_lib-1.0.5/charzr_lib/
+-rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.5/charzr_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.5/charzr_lib/pokemon.csv
+-rw-rw-rw-   0        0        0     1969 2024-05-08 03:26:28.000000 charzr_lib-1.0.5/charzr_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:27:19.209149 charzr_lib-1.0.5/charzr_lib.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:27:19.215984 charzr_lib-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      454 2024-05-08 03:27:15.000000 charzr_lib-1.0.5/setup.py
```

### Comparing `charzr_lib-1.0.4/README.md` & `charzr_lib-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.4/charzr_lib/pokemon.csv` & `charzr_lib-1.0.5/charzr_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.4/charzr_lib/random_pokemon.py` & `charzr_lib-1.0.5/charzr_lib/random_pokemon.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,22 +12,71 @@
         self._type1 = None
 
     def generate_random(self):
        self._pokemon = self._file. sample()
        self._number = self._pokemon["#"]. values[0]
        self._name = self._pokemon["Name"]. values[0]
        self._type1 = self._pokemon["Type 1"]. values[0]
+       self._type2 = self._pokemon["Type 2"].values[0]
+       self._total = self._pokemon["Total"].values[0]
+       self._hp = self._pokemon["hp"].values[0]
+       self._attack = self._pokemon["Attack"].values[0]
+       self._defense = self._pokemon["Defense"].values[0]
+       self._spatk = self._pokemon["sp.Atk"].values[0]
+       self._spdef = self._pokemon["Sp.Def"].values[0]
+       self._speed = self._pokemon["Speed"].values[0]
+       self._generation = self._pokemon["Generation"].values[0]
+       self._legendary = self._pokemon["Legendary"].values[0]
 
     def getPokemon(self):
        return self._pokemon
 
     def getNumber(self):
        return self._number
 
     def getName(self):
         return self._name
 
     def getType1(self):
         return self._type1
 
 
+    def getType2(self):
+        return self._type2
+
+
+    def getTotal(self):
+        return self._total
+
+
+    def getHp(self):
+        return self._hp
+
+    def getAttack(self):
+        return self._attack
+
+    def getDefense(self):
+        return self._defense
+
+    def getSpAtk(self):
+        return self._spatk
+
+    def getspdef(self):
+        return self._spdef
+
+    def getSpeed(self):
+        return self._speed
+
+    def getGeneration(self):
+        return self._generation
+
+    def getLegendary(self):
+        return self._legendary
+
+
+
+
+
+
+
+
```


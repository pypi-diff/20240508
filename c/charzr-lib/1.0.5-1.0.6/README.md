# Comparing `tmp/charzr_lib-1.0.5.tar.gz` & `tmp/charzr_lib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charzr_lib-1.0.5.tar", last modified: Wed May  8 03:27:19 2024, max compression
+gzip compressed data, was "charzr_lib-1.0.6.tar", last modified: Wed May  8 03:44:45 2024, max compression
```

## Comparing `charzr_lib-1.0.5.tar` & `charzr_lib-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 03:27:19.215009 charzr_lib-1.0.5/
--rw-rw-rw-   0        0        0      316 2024-05-08 03:27:19.212078 charzr_lib-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 03:27:19.108591 charzr_lib-1.0.5/charzr_lib/
--rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.5/charzr_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.5/charzr_lib/pokemon.csv
--rw-rw-rw-   0        0        0     1969 2024-05-08 03:26:28.000000 charzr_lib-1.0.5/charzr_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:27:19.209149 charzr_lib-1.0.5/charzr_lib.egg-info/
--rw-rw-rw-   0        0        0      316 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 03:27:18.000000 charzr_lib-1.0.5/charzr_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 03:27:19.215984 charzr_lib-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      454 2024-05-08 03:27:15.000000 charzr_lib-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:44:45.920518 charzr_lib-1.0.6/
+-rw-rw-rw-   0        0        0      316 2024-05-08 03:44:45.914660 charzr_lib-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-08 00:49:10.000000 charzr_lib-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 03:44:45.793600 charzr_lib-1.0.6/charzr_lib/
+-rw-rw-rw-   0        0        0       43 2024-05-08 00:16:26.000000 charzr_lib-1.0.6/charzr_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 charzr_lib-1.0.6/charzr_lib/pokemon.csv
+-rw-rw-rw-   0        0        0     2258 2024-05-08 03:42:57.000000 charzr_lib-1.0.6/charzr_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:44:45.909779 charzr_lib-1.0.6/charzr_lib.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 03:44:44.000000 charzr_lib-1.0.6/charzr_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:44:45.921495 charzr_lib-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      454 2024-05-08 03:42:57.000000 charzr_lib-1.0.6/setup.py
```

### Comparing `charzr_lib-1.0.5/README.md` & `charzr_lib-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.5/charzr_lib/pokemon.csv` & `charzr_lib-1.0.6/charzr_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `charzr_lib-1.0.5/charzr_lib/random_pokemon.py` & `charzr_lib-1.0.6/charzr_lib/random_pokemon.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 
     def __init__(self):
         self._file = pd.read_csv(RandomPokemon.FILE_PATH)
         self._pokemon = None
         self._number = None
         self._name = None
         self._type1 = None
+        self._type2 = None
+        self._total = None
+        self._hp = None
+        self._attack = None
+        self._defense = None
+        self._spatk = None
+        self._spdef = None
+        self._speed = None
+        self._generation = None
+        self._legendary = None
 
     def generate_random(self):
        self._pokemon = self._file. sample()
        self._number = self._pokemon["#"]. values[0]
        self._name = self._pokemon["Name"]. values[0]
        self._type1 = self._pokemon["Type 1"]. values[0]
        self._type2 = self._pokemon["Type 2"].values[0]
```


# Comparing `tmp/chrmnder_lib-1.0.0.tar.gz` & `tmp/chrmnder_lib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrmnder_lib-1.0.0.tar", last modified: Wed May  8 06:45:18 2024, max compression
+gzip compressed data, was "chrmnder_lib-1.0.1.tar", last modified: Wed May  8 07:11:10 2024, max compression
```

## Comparing `chrmnder_lib-1.0.0.tar` & `chrmnder_lib-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:45:18.766507 chrmnder_lib-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:45:18.663997 chrmnder_lib-1.0.0/Chrmnder_lib/
--rw-rw-rw-   0        0        0       41 2024-05-08 06:31:49.000000 chrmnder_lib-1.0.0/Chrmnder_lib/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 chrmnder_lib-1.0.0/Chrmnder_lib/pokemon.csv
--rw-rw-rw-   0        0        0     2259 2024-05-08 06:31:02.000000 chrmnder_lib-1.0.0/Chrmnder_lib/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:45:18.759675 chrmnder_lib-1.0.0/Chrmnder_lib.egg-info/
--rw-rw-rw-   0        0        0      318 2024-05-08 06:45:17.000000 chrmnder_lib-1.0.0/Chrmnder_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-08 06:45:17.000000 chrmnder_lib-1.0.0/Chrmnder_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:45:17.000000 chrmnder_lib-1.0.0/Chrmnder_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-08 06:45:17.000000 chrmnder_lib-1.0.0/Chrmnder_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-08 06:45:17.000000 chrmnder_lib-1.0.0/Chrmnder_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      318 2024-05-08 06:45:18.762607 chrmnder_lib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      992 2024-05-08 06:33:50.000000 chrmnder_lib-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 06:45:18.767485 chrmnder_lib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      460 2024-05-08 06:44:50.000000 chrmnder_lib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:11:10.278702 chrmnder_lib-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-08 07:11:10.197670 chrmnder_lib-1.0.1/Chrmnder_lib/
+-rw-rw-rw-   0        0        0       41 2024-05-08 06:31:49.000000 chrmnder_lib-1.0.1/Chrmnder_lib/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 chrmnder_lib-1.0.1/Chrmnder_lib/pokemon.csv
+-rw-rw-rw-   0        0        0     2259 2024-05-08 07:10:42.000000 chrmnder_lib-1.0.1/Chrmnder_lib/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:11:10.269916 chrmnder_lib-1.0.1/Chrmnder_lib.egg-info/
+-rw-rw-rw-   0        0        0      318 2024-05-08 07:11:09.000000 chrmnder_lib-1.0.1/Chrmnder_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-08 07:11:09.000000 chrmnder_lib-1.0.1/Chrmnder_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:11:09.000000 chrmnder_lib-1.0.1/Chrmnder_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 07:11:09.000000 chrmnder_lib-1.0.1/Chrmnder_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-08 07:11:09.000000 chrmnder_lib-1.0.1/Chrmnder_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      318 2024-05-08 07:11:10.273823 chrmnder_lib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      992 2024-05-08 06:33:50.000000 chrmnder_lib-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:11:10.279679 chrmnder_lib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      460 2024-05-08 07:10:42.000000 chrmnder_lib-1.0.1/setup.py
```

### Comparing `chrmnder_lib-1.0.0/Chrmnder_lib/pokemon.csv` & `chrmnder_lib-1.0.1/Chrmnder_lib/pokemon.csv`

 * *Files identical despite different names*

### Comparing `chrmnder_lib-1.0.0/Chrmnder_lib/random_pokemon.py` & `chrmnder_lib-1.0.1/Chrmnder_lib/random_pokemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,27 +54,27 @@
         return self._type2
 
 
     def getTotal(self):
         return self._total
 
 
-    def getHP(self):
+    def getHp(self):
         return self._hp
 
     def getAttack(self):
         return self._attack
 
     def getDefense(self):
         return self._defense
 
-    def getSpAtk(self):
+    def getSpatk(self):
         return self._spatk
 
-    def getSpDef(self):
+    def getSpdef(self):
         return self._spdef
 
     def getSpeed(self):
         return self._speed
 
     def getGeneration(self):
         return self._generation
```

### Comparing `chrmnder_lib-1.0.0/README.md` & `chrmnder_lib-1.0.1/README.md`

 * *Files identical despite different names*


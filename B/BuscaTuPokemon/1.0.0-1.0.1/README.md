# Comparing `tmp/BuscaTuPokemon-1.0.0.tar.gz` & `tmp/buscatupokemon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buscatupokemon-1.0.0.tar", last modified: Thu May  2 20:42:51 2024, max compression
+gzip compressed data, was "buscatupokemon-1.0.1.tar", last modified: Wed May  8 05:49:13 2024, max compression
```

## Comparing `BuscaTuPokemon-1.0.0.tar` & `buscatupokemon-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:51.962387 buscatupokemon-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:51.856580 buscatupokemon-1.0.0/BuscaTuPokemon/
--rw-rw-rw-   0        0        0       45 2024-05-02 20:32:04.000000 buscatupokemon-1.0.0/BuscaTuPokemon/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 buscatupokemon-1.0.0/BuscaTuPokemon/pokemon.csv
--rw-rw-rw-   0        0        0      822 2024-05-02 20:42:33.000000 buscatupokemon-1.0.0/BuscaTuPokemon/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:51.940913 buscatupokemon-1.0.0/BuscaTuPokemon.egg-info/
--rw-rw-rw-   0        0        0      288 2024-05-02 20:42:50.000000 buscatupokemon-1.0.0/BuscaTuPokemon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-02 20:42:51.000000 buscatupokemon-1.0.0/BuscaTuPokemon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 20:42:50.000000 buscatupokemon-1.0.0/BuscaTuPokemon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-02 20:42:50.000000 buscatupokemon-1.0.0/BuscaTuPokemon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-02 20:42:50.000000 buscatupokemon-1.0.0/BuscaTuPokemon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      288 2024-05-02 20:42:51.946767 buscatupokemon-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2024-05-01 04:42:16.000000 buscatupokemon-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 20:42:51.963363 buscatupokemon-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      518 2024-05-01 04:42:16.000000 buscatupokemon-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:49:13.169374 buscatupokemon-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-08 05:49:13.022932 buscatupokemon-1.0.1/BuscaTuPokemon/
+-rw-rw-rw-   0        0        0       45 2024-05-02 20:32:04.000000 buscatupokemon-1.0.1/BuscaTuPokemon/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 buscatupokemon-1.0.1/BuscaTuPokemon/pokemon.csv
+-rw-rw-rw-   0        0        0     2260 2024-05-08 05:48:22.000000 buscatupokemon-1.0.1/BuscaTuPokemon/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-08 05:49:13.164496 buscatupokemon-1.0.1/BuscaTuPokemon.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-05-08 05:49:11.000000 buscatupokemon-1.0.1/BuscaTuPokemon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-08 05:49:11.000000 buscatupokemon-1.0.1/BuscaTuPokemon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 05:49:11.000000 buscatupokemon-1.0.1/BuscaTuPokemon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 05:49:11.000000 buscatupokemon-1.0.1/BuscaTuPokemon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-08 05:49:11.000000 buscatupokemon-1.0.1/BuscaTuPokemon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      288 2024-05-08 05:49:13.166446 buscatupokemon-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1039 2024-05-01 04:42:16.000000 buscatupokemon-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-08 05:49:13.170351 buscatupokemon-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      518 2024-05-08 05:48:22.000000 buscatupokemon-1.0.1/setup.py
```

### Comparing `buscatupokemon-1.0.0/BuscaTuPokemon/pokemon.csv` & `buscatupokemon-1.0.1/BuscaTuPokemon/pokemon.csv`

 * *Files identical despite different names*

### Comparing `buscatupokemon-1.0.0/README.md` & `buscatupokemon-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `buscatupokemon-1.0.0/setup.py` & `buscatupokemon-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 
     name='BuscaTuPokemon',
-    version='1.0.0',
+    version='1.0.1',
     author= 'Milton Angel',
     author_email='milton_ac@tesch.edu.mx',
     description='Es una libreria la cual permitira generar un pokemon aleatorio',
     packages= ['BuscaTuPokemon'],
     package_data={'BuscaTuPokemon': ['pokemon.csv']},
     install_requires=['pandas',
                       'twine',
```


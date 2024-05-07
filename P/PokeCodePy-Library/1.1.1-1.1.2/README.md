# Comparing `tmp/pokecodepy_library-1.1.1.tar.gz` & `tmp/pokecodepy_library-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokecodepy_library-1.1.1.tar", last modified: Thu May  2 22:03:43 2024, max compression
+gzip compressed data, was "pokecodepy_library-1.1.2.tar", last modified: Tue May  7 00:52:40 2024, max compression
```

## Comparing `pokecodepy_library-1.1.1.tar` & `pokecodepy_library-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 22:03:43.441920 pokecodepy_library-1.1.1/
--rw-rw-rw-   0        0        0      316 2024-05-02 22:03:43.436795 pokecodepy_library-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 22:03:43.386173 pokecodepy_library-1.1.1/PokeCodePy_Library/
--rw-rw-rw-   0        0        0       55 2024-05-02 03:24:01.000000 pokecodepy_library-1.1.1/PokeCodePy_Library/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 11:51:28.000000 pokecodepy_library-1.1.1/PokeCodePy_Library/pokemon.csv
--rw-rw-rw-   0        0        0      806 2024-05-02 02:12:24.000000 pokecodepy_library-1.1.1/PokeCodePy_Library/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-05-02 22:03:43.434424 pokecodepy_library-1.1.1/PokeCodePy_Library.egg-info/
--rw-rw-rw-   0        0        0      316 2024-05-02 22:03:43.000000 pokecodepy_library-1.1.1/PokeCodePy_Library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-05-02 22:03:43.000000 pokecodepy_library-1.1.1/PokeCodePy_Library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 22:03:43.000000 pokecodepy_library-1.1.1/PokeCodePy_Library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-02 22:03:43.000000 pokecodepy_library-1.1.1/PokeCodePy_Library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-02 22:03:43.000000 pokecodepy_library-1.1.1/PokeCodePy_Library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1017 2024-05-02 01:51:47.000000 pokecodepy_library-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 22:03:43.443925 pokecodepy_library-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-02 22:01:52.000000 pokecodepy_library-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:52:40.297574 pokecodepy_library-1.1.2/
+-rw-rw-rw-   0        0        0      316 2024-05-07 00:52:40.291409 pokecodepy_library-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-07 00:52:40.227969 pokecodepy_library-1.1.2/PokeCodePy_Library/
+-rw-rw-rw-   0        0        0       55 2024-05-02 03:24:01.000000 pokecodepy_library-1.1.2/PokeCodePy_Library/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 11:51:28.000000 pokecodepy_library-1.1.2/PokeCodePy_Library/pokemon.csv
+-rw-rw-rw-   0        0        0     2443 2024-05-07 00:52:08.000000 pokecodepy_library-1.1.2/PokeCodePy_Library/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-05-07 00:52:40.287322 pokecodepy_library-1.1.2/PokeCodePy_Library.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-05-07 00:52:39.000000 pokecodepy_library-1.1.2/PokeCodePy_Library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-05-07 00:52:40.000000 pokecodepy_library-1.1.2/PokeCodePy_Library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 00:52:39.000000 pokecodepy_library-1.1.2/PokeCodePy_Library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-07 00:52:39.000000 pokecodepy_library-1.1.2/PokeCodePy_Library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-07 00:52:39.000000 pokecodepy_library-1.1.2/PokeCodePy_Library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1005 2024-05-06 22:33:56.000000 pokecodepy_library-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-07 00:52:40.298661 pokecodepy_library-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-07 00:52:08.000000 pokecodepy_library-1.1.2/setup.py
```

### Comparing `pokecodepy_library-1.1.1/PokeCodePy_Library/pokemon.csv` & `pokecodepy_library-1.1.2/PokeCodePy_Library/pokemon.csv`

 * *Files identical despite different names*

### Comparing `pokecodepy_library-1.1.1/README.md` & `pokecodepy_library-1.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Pokemon_Library
- Pokemon_Library es una biblioteca de Python que te permite trabajar con datos de Pokémon.
+# PokeCodePy_Library
+ Es una biblioteca de Python que nos permite trabajar con datos de Pokémon.
  ## Instalación
  Puedes instalar la biblioteca usando pip install PokeCodePy_Library
  ## Uso
  Aquí hay un ejemplo de cómo puedes usar la biblioteca para obtener información sobre Pokémon aleatorios:
  python
  from Pokemon_Library import RandomPokemon
  # Crear una instancia de RandomPokemon
```


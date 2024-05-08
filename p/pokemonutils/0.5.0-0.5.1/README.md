# Comparing `tmp/pokemonutils-0.5.0.tar.gz` & `tmp/pokemonutils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokemonutils-0.5.0.tar", max compression
+gzip compressed data, was "pokemonutils-0.5.1.tar", max compression
```

## Comparing `pokemonutils-0.5.0.tar` & `pokemonutils-0.5.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1116 2024-05-08 00:34:16.299636 pokemonutils-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     2137 2024-05-08 00:29:39.911869 pokemonutils-0.5.0/README.md
--rw-r--r--   0        0        0       33 2024-05-08 00:58:36.537064 pokemonutils-0.5.0/pokemonutils/__init__.py
--rw-r--r--   0        0        0     1628 2024-05-08 00:34:42.447516 pokemonutils-0.5.0/pokemonutils/pokemon_utils.py
--rw-r--r--   0        0        0      403 2024-05-08 01:03:14.085104 pokemonutils-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 pokemonutils-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1116 2024-05-08 00:34:16.299636 pokemonutils-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     2132 2024-05-08 01:10:47.425310 pokemonutils-0.5.1/README.md
+-rw-r--r--   0        0        0       62 2024-05-08 01:09:56.485380 pokemonutils-0.5.1/pokemonutils/__init__.py
+-rw-r--r--   0        0        0     1628 2024-05-08 00:34:42.447516 pokemonutils-0.5.1/pokemonutils/pokemon_utils.py
+-rw-r--r--   0        0        0      403 2024-05-08 01:10:27.413338 pokemonutils-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 pokemonutils-0.5.1/PKG-INFO
```

### Comparing `pokemonutils-0.5.0/LICENSE.txt` & `pokemonutils-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pokemonutils-0.5.0/README.md` & `pokemonutils-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 
 This class has 3 parameters: pokemon, region, and language. The pokemon value can either be the pokemon's name, like ditto, or it can be its national dex number, like 132 for ditto. You can find a list of pokemon national dex numbers at [Bulbapedia].(https://bulbapedia.bulbagarden.net/wiki/List_of_Pok%C3%A9mon_by_National_Pok%C3%A9dex_number)
 
 Example:
 
 ```
 #With name
-ditto = pokemon_utils.Pokemon("ditto", "sword", "en")
+ditto = pokemonutils.Pokemon("ditto", "sword", "en")
 
 #With number
-ditto = pokemon_utils.Pokemon(132, "sword", "en")
+ditto = pokemonutils.Pokemon(132, "sword", "en")
 ```
 
 I don't really know all the abbreviations of the languages, so you have to look that up, sorry.
 
 ### getPokedexEntry
 This function allows you to get the pokedex entry for the pokemon chosen in the chosen region with the language.
 
 Example:
 
 ```
 #Setup class
-ditto = pokemon_utils.Pokemon("ditto", "sword", "en")
+ditto = pokemonutils.Pokemon("ditto", "sword", "en")
 
 #Get the pokedex entry
 print(ditto.getPokedexEntry())
 ```
 
 Output:
 
@@ -43,15 +43,15 @@
 ### getTypes
 This one outputs a dictionary of the types of the pokemon. If the pokemon only has 1 type, type2 will output None.
 
 Example:
 
 ```
 #Setup class
-ditto = pokemon_utils.Pokemon(132, "sword", "en")
+ditto = pokemonutils.Pokemon(132, "sword", "en")
 
 #Get the types
 print(ditto.getTypes())
 ```
 
 Output:
 
@@ -65,15 +65,15 @@
 ### getAbilities
 This one outputs a dictionary of the abilities of the pokemon. The hidden ability of the pokemon will have a key of "hidden-ability" and the other abilities will be "ability1" or "ability2".
 
 Example:
 
 ```
 #Setup class
-ditto = pokemon_utils.Pokemon("ditto", "sword", "en")
+ditto = pokemonutils.Pokemon("ditto", "sword", "en")
 
 #Get the abilities
 print(ditto.getAbilities())
 ```
 
 Output:
```

### Comparing `pokemonutils-0.5.0/pokemonutils/pokemon_utils.py` & `pokemonutils-0.5.1/pokemonutils/pokemon_utils.py`

 * *Files identical despite different names*

### Comparing `pokemonutils-0.5.0/PKG-INFO` & `pokemonutils-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokemonutils
-Version: 0.5.0
+Version: 0.5.1
 Summary: A simple way to get Pokemon data
 Keywords: pokemon,data,api
 Author: Oscar F
 Author-email: 13097554-falconosc@users.noreply.replit.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -22,30 +22,30 @@
 
 This class has 3 parameters: pokemon, region, and language. The pokemon value can either be the pokemon's name, like ditto, or it can be its national dex number, like 132 for ditto. You can find a list of pokemon national dex numbers at [Bulbapedia].(https://bulbapedia.bulbagarden.net/wiki/List_of_Pok%C3%A9mon_by_National_Pok%C3%A9dex_number)
 
 Example:
 
 ```
 #With name
-ditto = pokemon_utils.Pokemon("ditto", "sword", "en")
+ditto = pokemonutils.Pokemon("ditto", "sword", "en")
 
 #With number
-ditto = pokemon_utils.Pokemon(132, "sword", "en")
+ditto = pokemonutils.Pokemon(132, "sword", "en")
 ```
 
 I don't really know all the abbreviations of the languages, so you have to look that up, sorry.
 
 ### getPokedexEntry
 This function allows you to get the pokedex entry for the pokemon chosen in the chosen region with the language.
 
 Example:
 
 ```
 #Setup class
-ditto = pokemon_utils.Pokemon("ditto", "sword", "en")
+ditto = pokemonutils.Pokemon("ditto", "sword", "en")
 
 #Get the pokedex entry
 print(ditto.getPokedexEntry())
 ```
 
 Output:
 
@@ -56,15 +56,15 @@
 ### getTypes
 This one outputs a dictionary of the types of the pokemon. If the pokemon only has 1 type, type2 will output None.
 
 Example:
 
 ```
 #Setup class
-ditto = pokemon_utils.Pokemon(132, "sword", "en")
+ditto = pokemonutils.Pokemon(132, "sword", "en")
 
 #Get the types
 print(ditto.getTypes())
 ```
 
 Output:
 
@@ -78,15 +78,15 @@
 ### getAbilities
 This one outputs a dictionary of the abilities of the pokemon. The hidden ability of the pokemon will have a key of "hidden-ability" and the other abilities will be "ability1" or "ability2".
 
 Example:
 
 ```
 #Setup class
-ditto = pokemon_utils.Pokemon("ditto", "sword", "en")
+ditto = pokemonutils.Pokemon("ditto", "sword", "en")
 
 #Get the abilities
 print(ditto.getAbilities())
 ```
 
 Output:
```


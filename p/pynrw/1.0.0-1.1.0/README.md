# Comparing `tmp/pynrw-1.0.0.tar.gz` & `tmp/pynrw-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrw-1.0.0.tar", last modified: Sun Apr 28 21:31:34 2024, max compression
+gzip compressed data, was "pynrw-1.1.0.tar", last modified: Tue May  7 20:56:33 2024, max compression
```

## Comparing `pynrw-1.0.0.tar` & `pynrw-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:31:34.109541 pynrw-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-28 21:31:24.000000 pynrw-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-28 21:31:34.109541 pynrw-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-28 21:31:24.000000 pynrw-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:31:34.101541 pynrw-1.0.0/nrw/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:31:34.105541 pynrw-1.0.0/nrw/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/algorithms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/algorithms/_searching.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/algorithms/_searching.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/algorithms/_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/algorithms/_sorting.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/algorithms/_traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/algorithms/_traversal.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:31:34.105541 pynrw-1.0.0/nrw/datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_binary_search_tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_binary_tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_comparable_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_edge.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_graph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_queue.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_stack.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/datastructures/_vertex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 21:31:24.000000 pynrw-1.0.0/nrw/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 21:31:34.109541 pynrw-1.0.0/pynrw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-28 21:31:34.000000 pynrw-1.0.0/pynrw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-28 21:31:34.000000 pynrw-1.0.0/pynrw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 21:31:34.000000 pynrw-1.0.0/pynrw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-28 21:31:34.000000 pynrw-1.0.0/pynrw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-28 21:31:34.000000 pynrw-1.0.0/pynrw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-28 21:31:24.000000 pynrw-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 21:31:34.109541 pynrw-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:56:33.587635 pynrw-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 20:56:24.000000 pynrw-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-07 20:56:33.587635 pynrw-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-05-07 20:56:24.000000 pynrw-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:56:33.579635 pynrw-1.1.0/nrw/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:56:33.579635 pynrw-1.1.0/nrw/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/algorithms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/algorithms/_searching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/algorithms/_searching.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/algorithms/_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/algorithms/_sorting.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/algorithms/_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/algorithms/_traversal.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:56:33.583635 pynrw-1.1.0/nrw/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_binary_search_tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_binary_tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_comparable_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_edge.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_graph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_queue.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_stack.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/datastructures/_vertex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:56:24.000000 pynrw-1.1.0/nrw/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:56:33.583635 pynrw-1.1.0/pynrw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-07 20:56:33.000000 pynrw-1.1.0/pynrw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-07 20:56:33.000000 pynrw-1.1.0/pynrw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:56:33.000000 pynrw-1.1.0/pynrw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 20:56:33.000000 pynrw-1.1.0/pynrw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 20:56:33.000000 pynrw-1.1.0/pynrw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-07 20:56:24.000000 pynrw-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:56:33.587635 pynrw-1.1.0/setup.cfg
```

### Comparing `pynrw-1.0.0/LICENSE` & `pynrw-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/PKG-INFO` & `pynrw-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.0.0
+Version: 1.1.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
-Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung
+Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -62,17 +62,20 @@
 - [`BinaryTree`](/nrw/datastructures/_binary_tree.py)
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
 - [`Vertex`](/nrw/datastructures/_vertex.py)
 - [`Edge`](/nrw/datastructures/_edge.py)
 - [`Graph`](/nrw/datastructures/_graph.py)
 
 Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d.h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
+
 Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein `TypeVar`(<https://docs.python.org/3/library/typing.html#typing.TypeVar>) `ComparableContentT` zur Verfügung.
 
-Außerdem sind (triviale) Optimierungen vorgenommen worden:
+Außerdem implementieren die linearen Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht.
+
+Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
 
 Zusätzlich enthält dieses Package nützliche Funktionen zum Sortieren, Suchen und Traversiern, zu finden in [`nrw.algorithms`](/nrw/algorithms/):
 
@@ -119,21 +122,23 @@
 from nrw.datastructures import List
 
 lst: List[int] = List()
 
 for i in range(0, 10, -1):
   lst.append(i)
 
-print(lst.content) # None
+print(lst.content)  # None
 lst.to_first()
-print(lst.content) # 9
+print(lst.content)  # 9
+print(lst)  # List(9 -> 8 -> 7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1 -> 0)
 
 sorted_lst: List[int] = quick_sort(lst)
 sorted_lst.to_first()
-print(sorted_lst.content) # 0
+print(sorted_lst.content)  # 0
+print(sorted_lst)  # List(0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9)
 ```
 
 ## Motivation
 
 Vereinfacht: Java, als Programmiersprache in der Bildung, ist eine schlechte Wahl, da ...
 
 - Java veraltet ist.
```

### Comparing `pynrw-1.0.0/README.md` & `pynrw-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,20 @@
 - [`BinaryTree`](/nrw/datastructures/_binary_tree.py)
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
 - [`Vertex`](/nrw/datastructures/_vertex.py)
 - [`Edge`](/nrw/datastructures/_edge.py)
 - [`Graph`](/nrw/datastructures/_graph.py)
 
 Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d.h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
+
 Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein `TypeVar`(<https://docs.python.org/3/library/typing.html#typing.TypeVar>) `ComparableContentT` zur Verfügung.
 
-Außerdem sind (triviale) Optimierungen vorgenommen worden:
+Außerdem implementieren die linearen Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht.
+
+Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
 
 Zusätzlich enthält dieses Package nützliche Funktionen zum Sortieren, Suchen und Traversiern, zu finden in [`nrw.algorithms`](/nrw/algorithms/):
 
@@ -84,21 +87,23 @@
 from nrw.datastructures import List
 
 lst: List[int] = List()
 
 for i in range(0, 10, -1):
   lst.append(i)
 
-print(lst.content) # None
+print(lst.content)  # None
 lst.to_first()
-print(lst.content) # 9
+print(lst.content)  # 9
+print(lst)  # List(9 -> 8 -> 7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1 -> 0)
 
 sorted_lst: List[int] = quick_sort(lst)
 sorted_lst.to_first()
-print(sorted_lst.content) # 0
+print(sorted_lst.content)  # 0
+print(sorted_lst)  # List(0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9)
 ```
 
 ## Motivation
 
 Vereinfacht: Java, als Programmiersprache in der Bildung, ist eine schlechte Wahl, da ...
 
 - Java veraltet ist.
```

### Comparing `pynrw-1.0.0/nrw/algorithms/__init__.py` & `pynrw-1.1.0/nrw/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/algorithms/__init__.pyi` & `pynrw-1.1.0/nrw/algorithms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/algorithms/_searching.py` & `pynrw-1.1.0/nrw/algorithms/_searching.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/algorithms/_sorting.py` & `pynrw-1.1.0/nrw/algorithms/_sorting.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/algorithms/_sorting.pyi` & `pynrw-1.1.0/nrw/algorithms/_sorting.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/algorithms/_traversal.py` & `pynrw-1.1.0/nrw/algorithms/_traversal.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/algorithms/_traversal.pyi` & `pynrw-1.1.0/nrw/algorithms/_traversal.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/__init__.py` & `pynrw-1.1.0/nrw/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/__init__.pyi` & `pynrw-1.1.0/nrw/datastructures/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_binary_search_tree.py` & `pynrw-1.1.0/nrw/datastructures/_binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_binary_search_tree.pyi` & `pynrw-1.1.0/nrw/datastructures/_binary_search_tree.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_binary_tree.py` & `pynrw-1.1.0/nrw/datastructures/_binary_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,19 +57,18 @@
         Sind `left_tree` und `right_tree` `None`, wird der entsprechende
         Teilbaum als leerer Binaerbaum eingefügt. So kann es also nie passieren,
         dass linke oder rechte Teilbäume `None` sind. Wenn der Parameter `content`
         `None` ist, wird ein leerer Binaerbaum erzeugt.
         """
         if content is None:
             self._node: _BTNode[_T] | None = None
-            return
-
-        self._node = _BTNode(content)
-        self._node._left = left_tree if left_tree is not None else BinaryTree()
-        self._node._right = right_tree if right_tree is not None else BinaryTree()
+        else:
+            self._node = _BTNode(content)
+            self._node._left = left_tree if left_tree is not None else BinaryTree()
+            self._node._right = right_tree if right_tree is not None else BinaryTree()
 
     @property
     def is_empty(self) -> bool:
         """Diese Anfrage liefert das Inhaltsobjekt des Binaerbaums. Wenn der Binaerbaum
         leer ist, wird `None` zurueckgegeben.
         """
         return self._node is None
```

### Comparing `pynrw-1.0.0/nrw/datastructures/_binary_tree.pyi` & `pynrw-1.1.0/nrw/datastructures/_binary_tree.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_comparable_content.py` & `pynrw-1.1.0/nrw/datastructures/_comparable_content.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_edge.py` & `pynrw-1.1.0/nrw/datastructures/_edge.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_edge.pyi` & `pynrw-1.1.0/nrw/datastructures/_edge.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_graph.py` & `pynrw-1.1.0/nrw/datastructures/_graph.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_graph.pyi` & `pynrw-1.1.0/nrw/datastructures/_graph.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_list.py` & `pynrw-1.1.0/nrw/datastructures/_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implementation der generischen Klasse `List[_T]`."""
 
 from __future__ import annotations
 
 __all__: Final[tuple[str]] = ("List",)
 
+from io import StringIO
 from typing import Final, Generic, TypeVar
 
 _T = TypeVar("_T")
 
 
 class _ListNode(Generic[_T]):
     __slots__: Final[tuple[str, str]] = ("_content", "_next_node")
@@ -59,14 +60,24 @@
 
     def __init__(self) -> None:
         """Eine leere Liste wird erzeugt."""
         self._first: _ListNode[_T] | None = None
         self._last: _ListNode[_T] | None = None
         self._current: _ListNode[_T] | None = None
 
+    def __str__(self) -> str:
+        with StringIO() as buffer:
+            buffer.write(f"{self.__class__.__name__}(")
+            temp: _ListNode[_T] | None = self._first
+            while temp is not self._last:
+                buffer.write(f"{temp.content} -> ")
+                temp = temp.next_node
+            buffer.write(f"{temp.content})")
+            return buffer.getvalue()
+
     @property
     def is_empty(self) -> bool:
         """Die Anfrage liefert den Wert `True`, wenn die Liste keine Objekte enthält,
         sonst liefert sie den Wert `False`.
         """
         return self._first is None
```

### Comparing `pynrw-1.0.0/nrw/datastructures/_list.pyi` & `pynrw-1.1.0/nrw/datastructures/_list.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/nrw/datastructures/_queue.py` & `pynrw-1.1.0/nrw/datastructures/_queue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implementation der generischen Klasse `Queue[_T]`."""
 
 from __future__ import annotations
 
 __all__: Final[tuple[str]] = ("Queue",)
 
+from io import StringIO
 from typing import Final, Generic, TypeVar
 
 _T = TypeVar("_T")
 
 
 class _QueueNode(Generic[_T]):
     __slots__: Final[tuple[str, str]] = ("_content", "_next_node")
@@ -46,14 +47,24 @@
     __hash__ = None  # type: ignore[assignment]
 
     def __init__(self) -> None:
         """Eine leere Schlange wird erzeugt."""
         self._head: _QueueNode[_T] | None = None
         self._tail: _QueueNode[_T] | None = None
 
+    def __str__(self) -> str:
+        with StringIO() as buffer:
+            buffer.write(f"{self.__class__.__name__}(")
+            temp: _QueueNode[_T] | None = self._head
+            while temp is not self._tail:
+                buffer.write(f"{temp.content} -> ")
+                temp = temp.next_node
+            buffer.write(f"{temp.content})")
+            return buffer.getvalue()
+
     @property
     def is_empty(self) -> bool:
         """Die Anfrage liefert den Wert `True`, wenn die Schlange keine Objekte enthält,
         sonst liefert sie den Wert `False`.
         """
         return self._head is None
```

### Comparing `pynrw-1.0.0/nrw/datastructures/_stack.py` & `pynrw-1.1.0/nrw/datastructures/_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implementation der generischen Klasse `Stack[_T]`."""
 
 from __future__ import annotations
 
 __all__: Final[tuple[str]] = ("Stack",)
 
+from io import StringIO
 from typing import Final, Generic, TypeVar
 
 _T = TypeVar("_T")
 
 
 class _StackNode(Generic[_T]):
     __slots__: Final[tuple[str, str]] = ("_content", "_next_node")
@@ -46,14 +47,24 @@
     __slots__: Final[tuple[str]] = ("_head",)
     __hash__ = None  # type: ignore[assignment]
 
     def __init__(self) -> None:
         """Ein leerer Stapel wird erzeugt."""
         self._head: _StackNode[_T] | None = None
 
+    def __str__(self) -> str:
+        with StringIO() as buffer:
+            buffer.write(f"{self.__class__.__name__}(")
+            temp: _StackNode[_T] | None = self._head
+            while temp is not None and temp.next_node is not None:
+                buffer.write(f"{temp.content} -> ")
+                temp = temp.next_node
+            buffer.write(f"{temp.content})")
+            return buffer.getvalue()
+
     @property
     def is_empty(self) -> bool:
         """Die Anfrage liefert den Wert `True`, wenn der Stapel keine Objekte enthält,
         sonst liefert sie den Wert `False`.
         """
         return self._head is None
```

### Comparing `pynrw-1.0.0/nrw/datastructures/_vertex.py` & `pynrw-1.1.0/nrw/datastructures/_vertex.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/pynrw.egg-info/PKG-INFO` & `pynrw-1.1.0/pynrw.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.0.0
+Version: 1.1.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
-Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung
+Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -62,17 +62,20 @@
 - [`BinaryTree`](/nrw/datastructures/_binary_tree.py)
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
 - [`Vertex`](/nrw/datastructures/_vertex.py)
 - [`Edge`](/nrw/datastructures/_edge.py)
 - [`Graph`](/nrw/datastructures/_graph.py)
 
 Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d.h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
+
 Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein `TypeVar`(<https://docs.python.org/3/library/typing.html#typing.TypeVar>) `ComparableContentT` zur Verfügung.
 
-Außerdem sind (triviale) Optimierungen vorgenommen worden:
+Außerdem implementieren die linearen Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht.
+
+Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
 
 Zusätzlich enthält dieses Package nützliche Funktionen zum Sortieren, Suchen und Traversiern, zu finden in [`nrw.algorithms`](/nrw/algorithms/):
 
@@ -119,21 +122,23 @@
 from nrw.datastructures import List
 
 lst: List[int] = List()
 
 for i in range(0, 10, -1):
   lst.append(i)
 
-print(lst.content) # None
+print(lst.content)  # None
 lst.to_first()
-print(lst.content) # 9
+print(lst.content)  # 9
+print(lst)  # List(9 -> 8 -> 7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1 -> 0)
 
 sorted_lst: List[int] = quick_sort(lst)
 sorted_lst.to_first()
-print(sorted_lst.content) # 0
+print(sorted_lst.content)  # 0
+print(sorted_lst)  # List(0 -> 1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> 8 -> 9)
 ```
 
 ## Motivation
 
 Vereinfacht: Java, als Programmiersprache in der Bildung, ist eine schlechte Wahl, da ...
 
 - Java veraltet ist.
```

### Comparing `pynrw-1.0.0/pynrw.egg-info/SOURCES.txt` & `pynrw-1.1.0/pynrw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynrw-1.0.0/pyproject.toml` & `pynrw-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   "nrw",
   "datastructures",
   "datenstrukturen",
   "algorithms",
   "algorithmen",
   "education",
   "bildung",
+  "abitur",
 ]
 readme = "README.md"
 authors = [{ name = "realshouzy" }]
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
@@ -94,15 +95,24 @@
 [[tool.mypy.overrides]]
 module = "tests.*"
 disallow_untyped_decorators = false
 disable_error_code = ["attr-defined"]
 
 [tool.ruff]
 lint.select = ["ALL"]
-lint.ignore = ["ANN101", "D205", "UP035", "UP036", "SLF001", "FBT001", "S101"]
+lint.ignore = [
+  "ANN101",
+  "D205",
+  "UP035",
+  "UP036",
+  "SLF001",
+  "FBT001",
+  "S101",
+  "PYI026",
+]
 lint.fixable = ["ALL"]
 lint.unfixable = []
 show-fixes = true
 target-version = "py312"
 line-length = 88
 
 [tool.ruff.lint.extend-per-file-ignores]
```


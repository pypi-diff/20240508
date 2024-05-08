# Comparing `tmp/ojax-2.0.0.tar.gz` & `tmp/ojax-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ojax-2.0.0.tar", last modified: Sun May  5 16:16:35 2024, max compression
+gzip compressed data, was "ojax-2.0.1.tar", last modified: Wed May  8 09:51:09 2024, max compression
```

## Comparing `ojax-2.0.0.tar` & `ojax-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-05 16:16:35.453082 ojax-2.0.0/
--rw-rw-r--   0 ys        (1000) ys        (1000)    11357 2024-05-04 19:05:49.000000 ojax-2.0.0/LICENSE
--rw-r--r--   0 ys        (1000) ys        (1000)     4266 2024-05-05 16:16:35.453082 ojax-2.0.0/PKG-INFO
-drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-05 16:16:35.453082 ojax-2.0.0/ojax/
--rw-rw-r--   0 ys        (1000) ys        (1000)      245 2024-05-05 16:13:02.000000 ojax-2.0.0/ojax/__init__.py
--rw-rw-r--   0 ys        (1000) ys        (1000)    11042 2024-05-05 16:13:02.000000 ojax-2.0.0/ojax/otree.py
--rw-rw-r--   0 ys        (1000) ys        (1000)     3818 2024-05-04 19:05:49.000000 ojax-2.0.0/ojax/pureclass.py
--rw-rw-r--   0 ys        (1000) ys        (1000)        0 2024-05-04 19:05:49.000000 ojax-2.0.0/ojax/py.typed
-drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-05 16:16:35.453082 ojax-2.0.0/ojax.egg-info/
--rw-r--r--   0 ys        (1000) ys        (1000)     4266 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/PKG-INFO
--rw-rw-r--   0 ys        (1000) ys        (1000)      285 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/SOURCES.txt
--rw-rw-r--   0 ys        (1000) ys        (1000)        1 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/dependency_links.txt
--rw-rw-r--   0 ys        (1000) ys        (1000)        4 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/requires.txt
--rw-rw-r--   0 ys        (1000) ys        (1000)        5 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/top_level.txt
--rw-rw-r--   0 ys        (1000) ys        (1000)      498 2024-05-04 19:05:49.000000 ojax-2.0.0/pyproject.toml
--rw-rw-r--   0 ys        (1000) ys        (1000)     3976 2024-05-05 14:48:35.000000 ojax-2.0.0/readme.rst
--rw-rw-r--   0 ys        (1000) ys        (1000)       38 2024-05-05 16:16:35.453082 ojax-2.0.0/setup.cfg
--rw-rw-r--   0 ys        (1000) ys        (1000)       96 2024-05-04 19:05:49.000000 ojax-2.0.0/setup.py
-drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-05 16:16:35.453082 ojax-2.0.0/tests/
--rw-rw-r--   0 ys        (1000) ys        (1000)     2611 2024-05-05 16:13:02.000000 ojax-2.0.0/tests/test_example.py
--rw-rw-r--   0 ys        (1000) ys        (1000)     5746 2024-05-05 16:13:02.000000 ojax-2.0.0/tests/test_ojax.py
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-08 09:51:09.041495 ojax-2.0.1/
+-rw-rw-r--   0 ys        (1000) ys        (1000)    11357 2024-05-04 19:05:49.000000 ojax-2.0.1/LICENSE
+-rw-r--r--   0 ys        (1000) ys        (1000)     4061 2024-05-08 09:51:09.041495 ojax-2.0.1/PKG-INFO
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-08 09:51:09.037495 ojax-2.0.1/ojax/
+-rw-rw-r--   0 ys        (1000) ys        (1000)      245 2024-05-08 09:43:31.000000 ojax-2.0.1/ojax/__init__.py
+-rw-rw-r--   0 ys        (1000) ys        (1000)    11042 2024-05-08 09:29:48.000000 ojax-2.0.1/ojax/otree.py
+-rw-rw-r--   0 ys        (1000) ys        (1000)     3818 2024-05-04 19:05:49.000000 ojax-2.0.1/ojax/pureclass.py
+-rw-rw-r--   0 ys        (1000) ys        (1000)        0 2024-05-04 19:05:49.000000 ojax-2.0.1/ojax/py.typed
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-08 09:51:09.041495 ojax-2.0.1/ojax.egg-info/
+-rw-r--r--   0 ys        (1000) ys        (1000)     4061 2024-05-08 09:51:08.000000 ojax-2.0.1/ojax.egg-info/PKG-INFO
+-rw-rw-r--   0 ys        (1000) ys        (1000)      285 2024-05-08 09:51:09.000000 ojax-2.0.1/ojax.egg-info/SOURCES.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)        1 2024-05-08 09:51:08.000000 ojax-2.0.1/ojax.egg-info/dependency_links.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)        4 2024-05-08 09:51:08.000000 ojax-2.0.1/ojax.egg-info/requires.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)        5 2024-05-08 09:51:08.000000 ojax-2.0.1/ojax.egg-info/top_level.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)      498 2024-05-04 19:05:49.000000 ojax-2.0.1/pyproject.toml
+-rw-rw-r--   0 ys        (1000) ys        (1000)     3771 2024-05-08 09:43:31.000000 ojax-2.0.1/readme.rst
+-rw-rw-r--   0 ys        (1000) ys        (1000)       38 2024-05-08 09:51:09.041495 ojax-2.0.1/setup.cfg
+-rw-rw-r--   0 ys        (1000) ys        (1000)       96 2024-05-04 19:05:49.000000 ojax-2.0.1/setup.py
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-08 09:51:09.041495 ojax-2.0.1/tests/
+-rw-rw-r--   0 ys        (1000) ys        (1000)     2611 2024-05-08 09:29:48.000000 ojax-2.0.1/tests/test_example.py
+-rw-rw-r--   0 ys        (1000) ys        (1000)     5746 2024-05-08 09:29:48.000000 ojax-2.0.1/tests/test_ojax.py
```

### Comparing `ojax-2.0.0/LICENSE` & `ojax-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ojax-2.0.0/PKG-INFO` & `ojax-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ojax
-Version: 2.0.0
+Version: 2.0.1
 Summary: An extension for modular JAX code.
 Author: Yuesong Shen
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/ysngshn/ojax
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -83,18 +83,14 @@
 However, none of them offers a perfect "JAX base class" that fulfills all of
 the desiderata below:
 
 * Simple to understand and use
 * Flexible custom classes for general JAX computation
 * Compatible with JAX and its functional paradigm
 
-`Simple Pytree`_ comes pretty close to this goal. However, its dataclass /
-non-dataclass initializations and ``mutable=True`` option can be confusing and
-it is not clear which should be the right choice.
-
 OJAX strives to define how a JAX base class should be. It provides a natural 
 way to structure custom JAX code and discourages users from common pitfalls.
 
 P.S.: the name "OJAX" is a chapeau-bas to `OCaml <https://ocaml.org>`_, an
 awesome functional programming language.
 
 How to code with OJAX
```

### Comparing `ojax-2.0.0/ojax/otree.py` & `ojax-2.0.1/ojax/otree.py`

 * *Files identical despite different names*

### Comparing `ojax-2.0.0/ojax/pureclass.py` & `ojax-2.0.1/ojax/pureclass.py`

 * *Files identical despite different names*

### Comparing `ojax-2.0.0/ojax.egg-info/PKG-INFO` & `ojax-2.0.1/ojax.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ojax
-Version: 2.0.0
+Version: 2.0.1
 Summary: An extension for modular JAX code.
 Author: Yuesong Shen
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/ysngshn/ojax
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -83,18 +83,14 @@
 However, none of them offers a perfect "JAX base class" that fulfills all of
 the desiderata below:
 
 * Simple to understand and use
 * Flexible custom classes for general JAX computation
 * Compatible with JAX and its functional paradigm
 
-`Simple Pytree`_ comes pretty close to this goal. However, its dataclass /
-non-dataclass initializations and ``mutable=True`` option can be confusing and
-it is not clear which should be the right choice.
-
 OJAX strives to define how a JAX base class should be. It provides a natural 
 way to structure custom JAX code and discourages users from common pitfalls.
 
 P.S.: the name "OJAX" is a chapeau-bas to `OCaml <https://ocaml.org>`_, an
 awesome functional programming language.
 
 How to code with OJAX
```

### Comparing `ojax-2.0.0/readme.rst` & `ojax-2.0.1/readme.rst`

 * *Files 9% similar despite different names*

```diff
@@ -71,18 +71,14 @@
 However, none of them offers a perfect "JAX base class" that fulfills all of
 the desiderata below:
 
 * Simple to understand and use
 * Flexible custom classes for general JAX computation
 * Compatible with JAX and its functional paradigm
 
-`Simple Pytree`_ comes pretty close to this goal. However, its dataclass /
-non-dataclass initializations and ``mutable=True`` option can be confusing and
-it is not clear which should be the right choice.
-
 OJAX strives to define how a JAX base class should be. It provides a natural 
 way to structure custom JAX code and discourages users from common pitfalls.
 
 P.S.: the name "OJAX" is a chapeau-bas to `OCaml <https://ocaml.org>`_, an
 awesome functional programming language.
 
 How to code with OJAX
```

### Comparing `ojax-2.0.0/tests/test_example.py` & `ojax-2.0.1/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `ojax-2.0.0/tests/test_ojax.py` & `ojax-2.0.1/tests/test_ojax.py`

 * *Files identical despite different names*


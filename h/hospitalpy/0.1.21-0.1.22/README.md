# Comparing `tmp/hospitalpy-0.1.21.tar.gz` & `tmp/hospitalpy-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hospitalpy-0.1.21.tar", last modified: Wed May  8 00:18:26 2024, max compression
+gzip compressed data, was "hospitalpy-0.1.22.tar", last modified: Wed May  8 00:45:57 2024, max compression
```

## Comparing `hospitalpy-0.1.21.tar` & `hospitalpy-0.1.22.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:18:26.140426 hospitalpy-0.1.21/
--rw-r--r--   0 michaelchary   (501) staff       (20)      360 2024-05-08 00:18:26.140254 hospitalpy-0.1.21/PKG-INFO
--rw-r--r--   0 michaelchary   (501) staff       (20)        5 2024-05-01 20:53:36.000000 hospitalpy-0.1.21/README.md
-drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:18:26.140077 hospitalpy-0.1.21/hospitalpy.egg-info/
--rw-r--r--   0 michaelchary   (501) staff       (20)      360 2024-05-08 00:18:26.000000 hospitalpy-0.1.21/hospitalpy.egg-info/PKG-INFO
--rw-r--r--   0 michaelchary   (501) staff       (20)      202 2024-05-08 00:18:26.000000 hospitalpy-0.1.21/hospitalpy.egg-info/SOURCES.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-08 00:18:26.000000 hospitalpy-0.1.21/hospitalpy.egg-info/dependency_links.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)       13 2024-05-08 00:18:26.000000 hospitalpy-0.1.21/hospitalpy.egg-info/requires.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-08 00:18:26.000000 hospitalpy-0.1.21/hospitalpy.egg-info/top_level.txt
--rw-r--r--   0 michaelchary   (501) staff       (20)      455 2024-05-08 00:18:18.000000 hospitalpy-0.1.21/pyproject.toml
--rw-r--r--   0 michaelchary   (501) staff       (20)       38 2024-05-08 00:18:26.140462 hospitalpy-0.1.21/setup.cfg
--rw-r--r--   0 michaelchary   (501) staff       (20)      492 2024-05-07 23:04:38.000000 hospitalpy-0.1.21/setup.py
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:45:57.302163 hospitalpy-0.1.22/
+-rw-r--r--   0 michaelchary   (501) staff       (20)     1074 2024-05-08 00:29:19.000000 hospitalpy-0.1.22/LICENSE
+-rw-r--r--   0 michaelchary   (501) staff       (20)     1618 2024-05-08 00:45:57.301990 hospitalpy-0.1.22/PKG-INFO
+-rw-r--r--   0 michaelchary   (501) staff       (20)        5 2024-05-01 20:53:36.000000 hospitalpy-0.1.22/README.md
+-rw-r--r--   0 michaelchary   (501) staff       (20)      527 2024-05-08 00:31:36.000000 hospitalpy-0.1.22/pyproject.toml
+-rw-r--r--   0 michaelchary   (501) staff       (20)       38 2024-05-08 00:45:57.302214 hospitalpy-0.1.22/setup.cfg
+-rw-r--r--   0 michaelchary   (501) staff       (20)      535 2024-05-08 00:36:46.000000 hospitalpy-0.1.22/setup.py
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:45:57.299974 hospitalpy-0.1.22/src/
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:45:57.301097 hospitalpy-0.1.22/src/hospitalpy/
+-rw-r--r--   0 michaelchary   (501) staff       (20)      760 2024-05-08 00:15:32.000000 hospitalpy-0.1.22/src/hospitalpy/Evaluator.py
+-rw-r--r--   0 michaelchary   (501) staff       (20)     4334 2024-05-08 00:15:32.000000 hospitalpy-0.1.22/src/hospitalpy/Tokenizer.py
+-rw-r--r--   0 michaelchary   (501) staff       (20)      249 2024-05-08 00:15:32.000000 hospitalpy-0.1.22/src/hospitalpy/__init__.py
+-rw-r--r--   0 michaelchary   (501) staff       (20)      159 2024-05-08 00:15:32.000000 hospitalpy-0.1.22/src/hospitalpy/config.py
+-rw-r--r--   0 michaelchary   (501) staff       (20)     1205 2024-05-08 00:15:32.000000 hospitalpy-0.1.22/src/hospitalpy/sandbox.py
+drwxr-xr-x   0 michaelchary   (501) staff       (20)        0 2024-05-08 00:45:57.301798 hospitalpy-0.1.22/src/hospitalpy.egg-info/
+-rw-r--r--   0 michaelchary   (501) staff       (20)     1618 2024-05-08 00:45:57.000000 hospitalpy-0.1.22/src/hospitalpy.egg-info/PKG-INFO
+-rw-r--r--   0 michaelchary   (501) staff       (20)      364 2024-05-08 00:45:57.000000 hospitalpy-0.1.22/src/hospitalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)        1 2024-05-08 00:45:57.000000 hospitalpy-0.1.22/src/hospitalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)       13 2024-05-08 00:45:57.000000 hospitalpy-0.1.22/src/hospitalpy.egg-info/requires.txt
+-rw-r--r--   0 michaelchary   (501) staff       (20)       11 2024-05-08 00:45:57.000000 hospitalpy-0.1.22/src/hospitalpy.egg-info/top_level.txt
```


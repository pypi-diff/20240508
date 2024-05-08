# Comparing `tmp/easyscience-0.0.1a0.tar.gz` & `tmp/easyscience-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyscience-0.0.1a0.tar", last modified: Wed Apr 17 09:16:27 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `easyscience-0.0.1a0.tar` & `easyscience-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,51 @@
-drwxr-xr-x   0 andrewsazonov   (503) staff       (20)        0 2024-04-17 09:16:27.872493 easyscience-0.0.1a0/
--rw-r--r--   0 andrewsazonov   (503) staff       (20)      131 2024-04-17 09:16:27.872299 easyscience-0.0.1a0/PKG-INFO
-drwxr-xr-x   0 andrewsazonov   (503) staff       (20)        0 2024-04-17 09:16:27.871549 easyscience-0.0.1a0/easyscience/
--rw-r--r--   0 andrewsazonov   (503) staff       (20)        0 2024-04-17 09:12:14.000000 easyscience-0.0.1a0/easyscience/__init__.py
-drwxr-xr-x   0 andrewsazonov   (503) staff       (20)        0 2024-04-17 09:16:27.872156 easyscience-0.0.1a0/easyscience.egg-info/
--rw-r--r--   0 andrewsazonov   (503) staff       (20)      131 2024-04-17 09:16:27.000000 easyscience-0.0.1a0/easyscience.egg-info/PKG-INFO
--rw-r--r--   0 andrewsazonov   (503) staff       (20)      178 2024-04-17 09:16:27.000000 easyscience-0.0.1a0/easyscience.egg-info/SOURCES.txt
--rw-r--r--   0 andrewsazonov   (503) staff       (20)        1 2024-04-17 09:16:27.000000 easyscience-0.0.1a0/easyscience.egg-info/dependency_links.txt
--rw-r--r--   0 andrewsazonov   (503) staff       (20)       12 2024-04-17 09:16:27.000000 easyscience-0.0.1a0/easyscience.egg-info/top_level.txt
--rw-r--r--   0 andrewsazonov   (503) staff       (20)      158 2024-04-17 09:16:19.000000 easyscience-0.0.1a0/pyproject.toml
--rw-r--r--   0 andrewsazonov   (503) staff       (20)       38 2024-04-17 09:16:27.872532 easyscience-0.0.1a0/setup.cfg
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/REDIRECT.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/__version__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Datasets/__init__.py
+-rw-r--r--   0        0        0    31311 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Datasets/xarray.py
+-rw-r--r--   0        0        0    17846 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Fitting/Constraints.py
+-rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Fitting/DFO_LS.py
+-rw-r--r--   0        0        0    17636 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Fitting/Fitting.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Fitting/__init__.py
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Fitting/bumps.py
+-rw-r--r--   0        0        0     8273 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Fitting/fitting_template.py
+-rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Fitting/lmfit.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Borg.py
+-rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Graph.py
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Groups.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Inferface.py
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/ObjectClasses.py
+-rw-r--r--   0        0        0    30140 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Variable.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/__init__.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/core.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/virtual.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Job/Analysis.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Job/Experiment.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Job/Job.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Job/Theory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Objects/Job/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/Exceptions.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/Logging.py
+-rw-r--r--   0        0        0    14417 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/UndoRedo.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/__init__.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/classTools.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/classUtils.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/decorators.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/string.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/typing.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/Hugger/Hugger.py
+-rw-r--r--   0        0        0    11169 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/Hugger/Property.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/Hugger/__init__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/io/__init__.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/io/dict.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/io/json.py
+-rw-r--r--   0        0        0    19384 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/io/star.py
+-rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/io/template.py
+-rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/Utils/io/xml.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/models/__init__.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 easyscience-0.6.0/src/easyscience/models/polynomial.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 easyscience-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 easyscience-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 easyscience-0.6.0/README.md
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 easyscience-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 easyscience-0.6.0/PKG-INFO
```


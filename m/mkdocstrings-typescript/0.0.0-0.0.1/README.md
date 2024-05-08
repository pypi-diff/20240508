# Comparing `tmp/mkdocstrings-typescript-0.0.0.tar.gz` & `tmp/mkdocstrings_typescript-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings-typescript-0.0.0.tar", last modified: Fri Nov 17 14:37:10 2023, max compression
+gzip compressed data, was "mkdocstrings_typescript-0.0.1.tar", last modified: Wed May  8 19:31:49 2024, max compression
```

## Comparing `mkdocstrings-typescript-0.0.0.tar` & `mkdocstrings_typescript-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,8 @@
-drwxr-xr-x   0 pawamoy   (1000) pawamoy   (1000)        0 2023-11-17 14:37:09.998674 mkdocstrings-typescript-0.0.0/
--rw-r--r--   0 pawamoy   (1000) pawamoy   (1000)      531 2023-11-17 14:37:09.998674 mkdocstrings-typescript-0.0.0/PKG-INFO
--rw-r--r--   0 pawamoy   (1000) pawamoy   (1000)      224 2023-11-17 14:37:01.000000 mkdocstrings-typescript-0.0.0/README.md
-drwxr-xr-x   0 pawamoy   (1000) pawamoy   (1000)        0 2023-11-17 14:37:09.998674 mkdocstrings-typescript-0.0.0/mkdocstrings_typescript.egg-info/
--rw-r--r--   0 pawamoy   (1000) pawamoy   (1000)      531 2023-11-17 14:37:09.000000 mkdocstrings-typescript-0.0.0/mkdocstrings_typescript.egg-info/PKG-INFO
--rw-r--r--   0 pawamoy   (1000) pawamoy   (1000)      212 2023-11-17 14:37:09.000000 mkdocstrings-typescript-0.0.0/mkdocstrings_typescript.egg-info/SOURCES.txt
--rw-r--r--   0 pawamoy   (1000) pawamoy   (1000)        1 2023-11-17 14:37:09.000000 mkdocstrings-typescript-0.0.0/mkdocstrings_typescript.egg-info/dependency_links.txt
--rw-r--r--   0 pawamoy   (1000) pawamoy   (1000)        1 2023-11-17 14:37:09.000000 mkdocstrings-typescript-0.0.0/mkdocstrings_typescript.egg-info/top_level.txt
--rw-r--r--   0 pawamoy   (1000) pawamoy   (1000)      315 2023-11-17 14:37:01.000000 mkdocstrings-typescript-0.0.0/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) pawamoy   (1000)       38 2023-11-17 14:37:09.998674 mkdocstrings-typescript-0.0.0/setup.cfg
+-rw-r--r--   0        0        0      754 2024-05-08 19:01:17.771149 mkdocstrings_typescript-0.0.1/LICENSE
+-rw-r--r--   0        0        0      755 2024-05-08 19:01:17.771149 mkdocstrings_typescript-0.0.1/README.md
+-rw-r--r--   0        0        0     1835 2024-05-08 19:31:49.475983 mkdocstrings_typescript-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      136 2024-05-08 19:01:17.777815 mkdocstrings_typescript-0.0.1/src/mkdocstrings_handlers/typescript/__init__.py
+-rw-r--r--   0        0        0     2870 2024-05-08 19:01:17.777815 mkdocstrings_typescript-0.0.1/src/mkdocstrings_handlers/typescript/debug.py
+-rw-r--r--   0        0        0     6932 2024-05-08 19:24:05.738134 mkdocstrings_typescript-0.0.1/src/mkdocstrings_handlers/typescript/handler.py
+-rw-r--r--   0        0        0        0 2024-05-08 19:01:17.777815 mkdocstrings_typescript-0.0.1/src/mkdocstrings_handlers/typescript/py.typed
+-rw-r--r--   0        0        0     2312 1970-01-01 00:00:00.000000 mkdocstrings_typescript-0.0.1/PKG-INFO
```


# Comparing `tmp/dyff_schema-0.4.0.tar.gz` & `tmp/dyff_schema-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_schema-0.4.0.tar", last modified: Wed Apr 17 20:40:21 2024, max compression
+gzip compressed data, was "dyff_schema-0.5.0.tar", last modified: Wed May  8 04:20:54 2024, max compression
```

## Comparing `dyff_schema-0.4.0.tar` & `dyff_schema-0.5.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.516099 dyff_schema-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-17 20:40:21.516099 dyff_schema-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.501099 dyff_schema-0.4.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.508099 dyff_schema-0.4.0/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.510099 dyff_schema-0.4.0/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.510099 dyff_schema-0.4.0/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.510099 dyff_schema-0.4.0/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.512099 dyff_schema-0.4.0/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23552 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17139 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.514099 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12312 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.514099 dyff_schema-0.4.0/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    56634 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.516099 dyff_schema-0.4.0/dyff_schema.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3458 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1358 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-17 20:40:21.000000 dyff_schema-0.4.0/dyff_schema.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 20:40:21.517099 dyff_schema-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 20:40:21.515099 dyff_schema-0.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1449 2024-04-17 20:40:15.000000 dyff_schema-0.4.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.747528 dyff_schema-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-08 04:20:54.747528 dyff_schema-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.733528 dyff_schema-0.5.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.740528 dyff_schema-0.5.0/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.741528 dyff_schema-0.5.0/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.741528 dyff_schema-0.5.0/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.741528 dyff_schema-0.5.0/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.743528 dyff_schema-0.5.0/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23552 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17139 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.744528 dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12312 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.745528 dyff_schema-0.5.0/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    59912 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     7851 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.746528 dyff_schema-0.5.0/dyff_schema.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3458 2024-05-08 04:20:54.000000 dyff_schema-0.5.0/dyff_schema.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2024-05-08 04:20:54.000000 dyff_schema-0.5.0/dyff_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 04:20:54.000000 dyff_schema-0.5.0/dyff_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-08 04:20:54.000000 dyff_schema-0.5.0/dyff_schema.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-08 04:20:54.000000 dyff_schema-0.5.0/dyff_schema.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 04:20:54.747528 dyff_schema-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 04:20:54.746528 dyff_schema-0.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1449 2024-05-08 04:20:48.000000 dyff_schema-0.5.0/tests/test_import.py
```

### Comparing `dyff_schema-0.4.0/.gitlab-ci.yml` & `dyff_schema-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/.pre-commit-config.yaml` & `dyff_schema-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/.secrets.baseline` & `dyff_schema-0.5.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/CODE_OF_CONDUCT.md` & `dyff_schema-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/LICENSE` & `dyff_schema-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/PKG-INFO` & `dyff_schema-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.4.0
+Version: 0.5.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.4.0/README.md` & `dyff_schema-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/__init__.py` & `dyff_schema-0.5.0/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/copydoc.py` & `dyff_schema-0.5.0/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/ids.py` & `dyff_schema-0.5.0/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/quantity.py` & `dyff_schema-0.5.0/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/adapters.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/base.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/__init__.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/arrow.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/binary.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/dataset/text.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/io/vllm.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/platform.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import pydantic
 from typing_extensions import TypeAlias
 
 from ... import named_data_schema, product_schema
 from ...version import SomeSchemaVersion
 from .base import DyffSchemaBaseModel
 from .dataset import arrow, make_item_type, make_response_type
-from .version import VERSION, Versioned
+from .version import SCHEMA_VERSION, SchemaVersion
 
 SYSTEM_ATTRIBUTES = frozenset(["creationTime", "status", "reason"])
 
 
 def _k8s_quantity_regex():
     # This is copy-pasted from the regex that operator-sdk generates for resource.Quantity types
     return r"^(\+|-)?(([0-9]+(\.[0-9]*)?)|(\.[0-9]+))(([KMGTPE]i)|[numkMGTPE]|([eE](\+|-)?(([0-9]+(\.[0-9]*)?)|(\.[0-9]+))))?$"
@@ -145,41 +145,45 @@
     Account = "Account"
     Analysis = "Analysis"
     Audit = "Audit"
     AuditProcedure = "AuditProcedure"
     DataSource = "DataSource"
     Dataset = "Dataset"
     Evaluation = "Evaluation"
+    Family = "Family"
     InferenceService = "InferenceService"
     InferenceSession = "InferenceSession"
     Measurement = "Measurement"
     Method = "Method"
     Model = "Model"
     Module = "Module"
     Report = "Report"
     SafetyCase = "SafetyCase"
+    Tag = "Tag"
 
 
 class Resources(str, enum.Enum):
     """The resource names corresponding to entities that have API endpoints."""
 
     Analysis = "analyses"
     Audit = "audits"
     AuditProcedure = "auditprocedures"
     Dataset = "datasets"
     DataSource = "datasources"
     Evaluation = "evaluations"
+    Family = "families"
     InferenceService = "inferenceservices"
     InferenceSession = "inferencesessions"
     Measurement = "measurements"
     Method = "methods"
     Model = "models"
     Module = "modules"
     Report = "reports"
     SafetyCase = "safetycases"
+    Tag = "tags"
 
     Task = "tasks"
     """
     .. deprecated:: 0.5.0
 
         The Task resource no longer exists, but removing this enum entry
         breaks existing API keys.
@@ -290,15 +294,104 @@
     )
 
     reason: Optional[str] = pydantic.Field(
         default=None, description="Reason for current status (assigned by system)"
     )
 
 
-class DyffEntity(Status, Labeled, Versioned, DyffModelWithID):
+class Documentation(DyffSchemaBaseModel):
+    title: Optional[str] = pydantic.Field(
+        default=None,
+        description='A short plain string suitable as a title or "headline".',
+    )
+
+    summary: Optional[str] = pydantic.Field(
+        default=None,
+        description="A brief summary, suitable for display in"
+        " small UI elements. Interpreted as Markdown. Excessively long"
+        " summaries may be truncated in the UI, especially on small displays.",
+    )
+
+    fullPage: Optional[str] = pydantic.Field(
+        default=None,
+        description="Long-form documentation. Interpreted as"
+        " Markdown. There are no length constraints, but be reasonable.",
+    )
+
+
+class Documented(DyffSchemaBaseModel):
+    documentation: Documentation = pydantic.Field(
+        default_factory=Documentation,
+        description="Documentation of the resource. The content is used to"
+        " populate various views in the web UI.",
+    )
+
+
+class FamilyMemberKind(str, enum.Enum):
+    """The kinds of entities that can be members of a Family.
+
+    These are resources for which it makes sense to have different versions or variants
+    that evolve over time.
+    """
+
+    Dataset = "Dataset"
+    InferenceService = "InferenceService"
+    Method = "Method"
+    Model = "Model"
+    Module = "Module"
+
+
+class FamilyMember(DyffSchemaBaseModel):
+    family: Optional[str] = pydantic.Field(
+        default=None,
+        description="ID of the Family to which the resource belongs.",
+    )
+
+
+class TagBase(DyffSchemaBaseModel):
+    tag: str = pydantic.Field(
+        description="An interpretable identifier for the tag that is unique in"
+        " the context of the corresponding Family."
+    )
+
+    resource: str = pydantic.Field(
+        description="ID of the resource this tag references.",
+    )
+
+    description: str = pydantic.Field(
+        description="A short description of the tag. Interpreted as Markdown."
+        " This should include information about how the tagged version is"
+        " different from other versions."
+    )
+
+
+class Tag(TagBase):
+    created: datetime = pydantic.Field(description="Tag creation time.")
+
+
+class Family(Labeled, SchemaVersion, DyffModelWithID):
+    kind: Literal["Family"] = "Family"
+
+    resourceKind: FamilyMemberKind = pydantic.Field(
+        description="The kind of resource that comprises the family.",
+    )
+
+    tags: list[Tag] = pydantic.Field(
+        default_factory=list,
+        description="Tags mapping interpretable names to resource IDs.",
+    )
+
+    documentation: Documentation = pydantic.Field(
+        default_factory=Documentation,
+        description="Documentation of the resource family. The content is used"
+        " to populate various views in the web UI.",
+    )
+
+
+class DyffEntity(Status, Labeled, SchemaVersion, DyffModelWithID):
     kind: Literal[
         "Analysis",
         "Audit",
         "AuditProcedure",
         "DataSource",
         "Dataset",
         "Evaluation",
@@ -369,14 +462,17 @@
 
     get = "get"
     """Retrieve a single resource instance by ID."""
 
     query = "query"
     """Query the resource collection."""
 
+    edit = "edit"
+    """Edit properties of existing resources."""
+
     download = "download"
     """
     .. deprecated:: 0.5.0
 
         This functionality has been consolidated into ``data``.
     """
 
@@ -574,15 +670,15 @@
 class DyffDataSchema(DyffSchemaBaseModel):
     components: list[str] = pydantic.Field(
         min_items=1,
         description="A list of named dyff data schemas. The final schema is"
         " the composition of these component schemas.",
     )
     schemaVersion: SomeSchemaVersion = pydantic.Field(
-        default=VERSION, description="The dyff schema version"
+        default=SCHEMA_VERSION, description="The dyff schema version"
     )
 
     def model_type(self) -> Type[DyffSchemaBaseModel]:
         """The composite model type."""
         return product_schema(
             named_data_schema(c, self.schemaVersion) for c in self.components
         )
@@ -598,14 +694,20 @@
         default=None, description="The schema in DyffDataSchema format"
     )
     jsonSchema: Optional[dict[str, Any]] = pydantic.Field(
         default=None, description="The schema in JSON Schema format"
     )
 
     @staticmethod
+    def from_model(model: Type[DyffSchemaBaseModel]) -> "DataSchema":
+        arrowSchema = arrow.encode_schema(arrow.arrow_schema(model))
+        jsonSchema = model.schema()
+        return DataSchema(arrowSchema=arrowSchema, jsonSchema=jsonSchema)
+
+    @staticmethod
     def make_input_schema(
         schema: Union[pyarrow.Schema, Type[DyffSchemaBaseModel], DyffDataSchema],
     ) -> "DataSchema":
         """Construct a complete ``DataSchema`` for inference inputs.
 
         This function will add required special fields for input data and then
         convert the augmented schema as necessary to populate at least the
@@ -1742,14 +1844,17 @@
     "DyffEntity",
     "DyffModelWithID",
     "DyffSchemaBaseModel",
     "Entities",
     "Evaluation",
     "EvaluationBase",
     "ExtractorStep",
+    "Family",
+    "FamilyMember",
+    "FamilyMemberKind",
     "ForeignInferenceService",
     "ForeignMethod",
     "ForeignModel",
     "Frameworks",
     "InferenceInterface",
     "InferenceService",
     "InferenceServiceBase",
@@ -1803,14 +1908,16 @@
     "ReportBase",
     "Resources",
     "SafetyCase",
     "SafetyCaseSpec",
     "SchemaAdapter",
     "Status",
     "StorageSignedURL",
+    "Tag",
+    "TagBase",
     "TaskSchema",
     "entity_class",
     "JobStatus",
     "EntityStatus",
     "EntityStatusReason",
     "AuditStatus",
     "DataSourceStatus",
```

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/requests.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,20 @@
     InferenceServiceBase,
     InferenceSessionBase,
     Labeled,
     MethodBase,
     ModelSpec,
     ModuleBase,
     ReportBase,
+    TagBase,
 )
-from .version import Versioned
+from .version import SchemaVersion
 
 
-class DyffEntityCreateRequest(Versioned, DyffSchemaBaseModel):
+class DyffEntityCreateRequest(SchemaVersion, DyffSchemaBaseModel):
     account: str = pydantic.Field(description="Account that owns the entity")
 
 
 class AnalysisCreateRequest(DyffEntityCreateRequest, AnalysisBase):
     """An Analysis transforms Datasets, Evaluations, and Measurements into new
     Measurements or SafetyCases."""
 
@@ -101,14 +102,18 @@
 
     evaluationView: Optional[Union[str, DataView]] = pydantic.Field(
         default=None,
         description="View of the evaluation output data required by the report.",
     )
 
 
+class TagCreateRequest(TagBase):
+    pass
+
+
 class LabelUpdateRequest(Labeled):
     pass
 
 
 # Note: Query requests, as they currently exist, don't work with Versioned
 # because fastapi will assign None to every field that the client doesn't
 # specify. I think it's not that important, because all of the query parameters
@@ -225,8 +230,9 @@
     "ModelCreateRequest",
     "ModelQueryRequest",
     "ModuleCreateRequest",
     "ModuleQueryRequest",
     "ReportCreateRequest",
     "ReportQueryRequest",
     "SafetyCaseQueryRequest",
+    "TagCreateRequest",
 ]
```

### Comparing `dyff_schema-0.4.0/dyff/schema/v0/r1/test.py` & `dyff_schema-0.5.0/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/dyff_schema.egg-info/PKG-INFO` & `dyff_schema-0.5.0/dyff_schema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-schema
-Version: 0.4.0
+Version: 0.5.0
 Summary: Data models for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-schema
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-schema/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_schema-0.4.0/dyff_schema.egg-info/SOURCES.txt` & `dyff_schema-0.5.0/dyff_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/pyproject.toml` & `dyff_schema-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_schema-0.4.0/tests/test_import.py` & `dyff_schema-0.5.0/tests/test_import.py`

 * *Files identical despite different names*


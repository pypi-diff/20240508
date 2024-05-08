# Comparing `tmp/dyff_storage-0.6.2.tar.gz` & `tmp/dyff_storage-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_storage-0.6.2.tar", last modified: Wed Apr 17 22:34:29 2024, max compression
+gzip compressed data, was "dyff_storage-0.7.1.tar", last modified: Wed May  8 20:08:59 2024, max compression
```

## Comparing `dyff_storage-0.6.2.tar` & `dyff_storage-0.7.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.058498 dyff_storage-0.6.2/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1706 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-04-17 22:34:29.057498 dyff_storage-0.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.045498 dyff_storage-0.6.2/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.052498 dyff_storage-0.6.2/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.052498 dyff_storage-0.6.2/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.053498 dyff_storage-0.6.2/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)    12255 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.053498 dyff_storage-0.6.2/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.054498 dyff_storage-0.6.2/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9209 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.054498 dyff_storage-0.6.2/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.055498 dyff_storage-0.6.2/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    20365 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.055498 dyff_storage-0.6.2/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15072 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2946 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.057498 dyff_storage-0.6.2/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-04-17 22:34:29.000000 dyff_storage-0.6.2/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-04-17 22:34:29.000000 dyff_storage-0.6.2/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 22:34:29.000000 dyff_storage-0.6.2/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-04-17 22:34:29.000000 dyff_storage-0.6.2/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-17 22:34:29.000000 dyff_storage-0.6.2/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 22:34:29.058498 dyff_storage-0.6.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:34:29.057498 dyff_storage-0.6.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-17 22:34:23.000000 dyff_storage-0.6.2/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.973514 dyff_storage-0.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-08 20:08:59.972514 dyff_storage-0.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.961514 dyff_storage-0.7.1/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.967514 dyff_storage-0.7.1/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.967514 dyff_storage-0.7.1/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.968514 dyff_storage-0.7.1/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    14287 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.969514 dyff_storage-0.7.1/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.969514 dyff_storage-0.7.1/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.970514 dyff_storage-0.7.1/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.970514 dyff_storage-0.7.1/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    24016 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.971514 dyff_storage-0.7.1/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15072 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.972514 dyff_storage-0.7.1/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 20:08:59.973514 dyff_storage-0.7.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.972514 dyff_storage-0.7.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/tests/test_import.py
```

### Comparing `dyff_storage-0.6.2/.gitignore` & `dyff_storage-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/.gitlab-ci.yml` & `dyff_storage-0.7.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/.licenserc.yaml` & `dyff_storage-0.7.1/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/.pre-commit-config.yaml` & `dyff_storage-0.7.1/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-merge-conflict
       - id: end-of-file-fixer
       - id: fix-byte-order-marker
       - id: trailing-whitespace
 
   - repo: https://github.com/PyCQA/autoflake
-    rev: "v2.3.0"
+    rev: "v2.3.1"
     hooks:
       - id: autoflake
         args:
           - "--in-place"
           - "--expand-star-imports"
           - "--remove-duplicate-keys"
           - "--remove-unused-variables"
           - "--remove-all-unused-imports"
 
   - repo: https://github.com/psf/black
-    rev: 24.2.0
+    rev: 24.4.2
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: "5.13.2"
     hooks:
       - id: isort
@@ -37,31 +37,31 @@
     rev: v1.7.5
     hooks:
       - id: docformatter
         additional_dependencies: [tomli]
         args: ["--in-place", "--black", "--config", "./pyproject.toml"]
 
   - repo: https://gitlab.com/buildgarden/pipelines/skywalking-eyes
-    rev: "0.2.0"
+    rev: "0.2.1"
     hooks:
       - id: license-eye-header-fix
 
   - repo: https://gitlab.com/buildgarden/tools/badgie
-    rev: "0.11.0"
+    rev: "0.12.0"
     hooks:
       - id: badgie
 
   - repo: https://gitlab.com/buildgarden/tools/cici-tools
-    rev: "0.6.0"
+    rev: "0.7.0"
     hooks:
       - id: cici-update
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
 
   - repo: https://github.com/Yelp/detect-secrets
-    rev: v1.4.0
+    rev: v1.5.0
     hooks:
       - id: detect-secrets
         args: ["--baseline", ".secrets.baseline"]
```

### Comparing `dyff_storage-0.6.2/.secrets.baseline` & `dyff_storage-0.7.1/.secrets.baseline`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'version'": "'1.5.0'"}*

```diff
@@ -118,9 +118,9 @@
                 "hashed_secret": "bd564db5d5cc358eb0e3523d3e03041739f230d5",
                 "is_verified": false,
                 "line_number": 82,
                 "type": "Basic Auth Credentials"
             }
         ]
     },
-    "version": "1.4.0"
+    "version": "1.5.0"
 }
```

### Comparing `dyff_storage-0.6.2/CODE_OF_CONDUCT.md` & `dyff_storage-0.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/LICENSE` & `dyff_storage-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/PKG-INFO` & `dyff_storage-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.6.2
+Version: 0.7.1
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.6.2/README.md` & `dyff_storage-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/__init__.py` & `dyff_storage-0.7.1/dyff/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/base/auth.py` & `dyff_storage-0.7.1/dyff/storage/backend/base/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/base/command.py` & `dyff_storage-0.7.1/dyff/storage/backend/base/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/base/query.py` & `dyff_storage-0.7.1/dyff/storage/backend/base/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,37 +7,42 @@
 from typing import Collection, NamedTuple, Optional, Set
 
 from dyff.schema.platform import (
     Analysis,
     Audit,
     Dataset,
     DataSource,
+    Documentation,
     Evaluation,
+    Family,
     InferenceService,
     InferenceSession,
     Measurement,
     Method,
     Model,
     Module,
     Report,
     SafetyCase,
+    Tag,
 )
 from dyff.schema.requests import (
     AnalysisQueryRequest,
     AuditQueryRequest,
     DatasetQueryRequest,
+    DocumentationEditRequest,
     EvaluationQueryRequest,
     InferenceServiceQueryRequest,
     InferenceSessionQueryRequest,
     MeasurementQueryRequest,
     MethodQueryRequest,
     ModelQueryRequest,
     ModuleQueryRequest,
     ReportQueryRequest,
     SafetyCaseQueryRequest,
+    TagCreateRequest,
 )
 
 
 class Whitelist(NamedTuple):
     accounts: Set[str]
     entities: Set[str]
 
@@ -148,14 +153,39 @@
             been granted access to.
           **query: Equality constraints on fields of the Dataset entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
 
     @abc.abstractmethod
+    def edit_documentation(
+        self, id: str, edit: DocumentationEditRequest
+    ) -> Optional[Documentation]:
+        """Edit the Documentation entity associated with a resource.
+
+        Parameters:
+          id: ID of the documented resource.
+          edit: Edit request containing changes to make to the documentation.
+
+        Returns:
+          The new Documentation, or None if no resource exists with the given ID.
+        """
+
+    @abc.abstractmethod
+    def get_documentation(self, id: str) -> Optional[Documentation]:
+        """Retrieve the Documentation entity associated with a resource.
+
+        Parameters:
+          id: ID of the documented resource.
+
+        Returns:
+          The Documentation, or None if no resource exists with the given ID.
+        """
+
+    @abc.abstractmethod
     def get_evaluation(self, id: str) -> Optional[Evaluation]:
         """Retrieve an Evaluation entity.
 
         Parameters:
           id: The unique key of the Evaluation.
 
         Returns:
@@ -173,14 +203,25 @@
             been granted access to.
           **query: Equality constraints on fields of the Evaluation entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
 
     @abc.abstractmethod
+    def get_family(self, id: str) -> Optional[Family]:
+        """Retrieve a Family entity.
+
+        Parameters:
+          id: The unique ID of the Family.
+
+        Returns:
+          The Family, or None if no Family with the specified ID exists.
+        """
+
+    @abc.abstractmethod
     def get_inference_service(self, id: str) -> Optional[InferenceService]:
         """Retrieve an InferenceService entity.
 
         Parameters:
           id: The unique key of the InferenceService.
 
         Returns:
@@ -371,7 +412,33 @@
         Parameters:
           whitelist: The set of accounts and entities that the caller has
             been granted access to.
           **query: Equality constraints on fields of the SafetyCase entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
+
+    @abc.abstractmethod
+    def get_tag(self, id: str) -> Optional[Tag]:
+        """Retrieve a Tag entity.
+
+        Parameters:
+          id: The unique ID of the Tag.
+
+        Returns:
+          The Tag, or None if no Tag with the specified ID exists.
+        """
+
+    @abc.abstractmethod
+    def create_tag(self, family: str, tag_request: TagCreateRequest) -> Optional[Tag]:
+        """Create a new Tag in an existing Family. Has no effect and returns None if a
+        tag with the same name already exists.
+
+        Parameters:
+          family: The ID of the Family to add the tag to.
+          request: TagCreateRequest
+
+        Returns:
+          The created Tag, or None if no Tag was created. This could be because
+          the Family doesn't exist, or because a tag with the same name already
+          exists in the family.
+        """
```

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/base/storage.py` & `dyff_storage-0.7.1/dyff/storage/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/gcloud/storage.py` & `dyff_storage-0.7.1/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/kafka/command.py` & `dyff_storage-0.7.1/dyff/storage/backend/kafka/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/mock/command.py` & `dyff_storage-0.7.1/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/mongodb/auth.py` & `dyff_storage-0.7.1/dyff/storage/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/mongodb/query.py` & `dyff_storage-0.7.1/dyff/storage/backend/mongodb/query.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,41 +9,47 @@
 import pymongo
 
 from dyff.schema.platform import (
     Analysis,
     Audit,
     Dataset,
     DataSource,
+    Documentation,
     Entities,
     Evaluation,
+    Family,
     InferenceService,
     InferenceSession,
     Labeled,
     Measurement,
     Method,
     Model,
     Module,
     Report,
     Resources,
     SafetyCase,
+    Tag,
 )
 from dyff.schema.requests import (
     AnalysisQueryRequest,
     AuditQueryRequest,
     DatasetQueryRequest,
+    DocumentationEditRequest,
     EvaluationQueryRequest,
     InferenceServiceQueryRequest,
     InferenceSessionQueryRequest,
     MeasurementQueryRequest,
     MethodQueryRequest,
     ModelQueryRequest,
     ModuleQueryRequest,
     ReportQueryRequest,
     SafetyCaseQueryRequest,
+    TagCreateRequest,
 )
+from dyff.storage import timestamp
 from dyff.storage.backend.base.query import QueryBackend, Whitelist
 from dyff.storage.config import config
 
 
 class MongoDBQueryBackend(QueryBackend):
     def __init__(self):
         connection_string = config.api.query.mongodb.connection_string
@@ -245,14 +251,57 @@
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
         qdict = query.dict()
         results = self._query_entities(Entities.Dataset, whitelist, qdict)
         return [Dataset.parse_obj(result) for result in results]
 
+    def edit_documentation(
+        self, id: str, edit: DocumentationEditRequest
+    ) -> Optional[Documentation]:
+        """Edit the Documentation entity associated with a resource.
+
+        Parameters:
+          id: ID of the documented resource.
+          edit: Edit request containing changes to make to the documentation.
+
+        Returns:
+          The new Documentation, or None if no resource exists with the given ID.
+        """
+        collection = self._workflows_db["documentation"]
+        # Users can explicitly set a field to None, but we don't want to
+        # overwrite with None implicitly
+        edit_dict = edit.dict(exclude_unset=True)
+        result = collection.find_one_and_update(
+            {"_id": id},
+            {"$set": edit_dict},
+            upsert=True,
+            return_document=pymongo.ReturnDocument.AFTER,
+        )
+        if result is None:
+            return None
+        del result["_id"]
+        return Documentation.parse_obj(result)
+
+    def get_documentation(self, id: str) -> Optional[Documentation]:
+        """Retrieve the Documentation entity associated with a resource.
+
+        Parameters:
+          id: ID of the documented resource.
+
+        Returns:
+          The Documentation, or None if no resource exists with the given ID.
+        """
+        collection = self._workflows_db["documentation"]
+        result = collection.find_one({"_id": id})
+        if result is None:
+            return None
+        del result["_id"]
+        return Documentation.parse_obj(result)
+
     def get_evaluation(self, id: str) -> Optional[Evaluation]:
         """Retrieve an Evaluation entity.
 
         Parameters:
           id: The unique key of the Evaluation.
 
         Returns:
@@ -285,14 +334,26 @@
         )
         self._rename_query_key(
             qdict, "modelName", "inferenceSession.inferenceService.model.name"
         )
         results = self._query_entities(Entities.Evaluation, whitelist, qdict)
         return [Evaluation.parse_obj(result) for result in results]
 
+    def get_family(self, id: str) -> Optional[Family]:
+        """Retrieve a Family entity.
+
+        Parameters:
+          id: The unique ID of the Family.
+
+        Returns:
+          The Family, or None if no Family with the specified ID exists.
+        """
+        result = self._get_entity(Entities.Family, id)
+        return Family.parse_obj(result) if result else None
+
     def get_inference_service(self, id: str) -> Optional[InferenceService]:
         """Retrieve an InferenceService entity.
 
         Parameters:
           id: The unique key of the InferenceService.
 
         Returns:
@@ -519,7 +580,51 @@
             'field: value' in kwargs.
         """
         qdict = query.dict()
         self._rename_query_key(qdict, "method", "method.id")
         self._rename_query_key(qdict, "methodName", "method.name")
         results = self._query_entities(Entities.SafetyCase, whitelist, qdict)
         return [SafetyCase.parse_obj(result) for result in results]
+
+    def get_tag(self, id: str) -> Optional[Tag]:
+        """Retrieve a Tag entity.
+
+        Parameters:
+          id: The unique ID of the Tag.
+
+        Returns:
+          The Tag, or None if no Tag with the specified ID exists.
+        """
+        result = self._get_entity(Entities.Tag, id)
+        return Tag.parse_obj(result) if result else None
+
+    def create_tag(self, family: str, tag_request: TagCreateRequest) -> Optional[Tag]:
+        """Create a new Tag in an existing Family. Has no effect and returns None if a
+        tag with the same name already exists.
+
+        Parameters:
+          family: The ID of the Family to add the tag to.
+          request: TagCreateRequest
+
+        Returns:
+          The created Tag, or None if no Tag was created. This could be because
+          the Family doesn't exist, or because a tag with the same name already
+          exists in the family.
+        """
+        tag_dict = tag_request.dict()
+        tag_dict["created"] = timestamp.now()
+        new_tag = Tag.parse_obj(tag_dict)
+        families_collection = self._workflows_db[Resources.Family]
+        # Atomically check if the tag exists and add it only if it does not exist
+        result = families_collection.update_one(
+            {
+                # Specified Family
+                "_id": family,
+                # Tag does not exist in .tags list
+                "tags": {"$not": {"$elemMatch": {"tag": new_tag.tag}}},
+            },
+            {"$push": {"tags": new_tag.dict()}},
+        )
+        if result.modified_count > 0:
+            return new_tag
+        else:
+            return None
```

### Comparing `dyff_storage-0.6.2/dyff/storage/backend/s3/storage.py` & `dyff_storage-0.7.1/dyff/storage/backend/s3/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/config.py` & `dyff_storage-0.7.1/dyff/storage/config.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/paths.py` & `dyff_storage-0.7.1/dyff/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff/storage/timestamp.py` & `dyff_storage-0.7.1/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/dyff_storage.egg-info/PKG-INFO` & `dyff_storage-0.7.1/dyff_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.6.2
+Version: 0.7.1
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.6.2/dyff_storage.egg-info/SOURCES.txt` & `dyff_storage-0.7.1/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/makefile` & `dyff_storage-0.7.1/makefile`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/pyproject.toml` & `dyff_storage-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.6.2/tests/test_import.py` & `dyff_storage-0.7.1/tests/test_import.py`

 * *Files identical despite different names*


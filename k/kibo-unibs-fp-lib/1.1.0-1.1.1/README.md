# Comparing `tmp/kibo_unibs_fp_lib-1.1.0.tar.gz` & `tmp/kibo_unibs_fp_lib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kibo_unibs_fp_lib-1.1.0.tar", last modified: Thu May  2 14:05:23 2024, max compression
+gzip compressed data, was "kibo_unibs_fp_lib-1.1.1.tar", last modified: Wed May  8 07:54:43 2024, max compression
```

## Comparing `kibo_unibs_fp_lib-1.1.0.tar` & `kibo_unibs_fp_lib-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/ansi_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/file_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    11949 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/known_problems.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/pretty_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib/random_draws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-02 14:05:23.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-02 14:05:23.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:05:23.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 14:05:23.000000 kibo_unibs_fp_lib-1.1.0/kibo_unibs_fp_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:05:23.169391 kibo_unibs_fp_lib-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-02 14:05:18.000000 kibo_unibs_fp_lib-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:54:43.838726 kibo_unibs_fp_lib-1.1.1/
+-rw-rw-rw-   0        0        0      409 2024-05-08 07:54:43.836725 kibo_unibs_fp_lib-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2024-05-08 07:46:03.000000 kibo_unibs_fp_lib-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 07:54:43.834729 kibo_unibs_fp_lib-1.1.1/kibo_unibs_fp_lib.egg-info/
+-rw-rw-rw-   0        0        0      409 2024-05-08 07:54:43.000000 kibo_unibs_fp_lib-1.1.1/kibo_unibs_fp_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-05-08 07:54:43.000000 kibo_unibs_fp_lib-1.1.1/kibo_unibs_fp_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:54:43.000000 kibo_unibs_fp_lib-1.1.1/kibo_unibs_fp_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 07:54:43.000000 kibo_unibs_fp_lib-1.1.1/kibo_unibs_fp_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:54:43.000000 kibo_unibs_fp_lib-1.1.1/kibo_unibs_fp_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:54:43.838726 kibo_unibs_fp_lib-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      580 2024-05-08 07:44:59.000000 kibo_unibs_fp_lib-1.1.1/setup.py
```


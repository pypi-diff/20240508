# Comparing `tmp/vertagus-0.1.0b1.tar.gz` & `tmp/vertagus-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertagus-0.1.0b1.tar", last modified: Wed May  8 17:25:13 2024, max compression
+gzip compressed data, was "vertagus-0.1.0b2.tar", last modified: Wed May  8 19:57:28 2024, max compression
```

## Comparing `vertagus-0.1.0b1.tar` & `vertagus-0.1.0b2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1054 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.151233 vertagus-0.1.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.155233 vertagus-0.1.0b1/src/vertagus/
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.159233 vertagus-0.1.0b1/src/vertagus/aliases/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/aliases/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/aliases/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      699 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/aliases/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.159233 vertagus-0.1.0b1/src/vertagus/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.159233 vertagus-0.1.0b1/src/vertagus/cli/commands/
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/cli/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1132 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/cli/commands/create_tag.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1009 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.159233 vertagus-0.1.0b1/src/vertagus/configuration/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/configuration/load.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4233 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/configuration/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.159233 vertagus-0.1.0b1/src/vertagus/core/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      477 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/core/manifest_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/core/package_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5961 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/core/project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/core/rule_bases.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/core/scm_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/core/stage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/core/tag_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2962 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.159233 vertagus-0.1.0b1/src/vertagus/providers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.159233 vertagus-0.1.0b1/src/vertagus/providers/manifest/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/providers/manifest/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      552 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/providers/manifest/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.159233 vertagus-0.1.0b1/src/vertagus/providers/manifest/setuptools_/
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/providers/manifest/setuptools_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      618 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/src/vertagus/providers/scm/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/providers/scm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/src/vertagus/providers/scm/git_/
--rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/providers/scm/git_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3800 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/providers/scm/git_/git_scm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/providers/scm/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/src/vertagus/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/src/vertagus/rules/comparison/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/rules/comparison/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      908 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/rules/comparison/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/rules/comparison/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/src/vertagus/rules/single_version/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/rules/single_version/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/rules/single_version/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      729 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/rules/single_version/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/src/vertagus/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/utils/factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      533 2024-05-08 17:25:09.000000 vertagus-0.1.0b1/src/vertagus/utils/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:25:13.163233 vertagus-0.1.0b1/src/vertagus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-08 17:25:13.000000 vertagus-0.1.0b1/src/vertagus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-08 17:25:13.000000 vertagus-0.1.0b1/src/vertagus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:25:13.000000 vertagus-0.1.0b1/src/vertagus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 17:25:13.000000 vertagus-0.1.0b1/src/vertagus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 17:25:13.000000 vertagus-0.1.0b1/src/vertagus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 17:25:13.000000 vertagus-0.1.0b1/src/vertagus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.058620 vertagus-0.1.0b2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1054 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-08 19:57:28.058620 vertagus-0.1.0b2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1100 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:57:28.058620 vertagus-0.1.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.046620 vertagus-0.1.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.050619 vertagus-0.1.0b2/src/vertagus/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.050619 vertagus-0.1.0b2/src/vertagus/aliases/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/aliases/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/aliases/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      699 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/aliases/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/cli/commands/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/cli/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1132 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/cli/commands/create_tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1009 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/configuration/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/configuration/load.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4233 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/configuration/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/core/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      477 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/core/manifest_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/core/package_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5961 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/core/project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/core/rule_bases.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/core/scm_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/core/stage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/core/tag_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2962 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/providers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/providers/manifest/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/providers/manifest/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      552 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/providers/manifest/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/providers/manifest/setuptools_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/providers/manifest/setuptools_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      618 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/providers/scm/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/providers/scm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/providers/scm/git_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/providers/scm/git_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3975 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/providers/scm/git_/git_scm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/providers/scm/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.054620 vertagus-0.1.0b2/src/vertagus/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.058620 vertagus-0.1.0b2/src/vertagus/rules/comparison/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/rules/comparison/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      908 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/rules/comparison/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/rules/comparison/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.058620 vertagus-0.1.0b2/src/vertagus/rules/single_version/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/rules/single_version/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/rules/single_version/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      729 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/rules/single_version/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.058620 vertagus-0.1.0b2/src/vertagus/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/utils/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/utils/factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      533 2024-05-08 19:57:24.000000 vertagus-0.1.0b2/src/vertagus/utils/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:57:28.058620 vertagus-0.1.0b2/src/vertagus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-08 19:57:28.000000 vertagus-0.1.0b2/src/vertagus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-08 19:57:28.000000 vertagus-0.1.0b2/src/vertagus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:57:28.000000 vertagus-0.1.0b2/src/vertagus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 19:57:28.000000 vertagus-0.1.0b2/src/vertagus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 19:57:28.000000 vertagus-0.1.0b2/src/vertagus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 19:57:28.000000 vertagus-0.1.0b2/src/vertagus.egg-info/top_level.txt
```

### Comparing `vertagus-0.1.0b1/LICENSE` & `vertagus-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/PKG-INFO` & `vertagus-0.1.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertagus
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: A tool to assist the maintenance of package versioning with scm tags
 Author-email: John Raines <johndanielraines@gmail.com>
 License: Copyright (c) 2024 John Raines
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: GitPython
 Requires-Dist: tomli
 Requires-Dist: packaging
+Requires-Dist: PyYAML>=6
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: qa
 Requires-Dist: pytest; extra == "qa"
 Requires-Dist: pytest-cov; extra == "qa"
```

### Comparing `vertagus-0.1.0b1/README.md` & `vertagus-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/pyproject.toml` & `vertagus-0.1.0b2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vertagus"
-version = "0.1.0b1"
+version = "0.1.0b2"
 description = "A tool to assist the maintenance of package versioning with scm tags"
 readme = "README.md"
 authors = [
     {"name" = "John Raines", "email" = "johndanielraines@gmail.com"}
 ]
 dependencies = [
     "click",
     "GitPython",
     "tomli",
-    "packaging"
+    "packaging",
+    "PyYAML>=6"
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Topic :: Software Development",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
```

### Comparing `vertagus-0.1.0b1/src/vertagus/aliases/library.py` & `vertagus-0.1.0b2/src/vertagus/aliases/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/aliases/loader.py` & `vertagus-0.1.0b2/src/vertagus/aliases/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/cli/commands/create_tag.py` & `vertagus-0.1.0b2/src/vertagus/cli/commands/create_tag.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/cli/commands/validate.py` & `vertagus-0.1.0b2/src/vertagus/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/configuration/types.py` & `vertagus-0.1.0b2/src/vertagus/configuration/types.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/core/package_base.py` & `vertagus-0.1.0b2/src/vertagus/core/package_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/core/project.py` & `vertagus-0.1.0b2/src/vertagus/core/project.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/core/rule_bases.py` & `vertagus-0.1.0b2/src/vertagus/core/rule_bases.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/core/scm_base.py` & `vertagus-0.1.0b2/src/vertagus/core/scm_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/core/stage.py` & `vertagus-0.1.0b2/src/vertagus/core/stage.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/factory.py` & `vertagus-0.1.0b2/src/vertagus/factory.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/operations.py` & `vertagus-0.1.0b2/src/vertagus/operations.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/providers/manifest/registry.py` & `vertagus-0.1.0b2/src/vertagus/providers/manifest/registry.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py` & `vertagus-0.1.0b2/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/providers/scm/git_/git_scm.py` & `vertagus-0.1.0b2/src/vertagus/providers/scm/git_/git_scm.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,19 +72,23 @@
         except GitCommandError as e:
             logger.warning(
                 f"Error encountered while deleting remote tag {tag_text!r}: {e.__class__.__name__}: {e}"
             )
         self._repo.git.push(tags=True)
     
     def list_tags(self, prefix: str=None):
-        tags = self._repo.tags
+        tags = [
+            t.split("tags/")[-1].strip() for t in
+            self._repo.git.execute(["git", "ls-remote", "--tags", self.remote_name]).split("\n")
+            if not t.endswith("^{}")
+        ]
         if not prefix and self.tag_prefix:
             prefix = self.tag_prefix
         if prefix:
-            tags = [tag for tag in tags if tag.name.startswith(prefix)]
+            tags = [tag for tag in tags if tag.startswith(prefix)]
         return tags
 
     def migrate_alias(self, alias: AliasBase, ref: str = None):
         logger.info(
             f"Migrating alias {alias.name} to ref {ref}"
         )
         try:
```

### Comparing `vertagus-0.1.0b1/src/vertagus/rules/comparison/library.py` & `vertagus-0.1.0b2/src/vertagus/rules/comparison/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/rules/comparison/loader.py` & `vertagus-0.1.0b2/src/vertagus/rules/comparison/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/rules/single_version/library.py` & `vertagus-0.1.0b2/src/vertagus/rules/single_version/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/rules/single_version/loader.py` & `vertagus-0.1.0b2/src/vertagus/rules/single_version/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus/utils/regex.py` & `vertagus-0.1.0b2/src/vertagus/utils/regex.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b1/src/vertagus.egg-info/PKG-INFO` & `vertagus-0.1.0b2/src/vertagus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertagus
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: A tool to assist the maintenance of package versioning with scm tags
 Author-email: John Raines <johndanielraines@gmail.com>
 License: Copyright (c) 2024 John Raines
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: GitPython
 Requires-Dist: tomli
 Requires-Dist: packaging
+Requires-Dist: PyYAML>=6
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: qa
 Requires-Dist: pytest; extra == "qa"
 Requires-Dist: pytest-cov; extra == "qa"
```

### Comparing `vertagus-0.1.0b1/src/vertagus.egg-info/SOURCES.txt` & `vertagus-0.1.0b2/src/vertagus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,9 +42,10 @@
 src/vertagus/rules/comparison/__init__.py
 src/vertagus/rules/comparison/library.py
 src/vertagus/rules/comparison/loader.py
 src/vertagus/rules/single_version/__init__.py
 src/vertagus/rules/single_version/library.py
 src/vertagus/rules/single_version/loader.py
 src/vertagus/utils/__init__.py
+src/vertagus/utils/config.py
 src/vertagus/utils/factory.py
 src/vertagus/utils/regex.py
```


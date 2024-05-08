# Comparing `tmp/tach-0.1.7.tar.gz` & `tmp/tach-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.1.7.tar", last modified: Sun May  5 04:16:13 2024, max compression
+gzip compressed data, was "tach-0.1.8.tar", last modified: Wed May  8 01:31:01 2024, max compression
```

## Comparing `tach-0.1.7.tar` & `tach-0.1.8.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.020540 tach-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:12.996539 tach-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.004539 tach-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-05 04:16:04.000000 tach-0.1.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-05 04:16:04.000000 tach-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-05 04:16:04.000000 tach-0.1.7/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-05 04:16:04.000000 tach-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-05 04:16:04.000000 tach-0.1.7/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-05 04:16:04.000000 tach-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-05 04:16:13.020540 tach-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-05 04:16:04.000000 tach-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-05 04:16:04.000000 tach-0.1.7/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.004539 tach-0.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-05 04:16:04.000000 tach-0.1.7/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-05 04:16:04.000000 tach-0.1.7/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-05 04:16:04.000000 tach-0.1.7/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-05 04:16:04.000000 tach-0.1.7/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-05 04:16:04.000000 tach-0.1.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-05 04:16:04.000000 tach-0.1.7/docs/strict-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-05 04:16:04.000000 tach-0.1.7/docs/tach-ignore.md
--rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-05 04:16:04.000000 tach-0.1.7/docs/tach_demo.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-05 04:16:04.000000 tach-0.1.7/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-05 04:16:04.000000 tach-0.1.7/docs/why-tach.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-05 04:16:04.000000 tach-0.1.7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-05 04:16:04.000000 tach-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 04:16:13.020540 tach-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.008539 tach-0.1.7/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-05 04:16:04.000000 tach-0.1.7/tach/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-05-05 04:16:04.000000 tach-0.1.7/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-05 04:16:04.000000 tach-0.1.7/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.008539 tach-0.1.7/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-05 04:16:04.000000 tach-0.1.7/tach/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 04:16:04.000000 tach-0.1.7/tach/colors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.008539 tach-0.1.7/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 04:16:04.000000 tach-0.1.7/tach/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 04:16:04.000000 tach-0.1.7/tach/constants/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.008539 tach-0.1.7/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 04:16:04.000000 tach-0.1.7/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-05 04:16:04.000000 tach-0.1.7/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-05 04:16:04.000000 tach-0.1.7/tach/core/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 04:16:04.000000 tach-0.1.7/tach/core/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.008539 tach-0.1.7/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-05 04:16:04.000000 tach-0.1.7/tach/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 04:16:04.000000 tach-0.1.7/tach/errors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.012539 tach-0.1.7/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-05 04:16:04.000000 tach-0.1.7/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-05 04:16:04.000000 tach-0.1.7/tach/filesystem/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-05 04:16:04.000000 tach-0.1.7/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 04:16:04.000000 tach-0.1.7/tach/filesystem/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-05 04:16:04.000000 tach-0.1.7/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-05 04:16:04.000000 tach-0.1.7/tach/filesystem/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.012539 tach-0.1.7/tach/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-05 04:16:04.000000 tach-0.1.7/tach/hooks/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-05 04:16:04.000000 tach-0.1.7/tach/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-05 04:16:04.000000 tach-0.1.7/tach/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 04:16:04.000000 tach-0.1.7/tach/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.012539 tach-0.1.7/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-05 04:16:04.000000 tach-0.1.7/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-05 04:16:04.000000 tach-0.1.7/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-05 04:16:04.000000 tach-0.1.7/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-05 04:16:04.000000 tach-0.1.7/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-05 04:16:04.000000 tach-0.1.7/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-05 04:16:04.000000 tach-0.1.7/tach/parsing/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 04:16:04.000000 tach-0.1.7/tach/parsing/packages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.020540 tach-0.1.7/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-05 04:16:12.000000 tach-0.1.7/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-05 04:16:12.000000 tach-0.1.7/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 04:16:12.000000 tach-0.1.7/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-05 04:16:12.000000 tach-0.1.7/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-05 04:16:12.000000 tach-0.1.7/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 04:16:12.000000 tach-0.1.7/tach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 04:16:04.000000 tach-0.1.7/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.012539 tach-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.012539 tach-0.1.7/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.016540 tach-0.1.7/tests/example/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.016540 tach-0.1.7/tests/example/domain_one/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_one/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.016540 tach-0.1.7/tests/example/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_three/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.016540 tach-0.1.7/tests/example/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_two/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_two/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.016540 tach-0.1.7/tests/example/domain_two/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/domain_two/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.016540 tach-0.1.7/tests/example/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.016540 tach-0.1.7/tests/example/invalid/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/empty/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/empty/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.016540 tach-0.1.7/tests/example/invalid/hidden/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.016540 tach-0.1.7/tests/example/invalid/hidden/.hidden/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/hidden/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.020540 tach-0.1.7/tests/example/invalid/hidden/unhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/invalid/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.020540 tach-0.1.7/tests/example/valid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/valid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.020540 tach-0.1.7/tests/example/valid/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/valid/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.020540 tach-0.1.7/tests/example/valid/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/valid/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:16:13.020540 tach-0.1.7/tests/example/valid/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/valid/domain_two/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-05 04:16:04.000000 tach-0.1.7/tests/example/valid/tach.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-05 04:16:04.000000 tach-0.1.7/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-05 04:16:04.000000 tach-0.1.7/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-05 04:16:04.000000 tach-0.1.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-05 04:16:04.000000 tach-0.1.7/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-05 04:16:04.000000 tach-0.1.7/tests/test_module_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-05 04:16:04.000000 tach-0.1.7/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 04:16:04.000000 tach-0.1.7/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.448600 tach-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.428600 tach-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.432600 tach-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-08 01:30:57.000000 tach-0.1.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-08 01:30:57.000000 tach-0.1.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 01:30:57.000000 tach-0.1.8/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-08 01:30:57.000000 tach-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 01:30:57.000000 tach-0.1.8/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 01:30:57.000000 tach-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-08 01:31:01.448600 tach-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-08 01:30:57.000000 tach-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 01:30:57.000000 tach-0.1.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-08 01:30:57.000000 tach-0.1.8/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-08 01:30:57.000000 tach-0.1.8/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-08 01:30:57.000000 tach-0.1.8/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 01:30:57.000000 tach-0.1.8/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 01:30:57.000000 tach-0.1.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-08 01:30:57.000000 tach-0.1.8/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-08 01:30:57.000000 tach-0.1.8/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-08 01:30:57.000000 tach-0.1.8/docs/tach_demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-08 01:30:57.000000 tach-0.1.8/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-08 01:30:57.000000 tach-0.1.8/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 01:30:57.000000 tach-0.1.8/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-08 01:30:57.000000 tach-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:31:01.448600 tach-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-08 01:30:57.000000 tach-0.1.8/tach/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-08 01:30:57.000000 tach-0.1.8/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-08 01:30:57.000000 tach-0.1.8/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 01:30:57.000000 tach-0.1.8/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 01:30:57.000000 tach-0.1.8/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-08 01:30:57.000000 tach-0.1.8/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 01:30:57.000000 tach-0.1.8/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 01:30:57.000000 tach-0.1.8/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-08 01:30:57.000000 tach-0.1.8/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-08 01:30:57.000000 tach-0.1.8/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 01:30:57.000000 tach-0.1.8/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.436601 tach-0.1.8/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 01:30:57.000000 tach-0.1.8/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 01:30:57.000000 tach-0.1.8/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-08 01:30:57.000000 tach-0.1.8/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tach/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       83 2024-05-08 01:30:57.000000 tach-0.1.8/tach/hooks/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-08 01:30:57.000000 tach-0.1.8/tach/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 01:30:57.000000 tach-0.1.8/tach/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 01:30:57.000000 tach-0.1.8/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-08 01:30:57.000000 tach-0.1.8/tach/parsing/packages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 01:31:01.000000 tach-0.1.8/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 01:30:57.000000 tach-0.1.8/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.440600 tach-0.1.8/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:31:01.444600 tach-0.1.8/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-08 01:30:57.000000 tach-0.1.8/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_module_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:30:57.000000 tach-0.1.8/tests/test_show.py
```

### Comparing `tach-0.1.7/.github/workflows/ci.yml` & `tach-0.1.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/.github/workflows/publish.yml` & `tach-0.1.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/.github/workflows/publish_docs.yml` & `tach-0.1.8/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/.gitignore` & `tach-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/LICENSE` & `tach-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/PKG-INFO` & `tach-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -55,15 +55,15 @@
 `tach` is incredibly lightweight, and has no impact on your runtime. Instead, its checks are performed as a lint check through the CLI.
 
 ## Installation
 ```bash
 pip install tach
 ```
 
-## Initial Setup
+## Quickstart
 `tach` comes bundled with a command to set up and define your initial boundaries.
 ```bash
 tach init
 ```
 By running `tach init` from the root of your Python project, `tach` will initialize each top-level Python package. Each package will receive a `package.yml` with a single tag based on the folder name. 
 The tool will take into consideration the usages between packages, and write a matching set of dependencies to `tach.yml` in the project root.
```

### Comparing `tach-0.1.7/README.md` & `tach-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 `tach` is incredibly lightweight, and has no impact on your runtime. Instead, its checks are performed as a lint check through the CLI.
 
 ## Installation
 ```bash
 pip install tach
 ```
 
-## Initial Setup
+## Quickstart
 `tach` comes bundled with a command to set up and define your initial boundaries.
 ```bash
 tach init
 ```
 By running `tach init` from the root of your Python project, `tach` will initialize each top-level Python package. Each package will receive a `package.yml` with a single tag based on the folder name. 
 The tool will take into consideration the usages between packages, and write a matching set of dependencies to `tach.yml` in the project root.
```

### Comparing `tach-0.1.7/docs/configuration.md` & `tach-0.1.8/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/docs/faq.md` & `tach-0.1.8/docs/faq.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/docs/favicon.ico` & `tach-0.1.8/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/docs/getting-started.md` & `tach-0.1.8/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/docs/index.md` & `tach-0.1.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/docs/strict-mode.md` & `tach-0.1.8/docs/strict-mode.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/docs/tach-ignore.md` & `tach-0.1.8/docs/tach-ignore.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/docs/tach_demo.mp4` & `tach-0.1.8/docs/tach_demo.mp4`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/docs/usage.md` & `tach-0.1.8/docs/usage.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/docs/why-tach.md` & `tach-0.1.8/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/mkdocs.yml` & `tach-0.1.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/pyproject.toml` & `tach-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tach-0.1.7/tach/add.py` & `tach-0.1.8/tach/add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/check.py` & `tach-0.1.8/tach/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,19 @@
     for file_path in fs.walk_pyfiles(
         root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
     ):
         mod_path = fs.file_to_module_path(file_path)
         nearest_package = package_trie.find_nearest(mod_path)
         if nearest_package is None:
             continue
-        import_mod_paths = get_project_imports(root, file_path)
+        import_mod_paths = get_project_imports(
+            root,
+            file_path,
+            ignore_type_checking_imports=project_config.ignore_type_checking_imports,
+        )
         # This should only give us imports from within our project
         # (excluding stdlib, builtins, and 3rd party packages)
         for import_mod_path in import_mod_paths:
             check_result = check_import(
                 project_config=project_config,
                 package_trie=package_trie,
                 import_mod_path=import_mod_path,
```

### Comparing `tach-0.1.7/tach/cli.py` & `tach-0.1.8/tach/cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/core/config.py` & `tach-0.1.8/tach/core/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 class ProjectConfig(Config):
     """
     Configuration applied globally to a project.
     """
 
     constraints: List[TagDependencyRules] = Field(default_factory=list)
     exclude: Optional[List[str]] = Field(default_factory=lambda: ["tests", "docs"])
-    exclude_hidden_paths: Optional[bool] = True
+    exclude_hidden_paths: bool = True
+    ignore_type_checking_imports: bool = False
 
     def dependencies_for_tag(self, tag: str) -> list[str]:
         return next(
             (
                 constraint.depends_on
                 for constraint in self.constraints
                 if constraint.tag == tag
```

### Comparing `tach-0.1.7/tach/core/package.py` & `tach-0.1.8/tach/core/package.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/filesystem/__init__.py` & `tach-0.1.8/tach/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/filesystem/install.py` & `tach-0.1.8/tach/filesystem/install.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/filesystem/project.py` & `tach-0.1.8/tach/filesystem/project.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/filesystem/service.py` & `tach-0.1.8/tach/filesystem/service.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/init.py` & `tach-0.1.8/tach/init.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/loading.py` & `tach-0.1.8/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/parsing/config.py` & `tach-0.1.8/tach/parsing/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/parsing/imports.py` & `tach-0.1.8/tach/parsing/imports.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,28 +35,38 @@
 class ImportVisitor(ast.NodeVisitor):
     def __init__(
         self,
         project_root: str,
         current_mod_path: str,
         is_package: bool = False,
         ignore_directives: Optional[dict[int, IgnoreDirective]] = None,
+        ignore_type_checking_imports: bool = False,
     ):
         self.project_root = project_root
         self.current_mod_path = current_mod_path
         self.is_package = is_package
         self.ignored_imports = ignore_directives or {}
         self.imports: list[str] = []
+        self.ignore_type_checking_imports = ignore_type_checking_imports
 
     def _get_ignored_modules(self, lineno: int) -> Optional[list[str]]:
         # Check for ignore directive at the previous line or on the current line
         directive = self.ignored_imports.get(lineno - 1) or self.ignored_imports.get(
             lineno
         )
         return directive.modules if directive else None
 
+    def visit_If(self, node: ast.If):
+        if isinstance(node.test, ast.Name) and node.test.id == "TYPE_CHECKING":
+            if self.ignore_type_checking_imports:
+                return
+
+        # assume other conditional imports represent real dependencies
+        self.generic_visit(node)
+
     def visit_ImportFrom(self, node: ast.ImportFrom):
         # For relative imports (level > 0), adjust the base module path
         if node.module is not None and node.level > 0:
             num_paths_to_strip = node.level - 1 if self.is_package else node.level
             base_path_parts = self.current_mod_path.split(".")
             if num_paths_to_strip:
                 base_path_parts = base_path_parts[:-num_paths_to_strip]
@@ -95,20 +105,23 @@
             if alias.name in ignored_modules or not fs.is_project_import(
                 self.project_root, alias.name
             ):
                 continue
             self.imports.append(alias.name)
 
 
-def get_project_imports(project_root: str, file_path: str) -> list[str]:
+def get_project_imports(
+    project_root: str, file_path: str, ignore_type_checking_imports: bool = False
+) -> list[str]:
     file_content = fs.read_file(file_path)
     parsed_ast = fs.parse_ast(file_path)
     ignore_directives = get_ignore_directives(file_content)
     mod_path = fs.file_to_module_path(file_path)
     import_visitor = ImportVisitor(
         project_root=project_root,
         is_package=file_path.endswith("__init__.py"),
         current_mod_path=mod_path,
         ignore_directives=ignore_directives,
+        ignore_type_checking_imports=ignore_type_checking_imports,
     )
     import_visitor.visit(parsed_ast)
     return import_visitor.imports
```

### Comparing `tach-0.1.7/tach/parsing/interface.py` & `tach-0.1.8/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach/parsing/packages.py` & `tach-0.1.8/tach/parsing/packages.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tach.egg-info/PKG-INFO` & `tach-0.1.8/tach.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -55,15 +55,15 @@
 `tach` is incredibly lightweight, and has no impact on your runtime. Instead, its checks are performed as a lint check through the CLI.
 
 ## Installation
 ```bash
 pip install tach
 ```
 
-## Initial Setup
+## Quickstart
 `tach` comes bundled with a command to set up and define your initial boundaries.
 ```bash
 tach init
 ```
 By running `tach init` from the root of your Python project, `tach` will initialize each top-level Python package. Each package will receive a `package.yml` with a single tag based on the folder name. 
 The tool will take into consideration the usages between packages, and write a matching set of dependencies to `tach.yml` in the project root.
```

### Comparing `tach-0.1.7/tach.egg-info/SOURCES.txt` & `tach-0.1.8/tach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tests/test_add.py` & `tach-0.1.8/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tests/test_check.py` & `tach-0.1.8/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tests/test_cli.py` & `tach-0.1.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tests/test_init.py` & `tach-0.1.8/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tests/test_module_trie.py` & `tach-0.1.8/tests/test_module_trie.py`

 * *Files identical despite different names*

### Comparing `tach-0.1.7/tests/test_parsing.py` & `tach-0.1.8/tests/test_parsing.py`

 * *Files identical despite different names*


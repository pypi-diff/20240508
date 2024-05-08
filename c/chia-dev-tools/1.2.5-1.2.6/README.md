# Comparing `tmp/chia_dev_tools-1.2.5.tar.gz` & `tmp/chia_dev_tools-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chia_dev_tools-1.2.5.tar", last modified: Thu May  2 22:52:44 2024, max compression
+gzip compressed data, was "chia_dev_tools-1.2.6.tar", last modified: Wed May  8 17:14:08 2024, max compression
```

## Comparing `chia_dev_tools-1.2.5.tar` & `chia_dev_tools-1.2.6.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.122604 chia_dev_tools-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.110603 chia_dev_tools-1.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.106603 chia_dev_tools-1.2.5/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.110603 chia_dev_tools-1.2.5/.github/actions/install/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/actions/install/action.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/actions/install/install.ps1
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/actions/install/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/workflows/precommit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/workflows/run-test-suite.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/workflows/super-linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.github/workflows/test-blockchain-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.markdown-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-02 22:52:44.122604 chia_dev_tools-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      230 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/activated.ps1
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/activated.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      230 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/activated.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/clibs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/clibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/clibs/condition_codes.clib
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/clibs/curry_and_treehash.clib
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/clibs/sha256tree.clib
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/clibs/singleton_truths.clib
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/clibs/utility_macros.clib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30371 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/cmds/chia_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/cmds/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/cmds/clsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15105 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/cmds/rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/cmds/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/examples/clsp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/examples/clsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/examples/clsp/piggybank.clsp
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/examples/clsp/piggybank.clsp.hex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/examples/clvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/examples/clvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/examples/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/examples/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/examples/drivers/piggybank_drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/examples/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/examples/tests/test_piggybank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/test/
--rw-r--r--   0 runner    (1001) docker     (127)    29495 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/test/test_skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.114604 chia_dev_tools-1.2.5/cdv/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/util/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/cdv/util/load_clvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.118604 chia_dev_tools-1.2.5/chia_dev_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-02 22:52:44.000000 chia_dev_tools-1.2.5/chia_dev_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-02 22:52:44.000000 chia_dev_tools-1.2.5/chia_dev_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 22:52:44.000000 chia_dev_tools-1.2.5/chia_dev_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 22:52:44.000000 chia_dev_tools-1.2.5/chia_dev_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 22:52:44.000000 chia_dev_tools-1.2.5/chia_dev_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 22:52:44.000000 chia_dev_tools-1.2.5/chia_dev_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 22:52:44.122604 chia_dev_tools-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.118604 chia_dev_tools-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/build-init-files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.118604 chia_dev_tools-1.2.5/tests/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.110603 chia_dev_tools-1.2.5/tests/cmds/object_files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.118604 chia_dev_tools-1.2.5/tests/cmds/object_files/coinrecords/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/coinrecords/coinrecord.hex
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/coinrecords/coinrecord.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/coinrecords/coinrecord_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/coinrecords/coinrecord_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.118604 chia_dev_tools-1.2.5/tests/cmds/object_files/coins/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/coins/coin.json
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/coins/coin_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/coins/coin_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.118604 chia_dev_tools-1.2.5/tests/cmds/object_files/spendbundles/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/spendbundles/spendbundle.hex
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/spendbundles/spendbundle.json
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/spendbundles/spendbundle_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/spendbundles/spendbundle_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 22:52:44.118604 chia_dev_tools-1.2.5/tests/cmds/object_files/spends/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/spends/spend.hex
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/spends/spend.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/spends/spend_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/spends/spend_invalid.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/object_files/spends/spend_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/test_cdv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/test_clsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/cmds/test_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-02 22:52:18.000000 chia_dev_tools-1.2.5/tests/test_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.218783 chia_dev_tools-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.202784 chia_dev_tools-1.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.198784 chia_dev_tools-1.2.6/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.202784 chia_dev_tools-1.2.6/.github/actions/install/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/actions/install/action.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/actions/install/install.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/actions/install/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.206784 chia_dev_tools-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/workflows/precommit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/workflows/run-test-suite.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/workflows/super-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.github/workflows/test-blockchain-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.markdown-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/.repo-content-updater.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-08 17:14:08.214784 chia_dev_tools-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      230 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/activated.ps1
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/activated.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/activated.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.206784 chia_dev_tools-1.2.6/cdv/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.206784 chia_dev_tools-1.2.6/cdv/clibs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/clibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/clibs/condition_codes.clib
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/clibs/curry_and_treehash.clib
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/clibs/sha256tree.clib
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/clibs/singleton_truths.clib
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/clibs/utility_macros.clib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.206784 chia_dev_tools-1.2.6/cdv/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30431 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/cmds/chia_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/cmds/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/cmds/clsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15105 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/cmds/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/cmds/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.206784 chia_dev_tools-1.2.6/cdv/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.206784 chia_dev_tools-1.2.6/cdv/examples/clsp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/examples/clsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/examples/clsp/piggybank.clsp
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/examples/clsp/piggybank.clsp.hex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.206784 chia_dev_tools-1.2.6/cdv/examples/clvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/examples/clvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.210784 chia_dev_tools-1.2.6/cdv/examples/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/examples/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/examples/drivers/piggybank_drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.210784 chia_dev_tools-1.2.6/cdv/examples/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/examples/tests/test_piggybank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.210784 chia_dev_tools-1.2.6/cdv/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    29257 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/test/test_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.210784 chia_dev_tools-1.2.6/cdv/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/util/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/cdv/util/load_clvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.214784 chia_dev_tools-1.2.6/chia_dev_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-08 17:14:08.000000 chia_dev_tools-1.2.6/chia_dev_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-08 17:14:08.000000 chia_dev_tools-1.2.6/chia_dev_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:14:08.000000 chia_dev_tools-1.2.6/chia_dev_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 17:14:08.000000 chia_dev_tools-1.2.6/chia_dev_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-08 17:14:08.000000 chia_dev_tools-1.2.6/chia_dev_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 17:14:08.000000 chia_dev_tools-1.2.6/chia_dev_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:14:08.218783 chia_dev_tools-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.210784 chia_dev_tools-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/build-init-files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.210784 chia_dev_tools-1.2.6/tests/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.202784 chia_dev_tools-1.2.6/tests/cmds/object_files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.210784 chia_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/coinrecord.hex
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/coinrecord.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/coinrecord_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/coinrecords/coinrecord_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.214784 chia_dev_tools-1.2.6/tests/cmds/object_files/coins/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/coins/coin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/coins/coin_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/coins/coin_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.214784 chia_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle.hex
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle.json
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:14:08.214784 chia_dev_tools-1.2.6/tests/cmds/object_files/spends/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/spends/spend.hex
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/spends/spend.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/spends/spend_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/spends/spend_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/object_files/spends/spend_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/test_cdv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/test_clsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/cmds/test_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-08 17:13:40.000000 chia_dev_tools-1.2.6/tests/test_skeleton.py
```

### Comparing `chia_dev_tools-1.2.5/.github/actions/install/action.yml` & `chia_dev_tools-1.2.6/.github/actions/install/action.yml`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/.github/dependabot.yml` & `chia_dev_tools-1.2.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/.github/workflows/codeql-analysis.yml` & `chia_dev_tools-1.2.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/.github/workflows/dependency-review.yml` & `chia_dev_tools-1.2.6/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/.github/workflows/precommit.yml` & `chia_dev_tools-1.2.6/.github/workflows/precommit.yml`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,18 @@
     steps:
     - name: Clean workspace
       uses: Chia-Network/actions/clean-workspace@main
 
     - name: Add safe git directory
       uses: Chia-Network/actions/git-mark-workspace-safe@main
 
+    - name: disable git autocrlf
+      run: |
+        git config --global core.autocrlf false
+
     - uses: actions/checkout@v4
 
     - uses: Chia-Network/actions/setup-python@main
       with:
         python-version: ${{ matrix.python.major_dot_minor }}
 
     - uses: ./.github/actions/install
```

### Comparing `chia_dev_tools-1.2.5/.github/workflows/publish-to-pypi.yml` & `chia_dev_tools-1.2.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/.github/workflows/run-test-suite.yml` & `chia_dev_tools-1.2.6/.github/workflows/run-test-suite.yml`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/.github/workflows/super-linter.yml` & `chia_dev_tools-1.2.6/.github/workflows/super-linter.yml`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
           VALIDATE_JSON: true
           VALIDATE_MD: true
           VALIDATE_POWERSHELL: true
           VALIDATE_PYTHON: true
           VALIDATE_PYTHON_PYLINT: true
           VALIDATE_PYTHON_ISORT: true
           PYTHON_ISORT_CONFIG_FILE: pyproject.toml
-          VALIDATE_SHELL_SHFMT: true
           VALIDATE_TYPESCRIPT_ES: true
           VALIDATE_YAML: true
           DISABLE_ERRORS: false
           PYTHONPATH: ${{ github.workspace }}:$PYTHONPATH
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           FILTER_REGEX_EXCLUDE: .*github/ISSUE_TEMPLATE/config.yml
 #          ACTIONS_RUNNER_DEBUG: true
```

### Comparing `chia_dev_tools-1.2.5/.github/workflows/test-blockchain-main.yml` & `chia_dev_tools-1.2.6/.github/workflows/test-blockchain-main.yml`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/.markdown-lint.yml` & `chia_dev_tools-1.2.6/.markdown-lint.yml`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/.pre-commit-config.yaml` & `chia_dev_tools-1.2.6/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,19 @@
         require_serial: true
         language: python
         language_version: python3
         types_or: [cython, pyi, python]
         args: ['--filter-files']
         minimum_pre_commit_version: '2.9.2'
         additional_dependencies: [isort==5.10.1]
+-   repo: https://github.com/scop/pre-commit-shfmt
+    rev: v3.8.0-1
+    hooks:
+    -   id: shfmt
+        args: ["--diff", "--write", "-i", "2"]
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.0.1
     hooks:
     -   id: check-yaml
     -   id: end-of-file-fixer
         exclude: ".*?(.hex|.clvm|.clib)"
     -   id: trailing-whitespace
```

### Comparing `chia_dev_tools-1.2.5/LICENSE` & `chia_dev_tools-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/PKG-INFO` & `chia_dev_tools-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chia_dev_tools
-Version: 1.2.5
+Version: 1.2.6
 Summary: Chia development commands
 Home-page: https://github.com/Chia-Network
 Author: Quexington
 Author-email: m.hauff@chia.net
 License: https://opensource.org/licenses/Apache-2.0
 Project-URL: Bug Reports, https://github.com/Chia-Network/chia-dev-tools
 Project-URL: Source, https://github.com/Chia-Network/chia-dev-tools
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 Requires-Dist: pytimeparse
 Requires-Dist: anyio
-Requires-Dist: chia-blockchain==2.2.1
+Requires-Dist: chia-blockchain==2.3.0
 Provides-Extra: dev
 Requires-Dist: anyio; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: types-aiofiles; extra == "dev"
 Requires-Dist: types-click; extra == "dev"
```

### Comparing `chia_dev_tools-1.2.5/README.md` & `chia_dev_tools-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/activated.py` & `chia_dev_tools-1.2.6/activated.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/clibs/condition_codes.clib` & `chia_dev_tools-1.2.6/cdv/clibs/condition_codes.clib`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/clibs/curry_and_treehash.clib` & `chia_dev_tools-1.2.6/cdv/clibs/curry_and_treehash.clib`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/clibs/singleton_truths.clib` & `chia_dev_tools-1.2.6/cdv/clibs/singleton_truths.clib`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/cmds/chia_inspect.py` & `chia_dev_tools-1.2.6/cdv/cmds/chia_inspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from chia.consensus.default_constants import DEFAULT_CONSTANTS
 from chia.full_node.bundle_tools import simple_solution_generator
 from chia.full_node.mempool_check_conditions import get_name_puzzle_conditions
 from chia.types.blockchain_format.coin import Coin
 from chia.types.blockchain_format.program import INFINITE_COST, Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.coin_record import CoinRecord
-from chia.types.coin_spend import CoinSpend
+from chia.types.coin_spend import CoinSpend, make_spend
 from chia.types.generator_types import BlockGenerator
 from chia.types.spend_bundle import SpendBundle
 from chia.util.byte_types import hexstr_to_bytes
 from chia.util.condition_tools import conditions_dict_for_solution, pkm_pairs_for_conditions_dict
 from chia.util.config import load_config
 from chia.util.default_root import DEFAULT_ROOT_PATH
 from chia.util.ints import uint32, uint64
@@ -160,14 +160,15 @@
     for obj in input_objects:
         if type(obj) == str:
             print(f"Could not guess the type of {obj}")
         elif type(obj) == Coin:  # type: ignore[comparison-overlap]
             assert isinstance(obj, Coin)  # mypy otherwise complains that obj is a str
             do_inspect_coin_cmd(ctx, [obj])
         elif type(obj) == CoinSpend:  # type: ignore[comparison-overlap]
+            assert isinstance(obj, CoinSpend)
             do_inspect_coin_spend_cmd(ctx, [obj])
         elif type(obj) == SpendBundle:  # type: ignore[comparison-overlap]
             do_inspect_spend_bundle_cmd(ctx, [obj])
         elif type(obj) == CoinRecord:  # type: ignore[comparison-overlap]
             do_inspect_coin_record_cmd(ctx, [obj])
         elif type(obj) == Program:
             do_inspect_program_cmd(ctx, [obj])
@@ -268,28 +269,28 @@
         del kwargs["cost"]
         del kwargs["ignore_byte_cost"]
     # If this is being built from the command line and the two required args are there
     if kwargs and all([kwargs["puzzle_reveal"], kwargs["solution"]]):
         # If they specified the coin components
         if (not kwargs["coin"]) and all([kwargs["parent_id"], kwargs["puzzle_hash"], kwargs["amount"]]):
             coin_spend_objs: List[CoinSpend] = [
-                CoinSpend(
+                make_spend(
                     Coin(
                         bytes32.from_hexstr(kwargs["parent_id"]),
                         bytes32.from_hexstr(kwargs["puzzle_hash"]),
                         uint64(kwargs["amount"]),
                     ),
                     parse_program(kwargs["puzzle_reveal"]),
                     parse_program(kwargs["solution"]),
                 )
             ]
         # If they specifed a coin object to parse
         elif kwargs["coin"]:
             coin_spend_objs = [
-                CoinSpend(
+                make_spend(
                     do_inspect_coin_cmd(ctx, [kwargs["coin"]], print_results=False)[0],
                     parse_program(kwargs["puzzle_reveal"]),
                     parse_program(kwargs["solution"]),
                 )
             ]
         else:
             print("Invalid arguments specified.")
```

### Comparing `chia_dev_tools-1.2.5/cdv/cmds/cli.py` & `chia_dev_tools-1.2.6/cdv/cmds/cli.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/cmds/clsp.py` & `chia_dev_tools-1.2.6/cdv/cmds/clsp.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/cmds/rpc.py` & `chia_dev_tools-1.2.6/cdv/cmds/rpc.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/cmds/util.py` & `chia_dev_tools-1.2.6/cdv/cmds/util.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/examples/clsp/piggybank.clsp` & `chia_dev_tools-1.2.6/cdv/examples/clsp/piggybank.clsp`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/examples/drivers/piggybank_drivers.py` & `chia_dev_tools-1.2.6/cdv/examples/drivers/piggybank_drivers.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/examples/tests/test_piggybank.py` & `chia_dev_tools-1.2.6/cdv/examples/tests/test_piggybank.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/test/__init__.py` & `chia_dev_tools-1.2.6/cdv/test/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pytimeparse
 from chia.clvm.spend_sim import SimClient, SpendSim
 from chia.consensus.default_constants import DEFAULT_CONSTANTS
 from chia.types.blockchain_format.coin import Coin
 from chia.types.blockchain_format.program import Program
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.types.coin_record import CoinRecord
-from chia.types.coin_spend import CoinSpend
+from chia.types.coin_spend import CoinSpend, make_spend
 from chia.types.spend_bundle import SpendBundle
 from chia.util.condition_tools import ConditionOpcode
 from chia.util.hash import std_hash
 from chia.util.ints import uint32, uint64
 from chia.wallet.derive_keys import master_sk_to_wallet_sk
 from chia.wallet.puzzles.p2_delegated_puzzle_or_hidden_puzzle import (  # standard_transaction
     DEFAULT_HIDDEN_PUZZLE_HASH,
@@ -451,21 +451,15 @@
                 delegated_puzzle_solution.get_tree_hash()
                 + found_coin.name()
                 + DEFAULT_CONSTANTS.AGG_SIG_ME_ADDITIONAL_DATA
             ),
         )
 
         spend_bundle = SpendBundle(
-            [
-                CoinSpend(
-                    found_coin.coin,  # Coin to spend
-                    self.puzzle,  # Puzzle used for found_coin
-                    solution,  # The solution to the puzzle locking found_coin
-                )
-            ],
+            [make_spend(found_coin.coin, self.puzzle, solution)],
             signature,
         )
         pushed: Dict[str, Union[str, List[Coin]]] = await self.parent.push_tx(spend_bundle)
         if "error" not in pushed:
             return cw.custom_coin(found_coin.coin, amt)
         else:
             return None
@@ -531,19 +525,15 @@
             delegated_puzzle_solution = Program.to((1, solution_list))
             # Solution is the solution for the old coin.
             solution = Program.to([[], delegated_puzzle_solution, []])
         else:
             delegated_puzzle_solution = Program.to(kwargs["args"])
             solution = delegated_puzzle_solution
 
-        solution_for_coin = CoinSpend(
-            coin.coin,
-            coin.puzzle(),
-            solution,
-        )
+        solution_for_coin = make_spend(coin.coin, coin.puzzle(), solution)
 
         # The reason this use of sign_coin_spends exists is that it correctly handles
         # the signing for non-standard coins.  I don't fully understand the difference but
         # this definitely does the right thing.
         try:
             spend_bundle: SpendBundle = await sign_coin_spends(
                 [solution_for_coin],
```

### Comparing `chia_dev_tools-1.2.5/cdv/test/test_skeleton.py` & `chia_dev_tools-1.2.6/cdv/test/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/util/keys.py` & `chia_dev_tools-1.2.6/cdv/util/keys.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/cdv/util/load_clvm.py` & `chia_dev_tools-1.2.6/cdv/util/load_clvm.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/chia_dev_tools.egg-info/PKG-INFO` & `chia_dev_tools-1.2.6/chia_dev_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chia_dev_tools
-Version: 1.2.5
+Version: 1.2.6
 Summary: Chia development commands
 Home-page: https://github.com/Chia-Network
 Author: Quexington
 Author-email: m.hauff@chia.net
 License: https://opensource.org/licenses/Apache-2.0
 Project-URL: Bug Reports, https://github.com/Chia-Network/chia-dev-tools
 Project-URL: Source, https://github.com/Chia-Network/chia-dev-tools
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: packaging
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 Requires-Dist: pytimeparse
 Requires-Dist: anyio
-Requires-Dist: chia-blockchain==2.2.1
+Requires-Dist: chia-blockchain==2.3.0
 Provides-Extra: dev
 Requires-Dist: anyio; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: types-aiofiles; extra == "dev"
 Requires-Dist: types-click; extra == "dev"
```

### Comparing `chia_dev_tools-1.2.5/chia_dev_tools.egg-info/SOURCES.txt` & `chia_dev_tools-1.2.6/chia_dev_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .flake8
 .gitignore
 .isort.cfg
 .markdown-lint.yml
 .pre-commit-config.yaml
+.repo-content-updater.yml
 LICENSE
 README.md
 activated.ps1
 activated.py
 activated.sh
 mypy.ini
 pyproject.toml
```

### Comparing `chia_dev_tools-1.2.5/mypy.ini` & `chia_dev_tools-1.2.6/mypy.ini`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/pyproject.toml` & `chia_dev_tools-1.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/setup.py` & `chia_dev_tools-1.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 dependencies = [
     "packaging",
     "pytest",
     "pytest-asyncio",
     "pytimeparse",
     "anyio",
-    "chia-blockchain==2.2.1",
+    "chia-blockchain==2.3.0",
 ]
 
 dev_dependencies = [
     "anyio",
     "flake8",
     "mypy",
     "black==24.4.2",
```

### Comparing `chia_dev_tools-1.2.5/tests/build-init-files.py` & `chia_dev_tools-1.2.6/tests/build-init-files.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/tests/cmds/object_files/spendbundles/spendbundle.json` & `chia_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'spend_bundle'": "{'coin_spends': {0: {'solution': '0x80'}}}"}*

```diff
@@ -5,12 +5,12 @@
             {
                 "coin": {
                     "amount": 0,
                     "parent_coin_info": "0x0000000000000000000000000000000000000000000000000000000000000000",
                     "puzzle_hash": "0x0000000000000000000000000000000000000000000000000000000000000000"
                 },
                 "puzzle_reveal": "0x01",
-                "solution": "80"
+                "solution": "0x80"
             }
         ]
     }
 }
```

### Comparing `chia_dev_tools-1.2.5/tests/cmds/object_files/spendbundles/spendbundle_invalid.json` & `chia_dev_tools-1.2.6/tests/cmds/object_files/spendbundles/spendbundle_invalid.json`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/tests/cmds/test_cdv.py` & `chia_dev_tools-1.2.6/tests/cmds/test_cdv.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/tests/cmds/test_clsp.py` & `chia_dev_tools-1.2.6/tests/cmds/test_clsp.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/tests/cmds/test_inspect.py` & `chia_dev_tools-1.2.6/tests/cmds/test_inspect.py`

 * *Files identical despite different names*

### Comparing `chia_dev_tools-1.2.5/tests/test_skeleton.py` & `chia_dev_tools-1.2.6/tests/test_skeleton.py`

 * *Files identical despite different names*


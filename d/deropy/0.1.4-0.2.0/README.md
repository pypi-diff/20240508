# Comparing `tmp/deropy-0.1.4.tar.gz` & `tmp/deropy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deropy-0.1.4.tar", last modified: Sun May  5 09:16:42 2024, max compression
+gzip compressed data, was "deropy-0.2.0.tar", last modified: Wed May  8 16:20:59 2024, max compression
```

## Comparing `deropy-0.1.4.tar` & `deropy-0.2.0.tar`

### file list

```diff
@@ -1,73 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:42.596910 deropy-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-05 09:16:38.000000 deropy-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-05 09:16:42.596910 deropy-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-05 09:16:38.000000 deropy-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:42.584910 deropy-0.1.4/deropy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:42.588910 deropy-0.1.4/deropy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/commands/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:42.588910 deropy-0.1.4/deropy/dvm/
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/Smartcontract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/Wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:42.596910 deropy-0.1.4/deropy/dvm/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/AddressRaw.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/AddressString.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/AssetValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Atoi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Blid.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/BlockHeight.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/BlockTimestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Dero.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/DeroValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Function.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/HexDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/IsAddressValid.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Itoa.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/MapDelete.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/MapExists.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/MapGet.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/MapStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Panic.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Random.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Scid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/SendAssetToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/SendDeroToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Sha3256.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Signer.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Store.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Strlen.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Substr.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/Txid.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/UpdateScCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/dvm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:42.596910 deropy-0.1.4/deropy/python_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/python_templates/Nameservice.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/python_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/python_templates/lottery.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/python_templates/minimum_sc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-05 09:16:38.000000 deropy-0.1.4/deropy/python_templates/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:42.596910 deropy-0.1.4/deropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-05 09:16:42.000000 deropy-0.1.4/deropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-05 09:16:42.000000 deropy-0.1.4/deropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 09:16:42.000000 deropy-0.1.4/deropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-05 09:16:42.000000 deropy-0.1.4/deropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 09:16:42.000000 deropy-0.1.4/deropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 09:16:42.000000 deropy-0.1.4/deropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 09:16:42.596910 deropy-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-05 09:16:38.000000 deropy-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:16:42.596910 deropy-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-05 09:16:38.000000 deropy-0.1.4/tests/test_compute_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-05 09:16:38.000000 deropy-0.1.4/tests/test_map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-05 09:16:38.000000 deropy-0.1.4/tests/test_storage_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.619024 deropy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-08 16:20:54.000000 deropy-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-08 16:20:59.615024 deropy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-08 16:20:54.000000 deropy-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.603024 deropy-0.2.0/deropy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.603024 deropy-0.2.0/deropy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/transpile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.603024 deropy-0.2.0/deropy/dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/Smartcontract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/Wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.607024 deropy-0.2.0/deropy/dvm/dast/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/assignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/binaryOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/dast_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/declaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/functionCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/functionDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/goto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/ifTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/variableDeclarationAdnAssignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/whileLoop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.611024 deropy-0.2.0/deropy/dvm/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/AddressRaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/AddressString.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/AssetValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Atoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Blid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/BlockHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/BlockTimestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Dero.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/DeroValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/HexDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/IsAddressValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Itoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/MapDelete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/MapExists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/MapGet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/MapStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Panic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Scid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/SendAssetToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/SendDeroToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Sha3256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Strlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Substr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Txid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/UpdateScCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.615024 deropy-0.2.0/deropy/dvm/iast/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/IastNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/assignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/binaryOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/functionCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/functionDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/iast_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/ifTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/variableDeclarationAdnAssignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/whileLoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.615024 deropy-0.2.0/deropy/python_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/Nameservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/lottery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/minimum_sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.615024 deropy-0.2.0/deropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:20:59.619024 deropy-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 16:20:54.000000 deropy-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.615024 deropy-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-08 16:20:54.000000 deropy-0.2.0/tests/test_compute_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-08 16:20:54.000000 deropy-0.2.0/tests/test_map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-08 16:20:54.000000 deropy-0.2.0/tests/test_storage_functions.py
```

### Comparing `deropy-0.1.4/LICENSE` & `deropy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/PKG-INFO` & `deropy-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.1.4
+Version: 0.2.0
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.1.4/README.md` & `deropy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/commands/deploy.py` & `deropy-0.2.0/deropy/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/commands/generate.py` & `deropy-0.2.0/deropy/commands/generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import click
 import os
 
 
+simulator_host = 'http://127.0.0.1:30000'
+
+
 @click.command('generate')
 @click.argument('file', type=click.Path())
 @click.option('-s', '--scid', type=str, help='The SCID of the smart contract', default='')
-def generate(file, scid):
-    _generate_class(file, scid)
-    _generate_tests(file)
+@click.option('--network', type=click.Choice(['simulator', 'mainnet']), default='simulator')
+@click.option('-o', '--output', type=click.Path(), help='The output file')
+def generate(file, scid, network, output):
+    _generate(file, scid, network, output)
+
+
+def _generate(file, scid, network, output):
+    host = simulator_host
+
+    _generate_class(file, scid, output)
+    # _generate_tests(file
 
 
 def _generate_tests(file):
     file_content = _read_bas(file)
     functions = _parse_function(file_content)
 
     lines = ['from SC import SC']
     lines += ['import unittest']
-    lines += ['']
+    lines += ['', '']
     lines += ['class TestSC(unittest.TestCase):']
     lines += ['']
     lines += ['    def setUp(self):']
     lines += ['        self.SC = SC()']
     lines += ['']
 
     for f, p in functions.items():
@@ -30,15 +41,15 @@
     os.makedirs('tests', exist_ok=True)
     with open('tests/test_SC.py', 'w') as f:
         for line in lines:
             f.write(f'{line}\n')
 
 
 def _generate_test_method(f_name, p):
-    lines = [f'\n    def test_{_camelCase_to_snake_case(f_name)}(self):']
+    lines = [f'\n    def test_{f_name}(self):']
 
     # Create a parameter map
     if len(p) != 0:
         lines += ['        params = {']
         for k, v in p.items():
             lines += [f'            "{k}": {_SC_type_to_python_fake(v)},']
         lines += ['        }']
@@ -51,19 +62,19 @@
     lines += ['            "id": "1",']
     lines += ['        }']
     lines += ['']
 
     # Create the method call
     lines += ['        # ---- Invoke the SC function (use the commented line if you need to setup fee)']
     if len(p) > 0:
-        lines += [f'        response_json = SC.{_camelCase_to_snake_case(f_name)}(**params)']
-        lines += [f'        #response_json = SC.{_camelCase_to_snake_case(f_name)}_fee(1000, **params)']
+        lines += [f'        response_json = SC.{f_name}(**params)']
+        lines += [f'        #response_json = SC.{f_name}_fee(1000, **params)']
     else:
-        lines += [f'        response_json = SC.{_camelCase_to_snake_case(f_name)}()']
-        lines += [f'        #response_json = SC.{_camelCase_to_snake_case(f_name)}_fee(1000)']
+        lines += [f'        response_json = SC.{f_name}()']
+        lines += [f'        #response_json = SC.{f_name}_fee(1000)']
 
     lines += ['']
 
     # Read the smart contract (could be needed to check variables)
     lines += ['        # ---- Read the smart contract (could be needed to check variables)']
     lines += ['        sc_content = self.sc.read()']
     lines += ['']
@@ -71,34 +82,40 @@
     # Create the assertion
     lines += ['        # ---- Your test here']
     lines += ['        self.assertEqual(1, 1)']
 
     return lines
 
 
-def _generate_class(file: str, scid: str):
+def _generate_class(file: str, scid: str, output: str = None):
     file_content = _read_bas(file)
     functions = _parse_function(file_content)
 
+    output_path = output if output is not None else 'SC.py'
+
+    class_name = os.path.basename(file)
+    class_name = class_name.split('.')[0]
+    class_name = class_name.capitalize()
+
     lines = ['import requests']
     lines += ['import json\n']
-    lines += ['class SC:']
+    lines += [f'class {class_name}:']
     lines += [f'    SCID="{scid}"']
     lines += ['    def __init__(self):']
-    lines += ["        self.url = 'http://127.0.0.1:30000/json_rpc'"]
+    lines += [f"        self.url = '{simulator_host}/json_rpc'"]
     lines += ["        self.headers = {'content-type': 'application/json'}"]
     lines += ['']
     lines.extend(_generate_read_method(scid))
     for f, p in functions.items():
-        scinvoce_method = _generate_method_scinvoce(f, p)
-        transfer2_method = _generate_method_transfer2(f, p)
+        scinvoce_method = _generate_method_scinvoce(f, p, class_name)
+        # transfer2_method = _generate_method_transfer2(f, p)
         lines.extend(scinvoce_method)
-        lines.extend(transfer2_method)
+        # lines.extend(transfer2_method)
 
-    with open('SC.py', 'w') as f:
+    with open(output_path, 'w') as f:
         for line in lines:
             f.write(f'{line}\n')
 
 
 def _read_bas(path: str) -> str:
     with open(path, 'r') as f:
         return f.readlines()
@@ -145,30 +162,32 @@
         '            "params": {',
         f'                "scid": "{scid}",',
         '                "code": True,',
         '                "variables": True',
         '            }',
         '        }',
         '        response = requests.post(url, data=json.dumps(payload), headers=self.headers)',
-        '        print(response.json())',
-        '        return response.json()'
+        '        # keep only the `stringkeys` and `variables`',
+        '        data = response.json()',
+        '        self.storage = data["result"]["stringkeys"]',
+        '        return self.storage',
     ]
 
 
-def _generate_method_scinvoce(f_name, p):
+def _generate_method_scinvoce(f_name, p, class_name):
     # create the method definition
     method_parameters = ''
     for k, v in p.items():
-        method_parameters += f'{k}:{_SC_type_to_python_type(v)}, '
+        method_parameters += f'{k}: {_SC_type_to_python_type(v)}, '
     method_parameters = method_parameters[:-2]
 
     if len(method_parameters) == 0:
-        lines = [f'\n    def {_camelCase_to_snake_case(f_name)}(self):']
+        lines = [f'\n    def {f_name}(self, dero_deposit: int = 0, asset_deposit: int = 0, host: str = None):']
     else:
-        lines = [f'\n    def {_camelCase_to_snake_case(f_name)}(self, {method_parameters}):']
+        lines = [f'\n    def {f_name}(self, {method_parameters}, dero_deposit: int = 0, asset_deposit: int = 0, host: str = None):']
 
     scrpc = [
         '                    "sc_rpc": [',
         '                        {',
         '                            "name": "entrypoint",',
         '                            "datatype": "S",',
         f'                            "value": "{f_name}"',
@@ -186,40 +205,50 @@
 
     payload = [
         '        payload = {',
         '                "jsonrpc": "2.0",',
         '                "id": "1",',
         '                "method": "scinvoke",',
         '                "params": {',
-        '                    "scid": SC.SCID,',
+        f'                    "scid": {class_name}.SCID,',
         '                    "ringsize": 2,',
     ]
+    if f_name != 'Initialize':
+        payload += [
+            '                    "sc_dero_deposit": dero_deposit,',
+            '                    "sc_asset_deposit": asset_deposit,',
+        ]
     payload += scrpc
     payload += [
         '                    ]',
         '                }',
         '            }',
     ]
     lines.extend(payload)
-    lines += ['        response = requests.post(self.url, data=json.dumps(payload), headers=self.headers)']
-    lines += ['        print(response.json())']
+    lines += [
+        '        import pprint',
+        '        pprint.pprint(payload)',
+        '        url = self.url if host is None else host',
+        '        print(f"using url {url}")',
+        '        response = requests.post(url, data=json.dumps(payload), headers=self.headers)',
+        '        pprint.pprint(response.json())']
     return lines
 
 
 def _generate_method_transfer2(f_name, p):
     # create the method definition
     method_parameters = ''
     for k, v in p.items():
         method_parameters += f'{k}:{_SC_type_to_python_type(v)}, '
     method_parameters = method_parameters[:-2]
 
     if len(method_parameters) == 0:
-        lines = [f'\n    def {_camelCase_to_snake_case(f_name)}_fee(self, fee: int):']
+        lines = [f'\n    def {f_name}_fee(self, fee: int):']
     else:
-        lines = [f'\n    def {_camelCase_to_snake_case(f_name)}_fee(self, fee: int, {method_parameters}):']
+        lines = [f'\n    def {f_name}_fee(self, fee: int, {method_parameters}):']
 
     scrpc = [
         '                    "sc_rpc": [',
         '                        {',
         '                            "name": "entrypoint",',
         '                            "datatype": "S",',
         f'                            "value": "{f_name}"',
@@ -278,10 +307,7 @@
 def _SC_type_to_jsonrpc(t: str):
     if t == "String":
         return "S"
     if t == "Uint64":
         return "U"
     raise RuntimeError(f'type {t} do not exist in DERO')
 
-
-def _camelCase_to_snake_case(name: str) -> str:
-    return ''.join(['_' + i.lower() if i.isupper() else i for i in name]).lstrip('_')
```

### Comparing `deropy-0.1.4/deropy/dvm/Smartcontract.py` & `deropy-0.2.0/deropy/dvm/Smartcontract.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,23 +33,32 @@
     def get_instance(cls):
         if not hasattr(cls, 'instance'):
             cls.instance = super(SmartContract, cls).__new__(cls)
             cls.instance._initialize()
         return cls.instance
 
     def _initialize(self):
-        self.storage = dict()
-        self.memory = dict()
-        self.gasStorage = []
-        self.gasCompute = []
+        SmartContract.storage = dict()
+        SmartContract.memory = dict()
+        SmartContract.gasStorage = []
+        SmartContract.gasCompute = []
 
         # At first instanciaion, create the smart-contract Id
         if SmartContract.scid is None:
             SmartContract.scid = sha256(str(time.time()*2).encode()).hexdigest()
 
+    def read(self):
+        return SmartContract.storage
+
+    def store(self, key, value):
+        SmartContract.storage[key] = value
+
+    def load(self, key):
+        return SmartContract.storage[key]
+
     @staticmethod
     def send_dero_with_tx(amount):
         SmartContract.dero_value = amount
 
     @staticmethod
     def send_asset_with_tx(amount, asset_id):
         if SmartContract.asset_value is None:
```

### Comparing `deropy-0.1.4/deropy/dvm/functions/AddressRaw.py` & `deropy-0.2.0/deropy/dvm/functions/AddressRaw.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/AddressString.py` & `deropy-0.2.0/deropy/dvm/functions/AddressString.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/AssetValue.py` & `deropy-0.2.0/deropy/dvm/functions/AssetValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Atoi.py` & `deropy-0.2.0/deropy/dvm/functions/Atoi.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/BlockHeight.py` & `deropy-0.2.0/deropy/dvm/functions/BlockHeight.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Dero.py` & `deropy-0.2.0/deropy/dvm/functions/Dero.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/DeroValue.py` & `deropy-0.2.0/deropy/dvm/functions/DeroValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Exists.py` & `deropy-0.2.0/deropy/dvm/functions/Exists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Function.py` & `deropy-0.2.0/deropy/dvm/functions/Function.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/IsAddressValid.py` & `deropy-0.2.0/deropy/dvm/functions/IsAddressValid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Itoa.py` & `deropy-0.2.0/deropy/dvm/functions/Itoa.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Keccak256.py` & `deropy-0.2.0/deropy/dvm/functions/Keccak256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Load.py` & `deropy-0.2.0/deropy/dvm/functions/Load.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 
         if len(loaded_value) < 10:
             return 1
         return len(loaded_value) // 10
 
     def _exec(self, *args, **kwargs):
         self.parameters["key"]["value"] = kwargs["key"]
-        return self.sc.storage[kwargs["key"]]
+        return self.sc.load(kwargs["key"])
 
 
 def load(key: str):
     return Load()(key=key)
```

### Comparing `deropy-0.1.4/deropy/dvm/functions/MapExists.py` & `deropy-0.2.0/deropy/dvm/functions/MapExists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/MapStore.py` & `deropy-0.2.0/deropy/dvm/functions/MapStore.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Random.py` & `deropy-0.2.0/deropy/dvm/functions/Random.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Scid.py` & `deropy-0.2.0/deropy/dvm/functions/Scid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/SendAssetToAddress.py` & `deropy-0.2.0/deropy/dvm/functions/SendAssetToAddress.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/SendDeroToAddress.py` & `deropy-0.2.0/deropy/dvm/functions/SendDeroToAddress.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Sha256.py` & `deropy-0.2.0/deropy/dvm/functions/Sha256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Sha3256.py` & `deropy-0.2.0/deropy/dvm/functions/Sha3256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Signer.py` & `deropy-0.2.0/deropy/dvm/functions/Signer.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/Store.py` & `deropy-0.2.0/deropy/dvm/functions/Store.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             "value": {"type": "Any", "value": None},
         }
         super().__init__("store", 10_000, 0, func_parameters)
 
     def _exec(self, *args, **kwargs):
         self.parameters["key"]["value"] = kwargs["key"]
         self.parameters["value"]["value"] = kwargs["value"]
-        self.sc.storage[kwargs["key"]] = kwargs["value"]
+        self.sc.store(kwargs["key"], kwargs["value"])
 
     def _computeGasStorageCost(self):
         if isinstance(self.parameters["value"]["value"], int):
             return 8
         else:
             return len(self.parameters["value"]["value"])
```

### Comparing `deropy-0.1.4/deropy/dvm/functions/Substr.py` & `deropy-0.2.0/deropy/dvm/functions/Substr.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/UpdateScCode.py` & `deropy-0.2.0/deropy/dvm/functions/UpdateScCode.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/functions/__init__.py` & `deropy-0.2.0/deropy/dvm/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/dvm/utils.py` & `deropy-0.2.0/deropy/dvm/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+import ast
+
 import hashlib
 
 
 def type_python_to_intermediate(python_hint):
     return {
         "int": "number",
         "str": "String"
@@ -24,23 +27,38 @@
             output.extend(flatten_list(i))
         else:
             output.append(i)
 
     return output
 
 
+def filter_args_out(args):
+    if isinstance(args, ast.arg):
+        if args.arg == 'self':
+            return False
+    return True
+
+
 def print_interpreter(msg: list):
+    try:
+        term_width = os.get_terminal_size().columns
+    except OSError:
+        term_width = 80
+
     def format_column(content, width):
         if len(content) > width:
             content = content[:width-3] + "..."
         else:
             content = content + " " * (width - len(content))
         return content
-
-    msg = f'{format_column(msg[0], 80)} {format_column(msg[1], 20)} {format_column(msg[2], 20)}'
+    
+    # split the terminal into three columns, 50%, 25%, 25%
+    widths = [int(term_width * 0.48), int(term_width * 0.25), int(term_width * 0.25)]
+    
+    msg = f'{format_column(msg[0], widths[0])} {format_column(msg[1], widths[1])} {format_column(msg[2], widths[2])}'
     print(msg)
 
 
 def get_address(id):
     return hashlib.sha256(str(id).encode()).hexdigest()
```

### Comparing `deropy-0.1.4/deropy/python_templates/Nameservice.py` & `deropy-0.2.0/deropy/python_templates/Nameservice.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/python_templates/lottery.py` & `deropy-0.2.0/deropy/python_templates/lottery.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,34 +3,33 @@
 
 
 @sc_logger(logger)
 class Lottery(SmartContract):
     def Initialize(self) -> int:
         if exists('owner') == 0:
             store('owner', signer())
-            store('lotteryeveryXdeposit', 2)
+            store('lotteryeveryXdeposit', 5)
             store('lotterygiveback', 9900)
             store('deposit_total', 0)
             store('deposit_count', 0)
             return 0
-        else:
-            return 1
+        return 1
 
-    def Lottery(self, value: int) -> int:
+    def Lottery(self, val: int) -> int:
         deposit_count: int = load("deposit_count") + 1
-        if value == 0:
+        if val == 0:
             return 0
-        store('depositor_address' + str(deposit_count - 1), signer())
-        store('deposit_total', load('deposit_total') + value)
+        store('depositor_address' + str(deposit_count), signer())
+        store('deposit_total', load('deposit_total') + val)
         store('deposit_count', deposit_count)
 
-        if load('lotteryeveryXdeposit') > deposit_count:
+        if load('lotteryeveryXdeposit') >= deposit_count:
             return 0
 
-        winner: int = random(0, deposit_count)
+        winner: int = random(deposit_count) + 1
         send_dero_to_address(load('depositor_address' + str(winner)), load('lotterygiveback')*load("deposit_total")/10000)
         store('deposit_total', 0)
         store('deposit_count', 0)
         return 0
 
     def TuneLotteryParameters(self, lotteryeveryXdeposit: int, lotterygiveback: int) -> int:
         if load('owner') != signer():
@@ -62,8 +61,8 @@
         return 0
 
     def UpdateCode(self, new_code: str) -> int:
         if load('owner') != signer():
             return 1
 
         update_sc_code(new_code)
-        return 0
+        return 0
```

### Comparing `deropy-0.1.4/deropy/python_templates/minimum_sc.py` & `deropy-0.2.0/deropy/python_templates/minimum_sc.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy/python_templates/token.py` & `deropy-0.2.0/deropy/python_templates/token.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/deropy.egg-info/PKG-INFO` & `deropy-0.2.0/deropy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.1.4
+Version: 0.2.0
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.1.4/deropy.egg-info/SOURCES.txt` & `deropy-0.2.0/deropy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,48 @@
 LICENSE
 README.md
 setup.py
 deropy/__init__.py
 deropy/main.py
+deropy/utils.py
 deropy.egg-info/PKG-INFO
 deropy.egg-info/SOURCES.txt
 deropy.egg-info/dependency_links.txt
 deropy.egg-info/entry_points.txt
 deropy.egg-info/requires.txt
 deropy.egg-info/top_level.txt
 deropy/commands/__init__.py
 deropy/commands/configure.py
 deropy/commands/deploy.py
 deropy/commands/generate.py
+deropy/commands/simulate.py
+deropy/commands/transpile.py
 deropy/dvm/Smartcontract.py
 deropy/dvm/Wallet.py
 deropy/dvm/__init__.py
+deropy/dvm/parser.py
+deropy/dvm/tester.py
 deropy/dvm/utils.py
+deropy/dvm/dast/__init__.py
+deropy/dvm/dast/argument.py
+deropy/dvm/dast/assignement.py
+deropy/dvm/dast/binaryOperator.py
+deropy/dvm/dast/compare.py
+deropy/dvm/dast/constant.py
+deropy/dvm/dast/dast_converter.py
+deropy/dvm/dast/declaration.py
+deropy/dvm/dast/functionCall.py
+deropy/dvm/dast/functionDef.py
+deropy/dvm/dast/goto.py
+deropy/dvm/dast/ifTest.py
+deropy/dvm/dast/name.py
+deropy/dvm/dast/operator.py
+deropy/dvm/dast/returns.py
+deropy/dvm/dast/variableDeclarationAdnAssignement.py
+deropy/dvm/dast/whileLoop.py
 deropy/dvm/functions/AddressRaw.py
 deropy/dvm/functions/AddressString.py
 deropy/dvm/functions/AssetValue.py
 deropy/dvm/functions/Atoi.py
 deropy/dvm/functions/Blid.py
 deropy/dvm/functions/BlockHeight.py
 deropy/dvm/functions/BlockTimestamp.py
@@ -49,14 +71,30 @@
 deropy/dvm/functions/Signer.py
 deropy/dvm/functions/Store.py
 deropy/dvm/functions/Strlen.py
 deropy/dvm/functions/Substr.py
 deropy/dvm/functions/Txid.py
 deropy/dvm/functions/UpdateScCode.py
 deropy/dvm/functions/__init__.py
+deropy/dvm/iast/IastNode.py
+deropy/dvm/iast/__init__.py
+deropy/dvm/iast/argument.py
+deropy/dvm/iast/assignement.py
+deropy/dvm/iast/binaryOperator.py
+deropy/dvm/iast/compare.py
+deropy/dvm/iast/constant.py
+deropy/dvm/iast/functionCall.py
+deropy/dvm/iast/functionDef.py
+deropy/dvm/iast/iast_converter.py
+deropy/dvm/iast/ifTest.py
+deropy/dvm/iast/name.py
+deropy/dvm/iast/operator.py
+deropy/dvm/iast/returns.py
+deropy/dvm/iast/variableDeclarationAdnAssignement.py
+deropy/dvm/iast/whileLoop.py
 deropy/python_templates/Nameservice.py
 deropy/python_templates/__init__.py
 deropy/python_templates/lottery.py
 deropy/python_templates/minimum_sc.py
 deropy/python_templates/token.py
 tests/test_compute_storage.py
 tests/test_map_functions.py
```

### Comparing `deropy-0.1.4/setup.py` & `deropy-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='deropy',
-    version=os.getenv('DEROPY_VERSION') or '0.1.4',
+    version=os.getenv('DEROPY_VERSION') or '0.2.0',
     url='https://github.com/dero-hyperbolic/deropy.git',
     author_email='leocances@gmail.com',
     description='A set of tool to help of DERO smart contract development',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `deropy-0.1.4/tests/test_compute_storage.py` & `deropy-0.2.0/tests/test_compute_storage.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/tests/test_map_functions.py` & `deropy-0.2.0/tests/test_map_functions.py`

 * *Files identical despite different names*

### Comparing `deropy-0.1.4/tests/test_storage_functions.py` & `deropy-0.2.0/tests/test_storage_functions.py`

 * *Files identical despite different names*


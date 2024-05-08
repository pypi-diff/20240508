# Comparing `tmp/vyper-0.4.0rc2.tar.gz` & `tmp/vyper-0.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vyper-0.4.0rc2.tar", last modified: Sun Apr 14 02:52:25 2024, max compression
+gzip compressed data, was "vyper-0.4.0rc3.tar", last modified: Wed May  8 16:11:14 2024, max compression
```

## Comparing `vyper-0.4.0rc2.tar` & `vyper-0.4.0rc3.tar`

### file list

```diff
@@ -1,587 +1,606 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.821169 vyper-0.4.0rc2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.753169 vyper-0.4.0rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.753169 vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/vip.md
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.753169 vyper-0.4.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/era-tester.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/ghcr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/release-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-14 02:52:25.821169 vyper-0.4.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.757169 vyper-0.4.0rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.757169 vyper-0.4.0rc2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (127)    38119 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/built-in-functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/compiler-exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/compiling-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/constants-and-vars.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/control-structures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/deploying-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/event-logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/installing-vyper.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/natspec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/scoping-and-declarations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/statements.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/structure-of-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/style-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/testing-contracts-brownie.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/testing-contracts-ethtester.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/testing-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/docs/vyper-by-example.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.757169 vyper-0.4.0rc2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/auctions/blind_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/auctions/simple_open_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/crowdfund.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/factory/Exchange.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/factory/Factory.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/market_maker/on_chain_market_maker.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/name_registry/name_registry.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/safe_remote_purchase/safe_remote_purchase.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/stock/
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/stock/company.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/storage/advanced_storage.vy
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/storage/storage.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/tokens/ERC1155ownable.vy
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/tokens/ERC20.vy
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/tokens/ERC4626.vy
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/tokens/ERC721.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/voting/ballot.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/examples/wallet/wallet.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/hooks/build
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/make.cmd
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/quicktest.sh
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-14 02:52:25.821169 vyper-0.4.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19787 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/fixtures/memorymock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.761169 vyper-0.4.0rc2/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.745169 vyper-0.4.0rc2/tests/functional/builtins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.765169 vyper-0.4.0rc2/tests/functional/builtins/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_addmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)    20923 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19720 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_create_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ecrecover.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_is_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)    16894 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/codegen/test_unsafe_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.769169 vyper-0.4.0rc2/tests/functional/builtins/folding/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_addmod_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_floor_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_fold_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_keccak_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/builtins/folding/test_powmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.769169 vyper-0.4.0rc2/tests/functional/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.769169 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_default_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_default_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_erc20_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    59140 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_self_call_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.769169 vyper-0.4.0rc2/tests/functional/codegen/environment_variables/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/environment_variables/test_block_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/environment_variables/test_blockhash.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/environment_variables/test_tx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.773169 vyper-0.4.0rc2/tests/functional/codegen/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.773169 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_private.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_pure.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.773169 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_break.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_for_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_range_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_address_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_assert_unreachable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_bytes_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    16224 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_clampers.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_immutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    15764 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_internal_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    33812 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_logging_bytes_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_logging_from_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_memory_alloc.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_memory_dealloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_reverting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_short_circuiting.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_string_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/features/test_transient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.773169 vyper-0.4.0rc2/tests/functional/codegen/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/integration/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/integration/test_crowdfund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/integration/test_escrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.777169 vyper-0.4.0rc2/tests/functional/codegen/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_flag_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_interface_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_module_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_module_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/modules/test_stateless_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.777169 vyper-0.4.0rc2/tests/functional/codegen/storage_variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_setters.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_storage_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/test_call_graph_stability.py
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/test_selector_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/test_selector_table_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.777169 vyper-0.4.0rc2/tests/functional/codegen/types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8450 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_decimals.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_division.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_exponents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_isqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_modulo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_signed_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_sqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_unsigned_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_array_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes_zero_padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    50402 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_identifier_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    23876 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_node_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/codegen/types/test_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/auctions/test_blind_auction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/auctions/test_simple_open_auction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/company/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/company/test_company.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/crowdfund/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/crowdfund/test_crowdfund_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/factory/test_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/market_maker/test_on_chain_market_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/name_registry/test_name_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/storage/test_advanced_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/storage/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc1155.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc4626.py
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc721.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/voting/test_ballot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/examples/wallet/test_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.781169 vyper-0.4.0rc2/tests/functional/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/grammar/test_grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.789169 vyper-0.4.0rc2/tests/functional/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/functional/syntax/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_argument_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_call_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_constancy_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_function_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_instantiation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_type_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_namespace_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_overflow_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_structure_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_syntax_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_undeclared_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/functional/syntax/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/test_deploy_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/test_implements.py
--rw-r--r--   0 runner    (1001) docker     (127)    28241 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/modules/test_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/functional/syntax/names/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/names/test_event_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/names/test_function_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/names/test_variable_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/functional/syntax/signatures/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/signatures/test_invalid_function_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/signatures/test_method_id_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_addmulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_address_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_ann_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_as_uint256.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_blockscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_bool_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_chainid.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_code_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_codehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_create_with_code_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_external_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_functions_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_immutables.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_invalids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_msg_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_nested_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_no_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_powmod.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_return_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_self_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_selfdestruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_tuple_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/functional/syntax/test_unbalanced_return.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/unit/abi_types/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/abi_types/test_invalid_abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.793169 vyper-0.4.0rc2/tests/unit/ast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/ast/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_compare_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_binop_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_binop_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_boolop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_unaryop.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_from_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_get_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_get_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/nodes/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_annotate_and_optimize_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_ast_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_metadata_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/ast/test_source_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.749169 vyper-0.4.0rc2/tests/unit/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/cli/storage_layout/
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/storage_layout/test_storage_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/cli/vyper_compile/
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_compile/test_compile_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_compile/test_parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/cli/vyper_json/
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_compile_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_get_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_get_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_output_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.797169 vyper-0.4.0rc2/tests/unit/compiler/asm/
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/asm/test_asm_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/compiler/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_calldatacopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_optimize_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_repeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/ir/test_with.py
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_bytecode_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_compile_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_sha3_32.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/test_source_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/compiler/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_convert_basicblock_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_dominator_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_duplicate_operands.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_liveness_simple_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_multi_entry_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_stack_at_external_return.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/compiler/venom/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/semantics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/analysis/test_array_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/analysis/test_cyclic_function_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/analysis/test_for_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/analysis/test_potential_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/test_storage_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_pure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_size_in_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_type_from_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/semantics/types/test_type_from_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.801169 vyper-0.4.0rc2/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/unit/utils/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.805169 vyper-0.4.0rc2/vyper/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.805169 vyper-0.4.0rc2/vyper/ast/
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/grammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    46130 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.809169 vyper-0.4.0rc2/vyper/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/_signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    91096 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.809169 vyper-0.4.0rc2/vyper/builtins/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC165.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC20.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC20Detailed.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC4626.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/builtins/interfaces/IERC721.vyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.809169 vyper-0.4.0rc2/vyper/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10533 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/cli/vyper_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/cli/vyper_ir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15843 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/cli/vyper_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.809169 vyper-0.4.0rc2/vyper/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/abi_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    42565 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    30728 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/external_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/codegen/function_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/function_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/function_definitions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/function_definitions/external_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/function_definitions/internal_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/ir_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/jumptable_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/keccak256_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/memory_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/return_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/self_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/codegen/stmt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/compiler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/evm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/evm/address_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/evm/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/ir/
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45834 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/ir/s_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.813169 vyper-0.4.0rc2/vyper/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.817169 vyper-0.4.0rc2/vyper/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/constant_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/data_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/global_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/import_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/levenshtein_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37264 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    36587 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/data_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.817169 vyper-0.4.0rc2/vyper/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/bytestrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    30949 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    12439 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/subscriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/semantics/types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.817169 vyper-0.4.0rc2/vyper/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15338 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/basicblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/bb_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/dominators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/ir_node_to_venom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.821169 vyper-0.4.0rc2/vyper/venom/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/base_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/constant_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/dft.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/simplify_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/passes/stack_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/stack_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/venom/venom_to_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 02:52:22.000000 vyper-0.4.0rc2/vyper/vyper_git_commithash.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-14 02:52:16.000000 vyper-0.4.0rc2/vyper/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:52:25.805169 vyper-0.4.0rc2/vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20397 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 02:52:25.000000 vyper-0.4.0rc2/vyper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.832811 vyper-0.4.0rc3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.832811 vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/vip.md
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.832811 vyper-0.4.0rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/era-tester.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/ghcr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-08 16:11:14.904812 vyper-0.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (127)    39020 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/built-in-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/compiler-exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/compiling-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/constants-and-vars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/control-structures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/deploying-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/event-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/installing-vyper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/natspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/scoping-and-declarations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/statements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/structure-of-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/style-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/testing-contracts-brownie.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/testing-contracts-ethtester.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/testing-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/docs/vyper-by-example.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/auctions/blind_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/auctions/simple_open_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/crowdfund.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/factory/Exchange.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/factory/Factory.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/market_maker/on_chain_market_maker.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/name_registry/name_registry.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/safe_remote_purchase/safe_remote_purchase.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.836812 vyper-0.4.0rc3/examples/stock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/stock/company.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/storage/advanced_storage.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/storage/storage.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/tokens/ERC1155ownable.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/tokens/ERC20.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/tokens/ERC4626.vy
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/tokens/ERC721.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/voting/ballot.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/examples/wallet/wallet.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/hooks/build
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/make.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/quicktest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-08 16:11:14.904812 vyper-0.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/tests/evm_backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/abi_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/base_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/pyevm_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/evm_backends/revm_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.840812 vyper-0.4.0rc3/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.824812 vyper-0.4.0rc3/tests/functional/builtins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.844812 vyper-0.4.0rc3/tests/functional/builtins/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_addmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_blobhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20237 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_create_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ecrecover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_is_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16628 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14884 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/codegen/test_unsafe_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.848812 vyper-0.4.0rc3/tests/functional/builtins/folding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_addmod_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_floor_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_fold_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_keccak_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/builtins/folding/test_powmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.848812 vyper-0.4.0rc3/tests/functional/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.848812 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_default_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_default_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_erc20_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57029 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_self_call_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.848812 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_blobbasefee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_block_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_blockhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/environment_variables/test_tx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.852812 vyper-0.4.0rc3/tests/functional/codegen/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.852812 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_pure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.856812 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_for_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_range_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_address_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_assert_unreachable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_bytes_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_clampers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_immutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_internal_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27866 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_logging_bytes_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_logging_from_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_memory_alloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_memory_dealloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_short_circuiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_string_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/features/test_transient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.856812 vyper-0.4.0rc3/tests/functional/codegen/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/integration/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/integration/test_crowdfund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/integration/test_escrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.856812 vyper-0.4.0rc3/tests/functional/codegen/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_flag_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_interface_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_module_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_module_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/modules/test_stateless_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.856812 vyper-0.4.0rc3/tests/functional/codegen/storage_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_storage_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/test_call_graph_stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15992 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/test_selector_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/test_selector_table_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/codegen/types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_decimals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_exponents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_isqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_modulo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_signed_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_unsigned_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_array_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes_zero_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48925 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_identifier_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23216 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_node_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/codegen/types/test_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.824812 vyper-0.4.0rc3/tests/functional/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/auctions/test_blind_auction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/auctions/test_simple_open_auction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/company/
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/company/test_company.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/crowdfund/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/crowdfund/test_crowdfund_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/factory/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/market_maker/test_on_chain_market_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/name_registry/test_name_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.860812 vyper-0.4.0rc3/tests/functional/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/storage/test_advanced_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/storage/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.864812 vyper-0.4.0rc3/tests/functional/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc4626.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc721.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.864812 vyper-0.4.0rc3/tests/functional/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/voting/test_ballot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.864812 vyper-0.4.0rc3/tests/functional/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/examples/wallet/test_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.864812 vyper-0.4.0rc3/tests/functional/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/grammar/test_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.872812 vyper-0.4.0rc3/tests/functional/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.872812 vyper-0.4.0rc3/tests/functional/syntax/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_argument_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_call_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_constancy_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_function_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_instantiation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_type_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_namespace_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_overflow_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_structure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_syntax_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_undeclared_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.872812 vyper-0.4.0rc3/tests/functional/syntax/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/test_deploy_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/test_implements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28241 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/modules/test_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/functional/syntax/names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/names/test_event_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/names/test_function_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/names/test_variable_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/functional/syntax/signatures/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/signatures/test_invalid_function_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/signatures/test_method_id_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_addmulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_address_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_ann_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_as_uint256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_blockscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_bool_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_chainid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_code_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_codehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_create_with_code_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_external_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_functions_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_immutables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_invalids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_msg_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_nested_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_no_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_powmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_return_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_self_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_selfdestruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_tuple_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/functional/syntax/test_unbalanced_return.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/abi_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/abi_types/test_invalid_abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/ast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/ast/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_compare_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_binop_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_binop_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_boolop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_unaryop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_from_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_get_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_get_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/nodes/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_annotate_and_optimize_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_ast_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_metadata_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/ast/test_source_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.824812 vyper-0.4.0rc3/tests/unit/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/cli/storage_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/storage_layout/test_storage_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.876812 vyper-0.4.0rc3/tests/unit/cli/vyper_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)    12444 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_compile/test_compile_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_compile/test_parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/cli/vyper_json/
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_compile_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_get_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_output_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/compiler/asm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/asm/test_asm_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/compiler/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_calldatacopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_optimize_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/ir/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_bytecode_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_compile_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8697 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_sha3_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/test_source_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.880812 vyper-0.4.0rc3/tests/unit/compiler/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_convert_basicblock_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_dominator_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_duplicate_operands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_liveness_simple_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_multi_entry_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_sccp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_stack_at_external_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/compiler/venom/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/tests/unit/semantics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/tests/unit/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/analysis/test_array_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/analysis/test_cyclic_function_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/analysis/test_for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/analysis/test_potential_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/test_storage_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/tests/unit/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_pure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_size_in_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_type_from_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/semantics/types/test_type_from_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/unit/utils/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/vyper/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.888812 vyper-0.4.0rc3/vyper/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.888812 vyper-0.4.0rc3/vyper/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91585 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.888812 vyper-0.4.0rc3/vyper/builtins/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC165.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC20.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC20Detailed.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC4626.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/builtins/interfaces/IERC721.vyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.888812 vyper-0.4.0rc3/vyper/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/compile_archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13215 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/vyper_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/vyper_ir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15923 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/cli/vyper_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.892812 vyper-0.4.0rc3/vyper/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/abi_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13045 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42566 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30724 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/external_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.892812 vyper-0.4.0rc3/vyper/codegen/function_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/function_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/function_definitions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/function_definitions/external_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/function_definitions/internal_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/ir_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/jumptable_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/keccak256_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/memory_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/return_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/self_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/codegen/stmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.892812 vyper-0.4.0rc3/vyper/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/output_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/compiler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.892812 vyper-0.4.0rc3/vyper/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/evm/address_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/evm/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.896812 vyper-0.4.0rc3/vyper/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45899 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/ir/s_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.896812 vyper-0.4.0rc3/vyper/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.896812 vyper-0.4.0rc3/vyper/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/constant_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/data_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/global_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/import_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/levenshtein_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37264 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/data_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/bytestrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30949 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18935 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/subscriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/semantics/types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/venom/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/dfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/dominators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/dup_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/analysis/liveness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16433 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/basicblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19028 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/ir_node_to_venom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/venom/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/base_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/mem2var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/remove_unused_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.900812 vyper-0.4.0rc3/vyper/venom/passes/sccp/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/sccp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/sccp/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/sccp/sccp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/simplify_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/passes/stack_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/stack_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20025 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/venom/venom_to_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 16:11:11.000000 vyper-0.4.0rc3/vyper/vyper_git_commithash.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-08 16:11:03.000000 vyper-0.4.0rc3/vyper/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:11:14.884812 vyper-0.4.0rc3/vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21016 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 16:11:14.000000 vyper-0.4.0rc3/vyper.egg-info/top_level.txt
```

### Comparing `vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/bug.md` & `vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/.github/ISSUE_TEMPLATE/vip.md` & `vyper-0.4.0rc3/.github/ISSUE_TEMPLATE/vip.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/.github/workflows/build.yml` & `vyper-0.4.0rc3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/.github/workflows/codeql.yml` & `vyper-0.4.0rc3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/.github/workflows/era-tester.yml` & `vyper-0.4.0rc3/.github/workflows/era-tester.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/.github/workflows/ghcr.yml` & `vyper-0.4.0rc3/.github/workflows/ghcr.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/.github/workflows/pull-request.yaml` & `vyper-0.4.0rc3/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/.github/workflows/release-pypi.yml` & `vyper-0.4.0rc3/.github/workflows/release-pypi.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/.github/workflows/test.yml` & `vyper-0.4.0rc3/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -66,69 +66,99 @@
     strategy:
       matrix:
         python-version: [["3.11", "311"]]
         opt-mode: ["gas", "none", "codesize"]
         debug: [true, false]
         evm-version: [shanghai]
         experimental-codegen: [false]
-        memorymock: [false]
+        evm-backend: [revm]
 
         # https://docs.github.com/en/actions/using-jobs/using-a-matrix-for-your-jobs#expanding-or-adding-matrix-configurations
         include:
           # test default settings with 3.11 across all supported evm versions
           - python-version: ["3.11", "311"]
             debug: false
             opt-mode: gas
             evm-version: london
+            evm-backend: revm
+
           - python-version: ["3.11", "311"]
             debug: false
             opt-mode: gas
             evm-version: paris
+            evm-backend: revm
 
           # redundant rule, for clarity
           - python-version: ["3.11", "311"]
             debug: false
             opt-mode: gas
             evm-version: shanghai
+            evm-backend: revm
+
+          - python-version: ["3.11", "311"]
+            debug: false
+            opt-mode: gas
+            evm-version: cancun
+            evm-backend: revm
+
+          # py-evm rules
+          - python-version: ["3.11", "311"]
+            debug: false
+            opt-mode: codesize
+            evm-version: london
+            evm-backend: py-evm
 
           - python-version: ["3.11", "311"]
             debug: false
             opt-mode: gas
             evm-version: cancun
+            evm-backend: py-evm
 
           # test experimental pipeline
           - python-version: ["3.11", "311"]
             opt-mode: gas
             debug: false
             evm-version: shanghai
+            evm-backend: revm
             experimental-codegen: true
-          # TODO: test experimental_codegen + -Ocodesize
 
-          # run with `--memorymock`, but only need to do it one configuration
-          # TODO: consider removing the memorymock tests
           - python-version: ["3.11", "311"]
-            opt-mode: gas
+            opt-mode: codesize
             debug: false
             evm-version: shanghai
-            memorymock: true
+            evm-backend: revm
+            experimental-codegen: true
+
+          - python-version: ["3.11", "311"]
+            opt-mode: none
+            debug: false
+            evm-version: shanghai
+            evm-backend: revm
+            experimental-codegen: true
 
           # run across other python versions. we don't really need to run all
           # modes across all python versions - one is enough
           - python-version: ["3.10", "310"]
             opt-mode: gas
             debug: false
             evm-version: shanghai
+            evm-backend: revm
 
           - python-version: ["3.12", "312"]
             opt-mode: gas
             debug: false
             evm-version: shanghai
+            evm-backend: revm
 
-
-    name: py${{ matrix.python-version[1] }}-opt-${{ matrix.opt-mode }}${{ matrix.debug && '-debug' || '' }}${{ matrix.memorymock && '-memorymock' || '' }}${{ matrix.experimental-codegen && '-experimental' || '' }}-${{ matrix.evm-version }}
+    name: "py${{ matrix.python-version[1] }}\
+      -opt-${{ matrix.opt-mode }}\
+      ${{ matrix.debug && '-debug' || '' }}\
+      ${{ matrix.experimental-codegen && '-experimental' || '' }}\
+      -${{ matrix.evm-version }}\
+      -${{ matrix.evm-backend }}"
 
     steps:
     - uses: actions/checkout@v4
       with:
           # need to fetch unshallow so that setuptools_scm can infer the version
           fetch-depth: 0
 
@@ -146,24 +176,24 @@
 
     - name: Run tests
       run: |
         pytest \
           -m "not fuzzing" \
           --optimize ${{ matrix.opt-mode }} \
           --evm-version ${{ matrix.evm-version }} \
+          ${{ matrix.evm-backend && format('--evm-backend {0}', matrix.evm-backend) || '' }} \
           ${{ matrix.debug && '--enable-compiler-debug-mode' || '' }} \
-          ${{ matrix.memorymock && '--memorymock' || '' }} \
           ${{ matrix.experimental-codegen && '--experimental-codegen' || '' }} \
           --cov-branch \
           --cov-report xml:coverage.xml \
           --cov=vyper \
           tests/
 
     - name: Upload Coverage
-      uses: codecov/codecov-action@v4
+      uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
 
 
   core-tests-success:
     if: always()
@@ -216,15 +246,15 @@
           --splitting-algorithm least_duration \
           --cov-branch \
           --cov-report xml:coverage.xml \
           --cov=vyper \
           tests/
 
     - name: Upload Coverage
-      uses: codecov/codecov-action@v4
+      uses: codecov/codecov-action@v3
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
 
   slow-tests-success:
     if: always()
     # summary result from test matrix.
```

### Comparing `vyper-0.4.0rc2/.pre-commit-config.yaml` & `vyper-0.4.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/Dockerfile` & `vyper-0.4.0rc3/Dockerfile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/LICENSE` & `vyper-0.4.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/Makefile` & `vyper-0.4.0rc3/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 		--implicit-optional \
 		-p vyper
 
 black:
 	black -C -t py311 vyper/ tests/ setup.py --force-exclude=vyper/version.py
 
 flake8: black
-	flake8 vyper/ tests/
+	flake8 --enable-extensions=FS003 vyper/ tests/
 
 isort: black
 	isort vyper/ tests/ setup.py
 
 docs:
 	rm -f docs/vyper.rst
 	rm -f docs/modules.rst
```

### Comparing `vyper-0.4.0rc2/PKG-INFO` & `vyper-0.4.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0rc2
+Version: 0.4.0rc3
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0rc2/README.md` & `vyper-0.4.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/Makefile` & `vyper-0.4.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/_templates/versions.html` & `vyper-0.4.0rc3/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/built-in-functions.rst` & `vyper-0.4.0rc3/docs/built-in-functions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -945,14 +945,38 @@
             return blockhash(block.number - 16)
 
     .. code-block:: vyper
 
         >>> ExampleContract.foo()
         0xf3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855
 
+.. py:function:: blobhash(index: uint256) -> bytes32
+
+    Return the versioned hash of the ``index``-th BLOB associated with the current transaction.
+
+    .. note::
+
+         A versioned hash consists of a single byte representing the version (currently ``0x01``), followed by the last 31 bytes of the ``SHA256`` hash of the KZG commitment (`EIP-4844 <https://eips.ethereum.org/EIPS/eip-4844>`_). For the case ``index >= len(tx.blob_versioned_hashes)``, ``blobhash(index: uint256)`` returns ``empty(bytes32)``.
+
+    .. code-block:: vyper
+
+        @external
+        @view
+        def foo(index: uint256) -> bytes32:
+            return blobhash(index)
+
+    .. code-block:: vyper
+
+        >>> ExampleContract.foo(0)
+        0xfd28610fb309939bfec12b6db7c4525446f596a5a5a66b8e2cb510b45b2bbeb5
+
+        >>> ExampleContract.foo(6)
+        0x0000000000000000000000000000000000000000000000000000000000000000
+
+
 .. py:function:: empty(typename) -> Any
 
     Return a value which is the default (zero-ed) value of its type. Useful for initializing new memory variables.
 
     * ``typename``: Name of the type, except ``HashMap[_KeyType, _ValueType]``
 
     .. code-block:: vyper
```

### Comparing `vyper-0.4.0rc2/docs/compiler-exceptions.rst` & `vyper-0.4.0rc3/docs/compiler-exceptions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/compiling-a-contract.rst` & `vyper-0.4.0rc3/docs/compiling-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/conf.py` & `vyper-0.4.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/constants-and-vars.rst` & `vyper-0.4.0rc3/docs/constants-and-vars.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,34 @@
 =====================
 
 Environment variables always exist in the namespace and are primarily used to provide information about the blockchain or current transaction.
 
 Block and Transaction Properties
 --------------------------------
 
-==================== ================ =========================================================
-Name                 Type             Value
-==================== ================ =========================================================
-``block.coinbase``   ``address``      Current block miner's address
-``block.difficulty`` ``uint256``      Current block difficulty
-``block.prevrandao`` ``bytes32``      Current randomness beacon provided by the beacon chain
-``block.number``     ``uint256``      Current block number
-``block.prevhash``   ``bytes32``      Equivalent to ``blockhash(block.number - 1)``
-``block.timestamp``  ``uint256``      Current block epoch timestamp
-``chain.id``         ``uint256``      Chain ID
-``msg.data``         ``Bytes``        Message data
-``msg.gas``          ``uint256``      Remaining gas
-``msg.sender``       ``address``      Sender of the message (current call)
-``msg.value``        ``uint256``      Number of wei sent with the message
-``tx.origin``        ``address``      Sender of the transaction (full call chain)
-``tx.gasprice``      ``uint256``      Gas price of current transaction in wei
-==================== ================ =========================================================
+===================== ================ =========================================================
+Name                  Type             Value
+===================== ================ =========================================================
+``block.coinbase``    ``address``      Current block miner's address
+``block.difficulty``  ``uint256``      Current block difficulty
+``block.prevrandao``  ``bytes32``      Current randomness beacon provided by the beacon chain
+``block.number``      ``uint256``      Current block number
+``block.gaslimit``    ``uint256``      Current block's gas limit
+``block.basefee``     ``uint256``      Current block's base fee
+``block.blobbasefee`` ``uint256``      Current block's blob gas base fee
+``block.prevhash``    ``bytes32``      Equivalent to ``blockhash(block.number - 1)``
+``block.timestamp``   ``uint256``      Current block epoch timestamp
+``chain.id``          ``uint256``      Chain ID
+``msg.data``          ``Bytes``        Message data
+``msg.gas``           ``uint256``      Remaining gas
+``msg.sender``        ``address``      Sender of the message (current call)
+``msg.value``         ``uint256``      Number of wei sent with the message
+``tx.origin``         ``address``      Sender of the transaction (full call chain)
+``tx.gasprice``       ``uint256``      Gas price of current transaction in wei
+===================== ================ =========================================================
 
 .. note::
 
     ``block.prevrandao`` is an alias for the ``block.difficulty`` opcode. Since ``block.difficulty`` is considered deprecated according to `EIP-4399 <https://eips.ethereum.org/EIPS/eip-4399>`_ after "The Merge" (Paris hard fork), we recommend using ``block.prevrandao``.
 
 .. note::
```

### Comparing `vyper-0.4.0rc2/docs/contributing.rst` & `vyper-0.4.0rc3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/control-structures.rst` & `vyper-0.4.0rc3/docs/control-structures.rst`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 You can put the ``@nonreentrant`` decorator on a ``__default__`` function but we recommend against it because in most circumstances it will not work in a meaningful way.
 
 Nonreentrancy locks work by setting a specially allocated storage slot to a ``<locked>`` value on function entrance, and setting it to an ``<unlocked>`` value on function exit. On function entrance, if the storage slot is detected to be the ``<locked>`` value, execution reverts.
 
 You cannot put the ``@nonreentrant`` decorator on a ``pure`` function. You can put it on a ``view`` function, but it only checks that the function is not in a callback (the storage slot is not in the ``<locked>`` state), as ``view`` functions can only read the state, not change it.
 
-You can view where the nonreentrant key is physically laid out in storage by using ``vyper`` with the ``-f layout`` option (e.g., ``vyper -f layout foo.vy``). Unless it is overriden, the compiler will allocate it at slot ``0``.
+You can view where the nonreentrant key is physically laid out in storage by using ``vyper`` with the ``-f layout`` option (e.g., ``vyper -f layout foo.vy``). Unless it is overridden, the compiler will allocate it at slot ``0``.
 
 .. note::
     A mutable function can protect a ``view`` function from being called back into (which is useful for instance, if a ``view`` function would return inconsistent state during a mutable function), but a ``view`` function cannot protect itself from being called back into. Note that mutable functions can never be called from a ``view`` function because all external calls out from a ``view`` function are protected by the use of the ``STATICCALL`` opcode.
 
 .. note::
 
     A nonreentrant lock has an ``<unlocked>`` value of 3, and a ``<locked>`` value of 2. Nonzero values are used to take advantage of net gas metering - as of the Berlin hard fork, the net cost for utilizing a nonreentrant lock is 2300 gas. Prior to v0.3.4, the ``<unlocked>`` and ``<locked>`` values were 0 and 1, respectively.
```

### Comparing `vyper-0.4.0rc2/docs/deploying-contracts.rst` & `vyper-0.4.0rc3/docs/deploying-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/event-logging.rst` & `vyper-0.4.0rc3/docs/event-logging.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/index.rst` & `vyper-0.4.0rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/installing-vyper.rst` & `vyper-0.4.0rc3/docs/installing-vyper.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/interfaces.rst` & `vyper-0.4.0rc3/docs/interfaces.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/logo.svg` & `vyper-0.4.0rc3/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/make.bat` & `vyper-0.4.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/natspec.rst` & `vyper-0.4.0rc3/docs/natspec.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/release-notes.rst` & `vyper-0.4.0rc3/docs/release-notes.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/resources.rst` & `vyper-0.4.0rc3/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/scoping-and-declarations.rst` & `vyper-0.4.0rc3/docs/scoping-and-declarations.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/statements.rst` & `vyper-0.4.0rc3/docs/statements.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/structure-of-a-contract.rst` & `vyper-0.4.0rc3/docs/structure-of-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/style-guide.rst` & `vyper-0.4.0rc3/docs/style-guide.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/testing-contracts-brownie.rst` & `vyper-0.4.0rc3/docs/testing-contracts-brownie.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/testing-contracts-ethtester.rst` & `vyper-0.4.0rc3/docs/testing-contracts-ethtester.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/testing-contracts.rst` & `vyper-0.4.0rc3/docs/testing-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/toctree.rst` & `vyper-0.4.0rc3/docs/toctree.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/types.rst` & `vyper-0.4.0rc3/docs/types.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/versioning.rst` & `vyper-0.4.0rc3/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/docs/vyper-by-example.rst` & `vyper-0.4.0rc3/docs/vyper-by-example.rst`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 not equal to zero pass, we can safely conclude that we have a valid new highest bid.
 We will send back the previous ``highestBid`` to the previous ``highestBidder`` and set
 our new ``highestBid`` and ``highestBidder``.
 
 .. literalinclude:: ../examples/auctions/simple_open_auction.vy
   :language: vyper
   :lineno-start: 60
-  :lines: 60-85
+  :lines: 60-87
 
 With the ``endAuction()`` method, we check whether our current time is past
 the ``auctionEnd`` time we set upon initialization of the contract. We also
 check that ``self.ended`` had not previously been set to True. We do this
 to prevent any calls to the method if the auction had already ended,
 which could potentially be malicious if the check had not been made.
 We then officially end the auction by setting ``self.ended`` to ``True``
```

### Comparing `vyper-0.4.0rc2/examples/auctions/blind_auction.vy` & `vyper-0.4.0rc3/examples/auctions/blind_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/auctions/simple_open_auction.vy` & `vyper-0.4.0rc3/examples/auctions/simple_open_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/crowdfund.vy` & `vyper-0.4.0rc3/examples/crowdfund.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/factory/Exchange.vy` & `vyper-0.4.0rc3/examples/factory/Exchange.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/factory/Factory.vy` & `vyper-0.4.0rc3/examples/factory/Factory.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/market_maker/on_chain_market_maker.vy` & `vyper-0.4.0rc3/examples/market_maker/on_chain_market_maker.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/safe_remote_purchase/safe_remote_purchase.vy` & `vyper-0.4.0rc3/examples/safe_remote_purchase/safe_remote_purchase.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/stock/company.vy` & `vyper-0.4.0rc3/examples/stock/company.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/tokens/ERC1155ownable.vy` & `vyper-0.4.0rc3/examples/tokens/ERC1155ownable.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/tokens/ERC20.vy` & `vyper-0.4.0rc3/examples/tokens/ERC20.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/tokens/ERC4626.vy` & `vyper-0.4.0rc3/examples/tokens/ERC4626.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/tokens/ERC721.vy` & `vyper-0.4.0rc3/examples/tokens/ERC721.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/voting/ballot.vy` & `vyper-0.4.0rc3/examples/voting/ballot.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/examples/wallet/wallet.vy` & `vyper-0.4.0rc3/examples/wallet/wallet.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/make.cmd` & `vyper-0.4.0rc3/make.cmd`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/setup.cfg` & `vyper-0.4.0rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/setup.py` & `vyper-0.4.0rc3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 extras_require = {
     "test": [
         "pytest>=8.0,<9.0",
         "pytest-cov>=4.1,<5.0",
         "pytest-instafail>=0.4,<1.0",
         "pytest-xdist>=3.0,<3.4",
         "pytest-split>=0.7.0,<1.0",
-        "eth-tester[py-evm]>=0.10.0b4,<0.11",
-        "eth_abi>=4.0.0,<5.0.0",
-        "py-evm>=0.10.0b4,<0.11",
-        "web3==6.0.0",
+        "eth_abi>=5.0.0,<6.0.0",
+        "py-evm>=0.10.1b1,<0.11",
         "lark==1.1.9",
         "hypothesis[lark]>=6.0,<7.0",
         "eth-stdlib==0.2.7",
+        "eth-account==0.12.2",
         "setuptools",
         "hexbytes>=1.2",
+        "pyrevm>=0.3.2",
     ],
     "lint": [
         "black==23.12.0",
         "flake8==6.1.0",
         "flake8-bugbear==23.12.2",
         "flake8-use-fstring==1.4",
         "isort==5.13.2",
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_abi_decode.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_abi_decode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from eth.codecs import abi
 
+from tests.evm_backends.base_env import EvmError, ExecutionReverted
 from tests.utils import decimal_to_int
-from vyper.exceptions import ArgumentException, StackTooDeep, StructureException
+from vyper.exceptions import ArgumentException, StructureException
 
 TEST_ADDR = "0x" + b"".join(chr(i).encode("utf-8") for i in range(20)).hex()
 
 
 def test_abi_decode_complex(get_contract):
     contract = """
 struct Animal:
@@ -65,18 +66,18 @@
     )
 
     test_bytes32 = b"".join(chr(i).encode("utf-8") for i in range(32))
     human_tuple = (
         "foobar",
         ("vyper", TEST_ADDR, 123, True, decimal_to_int("123.4"), [123, 456, 789], test_bytes32),
     )
-    args = tuple([human_tuple[0]] + list(human_tuple[1]))
+
     human_t = "((string,(string,address,int128,bool,int168,uint256[3],bytes32)))"
     human_encoded = abi.encode(human_t, (human_tuple,))
-    assert tuple(c.abi_decode_struct(human_encoded)) == (
+    assert c.abi_decode_struct(human_encoded) == (
         "foobar",
         ("vyper", TEST_ADDR, 123, True, decimal_to_int("123.4"), [123, 456, 789], test_bytes32),
     )
 
 
 @pytest.mark.parametrize(
     "expected,input_len,output_typ,abi_typ,unwrap_tuple",
@@ -87,17 +88,15 @@
         ("vyper", 96, "String[5]", "(string)", True),
         ([123, 456, 789], 96, "uint256[3]", "uint256[3]", False),
         ([123, 456, 789], 96, "uint256[3]", "(uint256[3])", True),
         ([123, 456, 789], 128, "DynArray[uint256, 3]", "uint256[]", False),
         ([123, 456, 789], 160, "DynArray[uint256, 3]", "(uint256[])", True),
     ],
 )
-def test_abi_decode_single(
-    w3, get_contract, expected, input_len, output_typ, abi_typ, unwrap_tuple
-):
+def test_abi_decode_single(get_contract, expected, input_len, output_typ, abi_typ, unwrap_tuple):
     contract = f"""
 @external
 def foo(x: Bytes[{input_len}]) -> {output_typ}:
     a: {output_typ} = _abi_decode(x, {output_typ}, unwrap_tuple={unwrap_tuple})
     return a
     """
     c = get_contract(contract)
@@ -197,15 +196,14 @@
     [[[123, 456, 789], [234, 567]], [[234]], [[567], [912], [345]]],
     [[[]]],
 ]
 
 
 @pytest.mark.parametrize("args", nested_3d_array_args)
 @pytest.mark.parametrize("unwrap_tuple", (True, False))
-@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_abi_decode_nested_dynarray2(get_contract, args, unwrap_tuple):
     if unwrap_tuple is True:
         encoded = abi.encode("(uint256[][][])", (args,))
         len = 1696
     else:
         encoded = abi.encode("uint256[][][]", args)
         len = 1664
@@ -272,18 +270,17 @@
     dont_clobber_me: uint256 = max_value(uint256)
     self._foo(bs)
     return dont_clobber_me, self.bytez
     """
     c = get_contract(code)
     bs = [1, 2, 3]
     encoded = abi.encode("(uint256[])", (bs,))
-    assert c.foo(encoded) == [2**256 - 1, bs]
+    assert c.foo(encoded) == (2**256 - 1, bs)
 
 
-@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_abi_decode_private_nested_dynarray(get_contract):
     code = """
 bytez: DynArray[DynArray[DynArray[uint256, 3], 3], 3]
 
 @internal
 def _foo(bs: Bytes[1696]):
     self.bytez = _abi_decode(bs, DynArray[DynArray[DynArray[uint256, 3], 3], 3])
@@ -297,15 +294,15 @@
     c = get_contract(code)
     bs = [
         [[1, 2, 3], [4, 5, 6], [7, 8, 9]],
         [[10, 11, 12], [13, 14, 15], [16, 17, 18]],
         [[19, 20, 21], [22, 23, 24], [25, 26, 27]],
     ]
     encoded = abi.encode("(uint256[][][])", (bs,))
-    assert c.foo(encoded) == [2**256 - 1, bs]
+    assert c.foo(encoded) == (2**256 - 1, bs)
 
 
 def test_abi_decode_return(get_contract):
     contract = """
 @external
 def abi_decode(x: Bytes[64]) -> (address, int128):
     return _abi_decode(x, (address, int128))
@@ -421,33 +418,35 @@
     """
     c = get_contract(contract)
     encoded = abi.encode(encoding, (arg,))
     assert c.abi_decode(encoded) == expected
 
 
 @pytest.mark.parametrize(
-    "output_typ1,output_typ2,input_",
+    "output_typ1,output_typ2,input_,error,error_property",
     [
-        ("DynArray[uint256, 3]", "uint256", b""),
-        ("DynArray[uint256, 3]", "uint256", b"\x01" * 128),
-        ("Bytes[5]", "address", b""),
-        ("Bytes[5]", "address", b"\x01" * 128),
+        ("DynArray[uint256, 3]", "uint256", b"", ExecutionReverted, ""),
+        ("DynArray[uint256, 3]", "uint256", b"\x01" * 128, EvmError, "OUT_OF_GAS_ERROR"),
+        ("Bytes[5]", "address", b"", ExecutionReverted, ""),
+        ("Bytes[5]", "address", b"\x01" * 128, EvmError, "OUT_OF_GAS_ERROR"),
     ],
 )
-def test_clamper_dynamic_tuple(get_contract, tx_failed, output_typ1, output_typ2, input_):
+def test_clamper_dynamic_tuple(
+    get_contract, tx_failed, output_typ1, output_typ2, input_, error, error_property, env
+):
     contract = f"""
 @external
 def abi_decode(x: Bytes[224]) -> ({output_typ1}, {output_typ2}):
     a: {output_typ1} = empty({output_typ1})
     b: {output_typ2} = empty({output_typ2})
     a, b = _abi_decode(x, ({output_typ1}, {output_typ2}))
     return a, b
     """
     c = get_contract(contract)
-    with tx_failed():
+    with tx_failed(error, exc_text=getattr(env, error_property, None)):
         c.abi_decode(input_)
 
 
 FAIL_LIST = [
     (
         """
 @external
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_abi_encode.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_abi_encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 from eth.codecs import abi
 
 from tests.utils import decimal_to_int
-from vyper.exceptions import StackTooDeep
 
 
 # @pytest.mark.parametrize("string", ["a", "abc", "abcde", "potato"])
 def test_abi_encode(get_contract):
     code = """
 struct Animal:
   name: String[5]
@@ -223,15 +222,14 @@
     [[[]], [[123]], [[]]],
     [[[123, 456, 789], [234, 567]], [[234]], [[567], [912], [345]]],
     [[[]]],
 ]
 
 
 @pytest.mark.parametrize("args", nested_3d_array_args)
-@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_abi_encode_nested_dynarray_2(get_contract, args):
     code = """
 @external
 def abi_encode(
     d: DynArray[DynArray[DynArray[uint256, 3], 3], 3],
     ensure_tuple: bool,
     include_method_id: bool
@@ -308,15 +306,15 @@
 def foo(bs: Bytes[32]) -> (uint256, Bytes[96]):
     dont_clobber_me: uint256 = max_value(uint256)
     self._foo(bs)
     return dont_clobber_me, self.bytez
     """
     c = get_contract(code)
     bs = b"\x00" * 32
-    assert c.foo(bs) == [2**256 - 1, abi.encode("(bytes)", (bs,))]
+    assert c.foo(bs) == (2**256 - 1, abi.encode("(bytes)", (bs,)))
 
 
 def test_abi_encode_private_dynarray(get_contract):
     code = """
 bytez: Bytes[160]
 @internal
 def _foo(bs: DynArray[uint256, 3]):
@@ -325,18 +323,17 @@
 def foo(bs: DynArray[uint256, 3]) -> (uint256, Bytes[160]):
     dont_clobber_me: uint256 = max_value(uint256)
     self._foo(bs)
     return dont_clobber_me, self.bytez
     """
     c = get_contract(code)
     bs = [1, 2, 3]
-    assert c.foo(bs) == [2**256 - 1, abi.encode("(uint256[])", (bs,))]
+    assert c.foo(bs) == (2**256 - 1, abi.encode("(uint256[])", (bs,)))
 
 
-@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_abi_encode_private_nested_dynarray(get_contract):
     code = """
 bytez: Bytes[1696]
 @internal
 def _foo(bs: DynArray[DynArray[DynArray[uint256, 3], 3], 3]):
     self.bytez = _abi_encode(bs)
 
@@ -348,15 +345,15 @@
     """
     c = get_contract(code)
     bs = [
         [[1, 2, 3], [4, 5, 6], [7, 8, 9]],
         [[10, 11, 12], [13, 14, 15], [16, 17, 18]],
         [[19, 20, 21], [22, 23, 24], [25, 26, 27]],
     ]
-    assert c.foo(bs) == [2**256 - 1, abi.encode("(uint256[][][])", (bs,))]
+    assert c.foo(bs) == (2**256 - 1, abi.encode("(uint256[][][])", (bs,)))
 
 
 @pytest.mark.parametrize("empty_literal", ('b""', '""', "empty(Bytes[1])", "empty(String[1])"))
 def test_abi_encode_empty_string(get_contract, empty_literal):
     code = f"""
 @external
 def foo(ensure_tuple: bool) -> Bytes[96]:
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_addmod.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_addmod.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-def test_uint256_addmod(tx_failed, get_contract_with_gas_estimation):
+def test_uint256_addmod(tx_failed, get_contract):
     uint256_code = """
 @external
 def _uint256_addmod(x: uint256, y: uint256, z: uint256) -> uint256:
     return uint256_addmod(x, y, z)
     """
 
-    c = get_contract_with_gas_estimation(uint256_code)
+    c = get_contract(uint256_code)
 
     assert c._uint256_addmod(1, 2, 2) == 1
     assert c._uint256_addmod(32, 2, 32) == 2
     assert c._uint256_addmod((2**256) - 1, 0, 2) == 1
     assert c._uint256_addmod(2**255, 2**255, 6) == 4
     with tx_failed():
         c._uint256_addmod(1, 2, 0)
 
 
-def test_uint256_addmod_ext_call(
-    w3, side_effects_contract, assert_side_effects_invoked, get_contract
-):
+def test_uint256_addmod_ext_call(side_effects_contract, assert_side_effects_invoked, get_contract):
     code = """
 interface Foo:
     def foo(x: uint256) -> uint256: payable
 
 @external
 def foo(f: Foo) -> uint256:
     return uint256_addmod(32, 2, extcall f.foo(32))
     """
 
     c1 = side_effects_contract("uint256")
     c2 = get_contract(code)
 
     assert c2.foo(c1.address) == 2
-    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address, transact={}))
+    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address))
 
 
-def test_uint256_addmod_internal_call(get_contract_with_gas_estimation):
+def test_uint256_addmod_internal_call(get_contract):
     code = """
 @external
 def foo() -> uint256:
     return uint256_addmod(self.a(), self.b(), self.c())
 
 @internal
 def a() -> uint256:
@@ -49,20 +47,20 @@
     return 2
 
 @internal
 def c() -> uint256:
     return 32
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.foo() == 2
 
 
-def test_uint256_addmod_evaluation_order(get_contract_with_gas_estimation):
+def test_uint256_addmod_evaluation_order(get_contract):
     code = """
 a: uint256
 
 @external
 def foo1() -> uint256:
     self.a = 0
     return uint256_addmod(self.a, 1, self.bar())
@@ -79,12 +77,12 @@
 
 @internal
 def bar() -> uint256:
     self.a = 1
     return 2
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.foo1() == 1
     assert c.foo2() == 2
     assert c.foo3() == 1
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_as_wei_value.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_as_wei_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+from eth_utils import to_wei
 
 from tests.utils import decimal_to_int
 from vyper.semantics.types import DecimalT
 from vyper.utils import quantize, round_towards_zero
 
 wei_denoms = {
     "femtoether": 3,
@@ -96,38 +97,36 @@
     return as_wei_value(a, "{denom}")
     """
 
     c = get_contract(code)
     assert c.foo(0) == 0
 
 
-def test_ext_call(w3, side_effects_contract, assert_side_effects_invoked, get_contract):
+def test_ext_call(side_effects_contract, assert_side_effects_invoked, get_contract):
     code = """
 interface Foo:
     def foo(x: uint8) -> uint8: nonpayable
 
 @external
 def foo(a: Foo) -> uint256:
     return as_wei_value(extcall a.foo(7), "ether")
     """
 
     c1 = side_effects_contract("uint8")
     c2 = get_contract(code)
 
-    assert c2.foo(c1.address) == w3.to_wei(7, "ether")
-    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address, transact={}))
+    assert c2.foo(c1.address) == to_wei(7, "ether")
+    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address))
 
 
-def test_internal_call(w3, get_contract_with_gas_estimation):
+def test_internal_call(get_contract):
     code = """
 @external
 def foo() -> uint256:
     return as_wei_value(self.bar(), "ether")
 
 @internal
 def bar() -> uint8:
     return 7
     """
-
-    c = get_contract_with_gas_estimation(code)
-
-    assert c.foo() == w3.to_wei(7, "ether")
+    c = get_contract(code)
+    assert c.foo() == to_wei(7, "ether")
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_bitwise.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_bitwise.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,40 +33,40 @@
 
 def test_bitwise_opcodes():
     opcodes = compile_code(code, output_formats=["opcodes"])["opcodes"]
     assert "SHL" in opcodes
     assert "SHR" in opcodes
 
 
-def test_test_bitwise(get_contract_with_gas_estimation):
-    c = get_contract_with_gas_estimation(code)
+def test_test_bitwise(get_contract):
+    c = get_contract(code)
     x = 126416208461208640982146408124
     y = 7128468721412412459
     assert c._bitwise_and(x, y) == (x & y)
     assert c._bitwise_or(x, y) == (x | y)
     assert c._bitwise_xor(x, y) == (x ^ y)
     assert c._bitwise_not(x) == 2**256 - 1 - x
 
     for t in (x, y):
         for s in (0, 1, 3, 255, 256):
             assert c._shr(t, s) == t >> s
             assert c._shl(t, s) == (t << s) % (2**256)
 
 
-def test_signed_shift(get_contract_with_gas_estimation):
+def test_signed_shift(get_contract):
     code = """
 @external
 def _sar(x: int256, y: uint256) -> int256:
     return x >> y
 
 @external
 def _shl(x: int256, y: uint256) -> int256:
     return x << y
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     x = 126416208461208640982146408124
     y = 7128468721412412459
     cases = [x, y, -x, -y]
 
     for t in cases:
         for s in (0, 1, 3, 255, 256):
             assert c._sar(t, s) == t >> s
@@ -164,9 +164,9 @@
     """,
         InvalidLiteral,
     ),
 ]
 
 
 @pytest.mark.parametrize("bad_code,exc", fail_list)
-def test_shift_fail(get_contract_with_gas_estimation, bad_code, exc, assert_compile_failed):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(bad_code), exc)
+def test_shift_fail(get_contract, bad_code, exc, assert_compile_failed):
+    assert_compile_failed(lambda: get_contract(bad_code), exc)
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ceil.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ceil.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from decimal import Decimal
 
 from tests.utils import decimal_to_int
 
 
-def test_ceil(get_contract_with_gas_estimation):
+def test_ceil(get_contract):
     code = """
 x: decimal
 
 @deploy
 def __init__():
     self.x = 504.0000000001
 
@@ -36,26 +36,26 @@
 def fou() -> int256:
     a: int128 = 305
     b: int128 = 100
     c: decimal = convert(a, decimal) / convert(b, decimal)
     return ceil(c)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.x_ceil() == 505
     assert c.foo() == 1
     assert c.fop() == 1
     assert c.foq() == math.ceil(Decimal(2**167) / 10**10)
     assert c.fos() == 0
     assert c.fou() == 4
 
 
 # ceil(x) should yield the smallest integer greater than or equal to x
-def test_ceil_negative(get_contract_with_gas_estimation):
+def test_ceil_negative(get_contract):
     code = """
 x: decimal
 
 @deploy
 def __init__():
     self.x = -504.0000000001
 
@@ -91,52 +91,52 @@
     return ceil(c)
 
 @external
 def ceil_param(p: decimal) -> int256:
     return ceil(p)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.x_ceil() == -504
     assert c.foo() == -11
     assert c.fop() == -5
     assert c.foq() == 0
     assert c.fos() == -5472
     assert c.fot() == math.ceil(-(Decimal(2**167 - 1)) / 10**10)
     assert c.fou() == -3
     assert c.ceil_param(decimal_to_int("-0.5")) == 0
     assert c.ceil_param(decimal_to_int("-7777777.7777777")) == -7777777
 
 
-def test_ceil_ext_call(w3, side_effects_contract, assert_side_effects_invoked, get_contract):
+def test_ceil_ext_call(side_effects_contract, assert_side_effects_invoked, get_contract):
     code = """
 interface Foo:
     def foo(x: decimal) -> decimal: payable
 
 @external
 def foo(a: Foo) -> int256:
     return ceil(extcall a.foo(2.5))
     """
 
     c1 = side_effects_contract("decimal")
     c2 = get_contract(code)
 
     assert c2.foo(c1.address) == 3
 
-    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address, transact={}))
+    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address))
 
 
-def test_ceil_internal_call(get_contract_with_gas_estimation):
+def test_ceil_internal_call(get_contract):
     code = """
 @external
 def foo() -> int256:
     return ceil(self.bar())
 
 @internal
 def bar() -> decimal:
     return 2.5
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.foo() == 3
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_concat.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_concat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-def test_concat(get_contract_with_gas_estimation):
+def test_concat(get_contract):
     test_concat = """
 @external
 def foo2(input1: Bytes[50], input2: Bytes[50]) -> Bytes[1000]:
     return concat(input1, input2)
 
 @external
 def foo3(input1: Bytes[50], input2: Bytes[50], input3: Bytes[50]) -> Bytes[1000]:
     return concat(input1, input2, input3)
     """
 
-    c = get_contract_with_gas_estimation(test_concat)
+    c = get_contract(test_concat)
     assert c.foo2(b"h", b"orse") == b"horse"
     assert c.foo2(b"h", b"") == b"h"
     assert c.foo2(b"", b"") == b""
     assert c.foo2(b"", b"orse") == b"orse"
     assert c.foo3(b"Buffalo", b" ", b"buffalo") == b"Buffalo buffalo"
     assert c.foo2(b"\x36", b"\x35" * 32) == b"\x36" + b"\x35" * 32
     assert c.foo2(b"\x36" * 48, b"\x35" * 32) == b"\x36" * 48 + b"\x35" * 32
     assert (
         c.foo3(b"horses" * 4, b"mice" * 7, b"crows" * 10)
         == b"horses" * 4 + b"mice" * 7 + b"crows" * 10
     )  # noqa: E501
     print("Passed simple concat test")
 
 
-def test_concat2(get_contract_with_gas_estimation):
+def test_concat2(get_contract):
     test_concat2 = """
 @external
 def foo(inp: Bytes[50]) -> Bytes[1000]:
     x: Bytes[50] = inp
     return concat(x, inp, x, inp, x, inp, x, inp, x, inp)
     """
 
-    c = get_contract_with_gas_estimation(test_concat2)
+    c = get_contract(test_concat2)
     assert c.foo(b"horse" * 9 + b"vyper") == (b"horse" * 9 + b"vyper") * 10
     print("Passed second concat test")
 
 
-def test_crazy_concat_code(get_contract_with_gas_estimation):
+def test_crazy_concat_code(get_contract):
     crazy_concat_code = """
 y: Bytes[10]
 
 @external
 def krazykonkat(z: Bytes[10]) -> Bytes[25]:
     x: Bytes[3] = b"cow"
     self.y = b"horse"
     return concat(x, b" ", self.y, b" ", z)
     """
 
-    c = get_contract_with_gas_estimation(crazy_concat_code)
+    c = get_contract(crazy_concat_code)
 
     assert c.krazykonkat(b"moose") == b"cow horse moose"
 
     print("Passed third concat test")
 
 
 def test_concat_buffer(get_contract):
@@ -115,39 +115,39 @@
     b: uint256 = self.bar()
     return i
     """
     c = get_contract(code)
     assert c.foo() == -1
 
 
-def test_concat_bytes32(get_contract_with_gas_estimation):
+def test_concat_bytes32(get_contract):
     test_concat_bytes32 = """
 @external
 def sandwich(inp: Bytes[100], inp2: bytes32) -> Bytes[164]:
     return concat(inp2, inp, inp2)
 
 @external
 def fivetimes(inp: bytes32) -> Bytes[160]:
     return concat(inp, inp, inp, inp, inp)
     """
 
-    c = get_contract_with_gas_estimation(test_concat_bytes32)
+    c = get_contract(test_concat_bytes32)
     assert c.sandwich(b"cow", b"\x35" * 32) == b"\x35" * 32 + b"cow" + b"\x35" * 32, c.sandwich(
         b"cow", b"\x35" * 32
     )  # noqa: E501
     assert c.sandwich(b"", b"\x46" * 32) == b"\x46" * 64
     assert c.sandwich(b"\x57" * 95, b"\x57" * 32) == b"\x57" * 159
     assert c.sandwich(b"\x57" * 96, b"\x57" * 32) == b"\x57" * 160
     assert c.sandwich(b"\x57" * 97, b"\x57" * 32) == b"\x57" * 161
     assert c.fivetimes(b"mongoose" * 4) == b"mongoose" * 20
 
     print("Passed concat bytes32 test")
 
 
-def test_konkat_code(get_contract_with_gas_estimation):
+def test_konkat_code(get_contract):
     konkat_code = """
 ecks: bytes32
 
 @external
 def foo(x: bytes32, y: bytes32) -> Bytes[64]:
     self.ecks = x
     return concat(self.ecks, y)
@@ -158,35 +158,35 @@
     return concat(self.ecks, y)
 
 @external
 def hoo(x: bytes32, y: bytes32) -> Bytes[64]:
     return concat(x, y)
     """
 
-    c = get_contract_with_gas_estimation(konkat_code)
+    c = get_contract(konkat_code)
     assert c.foo(b"\x35" * 32, b"\x00" * 32) == b"\x35" * 32 + b"\x00" * 32
     assert c.goo(b"\x35" * 32, b"\x00" * 32) == b"\x35" * 32 + b"\x00" * 32
     assert c.hoo(b"\x35" * 32, b"\x00" * 32) == b"\x35" * 32 + b"\x00" * 32
 
     print("Passed second concat tests")
 
 
-def test_small_output(get_contract_with_gas_estimation):
+def test_small_output(get_contract):
     code = """
 @external
 def small_output(a: String[5], b: String[4]) -> String[9]:
     c: String[9] = concat(a, b)
     return c
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.small_output("abcde", "fghi") == "abcdefghi"
     assert c.small_output("", "") == ""
 
 
-def test_small_bytes(get_contract_with_gas_estimation):
+def test_small_bytes(get_contract):
     # TODO maybe use parametrization or hypothesis for the examples
     code = """
 @external
 def small_bytes1(a: bytes1, b: Bytes[2]) -> Bytes[3]:
     return concat(a, b)
 
 @external
@@ -197,15 +197,15 @@
 def small_bytes3(a: bytes4, b: bytes32) -> Bytes[36]:
     return concat(a, b)
 
 @external
 def small_bytes4(a: bytes8, b: Bytes[32], c: bytes8) -> Bytes[48]:
     return concat(a, b, c)
     """
-    contract = get_contract_with_gas_estimation(code)
+    contract = get_contract(code)
 
     i = 0
 
     def bytes_for_len(n):
         nonlocal i
         # bytes constructor with state
         # (so we don't keep generating the same string)
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_convert.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,14 @@
     unsigned_to_signed,
 )
 
 BASE_TYPES = set(IntegerT.all()) | set(BytesM_T.all()) | {DecimalT(), AddressT(), BoolT()}
 
 TEST_TYPES = BASE_TYPES | {BytesT(32)} | {StringT(32)}
 
-ZERO_ADDRESS = "0x0000000000000000000000000000000000000000"
-
 # decimal increment, aka smallest decimal > 0
 DECIMAL_EPSILON = Decimal(1) / DECIMAL_DIVISOR
 
 
 def _bits_of_type(typ):
     if isinstance(typ, (IntegerT, DecimalT)):
         return typ.bits
@@ -425,134 +423,124 @@
         val = quantize(val)
         assert tmp == val
     return str(val)
 
 
 @pytest.mark.parametrize("i_typ,o_typ,val", generate_passing_cases())
 @pytest.mark.fuzzing
-def test_convert_passing(
-    get_contract_with_gas_estimation, assert_compile_failed, i_typ, o_typ, val
-):
+def test_convert_passing(get_contract, assert_compile_failed, i_typ, o_typ, val):
     expected_val = _py_convert(val, i_typ, o_typ)
-    if isinstance(o_typ, AddressT) and expected_val == "0x" + "00" * 20:
-        # web3 has special formatter for zero address
-        expected_val = None
 
     if isinstance(o_typ, DecimalT):
         expected_val = decimal_to_int(expected_val)
 
     input_val = val
     if isinstance(i_typ, DecimalT):
         input_val = decimal_to_int(val)
 
     contract_1 = f"""
 @external
 def test_convert() -> {o_typ}:
     return convert({_vyper_literal(val, i_typ)}, {o_typ})
     """
 
-    c1_exception = None
     skip_c1 = False
 
     # Skip bytes20 literals when there is ambiguity with `address` since address takes precedence.
     # generally happens when there are only digits in the literal.
     if i_typ == BYTES20_T and is_checksum_encoded(_vyper_literal(val, BYTES20_T)):
         skip_c1 = True
 
     # typechecker inference borked, ambiguity with bytes20
     if isinstance(i_typ, AddressT) and o_typ == BYTES20_T and val == val.lower():
         skip_c1 = True
 
-    if c1_exception is not None:
-        assert_compile_failed(lambda: get_contract_with_gas_estimation(contract_1), c1_exception)
-    elif not skip_c1:
-        c1 = get_contract_with_gas_estimation(contract_1)
+    if not skip_c1:
+        c1 = get_contract(contract_1)
         assert c1.test_convert() == expected_val
 
     contract_2 = f"""
 @external
 def test_input_convert(x: {i_typ}) -> {o_typ}:
     return convert(x, {o_typ})
     """
 
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c2 = get_contract(contract_2)
     assert c2.test_input_convert(input_val) == expected_val
 
     contract_3 = f"""
 bar: {i_typ}
 
 @external
 def test_state_variable_convert() -> {o_typ}:
     self.bar = {_vyper_literal(val, i_typ)}
     return convert(self.bar, {o_typ})
     """
 
-    c3 = get_contract_with_gas_estimation(contract_3)
+    c3 = get_contract(contract_3)
     assert c3.test_state_variable_convert() == expected_val
 
     contract_4 = f"""
 @external
 def test_memory_variable_convert(x: {i_typ}) -> {o_typ}:
     y: {i_typ} = x
     return convert(y, {o_typ})
     """
 
-    c4 = get_contract_with_gas_estimation(contract_4)
+    c4 = get_contract(contract_4)
     assert c4.test_memory_variable_convert(input_val) == expected_val
 
 
 @pytest.mark.parametrize("typ", ["uint8", "int128", "int256", "uint256"])
 @pytest.mark.parametrize("val", [1, 2, 2**128, 2**256 - 1, 2**256 - 2])
-def test_flag_conversion(get_contract_with_gas_estimation, assert_compile_failed, val, typ):
+def test_flag_conversion(get_contract, assert_compile_failed, val, typ):
     roles = "\n    ".join([f"ROLE_{i}" for i in range(256)])
     contract = f"""
 flag Roles:
     {roles}
 
 @external
 def foo(a: Roles) -> {typ}:
     return convert(a, {typ})
 
 @external
 def bar(a: uint256) -> Roles:
     return convert(a, Roles)
     """
     if typ == "uint256":
-        c = get_contract_with_gas_estimation(contract)
+        c = get_contract(contract)
         assert c.foo(val) == val
         assert c.bar(val) == val
     else:
-        assert_compile_failed(lambda: get_contract_with_gas_estimation(contract), TypeMismatch)
+        assert_compile_failed(lambda: get_contract(contract), TypeMismatch)
 
 
 @pytest.mark.parametrize("typ", ["uint8", "int128", "int256", "uint256"])
 @pytest.mark.parametrize("val", [1, 2, 3, 4, 2**128, 2**256 - 1, 2**256 - 2])
-def test_flag_conversion_2(
-    get_contract_with_gas_estimation, assert_compile_failed, tx_failed, val, typ
-):
+def test_flag_conversion_2(get_contract, assert_compile_failed, tx_failed, val, typ):
     contract = f"""
 flag Status:
     STARTED
     PAUSED
     STOPPED
 
 @external
 def foo(a: {typ}) -> Status:
     return convert(a, Status)
     """
     if typ == "uint256":
-        c = get_contract_with_gas_estimation(contract)
+        c = get_contract(contract)
         lo, hi = int_bounds(signed=False, bits=3)
         if lo <= val <= hi:
             assert c.foo(val) == val
         else:
             with tx_failed():
                 c.foo(val)
     else:
-        assert_compile_failed(lambda: get_contract_with_gas_estimation(contract), TypeMismatch)
+        assert_compile_failed(lambda: get_contract(contract), TypeMismatch)
 
 
 # uint256 conversion is currently valid due to type inference on literals
 # not quite working yet
 same_type_conversion_blocked = sorted(TEST_TYPES - {UINT256_T})
 
 
@@ -644,15 +632,15 @@
 
     failing_code = code_2_template.format(typ=typ2, arg=bytestring(cls1, "1" * 33))
     with pytest.raises(TypeMismatch):
         compile_code(failing_code)
 
 
 @pytest.mark.parametrize("n", range(1, 33))
-def test_Bytes_to_bytes(get_contract, n):
+def test_Bytes_to_bytes(get_contract, n: int):
     t_bytes = f"bytes{n}"
     t_Bytes = f"Bytes[{n}]"
 
     test_data = b"\xff" * n
 
     code1 = f"""
 @external
@@ -672,17 +660,15 @@
     """
     c2 = get_contract(code2)
     assert c2.foo() == test_data
 
 
 @pytest.mark.parametrize("i_typ,o_typ,val", generate_reverting_cases())
 @pytest.mark.fuzzing
-def test_conversion_failures(
-    get_contract_with_gas_estimation, assert_compile_failed, tx_failed, i_typ, o_typ, val
-):
+def test_conversion_failures(get_contract, assert_compile_failed, tx_failed, i_typ, o_typ, val):
     """
     Test multiple contracts and check for a specific exception.
     If no exception is provided, a runtime revert is expected (e.g. clamping).
     """
     contract_1 = f"""
 @external
 def foo() -> {o_typ}:
@@ -705,32 +691,32 @@
     if isinstance(o_typ, BytesM_T):
         skip_c1 = True
 
     # if o_typ in (AddressT(), BYTES20_T):
     #    skip_c1 = True
 
     if not skip_c1:
-        assert_compile_failed(lambda: get_contract_with_gas_estimation(contract_1), c1_exception)
+        assert_compile_failed(lambda: get_contract(contract_1), c1_exception)
 
     contract_2 = f"""
 @external
 def foo():
     bar: {i_typ} = {_vyper_literal(val, i_typ)}
     foobar: {o_typ} = convert(bar, {o_typ})
     """
 
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c2 = get_contract(contract_2)
     with tx_failed():
         c2.foo()
 
     contract_3 = f"""
 @external
 def foo(bar: {i_typ}) -> {o_typ}:
     return convert(bar, {o_typ})
     """
 
-    c3 = get_contract_with_gas_estimation(contract_3)
+    c3 = get_contract(contract_3)
     input_val = val
     if isinstance(i_typ, DecimalT):
         input_val = decimal_to_int(input_val)
     with tx_failed():
         c3.foo(input_val)
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_create_functions.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_create_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 import rlp
 from eth.codecs import abi
 from hexbytes import HexBytes
 
 import vyper.ir.compile_ir as compile_ir
+from tests.utils import ZERO_ADDRESS
 from vyper.codegen.ir_node import IRnode
 from vyper.compiler.settings import OptimizationLevel
 from vyper.utils import EIP_170_LIMIT, ERC5202_PREFIX, checksum_encode, keccak256
 
 
 # initcode used by create_minimal_proxy_to
 def eip1167_initcode(_addr):
@@ -38,15 +39,15 @@
     address_bits = int(c.address, 16)
     nonce = 1
     rlp_encoded = rlp.encode([address_bits, nonce])
     expected_create_address = keccak256(rlp_encoded)[12:].rjust(20, b"\x00")
     assert c.test() == checksum_encode("0x" + expected_create_address.hex())
 
 
-def test_create_minimal_proxy_to_call(get_contract, w3):
+def test_create_minimal_proxy_to_call(get_contract):
     code = """
 interface SubContract:
     def hello() -> Bytes[100]: view
 
 other: public(address)
 
 @external
@@ -62,19 +63,19 @@
 def test2() -> Bytes[100]:
     return staticcall SubContract(self.other).hello()
     """
 
     c = get_contract(code)
 
     assert c.hello() == b"hello world!"
-    c.test(transact={})
+    c.test()
     assert c.test2() == b"hello world!"
 
 
-def test_minimal_proxy_exception(w3, get_contract, tx_failed):
+def test_minimal_proxy_exception(env, get_contract, tx_failed):
     code = """
 interface SubContract:
     def hello(a: uint256) -> Bytes[100]: view
 
 other: public(address)
 
 @external
@@ -91,27 +92,26 @@
 def test2(a: uint256) -> Bytes[100]:
     return staticcall SubContract(self.other).hello(a)
     """
 
     c = get_contract(code)
 
     assert c.hello(1) == b"hello world!"
-    c.test(transact={})
+    c.test()
     assert c.test2(1) == b"hello world!"
 
-    with tx_failed():
+    with tx_failed(exc_text="invaliddddd"):
         c.test2(0)
 
-    GAS_SENT = 30000
-    tx_hash = c.test2(0, transact={"gas": GAS_SENT})
-
-    receipt = w3.eth.get_transaction_receipt(tx_hash)
+    gas_sent = 30000
+    with tx_failed(exc_text="invaliddddd"):
+        c.test2(0, gas=gas_sent)
 
-    assert receipt["status"] == 0
-    assert receipt["gasUsed"] < GAS_SENT
+    # check we issued `revert`, which does not consume all gas
+    assert env.last_result.gas_used < gas_sent
 
 
 @pytest.mark.parametrize("revert_on_failure", [True, False, None])
 def test_create_minimal_proxy_to_create2(
     get_contract, create2_address_of, keccak, tx_failed, revert_on_failure
 ):
     revert_arg = "" if revert_on_failure is None else f", revert_on_failure={revert_on_failure}"
@@ -123,35 +123,33 @@
     self.main = create_minimal_proxy_to(self, salt=_salt{revert_arg})
     return self.main
     """
 
     c = get_contract(code)
 
     salt = keccak(b"vyper")
-    assert HexBytes(c.test(salt)) == create2_address_of(
-        c.address, salt, eip1167_initcode(c.address)
-    )
+    result = c.test(salt)
+    assert HexBytes(result) == create2_address_of(c.address, salt, eip1167_initcode(c.address))
 
-    c.test(salt, transact={})
     # revert on collision
     if revert_on_failure is False:
-        assert not c.test(salt)
+        assert c.test(salt) == ZERO_ADDRESS
     else:
         with tx_failed():
-            c.test(salt, transact={})
+            c.test(salt)
 
 
 # test blueprints with various prefixes - 0xfe would block calls to the blueprint
 # contract, and 0xfe7100 is ERC5202 magic
 @pytest.mark.parametrize("blueprint_prefix", [b"", b"\xfe", ERC5202_PREFIX])
 @pytest.mark.parametrize("revert_on_failure", [True, False, None])
 def test_create_from_blueprint(
     get_contract,
     deploy_blueprint_for,
-    w3,
+    env,
     keccak,
     create2_address_of,
     tx_failed,
     blueprint_prefix,
     revert_on_failure,
 ):
     revert_arg = "" if revert_on_failure is None else f", revert_on_failure={revert_on_failure}"
@@ -174,56 +172,56 @@
     self.created_address = create_from_blueprint(
         target, code_offset={prefix_len}, salt=salt{revert_arg}
     )
     """
 
     # deploy a foo, so we can compare its bytecode with factory deployed version
     foo_contract = get_contract(code)
-    expected_runtime_code = w3.eth.get_code(foo_contract.address)
+    expected_runtime_code = env.get_code(foo_contract.address)
 
     f, FooContract = deploy_blueprint_for(code, initcode_prefix=blueprint_prefix)
 
     d = get_contract(deployer_code)
 
-    d.test(f.address, transact={})
+    d.test(f.address)
 
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == 123
 
     # extcodesize check
     zero_address = "0x" + "00" * 20
     with tx_failed():
         d.test(zero_address)
 
     # now same thing but with create2
     salt = keccak(b"vyper")
-    d.test2(f.address, salt, transact={})
+    d.test2(f.address, salt)
 
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == 123
 
     # check if the create2 address matches our offchain calculation
-    initcode = w3.eth.get_code(f.address)
+    initcode = env.get_code(f.address)
     initcode = initcode[len(blueprint_prefix) :]  # strip the prefix
     assert HexBytes(test.address) == create2_address_of(d.address, salt, initcode)
 
     # can't collide addresses
     if revert_on_failure is False:
         assert not d.test2(f.address, salt)
     else:
         with tx_failed():
             d.test2(f.address, salt)
 
 
 # test blueprints with 0xfe7100 prefix, which is the EIP 5202 standard.
 # code offset by default should be 3 here.
 def test_create_from_blueprint_default_offset(
-    get_contract, deploy_blueprint_for, w3, keccak, create2_address_of, tx_failed
+    get_contract, deploy_blueprint_for, env, keccak, create2_address_of, tx_failed
 ):
     code = """
 @external
 def foo() -> uint256:
     return 123
     """
 
@@ -237,51 +235,51 @@
 @external
 def test2(target: address, salt: bytes32):
     self.created_address = create_from_blueprint(target, salt=salt)
     """
 
     # deploy a foo so we can compare its bytecode with factory deployed version
     foo_contract = get_contract(code)
-    expected_runtime_code = w3.eth.get_code(foo_contract.address)
+    expected_runtime_code = env.get_code(foo_contract.address)
 
     f, FooContract = deploy_blueprint_for(code)
 
     d = get_contract(deployer_code)
 
-    d.test(f.address, transact={})
+    d.test(f.address)
 
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == 123
 
     # extcodesize check
     zero_address = "0x" + "00" * 20
     with tx_failed():
         d.test(zero_address)
 
     # now same thing but with create2
     salt = keccak(b"vyper")
-    d.test2(f.address, salt, transact={})
+    d.test2(f.address, salt)
 
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == 123
 
     # check if the create2 address matches our offchain calculation
-    initcode = w3.eth.get_code(f.address)
+    initcode = env.get_code(f.address)
     initcode = initcode[len(ERC5202_PREFIX) :]  # strip the prefix
     assert HexBytes(test.address) == create2_address_of(d.address, salt, initcode)
 
     # can't collide addresses
     with tx_failed():
         d.test2(f.address, salt)
 
 
 def test_create_from_blueprint_bad_code_offset(
-    get_contract, get_contract_from_ir, deploy_blueprint_for, w3, tx_failed
+    get_contract, get_contract_from_ir, deploy_blueprint_for, env, tx_failed
 ):
     deployer_code = """
 BLUEPRINT: immutable(address)
 
 @deploy
 def __init__(blueprint_address: address):
     BLUEPRINT = blueprint_address
@@ -297,19 +295,16 @@
     # zeroes (so no matter which offset, create_from_blueprint will
     # return empty code)
     ir = IRnode.from_list(["deploy", 0, ["seq"] + ["stop"] * initcode_len, 0])
     bytecode, _ = compile_ir.assembly_to_evm(
         compile_ir.compile_to_assembly(ir, optimize=OptimizationLevel.NONE)
     )
     # manually deploy the bytecode
-    c = w3.eth.contract(abi=[], bytecode=bytecode)
-    deploy_transaction = c.constructor()
-    tx_info = {"from": w3.eth.accounts[0], "value": 0, "gasPrice": 0}
-    tx_hash = deploy_transaction.transact(tx_info)
-    blueprint_address = w3.eth.get_transaction_receipt(tx_hash)["contractAddress"]
+    c = env.deploy(abi=[], bytecode=bytecode)
+    blueprint_address = c.address
 
     d = get_contract(deployer_code, blueprint_address)
 
     # deploy with code_ofst=0 fine
     d.test(0)
 
     # deploy with code_ofst=len(blueprint) - 1 fine
@@ -322,15 +317,15 @@
     # code_offset=EIP_170_LIMIT definitely not fine!
     with tx_failed():
         d.test(EIP_170_LIMIT)
 
 
 # test create_from_blueprint with args
 def test_create_from_blueprint_args(
-    get_contract, deploy_blueprint_for, w3, keccak, create2_address_of, tx_failed
+    get_contract, deploy_blueprint_for, env, keccak, create2_address_of, tx_failed
 ):
     code = """
 struct Bar:
     x: String[32]
 
 FOO: immutable(String[128])
 BAR: immutable(Bar)
@@ -376,82 +371,84 @@
     self.created_address = create_from_blueprint(target, arg1, arg2)
     """
     FOO = "hello!"
     BAR = ("world!",)
 
     # deploy a foo so we can compare its bytecode with factory deployed version
     foo_contract = get_contract(code, FOO, BAR)
-    expected_runtime_code = w3.eth.get_code(foo_contract.address)
+    expected_runtime_code = env.get_code(foo_contract.address)
 
     f, FooContract = deploy_blueprint_for(code)
 
     d = get_contract(deployer_code)
 
-    initcode = w3.eth.get_code(f.address)[3:]
+    initcode = env.get_code(f.address)[3:]
 
-    d.test(f.address, FOO, BAR, transact={})
+    d.test(f.address, FOO, BAR)
 
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == FOO
     assert test.bar() == BAR
 
     # extcodesize check
     with tx_failed():
         d.test("0x" + "00" * 20, FOO, BAR)
 
     # now same thing but with create2
     salt = keccak(b"vyper")
-    d.test2(f.address, FOO, BAR, salt, transact={})
+    d.test2(f.address, FOO, BAR, salt)
 
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == FOO
     assert test.bar() == BAR
 
     encoded_args = abi.encode("(string,(string))", (FOO, BAR))
     assert HexBytes(test.address) == create2_address_of(d.address, salt, initcode + encoded_args)
 
-    d.test3(f.address, encoded_args, transact={})
+    d.test3(f.address, encoded_args)
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == FOO
     assert test.bar() == BAR
 
-    d.test4(f.address, encoded_args, keccak(b"test4"), transact={})
+    d.test4(f.address, encoded_args, keccak(b"test4"))
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == FOO
     assert test.bar() == BAR
 
     # can't collide addresses
     with tx_failed():
         d.test2(f.address, FOO, BAR, salt)
     # ditto - with raw_args
     with tx_failed():
         d.test4(f.address, encoded_args, salt)
 
     # but creating a contract with different args is ok
     FOO = "bar"
-    d.test2(f.address, FOO, BAR, salt, transact={})
+    d.test2(f.address, FOO, BAR, salt)
     # just for kicks
     assert FooContract(d.created_address()).foo() == FOO
     assert FooContract(d.created_address()).bar() == BAR
 
     # Foo constructor should fail
     FOO = "01" * 129
     BAR = ("",)
     sig = keccak("should_fail(address,string,(string))".encode()).hex()[:10]
     encoded = abi.encode("(address,string,(string))", (f.address, FOO, BAR)).hex()
     with tx_failed():
-        w3.eth.send_transaction({"to": d.address, "data": f"{sig}{encoded}"})
+        env.message_call(d.address, env.deployer, f"{sig}{encoded}")
 
 
 @pytest.mark.parametrize("revert_on_failure", [True, False, None])
-def test_create_copy_of(get_contract, w3, keccak, create2_address_of, tx_failed, revert_on_failure):
+def test_create_copy_of(
+    get_contract, env, keccak, create2_address_of, tx_failed, revert_on_failure
+):
     revert_arg = "" if revert_on_failure is None else f", revert_on_failure={revert_on_failure}"
     code = f"""
 created_address: public(address)
 @internal
 def _create_copy_of(target: address):
     self.created_address = create_copy_of(target{revert_arg})
 
@@ -471,49 +468,46 @@
     x: uint256 = 0
     self._create_copy_of2(target, salt)
     assert x == 0  # check memory not clobbered
     return self.created_address
     """
 
     c = get_contract(code)
-    bytecode = w3.eth.get_code(c.address)
+    bytecode = env.get_code(c.address)
 
-    c.test(c.address, transact={})
+    c.test(c.address)
     test1 = c.created_address()
-    assert w3.eth.get_code(test1) == bytecode
+    assert env.get_code(test1) == bytecode
 
     # extcodesize check
     with tx_failed():
         c.test("0x" + "00" * 20)
 
-    # test1 = c.test(b"\x01")
-    # assert w3.eth.get_code(test1) == b"\x01"
-
     salt = keccak(b"vyper")
-    c.test2(c.address, salt, transact={})
+    c.test2(c.address, salt)
     test2 = c.created_address()
-    assert w3.eth.get_code(test2) == bytecode
+    assert env.get_code(test2) == bytecode
 
     assert HexBytes(test2) == create2_address_of(c.address, salt, vyper_initcode(bytecode))
 
     # can't create2 where contract already exists
     if revert_on_failure is False:
-        assert not c.test2(c.address, salt)
+        assert c.test2(c.address, salt) == ZERO_ADDRESS
     else:
         with tx_failed():
             c.test2(c.address, salt)
 
 
 # XXX: these various tests to check the msize allocator for
 # create_copy_of and create_from_blueprint depend on calling convention
 # and variables writing to memory. think of ways to make more robust to
 # changes in calling convention and memory layout
 @pytest.mark.parametrize("blueprint_prefix", [b"", b"\xfe", b"\xfe\71\x00"])
 def test_create_from_blueprint_complex_value(
-    get_contract, deploy_blueprint_for, w3, blueprint_prefix
+    get_contract, deploy_blueprint_for, env, blueprint_prefix
 ):
     # check msize allocator does not get trampled by value= kwarg
     code = """
 var: uint256
 
 @deploy
 @payable
@@ -547,30 +541,31 @@
         code_offset={prefix_len},
         value=self.foo(),
         raw_args=True
     )
     """
 
     foo_contract = get_contract(code, 12)
-    expected_runtime_code = w3.eth.get_code(foo_contract.address)
+    expected_runtime_code = env.get_code(foo_contract.address)
 
     f, FooContract = deploy_blueprint_for(code, initcode_prefix=blueprint_prefix)
 
     d = get_contract(deployer_code)
 
-    d.test(f.address, transact={"value": 3})
+    env.set_balance(env.deployer, 3)
+    d.test(f.address, value=3)
 
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == 12
 
 
 @pytest.mark.parametrize("blueprint_prefix", [b"", b"\xfe", b"\xfe\71\x00"])
 def test_create_from_blueprint_complex_salt_raw_args(
-    get_contract, deploy_blueprint_for, w3, blueprint_prefix
+    get_contract, deploy_blueprint_for, env, blueprint_prefix
 ):
     # test msize allocator does not get trampled by salt= kwarg
     code = """
 var: uint256
 
 @deploy
 @payable
@@ -605,30 +600,30 @@
         code_offset={prefix_len},
         salt=self.foo(),
         raw_args= True
     )
     """
 
     foo_contract = get_contract(code, 12)
-    expected_runtime_code = w3.eth.get_code(foo_contract.address)
+    expected_runtime_code = env.get_code(foo_contract.address)
 
     f, FooContract = deploy_blueprint_for(code, initcode_prefix=blueprint_prefix)
 
     d = get_contract(deployer_code)
 
-    d.test(f.address, transact={})
+    d.test(f.address)
 
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == 12
 
 
 @pytest.mark.parametrize("blueprint_prefix", [b"", b"\xfe", b"\xfe\71\x00"])
 def test_create_from_blueprint_complex_salt_no_constructor_args(
-    get_contract, deploy_blueprint_for, w3, blueprint_prefix
+    get_contract, deploy_blueprint_for, env, blueprint_prefix
 ):
     # test msize allocator does not get trampled by salt= kwarg
     code = """
 var: uint256
 
 @deploy
 @payable
@@ -653,28 +648,28 @@
         target,
         code_offset={prefix_len},
         salt=keccak256(_abi_encode(target))
     )
     """
 
     foo_contract = get_contract(code)
-    expected_runtime_code = w3.eth.get_code(foo_contract.address)
+    expected_runtime_code = env.get_code(foo_contract.address)
 
     f, FooContract = deploy_blueprint_for(code, initcode_prefix=blueprint_prefix)
 
     d = get_contract(deployer_code)
 
-    d.test(f.address, transact={})
+    d.test(f.address)
 
     test = FooContract(d.created_address())
-    assert w3.eth.get_code(test.address) == expected_runtime_code
+    assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == 12
 
 
-def test_create_copy_of_complex_kwargs(get_contract, w3):
+def test_create_copy_of_complex_kwargs(get_contract, env):
     # test msize allocator does not get trampled by salt= kwarg
     complex_salt = """
 created_address: public(address)
 
 @external
 def test(target: address) -> address:
     self.created_address = create_copy_of(
@@ -682,18 +677,19 @@
         salt=keccak256(_abi_encode(target))
     )
     return self.created_address
 
     """
 
     c = get_contract(complex_salt)
-    bytecode = w3.eth.get_code(c.address)
-    c.test(c.address, transact={})
-    test1 = c.created_address()
-    assert w3.eth.get_code(test1) == bytecode
+    bytecode = env.get_code(c.address)
+    assert bytecode  # Sanity check
+    c.test(c.address)
+    test1 = c.address
+    assert env.get_code(test1) == bytecode
 
     # test msize allocator does not get trampled by value= kwarg
     complex_value = """
 created_address: public(address)
 
 @external
 @payable
@@ -701,12 +697,13 @@
     value: uint256 = 2
     self.created_address = create_copy_of(target, value = [2,2,2][value])
     return self.created_address
 
     """
 
     c = get_contract(complex_value)
-    bytecode = w3.eth.get_code(c.address)
+    bytecode = env.get_code(c.address)
+    env.set_balance(env.deployer, 2)
 
-    c.test(c.address, transact={"value": 2})
-    test1 = c.created_address()
-    assert w3.eth.get_code(test1) == bytecode
+    c.test(c.address, value=2)
+    test1 = c.address
+    assert env.get_code(test1) == bytecode
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ec.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ec.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 
 negative_G1 = [1, 21888242871839275222246405745257275088696311157297823662689037894645226208581]
 
 curve_order = 21888242871839275222246405745257275088548364400416034343698204186575808495617
 
 
-def test_ecadd(get_contract_with_gas_estimation):
+def test_ecadd(get_contract):
     ecadder = """
 x3: uint256[2]
 y3: uint256[2]
 
 @external
 def _ecadd(x: uint256[2], y: uint256[2]) -> uint256[2]:
     return ecadd(x, y)
@@ -33,54 +33,54 @@
 @external
 def _ecadd3(x: uint256[2], y: uint256[2]) -> uint256[2]:
     self.x3 = x
     self.y3 = [y[0], y[1]]
     return ecadd(self.x3, self.y3)
 
     """
-    c = get_contract_with_gas_estimation(ecadder)
+    c = get_contract(ecadder)
 
     assert c._ecadd(G1, G1) == G1_times_two
     assert c._ecadd2(G1, G1_times_two) == G1_times_three
     assert c._ecadd3(G1, [0, 0]) == G1
     assert c._ecadd3(G1, negative_G1) == [0, 0]
 
 
-def test_ecadd_internal_call(get_contract_with_gas_estimation):
+def test_ecadd_internal_call(get_contract):
     code = """
 @internal
 def a() -> uint256[2]:
     return [1, 2]
 
 @external
 def foo() -> uint256[2]:
     return ecadd([1, 2], self.a())
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == G1_times_two
 
 
-def test_ecadd_ext_call(w3, side_effects_contract, assert_side_effects_invoked, get_contract):
+def test_ecadd_ext_call(side_effects_contract, assert_side_effects_invoked, get_contract):
     code = """
 interface Foo:
     def foo(x: uint256[2]) -> uint256[2]: payable
 
 @external
 def foo(a: Foo) -> uint256[2]:
     return ecadd([1, 2], extcall a.foo([1, 2]))
     """
     c1 = side_effects_contract("uint256[2]")
     c2 = get_contract(code)
 
     assert c2.foo(c1.address) == G1_times_two
 
-    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address, transact={}))
+    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address))
 
 
-def test_ecadd_evaluation_order(get_contract_with_gas_estimation):
+def test_ecadd_evaluation_order(get_contract):
     code = """
 x: uint256[2]
 
 @internal
 def bar() -> uint256[2]:
     self.x = ecadd([1, 2], [1, 2])
     return [1, 2]
@@ -88,19 +88,19 @@
 @external
 def foo() -> bool:
     self.x = [1, 2]
     a: uint256[2] = ecadd([1, 2], [1, 2])
     b: uint256[2] = ecadd(self.x, self.bar())
     return a[0] == b[0] and a[1] == b[1]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() is True
 
 
-def test_ecmul(get_contract_with_gas_estimation):
+def test_ecmul(get_contract):
     ecmuller = """
 x3: uint256[2]
 y3: uint256
 
 @external
 def _ecmul(x: uint256[2], y: uint256) -> uint256[2]:
     return ecmul(x, y)
@@ -114,55 +114,55 @@
 @external
 def _ecmul3(x: uint256[2], y: uint256) -> uint256[2]:
     self.x3 = x
     self.y3 = y
     return ecmul(self.x3, self.y3)
 
 """
-    c = get_contract_with_gas_estimation(ecmuller)
+    c = get_contract(ecmuller)
 
     assert c._ecmul(G1, 0) == [0, 0]
     assert c._ecmul(G1, 1) == G1
     assert c._ecmul(G1, 3) == G1_times_three
     assert c._ecmul(G1, curve_order - 1) == negative_G1
     assert c._ecmul(G1, curve_order) == [0, 0]
 
 
-def test_ecmul_internal_call(get_contract_with_gas_estimation):
+def test_ecmul_internal_call(get_contract):
     code = """
 @internal
 def a() -> uint256:
     return 3
 
 @external
 def foo() -> uint256[2]:
     return ecmul([1, 2], self.a())
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == G1_times_three
 
 
-def test_ecmul_ext_call(w3, side_effects_contract, assert_side_effects_invoked, get_contract):
+def test_ecmul_ext_call(side_effects_contract, assert_side_effects_invoked, get_contract):
     code = """
 interface Foo:
     def foo(x: uint256) -> uint256: payable
 
 @external
 def foo(a: Foo) -> uint256[2]:
     return ecmul([1, 2], extcall a.foo(3))
     """
     c1 = side_effects_contract("uint256")
     c2 = get_contract(code)
 
     assert c2.foo(c1.address) == G1_times_three
 
-    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address, transact={}))
+    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address))
 
 
-def test_ecmul_evaluation_order(get_contract_with_gas_estimation):
+def test_ecmul_evaluation_order(get_contract):
     code = """
 x: uint256[2]
 
 @internal
 def bar() -> uint256:
     self.x = ecmul([1, 2], 3)
     return 3
@@ -170,9 +170,9 @@
 @external
 def foo() -> bool:
     self.x = [1, 2]
     a: uint256[2] = ecmul([1, 2], 3)
     b: uint256[2] = ecmul(self.x, self.bar())
     return a[0] == b[0] and a[1] == b[1]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() is True
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_ecrecover.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_ecrecover.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from eth_account import Account
 from eth_account._utils.signing import to_bytes32
 
+from tests.utils import ZERO_ADDRESS
 
-def test_ecrecover_test(get_contract_with_gas_estimation):
+
+def test_ecrecover_test(get_contract):
     ecrecover_test = """
 @external
 def test_ecrecover(h: bytes32, v: uint8, r: bytes32, s: bytes32) -> address:
     return ecrecover(h, v, r, s)
 
 @external
 def test_ecrecover_uints(h: bytes32, v: uint256, r: uint256, s: uint256) -> address:
@@ -24,15 +26,15 @@
     return ecrecover(0x3535353535353535353535353535353535353535353535353535353535353535,
                      28,
                      63198938615202175987747926399054383453528475999185923188997970550032613358815,
                      6577251522710269046055727877571505144084475024240851440410274049870970796685)
 
     """
 
-    c = get_contract_with_gas_estimation(ecrecover_test)
+    c = get_contract(ecrecover_test)
 
     h = b"\x35" * 32
     local_account = Account.from_key(b"\x46" * 32)
     sig = local_account.signHash(h)
 
     assert c.test_ecrecover(h, sig.v, to_bytes32(sig.r), to_bytes32(sig.s)) == local_account.address
     assert c.test_ecrecover_uints(h, sig.v, sig.r, sig.s) == local_account.address
@@ -52,16 +54,15 @@
     s: uint256 = self.dummies[msg.sender][msg.sender]
     return ecrecover(hash, v, r, s)
     """
     c = get_contract(code)
     hash_ = bytes(i for i in range(32))
     v = 0  # invalid v! ecrecover precompile will not write to output buffer
     r = 0
-    # note web3.py decoding of 0x000..00 address is None.
-    assert c.test_ecrecover(hash_, v, r) is None
+    assert c.test_ecrecover(hash_, v, r) == ZERO_ADDRESS
 
 
 # slightly more subtle example: get_v() stomps memory location 0,
 # so this tests that the output buffer stays clean during ecrecover()
 # builtin execution.
 def test_invalid_signature2(get_contract):
     code = """
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_empty.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_empty.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,16 +93,16 @@
         """
 @external
 def foo() -> bool:
     return empty(bool)
     """,
     ],
 )
-def test_empty_basic_type(contract, get_contract_with_gas_estimation):
-    c = get_contract_with_gas_estimation(contract)
+def test_empty_basic_type(contract, get_contract):
+    c = get_contract(contract)
     c.foo()
 
 
 @pytest.mark.parametrize(
     "contract",
     [
         """
@@ -219,16 +219,16 @@
     assert self.foobar[2] == empty(address)
     assert bar[0] == empty(address)
     assert bar[1] == empty(address)
     assert bar[2] == empty(address)
     """,
     ],
 )
-def test_empty_basic_type_lists(contract, get_contract_with_gas_estimation):
-    c = get_contract_with_gas_estimation(contract)
+def test_empty_basic_type_lists(contract, get_contract):
+    c = get_contract(contract)
     c.foo()
 
 
 @pytest.mark.parametrize(
     "contract",
     [
         """
@@ -255,34 +255,34 @@
 @external
 def foo():
     x: uint256 = 1
     empty(x)
     """,
     ],
 )
-def test_clear_literals(contract, assert_compile_failed, get_contract_with_gas_estimation):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(contract), Exception)
+def test_clear_literals(contract, assert_compile_failed, get_contract):
+    assert_compile_failed(lambda: get_contract(contract), Exception)
 
 
-def test_empty_bytes(get_contract_with_gas_estimation):
+def test_empty_bytes(get_contract):
     code = """
 foobar: Bytes[5]
 
 @external
 def foo() -> (Bytes[5], Bytes[5]):
     self.foobar = b'Hello'
     bar: Bytes[5] = b'World'
 
     self.foobar = empty(Bytes[5])
     bar = empty(Bytes[5])
 
     return (self.foobar, bar)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     a, b = c.foo()
     assert a == b == b""
 
 
 @pytest.mark.parametrize(
     "length,value,result",
     [
@@ -293,21 +293,21 @@
         (8, "", True),
         (40, "a", False),
         (40, "hellohellohellohellohellohellohellohello", False),
         (40, "", True),
     ],
 )
 @pytest.mark.parametrize("op", ["==", "!="])
-def test_empty_string_comparison(get_contract_with_gas_estimation, length, value, result, op):
+def test_empty_string_comparison(get_contract, length, value, result, op):
     contract = f"""
 @external
 def foo(xs: String[{length}]) -> bool:
     return xs {op} empty(String[{length}])
     """
-    c = get_contract_with_gas_estimation(contract)
+    c = get_contract(contract)
     if op == "==":
         assert c.foo(value) == result
     elif op == "!=":
         assert c.foo(value) != result
 
 
 @pytest.mark.parametrize(
@@ -320,28 +320,28 @@
         (8, b"", True),
         (40, b"a", False),
         (40, b"hellohellohellohellohellohellohellohello", False),
         (40, b"", True),
     ],
 )
 @pytest.mark.parametrize("op", ["==", "!="])
-def test_empty_bytes_comparison(get_contract_with_gas_estimation, length, value, result, op):
+def test_empty_bytes_comparison(get_contract, length, value, result, op):
     contract = f"""
 @external
 def foo(xs: Bytes[{length}]) -> bool:
     return empty(Bytes[{length}]) {op} xs
     """
-    c = get_contract_with_gas_estimation(contract)
+    c = get_contract(contract)
     if op == "==":
         assert c.foo(value) == result
     elif op == "!=":
         assert c.foo(value) != result
 
 
-def test_empty_struct(get_contract_with_gas_estimation):
+def test_empty_struct(get_contract):
     code = """
 struct FOOBAR:
     a: int128
     b: uint256
     c: bool
     d: decimal
     e: bytes32
@@ -382,19 +382,19 @@
     assert bar.b == 0
     assert bar.c == False
     assert bar.d == 0.0
     assert bar.e == 0x0000000000000000000000000000000000000000000000000000000000000000
     assert bar.f == empty(address)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     c.foo()
 
 
-def test_empty_dynarray(get_contract_with_gas_estimation):
+def test_empty_dynarray(get_contract):
     code = """
 foobar: DynArray[uint256, 10]
 bar: uint256
 
 @external
 def foo():
     self.bar = 1
@@ -403,21 +403,21 @@
 
     self.foobar = empty(DynArray[uint256, 10])
 
     assert len(self.foobar) == 0
     assert self.bar == 1
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     c.foo()
 
 
 # param empty not working yet
 @pytest.mark.xfail
-def test_param_empty(get_contract_with_gas_estimation):
+def test_param_empty(get_contract):
     code = """
 interface Mirror:
     # reuse the contract for this test by compiling two copies of it
     def test_empty(xs: int128[111], ys: Bytes[1024], zs: Bytes[31]) -> bool: view
 
 # a helper function which will write all over memory with random stuff
 @internal
@@ -443,25 +443,25 @@
     return self.priv(empty(int128[111]), empty(Bytes[1024]), empty(Bytes[31]))
 
 @external
 def pub3(x: address) -> bool:
     self.write_junk_to_memory()
     return staticcall Mirror(x).test_empty(empty(int128[111]), empty(Bytes[1024]), empty(Bytes[31]))
     """
-    c = get_contract_with_gas_estimation(code)
-    mirror = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
+    mirror = get_contract(code)
 
     assert c.test_empty([0] * 111, b"", b"")
     assert c.pub2()
     assert c.pub3(mirror.address)
 
 
 # return empty not working yet
 @pytest.mark.xfail
-def test_return_empty(get_contract_with_gas_estimation):
+def test_return_empty(get_contract):
     code = """
 struct X:
     foo: int128
     bar: address
     baz: decimal
     qux: int128[1]
 
@@ -493,24 +493,24 @@
     return empty(Bytes[55])
 
 @external
 def e() -> X:
     self.write_junk_to_memory()
     return empty(X)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.a() == 0
-    assert c.b() == [0] * 5
-    assert c.c() == [[0] * 5] * 5
+    assert c.b() == (0) * 5
+    assert c.c() == ([0] * 5) * 5
     assert c.d() == b""
     assert c.e() == (0, "0x" + "0" * 40, 0x0, [0])
 
 
-def test_map_clear(get_contract_with_gas_estimation):
+def test_map_clear(get_contract):
     code = """
 big_storage: HashMap[bytes32, bytes32]
 
 @external
 def set(key: bytes32, _value: bytes32):
     self.big_storage[key] = _value
 
@@ -519,27 +519,27 @@
     return self.big_storage[key]
 
 @external
 def delete(key: bytes32):
     self.big_storage[key] = empty(bytes32)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     key = b"test".ljust(32)
     val = b"value".ljust(32)
 
     assert c.get(key) == b"\x00" * 32
-    c.set(key, val, transact={})
+    c.set(key, val)
     assert c.get(key)[:5] == b"value"
-    c.delete(key, transact={})
+    c.delete(key)
     assert c.get(key) == b"\x00" * 32
 
 
-def test_map_clear_nested(get_contract_with_gas_estimation):
+def test_map_clear_nested(get_contract):
     code = """
 big_storage: HashMap[bytes32, HashMap[bytes32, bytes32]]
 
 @external
 def set(key1: bytes32, key2: bytes32, _value: bytes32):
     self.big_storage[key1][key2] = _value
 
@@ -548,28 +548,28 @@
     return self.big_storage[key1][key2]
 
 @external
 def delete(key1: bytes32, key2: bytes32):
     self.big_storage[key1][key2] = empty(bytes32)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     key1 = b"test1".ljust(32)
     key2 = b"test2".ljust(32)
     val = b"value".ljust(32)
 
     assert c.get(key1, key2) == b"\x00" * 32
-    c.set(key1, key2, val, transact={})
+    c.set(key1, key2, val)
     assert c.get(key1, key2)[:5] == b"value"
-    c.delete(key1, key2, transact={})
+    c.delete(key1, key2)
     assert c.get(key1, key2) == b"\x00" * 32
 
 
-def test_map_clear_struct(get_contract_with_gas_estimation):
+def test_map_clear_struct(get_contract):
     code = """
 struct X:
     a: int128
     b: int128
 
 structmap: HashMap[int128, X]
 
@@ -582,21 +582,21 @@
     return self.structmap[123].a, self.structmap[123].b
 
 @external
 def delete():
     self.structmap[123] = empty(X)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
-    assert c.get() == [0, 0]
-    c.set(transact={})
-    assert c.get() == [333, 444]
-    c.delete(transact={})
-    assert c.get() == [0, 0]
+    assert c.get() == (0, 0)
+    c.set()
+    assert c.get() == (333, 444)
+    c.delete()
+    assert c.get() == (0, 0)
 
 
 @pytest.mark.parametrize(
     "contract",
     [
         """
 @external
@@ -618,28 +618,28 @@
 def test_clear_typecheck(contract, get_contract, assert_compile_failed):
     assert_compile_failed(lambda: get_contract(contract), TypeMismatch)
 
 
 @pytest.mark.parametrize(
     "a,b,expected",
     [
-        ("empty(Bytes[65])", "b'hello'", [b"hello", b""]),
-        ("b'hello'", "empty(Bytes[33])", [b"", b"hello"]),
+        ("empty(Bytes[65])", "b'hello'", (b"hello", b"")),
+        ("b'hello'", "empty(Bytes[33])", (b"", b"hello")),
         (
             "empty(Bytes[65])",
             "b'thirty three bytes long baby!!!!!'",
-            [b"thirty three bytes long baby!!!!!", b""],
+            (b"thirty three bytes long baby!!!!!", b""),
         ),
         (
             "b'thirty three bytes long baby!!!aathirty three bytes long baby!!!a'",
             "b'thirty three bytes long baby!!!aa'",
-            [
+            (
                 b"thirty three bytes long baby!!!aa",
                 b"thirty three bytes long baby!!!aathirty three bytes long baby!!!a",
-            ],
+            ),
         ),
     ],
 )
 def test_empty_as_func_arg(get_contract, a, b, expected):
     code_a = """
 @view
 @external
@@ -660,15 +660,15 @@
 def bar(a: address) -> (uint256, Bytes[33], Bytes[65], uint256):
     return staticcall Foo(a).foo(12, {a}, 42, {b})
     """
 
     c1 = get_contract(code_a)
     c2 = get_contract(code_b)
 
-    assert c2.bar(c1.address) == [12] + expected + [42]
+    assert c2.bar(c1.address) == (12, *expected, 42)
 
 
 def test_empty_array_in_event_logging(get_contract, get_logs):
     code = """
 event MyLog:
     arg1: Bytes[64]
     arg2: int128[2][3]
@@ -684,15 +684,16 @@
         314159,
         b'helphelphelphelphelphelphelphelphelphelphelp',
         empty(uint256[3])
     )
     """
 
     c = get_contract(code)
-    log = get_logs(c.foo(transact={}), c, "MyLog")[0]
+    c.foo()
+    (log,) = get_logs(c, "MyLog")
 
     assert log.args.arg1 == b"hello" * 9
     assert log.args.arg2 == [[0, 0], [0, 0], [0, 0]]
     assert log.args.arg3 == 314159
     assert log.args.arg4 == b"help" * 11
     assert log.args.arg5 == [0, 0, 0]
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_extract32.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_extract32.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
 from vyper.evm.opcodes import version_check
 
 
 @pytest.mark.parametrize("location", ["storage", "transient"])
-def test_extract32_extraction(tx_failed, get_contract_with_gas_estimation, location):
+def test_extract32_extraction(tx_failed, get_contract, location):
     if location == "transient" and not version_check(begin="cancun"):
         pytest.skip(
             "Skipping test as storage_location is 'transient' and EVM version is pre-Cancun"
         )
     if location == "storage":
         decl = "y: Bytes[100]"
     elif location == "transient":
@@ -28,15 +28,15 @@
 
 @external
 def extrakt32_storage(index: uint256, inp: Bytes[100]) -> bytes32:
     self.y = inp
     return extract32(self.y, index)
     """
 
-    c = get_contract_with_gas_estimation(extract32_code)
+    c = get_contract(extract32_code)
     test_cases = (
         (b"c" * 31, 0),
         (b"c" * 32, 0),
         (b"c" * 33, 0),
         (b"c" * 33, 1),
         (b"c" * 33, 2),
         (b"cow" * 30, 0),
@@ -56,15 +56,15 @@
             assert c.extrakt32_mem(S, i) == expected_result
             assert c.extrakt32_storage(i, S) == expected_result
         else:
             with tx_failed():
                 c.extrakt32(S, i)
 
 
-def test_extract32_code(tx_failed, get_contract_with_gas_estimation):
+def test_extract32_code(tx_failed, get_contract):
     extract32_code = """
 @external
 def foo(inp: Bytes[32]) -> int128:
     return extract32(inp, 0, output_type=int128)
 
 @external
 def bar(inp: Bytes[32]) -> uint256:
@@ -79,15 +79,15 @@
     return extract32(inp, 0)
 
 @external
 def foq(inp: Bytes[32]) -> address:
     return extract32(inp, 0, output_type=address)
     """
 
-    c = get_contract_with_gas_estimation(extract32_code)
+    c = get_contract(extract32_code)
     assert c.foo(b"\x00" * 30 + b"\x01\x01") == 257
     assert c.bar(b"\x00" * 30 + b"\x01\x01") == 257
 
     with tx_failed():
         c.foo(b"\x80" + b"\x00" * 30)
 
     assert c.bar(b"\x80" + b"\x00" * 31) == 2**255
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_floor.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_floor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from decimal import Decimal
 
 from tests.utils import decimal_to_int
 
 
-def test_floor(get_contract_with_gas_estimation):
+def test_floor(get_contract):
     code = """
 x: decimal
 
 @deploy
 def __init__():
     self.x = 504.0000000001
 
@@ -39,25 +39,25 @@
 @external
 def fou() -> int256:
     a: decimal = 305.0
     b: decimal = 100.0
     c: decimal = a / b
     return floor(c)
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.x_floor() == 504
     assert c.foo() == 1
     assert c.fop() == 1
     assert c.foq() == math.floor(Decimal(2**167 - 1) / 10**10)
     assert c.fos() == 0
     assert c.fot() == 0
     assert c.fou() == 3
 
 
-def test_floor_negative(get_contract_with_gas_estimation):
+def test_floor_negative(get_contract):
     code = """
 x: decimal
 
 @deploy
 def __init__():
     self.x = -504.0000000001
 
@@ -95,52 +95,52 @@
     return floor(c)
 
 @external
 def floor_param(p: decimal) -> int256:
     return floor(p)
 """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.x_floor() == -505
     assert c.foo() == -7
     assert c.fop() == -27
     assert c.foq() == -9001
     assert c.fos() == -1
     assert c.fot() == math.floor(-Decimal(2**167) / 10**10)
     assert c.fou() == -4
     assert c.floor_param(decimal_to_int("-5.6")) == -6
     assert c.floor_param(decimal_to_int("-0.0000000001")) == -1
 
 
-def test_floor_ext_call(w3, side_effects_contract, assert_side_effects_invoked, get_contract):
+def test_floor_ext_call(side_effects_contract, assert_side_effects_invoked, get_contract):
     code = """
 interface Foo:
     def foo(x: decimal) -> decimal: nonpayable
 
 @external
 def foo(a: Foo) -> int256:
     return floor(extcall a.foo(2.5))
     """
 
     c1 = side_effects_contract("decimal")
     c2 = get_contract(code)
 
     assert c2.foo(c1.address) == 2
 
-    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address, transact={}))
+    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address))
 
 
-def test_floor_internal_call(get_contract_with_gas_estimation):
+def test_floor_internal_call(get_contract):
     code = """
 @external
 def foo() -> int256:
     return floor(self.bar())
 
 @internal
 def bar() -> decimal:
     return 2.5
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.foo() == 2
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_is_contract.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_is_contract.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-def test_is_contract(w3, get_contract_with_gas_estimation):
+def test_is_contract(env, get_contract):
     contract_1 = """
 @external
 def foo(arg1: address) -> bool:
     result: bool = arg1.is_contract
     return result
 """
 
     contract_2 = """
 @external
 def foo(arg1: address) -> bool:
     return arg1.is_contract
 """
-    a0, a1 = w3.eth.accounts[:2]
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    a0, a1 = env.accounts[:2]
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.foo(c1.address) is True
     assert c1.foo(c2.address) is True
     assert c1.foo(a1) is False
     assert c1.foo(a0) is False
     assert c2.foo(c1.address) is True
     assert c2.foo(c2.address) is True
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_length.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_length.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pytest
 
 
-def test_test_length(get_contract_with_gas_estimation):
+def test_test_length(get_contract):
     test_length = """
 y: Bytes[10]
 
 @external
 def foo(inp: Bytes[10]) -> uint256:
     x: Bytes[5] = slice(inp,1, 5)
     self.y = slice(inp, 2, 4)
     return len(inp) * 100 + len(x) * 10 + len(self.y)
     """
 
-    c = get_contract_with_gas_estimation(test_length)
+    c = get_contract(test_length)
     assert c.foo(b"badminton") == 954, c.foo(b"badminton")
     print("Passed length test")
 
 
 @pytest.mark.parametrize("typ", ["DynArray[uint256, 50]", "Bytes[50]", "String[50]"])
-def test_zero_length(get_contract_with_gas_estimation, typ):
+def test_zero_length(get_contract, typ):
     code = f"""
 @external
 def boo() -> uint256:
     e: uint256 = len(empty({typ}))
     return e
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.boo() == 0
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_method_id.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_method_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-def test_method_id_test(get_contract_with_gas_estimation):
+def test_method_id_test(get_contract):
     method_id_test = """
 @external
 def double(x: int128) -> int128:
     return x * 2
 
 @external
 def returnten() -> int128:
     ans: Bytes[32] = raw_call(self, concat(method_id("double(int128)"), convert(5, bytes32)), gas=50000, max_outsize=32)  # noqa: E501
     return convert(convert(ans, bytes32), int128)
     """
-    c = get_contract_with_gas_estimation(method_id_test)
+    c = get_contract(method_id_test)
     assert c.returnten() == 10
 
 
 def test_method_id_bytes4(get_contract):
     code = """
 @external
 def sig() -> bytes4:
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_minmax.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_minmax.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import pytest
 
 from tests.utils import decimal_to_int
 from vyper.semantics.types import IntegerT
 
 
-def test_minmax(get_contract_with_gas_estimation):
+def test_minmax(get_contract):
     minmax_test = """
 @external
 def foo() -> decimal:
     return min(3.0, 5.0) + max(10.0, 20.0) + min(200.1, 400.0) + max(3000.0, 8000.02) + min(50000.003, 70000.004)  # noqa: E501
 
 @external
 def goo() -> uint256:
     return min(3, 5) + max(40, 80)
     """
 
-    c = get_contract_with_gas_estimation(minmax_test)
+    c = get_contract(minmax_test)
     assert c.foo() == decimal_to_int("58223.123")
     assert c.goo() == 83
 
     print("Passed min/max test")
 
 
 @pytest.mark.parametrize("return_type", sorted(IntegerT.all()))
-def test_minmax_var_and_literal_and_bultin(get_contract_with_gas_estimation, return_type):
+def test_minmax_var_and_literal_and_bultin(get_contract, return_type):
     """
     Tests to verify that min and max work as expected when a variable/literal
     and a literal are passed for all integer types.
     """
     lo, hi = return_type.ast_bounds
 
     code = f"""
@@ -55,24 +55,24 @@
 def both_builtins_max() -> {return_type}:
     return max(min_value({return_type}), max_value({return_type}))
 
 @external
 def both_builtins_min() -> {return_type}:
     return min(min_value({return_type}), max_value({return_type}))
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == hi
     assert c.bar() == lo
     assert c.both_literals_max() == hi
     assert c.both_literals_min() == lo
     assert c.both_builtins_max() == hi
     assert c.both_builtins_min() == lo
 
 
-def test_max_var_uint256_literal_int128(get_contract_with_gas_estimation):
+def test_max_var_uint256_literal_int128(get_contract):
     """
     Tests to verify that max works as expected when a variable/literal uint256
     and a literal int128 are passed.
     """
     code = """
 @external
 def foo() -> uint256:
@@ -98,23 +98,23 @@
     b: uint256 = 5
     return max(5, a) + max(5, b)
 
 @external
 def both_literals() -> uint256:
     return max(2 ** 200, 2)
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == 2**200 + 5
     assert c.goo() == 2**200 + 5
     assert c.bar() == 5 + 5
     assert c.baz() == 5 + 5
     assert c.both_literals() == 2**200
 
 
-def test_min_var_uint256_literal_int128(get_contract_with_gas_estimation):
+def test_min_var_uint256_literal_int128(get_contract):
     """
     Tests to verify that max works as expected when a variable/literal uint256
     and a literal int128 are passed.
     """
     code = """
 @external
 def foo() -> uint256:
@@ -140,89 +140,87 @@
     b: uint256 = 5
     return min(5, a) + min(5, b)
 
 @external
 def both_literals() -> uint256:
     return min(2 ** 200, 2)
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == 5 + 5
     assert c.goo() == 5 + 5
     assert c.bar() == 2 + 5
     assert c.baz() == 2 + 5
     assert c.both_literals() == 2
 
 
-def test_minmax_var_uint256_var_int128(get_contract_with_gas_estimation, assert_compile_failed):
+def test_minmax_var_uint256_var_int128(get_contract, assert_compile_failed):
     """
     Tests to verify that max throws an error if a variable uint256 and a
     variable int128 are passed.
     """
     from vyper.exceptions import TypeMismatch
 
     code_1 = """
 @external
 def foo() -> uint256:
     a: uint256 = 2
     b: int128 = 3
     return max(a, b)
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code_1), TypeMismatch)
+    assert_compile_failed(lambda: get_contract(code_1), TypeMismatch)
 
     code_2 = """
 @external
 def foo() -> uint256:
     a: uint256 = 2
     b: int128 = 3
     return max(b, a)
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code_2), TypeMismatch)
+    assert_compile_failed(lambda: get_contract(code_2), TypeMismatch)
 
     code_3 = """
 @external
 def foo() -> uint256:
     a: uint256 = 2
     b: int128 = 3
     return min(a, b)
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code_3), TypeMismatch)
+    assert_compile_failed(lambda: get_contract(code_3), TypeMismatch)
 
     code_4 = """
 @external
 def foo() -> uint256:
     a: uint256 = 2
     b: int128 = 3
     return min(b, a)
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code_4), TypeMismatch)
+    assert_compile_failed(lambda: get_contract(code_4), TypeMismatch)
 
 
-def test_minmax_var_uint256_negative_int128(
-    get_contract_with_gas_estimation, tx_failed, assert_compile_failed
-):
+def test_minmax_var_uint256_negative_int128(get_contract, tx_failed, assert_compile_failed):
     from vyper.exceptions import TypeMismatch
 
     code_1 = """
 @external
 def foo() -> uint256:
     a: uint256 = 2 ** 200
     return max(a, -1)
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code_1), TypeMismatch)
+    assert_compile_failed(lambda: get_contract(code_1), TypeMismatch)
 
     code_2 = """
 @external
 def foo() -> uint256:
     a: uint256 = 2 ** 200
     return min(a, -1)
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code_2), TypeMismatch)
+    assert_compile_failed(lambda: get_contract(code_2), TypeMismatch)
 
 
-def test_unsigned(get_contract_with_gas_estimation):
+def test_unsigned(get_contract):
     code = """
 @external
 def foo1() -> uint256:
     return min(0, 2**255)
 
 @external
 def foo2() -> uint256:
@@ -233,22 +231,22 @@
     return max(0, 2**255)
 
 @external
 def foo4() -> uint256:
     return max(2**255, 0)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo1() == 0
     assert c.foo2() == 0
     assert c.foo3() == 2**255
     assert c.foo4() == 2**255
 
 
-def test_signed(get_contract_with_gas_estimation):
+def test_signed(get_contract):
     code = """
 @external
 def foo1() -> int128:
     return min(min_value(int128), max_value(int128))
 
 @external
 def foo2() -> int128:
@@ -259,12 +257,12 @@
     return max(min_value(int128), max_value(int128))
 
 @external
 def foo4() -> int128:
     return max(max_value(int128), min_value(int128))
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo1() == -(2**127)
     assert c.foo2() == -(2**127)
     assert c.foo3() == 2**127 - 1
     assert c.foo4() == 2**127 - 1
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_minmax_value.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_mulmod.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_mulmod.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,60 @@
-def test_uint256_mulmod(tx_failed, get_contract_with_gas_estimation):
+def test_uint256_mulmod(tx_failed, get_contract):
     uint256_code = """
 @external
 def _uint256_mulmod(x: uint256, y: uint256, z: uint256) -> uint256:
     return uint256_mulmod(x, y, z)
     """
 
-    c = get_contract_with_gas_estimation(uint256_code)
+    c = get_contract(uint256_code)
 
     assert c._uint256_mulmod(3, 1, 2) == 1
     assert c._uint256_mulmod(200, 3, 601) == 600
     assert c._uint256_mulmod(2**255, 1, 3) == 2
     assert c._uint256_mulmod(2**255, 2, 6) == 4
     with tx_failed():
         c._uint256_mulmod(2, 2, 0)
 
 
-def test_uint256_mulmod_complex(get_contract_with_gas_estimation):
+def test_uint256_mulmod_complex(get_contract):
     modexper = """
 @external
 def exponential(base: uint256, exponent: uint256, modulus: uint256) -> uint256:
     o: uint256 = 1
     for i: uint256 in range(256):
         o = uint256_mulmod(o, o, modulus)
         if exponent & shift(1, 255 - i) != 0:
             o = uint256_mulmod(o, base, modulus)
     return o
     """
 
-    c = get_contract_with_gas_estimation(modexper)
+    c = get_contract(modexper)
     assert c.exponential(3, 5, 100) == 43
     assert c.exponential(2, 997, 997) == 2
 
 
-def test_uint256_mulmod_ext_call(
-    w3, side_effects_contract, assert_side_effects_invoked, get_contract
-):
+def test_uint256_mulmod_ext_call(side_effects_contract, assert_side_effects_invoked, get_contract):
     code = """
 interface Foo:
     def foo(x: uint256) -> uint256: nonpayable
 
 @external
 def foo(f: Foo) -> uint256:
     return uint256_mulmod(200, 3, extcall f.foo(601))
     """
 
     c1 = side_effects_contract("uint256")
     c2 = get_contract(code)
 
     assert c2.foo(c1.address) == 600
 
-    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address, transact={}))
+    assert_side_effects_invoked(c1, lambda: c2.foo(c1.address))
 
 
-def test_uint256_mulmod_internal_call(get_contract_with_gas_estimation):
+def test_uint256_mulmod_internal_call(get_contract):
     code = """
 @external
 def foo() -> uint256:
     return uint256_mulmod(self.a(), self.b(), self.c())
 
 @internal
 def a() -> uint256:
@@ -67,20 +65,20 @@
     return 3
 
 @internal
 def c() -> uint256:
     return 601
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.foo() == 600
 
 
-def test_uint256_mulmod_evaluation_order(get_contract_with_gas_estimation):
+def test_uint256_mulmod_evaluation_order(get_contract):
     code = """
 a: uint256
 
 @external
 def foo1() -> uint256:
     self.a = 1
     return uint256_mulmod(self.a, 2, self.bar())
@@ -97,12 +95,12 @@
 
 @internal
 def bar() -> uint256:
     self.a = 7
     return 5
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.foo1() == 2
     assert c.foo2() == 1
     assert c.foo3() == 2
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_raw_call.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_raw_call.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import pytest
 from hexbytes import HexBytes
 
+from tests.utils import ZERO_ADDRESS
 from vyper import compile_code
 from vyper.builtins.functions import eip1167_bytecode
 from vyper.exceptions import ArgumentException, StateAccessViolation, TypeMismatch
 
-pytestmark = pytest.mark.usefixtures("memory_mocker")
-
 
 def test_max_outsize_exceeds_returndatasize(get_contract):
     source_code = """
 @external
 def foo() -> Bytes[7]:
     return raw_call(0x0000000000000000000000000000000000000004, b"moose", max_outsize=7)
     """
@@ -46,85 +45,85 @@
 def foo() -> Bytes[5]:
     return raw_call(0x0000000000000000000000000000000000000004, b"moose", max_outsize=5)
     """
     c = get_contract(source_code)
     assert c.foo() == b"moose"
 
 
-def test_multiple_levels(w3, get_contract_with_gas_estimation):
+def test_multiple_levels(env, get_contract):
     inner_code = """
 @external
 def returnten() -> int128:
     return 10
     """
 
-    c = get_contract_with_gas_estimation(inner_code)
+    c = get_contract(inner_code)
 
     outer_code = """
 @external
 def create_and_call_returnten(inp: address) -> int128:
     x: address = create_minimal_proxy_to(inp)
     o: int128 = extract32(raw_call(x, b"\\xd0\\x1f\\xb1\\xb8", max_outsize=32, gas=50000), 0, output_type=int128)  # noqa: E501
     return o
 
 @external
 def create_and_return_proxy(inp: address) -> address:
     x: address = create_minimal_proxy_to(inp)
     return x
     """
 
-    c2 = get_contract_with_gas_estimation(outer_code)
+    c2 = get_contract(outer_code)
     assert c2.create_and_call_returnten(c.address) == 10
-    c2.create_and_call_returnten(c.address, transact={})
+    c2.create_and_call_returnten(c.address)
 
     _, preamble, callcode = eip1167_bytecode()
 
-    c3 = c2.create_and_return_proxy(c.address, call={})
-    c2.create_and_return_proxy(c.address, transact={})
+    c3 = c2.create_and_return_proxy(c.address)
+    c2.create_and_return_proxy(c.address)
 
-    c3_contract_code = w3.to_bytes(w3.eth.get_code(c3))
+    c3_contract_code = env.get_code(c3)
 
     assert c3_contract_code[:10] == HexBytes(preamble)
     assert c3_contract_code[-15:] == HexBytes(callcode)
 
     print("Passed proxy test")
     # TODO: This one is special
     # print(f'Gas consumed: {(chain.head_state.receipts[-1].gas_used - chain.head_state.receipts[-2].gas_used - chain.last_tx.intrinsic_gas_used)}')  # noqa: E501
 
 
-def test_multiple_levels2(tx_failed, get_contract_with_gas_estimation):
+def test_multiple_levels2(tx_failed, get_contract):
     inner_code = """
 @external
 def returnten() -> int128:
     raise
     """
 
-    c = get_contract_with_gas_estimation(inner_code)
+    c = get_contract(inner_code)
 
     outer_code = """
 @external
 def create_and_call_returnten(inp: address) -> int128:
     x: address = create_minimal_proxy_to(inp)
     o: int128 = extract32(raw_call(x, b"\\xd0\\x1f\\xb1\\xb8", max_outsize=32, gas=50000), 0, output_type=int128)  # noqa: E501
     return o
 
 @external
 def create_and_return_proxy(inp: address) -> address:
     return create_minimal_proxy_to(inp)
     """
 
-    c2 = get_contract_with_gas_estimation(outer_code)
+    c2 = get_contract(outer_code)
 
     with tx_failed():
         c2.create_and_call_returnten(c.address)
 
     print("Passed minimal proxy exception test")
 
 
-def test_delegate_call(w3, get_contract):
+def test_delegate_call(env, get_contract):
     inner_code = """
 a: address  # this is required for storage alignment...
 owners: public(address[5])
 
 @external
 def set_owner(i: int128, o: address):
     self.owners[i] = o
@@ -151,28 +150,27 @@
         cdata,
         gas=msg.gas,
         max_outsize=0,
         is_delegate_call=True
     )
     """
 
-    a0, a1, a2 = w3.eth.accounts[:3]
-    outer_contract = get_contract(outer_code, *[inner_contract.address])
+    a0, a1, a2 = env.accounts[:3]
+    outer_contract = get_contract(outer_code, inner_contract.address)
 
     # Test setting on inners contract's state setting works.
-    inner_contract.set_owner(1, a2, transact={})
+    inner_contract.set_owner(1, a2)
     assert inner_contract.owners(1) == a2
 
     # Confirm outer contract's state is empty and contract to call has been set.
     assert outer_contract.owner_setter_contract() == inner_contract.address
-    assert outer_contract.owners(1) is None
+    assert outer_contract.owners(1) == ZERO_ADDRESS
 
     # Call outer contract, that make a delegate call to inner_contract.
-    tx_hash = outer_contract.set(1, a1, transact={})
-    assert w3.eth.get_transaction_receipt(tx_hash)["status"] == 1
+    outer_contract.set(1, a1)
     assert outer_contract.owners(1) == a1
 
 
 def test_gas(get_contract, tx_failed):
     inner_code = """
 bar: bytes32
 
@@ -198,15 +196,15 @@
     outer_contract.foo_call(inner_contract.address)
 
     # manually specifying a sufficient amount should succeed
     outer_contract = get_contract(outer_code.format(", gas=50000"))
     outer_contract.foo_call(inner_contract.address)
 
     # manually specifying an insufficient amount should fail
-    outer_contract = get_contract(outer_code.format(", gas=15000"))
+    outer_contract = get_contract(outer_code.format(", gas=2250"))
     with tx_failed():
         outer_contract.foo_call(inner_contract.address)
 
 
 def test_static_call(get_contract):
     target_source = """
 @external
@@ -230,15 +228,15 @@
 
     target = get_contract(target_source)
     caller = get_contract(caller_source)
 
     assert caller.foo(target.address) == 42
 
 
-def test_forward_calldata(get_contract, w3, keccak):
+def test_forward_calldata(get_contract, env, keccak):
     target_source = """
 @external
 def foo() -> uint256:
     return 123
     """
 
     caller_source = """
@@ -252,19 +250,19 @@
 def __default__():
     assert 123 == _abi_decode(raw_call(self.target, msg.data, max_outsize=32), uint256)
     """
 
     target = get_contract(target_source)
 
     caller = get_contract(caller_source)
-    caller.set_target(target.address, transact={})
+    caller.set_target(target.address)
 
     # manually construct msg.data for `caller` contract
     sig = keccak("foo()".encode()).hex()[:10]
-    w3.eth.send_transaction({"to": caller.address, "data": sig})
+    assert env.message_call(caller.address, data=sig) == b""
 
 
 # check max_outsize=0 does same thing as not setting max_outsize.
 # compile to bytecode and compare bytecode directly.
 def test_max_outsize_0():
     code1 = """
 @external
@@ -513,15 +511,15 @@
     self.buf = raw_call(self.bar(), msg.data, value = self.goo(), max_outsize=100)
     return self.canary
     """
     c = get_contract(code)
     assert c.foo() == "goo"
 
 
-def test_raw_call_clean_mem_kwargs_value(get_contract):
+def test_raw_call_clean_mem_kwargs_value(get_contract, env):
     # test msize uses clean memory and does not get overwritten by
     # any raw_call() kwargs
     code = """
 buf: Bytes[100]
 
 # add a dummy function to trigger memory expansion in the selector table routine
 @external
@@ -540,23 +538,24 @@
         0x0000000000000000000000000000000000000004,
         msg.data,
         max_outsize=100,
         value=self._value()
     )
     return self.buf
     """
+    env.set_balance(env.deployer, 1)
     c = get_contract(code, value=1)
 
     assert (
         c.bar(13).hex() == "0423a132"
         "000000000000000000000000000000000000000000000000000000000000000d"
     )
 
 
-def test_raw_call_clean_mem_kwargs_gas(get_contract):
+def test_raw_call_clean_mem_kwargs_gas(get_contract, env):
     # test msize uses clean memory and does not get overwritten by
     # any raw_call() kwargs
     code = """
 buf: Bytes[100]
 
 # add a dummy function to trigger memory expansion in the selector table routine
 @external
@@ -575,14 +574,15 @@
         0x0000000000000000000000000000000000000004,
         msg.data,
         max_outsize=100,
         gas=self._gas()
     )
     return self.buf
     """
+    env.set_balance(env.deployer, 1)
     c = get_contract(code, value=1)
 
     assert (
         c.bar(15).hex() == "0423a132"
         "000000000000000000000000000000000000000000000000000000000000000f"
     )
 
@@ -630,11 +630,9 @@
     """,
         TypeMismatch,
     ),
 ]
 
 
 @pytest.mark.parametrize("source_code,exc", uncompilable_code)
-def test_invalid_type_exception(
-    assert_compile_failed, get_contract_with_gas_estimation, source_code, exc
-):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(source_code), exc)
+def test_invalid_type_exception(assert_compile_failed, get_contract, source_code, exc):
+    assert_compile_failed(lambda: get_contract(source_code), exc)
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_send.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_send.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-def test_send(tx_failed, get_contract):
+from tests.utils import ZERO_ADDRESS
+
+
+def test_send(tx_failed, get_contract, env):
     send_test = """
 @external
 def foo():
     send(msg.sender, self.balance + 1)
 
 @external
 def fop():
     send(msg.sender, 10)
     """
+    env.set_balance(env.deployer, 1000)
     c = get_contract(send_test, value=10)
     with tx_failed():
-        c.foo(transact={})
-    c.fop(transact={})
+        c.foo()
+    assert env.get_balance(c.address) == 10
+    c.fop()
+    assert env.get_balance(c.address) == 0
     with tx_failed():
-        c.fop(transact={})
+        c.fop()
 
 
-def test_default_gas(get_contract, w3):
+def test_default_gas(get_contract, env, tx_failed):
     """
     Tests to verify that send to default function will send limited gas (2300),
     but raw_call can send more.
     """
 
     sender_code = """
 @external
@@ -38,33 +44,35 @@
 
 @external
 @payable
 def __default__():
     self.last_sender = msg.sender
     """
 
+    env.set_balance(env.deployer, 300000)
     sender = get_contract(sender_code, value=1)
     receiver = get_contract(receiver_code)
 
-    sender.test_send(receiver.address, transact={"gas": 100000})
+    with tx_failed():
+        sender.test_send(receiver.address, gas=100000)
 
     # no value transfer happened, variable was not changed
-    assert receiver.last_sender() is None
-    assert w3.eth.get_balance(sender.address) == 1
-    assert w3.eth.get_balance(receiver.address) == 0
+    assert receiver.last_sender() == ZERO_ADDRESS
+    assert env.get_balance(sender.address) == 1
+    assert env.get_balance(receiver.address) == 0
 
-    sender.test_call(receiver.address, transact={"gas": 100000})
+    sender.test_call(receiver.address, gas=100000)
 
     # value transfer happened, variable was changed
     assert receiver.last_sender() == sender.address
-    assert w3.eth.get_balance(sender.address) == 0
-    assert w3.eth.get_balance(receiver.address) == 1
+    assert env.get_balance(sender.address) == 0
+    assert env.get_balance(receiver.address) == 1
 
 
-def test_send_gas_stipend(get_contract, w3):
+def test_send_gas_stipend(get_contract, env):
     """
     Tests to verify that adding gas stipend to send() will send sufficient gas
     """
 
     sender_code = """
 
 @external
@@ -79,16 +87,17 @@
 
 @external
 @payable
 def __default__():
     self.last_sender = msg.sender
     """
 
+    env.set_balance(env.deployer, 300000)
     sender = get_contract(sender_code, value=1)
     receiver = get_contract(receiver_code)
 
-    sender.test_send_stipend(receiver.address, transact={"gas": 100000})
+    sender.test_send_stipend(receiver.address, gas=100000)
 
     # value transfer happened, variable was changed
     assert receiver.last_sender() == sender.address
-    assert w3.eth.get_balance(sender.address) == 0
-    assert w3.eth.get_balance(receiver.address) == 1
+    assert env.get_balance(sender.address) == 0
+    assert env.get_balance(receiver.address) == 1
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_sha256.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_sha256.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,105 @@
 import hashlib
 
-import pytest
-
 from vyper.utils import hex_to_int
 
-pytestmark = pytest.mark.usefixtures("memory_mocker")
-
 
-def test_sha256_string_literal(get_contract_with_gas_estimation):
+def test_sha256_string_literal(get_contract):
     code = """
 @external
 def bar() -> bytes32:
     return sha256("test")
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.bar() == hashlib.sha256(b"test").digest()
 
 
-def test_sha256_literal_bytes(get_contract_with_gas_estimation):
+def test_sha256_literal_bytes(get_contract):
     code = """
 @external
 def bar() -> (bytes32 , bytes32):
     x: bytes32 = sha256("test")
     y: bytes32 = sha256(b"test")
     return x, y
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     h = hashlib.sha256(b"test").digest()
-    assert c.bar() == [h, h]
+    assert c.bar() == (h, h)
 
 
-def test_sha256_bytes32(get_contract_with_gas_estimation):
+def test_sha256_bytes32(get_contract):
     code = """
 @external
 def bar(a: bytes32) -> bytes32:
     return sha256(a)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     test_val = 8 * b"bBaA"
     assert c.bar(test_val) == hashlib.sha256(test_val).digest()
 
 
-def test_sha256_bytearraylike(get_contract_with_gas_estimation):
+def test_sha256_bytearraylike(get_contract):
     code = """
 @external
 def bar(a: String[100]) -> bytes32:
     return sha256(a)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     test_val = "test me! test me!"
     assert c.bar(test_val) == hashlib.sha256(test_val.encode()).digest()
     test_val = "fun"
     assert c.bar(test_val) == hashlib.sha256(test_val.encode()).digest()
 
 
-def test_sha256_bytearraylike_storage(get_contract_with_gas_estimation):
+def test_sha256_bytearraylike_storage(get_contract):
     code = """
 a: public(Bytes[100])
 
 @external
 def set(b: Bytes[100]):
     self.a = b
 
 @external
 def bar() -> bytes32:
     return sha256(self.a)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     test_val = b"test me! test me!"
-    c.set(test_val, transact={})
+    c.set(test_val)
     assert c.a() == test_val
     assert c.bar() == hashlib.sha256(test_val).digest()
 
 
-def test_sha256_constant_bytes32(get_contract_with_gas_estimation):
+def test_sha256_constant_bytes32(get_contract):
     hex_val = "0x1234567890123456789012345678901234567890123456789012345678901234"
     code = f"""
 FOO: constant(bytes32) = {hex_val}
 BAR: constant(bytes32) = sha256(FOO)
 @external
 def foo() -> bytes32:
     x: bytes32 = BAR
     return x
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == hashlib.sha256(hex_to_int(hex_val).to_bytes(32, "big")).digest()
 
 
-def test_sha256_constant_string(get_contract_with_gas_estimation):
+def test_sha256_constant_string(get_contract):
     str_val = "0x1234567890123456789012345678901234567890123456789012345678901234"
     code = f"""
 FOO: constant(String[66]) = "{str_val}"
 BAR: constant(bytes32) = sha256(FOO)
 @external
 def foo() -> bytes32:
     x: bytes32 = BAR
     return x
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == hashlib.sha256(str_val.encode()).digest()
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_slice.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_slice.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 _fun_bytes32_bounds = [(0, 32), (3, 29), (27, 5), (0, 5), (5, 3), (30, 2)]
 
 
 def _generate_bytes(length):
     return bytes(list(range(length)))
 
 
-def test_basic_slice(get_contract_with_gas_estimation):
+def test_basic_slice(get_contract):
     code = """
 @external
 def slice_tower_test(inp1: Bytes[50]) -> Bytes[50]:
     inp: Bytes[50] = inp1
     for i: uint256 in range(1, 11):
         inp = slice(inp, 1, 30 - i * 2)
     return inp
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     x = c.slice_tower_test(b"abcdefghijklmnopqrstuvwxyz1234")
     assert x == b"klmnopqrst", x
 
 
 # note: optimization boundaries at 32, 64 and 320 depending on mode
 _draw_1024 = st.integers(min_value=0, max_value=1024)
 _draw_1024_1 = st.integers(min_value=1, max_value=1024)
@@ -162,15 +162,20 @@
 @external
 def do_slice(inp: Bytes[{length_bound}], start: uint256, length: uint256) -> Bytes[{length_bound}]:
     {spliced_code}
     return slice({foo}, {_start}, {_length})
     """
 
     def _get_contract():
-        return get_contract(code, bytesdata, override_opt_level=opt_level)
+        if "__init__" in code:
+            # eth-tester used to ignore constructor arguments if no constructor was defined
+            # now we raise an exception, so only call the constructor if it exists
+            # TODO: Refactor so we don't rely on searching the source code.
+            return get_contract(code, bytesdata, override_opt_level=opt_level)
+        return get_contract(code, override_opt_level=opt_level)
 
     # length bound is the container size; input_bound is the bound on the input
     # (which can be different, if the input is a literal)
     input_bound = length_bound
     slice_output_too_large = False
 
     if location == "literal":
@@ -233,20 +238,20 @@
 def foo(x: uint256, y: uint256) -> (uint256, String[12]):
     self.bytez = "hello, world"
     dont_clobber_me: uint256 = max_value(uint256)
     self._slice(x, y)
     return dont_clobber_me, self.bytez
     """
     c = get_contract(code)
-    assert c.foo(0, 12) == [2**256 - 1, "hello, world"]
-    assert c.foo(12, 0) == [2**256 - 1, ""]
-    assert c.foo(7, 5) == [2**256 - 1, "world"]
-    assert c.foo(0, 5) == [2**256 - 1, "hello"]
-    assert c.foo(0, 1) == [2**256 - 1, "h"]
-    assert c.foo(11, 1) == [2**256 - 1, "d"]
+    assert c.foo(0, 12) == (2**256 - 1, "hello, world")
+    assert c.foo(12, 0) == (2**256 - 1, "")
+    assert c.foo(7, 5) == (2**256 - 1, "world")
+    assert c.foo(0, 5) == (2**256 - 1, "hello")
+    assert c.foo(0, 1) == (2**256 - 1, "h")
+    assert c.foo(11, 1) == (2**256 - 1, "d")
 
 
 def test_slice_storage_bytes32(get_contract):
     code = """
 bytez: bytes32
 @external
 def dice() -> Bytes[1]:
@@ -255,27 +260,27 @@
     return c
     """
 
     c = get_contract(code)
     assert c.dice() == b"A"
 
 
-def test_slice_immutable_length_arg(get_contract_with_gas_estimation):
+def test_slice_immutable_length_arg(get_contract):
     code = """
 LENGTH: immutable(uint256)
 
 @deploy
 def __init__():
     LENGTH = 5
 
 @external
 def do_slice(inp: Bytes[50]) -> Bytes[50]:
     return slice(inp, 0, LENGTH)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     x = c.do_slice(b"abcdefghijklmnopqrstuvwxyz1234")
     assert x == b"abcde", x
 
 
 def test_slice_at_end(get_contract):
     code = """
 @external
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_uint2str.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_uint2str.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from vyper.compiler import compile_code
 from vyper.exceptions import InvalidType, OverflowException
 
 VALID_BITS = list(range(8, 257, 8))
 
 
 @pytest.mark.parametrize("bits", VALID_BITS)
-def test_mkstr(get_contract_with_gas_estimation, bits):
+def test_mkstr(get_contract, bits):
     n_digits = math.ceil(bits * math.log(2) / math.log(10))
     code = f"""
 @external
 def foo(inp: uint{bits}) -> String[{n_digits}]:
     return uint2str(inp)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     for i in [1, 2, 2**bits - 1, 0]:
         assert c.foo(i) == str(i), (i, c.foo(i))
 
 
 # test for buffer overflow
 @pytest.mark.parametrize("bits", VALID_BITS)
 def test_mkstr_buffer(get_contract, bits):
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_unary.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_unary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/codegen/test_unsafe_math.py` & `vyper-0.4.0rc3/tests/functional/builtins/codegen/test_unsafe_math.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/folding/test_abs.py` & `vyper-0.4.0rc3/tests/functional/builtins/folding/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/folding/test_addmod_mulmod.py` & `vyper-0.4.0rc3/tests/functional/builtins/folding/test_addmod_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/folding/test_bitwise.py` & `vyper-0.4.0rc3/tests/functional/builtins/folding/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/folding/test_floor_ceil.py` & `vyper-0.4.0rc3/tests/functional/builtins/folding/test_floor_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/folding/test_fold_as_wei_value.py` & `vyper-0.4.0rc3/tests/functional/builtins/folding/test_fold_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/folding/test_keccak_sha.py` & `vyper-0.4.0rc3/tests/functional/builtins/folding/test_keccak_sha.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from tests.utils import parse_and_fold
 
-alphabet = '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!"#$%&()*+,-./:;<=>?@[]^_`{|}~'  # NOQA: E501
+alphabet = '0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!"#$%&()*+,-./:;<=>?@[]^_`{|}~'  # NOQA: E501, FS003
 
 
 @pytest.mark.fuzzing
 @given(value=st.text(alphabet=alphabet, min_size=0, max_size=100))
 @settings(max_examples=50)
 @pytest.mark.parametrize("fn_name", ["keccak256", "sha256"])
 def test_string(get_contract, value, fn_name):
```

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/folding/test_len.py` & `vyper-0.4.0rc3/tests/functional/builtins/folding/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/folding/test_min_max.py` & `vyper-0.4.0rc3/tests/functional/builtins/folding/test_min_max.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/builtins/folding/test_powmod.py` & `vyper-0.4.0rc3/tests/functional/builtins/folding/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_default_parameters.py` & `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_default_parameters.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import pytest
 
+from tests.utils import ZERO_ADDRESS
 from vyper.compiler import compile_code
 from vyper.exceptions import (
     InvalidLiteral,
     NonPayableViolation,
     StateAccessViolation,
     TypeMismatch,
     UndeclaredDefinition,
 )
+from vyper.utils import method_id
 
 
 def test_default_param_abi(get_contract):
     code = """
 @external
 @payable
 def safeTransferFrom(_data: Bytes[100] = b"test", _b: int128 = 1):
     pass
     """
-    abi = get_contract(code)._classic_contract.abi
+    abi = get_contract(code).abi
 
     assert len(abi) == 3
     assert set([fdef["name"] for fdef in abi]) == {"safeTransferFrom"}
     assert abi[0]["inputs"] == []
     assert abi[1]["inputs"] == [{"type": "bytes", "name": "_data"}]
     assert abi[2]["inputs"] == [
         {"type": "bytes", "name": "_data"},
@@ -47,16 +49,16 @@
     code = """
 @external
 def fooBar(a:int128, b: uint256 = 333) -> (int128, uint256):
     return a, b
     """
 
     c = get_contract(code)
-    assert c.fooBar(456, 444) == [456, 444]
-    assert c.fooBar(456) == [456, 333]
+    assert c.fooBar(456, 444) == (456, 444)
+    assert c.fooBar(456) == (456, 333)
 
 
 def test_basic_default_param_set_2args(get_contract):
     code = """
 @external
 def fooBar(a:int128, b: uint256 = 999, c: address = 0x0000000000000000000000000000000000000001) -> (int128, uint256, address):  # noqa: E501
     return a, b, c
@@ -64,55 +66,55 @@
 
     c = get_contract(code)
     c_default_value = "0x0000000000000000000000000000000000000001"
     b_default_value = 999
     addr2 = "0x1000000000000000000000000000000000004321"
 
     # b default value, c default value
-    assert c.fooBar(123) == [123, b_default_value, c_default_value]
+    assert c.fooBar(123) == (123, b_default_value, c_default_value)
     # c default_value, b set from param
-    assert c.fooBar(456, 444) == [456, 444, c_default_value]
+    assert c.fooBar(456, 444) == (456, 444, c_default_value)
     # no default values
-    assert c.fooBar(6789, 4567, addr2) == [6789, 4567, addr2]
+    assert c.fooBar(6789, 4567, addr2) == (6789, 4567, addr2)
 
 
 def test_default_param_bytes(get_contract):
     code = """
 @external
 def fooBar(a: Bytes[100], b: int128, c: Bytes[100] = b"testing", d: uint256 = 999) -> (Bytes[100], int128, Bytes[100], uint256):  # noqa: E501
     return a, b, c, d
     """
     c = get_contract(code)
     c_default = b"testing"
     d_default = 999
 
     # c set, 7d default value
-    assert c.fooBar(b"booo", 12321, b"woo") == [b"booo", 12321, b"woo", d_default]
+    assert c.fooBar(b"booo", 12321, b"woo") == (b"booo", 12321, b"woo", d_default)
     # d set, c set
-    assert c.fooBar(b"booo", 12321, b"lucky", 777) == [b"booo", 12321, b"lucky", 777]
+    assert c.fooBar(b"booo", 12321, b"lucky", 777) == (b"booo", 12321, b"lucky", 777)
     # no default values
-    assert c.fooBar(b"booo", 12321) == [b"booo", 12321, c_default, d_default]
+    assert c.fooBar(b"booo", 12321) == (b"booo", 12321, c_default, d_default)
 
 
 def test_default_param_array(get_contract):
     code = """
 @external
 def fooBar(a: Bytes[100], b: uint256[2], c: Bytes[6] = b"hello", d: int128[3] = [6, 7, 8]) -> (Bytes[100], uint256, Bytes[6], int128):  # noqa: E501
     return a, b[1], c, d[2]
     """
     c = get_contract(code)
     c_default = b"hello"
     d_default = 8
 
     # c set, d default value
-    assert c.fooBar(b"booo", [99, 88], b"woo") == [b"booo", 88, b"woo", d_default]
+    assert c.fooBar(b"booo", [99, 88], b"woo") == (b"booo", 88, b"woo", d_default)
     # d set, c set
-    assert c.fooBar(b"booo", [22, 11], b"lucky", [24, 25, 26]) == [b"booo", 11, b"lucky", 26]
+    assert c.fooBar(b"booo", [22, 11], b"lucky", [24, 25, 26]) == (b"booo", 11, b"lucky", 26)
     # no default values
-    assert c.fooBar(b"booo", [55, 66]) == [b"booo", 66, c_default, d_default]
+    assert c.fooBar(b"booo", [55, 66]) == (b"booo", 66, c_default, d_default)
 
 
 def test_default_param_interface(get_contract):
     code = """
 interface Foo:
     def bar(): payable
 
@@ -133,16 +135,16 @@
     c = get_contract(code)
 
     addr1 = "0xFFfFfFffFFfffFFfFFfFFFFFffFFFffffFfFFFfF"
     addr2 = "0xF5D4020dCA6a62bB1efFcC9212AAF3c9819E30D7"
 
     assert c.bar(1) == addr2
     assert c.bar(1, addr1) == addr1
-    assert c.baz(1) is None
-    assert c.baz(1, "0x0000000000000000000000000000000000000000") is None
+    assert c.baz(1) == ZERO_ADDRESS
+    assert c.baz(1, ZERO_ADDRESS) == ZERO_ADDRESS
     assert c.faz(1) == addr1
     assert c.faz(1, addr1) == addr1
 
 
 def test_default_param_internal_function(get_contract):
     code = """
 @internal
@@ -178,34 +180,33 @@
     """
     c = get_contract(code)
 
     assert c.foo([4, 5, 6]) == [4, 5, 6]
     assert c.foo() == [1, 2, 3]
 
 
-def test_default_param_clamp(get_contract, monkeypatch, tx_failed):
+def test_default_param_clamp(env, get_contract, tx_failed):
     code = """
 @external
 def bar(a: int128, b: int128 = -1) -> (int128, int128):  # noqa: E501
     return a, b
     """
 
     c = get_contract(code)
 
-    assert c.bar(-123) == [-123, -1]
-    assert c.bar(100, 100) == [100, 100]
+    assert c.bar(-123) == (-123, -1)
+    assert c.bar(100, 100) == (100, 100)
 
-    def validate_value(cls, value):
-        pass
+    method = method_id("bar(int128,int128)")
+    good_data = (200).to_bytes(32, "big") + (2**127 - 1).to_bytes(32, "big")
+    bad_data = (200).to_bytes(32, "big") + (2**127).to_bytes(32, "big")
 
-    monkeypatch.setattr("eth_abi.encoding.NumberEncoder.validate_value", validate_value)
-
-    assert c.bar(200, 2**127 - 1) == [200, 2**127 - 1]
+    assert env.message_call(c.address, data=method + good_data) == good_data
     with tx_failed():
-        c.bar(200, 2**127)
+        env.message_call(c.address, data=method + bad_data)
 
 
 def test_default_param_private(get_contract):
     code = """
 @internal
 def fooBar(a: Bytes[100], b: uint256, c: Bytes[20] = b"crazy") -> (Bytes[100], uint256, Bytes[20]):
     return a, b, c
@@ -222,19 +223,19 @@
     c: Bytes[20] = b""
     a, b, c = self.fooBar(b'here is my number', 555123456, b'baby')
     return a, b, c
     """
 
     c = get_contract(code)
 
-    # assert c.callMe() == [b'hello there', 123456, b'crazy']
-    assert c.callMeMaybe() == [b"here is my number", 555123456, b"baby"]
+    # assert c.callMe() == (b'hello there', 123456, b'crazy')
+    assert c.callMeMaybe() == (b"here is my number", 555123456, b"baby")
 
 
-def test_environment_vars_as_default(get_contract):
+def test_environment_vars_as_default(get_contract, env):
     code = """
 xx: uint256
 
 @external
 @payable
 def foo(a: uint256 = msg.value) -> bool:
     self.xx += a
@@ -245,19 +246,21 @@
     return self.xx
 
 @external
 def get_balance() -> uint256:
     return self.balance
     """
     c = get_contract(code)
-    c.foo(transact={"value": 31337})
+    env.set_balance(env.deployer, 31337 + 9001)
+    c.foo(value=31337)
     assert c.bar() == 31337
-    c.foo(666, transact={"value": 9001})
+    c.foo(666, value=9001)
     assert c.bar() == 31337 + 666
     assert c.get_balance() == 31337 + 9001
+    assert env.get_balance(env.deployer) == 0
 
 
 PASSING_CONTRACTS = [
     """
 @external
 def foo(a: bool = True, b: bool[2] = [True, False]): pass
     """,
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_erc20_abi.py` & `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_erc20_abi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from web3.exceptions import ValidationError
+from eth.codecs.abi.exceptions import EncodeError
 
 TOKEN_NAME = "Vypercoin"
 TOKEN_SYMBOL = "FANG"
 TOKEN_DECIMALS = 18
 TOKEN_INITIAL_SUPPLY = 21 * 10**6
 TOKEN_TOTAL_SUPPLY = TOKEN_INITIAL_SUPPLY * (10**TOKEN_DECIMALS)
 
@@ -68,51 +68,51 @@
 @external
 def allowance(_owner: address, _spender: address) -> uint256:
     return extcall self.token_address.allowance(_owner, _spender)
     """
     return get_contract(erc20_caller_code, *[erc20.address])
 
 
-def test_initial_state(w3, erc20_caller):
+def test_initial_state(env, erc20_caller):
     assert erc20_caller.totalSupply() == TOKEN_TOTAL_SUPPLY
-    assert erc20_caller.balanceOf(w3.eth.accounts[0]) == TOKEN_TOTAL_SUPPLY
-    assert erc20_caller.balanceOf(w3.eth.accounts[1]) == 0
+    assert erc20_caller.balanceOf(env.deployer) == TOKEN_TOTAL_SUPPLY
+    assert erc20_caller.balanceOf(env.accounts[1]) == 0
     assert erc20_caller.name() == TOKEN_NAME
     assert erc20_caller.symbol() == TOKEN_SYMBOL
     assert erc20_caller.decimals() == TOKEN_DECIMALS
 
 
-def test_call_transfer(w3, erc20, erc20_caller, tx_failed):
+def test_call_transfer(env, erc20, erc20_caller, tx_failed):
     # Basic transfer.
-    erc20.transfer(erc20_caller.address, 10, transact={})
+    erc20.transfer(erc20_caller.address, 10)
     assert erc20.balanceOf(erc20_caller.address) == 10
-    erc20_caller.transfer(w3.eth.accounts[1], 10, transact={})
+    erc20_caller.transfer(env.accounts[1], 10)
     assert erc20.balanceOf(erc20_caller.address) == 0
-    assert erc20.balanceOf(w3.eth.accounts[1]) == 10
+    assert erc20.balanceOf(env.accounts[1]) == 10
 
     # more than allowed
     with tx_failed():
-        erc20_caller.transfer(w3.eth.accounts[1], TOKEN_TOTAL_SUPPLY)
+        erc20_caller.transfer(env.accounts[1], TOKEN_TOTAL_SUPPLY)
 
     # Negative transfer value.
-    with tx_failed(ValidationError):
-        erc20_caller.transfer(w3.eth.accounts[1], -1)
+    with tx_failed(EncodeError):
+        erc20_caller.transfer(env.accounts[1], -1)
 
 
-def test_caller_approve_allowance(w3, erc20, erc20_caller):
+def test_caller_approve_allowance(env, erc20, erc20_caller):
     assert erc20_caller.allowance(erc20.address, erc20_caller.address) == 0
-    assert erc20.approve(erc20_caller.address, 10, transact={})
-    assert erc20_caller.allowance(w3.eth.accounts[0], erc20_caller.address) == 10
+    assert erc20.approve(erc20_caller.address, 10)
+    assert erc20_caller.allowance(env.deployer, erc20_caller.address) == 10
 
 
-def test_caller_tranfer_from(w3, erc20, erc20_caller, tx_failed):
+def test_caller_tranfer_from(env, erc20, erc20_caller, tx_failed):
     # Cannot transfer tokens that are unavailable
     with tx_failed():
-        erc20_caller.transferFrom(w3.eth.accounts[0], erc20_caller.address, 10)
+        erc20_caller.transferFrom(env.deployer, erc20_caller.address, 10)
     assert erc20.balanceOf(erc20_caller.address) == 0
-    assert erc20.approve(erc20_caller.address, 10, transact={})
-    erc20_caller.transferFrom(w3.eth.accounts[0], erc20_caller.address, 5, transact={})
+    assert erc20.approve(erc20_caller.address, 10)
+    erc20_caller.transferFrom(env.deployer, erc20_caller.address, 5)
     assert erc20.balanceOf(erc20_caller.address) == 5
-    assert erc20_caller.allowance(w3.eth.accounts[0], erc20_caller.address) == 5
-    erc20_caller.transferFrom(w3.eth.accounts[0], erc20_caller.address, 3, transact={})
+    assert erc20_caller.allowance(env.deployer, erc20_caller.address) == 5
+    erc20_caller.transferFrom(env.deployer, erc20_caller.address, 3)
     assert erc20.balanceOf(erc20_caller.address) == 8
-    assert erc20_caller.allowance(w3.eth.accounts[0], erc20_caller.address) == 2
+    assert erc20_caller.allowance(env.deployer, erc20_caller.address) == 2
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_external_contract_calls.py` & `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_external_contract_calls.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     StructureException,
     UndeclaredDefinition,
     UnknownType,
 )
 from vyper.utils import method_id
 
 
-def test_external_contract_calls(get_contract, get_contract_with_gas_estimation):
+def test_external_contract_calls(get_contract):
     contract_1 = """
 @external
 def foo(arg1: int128) -> int128:
     return arg1
     """
 
-    c = get_contract_with_gas_estimation(contract_1)
+    c = get_contract(contract_1)
 
     contract_2 = """
 interface Foo:
         def foo(arg1: int128) -> int128: view
 
 @external
 def bar(arg1: address, arg2: int128) -> int128:
@@ -33,15 +33,15 @@
     """
     c2 = get_contract(contract_2)
 
     assert c2.bar(c.address, 1) == 1
     print("Successfully executed an external contract call")
 
 
-def test_complicated_external_contract_calls(get_contract, get_contract_with_gas_estimation):
+def test_complicated_external_contract_calls(get_contract):
     contract_1 = """
 lucky: public(int128)
 
 @deploy
 def __init__(_lucky: int128):
     self.lucky = _lucky
 
@@ -51,29 +51,28 @@
 
 @external
 def array() -> Bytes[3]:
     return b'dog'
     """
 
     lucky_number = 7
-    c = get_contract_with_gas_estimation(contract_1, *[lucky_number])
+    c = get_contract(contract_1, *[lucky_number])
 
     contract_2 = """
 interface Foo:
     def foo() -> int128: nonpayable
     def array() -> Bytes[3]: view
 
 @external
 def bar(arg1: address) -> int128:
     return extcall Foo(arg1).foo()
     """
     c2 = get_contract(contract_2)
 
     assert c2.bar(c.address) == lucky_number
-    print("Successfully executed a complicated external contract call")
 
 
 @pytest.mark.parametrize("length", [3, 32, 33, 64])
 def test_external_contract_calls_with_bytes(get_contract, length):
     contract_1 = f"""
 @external
 def array() -> Bytes[{length}]:
@@ -164,16 +163,16 @@
     b: int128 = 0
     c: Bytes[{b}] = b""
     a, b, c = staticcall Foo(arg1).array()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.array() == [b"dog", 255, b"cat"]
-    assert c2.get_array(c.address) == [b"dog", 255, b"cat"]
+    assert c.array() == (b"dog", 255, b"cat")
+    assert c2.get_array(c.address) == (b"dog", 255, b"cat")
 
 
 @pytest.mark.parametrize("a,b", [(18, 7), (18, 18), (19, 6), (64, 6), (7, 19)])
 @pytest.mark.parametrize("c,d", [(19, 7), (64, 64)])
 def test_tuple_with_bytes_too_long(get_contract, tx_failed, a, c, b, d):
     contract_1 = f"""
 @external
@@ -193,15 +192,15 @@
     b: int128 = 0
     c: Bytes[{b}] = b""
     a, b, c = staticcall Foo(arg1).array()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.array() == [b"nineteen characters", 255, b"seven!!"]
+    assert c.array() == (b"nineteen characters", 255, b"seven!!")
     with tx_failed():
         c2.get_array(c.address)
 
 
 def test_tuple_with_bytes_too_long_two(get_contract, tx_failed):
     contract_1 = """
 @external
@@ -221,15 +220,15 @@
     b: int128 = 0
     c: Bytes[3] = b""
     a, b, c = staticcall Foo(arg1).array()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.array() == [b"nineteen characters", 255, b"seven!!"]
+    assert c.array() == (b"nineteen characters", 255, b"seven!!")
     with tx_failed():
         c2.get_array(c.address)
 
 
 @pytest.mark.parametrize("length", [8, 256])
 def test_external_contract_calls_with_uint8(get_contract, length):
     contract_1 = f"""
@@ -297,16 +296,16 @@
     b: Bytes[3] = b""
     c: uint{b} = 0
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [255, b"dog", 255]
-    assert c2.bar(c.address) == [255, b"dog", 255]
+    assert c.foo() == (255, b"dog", 255)
+    assert c2.bar(c.address) == (255, b"dog", 255)
 
 
 @pytest.mark.parametrize("a,b", [(8, 256), (256, 8), (256, 256)])
 def test_tuple_with_uint8_too_long(get_contract, tx_failed, a, b):
     contract_1 = f"""
 @external
 def foo() -> (uint{a}, Bytes[3], uint{b}):
@@ -325,15 +324,15 @@
     b: Bytes[3] = b""
     c: uint8 = 0
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [int(f"{(2**a)-1}"), b"dog", int(f"{(2**b)-1}")]
+    assert c.foo() == (int(f"{(2**a)-1}"), b"dog", int(f"{(2**b)-1}"))
     with tx_failed():
         c2.bar(c.address)
 
 
 @pytest.mark.parametrize("a,b", [(8, 256), (256, 8)])
 def test_tuple_with_uint8_too_long_two(get_contract, tx_failed, a, b):
     contract_1 = f"""
@@ -354,15 +353,15 @@
     b: Bytes[3] = b""
     c: uint{b} = 0
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [int(f"{(2**b)-1}"), b"dog", int(f"{(2**a)-1}")]
+    assert c.foo() == (int(f"{(2**b)-1}"), b"dog", int(f"{(2**a)-1}"))
     with tx_failed():
         c2.bar(c.address)
 
 
 @pytest.mark.parametrize("length", [128, 256])
 def test_external_contract_calls_with_int128(get_contract, length):
     contract_1 = f"""
@@ -430,16 +429,16 @@
     b: Bytes[3] = b""
     c: int{b} = 0
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [255, b"dog", 255]
-    assert c2.bar(c.address) == [255, b"dog", 255]
+    assert c.foo() == (255, b"dog", 255)
+    assert c2.bar(c.address) == (255, b"dog", 255)
 
 
 @pytest.mark.parametrize("a,b", [(128, 256), (256, 128), (256, 256)])
 def test_tuple_with_int128_too_long(get_contract, tx_failed, a, b):
     contract_1 = f"""
 @external
 def foo() -> (int{a}, Bytes[3], int{b}):
@@ -458,15 +457,15 @@
     b: Bytes[3] = b""
     c: int128 = 0
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [int(f"{(2**(a-1))-1}"), b"dog", int(f"{(2**(b-1))-1}")]
+    assert c.foo() == (int(f"{(2**(a-1))-1}"), b"dog", int(f"{(2**(b-1))-1}"))
     with tx_failed():
         c2.bar(c.address)
 
 
 @pytest.mark.parametrize("a,b", [(128, 256), (256, 128)])
 def test_tuple_with_int128_too_long_two(get_contract, tx_failed, a, b):
     contract_1 = f"""
@@ -487,15 +486,15 @@
     b: Bytes[3] = b""
     c: int{b} = 0
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [int(f"{(2**(b-1))-1}"), b"dog", int(f"{(2**(a-1))-1}")]
+    assert c.foo() == (int(f"{(2**(b-1))-1}"), b"dog", int(f"{(2**(a-1))-1}"))
     with tx_failed():
         c2.bar(c.address)
 
 
 @pytest.mark.parametrize("type", ["uint8", "uint256", "int128", "int256"])
 def test_external_contract_calls_with_decimal(get_contract, type):
     contract_1 = f"""
@@ -563,17 +562,17 @@
     b: Bytes[3] = b""
     c: decimal = 0.0
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
     """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [0, b"dog", 1]
+    assert c.foo() == (0, b"dog", 1)
     result = c2.bar(c.address)
-    assert result == [decimal_to_int("0.0"), b"dog", decimal_to_int("1e-10")]
+    assert result == (decimal_to_int("0.0"), b"dog", decimal_to_int("1e-10"))
 
 
 @pytest.mark.parametrize("a,b", [(8, 256), (256, 8), (256, 256)])
 def test_tuple_with_decimal_too_long(get_contract, tx_failed, a, b):
     contract_1 = f"""
 @external
 def foo() -> (uint{a}, Bytes[3], uint{b}):
@@ -592,15 +591,15 @@
     b: Bytes[3] = b""
     c: decimal = 0.0
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [2 ** (a - 1), b"dog", 2 ** (b - 1)]
+    assert c.foo() == (2 ** (a - 1), b"dog", 2 ** (b - 1))
     with tx_failed():
         c2.bar(c.address)
 
 
 @pytest.mark.parametrize("type", ["uint8", "uint256", "int128", "int256"])
 def test_external_contract_calls_with_bool(get_contract, type):
     contract_1 = f"""
@@ -668,16 +667,16 @@
     b: Bytes[3] = b""
     c: bool = False
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [1, b"dog", 0]
-    assert c2.bar(c.address) == [True, b"dog", False]
+    assert c.foo() == (1, b"dog", 0)
+    assert c2.bar(c.address) == (True, b"dog", False)
 
 
 @pytest.mark.parametrize("a", ["uint8", "uint256", "int128", "int256"])
 @pytest.mark.parametrize("b", ["uint8", "uint256", "int128", "int256"])
 def test_tuple_with_bool_too_long(get_contract, tx_failed, a, b):
     contract_1 = f"""
 @external
@@ -697,15 +696,15 @@
     b: Bytes[3] = b""
     c: bool = False
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [1, b"dog", 2]
+    assert c.foo() == (1, b"dog", 2)
     with tx_failed():
         c2.bar(c.address)
 
 
 @pytest.mark.parametrize("type", ["uint8", "int128", "uint256", "int256"])
 def test_external_contract_calls_with_address(get_contract, type):
     contract_1 = f"""
@@ -797,20 +796,20 @@
     b: Bytes[3] = b""
     c: address = empty(address)
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [16, b"dog", 1]
-    assert c2.bar(c.address) == [
+    assert c.foo() == (16, b"dog", 1)
+    assert c2.bar(c.address) == (
         "0x0000000000000000000000000000000000000010",
         b"dog",
         "0x0000000000000000000000000000000000000001",
-    ]
+    )
 
 
 @pytest.mark.parametrize("a", ["uint256", "int256"])
 @pytest.mark.parametrize("b", ["uint256", "int256"])
 def test_tuple_with_address_two(get_contract, a, b):
     contract_1 = f"""
 @external
@@ -830,15 +829,15 @@
     b: Bytes[3] = b""
     c: address = empty(address)
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [(2**160) - 1, b"dog", (2**160) - 2]
+    assert c.foo() == ((2**160) - 1, b"dog", (2**160) - 2)
     result = c2.bar(c.address)
     assert len(result) == 3
     assert result[0].lower() == "0xffffffffffffffffffffffffffffffffffffffff"
     assert result[1] == b"dog"
     assert result[2].lower() == "0xfffffffffffffffffffffffffffffffffffffffe"
 
 
@@ -863,15 +862,15 @@
     b: Bytes[3] = b""
     c: address = empty(address)
     a, b, c = staticcall Foo(arg1).foo()
     return a, b, c
 """
 
     c2 = get_contract(contract_2)
-    assert c.foo() == [(2**160) - 1, b"dog", 2**160]
+    assert c.foo() == ((2**160) - 1, b"dog", 2**160)
     with tx_failed():
         c2.bar(c.address)
 
 
 def test_external_contract_call_state_change(get_contract):
     contract_1 = """
 lucky: public(int128)
@@ -891,15 +890,15 @@
 @external
 def set_lucky(arg1: address, arg2: int128):
     extcall Foo(arg1).set_lucky(arg2)
     """
     c2 = get_contract(contract_2)
 
     assert c.lucky() == 0
-    c2.set_lucky(c.address, lucky_number, transact={})
+    c2.set_lucky(c.address, lucky_number)
     assert c.lucky() == lucky_number
     print("Successfully executed an external contract call state change")
 
 
 def test_constant_external_contract_call_cannot_change_state():
     c = """
 interface Foo:
@@ -957,16 +956,16 @@
 
 @external
 def set_lucky(arg1: address, arg2: int128):
     extcall Foo(arg1).set_lucky(arg2)
     """
     c3 = get_contract(contract_3)
 
-    c3.set_lucky(c.address, lucky_number_1, transact={})
-    c3.set_lucky(c2.address, lucky_number_2, transact={})
+    c3.set_lucky(c.address, lucky_number_1)
+    c3.set_lucky(c2.address, lucky_number_2)
     assert c.lucky() == lucky_number_1
     assert c2.lucky() == lucky_number_2
     print(
         "Successfully executed multiple external contract calls to different "
         "contracts based on address"
     )
 
@@ -1116,15 +1115,15 @@
     c2._stmt(c1.address)
     c2._stmt(c2.address)
 
     assert c2._expr(c1.address) == 1
     assert c2._expr(c2.address) == 1
 
 
-def test_invalid_nonexistent_contract_call(w3, tx_failed, get_contract):
+def test_invalid_nonexistent_contract_call(env, tx_failed, get_contract):
     contract_1 = """
 @external
 def bar() -> int128:
     return 1
     """
 
     contract_2 = """
@@ -1137,17 +1136,17 @@
     """
 
     c1 = get_contract(contract_1)
     c2 = get_contract(contract_2)
 
     assert c2.foo(c1.address) == 1
     with tx_failed():
-        c2.foo(w3.eth.accounts[0])
+        c2.foo(env.deployer)
     with tx_failed():
-        c2.foo(w3.eth.accounts[3])
+        c2.foo(env.accounts[3])
 
 
 def test_invalid_contract_reference_declaration(tx_failed, get_contract):
     contract = """
 interface Bar:
     get_magic_number: 1
 
@@ -1239,23 +1238,23 @@
     return staticcall self.bar_contract.get_lucky()
     """
 
     c1 = get_contract(contract_1)
     c2 = get_contract(contract_2)
     assert c1.get_lucky() == 0
     assert c2.get_lucky(c1.address) == 0
-    c1.set_lucky(6, transact={})
+    c1.set_lucky(6)
     assert c1.get_lucky() == 6
     assert c2.get_lucky(c1.address) == 6
-    c2.set_lucky(c1.address, transact={})
+    c2.set_lucky(c1.address)
     assert c1.get_lucky() == 1
     assert c2.get_lucky(c1.address) == 1
 
 
-def test_complex_external_contract_call_declaration(get_contract_with_gas_estimation):
+def test_complex_external_contract_call_declaration(get_contract):
     contract_1 = """
 @external
 def get_lucky() -> int128:
     return 1
 """
 
     contract_2 = """
@@ -1276,22 +1275,22 @@
     self.bar_contract = Bar(contract_address)
 
 @external
 def get_lucky() -> int128:
     return staticcall self.bar_contract.get_lucky()
 """
 
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
-    c3 = get_contract_with_gas_estimation(contract_3)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
+    c3 = get_contract(contract_3)
     assert c1.get_lucky() == 1
     assert c2.get_lucky() == 2
-    c3.set_contract(c1.address, transact={})
+    c3.set_contract(c1.address)
     assert c3.get_lucky() == 1
-    c3.set_contract(c2.address, transact={})
+    c3.set_contract(c2.address)
     assert c3.get_lucky() == 2
 
 
 def test_address_can_returned_from_contract_type(get_contract):
     contract_1 = """
 @external
 def bar() -> int128:
@@ -1309,15 +1308,15 @@
 
 @external
 def get_bar() -> int128:
     return staticcall self.bar_contract.bar()
 """
     c1 = get_contract(contract_1)
     c2 = get_contract(contract_2)
-    c2.foo(c1.address, transact={})
+    c2.foo(c1.address)
     assert c2.bar_contract() == c1.address
     assert c2.get_bar() == 1
 
 
 def test_invalid_external_contract_call_declaration_1(assert_compile_failed, get_contract):
     contract_1 = """
 interface Bar:
@@ -1348,15 +1347,15 @@
     return staticcall self.bar_contract.bar()
     """
 
     with pytest.raises(UnknownType):
         get_contract(contract_1)
 
 
-def test_external_with_payable_value(w3, get_contract_with_gas_estimation):
+def test_external_with_payable_value(env, get_contract):
     contract_1 = """
 @payable
 @external
 def get_lucky() -> int128:
     return 1
 
 @external
@@ -1379,42 +1378,42 @@
 def get_lucky(amount_to_send: uint256) -> int128:
     if amount_to_send != 0:
         return extcall self.bar_contract.get_lucky(value=amount_to_send)
     else: # send it all
         return extcall self.bar_contract.get_lucky(value=msg.value)
 """
 
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     # Set address.
     assert c1.get_lucky() == 1
     assert c1.get_balance() == 0
 
-    c2.set_contract(c1.address, transact={})
+    c2.set_contract(c1.address)
 
     # Send some eth
-    assert c2.get_lucky(0, call={"value": 500}) == 1
-    c2.get_lucky(0, transact={"value": 500})
+    env.set_balance(env.deployer, 10000)
+
+    assert c2.get_lucky(0, value=500) == 1
     # Contract 1 received money.
     assert c1.get_balance() == 500
-    assert w3.eth.get_balance(c1.address) == 500
-    assert w3.eth.get_balance(c2.address) == 0
+    assert env.get_balance(c1.address) == 500
+    assert env.get_balance(c2.address) == 0
 
     # Send subset of amount
-    assert c2.get_lucky(250, call={"value": 500}) == 1
-    c2.get_lucky(250, transact={"value": 500})
-
+    assert c2.get_lucky(250, value=500) == 1
     # Contract 1 received more money.
     assert c1.get_balance() == 750
-    assert w3.eth.get_balance(c1.address) == 750
-    assert w3.eth.get_balance(c2.address) == 250
+    assert env.get_balance(c1.address) == 750
+    assert env.get_balance(c2.address) == 250
+    assert env.get_balance(env.deployer) == 9000
 
 
-def test_external_call_with_gas(tx_failed, get_contract_with_gas_estimation):
+def test_external_call_with_gas(tx_failed, get_contract):
     contract_1 = """
 @external
 def get_lucky() -> int128:
     return 656598
 """
 
     contract_2 = """
@@ -1429,24 +1428,24 @@
     self.bar_contract = Bar(contract_address)
 
 @external
 def get_lucky(gas_amount: uint256) -> int128:
     return staticcall self.bar_contract.get_lucky(gas=gas_amount)
     """
 
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
-    c2.set_contract(c1.address, transact={})
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
+    c2.set_contract(c1.address)
 
     assert c2.get_lucky(1000) == 656598
     with tx_failed():
         c2.get_lucky(50)  # too little gas.
 
 
-def test_skip_contract_check(get_contract_with_gas_estimation):
+def test_skip_contract_check(get_contract):
     contract_2 = """
 @external
 @view
 def bar():
     pass
     """
     contract_1 = """
@@ -1461,45 +1460,45 @@
 @external
 def call_baz():
     # some address with no code
     addr: address = 0x1234567890AbcdEF1234567890aBcdef12345678
     # would fail if extcodesize check were on
     extcall Bar(addr).baz(skip_contract_check=True)
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
     c1.call_bar(c2.address)
     c1.call_baz()
 
 
-def test_invalid_keyword_on_call(assert_compile_failed, get_contract_with_gas_estimation):
+def test_invalid_keyword_on_call(assert_compile_failed, get_contract):
     contract_1 = """
 interface Bar:
     def set_lucky(arg1: int128): nonpayable
     def get_lucky() -> int128: view
 
 bar_contract: Bar
 
 @external
 def get_lucky(amount_to_send: int128) -> int128:
     return staticcall self.bar_contract.get_lucky(gass=1)
     """
 
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(contract_1), ArgumentException)
+    assert_compile_failed(lambda: get_contract(contract_1), ArgumentException)
 
 
-def test_invalid_contract_declaration(assert_compile_failed, get_contract_with_gas_estimation):
+def test_invalid_contract_declaration(assert_compile_failed, get_contract):
     contract_1 = """
 interface Bar:
     def set_lucky(arg1: int128): nonpayable
 
 bar_contract: Barr
     """
 
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(contract_1), UnknownType)
+    assert_compile_failed(lambda: get_contract(contract_1), UnknownType)
 
 
 FAILING_CONTRACTS_STRUCTURE_EXCEPTION = [
     """
 # wrong arg count
 interface Bar:
     def bar(arg1: int128) -> bool: view
@@ -1534,19 +1533,19 @@
 def foo(a: address, x: uint256, y: uint256):
     s: uint256 = staticcall Bar(a).bar(x, y=y)
     """,
 ]
 
 
 @pytest.mark.parametrize("bad_code", FAILING_CONTRACTS_STRUCTURE_EXCEPTION)
-def test_bad_code_struct_exc(assert_compile_failed, get_contract_with_gas_estimation, bad_code):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(bad_code), ArgumentException)
+def test_bad_code_struct_exc(assert_compile_failed, get_contract, bad_code):
+    assert_compile_failed(lambda: get_contract(bad_code), ArgumentException)
 
 
-def test_bad_skip_contract_check(assert_compile_failed, get_contract_with_gas_estimation):
+def test_bad_skip_contract_check(assert_compile_failed, get_contract):
     code = """
 # variable value for skip_contract_check
 interface Bar:
     def bar(): payable
 
 @external
 def foo():
@@ -1576,19 +1575,19 @@
     (a, b, c) = staticcall Test(addr).out_literals()
     return a, b,c
 
     """
     c1 = get_contract(contract_1)
     c2 = get_contract(contract_2)
 
-    assert c1.out_literals() == [1, "0x0000000000000000000000000000000000000123", b"random"]
-    assert c2.test(c1.address) == [1, "0x0000000000000000000000000000000000000123", b"random"]
+    assert c1.out_literals() == (1, "0x0000000000000000000000000000000000000123", b"random")
+    assert c2.test(c1.address) == (1, "0x0000000000000000000000000000000000000123", b"random")
 
 
-def test_struct_return_external_contract_call_1(get_contract_with_gas_estimation):
+def test_struct_return_external_contract_call_1(get_contract):
     contract_1 = """
 struct X:
     x: int128
     y: address
 @external
 def out_literals() -> X:
     return X(x=1, y=0x0000000000000000000000000000000000012345)
@@ -1603,23 +1602,23 @@
 
 @external
 def test(addr: address) -> (int128, address):
     ret: X = staticcall Test(addr).out_literals()
     return ret.x, ret.y
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.out_literals() == (1, "0x0000000000000000000000000000000000012345")
-    assert c2.test(c1.address) == list(c1.out_literals())
+    assert c2.test(c1.address) == c1.out_literals()
 
 
 @pytest.mark.parametrize("i,ln,s,", [(100, 6, "abcde"), (41, 40, "a" * 34), (57, 70, "z" * 68)])
-def test_struct_return_external_contract_call_2(get_contract_with_gas_estimation, i, ln, s):
+def test_struct_return_external_contract_call_2(get_contract, i, ln, s):
     contract_1 = f"""
 struct X:
     x: int128
     y: String[{ln}]
     z: Bytes[{ln}]
 @external
 def get_struct_x() -> X:
@@ -1636,22 +1635,22 @@
 
 @external
 def test(addr: address) -> (int128, String[{ln}], Bytes[{ln}]):
     ret: X = staticcall Test(addr).get_struct_x()
     return ret.x, ret.y, ret.z
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.get_struct_x() == (i, s, bytes(s, "utf-8"))
-    assert c2.test(c1.address) == list(c1.get_struct_x())
+    assert c2.test(c1.address) == c1.get_struct_x()
 
 
-def test_struct_return_external_contract_call_3(get_contract_with_gas_estimation):
+def test_struct_return_external_contract_call_3(get_contract):
     contract_1 = """
 struct X:
     x: int128
 @external
 def out_literals() -> X:
     return X(x=1)
     """
@@ -1664,22 +1663,22 @@
 
 @external
 def test(addr: address) -> int128:
     ret: X = staticcall Test(addr).out_literals()
     return ret.x
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.out_literals() == (1,)
     assert [c2.test(c1.address)] == list(c1.out_literals())
 
 
-def test_constant_struct_return_external_contract_call_1(get_contract_with_gas_estimation):
+def test_constant_struct_return_external_contract_call_1(get_contract):
     contract_1 = """
 struct X:
     x: int128
     y: address
 
 BAR: constant(X) = X(x=1, y=0x0000000000000000000000000000000000012345)
 
@@ -1697,25 +1696,23 @@
 
 @external
 def test(addr: address) -> (int128, address):
     ret: X = staticcall Test(addr).out_literals()
     return ret.x, ret.y
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.out_literals() == (1, "0x0000000000000000000000000000000000012345")
-    assert c2.test(c1.address) == list(c1.out_literals())
+    assert c2.test(c1.address) == c1.out_literals()
 
 
 @pytest.mark.parametrize("i,ln,s,", [(100, 6, "abcde"), (41, 40, "a" * 34), (57, 70, "z" * 68)])
-def test_constant_struct_return_external_contract_call_2(
-    get_contract_with_gas_estimation, i, ln, s
-):
+def test_constant_struct_return_external_contract_call_2(get_contract, i, ln, s):
     contract_1 = f"""
 struct X:
     x: int128
     y: String[{ln}]
     z: Bytes[{ln}]
 
 BAR: constant(X) = X(x={i}, y="{s}", z=b"{s}")
@@ -1735,22 +1732,22 @@
 
 @external
 def test(addr: address) -> (int128, String[{ln}], Bytes[{ln}]):
     ret: X = staticcall Test(addr).get_struct_x()
     return ret.x, ret.y, ret.z
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.get_struct_x() == (i, s, bytes(s, "utf-8"))
-    assert c2.test(c1.address) == list(c1.get_struct_x())
+    assert c2.test(c1.address) == c1.get_struct_x()
 
 
-def test_constant_struct_return_external_contract_call_3(get_contract_with_gas_estimation):
+def test_constant_struct_return_external_contract_call_3(get_contract):
     contract_1 = """
 struct X:
     x: int128
 
 BAR: constant(X) = X(x=1)
 
 @external
@@ -1766,22 +1763,22 @@
 
 @external
 def test(addr: address) -> int128:
     ret: X = staticcall Test(addr).out_literals()
     return ret.x
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.out_literals() == (1,)
     assert [c2.test(c1.address)] == list(c1.out_literals())
 
 
-def test_constant_struct_member_return_external_contract_call_1(get_contract_with_gas_estimation):
+def test_constant_struct_member_return_external_contract_call_1(get_contract):
     contract_1 = """
 struct X:
     x: int128
     y: address
 
 BAR: constant(X) = X(x=1, y=0x0000000000000000000000000000000000012345)
 
@@ -1795,25 +1792,23 @@
     def get_y() -> address: view
 
 @external
 def test(addr: address) -> address:
     ret: address = staticcall Test(addr).get_y()
     return ret
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.get_y() == "0x0000000000000000000000000000000000012345"
     assert c2.test(c1.address) == "0x0000000000000000000000000000000000012345"
 
 
 @pytest.mark.parametrize("i,ln,s,", [(100, 6, "abcde"), (41, 40, "a" * 34), (57, 70, "z" * 68)])
-def test_constant_struct_member_return_external_contract_call_2(
-    get_contract_with_gas_estimation, i, ln, s
-):
+def test_constant_struct_member_return_external_contract_call_2(get_contract, i, ln, s):
     contract_1 = f"""
 struct X:
     x: int128
     y: String[{ln}]
     z: Bytes[{ln}]
 
 BAR: constant(X) = X(x={i}, y="{s}", z=b"{s}")
@@ -1829,22 +1824,22 @@
 
 @external
 def test(addr: address) -> String[{ln}]:
     ret: String[{ln}] = staticcall Test(addr).get_y()
     return ret
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.get_y() == s
     assert c2.test(c1.address) == s
 
 
-def test_constant_struct_member_return_external_contract_call_3(get_contract_with_gas_estimation):
+def test_constant_struct_member_return_external_contract_call_3(get_contract):
     contract_1 = """
 struct X:
     x: int128
 
 BAR: constant(X) = X(x=1)
 
 @external
@@ -1858,22 +1853,22 @@
 
 @external
 def test(addr: address) -> int128:
     ret: int128 = staticcall Test(addr).get_x()
     return ret
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.get_x() == 1
     assert c2.test(c1.address) == 1
 
 
-def test_constant_nested_struct_return_external_contract_call_1(get_contract_with_gas_estimation):
+def test_constant_nested_struct_return_external_contract_call_1(get_contract):
     contract_1 = """
 struct X:
     x: int128
     y: address
 
 struct A:
     a: X
@@ -1899,25 +1894,23 @@
     def out_literals() -> A: view
 
 @external
 def test(addr: address) -> (X, uint256):
     ret: A = staticcall Test(addr).out_literals()
     return ret.a, ret.b
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.out_literals() == ((1, "0x0000000000000000000000000000000000012345"), 777)
-    assert c2.test(c1.address) == list(c1.out_literals())
+    assert c2.test(c1.address) == c1.out_literals()
 
 
 @pytest.mark.parametrize("i,ln,s,", [(100, 6, "abcde"), (41, 40, "a" * 34), (57, 70, "z" * 68)])
-def test_constant_nested_struct_return_external_contract_call_2(
-    get_contract_with_gas_estimation, i, ln, s
-):
+def test_constant_nested_struct_return_external_contract_call_2(get_contract, i, ln, s):
     contract_1 = f"""
 struct X:
     x: int128
     y: String[{ln}]
     z: Bytes[{ln}]
 
 struct A:
@@ -1946,22 +1939,22 @@
 
 @external
 def test(addr: address) -> (X, uint256):
     ret: A = staticcall Test(addr).get_struct_a()
     return ret.a, ret.b
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.get_struct_a() == ((i, s, bytes(s, "utf-8")), 777)
-    assert c2.test(c1.address) == list(c1.get_struct_a())
+    assert c2.test(c1.address) == c1.get_struct_a()
 
 
-def test_constant_nested_struct_return_external_contract_call_3(get_contract_with_gas_estimation):
+def test_constant_nested_struct_return_external_contract_call_3(get_contract):
     contract_1 = """
 struct X:
     x: int128
     y: int128
 
 struct A:
     a: X
@@ -1995,24 +1988,22 @@
     def out_literals() -> C : view
 
 @external
 def test(addr: address) -> (A, bool):
     ret: C = staticcall Test(addr).out_literals()
     return ret.c, ret.d
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
-    assert c1.out_literals() == (((1, -1), 777), True)
-    assert c2.test(c1.address) == list(c1.out_literals())
+    assert c1.out_literals() == ((((1, -1), 777)), True)
+    assert c2.test(c1.address) == c1.out_literals()
 
 
-def test_constant_nested_struct_member_return_external_contract_call_1(
-    get_contract_with_gas_estimation,
-):
+def test_constant_nested_struct_member_return_external_contract_call_1(get_contract):
     contract_1 = """
 struct X:
     x: int128
     y: address
 
 struct A:
     a: X
@@ -2030,25 +2021,23 @@
     def get_y() -> address: view
 
 @external
 def test(addr: address) -> address:
     ret: address = staticcall Test(addr).get_y()
     return ret
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.get_y() == "0x0000000000000000000000000000000000012345"
     assert c2.test(c1.address) == "0x0000000000000000000000000000000000012345"
 
 
 @pytest.mark.parametrize("i,ln,s,", [(100, 6, "abcde"), (41, 40, "a" * 34), (57, 70, "z" * 68)])
-def test_constant_nested_struct_member_return_external_contract_call_2(
-    get_contract_with_gas_estimation, i, ln, s
-):
+def test_constant_nested_struct_member_return_external_contract_call_2(get_contract, i, ln, s):
     contract_1 = f"""
 struct X:
     x: int128
     y: String[{ln}]
     z: Bytes[{ln}]
 
 struct A:
@@ -2069,24 +2058,22 @@
 
 @external
 def test(addr: address) -> String[{ln}]:
     ret: String[{ln}] = staticcall Test(addr).get_y()
     return ret
 
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.get_y() == s
     assert c2.test(c1.address) == s
 
 
-def test_constant_nested_struct_member_return_external_contract_call_3(
-    get_contract_with_gas_estimation,
-):
+def test_constant_nested_struct_member_return_external_contract_call_3(get_contract):
     contract_1 = """
 struct X:
     x: int128
     y: int128
 
 struct A:
     a: X
@@ -2118,25 +2105,25 @@
     return ret
 
 @external
 def test2(addr: address) -> uint256:
     ret: uint256 = staticcall Test(addr).get_b()
     return ret
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.get_y() == -1
     assert c2.test(c1.address) == -1
 
     assert c1.get_b() == 777
     assert c2.test2(c1.address) == 777
 
 
-def test_dynamically_sized_struct_external_contract_call(get_contract_with_gas_estimation):
+def test_dynamically_sized_struct_external_contract_call(get_contract):
     contract_1 = """
 struct X:
     x: uint256
     y: Bytes[6]
 
 @external
 def foo(x: X) -> Bytes[6]:
@@ -2153,22 +2140,22 @@
 
 @external
 def bar(addr: address) -> Bytes[6]:
     _X: X = X(x=1, y=b"hello")
     return extcall Foo(addr).foo(_X)
     """
 
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.foo((1, b"hello")) == b"hello"
     assert c2.bar(c1.address) == b"hello"
 
 
-def test_dynamically_sized_struct_external_contract_call_2(get_contract_with_gas_estimation):
+def test_dynamically_sized_struct_external_contract_call_2(get_contract):
     contract_1 = """
 struct X:
     x: uint256
     y: String[6]
 
 @external
 def foo(x: X) -> String[6]:
@@ -2185,22 +2172,22 @@
 
 @external
 def bar(addr: address) -> String[6]:
     _X: X = X(x=1, y="hello")
     return extcall Foo(addr).foo(_X)
     """
 
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.foo((1, "hello")) == "hello"
     assert c2.bar(c1.address) == "hello"
 
 
-def test_dynamically_sized_struct_member_external_contract_call(get_contract_with_gas_estimation):
+def test_dynamically_sized_struct_member_external_contract_call(get_contract):
     contract_1 = """
 @external
 def foo(b: Bytes[6]) -> Bytes[6]:
     return b
     """
 
     contract_2 = """
@@ -2213,22 +2200,22 @@
 
 @external
 def bar(addr: address) -> Bytes[6]:
     _X: X = X(x=1, y=b"hello")
     return extcall Foo(addr).foo(_X.y)
     """
 
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.foo(b"hello") == b"hello"
     assert c2.bar(c1.address) == b"hello"
 
 
-def test_dynamically_sized_struct_member_external_contract_call_2(get_contract_with_gas_estimation):
+def test_dynamically_sized_struct_member_external_contract_call_2(get_contract):
     contract_1 = """
 @external
 def foo(s: String[6]) -> String[6]:
     return s
     """
 
     contract_2 = """
@@ -2241,29 +2228,29 @@
 
 @external
 def bar(addr: address) -> String[6]:
     _X: X = X(x=1, y="hello")
     return extcall Foo(addr).foo(_X.y)
     """
 
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
     assert c1.foo("hello") == "hello"
     assert c2.bar(c1.address) == "hello"
 
 
-def test_list_external_contract_call(get_contract, get_contract_with_gas_estimation):
+def test_list_external_contract_call(get_contract):
     contract_1 = """
 @external
 def array() -> int128[3]:
     return [0, 0, 0]
     """
 
-    c = get_contract_with_gas_estimation(contract_1)
+    c = get_contract(contract_1)
 
     contract_2 = """
 interface Foo:
     def array() -> int128[3]: view
 @external
 def get_array(arg1: address) -> int128[3]:
     return staticcall Foo(arg1).array()
@@ -2492,51 +2479,51 @@
     assert c1.do_stuff(c2.address) == 1
 
 
 TEST_ADDR = b"".join(chr(i).encode("utf-8") for i in range(20)).hex()
 
 
 @pytest.mark.parametrize("typ,val", [("address", TEST_ADDR)])
-def test_calldata_clamp(w3, get_contract, tx_failed, typ, val):
+def test_calldata_clamp(env, get_contract, tx_failed, typ, val):
     code = f"""
 @external
 def foo(a: {typ}):
     pass
     """
     c1 = get_contract(code)
     sig = method_id(f"foo({typ})").hex()
     encoded = abi.encode(f"({typ})", (val,)).hex()
     data = f"0x{sig}{encoded}"
 
     # Static size is short by 1 byte
     malformed = data[:-2]
     with tx_failed():
-        w3.eth.send_transaction({"to": c1.address, "data": malformed})
+        env.message_call(c1.address, data=malformed)
 
     # Static size is exact
-    w3.eth.send_transaction({"to": c1.address, "data": data})
+    env.message_call(c1.address, data=data)
 
     # Static size exceeds by 1 byte, ok
-    w3.eth.send_transaction({"to": c1.address, "data": data + "ff"})
+    env.message_call(c1.address, data=data + "ff")
 
 
 @pytest.mark.parametrize("typ,val", [("address", ([TEST_ADDR] * 3, "vyper"))])
-def test_dynamic_calldata_clamp(w3, get_contract, tx_failed, typ, val):
+def test_dynamic_calldata_clamp(env, get_contract, tx_failed, typ, val):
     code = f"""
 @external
 def foo(a: DynArray[{typ}, 3], b: String[5]):
     pass
     """
 
     c1 = get_contract(code)
     sig = method_id(f"foo({typ}[],string)").hex()
     encoded = abi.encode(f"({typ}[],string)", val).hex()
     data = f"0x{sig}{encoded}"
 
     # Dynamic size is short by 1 byte
     malformed = data[:264]
     with tx_failed():
-        w3.eth.send_transaction({"to": c1.address, "data": malformed})
+        env.message_call(c1.address, data=malformed)
 
     # Dynamic size is at least minimum (132 bytes * 2 + 2 (for 0x) = 266)
     valid = data[:266]
-    w3.eth.send_transaction({"to": c1.address, "data": valid})
+    env.message_call(c1.address, data=valid)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py` & `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 @external
 def static_set_lucky(_lucky: int128):
     s: int128 = staticcall self.static_bar_contract.set_lucky(_lucky)
     """
 
     c1 = get_contract(contract_1)
     c2 = get_contract(contract_2, *[c1.address])
-    c2.modifiable_set_lucky(7, transact={})
+    c2.modifiable_set_lucky(7)
     assert c1.lucky() == 7
     # Fails attempting a state change after a call to a static address
     with tx_failed():
-        c2.static_set_lucky(5, transact={})
+        c2.static_set_lucky(5)
     assert c1.lucky() == 7
 
 
 def test_external_contract_call_declaration_stmt(get_contract, tx_failed):
     contract_1 = """
 lucky: public(int128)
 
@@ -81,19 +81,19 @@
 @external
 def static_set_lucky(_lucky: int128):
     x:int128 = staticcall self.static_bar_contract.set_lucky(_lucky)
     """
 
     c1 = get_contract(contract_1)
     c2 = get_contract(contract_2, *[c1.address])
-    c2.modifiable_set_lucky(7, transact={})
+    c2.modifiable_set_lucky(7)
     assert c1.lucky() == 7
     # Fails attempting a state change after a call to a static address
     with tx_failed():
-        c2.static_set_lucky(5, transact={})
+        c2.static_set_lucky(5)
     assert c1.lucky() == 7
 
 
 def test_multiple_contract_state_changes(get_contract, tx_failed):
     contract_1 = """
 lucky: public(int128)
 
@@ -162,22 +162,22 @@
     """
 
     c1 = get_contract(contract_1)
     c2 = get_contract(contract_2, *[c1.address])
     c3 = get_contract(contract_3, *[c2.address])
 
     assert c1.lucky() == 0
-    c3.modifiable_modifiable_set_lucky(7, transact={})
+    c3.modifiable_modifiable_set_lucky(7)
     assert c1.lucky() == 7
     with tx_failed():
-        c3.modifiable_static_set_lucky(6, transact={})
+        c3.modifiable_static_set_lucky(6)
     with tx_failed():
-        c3.static_modifiable_set_lucky(6, transact={})
+        c3.static_modifiable_set_lucky(6)
     with tx_failed():
-        c3.static_static_set_lucky(6, transact={})
+        c3.static_static_set_lucky(6)
     assert c1.lucky() == 7
 
 
 def test_address_can_returned_from_contract_type(get_contract):
     contract_1 = """
 @external
 def bar() -> int128:
@@ -195,15 +195,15 @@
 
 @external
 def get_bar() -> int128:
     return staticcall self.bar_contract.bar()
 """
     c1 = get_contract(contract_1)
     c2 = get_contract(contract_2)
-    c2.foo(c1.address, transact={})
+    c2.foo(c1.address)
     assert c2.bar_contract() == c1.address
     assert c2.get_bar() == 1
 
 
 def test_invalid_external_contract_call_declaration_1():
     contract_1 = """
 interface Bar:
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/calling_convention/test_return.py` & `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_return.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 import pytest
 
+from tests.utils import ZERO_ADDRESS
 from vyper import compile_code
 from vyper.exceptions import TypeMismatch
 
-pytestmark = pytest.mark.usefixtures("memory_mocker")
 
-
-def test_correct_abi_right_padding(tester, w3, get_contract_with_gas_estimation):
+def test_correct_abi_right_padding(env, get_contract):
     selfcall_code_6 = """
 @external
 def hardtest(arg1: Bytes[64], arg2: Bytes[64]) -> Bytes[128]:
     return concat(arg1, arg2)
     """
 
-    c = get_contract_with_gas_estimation(selfcall_code_6)
+    c = get_contract(selfcall_code_6)
 
     assert c.hardtest(b"hello" * 5, b"hello" * 10) == b"hello" * 15
 
-    # Make sure underlying structe is correctly right padded
-    classic_contract = c._classic_contract
-    func = classic_contract.functions.hardtest(b"hello" * 5, b"hello" * 10)
-    tx = func.build_transaction({"gasPrice": 0})
-    del tx["chainId"]
-    del tx["gasPrice"]
-
-    tx["from"] = w3.eth.accounts[0]
-    res = w3.to_bytes(hexstr=tester.call(tx))
-
+    res = env.message_call(
+        to=c.address, data=c.hardtest.prepare_calldata(b"hello" * 5, b"hello" * 10)
+    )
     static_offset = int.from_bytes(res[:32], "big")
     assert static_offset == 32
 
     dyn_section = res[static_offset:]
     assert len(dyn_section) % 32 == 0  # first right pad assert
 
     len_value = int.from_bytes(dyn_section[:32], "big")
 
     assert len_value == len(b"hello" * 15)
     assert dyn_section[32 : 32 + len_value] == b"hello" * 15
     # second right pad assert
     assert dyn_section[32 + len_value :] == b"\x00" * (len(dyn_section) - 32 - len_value)
 
 
-def test_return_type(get_contract_with_gas_estimation):
+def test_return_type(get_contract):
     long_string = 35 * "test"
 
     code = """
 struct Chunk:
     a: Bytes[8]
     b: Bytes[8]
     c: int128
@@ -86,47 +78,47 @@
     return self.chunk.a, self.chunk.c, self.chunk.b
 
 @external
 def out_very_long_bytes() -> (int128, Bytes[1024], int128, address):
     return 5555, b"testtesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttesttest", 6666, 0x0000000000000000000000000000000000001234  # noqa
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
-    assert c.out() == [3333, "0x0000000000000000000000000000000000000001"]
-    assert c.out_literals() == [1, None, b"random"]
-    assert c.out_bytes_first() == [b"test", 1234]
-    assert c.out_bytes_a(5555555, b"test") == [5555555, b"test"]
-    assert c.out_bytes_b(5555555, b"test") == [b"test", 5555555, b"test"]
-    assert c.four() == [1234, b"bytes", b"test", 4321]
-    assert c.out_chunk() == [b"hello", 5678, b"world"]
-    assert c.out_very_long_bytes() == [
+    assert c.out() == (3333, "0x0000000000000000000000000000000000000001")
+    assert c.out_literals() == (1, ZERO_ADDRESS, b"random")
+    assert c.out_bytes_first() == (b"test", 1234)
+    assert c.out_bytes_a(5555555, b"test") == (5555555, b"test")
+    assert c.out_bytes_b(5555555, b"test") == (b"test", 5555555, b"test")
+    assert c.four() == (1234, b"bytes", b"test", 4321)
+    assert c.out_chunk() == (b"hello", 5678, b"world")
+    assert c.out_very_long_bytes() == (
         5555,
         long_string.encode(),
         6666,
         "0x0000000000000000000000000000000000001234",
-    ]
+    )
 
 
-def test_return_type_signatures(get_contract_with_gas_estimation):
+def test_return_type_signatures(get_contract):
     code = """
 @external
 def out_literals() -> (int128, address, Bytes[6]):
     return 1, 0x0000000000000000000000000000000000000000, b"random"
     """
 
-    c = get_contract_with_gas_estimation(code)
-    assert c._classic_contract.abi[0]["outputs"] == [
+    c = get_contract(code)
+    assert c.abi[0]["outputs"] == [
         {"type": "int128", "name": ""},
         {"type": "address", "name": ""},
         {"type": "bytes", "name": ""},
     ]
 
 
-def test_return_tuple_assign(get_contract_with_gas_estimation):
+def test_return_tuple_assign(get_contract):
     code = """
 @internal
 def _out_literals() -> (int128, address, Bytes[10]):
     return 1, 0x0000000000000000000000000000000000000000, b"random"
 
 @external
 def out_literals() -> (int128, address, Bytes[10]):
@@ -137,20 +129,20 @@
     a: int128 = 0
     b: address = empty(address)
     c: Bytes[10] = b""
     (a, b, c) = self._out_literals()
     return a, b, c
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
-    assert c.out_literals() == c.test() == [1, None, b"random"]
+    assert c.out_literals() == c.test() == (1, ZERO_ADDRESS, b"random")
 
 
-def test_return_tuple_assign_storage(get_contract_with_gas_estimation):
+def test_return_tuple_assign_storage(get_contract):
     code = """
 a: int128
 b: address
 c: Bytes[20]
 d: Bytes[20]
 
 @internal
@@ -175,21 +167,21 @@
 @external
 def test3() -> (address, int128):
     x: address = empty(address)
     self.a, self.c, x, self.d = self._out_literals()
     return x, self.a
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     addr = "0x" + "00" * 19 + "23"
-    assert c.out_literals() == [1, b"testtesttest", addr, b"random"]
+    assert c.out_literals() == (1, b"testtesttest", addr, b"random")
     assert c.out_literals() == c.test1()
-    assert c.test2() == [1, c.out_literals()[2]]
-    assert c.test3() == [c.out_literals()[2], 1]
+    assert c.test2() == (1, c.out_literals()[2])
+    assert c.test3() == (c.out_literals()[2], 1)
 
 
 @pytest.mark.parametrize("string", ["a", "abc", "abcde", "potato"])
 def test_string_inside_tuple(get_contract, string):
     code = f"""
 @external
 def test_return() -> (String[6], uint256):
@@ -203,15 +195,15 @@
 
 @external
 def test_values(a: address) -> (String[6], uint256):
     return staticcall jsonabi(a).test_return()
     """
 
     c2 = get_contract(code)
-    assert c2.test_values(c1.address) == [string, 42]
+    assert c2.test_values(c1.address) == (string, 42)
 
 
 @pytest.mark.parametrize("string", ["a", "abc", "abcde", "potato"])
 def test_bytes_inside_tuple(get_contract, string):
     code = f"""
 @external
 def test_return() -> (Bytes[6], uint256):
@@ -225,28 +217,28 @@
 
 @external
 def test_values(a: address) -> (Bytes[6], uint256):
     return staticcall jsonabi(a).test_return()
     """
 
     c2 = get_contract(code)
-    assert c2.test_values(c1.address) == [bytes(string, "utf-8"), 42]
+    assert c2.test_values(c1.address) == (bytes(string, "utf-8"), 42)
 
 
-def test_tuple_return_typecheck(tx_failed, get_contract_with_gas_estimation):
+def test_tuple_return_typecheck(tx_failed, get_contract):
     code = """
 @external
 def getTimeAndBalance() -> (bool, address):
     return block.timestamp, self.balance
     """
     with pytest.raises(TypeMismatch):
         compile_code(code)
 
 
-def test_struct_return_abi(get_contract_with_gas_estimation):
+def test_struct_return_abi(get_contract):
     code = """
 struct Voter:
     weight: int128
     voted: bool
 
 @external
 def test() -> Voter:
@@ -255,20 +247,20 @@
     """
 
     out = compile_code(code, output_formats=["abi"])
     abi = out["abi"][0]
 
     assert abi["name"] == "test"
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.test() == (123, True)
 
 
-def test_single_struct_return_abi(get_contract_with_gas_estimation):
+def test_single_struct_return_abi(get_contract):
     code = """
 struct Voter:
     voted: bool
 
 @external
 def test() -> Voter:
     a: Voter = Voter(voted=True)
@@ -277,20 +269,20 @@
 
     out = compile_code(code, output_formats=["abi"])
     abi = out["abi"][0]
 
     assert abi["name"] == "test"
     assert abi["outputs"][0]["type"] == "tuple"
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.test() == (True,)
 
 
-def test_struct_return(get_contract_with_gas_estimation):
+def test_struct_return(get_contract):
     code = """
 struct Foo:
   x: int128
   y: uint256
 
 _foo: Foo
 _foos: HashMap[int128, Foo]
@@ -331,25 +323,25 @@
 @external
 def pub6() -> Foo:
     foo: Foo = Foo(x= 123, y=456)
     return self.return_arg(foo)
     """
     foo = (123, 456)
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.pub1() == (1, 2)
     assert c.pub2() == (3, 4)
     assert c.pub3() == (5, 6)
     assert c.pub4() == (7, 8)
     assert c.pub5(foo) == foo
     assert c.pub6() == foo
 
 
-def test_single_struct_return(get_contract_with_gas_estimation):
+def test_single_struct_return(get_contract):
     code = """
 struct Foo:
   x: int128
 
 _foo: Foo
 _foos: HashMap[int128, Foo]
 
@@ -388,15 +380,15 @@
 @external
 def pub6() -> Foo:
     foo: Foo = Foo(x=123)
     return self.return_arg(foo)
     """
     foo = (123,)
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.pub1() == (1,)
     assert c.pub2() == (3,)
     assert c.pub3() == (5,)
     assert c.pub4() == (7,)
     assert c.pub5(foo) == foo
     assert c.pub6() == foo
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_nonreentrant.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_nonreentrant.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,43 +161,43 @@
 @external
 def __default__():
     pass
     """
     contract = get_contract(protected_code)
     malicious = get_contract(malicious_code)
 
-    contract.set_callback(malicious.address, transact={})
+    contract.set_callback(malicious.address)
     assert contract.callback() == malicious.address
 
     # Test unprotected function.
-    contract.unprotected_function("some value", True, transact={})
+    contract.unprotected_function("some value", True)
     assert contract.special_value() == "surprise!"
 
     # Test protected function.
-    contract.protected_function("some value", False, transact={})
+    contract.protected_function("some value", False)
     assert contract.special_value() == "some value"
     assert contract.protected_view_fn() == "some value"
 
     with tx_failed():
-        contract.protected_function("zzz value", True, transact={})
+        contract.protected_function("zzz value", True)
 
-    contract.protected_function2("another value", False, transact={})
+    contract.protected_function2("another value", False)
     assert contract.special_value() == "another value"
 
     with tx_failed():
-        contract.protected_function2("zzz value", True, transact={})
+        contract.protected_function2("zzz value", True)
 
-    contract.protected_function3("another value", False, transact={})
+    contract.protected_function3("another value", False)
     assert contract.special_value() == "another value"
 
     with tx_failed():
-        contract.protected_function3("zzz value", True, transact={})
+        contract.protected_function3("zzz value", True)
 
 
-def test_nonreentrant_decorator_for_default(w3, get_contract, tx_failed):
+def test_nonreentrant_decorator_for_default(env, get_contract, tx_failed):
     calling_contract_code = """
 @external
 def send_funds(_amount: uint256):
     # raw_call() is used to overcome gas limit of send()
     response: Bytes[32] = raw_call(
         msg.sender,
         _abi_encode(msg.sender, _amount, method_id=method_id("transfer(address,uint256)")),
@@ -252,38 +252,39 @@
 def __default__():
     pass
     """
 
     reentrant_contract = get_contract(reentrant_code)
     calling_contract = get_contract(calling_contract_code)
 
-    reentrant_contract.set_callback(calling_contract.address, transact={})
+    reentrant_contract.set_callback(calling_contract.address)
     assert reentrant_contract.callback() == calling_contract.address
 
     # Test unprotected function without callback.
-    reentrant_contract.unprotected_function("some value", False, transact={"value": 1000})
+    env.set_balance(env.deployer, 10**6)
+    reentrant_contract.unprotected_function("some value", False, value=1000)
     assert reentrant_contract.special_value() == "some value"
-    assert w3.eth.get_balance(reentrant_contract.address) == 0
-    assert w3.eth.get_balance(calling_contract.address) == 1000
+    assert env.get_balance(reentrant_contract.address) == 0
+    assert env.get_balance(calling_contract.address) == 1000
 
     # Test unprotected function with callback to default.
-    reentrant_contract.unprotected_function("another value", True, transact={"value": 1000})
+    reentrant_contract.unprotected_function("another value", True, value=1000)
     assert reentrant_contract.special_value() == "another value"
-    assert w3.eth.get_balance(reentrant_contract.address) == 1000
-    assert w3.eth.get_balance(calling_contract.address) == 1000
+    assert env.get_balance(reentrant_contract.address) == 1000
+    assert env.get_balance(calling_contract.address) == 1000
 
     # Test protected function without callback.
-    reentrant_contract.protected_function("surprise!", False, transact={"value": 1000})
+    reentrant_contract.protected_function("surprise!", False, value=1000)
     assert reentrant_contract.special_value() == "surprise!"
-    assert w3.eth.get_balance(reentrant_contract.address) == 1000
-    assert w3.eth.get_balance(calling_contract.address) == 2000
+    assert env.get_balance(reentrant_contract.address) == 1000
+    assert env.get_balance(calling_contract.address) == 2000
 
     # Test protected function with callback to default.
     with tx_failed():
-        reentrant_contract.protected_function("zzz value", True, transact={"value": 1000})
+        reentrant_contract.protected_function("zzz value", True, value=1000)
 
 
 def test_disallow_on_init_function(get_contract):
     # nonreentrant has no effect when used on the __init__ fn
     # however, should disallow its usage regardless
     code = """
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_payable.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_payable.py`

 * *Files 14% similar despite different names*

```diff
@@ -176,21 +176,22 @@
 def baz() -> bool:
     return True
     """,
 ]
 
 
 @pytest.mark.parametrize("code", nonpayable_code)
-def test_nonpayable_runtime_assertion(w3, keccak, tx_failed, get_contract, code):
+def test_nonpayable_runtime_assertion(env, keccak, tx_failed, get_contract, code):
     c = get_contract(code)
+    env.set_balance(env.deployer, 10**18)
 
-    c.foo(transact={"value": 0})
+    c.foo(value=0)
     sig = keccak("foo()".encode()).hex()[:10]
     with tx_failed():
-        w3.eth.send_transaction({"to": c.address, "data": sig, "value": 10**18})
+        env.message_call(c.address, data=sig, value=10**18)
 
 
 payable_code = [
     """
 # single function, payable
 @payable
 @external
@@ -330,66 +331,68 @@
 def bar() -> bool:
     return True
     """,
 ]
 
 
 @pytest.mark.parametrize("code", payable_code)
-def test_payable_runtime_assertion(get_contract, code):
+def test_payable_runtime_assertion(env, get_contract, code):
     c = get_contract(code)
+    env.set_balance(env.deployer, 10**18)
+    c.foo(value=10**18)
+    c.foo(value=0)
 
-    c.foo(transact={"value": 10**18})
-    c.foo(transact={"value": 0})
 
-
-def test_payable_default_func_invalid_calldata(get_contract, w3):
+def test_payable_default_func_invalid_calldata(get_contract, env):
     code = """
 @external
 def foo() -> bool:
     return True
 
 @payable
 @external
 def __default__():
     pass
     """
-
     c = get_contract(code)
-    w3.eth.send_transaction({"to": c.address, "value": 100, "data": "0x12345678"})
+    env.set_balance(env.deployer, 100)
+    env.message_call(c.address, value=100, data="0x12345678")
 
 
-def test_nonpayable_default_func_invalid_calldata(get_contract, w3, tx_failed):
+def test_nonpayable_default_func_invalid_calldata(get_contract, env, tx_failed):
     code = """
 @external
 @payable
 def foo() -> bool:
     return True
 
 @external
 def __default__():
     pass
     """
 
     c = get_contract(code)
-    w3.eth.send_transaction({"to": c.address, "value": 0, "data": "0x12345678"})
+    env.message_call(c.address, value=0, data="0x12345678")
+    env.set_balance(env.deployer, 100)
     with tx_failed():
-        w3.eth.send_transaction({"to": c.address, "value": 100, "data": "0x12345678"})
+        env.message_call(c.address, value=100, data="0x12345678")
 
 
-def test_batch_nonpayable(get_contract, w3, tx_failed):
+def test_batch_nonpayable(get_contract, env, tx_failed):
     code = """
 @external
 def foo() -> bool:
     return True
 
 @external
 def __default__():
     pass
     """
 
     c = get_contract(code)
-    w3.eth.send_transaction({"to": c.address, "value": 0, "data": "0x12345678"})
+    env.message_call(c.address, value=0, data="0x12345678")
     data = bytes([1, 2, 3, 4])
     for i in range(5):
         calldata = "0x" + data[:i].hex()
+        env.set_balance(env.deployer, 100)
         with tx_failed():
-            w3.eth.send_transaction({"to": c.address, "value": 100, "data": calldata})
+            env.message_call(c.address, value=100, data=calldata)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_private.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_private.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import pytest
+from eth_utils import to_wei
 
 
-def test_private_test(get_contract_with_gas_estimation):
+def test_private_test(get_contract):
     private_test_code = """
 @internal
 def a() -> int128:
     return 5
 
 @external
 def returnten() -> int128:
     return self.a() * 2
     """
 
-    c = get_contract_with_gas_estimation(private_test_code)
+    c = get_contract(private_test_code)
     assert c.returnten() == 10
 
 
 def test_private_with_more_vars(get_contract):
     private_test_code = """
 @internal
 def afunc() -> int128:
@@ -37,15 +38,15 @@
     return a + b + c
     """
 
     c = get_contract(private_test_code)
     assert c.return_it() == 777
 
 
-def test_private_with_more_vars_nested(get_contract_with_gas_estimation):
+def test_private_with_more_vars_nested(get_contract):
     private_test_code = """
 @internal
 def more() -> int128:
     a: int128 = 50
     b: int128 = 50
     c: int128 = 11
     return a + b + c
@@ -63,19 +64,19 @@
     b: int128 = 111
     c: int128 = self.afunc()
     assert a == 222
     assert b == 111
     return a + b + c
     """
 
-    c = get_contract_with_gas_estimation(private_test_code)
+    c = get_contract(private_test_code)
     assert c.return_it() == 999
 
 
-def test_private_with_args(get_contract_with_gas_estimation):
+def test_private_with_args(get_contract):
     private_test_code = """
 @internal
 def add_times2(a: uint256, b: uint256) -> uint256:
     assert a == 100
     assert b == 11
     return 2 * (a + b)
 
@@ -83,19 +84,19 @@
 def return_it() -> uint256:
     a: uint256 = 111
     b: uint256 = 222
     c: uint256 = self.add_times2(100, 11)
     return a + b + c
     """
 
-    c = get_contract_with_gas_estimation(private_test_code)
+    c = get_contract(private_test_code)
     assert c.return_it() == 555
 
 
-def test_private_with_args_nested(get_contract_with_gas_estimation):
+def test_private_with_args_nested(get_contract):
     private_test_code = """
 @internal
 def multiply(a: uint256, b: uint256) -> uint256:
     c: uint256 = 7
     d: uint256 = 8
     e: uint256 = 9
     return a * b
@@ -108,19 +109,19 @@
 def return_it() -> uint256:
     a: uint256 = 111
     b: uint256 = 222
     c: uint256 = self.add_times2(0, a)
     return a + b + c
     """
 
-    c = get_contract_with_gas_estimation(private_test_code)
+    c = get_contract(private_test_code)
     assert c.return_it() == 666
 
 
-def test_private_bytes(get_contract_with_gas_estimation):
+def test_private_bytes(get_contract):
     private_test_code = """
 greeting: public(Bytes[100])
 
 @deploy
 def __init__():
     self.greeting = b"Hello "
 
@@ -130,20 +131,20 @@
 
 @external
 def hithere(name: Bytes[100]) -> Bytes[200]:
     d: Bytes[200] = self.construct(name)
     return d
     """
 
-    c = get_contract_with_gas_estimation(private_test_code)
+    c = get_contract(private_test_code)
     assert c.hithere(b"bob") == b"Hello bob"
     assert c.hithere(b"alice") == b"Hello alice"
 
 
-def test_private_statement(get_contract_with_gas_estimation):
+def test_private_statement(get_contract):
     private_test_code = """
 greeting: public(Bytes[20])
 
 @deploy
 def __init__():
     self.greeting = b"Hello "
 
@@ -171,22 +172,22 @@
 
 @external
 def hithere(name: Bytes[20]) -> Bytes[40]:
     d: Bytes[40] = self.construct(name)
     return d
     """
 
-    c = get_contract_with_gas_estimation(private_test_code)
+    c = get_contract(private_test_code)
     assert c.greeting() == b"Hello "
     assert c.hithere(b"Bob") == b"Hello Bob"
-    c.iprefer(b"Hi there, ", transact={})
+    c.iprefer(b"Hi there, ")
     assert c.hithere(b"Alice") == b"Hi there, Alice"
 
 
-def test_private_default_parameter(get_contract_with_gas_estimation):
+def test_private_default_parameter(get_contract):
     private_test_code = """
 @internal
 def addition(a: uint256, b: uint256 = 1) -> uint256:
     return a + b
 
 
 @external
@@ -202,21 +203,21 @@
     assert c == 333
     assert a_before == a
     assert b_before == b
 
     return d
     """
 
-    c = get_contract_with_gas_estimation(private_test_code)
+    c = get_contract(private_test_code)
 
     assert c.add_one(20) == 21
     assert c.added(10, 20) == 30
 
 
-def test_private_return_bytes(get_contract_with_gas_estimation):
+def test_private_return_bytes(get_contract):
     code = """
 a_message: Bytes[50]
 
 @internal
 def _test() -> (Bytes[100]):
     b: Bytes[50] = b"hello                   1           2"
     return b
@@ -255,24 +256,24 @@
 
 @external
 def test4() -> (Bytes[100]):
     d: Bytes[100] = b'xyzxyzxyzxyz'
     return self.get_msg()
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     test_str = b"                   1           2"
     assert c.test() == b"hello" + test_str
     assert c.test2() == b"hello" + test_str
     assert c.test3(b"alice") == b"alice"
-    c.set(b"hello daar", transact={})
+    c.set(b"hello daar")
     assert c.test4() == b"hello daar"
 
 
-def test_private_bytes_as_args(get_contract_with_gas_estimation):
+def test_private_bytes_as_args(get_contract):
     code = """
 @internal
 def _test(a: Bytes[40]) -> (Bytes[100]):
     b: Bytes[40] = b"hello "
     return concat(b, a)
 
 @external
@@ -283,20 +284,20 @@
 
 @external
 def test2() -> Bytes[100]:
     c: Bytes[10] = b"alice"
     return self._test(c)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.test(b"bob") == b"hello bob, jack attack"
     assert c.test2() == b"hello alice"
 
 
-def test_private_return_tuple_base_types(get_contract_with_gas_estimation):
+def test_private_return_tuple_base_types(get_contract):
     code = """
 @internal
 def _test(a: bytes32) -> (bytes32, uint256, int128):
     b: uint256 = 1000
     return a, b, -1200
 
 @external
@@ -310,21 +311,21 @@
     return f, b, c
 
 @external
 def test2(a: bytes32) -> (bytes32, uint256, int128):
     return self._test(a)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
-    assert c.test(b"test" + b"\x00" * 28) == [b"test" + 28 * b"\x00", 1000, -1200]
-    assert c.test2(b"test" + b"\x00" * 28) == [b"test" + 28 * b"\x00", 1000, -1200]
+    assert c.test(b"test" + b"\x00" * 28) == (b"test" + 28 * b"\x00", 1000, -1200)
+    assert c.test2(b"test" + b"\x00" * 28) == (b"test" + 28 * b"\x00", 1000, -1200)
 
 
-def test_private_return_tuple_bytes(get_contract_with_gas_estimation):
+def test_private_return_tuple_bytes(get_contract):
     code = """
 @internal
 def _test(a: int128, b: Bytes[50]) -> (int128, Bytes[100]):
     return a + 2, concat(b"badabing:", b)
 
 @internal
 def _test_combined(a: Bytes[50], x: int128, c:Bytes[50]) -> (int128, Bytes[100], Bytes[100]):
@@ -357,43 +358,43 @@
 
 @external
 def test4(a: Bytes[40]) -> (int128, Bytes[100], Bytes[100]):
     b: Bytes[50] = concat(a, b"_one")
     return self._test_combined(a, 8, b)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
-    assert c.test(11, b"jill") == [14, b"badabing:jill_one", b"jill_one"]
-    assert c.test2(b"jack") == [6, b"badabing:jack_one"]
-    assert c.test3(b"hill") == [10, b"hill", b"hill_two"]
-    assert c.test4(b"bucket") == [10, b"bucket", b"bucket_one_two"]
+    assert c.test(11, b"jill") == (14, b"badabing:jill_one", b"jill_one")
+    assert c.test2(b"jack") == (6, b"badabing:jack_one")
+    assert c.test3(b"hill") == (10, b"hill", b"hill_two")
+    assert c.test4(b"bucket") == (10, b"bucket", b"bucket_one_two")
 
 
-def test_private_return_list_types(get_contract_with_gas_estimation):
+def test_private_return_list_types(get_contract):
     code = """
 @internal
 def _test(b: int128[4]) -> int128[4]:
     assert b[1] == 2
     assert b[2] == 3
     assert b[3] == 4
     return [0, 1, 0, 1]
 
 @external
 def test() -> int128[4]:
     b: int128[4] = [1, 2, 3, 4]
     c: int128[2] = [11, 22]
     return self._test(b)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.test() == [0, 1, 0, 1]
 
 
-def test_private_payable(w3, get_contract_with_gas_estimation):
+def test_private_payable(env, get_contract):
     code = """
 @internal
 def _send_it(a: address, _value: uint256):
     send(a, _value)
 
 @payable
 @external
@@ -402,26 +403,26 @@
 
 @external
 @payable
 def __default__():
     pass
     """
 
-    c = get_contract_with_gas_estimation(code)
-
-    w3.eth.send_transaction({"to": c.address, "value": w3.to_wei(1, "ether")})
-    assert w3.eth.get_balance(c.address) == w3.to_wei(1, "ether")
-    a3 = w3.eth.accounts[2]
-    assert w3.eth.get_balance(a3) == w3.to_wei(1000000, "ether")
-    c.test(True, a3, w3.to_wei(0.05, "ether"), transact={})
-    assert w3.eth.get_balance(a3) == w3.to_wei(1000000.05, "ether")
-    assert w3.eth.get_balance(c.address) == w3.to_wei(0.95, "ether")
+    c = get_contract(code)
+    env.set_balance(env.deployer, to_wei(1, "ether"))
+    env.message_call(c.address, value=to_wei(1, "ether"))
+    assert env.get_balance(c.address) == to_wei(1, "ether")
+    a3 = env.accounts[2]
+    env.set_balance(a3, to_wei(1000000, "ether"))
+    c.test(True, a3, to_wei(0.05, "ether"))
+    assert env.get_balance(a3) == to_wei(1000000.05, "ether")
+    assert env.get_balance(c.address) == to_wei(0.95, "ether")
 
 
-def test_private_msg_sender(get_contract, w3):
+def test_private_msg_sender(get_contract, env, get_logs):
     code = """
 event Addr:
     addr: address
 
 @internal
 @view
 def _whoami() -> address:
@@ -438,19 +439,18 @@
     log Addr(self._whoami())
     return self._whoami()
     """
 
     c = get_contract(code)
     assert c.i_am_me()
 
-    addr = w3.eth.accounts[1]
-    txhash = c.whoami(transact={"from": addr})
-    receipt = w3.eth.wait_for_transaction_receipt(txhash)
-    logged_addr = w3.to_checksum_address(receipt.logs[0].data[-20:])
-    assert logged_addr == addr, "oh no"
+    addr = env.accounts[1]
+    c.whoami(sender=addr)
+    (log,) = get_logs(c)
+    assert log.args.addr == addr
 
 
 def test_nested_static_params_only(get_contract, tx_failed):
     code1 = """
 @internal
 @view
 def c() -> bool:
@@ -533,15 +533,15 @@
     if True:
         self.foo()
     """
 
     c = get_contract(code)
 
     assert c.test() is False
-    c.start(transact={})
+    c.start()
     assert c.test() is True
 
 
 def test_private_array_param(get_contract):
     code = """
 @internal
 def change_arr(arr: int128[2]):
@@ -581,15 +581,15 @@
 
 
 @external
 def foo(a: int128) -> (int128, int128):
     return self._test(a)
     """,
         (11,),
-        [13, 2],
+        (13, 2),
     ),
     (
         """
 struct A:
     one: uint8
 
 @internal
@@ -632,54 +632,54 @@
 
 @external
 def foo() -> (uint256[4], uint256):
     out: A = self._foo([1, 2, 3, 4], 5)
     return out.many, out.one
     """,
         (),
-        [[1, 2, 3, 4], 5],
+        ([1, 2, 3, 4], 5),
     ),
     (
         """
 @internal
 def _foo() -> (uint256[2], uint256[2]):
     return [1, 2], [5, 6]
 
 @external
 def foo() -> (uint256[2], uint256[2], uint256[2]):
     return self._foo()[0], [3, 4], self._foo()[1]
     """,
         (),
-        [[1, 2], [3, 4], [5, 6]],
+        ([1, 2], [3, 4], [5, 6]),
     ),
     (
         """
 @internal
 def _foo(a: int128, b: int128[3], c: int128[3]) -> (int128[3], int128, int128[3]):
     return c, 4, [b[1], a, b[0]]
 
 @external
 def foo(a: int128, b: int128[3], c: int128[3]) -> (int128[3], int128, int128[3]):
     return self._foo(a, b, c)
     """,
         (6, [7, 5, 8], [1, 2, 3]),
-        [[1, 2, 3], 4, [5, 6, 7]],
+        ([1, 2, 3], 4, [5, 6, 7]),
     ),
     (
         """
 @internal
 def _foo(a: int128, b: int128[3], c: int128[3]) -> (int128[3], int128, int128[3]):
     return c, 4, [b[1], a, b[0]]
 
 @external
 def foo(a: int128, b: int128[3], c: int128[3]) -> (int128[3], int128, int128[3]):
     return c, 4, self._foo(a, b, c)[2]
     """,
         (6, [7, 5, 8], [1, 2, 3]),
-        [[1, 2, 3], 4, [5, 6, 7]],
+        ([1, 2, 3], 4, [5, 6, 7]),
     ),
 ]
 
 
 @pytest.mark.parametrize("source_code,args,expected", tuple_return_sources)
 def test_tuple_return_types(get_contract, source_code, args, expected):
     c = get_contract(source_code)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_pure.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_pure.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/decorators/test_view.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/decorators/test_view.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 
 from vyper.exceptions import FunctionDeclarationException
 
 
-def test_constant_test(get_contract_with_gas_estimation_for_constants):
+def test_constant_test(get_contract):
     constant_test = """
 @external
 @view
 def foo() -> int128:
     return 5
     """
 
-    c = get_contract_with_gas_estimation_for_constants(constant_test)
+    c = get_contract(constant_test)
     assert c.foo() == 5
 
     print("Passed constant function test")
 
 
 @pytest.mark.requires_evm_version("cancun")
 def test_transient_test(get_contract):
@@ -27,20 +27,16 @@
 def foo() -> uint256:
     return self.x
     """
     c = get_contract(code)
     assert c.foo() == 0
 
 
-def test_invalid_constant_and_payable(
-    get_contract_with_gas_estimation_for_constants, assert_compile_failed
-):
+def test_invalid_constant_and_payable(get_contract, assert_compile_failed):
     code = """
 @external
 @payable
 @view
 def foo() -> num:
     return 5
 """
-    assert_compile_failed(
-        lambda: get_contract_with_gas_estimation_for_constants(code), FunctionDeclarationException
-    )
+    assert_compile_failed(lambda: get_contract(code), FunctionDeclarationException)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_break.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_break.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import pytest
 
 from tests.utils import decimal_to_int
 from vyper.exceptions import StructureException
 
 
-def test_break_test(get_contract_with_gas_estimation):
+def test_break_test(get_contract):
     break_test = """
 @external
 def foo(n: decimal) -> int128:
     c: decimal = n * 1.0
     output: int128 = 0
     for i: int128 in range(400):
         c = c / 1.2589
         if c < 1.0:
             output = i
             break
     return output
     """
 
-    c = get_contract_with_gas_estimation(break_test)
+    c = get_contract(break_test)
 
     assert c.foo(decimal_to_int("1")) == 0
     assert c.foo(decimal_to_int("2")) == 3
     assert c.foo(decimal_to_int("10")) == 10
     assert c.foo(decimal_to_int("200")) == 23
 
     print("Passed for-loop break test")
 
 
-def test_break_test_2(get_contract_with_gas_estimation):
+def test_break_test_2(get_contract):
     break_test_2 = """
 @external
 def foo(n: decimal) -> int128:
     c: decimal = n * 1.0
     output: int128 = 0
     for i: int128 in range(40):
         if c < 10.0:
@@ -43,24 +43,24 @@
         c = c / 1.2589
         if c < 1.0:
             output = output + i
             break
     return output
     """
 
-    c = get_contract_with_gas_estimation(break_test_2)
+    c = get_contract(break_test_2)
     assert c.foo(decimal_to_int("1")) == 0
     assert c.foo(decimal_to_int("2")) == 3
     assert c.foo(decimal_to_int("10")) == 10
     assert c.foo(decimal_to_int("200")) == 23
     assert c.foo(decimal_to_int("4000000")) == 66
     print("Passed for-loop break test 2")
 
 
-def test_break_test_3(get_contract_with_gas_estimation):
+def test_break_test_3(get_contract):
     break_test_3 = """
 @external
 def foo(n: int128) -> int128:
     c: decimal = convert(n, decimal)
     output: int128 = 0
     for i: int128 in range(40):
         if c < 10.0:
@@ -71,15 +71,15 @@
         c /= 1.2589
         if c < 1.0:
             output = output + i
             break
     return output
     """
 
-    c = get_contract_with_gas_estimation(break_test_3)
+    c = get_contract(break_test_3)
     assert c.foo(1) == 0
     assert c.foo(2) == 3
     assert c.foo(10) == 10
     assert c.foo(200) == 23
     assert c.foo(4000000) == 66
     print("Passed aug-assignment break composite test")
 
@@ -114,9 +114,9 @@
     """,
         StructureException,
     ),
 ]
 
 
 @pytest.mark.parametrize("bad_code,exc", fail_list)
-def test_block_fail(assert_compile_failed, get_contract_with_gas_estimation, bad_code, exc):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(bad_code), exc)
+def test_block_fail(assert_compile_failed, get_contract, bad_code, exc):
+    assert_compile_failed(lambda: get_contract(bad_code), exc)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_continue.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_continue.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 import pytest
 
 from vyper.exceptions import StructureException
 
 
-def test_continue1(get_contract_with_gas_estimation):
+def test_continue1(get_contract):
     code = """
 @external
 def foo() -> bool:
     for i: uint256 in range(2):
         continue
         return False
     return True
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo()
 
 
-def test_continue2(get_contract_with_gas_estimation):
+def test_continue2(get_contract):
     code = """
 @external
 def foo() -> int128:
     x: int128 = 0
     for i: int128 in range(3):
         x += 1
         continue
         x -= 1
     return x
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == 3
 
 
-def test_continue3(get_contract_with_gas_estimation):
+def test_continue3(get_contract):
     code = """
 @external
 def foo() -> int128:
     x: int128 = 0
     for i: int128 in range(3):
         x += i
         continue
     return x
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == 3
 
 
-def test_continue4(get_contract_with_gas_estimation):
+def test_continue4(get_contract):
     code = """
 @external
 def foo() -> int128:
     x: int128 = 0
     for i: int128 in range(6):
         if i % 2 == 0:
             continue
         x += 1
     return x
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() == 3
 
 
 fail_list = [
     (
         """
 @external
@@ -90,9 +90,9 @@
     """,
         StructureException,
     ),
 ]
 
 
 @pytest.mark.parametrize("bad_code,exc", fail_list)
-def test_block_fail(assert_compile_failed, get_contract_with_gas_estimation, bad_code, exc):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(bad_code), exc)
+def test_block_fail(assert_compile_failed, get_contract, bad_code, exc):
+    assert_compile_failed(lambda: get_contract(bad_code), exc)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_for_in_list.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_for_in_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
 @pytest.mark.parametrize("code, data", BASIC_FOR_LOOP_CODE)
 def test_basic_for_in_lists(code, data, get_contract):
     c = get_contract(code)
     assert c.data() == data
 
 
-def test_basic_for_list_storage(get_contract_with_gas_estimation):
+def test_basic_for_list_storage(get_contract):
     code = """
 x: int128[4]
 
 @external
 def set():
     self.x = [3, 5, 7, 9]
 
@@ -178,22 +178,22 @@
 def data() -> int128:
     for i: int128 in self.x:
         if i > 5:
             return i
     return -1
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.data() == -1
-    c.set(transact={})
+    c.set()
     assert c.data() == 7
 
 
-def test_basic_for_dyn_array_storage(get_contract_with_gas_estimation):
+def test_basic_for_dyn_array_storage(get_contract):
     code = """
 x: DynArray[int128, 4]
 
 @external
 def set(xs: DynArray[int128, 4]):
     self.x = xs
 
@@ -201,24 +201,24 @@
 def data() -> int128:
     t: int128 = 0
     for i: int128 in self.x:
         t += i
     return t
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.data() == 0
     # test all sorts of lists
     for xs in [[3, 5, 7, 9], [4, 6, 8], [1, 2], [5], []]:
-        c.set(xs, transact={})
+        c.set(xs)
         assert c.data() == sum(xs)
 
 
-def test_basic_for_list_storage_address(get_contract_with_gas_estimation):
+def test_basic_for_list_storage_address(get_contract):
     code = """
 addresses: address[3]
 
 @external
 def set(i: int128, val: address):
     self.addresses[i] = val
 
@@ -232,24 +232,24 @@
     for i: address in self.addresses:
         count += 1
         if count == 2:
             return i
     return empty(address)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
-    c.set(0, "0x82A978B3f5962A5b0957d9ee9eEf472EE55B42F1", transact={})
-    c.set(1, "0x7d577a597B2742b498Cb5Cf0C26cDCD726d39E6e", transact={})
-    c.set(2, "0xDCEceAF3fc5C0a63d195d69b1A90011B7B19650D", transact={})
+    c.set(0, "0x82A978B3f5962A5b0957d9ee9eEf472EE55B42F1")
+    c.set(1, "0x7d577a597B2742b498Cb5Cf0C26cDCD726d39E6e")
+    c.set(2, "0xDCEceAF3fc5C0a63d195d69b1A90011B7B19650D")
 
     assert c.ret(1) == c.iterate_return_second() == "0x7d577a597B2742b498Cb5Cf0C26cDCD726d39E6e"
 
 
-def test_basic_for_list_storage_decimal(get_contract_with_gas_estimation):
+def test_basic_for_list_storage_decimal(get_contract):
     code = """
 readings: decimal[3]
 
 @external
 def set(i: int128, val: decimal):
     self.readings[i] = val
 
@@ -263,59 +263,59 @@
     for i: decimal in self.readings:
         if count == break_count:
             return i
         count += 1
     return -1.111
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
-    c.set(0, decimal_to_int("0.0001"), transact={})
-    c.set(1, decimal_to_int("1.1"), transact={})
-    c.set(2, decimal_to_int("2.2"), transact={})
+    c.set(0, decimal_to_int("0.0001"))
+    c.set(1, decimal_to_int("1.1"))
+    c.set(2, decimal_to_int("2.2"))
 
     assert c.ret(2) == c.i_return(2) == decimal_to_int("2.2")
     assert c.ret(1) == c.i_return(1) == decimal_to_int("1.1")
     assert c.ret(0) == c.i_return(0) == decimal_to_int("0.0001")
 
 
-def test_for_in_list_iter_type(get_contract_with_gas_estimation):
+def test_for_in_list_iter_type(get_contract):
     code = """
 @external
 @view
 def func(amounts: uint256[3]) -> uint256:
     total: uint256 = as_wei_value(0, "wei")
 
     # calculate total
     for amount: uint256 in amounts:
         total += amount
 
     return total
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.func([100, 200, 300]) == 600
 
 
-def test_for_in_dyn_array(get_contract_with_gas_estimation):
+def test_for_in_dyn_array(get_contract):
     code = """
 @external
 @view
 def func(amounts: DynArray[uint256, 3]) -> uint256:
     total: uint256 = 0
 
     # calculate total
     for amount: uint256 in amounts:
         total += amount
 
     return total
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.func([100, 200, 300]) == 600
     assert c.func([100, 200]) == 300
 
 
 GOOD_CODE = [
     # multiple for loops
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/iteration/test_for_range.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/iteration/test_for_range.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import pytest
 
+from vyper.exceptions import StaticAssertionException
+from vyper.utils import SizeLimits
 
-def test_basic_repeater(get_contract_with_gas_estimation):
+
+def test_basic_repeater(get_contract):
     basic_repeater = """
 @external
 def repeat(z: int128) -> int128:
     x: int128 = 0
     for i: int128 in range(6):
         x = x + z
     return(x)
     """
-    c = get_contract_with_gas_estimation(basic_repeater)
+    c = get_contract(basic_repeater)
     assert c.repeat(9) == 54
 
 
 def test_range_bound(get_contract, tx_failed):
     code = """
 @external
 def repeat(n: uint256) -> uint256:
@@ -124,15 +127,15 @@
     for n in range(1, 7):
         with tx_failed():
             c.get_last(UINT_MAX - n, 0)
         with tx_failed():
             c.get_last(UINT_MAX, UINT_MAX - n)
 
 
-def test_digit_reverser(get_contract_with_gas_estimation):
+def test_digit_reverser(get_contract):
     digit_reverser = """
 @external
 def reverse_digits(x: int128) -> int128:
     dig: int128[6] = [0, 0, 0, 0, 0, 0]
     z: int128 = x
     for i: uint256 in range(6):
         dig[i] = z % 10
@@ -140,81 +143,81 @@
     o: int128 = 0
     for i: uint256 in range(6):
         o = o * 10 + dig[i]
     return o
 
     """
 
-    c = get_contract_with_gas_estimation(digit_reverser)
+    c = get_contract(digit_reverser)
     assert c.reverse_digits(123456) == 654321
 
 
-def test_more_complex_repeater(get_contract_with_gas_estimation):
+def test_more_complex_repeater(get_contract):
     more_complex_repeater = """
 @external
 def repeat() -> int128:
     out: int128 = 0
     for i: uint256 in range(6):
         out = out * 10
         for j: int128 in range(4):
             out = out + j
     return(out)
     """
 
-    c = get_contract_with_gas_estimation(more_complex_repeater)
+    c = get_contract(more_complex_repeater)
     assert c.repeat() == 666666
 
 
 @pytest.mark.parametrize("typ", ["int128", "uint256"])
-def test_offset_repeater(get_contract_with_gas_estimation, typ):
+def test_offset_repeater(get_contract, typ):
     offset_repeater = f"""
 @external
 def sum() -> {typ}:
     out: {typ} = 0
     for i: {typ} in range(80, 121):
         out = out + i
     return out
     """
 
-    c = get_contract_with_gas_estimation(offset_repeater)
+    c = get_contract(offset_repeater)
     assert c.sum() == 4100
 
 
 @pytest.mark.parametrize("typ", ["int128", "uint256"])
-def test_offset_repeater_2(get_contract_with_gas_estimation, typ):
+def test_offset_repeater_2(get_contract, typ):
     offset_repeater_2 = f"""
 @external
 def sum(frm: {typ}, to: {typ}) -> {typ}:
     out: {typ} = 0
     for i: {typ} in range(frm, frm + 101, bound=101):
         if i == to:
             break
         out = out + i
     return out
     """
 
-    c = get_contract_with_gas_estimation(offset_repeater_2)
+    c = get_contract(offset_repeater_2)
     assert c.sum(100, 99999) == 15150
     assert c.sum(70, 131) == 6100
 
 
-def test_loop_call_priv(get_contract_with_gas_estimation):
+def test_loop_call_priv(get_contract):
     code = """
 @internal
 def _bar() -> bool:
     return True
 
 @external
 def foo() -> bool:
     for i: uint256 in range(3):
         self._bar()
     return True
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() is True
 
 
 @pytest.mark.parametrize("typ", ["int128", "uint256"])
 def test_return_inside_repeater(get_contract, typ):
     code = f"""
 @internal
@@ -267,25 +270,46 @@
     assert found
     """
     c = get_contract(code)
     c.test()
 
 
 @pytest.mark.parametrize("typ", ["uint8", "int128", "uint256"])
-def test_for_range_oob_check(get_contract, tx_failed, typ):
+def test_for_range_oob_compile_time_check(get_contract, tx_failed, typ, experimental_codegen):
     code = f"""
 @external
 def test():
     x: {typ} = max_value({typ})
     for i: {typ} in range(x, x + 2, bound=2):
         pass
     """
+    if not experimental_codegen:
+        return
+    with pytest.raises(StaticAssertionException):
+        get_contract(code)
+
+
+@pytest.mark.parametrize(
+    "typ, max_value",
+    [
+        ("uint8", SizeLimits.MAX_UINT8),
+        ("int128", SizeLimits.MAX_INT128),
+        ("uint256", SizeLimits.MAX_UINT256),
+    ],
+)
+def test_for_range_oob_runtime_check(get_contract, tx_failed, typ, max_value):
+    code = f"""
+@external
+def test(x: {typ}):
+    for i: {typ} in range(x, x + 2, bound=2):
+        pass
+    """
     c = get_contract(code)
     with tx_failed():
-        c.test()
+        c.test(max_value)
 
 
 @pytest.mark.parametrize("typ", ["int128", "uint256"])
 def test_return_inside_nested_repeater(get_contract, typ):
     code = f"""
 @internal
 def _final(a: {typ}) -> {typ}:
@@ -372,15 +396,15 @@
         for x: {typ} in range(10):
             if i + x > a:
                 self.result = i + x
                 return
     self.result = 31337
     """
     c = get_contract(code)
-    c.foo(val, transact={})
+    c.foo(val)
     if val + 1 >= 19:
         assert c.result() == 31337
     else:
         assert c.result() == val + 1
 
 
 @pytest.mark.parametrize("typ", ["int128", "uint256"])
@@ -412,21 +436,40 @@
 
     c = get_contract(code)
     assert c.foo(100) == 6
     assert c.foo(1) == 666
     assert c.foo(0) == 31337
 
 
-def test_for_range_signed_int_overflow(get_contract, tx_failed):
+def test_for_range_signed_int_overflow_runtime_check(get_contract, tx_failed, experimental_codegen):
+    code = """
+@external
+def foo(_min:int256, _max: int256) -> DynArray[int256, 10]:
+    res: DynArray[int256, 10] = empty(DynArray[int256, 10])
+    x:int256 = _max
+    y:int256 = _min+2
+    for i:int256 in range(x,y , bound=10):
+        res.append(i)
+    return res
+    """
+    c = get_contract(code)
+    with tx_failed():
+        c.foo(SizeLimits.MIN_INT256, SizeLimits.MAX_INT256)
+
+
+def test_for_range_signed_int_overflow_compile_time_check(
+    get_contract, tx_failed, experimental_codegen
+):
     code = """
 @external
 def foo() -> DynArray[int256, 10]:
     res: DynArray[int256, 10] = empty(DynArray[int256, 10])
     x:int256 = max_value(int256)
     y:int256 = min_value(int256)+2
     for i:int256 in range(x,y , bound=10):
         res.append(i)
     return res
     """
-    c = get_contract(code)
-    with tx_failed():
-        c.foo()
+    if not experimental_codegen:
+        return
+    with pytest.raises(StaticAssertionException):
+        get_contract(code)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_assert.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,221 +1,246 @@
+import itertools
+
 import pytest
-from eth_tester.exceptions import TransactionFailed
+
+from tests.utils import ZERO_ADDRESS, decimal_to_int
+from vyper.compiler import compile_code
+from vyper.exceptions import TypeMismatch
+from vyper.utils import MemoryPositions
 
 
-# web3 returns f"execution reverted: {err_str}"
-# TODO move exception string parsing logic into tx_failed
-def _fixup_err_str(s):
-    return s.replace("execution reverted: ", "")
+def search_for_sublist(ir, sublist):
+    _list = ir.to_list() if hasattr(ir, "to_list") else ir
+    if _list == sublist:
+        return True
+    return isinstance(_list, list) and any(search_for_sublist(i, sublist) for i in _list)
 
 
-def test_assert_refund(w3, get_contract_with_gas_estimation, tx_failed):
+def test_builtin_constants(get_contract):
     code = """
 @external
-def foo():
-    raise
-    """
-    c = get_contract_with_gas_estimation(code)
-    a0 = w3.eth.accounts[0]
-    gas_sent = 10**6
-    tx_hash = c.foo(transact={"from": a0, "gas": gas_sent, "gasPrice": 10})
-    # More info on receipt status:
-    # https://github.com/ethereum/EIPs/blob/master/EIPS/eip-658.md#specification.
-    tx_receipt = w3.eth.get_transaction_receipt(tx_hash)
-    assert tx_receipt["status"] == 0
-    # Checks for gas refund from revert
-    assert tx_receipt["gasUsed"] < gas_sent
-
+def test_zaddress(a: address) -> bool:
+    return a == empty(address)
 
-def test_assert_reason(w3, get_contract_with_gas_estimation, tx_failed, memory_mocker):
-    code = """
-err: String[32]
 
 @external
-def test(a: int128) -> int128:
-    assert a > 1, "larger than one please"
-    return 1 + a
+def test_empty_bytes32(a: bytes32) -> bool:
+    return a == empty(bytes32)
+
 
 @external
-def test2(a: int128, b: int128, extra_reason: String[32]) -> int128:
-    c: int128 = 11
-    assert a > 1, "a is not large enough"
-    assert b == 1, concat("b may only be 1", extra_reason)
-    return a + b + c
+def test_int128(a: int128) -> (bool, bool):
+    return a == max_value(int128), a == min_value(int128)
+
 
 @external
-def test3(reason_str: String[32]):
-    raise reason_str
+def test_decimal(a: decimal) -> (bool, bool):
+    return a == max_value(decimal), a == min_value(decimal)
+
 
 @external
-def test4(a: int128, reason_str: String[32]) -> int128:
-    self.err = reason_str
-    assert a > 1, self.err
-    return 1 + a
+def test_uint256(a: uint256) -> bool:
+    return a == max_value(uint256)
+
 
 @external
-def test5(reason_str: String[32]):
-    self.err = reason_str
-    raise self.err
+def test_arithmetic(a: int128) -> int128:
+    return max_value(int128) - a
     """
-    c = get_contract_with_gas_estimation(code)
 
-    assert c.test(2) == 3
-    with pytest.raises(TransactionFailed) as e_info:
-        c.test(0)
+    c = get_contract(code)
+
+    assert c.test_empty_bytes32(b"\x00" * 32) is True
+    assert c.test_empty_bytes32(b"\x0F" * 32) is False
 
-    assert _fixup_err_str(e_info.value.args[0]) == "larger than one please"
-    # a = 0, b = 1
-    with pytest.raises(TransactionFailed) as e_info:
-        c.test2(0, 1, "")
-    assert _fixup_err_str(e_info.value.args[0]) == "a is not large enough"
-    # a = 1, b = 0
-    with pytest.raises(TransactionFailed) as e_info:
-        c.test2(2, 2, " because I said so")
-    assert _fixup_err_str(e_info.value.args[0]) == "b may only be 1" + " because I said so"
-    # return correct value
-    assert c.test2(5, 1, "") == 17
+    assert c.test_zaddress(ZERO_ADDRESS) is True
+    assert c.test_zaddress("0x0000000000000000000000000000000000000012") is False
 
-    with pytest.raises(TransactionFailed) as e_info:
-        c.test3("An exception")
-    assert _fixup_err_str(e_info.value.args[0]) == "An exception"
+    assert c.test_int128(2**127 - 1) == (True, False)
+    assert c.test_int128(-(2**127)) == (False, True)
+    assert c.test_int128(0) == (False, False)
 
-    assert c.test4(2, "msg") == 3
-    with pytest.raises(TransactionFailed) as e_info:
-        c.test4(0, "larger than one again please")
-    assert _fixup_err_str(e_info.value.args[0]) == "larger than one again please"
+    assert c.test_decimal(
+        decimal_to_int("18707220957835557353007165858768422651595.9365500927")
+    ) == (True, False)
+    assert c.test_decimal(
+        decimal_to_int("-18707220957835557353007165858768422651595.9365500928")
+    ) == (False, True)
+    assert c.test_decimal(decimal_to_int("0.1")) == (False, False)
 
-    with pytest.raises(TransactionFailed) as e_info:
-        c.test5("A storage exception")
-    assert _fixup_err_str(e_info.value.args[0]) == "A storage exception"
+    assert c.test_uint256(2**256 - 1) is True
 
+    assert c.test_arithmetic(5000) == 2**127 - 1 - 5000
 
-invalid_code = [
-    """
+
+def test_builtin_constants_assignment(get_contract):
+    code = """
 @external
-def test(a: int128) -> int128:
-    assert a > 1, ""
-    return 1 + a
-    """,
-    """
+def foo() -> int128:
+    bar: int128 = max_value(int128)
+    return bar
+
 @external
-def test(a: int128) -> int128:
-    raise ""
-    """,
-    """
+def goo() -> int128:
+    bar: int128 = min_value(int128)
+    return bar
+
 @external
-def test():
-    assert create_minimal_proxy_to(self)
-    """,
-]
+def hoo() -> bytes32:
+    bar: bytes32 = empty(bytes32)
+    return bar
 
+@external
+def joo() -> address:
+    bar: address = empty(address)
+    return bar
 
-@pytest.mark.parametrize("code", invalid_code)
-def test_invalid_assertions(get_contract, assert_compile_failed, code):
-    assert_compile_failed(lambda: get_contract(code))
+@external
+def koo() -> decimal:
+    bar: decimal = max_value(decimal)
+    return bar
 
+@external
+def loo() -> decimal:
+    bar: decimal = min_value(decimal)
+    return bar
 
-valid_code = [
-    """
 @external
-def mint(_to: address, _value: uint256):
-    raise
-    """,
+def zoo() -> uint256:
+    bar: uint256 = max_value(uint256)
+    return bar
     """
-@internal
-def ret1() -> int128:
-    return 1
+
+    c = get_contract(code)
+
+    assert c.foo() == 2**127 - 1
+    assert c.goo() == -(2**127)
+
+    assert c.hoo() == b"\x00" * 32
+
+    assert c.joo() == ZERO_ADDRESS
+
+    assert c.koo() == (2**167 - 1)
+    assert c.loo() == -(2**167)
+
+    assert c.zoo() == 2**256 - 1
+
+
+def test_custom_constants(get_contract):
+    code = """
+X_VALUE: constant(uint256) = 33
+
 @external
-def test():
-    assert self.ret1() == 1
-    """,
-    """
+def test() -> uint256:
+    return X_VALUE
+
 @external
-def test():
-    assert raw_call(msg.sender, b'', max_outsize=1, gas=10, value=1000*1000) == b''
-    """,
+def test_add(a: uint256) -> uint256:
+    return X_VALUE + a
     """
-@external
-def test():
-    assert create_minimal_proxy_to(self) == self
-    """,
-]
+    c = get_contract(code)
 
+    assert c.test() == 33
+    assert c.test_add(7) == 40
 
-@pytest.mark.parametrize("code", valid_code)
-def test_valid_assertions(get_contract, code):
-    get_contract(code)
 
+# Would be nice to put this somewhere accessible, like in vyper.types or something
+integer_types = ["uint8", "int128", "int256", "uint256"]
 
-def test_assert_staticcall(get_contract, tx_failed, memory_mocker):
-    foreign_code = """
-state: uint256
-@external
-def not_really_constant() -> uint256:
-    self.state += 1
-    return self.state
-    """
-    code = """
-interface ForeignContract:
-    def not_really_constant() -> uint256: view
+
+@pytest.mark.parametrize("storage_type,return_type", itertools.permutations(integer_types, 2))
+def test_custom_constants_fail(get_contract, assert_compile_failed, storage_type, return_type):
+    code = f"""
+MY_CONSTANT: constant({storage_type}) = 1
 
 @external
-def test():
-    assert staticcall ForeignContract(msg.sender).not_really_constant() == 1
+def foo() -> {return_type}:
+    return MY_CONSTANT
     """
-    c1 = get_contract(foreign_code)
-    c2 = get_contract(code, *[c1.address])
-    # static call prohibits state change
-    with tx_failed():
-        c2.test()
+    assert_compile_failed(lambda: get_contract(code), TypeMismatch)
 
 
-def test_assert_in_for_loop(get_contract, tx_failed, memory_mocker):
+def test_constant_address(get_contract):
     code = """
+OWNER: constant(address) = 0x0000000000000000000000000000000000000012
+
 @external
-def test(x: uint256[3]) -> bool:
-    for i: uint256 in range(3):
-        assert x[i] < 5
-    return True
-    """
+def get_owner() -> address:
+    return OWNER
 
+@external
+def is_owner() -> bool:
+    if msg.sender == OWNER:
+        return True
+    else:
+        return False
+    """
     c = get_contract(code)
 
-    c.test([1, 2, 3])
-    with tx_failed():
-        c.test([5, 1, 3])
-    with tx_failed():
-        c.test([1, 5, 3])
-    with tx_failed():
-        c.test([1, 3, 5])
+    assert c.get_owner() == "0x0000000000000000000000000000000000000012"
+    assert c.is_owner() is False
 
 
-def test_assert_with_reason_in_for_loop(get_contract, tx_failed, memory_mocker):
-    code = """
+def test_constant_bytes(get_contract):
+    test_str = b"Alabama, Arkansas. I do love my ma and pa"
+    code = f"""
+X: constant(Bytes[100]) = b"{test_str.decode()}"
+
 @external
-def test(x: uint256[3]) -> bool:
-    for i: uint256 in range(3):
-        assert x[i] < 5, "because reasons"
-    return True
+def test() -> Bytes[100]:
+    y: Bytes[100] = X
+
+    return y
     """
 
     c = get_contract(code)
 
-    c.test([1, 2, 3])
-    with tx_failed():
-        c.test([5, 1, 3])
-    with tx_failed():
-        c.test([1, 5, 3])
-    with tx_failed():
-        c.test([1, 3, 5])
+    assert c.test() == test_str
+
+
+def test_constant_folds(experimental_codegen):
+    some_prime = 10013677
+    code = f"""
+SOME_CONSTANT: constant(uint256) = 11 + 1
+SOME_PRIME: constant(uint256) = {some_prime}
+
+@external
+def test() -> uint256:
+    # calculate some constant which is really unlikely to be randomly
+    # in bytecode
+    ret: uint256 = 2**SOME_CONSTANT * SOME_PRIME
+    return ret
+    """
+    ir = compile_code(code, output_formats=["ir"])["ir"]
+    memory = "$alloca_64_32" if experimental_codegen else MemoryPositions.RESERVED_MEMORY
+    search = ["mstore", [memory], [2**12 * some_prime]]
+    assert search_for_sublist(ir, search)
 
 
-def test_assert_reason_revert_length(w3, get_contract, tx_failed, memory_mocker):
+def test_constant_lists(get_contract):
     code = """
+BYTE32_LIST: constant(bytes32[2]) = [
+    0x0000000000000000000000000000000000000000000000000000000000001321,
+    0x0000000000000000000000000000000000000000000000000000000000001123
+]
+
+SPECIAL: constant(int128[3]) = [33, 44, 55]
+
+@external
+def test() -> bytes32:
+    a: bytes32[2] = BYTE32_LIST
+    return a[1]
+
+@view
 @external
-def test() -> int128:
-    assert 1 == 2, "oops"
-    return 1
-"""
+def contains(a: int128) -> bool:
+    return a in SPECIAL
+    """
+
     c = get_contract(code)
-    with tx_failed(exc_text="oops"):
-        c.test()
+
+    assert c.test()[-2:] == b"\x11\x23"
+
+    assert c.contains(55) is True
+    assert c.contains(44) is True
+    assert c.contains(33) is True
+    assert c.contains(3) is False
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_assignment.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_assignment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from vyper.exceptions import ImmutableViolation, InvalidType, TypeMismatch
 
 
-def test_augassign(get_contract_with_gas_estimation):
+def test_augassign(get_contract):
     augassign_test = """
 @external
 def augadd(x: int128, y: int128) -> int128:
     z: int128 = x
     z += y
     return z
 
@@ -26,15 +26,15 @@
 @external
 def augmod(x: int128, y: int128) -> int128:
     z: int128 = x
     z %= y
     return z
     """
 
-    c = get_contract_with_gas_estimation(augassign_test)
+    c = get_contract(augassign_test)
 
     assert c.augadd(5, 12) == 17
     assert c.augmul(5, 12) == 60
     assert c.augsub(5, 12) == -7
     assert c.augmod(5, 12) == 5
     print("Passed aug-assignment test")
 
@@ -44,31 +44,31 @@
     [
         ("uint256", 77, 123),
         ("uint256[3]", [1, 2, 3], [4, 5, 6]),
         ("DynArray[uint256, 3]", [1, 2, 3], [4, 5, 6]),
         ("Bytes[5]", b"vyper", b"conda"),
     ],
 )
-def test_internal_assign(get_contract_with_gas_estimation, typ, in_val, out_val):
+def test_internal_assign(get_contract, typ, in_val, out_val):
     code = f"""
 @internal
 def foo(x: {typ}) -> {typ}:
     x = {out_val}
     return x
 
 @external
 def bar(x: {typ}) -> {typ}:
     return self.foo(x)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.bar(in_val) == out_val
 
 
-def test_internal_assign_struct(get_contract_with_gas_estimation):
+def test_internal_assign_struct(get_contract):
     code = """
 flag Bar:
     BAD
     BAK
     BAZ
 
 struct Foo:
@@ -81,20 +81,20 @@
     x = Foo(a=789, b=[Bar.BAZ, Bar.BAK, Bar.BAD], c=\"conda\")
     return x
 
 @external
 def bar(x: Foo) -> Foo:
     return self.foo(x)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.bar((123, [1, 2, 4], "vyper")) == (789, [4, 2, 1], "conda")
 
 
-def test_internal_assign_struct_member(get_contract_with_gas_estimation):
+def test_internal_assign_struct_member(get_contract):
     code = """
 flag Bar:
     BAD
     BAK
     BAZ
 
 struct Foo:
@@ -108,71 +108,71 @@
     x.b.pop()
     return x
 
 @external
 def bar(x: Foo) -> Foo:
     return self.foo(x)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.bar((123, [1, 2, 4], "vyper")) == (789, [1, 2], "vyper")
 
 
-def test_internal_augassign(get_contract_with_gas_estimation):
+def test_internal_augassign(get_contract):
     code = """
 @internal
 def foo(x: int128) -> int128:
     x += 77
     return x
 
 @external
 def bar(x: int128) -> int128:
     return self.foo(x)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.bar(123) == 200
 
 
 @pytest.mark.parametrize("typ", ["DynArray[uint256, 3]", "uint256[3]"])
-def test_internal_augassign_arrays(get_contract_with_gas_estimation, typ):
+def test_internal_augassign_arrays(get_contract, typ):
     code = f"""
 @internal
 def foo(x: {typ}) -> {typ}:
     x[1] += 77
     return x
 
 @external
 def bar(x: {typ}) -> {typ}:
     return self.foo(x)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.bar([1, 2, 3]) == [1, 79, 3]
 
 
-def test_invalid_external_assign(assert_compile_failed, get_contract_with_gas_estimation):
+def test_invalid_external_assign(assert_compile_failed, get_contract):
     code = """
 @external
 def foo(x: int128):
     x = 5
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), ImmutableViolation)
+    assert_compile_failed(lambda: get_contract(code), ImmutableViolation)
 
 
-def test_invalid_external_augassign(assert_compile_failed, get_contract_with_gas_estimation):
+def test_invalid_external_augassign(assert_compile_failed, get_contract):
     code = """
 @external
 def foo(x: int128):
     x += 5
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), ImmutableViolation)
+    assert_compile_failed(lambda: get_contract(code), ImmutableViolation)
 
 
-def test_valid_literal_increment(get_contract_with_gas_estimation):
+def test_valid_literal_increment(get_contract):
     code = """
 storx: uint256
 
 @external
 def foo1() -> int128:
     x: int128 = 122
     x += 1
@@ -186,51 +186,51 @@
 
 @external
 def foo3(y: uint256) -> uint256:
     self.storx = y
     self.storx += 1
     return self.storx
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.foo1() == 123
     assert c.foo2() == 123
     assert c.foo3(11) == 12
 
 
-def test_invalid_uint256_assignment(assert_compile_failed, get_contract_with_gas_estimation):
+def test_invalid_uint256_assignment(assert_compile_failed, get_contract):
     code = """
 storx: uint256
 
 @external
 def foo2() -> uint256:
     x: uint256 = -1
     x += 1
     return x
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), TypeMismatch)
+    assert_compile_failed(lambda: get_contract(code), TypeMismatch)
 
 
-def test_invalid_uint256_assignment_calculate_literals(get_contract_with_gas_estimation):
+def test_invalid_uint256_assignment_calculate_literals(get_contract):
     code = """
 storx: uint256
 
 @external
 def foo2() -> uint256:
     x: uint256 = 0
     x = 3 * 4 // 2 + 1 - 2
     return x
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.foo2() == 5
 
 
 # See #838. Confirm that nested keys and structs work properly.
-def test_nested_map_key_works(get_contract_with_gas_estimation):
+def test_nested_map_key_works(get_contract):
     code = """
 struct X:
     a: int128
     b: int128
 struct Y:
     c: int128
     d: int128
@@ -244,20 +244,20 @@
 
 
 @external
 def get(i: int128) -> int128:
     idx: int128 = self.test_map1[i].a
     return self.test_map2[idx].c
     """
-    c = get_contract_with_gas_estimation(code)
-    assert c.set(transact={})
+    c = get_contract(code)
+    c.set()
     assert c.get(1) == 111
 
 
-def test_nested_map_key_problem(get_contract_with_gas_estimation):
+def test_nested_map_key_problem(get_contract):
     code = """
 struct X:
     a: int128
     b: int128
 struct Y:
     c: int128
     d: int128
@@ -270,16 +270,16 @@
     self.test_map2[333].c = 111
 
 
 @external
 def get() -> int128:
     return self.test_map2[self.test_map1[1].a].c
     """
-    c = get_contract_with_gas_estimation(code)
-    assert c.set(transact={})
+    c = get_contract(code)
+    c.set()
     assert c.get() == 111
 
 
 @pytest.mark.parametrize(
     "contract",
     [
         """
@@ -345,31 +345,29 @@
 def foo():
     y: uint256 = 1
     z: bytes32 = empty(bytes32)
     z = y
     """,
     ],
 )
-def test_invalid_implicit_conversions(
-    contract, assert_compile_failed, get_contract_with_gas_estimation
-):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(contract), TypeMismatch)
+def test_invalid_implicit_conversions(contract, assert_compile_failed, get_contract):
+    assert_compile_failed(lambda: get_contract(contract), TypeMismatch)
 
 
-def test_invalid_nonetype_assignment(assert_compile_failed, get_contract_with_gas_estimation):
+def test_invalid_nonetype_assignment(assert_compile_failed, get_contract):
     code = """
 @internal
 def bar():
     pass
 
 @external
 def foo():
     ret : bool = self.bar()
 """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), InvalidType)
+    assert_compile_failed(lambda: get_contract(code), InvalidType)
 
     # GH issue 2418
 
 
 overlap_codes = [
     """
 @external
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_bytes_map_keys.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_bytes_map_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import pytest
 
 from vyper.exceptions import TypeMismatch
 
 
-def test_basic_bytes_keys(w3, get_contract):
+def test_basic_bytes_keys(env, get_contract):
     code = """
 mapped_bytes: HashMap[Bytes[5], int128]
 
 @external
 def set(k: Bytes[5], v: int128):
     self.mapped_bytes[k] = v
 
 @external
 def get(k: Bytes[5]) -> int128:
     return self.mapped_bytes[k]
     """
 
     c = get_contract(code)
 
-    c.set(b"test", 54321, transact={})
+    c.set(b"test", 54321)
 
     assert c.get(b"test") == 54321
 
 
 def test_basic_bytes_literal_key(get_contract):
     code = """
 mapped_bytes: HashMap[Bytes[5], int128]
@@ -34,15 +34,15 @@
 @external
 def get(k: Bytes[5]) -> int128:
     return self.mapped_bytes[k]
     """
 
     c = get_contract(code)
 
-    c.set(54321, transact={})
+    c.set(54321)
 
     assert c.get(b"test") == 54321
 
 
 def test_basic_long_bytes_as_keys(get_contract):
     code = """
 mapped_bytes: HashMap[Bytes[34], int128]
@@ -54,15 +54,15 @@
 @external
 def get(k: Bytes[34]) -> int128:
     return self.mapped_bytes[k]
     """
 
     c = get_contract(code)
 
-    c.set(b"a" * 34, 6789, transact={"gas": 10**6})
+    c.set(b"a" * 34, 6789, gas=10**6)
 
     assert c.get(b"a" * 34) == 6789
 
 
 def test_mismatched_byte_length(get_contract):
     code = """
 mapped_bytes: HashMap[Bytes[34], int128]
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_clampers.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_clampers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,95 @@
 from decimal import Decimal
 
 import pytest
 from eth.codecs import abi
 from eth_utils import keccak
 
-from tests.utils import decimal_to_int
+from tests.utils import ZERO_ADDRESS, decimal_to_int
 from vyper.exceptions import StackTooDeep
 from vyper.utils import int_bounds
 
 
-def _make_tx(w3, address, signature, values):
-    # helper function to broadcast transactions that fail clamping check
+def _make_tx(env, address, signature, values):
+    # helper function to create data that will fail runtime clamp
     sig = keccak(signature.encode()).hex()[:8]
     data = "".join(int(i).to_bytes(32, "big", signed=i < 0).hex() for i in values)
-    w3.eth.send_transaction({"to": address, "data": f"0x{sig}{data}"})
+    env.message_call(address, data=f"0x{sig}{data}")
 
 
-def _make_abi_encode_tx(w3, address, signature, input_types, values):
+def _make_abi_encode_tx(env, address, signature, input_types, values):
     # helper function to broadcast transactions where data is constructed from abi_encode
     sig = keccak(signature.encode()).hex()[:8]
     data = abi.encode(input_types, values).hex()
-    w3.eth.send_transaction({"to": address, "data": f"0x{sig}{data}"})
+    env.message_call(address, data=f"0x{sig}{data}")
 
 
 def _make_dynarray_data(offset, length, values):
     input = [offset] + [length] + values
     data = "".join(int(i).to_bytes(32, "big", signed=i < 0).hex() for i in input)
     return data
 
 
-def _make_invalid_dynarray_tx(w3, address, signature, data):
+def _make_invalid_dynarray_tx(env, address, signature, data):
     sig = keccak(signature.encode()).hex()[:8]
-    w3.eth.send_transaction({"to": address, "data": f"0x{sig}{data}"})
+    env.message_call(address, data=f"0x{sig}{data}")
 
 
-def test_bytes_clamper(tx_failed, get_contract_with_gas_estimation):
+def test_bytes_clamper(tx_failed, get_contract):
     clamper_test_code = """
 @external
 def foo(s: Bytes[3]) -> Bytes[3]:
     return s
     """
 
-    c = get_contract_with_gas_estimation(clamper_test_code)
+    c = get_contract(clamper_test_code)
     assert c.foo(b"ca") == b"ca"
     assert c.foo(b"cat") == b"cat"
     with tx_failed():
         c.foo(b"cate")
 
 
-def test_bytes_clamper_multiple_slots(tx_failed, get_contract_with_gas_estimation):
+def test_bytes_clamper_multiple_slots(tx_failed, get_contract):
     clamper_test_code = """
 @external
 def foo(s: Bytes[40]) -> Bytes[40]:
     return s
     """
 
     data = b"this is exactly forty characters long!!!"
-    c = get_contract_with_gas_estimation(clamper_test_code)
+    c = get_contract(clamper_test_code)
 
     assert c.foo(data[:30]) == data[:30]
     assert c.foo(data) == data
     with tx_failed():
         c.foo(data + b"!")
 
 
-def test_bytes_clamper_on_init(tx_failed, get_contract_with_gas_estimation):
+def test_bytes_clamper_on_init(tx_failed, get_contract):
     clamper_test_code = """
 foo: Bytes[3]
 
 @deploy
 def __init__(x: Bytes[3]):
     self.foo = x
 
 @external
 def get_foo() -> Bytes[3]:
     return self.foo
     """
 
-    c = get_contract_with_gas_estimation(clamper_test_code, *[b"cat"])
+    c = get_contract(clamper_test_code, b"cat")
     assert c.get_foo() == b"cat"
 
     with tx_failed():
-        get_contract_with_gas_estimation(clamper_test_code, *[b"cats"])
+        get_contract(clamper_test_code, b"cats")
 
 
 @pytest.mark.parametrize("n", list(range(1, 33)))
-def test_bytes_m_clamper_passing(w3, get_contract, n):
+def test_bytes_m_clamper_passing(env, get_contract, n):
     values = [b"\xff" * (i + 1) for i in range(n)]
 
     code = f"""
 @external
 def foo(s: bytes{n}) -> bytes{n}:
     return s
     """
@@ -97,15 +97,15 @@
     c = get_contract(code)
     for v in values:
         v = v.ljust(n, b"\x00")
         assert c.foo(v) == v
 
 
 @pytest.mark.parametrize("n", list(range(1, 32)))  # bytes32 always passes
-def test_bytes_m_clamper_failing(w3, get_contract, tx_failed, n):
+def test_bytes_m_clamper_failing(env, get_contract, tx_failed, n):
     values = []
     values.append(b"\x00" * n + b"\x80")  # just one bit set
     values.append(b"\xff" * n + b"\x80")  # n*8 + 1 bits set
     values.append(b"\x00" * 31 + b"\x01")  # bytes32
     values.append(b"\xff" * 32)  # bytes32
     values.append(bytes(range(32)))  # 0x00010203..1f
     values.append(bytes(range(1, 33)))  # 0x01020304..a0
@@ -116,21 +116,21 @@
 def foo(s: bytes{n}) -> bytes{n}:
     return s
     """
 
     c = get_contract(code)
     for v in values:
         # munge for `_make_tx`
+        int_value = int.from_bytes(v, byteorder="big")
         with tx_failed():
-            int_value = int.from_bytes(v, byteorder="big")
-            _make_tx(w3, c.address, f"foo(bytes{n})", [int_value])
+            _make_tx(env, c.address, f"foo(bytes{n})", [int_value])
 
 
 @pytest.mark.parametrize("n", list(range(32)))
-def test_sint_clamper_passing(w3, get_contract, n):
+def test_sint_clamper_passing(env, get_contract, n):
     bits = 8 * (n + 1)
     lo, hi = int_bounds(True, bits)
     values = [-1, 0, 1, lo, hi]
     code = f"""
 @external
 def foo(s: int{bits}) -> int{bits}:
     return s
@@ -138,57 +138,57 @@
 
     c = get_contract(code)
     for v in values:
         assert c.foo(v) == v
 
 
 @pytest.mark.parametrize("n", list(range(31)))  # int256 does not clamp
-def test_sint_clamper_failing(w3, tx_failed, get_contract, n):
+def test_sint_clamper_failing(env, tx_failed, get_contract, n):
     bits = 8 * (n + 1)
     lo, hi = int_bounds(True, bits)
     values = [-(2**255), 2**255 - 1, lo - 1, hi + 1]
     code = f"""
 @external
 def foo(s: int{bits}) -> int{bits}:
     return s
     """
 
     c = get_contract(code)
     for v in values:
         with tx_failed():
-            _make_tx(w3, c.address, f"foo(int{bits})", [v])
+            _make_tx(env, c.address, f"foo(int{bits})", [v])
 
 
 @pytest.mark.parametrize("value", [True, False])
-def test_bool_clamper_passing(w3, get_contract, value):
+def test_bool_clamper_passing(env, get_contract, value):
     code = """
 @external
 def foo(s: bool) -> bool:
     return s
     """
 
     c = get_contract(code)
     assert c.foo(value) == value
 
 
 @pytest.mark.parametrize("value", [2, 3, 4, 8, 16, 2**256 - 1])
-def test_bool_clamper_failing(w3, tx_failed, get_contract, value):
+def test_bool_clamper_failing(env, tx_failed, get_contract, value):
     code = """
 @external
 def foo(s: bool) -> bool:
     return s
     """
 
     c = get_contract(code)
     with tx_failed():
-        _make_tx(w3, c.address, "foo(bool)", [value])
+        _make_tx(env, c.address, "foo(bool)", [value])
 
 
 @pytest.mark.parametrize("value", [0] + [2**i for i in range(5)])
-def test_flag_clamper_passing(w3, get_contract, value):
+def test_flag_clamper_passing(env, get_contract, value):
     code = """
 flag Roles:
     USER
     STAFF
     ADMIN
     MANAGER
     CEO
@@ -199,15 +199,15 @@
     """
 
     c = get_contract(code)
     assert c.foo(value) == value
 
 
 @pytest.mark.parametrize("value", [2**i for i in range(5, 256)])
-def test_flag_clamper_failing(w3, tx_failed, get_contract, value):
+def test_flag_clamper_failing(env, tx_failed, get_contract, value):
     code = """
 flag Roles:
     USER
     STAFF
     ADMIN
     MANAGER
     CEO
@@ -215,83 +215,77 @@
 @external
 def foo(s: Roles) -> Roles:
     return s
     """
 
     c = get_contract(code)
     with tx_failed():
-        _make_tx(w3, c.address, "foo(uint256)", [value])
+        _make_tx(env, c.address, "foo(uint256)", [value])
 
 
 @pytest.mark.parametrize("n", list(range(32)))
-def test_uint_clamper_passing(w3, get_contract, n):
+def test_uint_clamper_passing(env, get_contract, n):
     bits = 8 * (n + 1)
     values = [0, 1, 2**bits - 1]
     code = f"""
 @external
 def foo(s: uint{bits}) -> uint{bits}:
     return s
     """
 
     c = get_contract(code)
     for v in values:
         assert c.foo(v) == v
 
 
 @pytest.mark.parametrize("n", list(range(31)))  # uint256 has no failing cases
-def test_uint_clamper_failing(w3, tx_failed, get_contract, n):
+def test_uint_clamper_failing(env, tx_failed, get_contract, n):
     bits = 8 * (n + 1)
     values = [-1, -(2**255), 2**bits]
     code = f"""
 @external
 def foo(s: uint{bits}) -> uint{bits}:
     return s
     """
     c = get_contract(code)
     for v in values:
         with tx_failed():
-            _make_tx(w3, c.address, f"foo(uint{bits})", [v])
+            _make_tx(env, c.address, f"foo(uint{bits})", [v])
 
 
 @pytest.mark.parametrize(
-    "value,expected",
+    "address",
     [
-        ("0x0000000000000000000000000000000000000000", None),
-        (
-            "0x0000000000000000000000000000000000000001",
-            "0x0000000000000000000000000000000000000001",
-        ),
-        (
-            "0xFFfFfFffFFfffFFfFFfFFFFFffFFFffffFfFFFfF",
-            "0xFFfFfFffFFfffFFfFFfFFFFFffFFFffffFfFFFfF",
-        ),
+        ZERO_ADDRESS,
+        "0x0000000000000000000000000000000000000001",
+        "0xFFfFfFffFFfffFFfFFfFFFFFffFFFffffFfFFFfF",
     ],
 )
-def test_address_clamper_passing(w3, get_contract, value, expected):
+def test_address_clamper_passing(get_contract, address):
     code = """
 @external
 def foo(s: address) -> address:
     return s
     """
 
     c = get_contract(code)
-    assert c.foo(value) == expected
+    assert c.foo(address) == address
 
 
 @pytest.mark.parametrize("value", [2**160, 2**256 - 1])
-def test_address_clamper_failing(w3, tx_failed, get_contract, value):
+def test_address_clamper_failing(env, tx_failed, get_contract, value):
     code = """
 @external
 def foo(s: address) -> address:
     return s
     """
 
     c = get_contract(code)
     with tx_failed():
-        _make_tx(w3, c.address, "foo(address)", [value])
+        _make_tx(env, c.address, "foo(address)", [value])
 
 
 @pytest.mark.parametrize(
     "value",
     [
         0,
         1,
@@ -326,29 +320,29 @@
     [
         2**167,
         -(2**167 + 1),
         187072209578355573530071658587684226515959365500928,  # 2 ** 167
         -187072209578355573530071658587684226515959365500929,  # - (2 ** 127 - 1e-10)
     ],
 )
-def test_decimal_clamper_failing(w3, tx_failed, get_contract, value):
+def test_decimal_clamper_failing(env, tx_failed, get_contract, value):
     code = """
 @external
 def foo(s: decimal) -> decimal:
     return s
     """
 
     c = get_contract(code)
 
     with tx_failed():
-        _make_tx(w3, c.address, "foo(int168)", [value])
+        _make_tx(env, c.address, "foo(int168)", [value])
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
-def test_int128_array_clamper_passing(w3, get_contract, value):
+def test_int128_array_clamper_passing(get_contract, value):
     code = """
 @external
 def foo(a: uint256, b: int128[5], c: uint256) -> int128[5]:
     return b
     """
 
     # on both ends of the array we place a `uint256` that would fail the clamp check,
@@ -356,94 +350,94 @@
     d = [value] * 5
     c = get_contract(code)
     assert c.foo(2**127, [value] * 5, 2**127) == d
 
 
 @pytest.mark.parametrize("bad_value", [2**127, -(2**127) - 1, 2**255 - 1, -(2**255)])
 @pytest.mark.parametrize("idx", range(5))
-def test_int128_array_clamper_failing(w3, tx_failed, get_contract, bad_value, idx):
+def test_int128_array_clamper_failing(env, tx_failed, get_contract, bad_value, idx):
     # ensure the invalid value is detected at all locations in the array
     code = """
 @external
 def foo(b: int128[5]) -> int128[5]:
     return b
     """
 
     values = [0] * 5
     values[idx] = bad_value
 
     c = get_contract(code)
     with tx_failed():
-        _make_tx(w3, c.address, "foo(int128[5])", values)
+        _make_tx(env, c.address, "foo(int128[5])", values)
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
-def test_int128_array_looped_clamper_passing(w3, get_contract, value):
+def test_int128_array_looped_clamper_passing(get_contract, value):
     # when an array is > 5 items, the arg clamper runs in a loop to reduce bytecode size
     code = """
 @external
 def foo(a: uint256, b: int128[10], c: uint256) -> int128[10]:
     return b
     """
 
     d = [value] * 10
     c = get_contract(code)
     assert c.foo(2**127, d, 2**127) == d
 
 
 @pytest.mark.parametrize("bad_value", [2**127, -(2**127) - 1, 2**255 - 1, -(2**255)])
 @pytest.mark.parametrize("idx", range(10))
-def test_int128_array_looped_clamper_failing(w3, tx_failed, get_contract, bad_value, idx):
+def test_int128_array_looped_clamper_failing(env, tx_failed, get_contract, bad_value, idx):
     code = """
 @external
 def foo(b: int128[10]) -> int128[10]:
     return b
     """
 
     values = [0] * 10
     values[idx] = bad_value
 
     c = get_contract(code)
     with tx_failed():
-        _make_tx(w3, c.address, "foo(int128[10])", values)
+        _make_tx(env, c.address, "foo(int128[10])", values)
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
-def test_multidimension_array_clamper_passing(w3, get_contract, value):
+def test_multidimension_array_clamper_passing(get_contract, value):
     code = """
 @external
 def foo(a: uint256, b: int128[6][3][1][8], c: uint256) -> int128[6][3][1][8]:
     return b
     """
 
     # 6 * 3 * 1 * 8 = 144, the total number of values in our multidimensional array
     d = [[[[value] * 6] * 3] * 1] * 8
     c = get_contract(code)
-    assert c.foo(2**127, d, 2**127, call={"gasPrice": 0}) == d
+    assert c.foo(2**127, d, 2**127) == d
 
 
 @pytest.mark.parametrize("bad_value", [2**127, -(2**127) - 1, 2**255 - 1, -(2**255)])
 @pytest.mark.parametrize("idx", range(12))
-def test_multidimension_array_clamper_failing(w3, tx_failed, get_contract, bad_value, idx):
+def test_multidimension_array_clamper_failing(env, tx_failed, get_contract, bad_value, idx):
     code = """
 @external
 def foo(b: int128[6][1][2]) -> int128[6][1][2]:
     return b
     """
 
     values = [0] * 12
     values[idx] = bad_value
 
     c = get_contract(code)
     with tx_failed():
-        _make_tx(w3, c.address, "foo(int128[6][1][2]])", values)
+        _make_tx(env, c.address, "foo(int128[6][1][2]])", values)
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
-def test_int128_dynarray_clamper_passing(w3, get_contract, value):
+def test_int128_dynarray_clamper_passing(get_contract, value):
     code = """
 @external
 def foo(a: uint256, b: DynArray[int128, 5], c: uint256) -> DynArray[int128, 5]:
     return b
     """
 
     # on both ends of the array we place a `uint256` that would fail the clamp check,
@@ -451,15 +445,15 @@
     d = [value] * 5
     c = get_contract(code)
     assert c.foo(2**127, d, 2**127) == d
 
 
 @pytest.mark.parametrize("bad_value", [2**127, -(2**127) - 1, 2**255 - 1, -(2**255)])
 @pytest.mark.parametrize("idx", range(5))
-def test_int128_dynarray_clamper_failing(w3, tx_failed, get_contract, bad_value, idx):
+def test_int128_dynarray_clamper_failing(env, tx_failed, get_contract, bad_value, idx):
     # ensure the invalid value is detected at all locations in the array
     code = """
 @external
 def foo(b: int128[5]) -> int128[5]:
     return b
     """
 
@@ -467,71 +461,71 @@
     values[idx] = bad_value
     signature = "foo(int128[])"
 
     c = get_contract(code)
 
     data = _make_dynarray_data(32, 5, values)
     with tx_failed():
-        _make_invalid_dynarray_tx(w3, c.address, signature, data)
+        _make_invalid_dynarray_tx(env, c.address, signature, data)
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
-def test_int128_dynarray_looped_clamper_passing(w3, get_contract, value):
+def test_int128_dynarray_looped_clamper_passing(get_contract, value):
     # when an array is > 5 items, the arg clamper runs in a loop to reduce bytecode size
     code = """
 @external
 def foo(a: uint256, b: DynArray[int128, 10], c: uint256) -> DynArray[int128, 10]:
     return b
     """
     d = [value] * 10
     c = get_contract(code)
     assert c.foo(2**127, d, 2**127) == d
 
 
 @pytest.mark.parametrize("bad_value", [2**127, -(2**127) - 1, 2**255 - 1, -(2**255)])
 @pytest.mark.parametrize("idx", range(10))
-def test_int128_dynarray_looped_clamper_failing(w3, tx_failed, get_contract, bad_value, idx):
+def test_int128_dynarray_looped_clamper_failing(env, tx_failed, get_contract, bad_value, idx):
     code = """
 @external
 def foo(b: DynArray[int128, 10]) -> DynArray[int128, 10]:
     return b
     """
 
     values = [0] * 10
     values[idx] = bad_value
 
     c = get_contract(code)
 
     data = _make_dynarray_data(32, 10, values)
     signature = "foo(int128[])"
     with tx_failed():
-        _make_invalid_dynarray_tx(w3, c.address, signature, data)
+        _make_invalid_dynarray_tx(env, c.address, signature, data)
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
 @pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
-def test_multidimension_dynarray_clamper_passing(w3, get_contract, value):
+def test_multidimension_dynarray_clamper_passing(get_contract, value):
     code = """
 @external
 def foo(
     a: uint256,
     b: DynArray[DynArray[DynArray[DynArray[int128, 5], 6], 7], 8],
     c: uint256
 ) -> DynArray[DynArray[DynArray[DynArray[int128, 5], 6], 7], 8]:
     return b
     """
     # Out of gas exception if outermost length is 6 and greater
     d = [[[[value] * 5] * 6] * 7] * 8
     c = get_contract(code)
-    assert c.foo(2**127, d, 2**127, call={"gasPrice": 0}) == d
+    assert c.foo(2**127, d, 2**127) == d
 
 
 @pytest.mark.parametrize("bad_value", [2**127, -(2**127) - 1, 2**255 - 1, -(2**255)])
 @pytest.mark.parametrize("idx", range(4))
-def test_multidimension_dynarray_clamper_failing(w3, tx_failed, get_contract, bad_value, idx):
+def test_multidimension_dynarray_clamper_failing(env, tx_failed, get_contract, bad_value, idx):
     code = """
 @external
 def foo(b: DynArray[DynArray[int128, 2], 2]) -> DynArray[DynArray[int128, 2], 2]:
     return b
     """
 
     values = [[0] * 2] * 2
@@ -544,19 +538,19 @@
         inner_data = "".join(int(_v).to_bytes(32, "big", signed=_v < 0).hex() for _v in v)
         data += inner_data
 
     signature = "foo(int128[][])"
 
     c = get_contract(code)
     with tx_failed():
-        _make_invalid_dynarray_tx(w3, c.address, signature, data)
+        _make_invalid_dynarray_tx(env, c.address, signature, data)
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
-def test_dynarray_list_clamper_passing(w3, get_contract, value):
+def test_dynarray_list_clamper_passing(get_contract, value):
     code = """
 @external
 def foo(
     a: uint256,
     b: DynArray[int128[5], 6],
     c: uint256
 ) -> DynArray[int128[5], 6]:
@@ -565,15 +559,15 @@
     d = [[value] * 5] * 6
     c = get_contract(code)
     assert c.foo(2**127, d, 2**127) == d
 
 
 @pytest.mark.parametrize("bad_value", [2**127, -(2**127) - 1, 2**255 - 1, -(2**255)])
 @pytest.mark.parametrize("idx", range(10))
-def test_dynarray_list_clamper_failing(w3, tx_failed, get_contract, bad_value, idx):
+def test_dynarray_list_clamper_failing(env, tx_failed, get_contract, bad_value, idx):
     # ensure the invalid value is detected at all locations in the array
     code = """
 @external
 def foo(b: DynArray[int128[5], 2]) -> DynArray[int128[5], 2]:
     return b
     """
 
@@ -584,8 +578,8 @@
     for v in values:
         inner_data = "".join(int(_v).to_bytes(32, "big", signed=_v < 0).hex() for _v in v)
         data += inner_data
 
     c = get_contract(code)
     signature = "foo(int128[5][])"
     with tx_failed():
-        _make_invalid_dynarray_tx(w3, c.address, signature, data)
+        _make_invalid_dynarray_tx(env, c.address, signature, data)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_comparison.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_comparison.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_immutable.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_immutable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 from vyper.compiler.settings import OptimizationLevel
-from vyper.exceptions import StackTooDeep
 
 
 @pytest.mark.parametrize(
     "typ,value",
     [
         ("uint256", 42),
         ("int256", -(2**200)),
@@ -73,15 +72,15 @@
 @view
 @external
 def get_values() -> (uint256, address, String[64]):
     return a, b, c
     """
     values = (3, "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE", "Hello world")
     c = get_contract(code, *values)
-    assert c.get_values() == list(values)
+    assert c.get_values() == values
 
 
 def test_struct_immutable(get_contract):
     code = """
 struct MyStruct:
     a: uint256
     b: uint256
@@ -195,15 +194,14 @@
     values = (100, 42, 23230)
     expected_values = [[100, 42, 23230], [42, 100, 23230], [23230, 42, 100]]
     c = get_contract(code, *values)
     assert c.get_my_list() == expected_values
     assert c.get_idx_two() == expected_values[2][2]
 
 
-@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_nested_dynarray_immutable(get_contract):
     code = """
 my_list: immutable(DynArray[DynArray[DynArray[int128, 3], 3], 3])
 
 @deploy
 def __init__(x: int128, y: int128, z: int128):
     my_list = [
@@ -391,15 +389,15 @@
 def fix():
     self.a()
     """
     c = get_contract(code)
     assert c.x() == 2
     assert c.d() == 2
 
-    c.thrash(transact={})
+    c.thrash()
 
     assert c.x() == 2
     assert c.d() == 2 + 5
 
-    c.fix(transact={})
+    c.fix()
     assert c.x() == 2
     assert c.d() == 2
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_init.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_internal_call.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_internal_call.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,35 +4,33 @@
 import pytest
 from hypothesis import given, settings
 
 from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import ArgumentException, CallViolation
 
-pytestmark = pytest.mark.usefixtures("memory_mocker")
 
-
-def test_selfcall_code(get_contract_with_gas_estimation):
+def test_selfcall_code(get_contract):
     selfcall_code = """
 @internal
 def _foo() -> int128:
     return 3
 
 @external
 def bar() -> int128:
     return self._foo()
     """
 
-    c = get_contract_with_gas_estimation(selfcall_code)
+    c = get_contract(selfcall_code)
     assert c.bar() == 3
 
     print("Passed no-argument self-call test")
 
 
-def test_selfcall_code_2(get_contract_with_gas_estimation, keccak):
+def test_selfcall_code_2(get_contract, keccak):
     selfcall_code_2 = """
 @internal
 def _double(x: int128) -> int128:
     return x * 2
 
 @external
 def returnten() -> int128:
@@ -43,15 +41,15 @@
     return keccak256(x)
 
 @external
 def return_hash_of_rzpadded_cow() -> bytes32:
     return self._hashy(0x636f770000000000000000000000000000000000000000000000000000000000)
     """
 
-    c = get_contract_with_gas_estimation(selfcall_code_2)
+    c = get_contract(selfcall_code_2)
     assert c.returnten() == 10
     assert c.return_hash_of_rzpadded_cow() == keccak(b"cow" + b"\x00" * 29)
 
     print("Passed single fixed-size argument self-call test")
 
 
 # test that side-effecting self calls do not get optimized out
@@ -65,18 +63,18 @@
     return self.counter
 @external
 def foo() -> (uint256, uint256):
     x: uint256 = unsafe_mul(self.increment_counter(), 0)
     return x, self.counter
     """
     c = get_contract(code)
-    assert c.foo() == [0, 1]
+    assert c.foo() == (0, 1)
 
 
-def test_selfcall_code_3(get_contract_with_gas_estimation, keccak):
+def test_selfcall_code_3(get_contract, keccak):
     selfcall_code_3 = """
 @internal
 def _hashy2(x: Bytes[100]) -> bytes32:
     return keccak256(x)
 
 @external
 def return_hash_of_cow_x_30() -> bytes32:
@@ -87,22 +85,22 @@
     return len(x)
 
 @external
 def returnten() -> uint256:
     return self._len(b"badminton!")
     """
 
-    c = get_contract_with_gas_estimation(selfcall_code_3)
+    c = get_contract(selfcall_code_3)
     assert c.return_hash_of_cow_x_30() == keccak(b"cow" * 30)
     assert c.returnten() == 10
 
     print("Passed single variable-size argument self-call test")
 
 
-def test_selfcall_code_4(get_contract_with_gas_estimation):
+def test_selfcall_code_4(get_contract):
     selfcall_code_4 = """
 @internal
 def _summy(x: int128, y: int128) -> int128:
     return x + y
 
 @internal
 def _catty(x: Bytes[5], y: Bytes[5]) -> Bytes[10]:
@@ -129,44 +127,44 @@
     return self._slicey1(b"goosedog", 5)
 
 @external
 def return_goose2() -> Bytes[10]:
     return self._slicey2(5, b"goosedog")
     """
 
-    c = get_contract_with_gas_estimation(selfcall_code_4)
+    c = get_contract(selfcall_code_4)
     assert c.returnten() == 10
     assert c.return_mongoose() == b"mongoose"
     assert c.return_goose() == b"goose"
     assert c.return_goose2() == b"goose"
 
     print("Passed multi-argument self-call test")
 
 
-def test_selfcall_code_5(get_contract_with_gas_estimation):
+def test_selfcall_code_5(get_contract):
     selfcall_code_5 = """
 counter: int128
 
 @internal
 def _increment():
     self.counter += 1
 
 @external
 def returnten() -> int128:
     for i: uint256 in range(10):
         self._increment()
     return self.counter
     """
-    c = get_contract_with_gas_estimation(selfcall_code_5)
+    c = get_contract(selfcall_code_5)
     assert c.returnten() == 10
 
     print("Passed self-call statement test")
 
 
-def test_selfcall_code_6(get_contract_with_gas_estimation):
+def test_selfcall_code_6(get_contract):
     selfcall_code_6 = """
 excls: Bytes[32]
 
 @internal
 def _set_excls(arg: Bytes[32]):
     self.excls = arg
 
@@ -180,21 +178,21 @@
 
 @external
 def return_mongoose_revolution_32_excls() -> Bytes[201]:
     self._set_excls(b"!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!")
     return self._hardtest(b"megamongoose123", 4, 8, concat(b"russian revolution", self.excls), 8, 42)
     """
 
-    c = get_contract_with_gas_estimation(selfcall_code_6)
+    c = get_contract(selfcall_code_6)
     assert c.return_mongoose_revolution_32_excls() == b"mongoose_revolution" + b"!" * 32
 
     print("Passed composite self-call test")
 
 
-def test_list_call(get_contract_with_gas_estimation):
+def test_list_call(get_contract):
     code = """
 @internal
 def _foo0(x: int128[2]) -> int128:
     return x[0]
 
 @internal
 def _foo1(x: int128[2]) -> int128:
@@ -217,22 +215,22 @@
 
 @external
 def bar3() -> int128:
     x: int128[2] = [55, 66]
     return self._foo1(x)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bar() == 0
     assert c.foo1([0, 0]) == 0
     assert c.bar2() == 55
     assert c.bar3() == 66
 
 
-def test_list_storage_call(get_contract_with_gas_estimation):
+def test_list_storage_call(get_contract):
     code = """
 y: int128[2]
 
 @internal
 def _foo0(x: int128[2]) -> int128:
     return x[0]
 
@@ -249,21 +247,21 @@
     return self._foo0(self.y)
 
 @external
 def bar1() -> int128:
     return self._foo1(self.y)
     """
 
-    c = get_contract_with_gas_estimation(code)
-    c.set(transact={})
+    c = get_contract(code)
+    c.set()
     assert c.bar0() == 88
     assert c.bar1() == 99
 
 
-def test_multi_arg_list_call(get_contract_with_gas_estimation):
+def test_multi_arg_list_call(get_contract):
     code = """
 @internal
 def _foo0(y: decimal, x: int128[2]) -> int128:
     return x[0]
 
 @internal
 def _foo1(x: int128[2], y: decimal) -> int128:
@@ -318,24 +316,24 @@
 def bar6() -> int128:
     x: int128[2] = [88, 77]
     y: int128[2] = [99, 66]
     return self._foo4(x, y)
 
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bar() == 0
     assert c.foo1([0, 0], decimal_to_int("0")) == 0
     assert c.bar2() == 55
     assert c.bar3() == decimal_to_int("1.33")
     assert c.bar4() == 77
     assert c.bar5() == 88
 
 
-def test_multi_mixed_arg_list_call(get_contract_with_gas_estimation):
+def test_multi_mixed_arg_list_call(get_contract):
     code = """
 @internal
 def _fooz(x: int128[2], y: decimal, z: int128[2], a: decimal) -> int128:
     return z[1]
 
 @internal
 def _fooa(x: int128[2], y: decimal, z: int128[2], a: decimal) -> decimal:
@@ -346,19 +344,19 @@
     x: int128[2] = [33, 44]
     y: decimal = 55.44
     z: int128[2] = [55, 66]
     a: decimal = 66.77
 
     return self._fooz(x, y, z, a), self._fooa(x, y, z, a)
     """
-    c = get_contract_with_gas_estimation(code)
-    assert c.bar() == [66, decimal_to_int("66.77")]
+    c = get_contract(code)
+    assert c.bar() == (66, decimal_to_int("66.77"))
 
 
-def test_internal_function_multiple_lists_as_args(get_contract_with_gas_estimation):
+def test_internal_function_multiple_lists_as_args(get_contract):
     code = """
 @internal
 def _foo(y: int128[2], x: Bytes[5]) -> int128:
     return y[0]
 
 @internal
 def _foo2(x: Bytes[5], y: int128[2]) -> int128:
@@ -369,20 +367,20 @@
     return self._foo([1, 2], b"hello")
 
 @external
 def bar2() -> int128:
     return self._foo2(b"hello", [1, 2])
 """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bar() == 1
     assert c.bar2() == 1
 
 
-def test_multi_mixed_arg_list_bytes_call(get_contract_with_gas_estimation):
+def test_multi_mixed_arg_list_bytes_call(get_contract):
     code = """
 @internal
 def _fooz(x: int128[2], y: decimal, z: Bytes[11], a: decimal) -> Bytes[11]:
     return z
 
 @internal
 def _fooa(x: int128[2], y: decimal, z: Bytes[11], a: decimal) -> decimal:
@@ -398,16 +396,16 @@
     x: int128[2] = [33, 44]
     y: decimal = 55.44
     z: Bytes[11] = b"hello world"
     a: decimal = 66.77
 
     return self._fooz(x, y, z, a), self._fooa(x, y, z, a), self._foox(x, y, z, a)
     """
-    c = get_contract_with_gas_estimation(code)
-    assert c.bar() == [b"hello world", decimal_to_int("66.77"), 44]
+    c = get_contract(code)
+    assert c.bar() == (b"hello world", decimal_to_int("66.77"), 44)
 
 
 FAILING_CONTRACTS_CALL_VIOLATION = [
     """
 # should not compile - public to public
 @external
 def bar() -> int128:
@@ -537,15 +535,15 @@
 def test_selfcall_kwarg_raises(failing_contract_code, decorator, assert_compile_failed):
     exc = ArgumentException if decorator == "internal" else CallViolation
     with pytest.raises(exc):
         _ = compile_code(failing_contract_code.format(decorator))
 
 
 @pytest.mark.parametrize("i,ln,s,", [(100, 6, "abcde"), (41, 40, "a" * 34), (57, 70, "z" * 68)])
-def test_struct_return_1(get_contract_with_gas_estimation, i, ln, s):
+def test_struct_return_1(get_contract, i, ln, s):
     contract = f"""
 struct X:
     x: int128
     y: String[{ln}]
     z: Bytes[{ln}]
 
 @internal
@@ -554,20 +552,20 @@
 
 @external
 def test() -> (int128, String[{ln}], Bytes[{ln}]):
     ret: X = self.get_struct_x()
     return ret.x, ret.y, ret.z
     """
 
-    c = get_contract_with_gas_estimation(contract)
+    c = get_contract(contract)
 
-    assert c.test() == [i, s, bytes(s, "utf-8")]
+    assert c.test() == (i, s, bytes(s, "utf-8"))
 
 
-def test_dynamically_sized_struct_as_arg(get_contract_with_gas_estimation):
+def test_dynamically_sized_struct_as_arg(get_contract):
     contract = """
 struct X:
     x: uint256
     y: Bytes[6]
 
 @internal
 def _foo(x: X) -> Bytes[6]:
@@ -575,20 +573,20 @@
 
 @external
 def bar() -> Bytes[6]:
     _X: X = X(x=1, y=b"hello")
     return self._foo(_X)
     """
 
-    c = get_contract_with_gas_estimation(contract)
+    c = get_contract(contract)
 
     assert c.bar() == b"hello"
 
 
-def test_dynamically_sized_struct_as_arg_2(get_contract_with_gas_estimation):
+def test_dynamically_sized_struct_as_arg_2(get_contract):
     contract = """
 struct X:
     x: uint256
     y: String[6]
 
 @internal
 def _foo(x: X) -> String[6]:
@@ -596,20 +594,20 @@
 
 @external
 def bar() -> String[6]:
     _X: X = X(x=1, y="hello")
     return self._foo(_X)
     """
 
-    c = get_contract_with_gas_estimation(contract)
+    c = get_contract(contract)
 
     assert c.bar() == "hello"
 
 
-def test_dynamically_sized_struct_member_as_arg(get_contract_with_gas_estimation):
+def test_dynamically_sized_struct_member_as_arg(get_contract):
     contract = """
 struct X:
     x: uint256
     y: Bytes[6]
 
 @internal
 def _foo(s: Bytes[6]) -> Bytes[6]:
@@ -617,20 +615,20 @@
 
 @external
 def bar() -> Bytes[6]:
     _X: X = X(x=1, y=b"hello")
     return self._foo(_X.y)
     """
 
-    c = get_contract_with_gas_estimation(contract)
+    c = get_contract(contract)
 
     assert c.bar() == b"hello"
 
 
-def test_dynamically_sized_struct_member_as_arg_2(get_contract_with_gas_estimation):
+def test_dynamically_sized_struct_member_as_arg_2(get_contract):
     contract = """
 struct X:
     x: uint256
     y: String[6]
 
 @internal
 def _foo(s: String[6]) -> String[6]:
@@ -638,15 +636,15 @@
 
 @external
 def bar() -> String[6]:
     _X: X = X(x=1, y="hello")
     return self._foo(_X.y)
     """
 
-    c = get_contract_with_gas_estimation(contract)
+    c = get_contract(contract)
 
     assert c.bar() == "hello"
 
 
 # TODO probably want to refactor these into general test utils
 st_uint256 = st.integers(min_value=0, max_value=2**256 - 1)
 st_string65 = st.text(max_size=65, alphabet=string.printable)
@@ -693,14 +691,14 @@
     return self.foo(x1)
 
 @external
 def test4(x1: {typ1}, x2: {typ2}) -> ({typ1}, {typ2}):
     return self.foo(x1, x2)
         """
         c = get_contract(code)
-        assert c.test0() == [default1, default2]
-        assert c.test1() == [kwarg1, default2]
-        assert c.test2() == [kwarg1, kwarg2]
-        assert c.test3(kwarg1) == [kwarg1, default2]
-        assert c.test4(kwarg1, kwarg2) == [kwarg1, kwarg2]
+        assert c.test0() == (default1, default2)
+        assert c.test1() == (kwarg1, default2)
+        assert c.test2() == (kwarg1, kwarg2)
+        assert c.test3(kwarg1) == (kwarg1, default2)
+        assert c.test4(kwarg1, kwarg2) == (kwarg1, kwarg2)
 
     fuzz()
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_logging_bytes_extended.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_logging_bytes_extended.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,74 @@
-def test_bytes_logging_extended(get_contract_with_gas_estimation, get_logs):
+def test_bytes_logging_extended(get_contract, get_logs):
     code = """
 event MyLog:
     arg1: int128
     arg2: Bytes[64]
     arg3: int128
 
 @external
 def foo():
     log MyLog(667788, b'hellohellohellohellohellohellohellohellohello', 334455)
     """
 
-    c = get_contract_with_gas_estimation(code)
-    log = get_logs(c.foo(transact={}), c, "MyLog")
+    c = get_contract(code)
+    c.foo()
+    (log,) = get_logs(c, "MyLog")
 
-    assert log[0].args.arg1 == 667788
-    assert log[0].args.arg2 == b"hello" * 9
-    assert log[0].args.arg3 == 334455
+    assert log.args.arg1 == 667788
+    assert log.args.arg2 == b"hello" * 9
+    assert log.args.arg3 == 334455
 
 
-def test_bytes_logging_extended_variables(get_contract_with_gas_estimation, get_logs):
+def test_bytes_logging_extended_variables(get_contract, get_logs):
     code = """
 event MyLog:
     arg1: Bytes[64]
     arg2: Bytes[64]
     arg3: Bytes[64]
 
 @external
 def foo():
     a: Bytes[64] = b'hellohellohellohellohellohellohellohellohello'
     b: Bytes[64] = b'hellohellohellohellohellohellohellohello'
     # test literal much smaller than buffer
     log MyLog(a, b, b'hello')
     """
 
-    c = get_contract_with_gas_estimation(code)
-    log = get_logs(c.foo(transact={}), c, "MyLog")
-
-    assert log[0].args.arg1 == b"hello" * 9
-    assert log[0].args.arg2 == b"hello" * 8
-    assert log[0].args.arg3 == b"hello" * 1
+    c = get_contract(code)
+    c.foo()
+    (log,) = get_logs(c, "MyLog")
+    assert log.args.arg1 == b"hello" * 9
+    assert log.args.arg2 == b"hello" * 8
+    assert log.args.arg3 == b"hello" * 1
 
 
-def test_bytes_logging_extended_passthrough(get_contract_with_gas_estimation, get_logs):
+def test_bytes_logging_extended_passthrough(get_contract, get_logs):
     code = """
 event MyLog:
     arg1: int128
     arg2: Bytes[64]
     arg3: int128
 
 @external
 def foo(a: int128, b: Bytes[64], c: int128):
     log MyLog(a, b, c)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
-    log = get_logs(c.foo(333, b"flower" * 8, 444, transact={}), c, "MyLog")
+    c.foo(333, b"flower" * 8, 444)
+    log = get_logs(c, "MyLog")
 
     assert log[0].args.arg1 == 333
     assert log[0].args.arg2 == b"flower" * 8
     assert log[0].args.arg3 == 444
 
 
-def test_bytes_logging_extended_storage(get_contract_with_gas_estimation, get_logs):
+def test_bytes_logging_extended_storage(get_contract, get_logs):
     code = """
 event MyLog:
     arg1: int128
     arg2: Bytes[64]
     arg3: int128
 
 a: int128
@@ -80,32 +82,32 @@
 @external
 def set(x: int128, y: Bytes[64], z: int128):
     self.a = x
     self.b = y
     self.c = z
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     c.foo()
-    log = get_logs(c.foo(transact={}), c, "MyLog")
+    log = get_logs(c, "MyLog")
 
     assert log[0].args.arg1 == 0
     assert log[0].args.arg2 == b""
     assert log[0].args.arg3 == 0
 
-    c.set(333, b"flower" * 8, 444, transact={})
-
-    log = get_logs(c.foo(transact={}), c, "MyLog")[0]
+    c.set(333, b"flower" * 8, 444)
+    c.foo()
 
+    (log,) = get_logs(c, "MyLog")
     assert log.args.arg1 == 333
     assert log.args.arg2 == b"flower" * 8
     assert log.args.arg3 == 444
 
 
-def test_bytes_logging_extended_mixed_with_lists(get_contract_with_gas_estimation, get_logs):
+def test_bytes_logging_extended_mixed_with_lists(get_contract, get_logs):
     code = """
 event MyLog:
     arg1: int128[2][2]
     arg2: Bytes[64]
     arg3: int128
     arg4: Bytes[64]
 
@@ -115,14 +117,15 @@
         [[24, 26], [12, 10]],
         b'hellohellohellohellohellohellohellohellohello',
         314159,
         b'helphelphelphelphelphelphelphelphelphelphelp'
     )
     """
 
-    c = get_contract_with_gas_estimation(code)
-    log = get_logs(c.foo(transact={}), c, "MyLog")[0]
+    c = get_contract(code)
+    c.foo()
+    (log,) = get_logs(c, "MyLog")
 
     assert log.args.arg1 == [[24, 26], [12, 10]]
     assert log.args.arg2 == b"hello" * 9
     assert log.args.arg3 == 314159
     assert log.args.arg4 == b"help" * 11
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_logging_from_call.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_logging_from_call.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import pytest
+from eth_utils import to_int
 
-pytestmark = pytest.mark.usefixtures("memory_mocker")
 
-
-def test_log_dynamic_static_combo(get_logs, get_contract_with_gas_estimation, w3):
+def test_log_dynamic_static_combo(get_logs, get_contract):
     code = """
 event TestLog:
     testData1: bytes32
     testData2: Bytes[60]
     testData3: Bytes[8]
 
 @internal
@@ -26,32 +24,30 @@
     log TestLog(self.to_bytes32(_value), data2, self.to_bytes(_value))
 
     loggedValue: bytes32 = self.to_bytes32(_value)
     loggedValue2: Bytes[8] = self.to_bytes(_value)
     log TestLog(loggedValue, data2, loggedValue2)
     """
 
-    c = get_contract_with_gas_estimation(code)
-
-    tx_hash = c.test_func(123, transact={})
+    c = get_contract(code)
 
-    logs = get_logs(tx_hash, c, "TestLog")
+    c.test_func(123)
+    log, log2 = get_logs(c, "TestLog")
 
-    log = logs[0].args
-    assert w3.to_int(log.testData1) == 123
-    assert w3.to_int(log.testData2[:32]) == 123
-    assert log.testData2[-7:] == b"testing"
-    assert log.testData2[32:] == b"\x00\x00\x00\x00\x00\x00\x00{testing"
-    assert log.testData3 == b"\x00\x00\x00\x00\x00\x00\x00{"
-    assert w3.to_int(log.testData3) == 123
+    assert to_int(log.args.testData1) == 123
+    assert to_int(log.args.testData2[:32]) == 123
+    assert log.args.testData2[-7:] == b"testing"
+    assert log.args.testData2[32:] == b"\x00\x00\x00\x00\x00\x00\x00{testing"
+    assert log.args.testData3 == b"\x00\x00\x00\x00\x00\x00\x00{"
+    assert to_int(log.args.testData3) == 123
 
-    assert logs[0].args == logs[1].args
+    assert log.args == log2.args
 
 
-def test_log_dynamic_static_combo2(get_logs, get_contract, w3):
+def test_log_dynamic_static_combo2(get_logs, get_contract):
     code = """
 event TestLog:
     testData1: bytes32
     testData2: Bytes[133]
     testData3: String[8]
 
 @internal
@@ -71,28 +67,26 @@
 
     # log TestLog(self.to_bytes32(_value),input,self.to_bytes(_value))
     log TestLog(self.to_bytes32(_value),input,"bababa")
     """
 
     c = get_contract(code)
 
-    # assert c.test_func(2**255, b'x' * 129, call={}) == b'x' * 129
-    tx_hash = c.test_func(1234444, b"x" * 129, transact={})
-    tx_receipt = w3.eth.get_transaction_receipt(tx_hash)
-    print(tx_receipt)
-    logs = get_logs(tx_hash, c, "TestLog")
+    # assert c.test_func(2**255, b'x' * 129) == b'x' * 129
+    c.test_func(1234444, b"x" * 129)
+    logs = get_logs(c, "TestLog")
 
     print(logs[0].args)
 
-    assert w3.to_int(logs[0].args.testData1) == 1234444
+    assert to_int(logs[0].args.testData1) == 1234444
     assert logs[0].args.testData3 == "bababa"
     assert logs[0].args.testData2 == b"x" * 129
 
 
-def test_log_single_function_call(get_logs, get_contract, w3):
+def test_log_single_function_call(get_logs, get_contract):
     code = """
 event TestLog:
     testData1: bytes32
     testData2: Bytes[133]
 
 @internal
 @view
@@ -107,22 +101,22 @@
     # log will be malformed
     # log TestLog(self.to_bytes32(_value),input,self.to_bytes(_value))
     log TestLog(self.to_bytes32(_value), input)
     """
 
     c = get_contract(code)
 
-    tx_hash = c.test_func(1234444, b"x" * 129, transact={})
-    logs = get_logs(tx_hash, c, "TestLog")
+    c.test_func(1234444, b"x" * 129)
+    (log,) = get_logs(c, "TestLog")
 
-    assert w3.to_int(logs[0].args.testData1) == 1234444
-    assert logs[0].args.testData2 == b"x" * 129
+    assert to_int(log.args.testData1) == 1234444
+    assert log.args.testData2 == b"x" * 129
 
 
-def test_original_problem_function(get_logs, get_contract, w3):
+def test_original_problem_function(get_logs, get_contract):
     # See #1205 for further details, this is kept as test case as it introduces very specific
     # edge cases to the ABI encoder when logging.
     code = """
 event TestLog:
     testData1: bytes32
     testData2: Bytes[2064]
     testData3: Bytes[8]
@@ -149,22 +143,19 @@
 
     # log will be normal
     log TestLog(self.to_bytes32(_value),data2,loggedValue)
     """
 
     c = get_contract(code)
 
-    tx_hash = c.test_func(333, b"x" * 132, transact={})
-    tx_receipt = w3.eth.get_transaction_receipt(tx_hash)
-    print(tx_receipt)
-    logs = get_logs(tx_hash, c, "TestLog")
-
-    print(logs[0].args)
+    c.test_func(333, b"x" * 132)
+    log1, log2 = get_logs(c, "TestLog")
 
-    assert w3.to_int(logs[0].args.testData1) == 333
+    print(log1.args)
 
-    assert w3.to_int(logs[0].args.testData2[0:8]) == 333
-    assert w3.to_int(logs[0].args.testData2[8:16]) == 333
-    assert logs[0].args.testData2[16:] == b"x" * 132
-    assert w3.to_int(logs[0].args.testData3) == 333
+    assert to_int(log1.args.testData1) == 333
+    assert to_int(log1.args.testData2[0:8]) == 333
+    assert to_int(log1.args.testData2[8:16]) == 333
+    assert log1.args.testData2[16:] == b"x" * 132
+    assert to_int(log1.args.testData3) == 333
 
-    assert logs[0].args == logs[1].args
+    assert log1.args == log2.args
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_memory_dealloc.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_memory_dealloc.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_packing.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_packing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def test_packing_test(get_contract_with_gas_estimation, memory_mocker):
+def test_packing_test(get_contract):
     packing_test = """
 struct Bar:
     a: int128
     b: int128
 struct Z:
     foo: int128[3]
     bar: Bar[2]
@@ -42,11 +42,11 @@
     _z.bar[1].a = 128
     _z.bar[1].b = 256
     _a = 512
     return _x + _y[0] + _y[4] + _z.foo[0] + _z.foo[2] + \
         _z.bar[0].a + _z.bar[0].b + _z.bar[1].a + _z.bar[1].b + _a
     """
 
-    c = get_contract_with_gas_estimation(packing_test)
+    c = get_contract(packing_test)
     assert c.foo() == 1023, c.foo()
     assert c.fop() == 1023, c.fop()
     print("Passed packing test")
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_short_circuiting.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_short_circuiting.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 
 import pytest
 
 
-def test_short_circuit_and_left_is_false(w3, get_contract):
+def test_short_circuit_and_left_is_false(get_contract):
     code = """
 
 called_left: public(bool)
 called_right: public(bool)
 
 @internal
 def left() -> bool:
@@ -22,20 +22,20 @@
 @external
 def foo() -> bool:
     return self.left() and self.right()
 """
     c = get_contract(code)
     assert not c.foo()
 
-    c.foo(transact={})
+    c.foo()
     assert c.called_left()
     assert not c.called_right()
 
 
-def test_short_circuit_and_left_is_true(w3, get_contract):
+def test_short_circuit_and_left_is_true(get_contract):
     code = """
 
 called_left: public(bool)
 called_right: public(bool)
 
 @internal
 def left() -> bool:
@@ -50,20 +50,20 @@
 @external
 def foo() -> bool:
     return self.left() and self.right()
 """
     c = get_contract(code)
     assert c.foo()
 
-    c.foo(transact={})
+    c.foo()
     assert c.called_left()
     assert c.called_right()
 
 
-def test_short_circuit_or_left_is_true(w3, get_contract):
+def test_short_circuit_or_left_is_true(get_contract):
     code = """
 
 called_left: public(bool)
 called_right: public(bool)
 
 @internal
 def left() -> bool:
@@ -78,20 +78,20 @@
 @external
 def foo() -> bool:
     return self.left() or self.right()
 """
     c = get_contract(code)
     assert c.foo()
 
-    c.foo(transact={})
+    c.foo()
     assert c.called_left()
     assert not c.called_right()
 
 
-def test_short_circuit_or_left_is_false(w3, get_contract):
+def test_short_circuit_or_left_is_false(get_contract):
     code = """
 
 called_left: public(bool)
 called_right: public(bool)
 
 @internal
 def left() -> bool:
@@ -106,36 +106,36 @@
 @external
 def foo() -> bool:
     return self.left() or self.right()
 """
     c = get_contract(code)
     assert not c.foo()
 
-    c.foo(transact={})
+    c.foo()
     assert c.called_left()
     assert c.called_right()
 
 
 @pytest.mark.parametrize("op", ["and", "or"])
 @pytest.mark.parametrize("a, b", itertools.product([True, False], repeat=2))
-def test_from_memory(w3, get_contract, a, b, op):
+def test_from_memory(get_contract, a, b, op):
     code = f"""
 @external
 def foo(a: bool, b: bool) -> bool:
     c: bool = a
     d: bool = b
     return c {op} d
 """
     c = get_contract(code)
     assert c.foo(a, b) == eval(f"{a} {op} {b}")
 
 
 @pytest.mark.parametrize("op", ["and", "or"])
 @pytest.mark.parametrize("a, b", itertools.product([True, False], repeat=2))
-def test_from_storage(w3, get_contract, a, b, op):
+def test_from_storage(get_contract, a, b, op):
     code = f"""
 c: bool
 d: bool
 
 @external
 def foo(a: bool, b: bool) -> bool:
     self.c = a
@@ -144,27 +144,27 @@
 """
     c = get_contract(code)
     assert c.foo(a, b) == eval(f"{a} {op} {b}")
 
 
 @pytest.mark.parametrize("op", ["and", "or"])
 @pytest.mark.parametrize("a, b", itertools.product([True, False], repeat=2))
-def test_from_calldata(w3, get_contract, a, b, op):
+def test_from_calldata(get_contract, a, b, op):
     code = f"""
 @external
 def foo(a: bool, b: bool) -> bool:
     return a {op} b
 """
     c = get_contract(code)
     assert c.foo(a, b) == eval(f"{a} {op} {b}")
 
 
 @pytest.mark.parametrize("a, b, c, d", itertools.product([True, False], repeat=4))
 @pytest.mark.parametrize("ops", itertools.product(["and", "or"], repeat=3))
-def test_complex_combination(w3, get_contract, a, b, c, d, ops):
+def test_complex_combination(get_contract, a, b, c, d, ops):
     boolop = f"a {ops[0]} b {ops[1]} c {ops[2]} d"
 
     code = f"""
 @external
 def foo(a: bool, b: bool, c: bool, d: bool) -> bool:
     return {boolop}
 """
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_string_map_keys.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_string_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_ternary.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_ternary.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
 @pytest.mark.parametrize("code", tuple_codes)
 @pytest.mark.parametrize("test", [True, False])
 def test_ternary_tuple(get_contract, code, test):
     c = get_contract(code)
 
     x, y = 1, 2
-    assert c.foo(test, x, y) == ([x, y] if test else [y, x])
+    assert c.foo(test, x, y) == ((x, y) if test else (y, x))
 
 
 @pytest.mark.parametrize("test", [True, False])
 def test_ternary_immutable(get_contract, test):
     code = """
 IMM: public(immutable(uint256))
 @deploy
@@ -265,15 +265,15 @@
 
 @external
 def foo(t: bool):
     self.foo_retval = self.x() if t else self.y()
     """
     c = get_contract(code)
 
-    c.foo(test, transact={})
+    c.foo(test)
     assert c.foo_retval() == (5 if test else 7)
 
     if test:
         assert c.track_taint_x() == 1
         assert c.track_taint_y() == 0
     else:
         assert c.track_taint_x() == 0
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/features/test_transient.py` & `vyper-0.4.0rc3/tests/functional/codegen/features/test_transient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import pytest
 
+from tests.utils import ZERO_ADDRESS
 from vyper.compiler import compile_code
 from vyper.exceptions import EvmVersionException, VyperException
 
 pytestmark = pytest.mark.requires_evm_version("cancun")
 
 
-# with eth-tester, each call happens in an isolated transaction and so we need to
-# test get/set within a single contract call. (we should remove this restriction
-# in the future by migrating away from eth-tester).
 def test_transient_compiles():
     getter_code = """
 my_map: public(transient(HashMap[address, uint256]))
     """
     t = compile_code(getter_code, output_formats=["opcodes_runtime"])
     t = t["opcodes_runtime"].split(" ")
 
@@ -48,41 +46,45 @@
 
 @pytest.mark.parametrize(
     "typ,value,zero",
     [
         ("uint256", 42, 0),
         ("int256", -(2**200), 0),
         ("int128", -(2**126), 0),
-        ("address", "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE", None),
+        ("address", "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE", ZERO_ADDRESS),
         ("bytes32", b"deadbeef" * 4, b"\x00" * 32),
         ("bool", True, False),
         ("String[10]", "Vyper hiss", ""),
         ("Bytes[10]", b"Vyper hiss", b""),
     ],
 )
-def test_value_storage_retrieval(typ, value, zero, get_contract):
+def test_value_storage_retrieval(typ, value, zero, get_contract, env):
     code = f"""
 bar: public(transient({typ}))
 
 @external
 def foo(a: {typ}) -> {typ}:
     self.bar = a
     return self.bar
     """
 
     c = get_contract(code)
     assert c.bar() == zero
     assert c.foo(value) == value
+    env.clear_transient_storage()
+
     assert c.bar() == zero
     assert c.foo(value) == value
+    env.clear_transient_storage()
+
     assert c.bar() == zero
 
 
 @pytest.mark.parametrize("val", [0, 1, 2**256 - 1])
-def test_usage_in_constructor(get_contract, val):
+def test_usage_in_constructor(get_contract, val, env):
     code = """
 A: transient(uint256)
 a: public(uint256)
 
 
 @deploy
 def __init__(_a: uint256):
@@ -94,18 +96,20 @@
 @view
 def a1() -> uint256:
     return self.A
     """
 
     c = get_contract(code, val)
     assert c.a() == val
+    env.clear_transient_storage()
+
     assert c.a1() == 0
 
 
-def test_multiple_transient_values(get_contract):
+def test_multiple_transient_values(get_contract, env):
     code = """
 a: public(transient(uint256))
 b: public(transient(address))
 c: public(transient(String[64]))
 
 @external
 def foo(_a: uint256, _b: address, _c: String[64]) -> (uint256, address, String[64]):
@@ -120,22 +124,24 @@
     except VyperException as e:
         assert e.message.count("EvmVersionException") == 3
         # raise EvmVersionException to satisfy `requires_evm_version` behavior
         raise EvmVersionException()
 
     values = (3, "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE", "Hello world")
     c = get_contract(code)
-    assert c.foo(*values) == list(values)
+    assert c.foo(*values) == values
+    env.clear_transient_storage()
+
     assert c.a() == 0
-    assert c.b() is None
+    assert c.b() == ZERO_ADDRESS
     assert c.c() == ""
-    assert c.foo(*values) == list(values)
+    assert c.foo(*values) == values
 
 
-def test_struct_transient(get_contract):
+def test_struct_transient(get_contract, env):
     code = """
 struct MyStruct:
     a: uint256
     b: uint256
     c: address
     d: int256
 
@@ -151,19 +157,21 @@
     )
     return self.my_struct
     """
     values = (100, 42, "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE", -(2**200))
 
     c = get_contract(code)
     assert c.foo(*values) == values
-    assert c.my_struct() == (0, 0, None, 0)
+    env.clear_transient_storage()
+
+    assert c.my_struct() == (0, 0, ZERO_ADDRESS, 0)
     assert c.foo(*values) == values
 
 
-def test_complex_struct_transient(get_contract):
+def test_complex_struct_transient(get_contract, env):
     code = """
 struct MyStruct:
     a: address
     b: MyStruct2
     c: DynArray[DynArray[uint256, 3], 3]
 
 struct MyStruct2:
@@ -180,19 +188,21 @@
     )
     return self.my_struct
     """
     values = ("0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE", ([1],), [[3, 4], [5, 6]])
 
     c = get_contract(code)
     assert c.foo(*values) == values
-    assert c.my_struct() == (None, ([],), [])
+    env.clear_transient_storage()
+
+    assert c.my_struct() == (ZERO_ADDRESS, ([],), [])
     assert c.foo(*values) == values
 
 
-def test_complex_transient_modifiable(get_contract):
+def test_complex_transient_modifiable(get_contract, env):
     code = """
 struct MyStruct:
     a: uint256
 
 my_struct: public(transient(MyStruct))
 
 @external
@@ -203,53 +213,58 @@
     self.my_struct.a += 1
 
     return self.my_struct
     """
 
     c = get_contract(code)
     assert c.foo(1) == (2,)
+    env.clear_transient_storage()
+
     assert c.my_struct() == (0,)
     assert c.foo(1) == (2,)
 
 
-def test_list_transient(get_contract):
+def test_list_transient(get_contract, env):
     code = """
 my_list: public(transient(uint256[3]))
 
 @external
 def foo(_a: uint256, _b: uint256, _c: uint256) -> uint256[3]:
     self.my_list = [_a, _b, _c]
     return self.my_list
     """
     values = (100, 42, 23230)
 
     c = get_contract(code)
     assert c.foo(*values) == list(values)
+    env.clear_transient_storage()
+
     for i in range(3):
         assert c.my_list(i) == 0
     assert c.foo(*values) == list(values)
 
 
-def test_hashmap_transient(get_contract):
+def test_hashmap_transient(get_contract, env):
     code = """
 my_map: public(transient(HashMap[uint256, uint256]))
 
 @external
 def foo(k: uint256, v: uint256) -> uint256:
     self.my_map[k] = v
     return self.my_map[k]
     """
     c = get_contract(code)
     for v in range(5):
         for k in range(5):
             assert c.foo(k, v) == v
+            env.clear_transient_storage()
             assert c.my_map(k) == 0
 
 
-def test_complex_hashmap_transient(get_contract):
+def test_complex_hashmap_transient(get_contract, env):
     code = """
 struct MyStruct:
     a: uint256
     b: DynArray[uint256, 3]
 
 my_map: public(transient(HashMap[uint256, MyStruct]))
 my_res: public(HashMap[uint256, MyStruct])
@@ -262,25 +277,26 @@
         for j: uint256 in range(3):
             s.b[j] = i + j
         s.a = i
         self.my_map[i] = s
         self.my_res[i] = self.my_map[i]
     """
     c = get_contract(code)
-    c.do_side_effects(transact={})
+    c.do_side_effects()
     for i in range(2):
         assert c.my_res(i)[0] == i
         assert c.my_map(i)[0] == 0
+        env.clear_transient_storage()
+
         for j in range(3):
-            print(c.my_res(i)[1])
             assert c.my_res(i)[1][j] == i + j
             assert c.my_map(i)[1] == []
 
 
-def test_dynarray_transient(get_contract, tx_failed):
+def test_dynarray_transient(get_contract, tx_failed, env):
     code = """
 my_list: public(transient(DynArray[uint256, 3]))
 
 @external
 def get_my_list(_a: uint256, _b: uint256, _c: uint256) -> DynArray[uint256, 3]:
     self.my_list = [_a, _b, _c]
     return self.my_list
@@ -290,17 +306,21 @@
     self.my_list = [_a, _b, _c]
     return self.my_list[2]
     """
     values = (100, 42, 23230)
 
     c = get_contract(code)
     assert c.get_my_list(*values) == list(values)
+    env.clear_transient_storage()
+
     with tx_failed():
         c.my_list(0)
     assert c.get_idx_two(*values) == values[2]
+    env.clear_transient_storage()
+
     with tx_failed():
         c.my_list(0)
 
 
 def test_nested_dynarray_transient_2(get_contract):
     code = """
 my_list: public(transient(DynArray[DynArray[uint256, 3], 3]))
@@ -319,15 +339,15 @@
     expected_values = [[100, 42, 23230], [42, 100, 23230], [23230, 42, 100]]
 
     c = get_contract(code)
     assert c.get_my_list(*values) == expected_values
     assert c.get_idx_two(*values) == expected_values[2][2]
 
 
-def test_nested_dynarray_transient(get_contract, tx_failed):
+def test_nested_dynarray_transient(get_contract, tx_failed, env):
     set_list = """
     self.my_list = [
         [[x, y, z], [y, z, x], [z, y, x]],
         [
             [x * 1000 + y, y * 1000 + z, z * 1000 + x],
             [- (x * 1000 + y), - (y * 1000 + z), - (z * 1000 + x)],
             [- (x * 1000) + y, - (y * 1000) + z, - (z * 1000) + x],
@@ -365,26 +385,32 @@
         [[37, 41, 73], [41, 73, 37], [73, 41, 37]],
         [[37041, 41073, 73037], [-37041, -41073, -73037], [-36959, -40927, -72963]],
         [[146, 123, 148], [-146, -123, -148], [-2993, -1517, -2701]],
     ]
 
     c = get_contract(code)
     assert c.get_my_list(*values) == expected_values
+    env.clear_transient_storage()
+
     with tx_failed():
         c.my_list(0, 0, 0)
     assert c.get_idx_two(*values) == expected_values[2][2][2]
+    env.clear_transient_storage()
+
     with tx_failed():
         c.my_list(0, 0, 0)
     assert c.get_idx_two_using_getter(*values) == expected_values[2][2][2]
+    env.clear_transient_storage()
+
     with tx_failed():
         c.my_list(0, 0, 0)
 
 
 @pytest.mark.parametrize("n", range(5))
-def test_internal_function_with_transient(get_contract, n):
+def test_internal_function_with_transient(get_contract, n, env):
     code = """
 @internal
 def foo() -> uint256:
     self.counter += 1
     return self.counter
 
 counter: uint256
@@ -396,19 +422,21 @@
     self.foo()
     self.val = self.foo()
     return self.val
     """
 
     c = get_contract(code)
     assert c.bar(n) == n + 2
+    env.clear_transient_storage()
+
     assert c.val() == 0
     assert c.bar(n) == n + 2
 
 
-def test_nested_internal_function_transient(get_contract):
+def test_nested_internal_function_transient(get_contract, env):
     code = """
 d: public(uint256)
 x: public(transient(uint256))
 
 @deploy
 def __init__():
     self.d = 1
@@ -422,18 +450,20 @@
 @internal
 def b():
     self.d = self.x
     """
 
     c = get_contract(code)
     assert c.d() == 2
+    env.clear_transient_storage()
+
     assert c.x() == 0
 
 
-def test_view_function_transient(get_contract):
+def test_view_function_transient(get_contract, env):
     c1 = """
 x: transient(uint256)
 
 @external
 def set_x(i: uint256):
     self.x = i
 
@@ -456,14 +486,16 @@
     """
 
     c1 = get_contract(c1)
     c2 = get_contract(c2)
 
     value = 333
     assert c2.bar(value, c1.address) == value
+    env.clear_transient_storage()
+
     assert c1.get_x() == 0
 
 
 def test_modules_transient(get_contract, make_input_bundle):
     lib1 = """
 counter: transient(uint256)
     """
@@ -492,15 +524,15 @@
     lib2.foo()
     lib2.counter = 10
     return lib1.counter, lib2.counter
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     c = get_contract(main, input_bundle=input_bundle)
-    assert c.foo() == [3, 10]
+    assert c.foo() == (3, 10)
 
 
 def test_complex_modules_transient(get_contract, make_input_bundle):
     lib1 = """
 l: transient(uint256[3])
     """
     lib2 = """
@@ -533,8 +565,8 @@
     lib2.foo()
     self.my_map[0] = 42
     return lib1.l, lib2.s.a, lib2.s.b, self.my_map[0]
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
 
     c = get_contract(main, input_bundle=input_bundle)
-    assert c.foo() == [[1, 2, 3], 1, 2, 42]
+    assert c.foo() == ([1, 2, 3], 1, 2, 42)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/integration/test_crowdfund.py` & `vyper-0.4.0rc3/tests/functional/codegen/integration/test_crowdfund.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,18 @@
+import pytest
+
+
+@pytest.fixture(autouse=True)
+def set_balance(env):
+    for a in env.accounts[:7]:
+        env.set_balance(a, 10**10)
+
+
 # TODO: check, this is probably redundant with examples/test_crowdfund.py
-def test_crowdfund(w3, tester, get_contract_with_gas_estimation_for_constants):
+def test_crowdfund(env, get_contract):
     crowdfund = """
 
 struct Funder:
     sender: address
     value: uint256
 funders: HashMap[int128, Funder]
 nextFunderIndex: int128
@@ -58,48 +67,48 @@
             return
         send(self.funders[i].sender, self.funders[i].value)
         self.funders[i].sender = 0x0000000000000000000000000000000000000000
         self.funders[i].value = 0
     self.refundIndex = ind + 30
 
     """
-    a0, a1, a2, a3, a4, a5, a6 = w3.eth.accounts[:7]
+    a0, a1, a2, a3, a4, a5, a6 = env.accounts[:7]
 
-    c = get_contract_with_gas_estimation_for_constants(crowdfund, *[a1, 50, 60])
-    start_timestamp = w3.eth.get_block(w3.eth.block_number).timestamp
+    c = get_contract(crowdfund, *[a1, 50, 60])
+    start_timestamp = env.timestamp
 
-    c.participate(transact={"value": 5})
+    c.participate(value=5)
     assert c.timelimit() == 60
     assert c.deadline() - start_timestamp == 60
     assert not c.expired()
     assert not c.reached()
-    c.participate(transact={"value": 49})
+    c.participate(value=49)
     assert c.reached()
-    pre_bal = w3.eth.get_balance(a1)
-    w3.testing.mine(100)
+    pre_bal = env.get_balance(a1)
+    env.timestamp += 100
     assert c.expired()
-    c.finalize(transact={})
-    post_bal = w3.eth.get_balance(a1)
+    c.finalize()
+    post_bal = env.get_balance(a1)
     assert post_bal - pre_bal == 54
 
-    c = get_contract_with_gas_estimation_for_constants(crowdfund, *[a1, 50, 60])
-    c.participate(transact={"value": 1, "from": a3})
-    c.participate(transact={"value": 2, "from": a4})
-    c.participate(transact={"value": 3, "from": a5})
-    c.participate(transact={"value": 4, "from": a6})
-    w3.testing.mine(100)
+    c = get_contract(crowdfund, *[a1, 50, 60])
+    c.participate(value=1, sender=a3)
+    c.participate(value=2, sender=a4)
+    c.participate(value=3, sender=a5)
+    c.participate(value=4, sender=a6)
+    env.timestamp += 100
     assert c.expired()
     assert not c.reached()
-    pre_bals = [w3.eth.get_balance(x) for x in [a3, a4, a5, a6]]
-    c.refund(transact={})
-    post_bals = [w3.eth.get_balance(x) for x in [a3, a4, a5, a6]]
+    pre_bals = [env.get_balance(x) for x in [a3, a4, a5, a6]]
+    c.refund()
+    post_bals = [env.get_balance(x) for x in [a3, a4, a5, a6]]
     assert [y - x for x, y in zip(pre_bals, post_bals)] == [1, 2, 3, 4]
 
 
-def test_crowdfund2(w3, tester, get_contract_with_gas_estimation_for_constants):
+def test_crowdfund2(env, get_contract):
     crowdfund2 = """
 struct Funder:
     sender: address
     value: uint256
 
 funders: HashMap[int128, Funder]
 nextFunderIndex: int128
@@ -152,36 +161,37 @@
             self.refundIndex = self.nextFunderIndex
             return
         send(self.funders[i].sender, self.funders[i].value)
         self.funders[i] = empty(Funder)
     self.refundIndex = ind + 30
 
     """
-    a0, a1, a2, a3, a4, a5, a6 = w3.eth.accounts[:7]
-    c = get_contract_with_gas_estimation_for_constants(crowdfund2, *[a1, 50, 60])
+    a0, a1, a2, a3, a4, a5, a6 = env.accounts[:7]
+    c = get_contract(crowdfund2, *[a1, 50, 60])
 
-    c.participate(transact={"value": 5})
+    c.participate(value=5)
+    env.timestamp += 1  # make sure auction has started
     assert c.timelimit() == 60
     assert c.deadline() - c.block_timestamp() == 59
     assert not c.expired()
     assert not c.reached()
-    c.participate(transact={"value": 49})
+    c.participate(value=49)
     assert c.reached()
-    pre_bal = w3.eth.get_balance(a1)
-    w3.testing.mine(100)
+    pre_bal = env.get_balance(a1)
+    env.timestamp += 100
     assert c.expired()
-    c.finalize(transact={})
-    post_bal = w3.eth.get_balance(a1)
+    c.finalize()
+    post_bal = env.get_balance(a1)
     assert post_bal - pre_bal == 54
 
-    c = get_contract_with_gas_estimation_for_constants(crowdfund2, *[a1, 50, 60])
-    c.participate(transact={"value": 1, "from": a3})
-    c.participate(transact={"value": 2, "from": a4})
-    c.participate(transact={"value": 3, "from": a5})
-    c.participate(transact={"value": 4, "from": a6})
-    w3.testing.mine(100)
+    c = get_contract(crowdfund2, *[a1, 50, 60])
+    c.participate(value=1, sender=a3)
+    c.participate(value=2, sender=a4)
+    c.participate(value=3, sender=a5)
+    c.participate(value=4, sender=a6)
+    env.timestamp += 100
     assert c.expired()
     assert not c.reached()
-    pre_bals = [w3.eth.get_balance(x) for x in [a3, a4, a5, a6]]
-    c.refund(transact={})
-    post_bals = [w3.eth.get_balance(x) for x in [a3, a4, a5, a6]]
+    pre_bals = [env.get_balance(x) for x in [a3, a4, a5, a6]]
+    c.refund()
+    post_bals = [env.get_balance(x) for x in [a3, a4, a5, a6]]
     assert [y - x for x, y in zip(pre_bals, post_bals)] == [1, 2, 3, 4]
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/modules/test_events.py` & `vyper-0.4.0rc3/tests/functional/codegen/modules/test_events.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 @external
 def bar():
     lib1.foo()
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1})
     c = get_contract(main, input_bundle=input_bundle)
-    logs = get_logs(c.bar(transact={}), c, "MyEvent")
+    c.bar()
+    logs = get_logs(c, "MyEvent")
     assert len(logs) == 1
 
 
 def test_module_event2(get_contract, make_input_bundle, get_logs):
     # log a module event from main contract
     lib1 = """
 event MyEvent:
@@ -32,17 +33,17 @@
 
 @external
 def bar():
     log lib1.MyEvent(5)
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1})
     c = get_contract(main, input_bundle=input_bundle)
-    logs = get_logs(c.bar(transact={}), c, "MyEvent")
-    assert len(logs) == 1
-    assert logs[0].args.x == 5
+    c.bar()
+    (log,) = get_logs(c, "MyEvent")
+    assert log.args.x == 5
 
 
 def test_module_event_indexed(get_contract, make_input_bundle, get_logs):
     lib1 = """
 event MyEvent:
     x: uint256
     y: indexed(uint256)
@@ -56,11 +57,11 @@
 
 @external
 def bar():
     lib1.foo()
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1})
     c = get_contract(main, input_bundle=input_bundle)
-    logs = get_logs(c.bar(transact={}), c, "MyEvent")
-    assert len(logs) == 1
-    assert logs[0].args.x == 5
-    assert logs[0].args.y == 6
+    c.bar()
+    (log,) = get_logs(c, "MyEvent")
+    assert log.args.x == 5
+    assert log.args.y == 6
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/modules/test_exports.py` & `vyper-0.4.0rc3/tests/functional/codegen/modules/test_exports.py`

 * *Files 6% similar despite different names*

```diff
@@ -194,19 +194,19 @@
 def qux() -> uint256:
     return 3
     """
     return make_input_bundle({"lib1.vy": lib1, "ifoo.vyi": ifoo, "ibar.vyi": ibar})
 
 
 @pytest.fixture
-def send_failing_tx_to_signature(w3, tx_failed):
+def send_failing_tx_to_signature(env, tx_failed):
     def _send_transaction(c, method_sig):
         data = method_id(method_sig)
         with tx_failed():
-            w3.eth.send_transaction({"to": c.address, "data": data})
+            env.message_call(c.address, data=data)
 
     return _send_transaction
 
 
 def test_exports_interface_simple(get_contract, simple_library):
     main = """
 import lib1
@@ -403,19 +403,19 @@
 @deploy
 def __init__():
     lib1.counter = 100
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1})
     c = get_contract(main, input_bundle=input_bundle)
     assert c.counter() == 100
-    c.foo(transact={})
+    c.foo()
     assert c.counter() == 101
 
 
-def test_export_module_with_default(w3, get_contract, make_input_bundle):
+def test_export_module_with_default(env, get_contract, make_input_bundle):
     lib1 = """
 counter: public(uint256)
 
 @external
 def foo() -> uint256:
     return 1
 
@@ -434,9 +434,9 @@
 exports: lib1.__interface__
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1})
     c = get_contract(main, input_bundle=input_bundle)
     assert c.foo() == 1
     assert c.counter() == 5
     # call `c.__default__()`
-    w3.eth.send_transaction({"to": c.address})
+    env.message_call(c.address)
     assert c.counter() == 6
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/modules/test_flag_imports.py` & `vyper-0.4.0rc3/tests/functional/codegen/modules/test_flag_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/modules/test_module_constants.py` & `vyper-0.4.0rc3/tests/functional/codegen/modules/test_module_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/modules/test_module_variables.py` & `vyper-0.4.0rc3/tests/functional/codegen/modules/test_module_variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """
 
     input_bundle = make_input_bundle({"lib.vy": lib1})
 
     c = get_contract(contract, input_bundle=input_bundle)
 
     assert c.get_counter() == 0
-    c.increment_counter(transact={})
+    c.increment_counter()
     assert c.get_counter() == 1
 
 
 def test_import_namespace(get_contract, make_input_bundle):
     # test what happens when things in current and imported modules share names
     lib = """
 counter: uint256
@@ -71,23 +71,23 @@
 
     input_bundle = make_input_bundle({"library.vy": lib})
 
     c = get_contract(contract, input_bundle=input_bundle)
 
     assert c.get_counter() == c.get_lib_counter() == 0
 
-    c.increment_counter(transact={})
+    c.increment_counter()
     assert c.get_counter() == 1
     assert c.get_lib_counter() == 0
 
-    c.increment_lib_counter(transact={})
+    c.increment_lib_counter()
     assert c.get_lib_counter() == 1
     assert c.get_counter() == 1
 
-    c.increment_lib_counter2(transact={})
+    c.increment_lib_counter2()
     assert c.get_lib_counter() == 6
     assert c.get_counter() == 1
 
 
 def test_init_function_side_effects(get_contract, make_input_bundle):
     lib = """
 counter: uint256
@@ -306,13 +306,13 @@
 
     input_bundle = make_input_bundle({"lib.vy": lib1})
 
     c = get_contract(contract, input_bundle=input_bundle)
 
     assert c.get_array_value(0) == 0
     assert c.get_hashmap_value(0) == 0
-    c.do_things(transact={})
+    c.do_things()
 
     assert c.get_array_value(0) == 0
     assert c.get_hashmap_value(0) == 0
     assert c.get_array_value(1) == 5
     assert c.get_hashmap_value(6) == 100
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/modules/test_nonreentrant.py` & `vyper-0.4.0rc3/tests/functional/codegen/modules/test_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/modules/test_stateless_functions.py` & `vyper-0.4.0rc3/tests/functional/codegen/modules/test_stateless_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     StructureException,
     TypeMismatch,
 )
 
 # test modules which have no variables - "libraries"
 
 
-def test_simple_library(get_contract, make_input_bundle, w3):
+def test_simple_library(get_contract, make_input_bundle, env):
     library_source = """
 @internal
 def foo() -> uint256:
     return block.number + 1
     """
     main = """
 import library
@@ -27,15 +27,15 @@
 def bar() -> uint256:
     return library.foo() - 1
     """
     input_bundle = make_input_bundle({"library.vy": library_source})
 
     c = get_contract(main, input_bundle=input_bundle)
 
-    assert c.bar() == w3.eth.block_number
+    assert c.bar() == env.block_number
 
 
 # is this the best place for this?
 def test_import_cycle(make_input_bundle):
     code_a = "import b\n"
     code_b = "import a\n"
 
@@ -175,15 +175,15 @@
 @external
 def qux() -> library.SomeStruct:
     return library.foo()
     """
     input_bundle = make_input_bundle({"library.vy": library_source, "contract.vy": contract_source})
     c = get_contract(contract_source, input_bundle=input_bundle)
 
-    assert c.bar((1,)) == []
+    assert c.bar((1,)) is None
 
     assert c.baz() == (2,)
     assert c.qux() == (1,)
 
 
 # test calls to library functions in statement position
 def test_library_statement_calls(get_contract, make_input_bundle, tx_failed):
@@ -203,15 +203,15 @@
     library.check_adds_to_ten(3, x)
     self.counter = x
     """
     input_bundle = make_input_bundle({"library.vy": library_source, "contract.vy": contract_source})
 
     c = get_contract(contract_source, input_bundle=input_bundle)
 
-    c.foo(7, transact={})
+    c.foo(7)
 
     assert c.counter() == 7
 
     with tx_failed():
         c.foo(8)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_getters.py` & `vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_getters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-def test_state_accessor(get_contract_with_gas_estimation_for_constants):
+def test_state_accessor(get_contract):
     state_accessor = """
 y: HashMap[int128, int128]
 
 @external
 def oo():
     self.y[3] = 5
 
 @external
 def foo() -> int128:
     return self.y[3]
 
     """
 
-    c = get_contract_with_gas_estimation_for_constants(state_accessor)
-    c.oo(transact={})
+    c = get_contract(state_accessor)
+    c.oo()
     assert c.foo() == 5
 
 
-def test_getter_code(get_contract_with_gas_estimation_for_constants):
+def test_getter_code(get_contract):
     getter_code = """
 interface V:
     def foo(): nonpayable
 
 struct W:
     a: uint256
     b: int128[7]
@@ -54,15 +54,15 @@
     self.w[3].g = 751
     self.a[1][4] = 666
     self.b[42][self] = [5,6,7,8]
     d = 1729
     e = [2, 3]
     """
 
-    c = get_contract_with_gas_estimation_for_constants(getter_code)
+    c = get_contract(getter_code)
     assert c.x() == 7
     assert c.y(1) == 9
     assert c.z() == b"cow"
     assert c.w(1)[0] == 11  # W.a
     assert c.w(1)[1][2] == 13  # W.b[2]
     assert c.w(1)[2] == b"horse"  # W.c
     assert c.w(2)[3][1][2] == 17  # W.e[1][2]
@@ -90,11 +90,11 @@
 @deploy
 def __init__():
     kune = 2
 """
 
     contract = get_contract(code)
 
-    for item in contract._classic_contract.abi:
+    for item in contract.abi:
         if item["type"] == "constructor":
             continue
         assert item["stateMutability"] == "view"
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_setters.py` & `vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_setters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from vyper.exceptions import InvalidAttribute
 
 
-def test_multi_setter_test(get_contract_with_gas_estimation):
+def test_multi_setter_test(get_contract):
     multi_setter_test = """
 dog: int128[3]
 bar: int128[3][3]
 @external
 def foo() -> int128:
     self.dog = [1, 2, 3]
     return(self.dog[0] + self.dog[1] * 10 + self.dog[2] * 100)
@@ -50,29 +50,29 @@
     gar: int128[3][3] = [[1, 2, 3], [4, 5, 6], [0, 0, 0]]
     gar[1] = empty(int128[3])
     return gar[0][0] + gar[0][1] * 10 + gar[0][2] * 100 + \
         gar[1][0] * 1000 + gar[1][1] * 10000 + gar[1][2] * 100000
 
     """
 
-    c = get_contract_with_gas_estimation(multi_setter_test)
+    c = get_contract(multi_setter_test)
     assert c.foo() == 321
-    c.foo(transact={})
+    c.foo()
     assert c.fop() == 654321
-    c.fop(transact={})
+    c.fop()
     assert c.goo() == 321
     assert c.gop() == 654321
     assert c.hoo() == 0
     assert c.hop() == 321
     assert c.joo() == 0
     assert c.jop() == 321
     print("Passed multi-setter literal test")
 
 
-def test_multi_setter_struct_test(get_contract_with_gas_estimation):
+def test_multi_setter_struct_test(get_contract):
     multi_setter_struct_test = """
 struct Dog:
     foo: int128
     bar: int128
 struct Bar:
     a: int128
     b: int128
@@ -137,15 +137,15 @@
         zed[1].foo[2] * 1000000000 + \
         zed[1].bar[0].a * 10000000000 + \
         zed[1].bar[0].b * 100000000000 + \
         zed[1].bar[1].a * 1000000000000 + \
         zed[1].bar[1].b * 10000000000000
     """
 
-    c = get_contract_with_gas_estimation(multi_setter_struct_test)
+    c = get_contract(multi_setter_struct_test)
     assert c.foo() == 654321
     assert c.fop() == 87198763254321
     assert c.goo() == 654321
     assert c.gop() == 87198763254321
 
 
 def test_struct_assignment_order(get_contract, assert_compile_failed):
@@ -159,33 +159,33 @@
 def test2() -> uint256:
     foo: Foo = Foo(b=2, a=297)
     return foo.a
     """
     assert_compile_failed(lambda: get_contract(code), InvalidAttribute)
 
 
-def test_type_converter_setter_test(get_contract_with_gas_estimation):
+def test_type_converter_setter_test(get_contract):
     type_converter_setter_test = """
 pap: decimal[2][2]
 
 @external
 def goo() -> int256:
     self.pap = [[1.0, 2.0], [3.0, 4.0]]
     return floor(
         self.pap[0][0] +
         self.pap[0][1] * 10.0 +
         self.pap[1][0] * 100.0 +
         self.pap[1][1] * 1000.0)
     """
 
-    c = get_contract_with_gas_estimation(type_converter_setter_test)
+    c = get_contract(type_converter_setter_test)
     assert c.goo() == 4321
 
 
-def test_composite_setter_test(get_contract_with_gas_estimation):
+def test_composite_setter_test(get_contract):
     composite_setter_test = """
 struct C:
     c: int128
 struct Mom:
     a: C[3]
     b: int128
 mom: Mom
@@ -213,11 +213,11 @@
 def foq() -> int128:
     popp: Mom = Mom(a=[C(c=1), C(c=2), C(c=3)], b=4)
     popp.a[0] = empty(C)
     popp.a[2] = empty(C)
     return popp.a[0].c + popp.a[1].c * 10 + popp.a[2].c * 100 + popp.b * 1000
     """
 
-    c = get_contract_with_gas_estimation(composite_setter_test)
+    c = get_contract(composite_setter_test)
     assert c.foo() == 4625
     assert c.fop() == 4625
     assert c.foq() == 4020
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/storage_variables/test_storage_variable.py` & `vyper-0.4.0rc3/tests/functional/codegen/storage_variables/test_storage_variable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pytest import raises
 
 from vyper.exceptions import UndeclaredDefinition
 
 
-def test_permanent_variables_test(get_contract_with_gas_estimation):
+def test_permanent_variables_test(get_contract):
     permanent_variables_test = """
 struct Var:
     a: int128
     b: int128
 var: Var
 
 @deploy
@@ -16,15 +16,15 @@
     self.var.b = b
 
 @external
 def returnMoose() -> int128:
     return self.var.a * 10 + self.var.b
     """
 
-    c = get_contract_with_gas_estimation(permanent_variables_test, *[5, 7])
+    c = get_contract(permanent_variables_test, *[5, 7])
     assert c.returnMoose() == 57
     print("Passed init argument and variable member test")
 
 
 def test_missing_global(get_contract):
     code = """
 @external
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/test_call_graph_stability.py` & `vyper-0.4.0rc3/tests/functional/codegen/test_call_graph_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/test_interfaces.py` & `vyper-0.4.0rc3/tests/functional/codegen/test_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 
 import pytest
+from eth_utils import to_wei
 
 from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import (
     ArgumentException,
     DuplicateImport,
     InterfaceViolation,
@@ -181,15 +182,15 @@
     code, exception_type, assert_compile_failed, make_input_bundle
 ):
     input_bundle = make_input_bundle({"a.vyi": "", "b/a.vyi": "", "c.vyi": ""})
     with pytest.raises(exception_type):
         compile_code(code, input_bundle=input_bundle)
 
 
-def test_external_call_to_interface(w3, get_contract, make_input_bundle):
+def test_external_call_to_interface(env, get_contract, make_input_bundle):
     token_interface = """
 @view
 @external
 def balanceOf(addr: address) -> uint256:
     ...
 
 @external
@@ -228,18 +229,18 @@
     extcall self.token_address.transfer(msg.sender, 1000)
     """
 
     token = get_contract(token_code, input_bundle=input_bundle)
 
     test_c = get_contract(code, *[token.address], input_bundle=input_bundle)
 
-    sender = w3.eth.accounts[0]
+    sender = env.deployer
     assert token.balanceOf(sender) == 0
 
-    test_c.test(transact={})
+    test_c.test()
     assert token.balanceOf(sender) == 1000
 
 
 @pytest.mark.parametrize(
     "kwarg,typ,expected",
     [
         ("max_value(uint256)", "uint256", 2**256 - 1),
@@ -275,20 +276,20 @@
 @external
 @view
 def bar(a_address: address) -> {typ}:
     return staticcall IContract(a_address).foo()
     """
 
     contract_a = get_contract(code1, input_bundle=input_bundle)
-    contract_b = get_contract(code2, *[contract_a.address], input_bundle=input_bundle)
+    contract_b = get_contract(code2, input_bundle=input_bundle)
 
     assert contract_b.bar(contract_a.address) == expected
 
 
-def test_external_call_to_builtin_interface(w3, get_contract):
+def test_external_call_to_builtin_interface(env, get_contract):
     token_code = """
 balanceOf: public(HashMap[address, uint256])
 
 @external
 def transfer(to: address, amount: uint256) -> bool:
     self.balanceOf[to] += amount
     return True
@@ -307,35 +308,35 @@
 def test():
     extcall self.token_address.transfer(msg.sender, 1000)
     """
 
     erc20 = get_contract(token_code)
     test_c = get_contract(code, *[erc20.address])
 
-    sender = w3.eth.accounts[0]
+    sender = env.deployer
     assert erc20.balanceOf(sender) == 0
 
-    test_c.test(transact={})
+    test_c.test()
     assert erc20.balanceOf(sender) == 1000
 
 
-def test_address_member(w3, get_contract):
+def test_address_member(env, get_contract):
     code = """
 interface Foo:
     def foo(): payable
 
 f: Foo
 
 @external
 def test(addr: address):
     self.f = Foo(addr)
     assert self.f.address == addr
     """
     c = get_contract(code)
-    for address in w3.eth.accounts:
+    for address in env.accounts:
         c.test(address)
 
 
 # test data returned from external interface gets clamped
 @pytest.mark.parametrize("typ", ("int128", "uint8"))
 def test_external_interface_int_clampers(get_contract, tx_failed, typ):
     external_contract = f"""
@@ -499,15 +500,15 @@
         c.test_fail1()
     with tx_failed():
         c.test_fail2()
     with tx_failed():
         c.test_fail3()
 
 
-def test_units_interface(w3, get_contract, make_input_bundle):
+def test_units_interface(env, get_contract, make_input_bundle):
     code = """
 import balanceof as BalanceOf
 
 implements: BalanceOf
 
 @external
 @view
@@ -522,15 +523,15 @@
     ...
     """
 
     input_bundle = make_input_bundle({"balanceof.vyi": interface_code})
 
     c = get_contract(code, input_bundle=input_bundle)
 
-    assert c.balanceOf(w3.eth.accounts[0]) == w3.to_wei(1, "ether")
+    assert c.balanceOf(env.deployer) == to_wei(1, "ether")
 
 
 def test_simple_implements(make_input_bundle):
     interface_code = """
 @external
 def foo() -> uint256:
     ...
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/test_selector_table.py` & `vyper-0.4.0rc3/tests/functional/codegen/test_selector_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -508,15 +508,15 @@
     )
 
 
 @pytest.mark.parametrize("opt_level", list(OptimizationLevel))
 # dense selector table packing boundaries at 256 and 65336
 @pytest.mark.parametrize("max_calldata_bytes", [255, 256, 65336])
 @pytest.mark.fuzzing
-def test_selector_table_fuzz(max_calldata_bytes, opt_level, w3, get_contract, tx_failed, get_logs):
+def test_selector_table_fuzz(max_calldata_bytes, opt_level, env, get_contract, tx_failed, get_logs):
     def abi_sig(func_id, calldata_words, n_default_args):
         params = [] if not calldata_words else [f"uint256[{calldata_words}]"]
         params.extend(["uint256"] * n_default_args)
         paramstr = ",".join(params)
         return f"foo{func_id}({paramstr})"
 
     def generate_func_def(func_id, mutability, calldata_words, n_default_args):
@@ -570,14 +570,15 @@
 
 {func_defs}
 
 {default_fn_code}
         """
 
         c = get_contract(code, override_opt_level=opt_level)
+        env.set_balance(env.deployer, 10**18)
 
         for func_id, mutability, n_calldata_words, n_strip_bytes, n_default_args in methods:
             funcname = f"foo{func_id}"
             func = getattr(c, funcname)
 
             for j in range(n_default_args + 1):
                 args = [[1] * n_calldata_words] if n_calldata_words else []
@@ -588,50 +589,49 @@
 
                 method_id = utils.method_id(abi_sig(func_id, n_calldata_words, j))
 
                 argsdata = b"\x00" * (n_calldata_words * 32 + j * 32)
 
                 # do payable check
                 if mutability == "@payable":
-                    tx = func(*args, transact={"value": 1})
-                    (event,) = get_logs(tx, c, "_Return")
+                    func(*args, value=1)
+                    (event,) = get_logs(c, "_Return")
                     assert event.args.val == func_id
                 else:
                     hexstr = (method_id + argsdata).hex()
-                    txdata = {"to": c.address, "data": hexstr, "value": 1}
                     with tx_failed():
-                        w3.eth.send_transaction(txdata)
+                        env.message_call(c.address, data=hexstr, value=1)
 
                 # now do calldatasize check
                 # strip some bytes
                 calldata = (method_id + argsdata)[:-n_strip_bytes]
                 hexstr = calldata.hex()
                 tx_params = {"to": c.address, "data": hexstr}
                 if n_calldata_words == 0 and j == 0:
                     # no args, hit default function
                     if default_fn_mutability == "":
                         with tx_failed():
-                            w3.eth.send_transaction(tx_params)
+                            env.message_call(**tx_params)
                     elif default_fn_mutability == "@payable":
                         # we should be able to send eth to it
                         tx_params["value"] = 1
-                        tx = w3.eth.send_transaction(tx_params)
-                        logs = get_logs(tx, c, "CalledDefault")
+                        env.message_call(**tx_params)
+                        logs = get_logs(c, "CalledDefault")
                         assert len(logs) == 1
                     else:
-                        tx = w3.eth.send_transaction(tx_params)
+                        env.message_call(**tx_params)
 
                         # note: can't emit logs from view/pure functions,
                         # so the logging is not tested.
                         if default_fn_mutability == "@nonpayable":
-                            logs = get_logs(tx, c, "CalledDefault")
+                            logs = get_logs(c, "CalledDefault")
                             assert len(logs) == 1
 
                         # check default function reverts
                         tx_params["value"] = 1
                         with tx_failed():
-                            w3.eth.send_transaction(tx_params)
+                            env.message_call(**tx_params)
                 else:
                     with tx_failed():
-                        w3.eth.send_transaction(tx_params)
+                        env.message_call(**tx_params)
 
     _test()
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/test_selector_table_stability.py` & `vyper-0.4.0rc3/tests/functional/codegen/test_selector_table_stability.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     output = compile_code(
         code, output_formats=["asm"], settings=Settings(optimize=OptimizationLevel.CODESIZE)
     )
 
     # test that the selector table data is stable across different runs
     # (xdist should provide different PYTHONHASHSEEDs).
-    expected_asm = """{ DATA _sym_BUCKET_HEADERS b\'\\x0bB\' _sym_bucket_0 b\'\\n\' b\'+\\x8d\' _sym_bucket_1 b\'\\x0c\' b\'\\x00\\x85\' _sym_bucket_2 b\'\\x08\' } { DATA _sym_bucket_1 b\'\\xd8\\xee\\xa1\\xe8\' _sym_external 6 foo6()3639517672 b\'\\x05\' b\'\\xd2\\x9e\\xe0\\xf9\' _sym_external 0 foo0()3533627641 b\'\\x05\' b\'\\x05\\xf1\\xe0_\' _sym_external 2 foo2()99737695 b\'\\x05\' b\'\\x91\\t\\xb4{\' _sym_external 23 foo23()2433332347 b\'\\x05\' b\'np3\\x7f\' _sym_external 11 foo11()1852846975 b\'\\x05\' b\'&\\xf5\\x96\\xf9\' _sym_external 13 foo13()653629177 b\'\\x05\' b\'\\x04ga\\xeb\' _sym_external 14 foo14()73884139 b\'\\x05\' b\'\\x89\\x06\\xad\\xc6\' _sym_external 17 foo17()2298916294 b\'\\x05\' b\'\\xe4%\\xac\\xd1\' _sym_external 4 foo4()3827674321 b\'\\x05\' b\'yj\\x01\\xac\' _sym_external 7 foo7()2036990380 b\'\\x05\' b\'\\xf1\\xe6K\\xe5\' _sym_external 29 foo29()4058401765 b\'\\x05\' b\'\\xd2\\x89X\\xb8\' _sym_external 3 foo3()3532216504 b\'\\x05\' } { DATA _sym_bucket_2 b\'\\x06p\\xffj\' _sym_external 25 foo25()108068714 b\'\\x05\' b\'\\x964\\x99I\' _sym_external 24 foo24()2520029513 b\'\\x05\' b\'s\\x81\\xe7\\xc1\' _sym_external 10 foo10()1937893313 b\'\\x05\' b\'\\x85\\xad\\xc11\' _sym_external 28 foo28()2242756913 b\'\\x05\' b\'\\xfa"\\xb1\\xed\' _sym_external 5 foo5()4196577773 b\'\\x05\' b\'A\\xe7[\\x05\' _sym_external 22 foo22()1105681157 b\'\\x05\' b\'\\xd3\\x89U\\xe8\' _sym_external 1 foo1()3548993000 b\'\\x05\' b\'hL\\xf8\\xf3\' _sym_external 20 foo20()1749874931 b\'\\x05\' } { DATA _sym_bucket_0 b\'\\xee\\xd9\\x1d\\xe3\' _sym_external 9 foo9()4007206371 b\'\\x05\' b\'a\\xbc\\x1ch\' _sym_external 16 foo16()1639717992 b\'\\x05\' b\'\\xd3*\\xa7\\x0c\' _sym_external 21 foo21()3542787852 b\'\\x05\' b\'\\x18iG\\xd9\' _sym_external 19 foo19()409552857 b\'\\x05\' b\'\\n\\xf1\\xf9\\x7f\' _sym_external 18 foo18()183630207 b\'\\x05\' b\')\\xda\\xd7`\' _sym_external 27 foo27()702207840 b\'\\x05\' b\'2\\xf6\\xaa\\xda\' _sym_external 12 foo12()855026394 b\'\\x05\' b\'\\xbe\\xb5\\x05\\xf5\' _sym_external 15 foo15()3199534581 b\'\\x05\' b\'\\xfc\\xa7_\\xe6\' _sym_external 8 foo8()4238827494 b\'\\x05\' b\'\\x1b\\x12C8\' _sym_external 26 foo26()454181688 b\'\\x05\' } }"""  # noqa: E501
+    expected_asm = """{ DATA _sym_BUCKET_HEADERS b\'\\x0bB\' _sym_bucket_0 b\'\\n\' b\'+\\x8d\' _sym_bucket_1 b\'\\x0c\' b\'\\x00\\x85\' _sym_bucket_2 b\'\\x08\' } { DATA _sym_bucket_1 b\'\\xd8\\xee\\xa1\\xe8\' _sym_external 6 foo6()3639517672 b\'\\x05\' b\'\\xd2\\x9e\\xe0\\xf9\' _sym_external 0 foo0()3533627641 b\'\\x05\' b\'\\x05\\xf1\\xe0_\' _sym_external 2 foo2()99737695 b\'\\x05\' b\'\\x91\\t\\xb4{\' _sym_external 23 foo23()2433332347 b\'\\x05\' b\'np3\\x7f\' _sym_external 11 foo11()1852846975 b\'\\x05\' b\'&\\xf5\\x96\\xf9\' _sym_external 13 foo13()653629177 b\'\\x05\' b\'\\x04ga\\xeb\' _sym_external 14 foo14()73884139 b\'\\x05\' b\'\\x89\\x06\\xad\\xc6\' _sym_external 17 foo17()2298916294 b\'\\x05\' b\'\\xe4%\\xac\\xd1\' _sym_external 4 foo4()3827674321 b\'\\x05\' b\'yj\\x01\\xac\' _sym_external 7 foo7()2036990380 b\'\\x05\' b\'\\xf1\\xe6K\\xe5\' _sym_external 29 foo29()4058401765 b\'\\x05\' b\'\\xd2\\x89X\\xb8\' _sym_external 3 foo3()3532216504 b\'\\x05\' } { DATA _sym_bucket_2 b\'\\x06p\\xffj\' _sym_external 25 foo25()108068714 b\'\\x05\' b\'\\x964\\x99I\' _sym_external 24 foo24()2520029513 b\'\\x05\' b\'s\\x81\\xe7\\xc1\' _sym_external 10 foo10()1937893313 b\'\\x05\' b\'\\x85\\xad\\xc11\' _sym_external 28 foo28()2242756913 b\'\\x05\' b\'\\xfa"\\xb1\\xed\' _sym_external 5 foo5()4196577773 b\'\\x05\' b\'A\\xe7[\\x05\' _sym_external 22 foo22()1105681157 b\'\\x05\' b\'\\xd3\\x89U\\xe8\' _sym_external 1 foo1()3548993000 b\'\\x05\' b\'hL\\xf8\\xf3\' _sym_external 20 foo20()1749874931 b\'\\x05\' } { DATA _sym_bucket_0 b\'\\xee\\xd9\\x1d\\xe3\' _sym_external 9 foo9()4007206371 b\'\\x05\' b\'a\\xbc\\x1ch\' _sym_external 16 foo16()1639717992 b\'\\x05\' b\'\\xd3*\\xa7\\x0c\' _sym_external 21 foo21()3542787852 b\'\\x05\' b\'\\x18iG\\xd9\' _sym_external 19 foo19()409552857 b\'\\x05\' b\'\\n\\xf1\\xf9\\x7f\' _sym_external 18 foo18()183630207 b\'\\x05\' b\')\\xda\\xd7`\' _sym_external 27 foo27()702207840 b\'\\x05\' b\'2\\xf6\\xaa\\xda\' _sym_external 12 foo12()855026394 b\'\\x05\' b\'\\xbe\\xb5\\x05\\xf5\' _sym_external 15 foo15()3199534581 b\'\\x05\' b\'\\xfc\\xa7_\\xe6\' _sym_external 8 foo8()4238827494 b\'\\x05\' b\'\\x1b\\x12C8\' _sym_external 26 foo26()454181688 b\'\\x05\' } }"""  # noqa: E501, FS003
     assert expected_asm in output["asm"]
 
 
 def test_sparse_jumptable_stability():
     function_names = [f"foo{i}()" for i in range(30)]
 
     # sparse jumptable is not as complicated in assembly.
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_constants.py` & `vyper-0.4.0rc3/tests/functional/codegen/calling_convention/test_default_function.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,245 +1,234 @@
-import itertools
+from eth_utils import to_wei
 
-import pytest
 
-from tests.utils import decimal_to_int
-from vyper.compiler import compile_code
-from vyper.exceptions import TypeMismatch
-from vyper.utils import MemoryPositions
+def test_throw_on_sending(env, tx_failed, get_contract):
+    code = """
+x: public(int128)
 
+@deploy
+def __init__():
+    self.x = 123
+    """
+    c = get_contract(code)
 
-def search_for_sublist(ir, sublist):
-    _list = ir.to_list() if hasattr(ir, "to_list") else ir
-    if _list == sublist:
-        return True
-    return isinstance(_list, list) and any(search_for_sublist(i, sublist) for i in _list)
+    assert c.x() == 123
+    assert env.get_balance(c.address) == 0
+    value = to_wei(0.1, "ether")
+    env.set_balance(env.deployer, value)
+    with tx_failed():
+        env.message_call(c.address, value=value, data=b"")  # call default function
+    assert env.get_balance(c.address) == 0
 
 
-def test_builtin_constants(get_contract_with_gas_estimation):
+def test_basic_default(env, get_logs, get_contract):
     code = """
-@external
-def test_zaddress(a: address) -> bool:
-    return a == empty(address)
-
-
-@external
-def test_empty_bytes32(a: bytes32) -> bool:
-    return a == empty(bytes32)
-
+event Sent:
+    sender: indexed(address)
 
 @external
-def test_int128(a: int128) -> (bool, bool):
-    return a == max_value(int128), a == min_value(int128)
+@payable
+def __default__():
+    log Sent(msg.sender)
+    """
+    c = get_contract(code)
+    env.set_balance(env.deployer, 10**18)
+    env.message_call(c.address, value=10**17, data=b"")  # call default function
+    (log,) = get_logs(c, "Sent")
+    assert env.deployer == log.args.sender
+    assert env.get_balance(c.address) == to_wei(0.1, "ether")
 
 
-@external
-def test_decimal(a: decimal) -> (bool, bool):
-    return a == max_value(decimal), a == min_value(decimal)
-
+def test_basic_default_default_param_function(env, get_logs, get_contract):
+    code = """
+event Sent:
+    sender: indexed(address)
 
 @external
-def test_uint256(a: uint256) -> bool:
-    return a == max_value(uint256)
-
+@payable
+def fooBar(a: int128 = 12345) -> int128:
+    log Sent(empty(address))
+    return a
 
 @external
-def test_arithmetic(a: int128) -> int128:
-    return max_value(int128) - a
+@payable
+def __default__():
+    log Sent(msg.sender)
     """
-
-    c = get_contract_with_gas_estimation(code)
-
-    assert c.test_empty_bytes32(b"\x00" * 32) is True
-    assert c.test_empty_bytes32(b"\x0F" * 32) is False
-
-    assert c.test_zaddress("0x0000000000000000000000000000000000000000") is True
-    assert c.test_zaddress("0x0000000000000000000000000000000000000012") is False
-
-    assert c.test_int128(2**127 - 1) == [True, False]
-    assert c.test_int128(-(2**127)) == [False, True]
-    assert c.test_int128(0) == [False, False]
-
-    assert c.test_decimal(
-        decimal_to_int("18707220957835557353007165858768422651595.9365500927")
-    ) == [True, False]
-    assert c.test_decimal(
-        decimal_to_int("-18707220957835557353007165858768422651595.9365500928")
-    ) == [False, True]
-    assert c.test_decimal(decimal_to_int("0.1")) == [False, False]
-
-    assert c.test_uint256(2**256 - 1) is True
-
-    assert c.test_arithmetic(5000) == 2**127 - 1 - 5000
+    c = get_contract(code)
+    env.set_balance(env.deployer, 10**18)
+    env.message_call(c.address, value=10**17, data=b"")  # call default function
+    (log,) = get_logs(c, "Sent")
+    assert env.deployer == log.args.sender
+    assert env.get_balance(c.address) == to_wei(0.1, "ether")
 
 
-def test_builtin_constants_assignment(get_contract_with_gas_estimation):
+def test_basic_default_not_payable(env, tx_failed, get_contract):
     code = """
-@external
-def foo() -> int128:
-    bar: int128 = max_value(int128)
-    return bar
-
-@external
-def goo() -> int128:
-    bar: int128 = min_value(int128)
-    return bar
-
-@external
-def hoo() -> bytes32:
-    bar: bytes32 = empty(bytes32)
-    return bar
+event Sent:
+    sender: indexed(address)
 
 @external
-def joo() -> address:
-    bar: address = empty(address)
-    return bar
+def __default__():
+    log Sent(msg.sender)
+    """
+    c = get_contract(code)
+    env.set_balance(env.deployer, 10**17)
 
-@external
-def koo() -> decimal:
-    bar: decimal = max_value(decimal)
-    return bar
+    with tx_failed():
+        env.message_call(c.address, value=10**17, data=b"")  # call default function
 
-@external
-def loo() -> decimal:
-    bar: decimal = min_value(decimal)
-    return bar
 
+def test_multi_arg_default(assert_compile_failed, get_contract):
+    code = """
+@payable
 @external
-def zoo() -> uint256:
-    bar: uint256 = max_value(uint256)
-    return bar
+def __default__(arg1: int128):
+    pass
     """
+    assert_compile_failed(lambda: get_contract(code))
 
-    c = get_contract_with_gas_estimation(code)
-
-    assert c.foo() == 2**127 - 1
-    assert c.goo() == -(2**127)
 
-    assert c.hoo() == b"\x00" * 32
+def test_always_public(assert_compile_failed, get_contract):
+    code = """
+@internal
+def __default__():
+    pass
+    """
+    assert_compile_failed(lambda: get_contract(code))
 
-    assert c.joo() is None
 
-    assert c.koo() == (2**167 - 1)
-    assert c.loo() == -(2**167)
+def test_always_public_2(assert_compile_failed, get_contract):
+    code = """
+event Sent:
+    sender: indexed(address)
 
-    assert c.zoo() == 2**256 - 1
+def __default__():
+    log Sent(msg.sender)
+    """
+    assert_compile_failed(lambda: get_contract(code))
 
 
-def test_custom_constants(get_contract):
+def test_zero_method_id(env, get_logs, get_contract, tx_failed):
+    # test a method with 0x00000000 selector,
+    # expects at least 36 bytes of calldata.
     code = """
-X_VALUE: constant(uint256) = 33
+event Sent:
+    sig: uint256
 
 @external
-def test() -> uint256:
-    return X_VALUE
+@payable
+# function selector: 0x00000000
+def blockHashAskewLimitary(v: uint256) -> uint256:
+    log Sent(2)
+    return 7
 
 @external
-def test_add(a: uint256) -> uint256:
-    return X_VALUE + a
+def __default__():
+    log Sent(1)
     """
     c = get_contract(code)
 
-    assert c.test() == 33
-    assert c.test_add(7) == 40
+    assert c.blockHashAskewLimitary(0) == 7
 
+    def _call_with_bytes(hexstr):
+        # call our special contract and return the logged value
+        data = bytes.fromhex(hexstr.removeprefix("0x"))
+        env.message_call(c.address, value=0, data=data)
+        (log,) = get_logs(c, "Sent")
+        return log.args.sig
 
-# Would be nice to put this somewhere accessible, like in vyper.types or something
-integer_types = ["uint8", "int128", "int256", "uint256"]
+    assert 1 == _call_with_bytes("0x")
 
+    # call blockHashAskewLimitary with proper calldata
+    assert 2 == _call_with_bytes("0x" + "00" * 36)
 
-@pytest.mark.parametrize("storage_type,return_type", itertools.permutations(integer_types, 2))
-def test_custom_constants_fail(get_contract, assert_compile_failed, storage_type, return_type):
-    code = f"""
-MY_CONSTANT: constant({storage_type}) = 1
+    # call blockHashAskewLimitary with extra trailing bytes in calldata
+    assert 2 == _call_with_bytes("0x" + "00" * 37)
 
-@external
-def foo() -> {return_type}:
-    return MY_CONSTANT
-    """
-    assert_compile_failed(lambda: get_contract(code), TypeMismatch)
+    for i in range(4):
+        # less than 4 bytes of calldata doesn't match the 0 selector and goes to default
+        assert 1 == _call_with_bytes("0x" + "00" * i)
+
+    for i in range(4, 36):
+        # match the full 4 selector bytes, but revert due to malformed (short) calldata
+        with tx_failed():
+            _call_with_bytes(f"0x{'00' * i}")
 
 
-def test_constant_address(get_contract):
+def test_another_zero_method_id(env, get_logs, get_contract, tx_failed):
+    # test another zero method id but which only expects 4 bytes of calldata
     code = """
-OWNER: constant(address) = 0x0000000000000000000000000000000000000012
+event Sent:
+    sig: uint256
 
 @external
-def get_owner() -> address:
-    return OWNER
+@payable
+# function selector: 0x00000000
+def wycpnbqcyf() -> uint256:
+    log Sent(2)
+    return 7
 
 @external
-def is_owner() -> bool:
-    if msg.sender == OWNER:
-        return True
-    else:
-        return False
+def __default__():
+    log Sent(1)
     """
     c = get_contract(code)
 
-    assert c.get_owner() == "0x0000000000000000000000000000000000000012"
-    assert c.is_owner() is False
+    assert c.wycpnbqcyf() == 7
 
+    def _call_with_bytes(hexstr):
+        # call our special contract and return the logged value
+        data = bytes.fromhex(hexstr.removeprefix("0x"))
+        env.message_call(c.address, value=0, data=data, gas=10**6)
+        (log,) = get_logs(c, "Sent")
+        return log.args.sig
 
-def test_constant_bytes(get_contract):
-    test_str = b"Alabama, Arkansas. I do love my ma and pa"
-    code = f"""
-X: constant(Bytes[100]) = b"{test_str.decode()}"
+    assert 1 == _call_with_bytes("0x")
 
-@external
-def test() -> Bytes[100]:
-    y: Bytes[100] = X
+    # call wycpnbqcyf
+    assert 2 == _call_with_bytes("0x" + "00" * 4)
 
-    return y
-    """
-
-    c = get_contract(code)
-
-    assert c.test() == test_str
+    # too many bytes ok
+    assert 2 == _call_with_bytes("0x" + "00" * 5)
 
+    # "right" method id but by accident - not enough bytes.
+    for i in range(4):
+        assert 1 == _call_with_bytes("0x" + "00" * i)
 
-def test_constant_folds():
-    some_prime = 10013677
-    code = f"""
-SOME_CONSTANT: constant(uint256) = 11 + 1
-SOME_PRIME: constant(uint256) = {some_prime}
-
-@external
-def test() -> uint256:
-    # calculate some constant which is really unlikely to be randomly
-    # in bytecode
-    ret: uint256 = 2**SOME_CONSTANT * SOME_PRIME
-    return ret
-    """
-    ir = compile_code(code, output_formats=["ir"])["ir"]
-    search = ["mstore", [MemoryPositions.RESERVED_MEMORY], [2**12 * some_prime]]
-    assert search_for_sublist(ir, search)
 
-
-def test_constant_lists(get_contract):
+def test_partial_selector_match_trailing_zeroes(env, get_logs, get_contract):
     code = """
-BYTE32_LIST: constant(bytes32[2]) = [
-    0x0000000000000000000000000000000000000000000000000000000000001321,
-    0x0000000000000000000000000000000000000000000000000000000000001123
-]
-
-SPECIAL: constant(int128[3]) = [33, 44, 55]
+event Sent:
+    sig: uint256
 
 @external
-def test() -> bytes32:
-    a: bytes32[2] = BYTE32_LIST
-    return a[1]
+@payable
+# function selector: 0xd88e0b00
+def fow() -> uint256:
+    log Sent(2)
+    return 7
 
-@view
 @external
-def contains(a: int128) -> bool:
-    return a in SPECIAL
+def __default__():
+    log Sent(1)
     """
-
     c = get_contract(code)
 
-    assert c.test()[-2:] == b"\x11\x23"
+    # sanity check - we can call c.fow()
+    assert c.fow() == 7
+
+    def _call_with_bytes(hexstr):
+        # call our special contract and return the logged value
+        data = bytes.fromhex(hexstr.removeprefix("0x"))
+        env.message_call(c.address, value=0, data=data)
+        (log,) = get_logs(c, "Sent")
+        return log.args.sig
+
+    # check we can call default function
+    assert 1 == _call_with_bytes("0x")
+
+    # check fow() selector is 0xd88e0b00
+    assert 2 == _call_with_bytes("0xd88e0b00")
 
-    assert c.contains(55) is True
-    assert c.contains(44) is True
-    assert c.contains(33) is True
-    assert c.contains(3) is False
+    # check calling d88e0b with no trailing zero goes to fallback instead of reverting
+    assert 1 == _call_with_bytes("0xd88e0b")
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_decimals.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_decimals.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 def foo(x: decimal) -> decimal:
     return {op} x
     """
     with pytest.raises(InvalidOperation):
         compile_code(code)
 
 
-def test_decimal_test(get_contract_with_gas_estimation):
+def test_decimal_test(get_contract):
     decimal_test = """
 @external
 def foo() -> int256:
     return(floor(999.0))
 
 @external
 def fop() -> int256:
@@ -98,15 +98,15 @@
     return(floor(1999.0 % 1000.0))
 
 @external
 def foop() -> int256:
     return(floor(1999.0 % 1000.0))
     """
 
-    c = get_contract_with_gas_estimation(decimal_test)
+    c = get_contract(decimal_test)
 
     assert c.foo() == 999
     assert c.fop() == 999
     assert c.foq() == 999
     assert c.bar() == 999
     assert c.baz() == 999
     assert c.mok() == 999
@@ -115,15 +115,15 @@
     assert c.moo() == 999
     assert c.foom() == 999
     assert c.foop() == 999
 
     print("Passed basic addition, subtraction and multiplication tests")
 
 
-def test_harder_decimal_test(get_contract_with_gas_estimation):
+def test_harder_decimal_test(get_contract):
     harder_decimal_test = """
 @external
 def phooey(inp: decimal) -> decimal:
     x: decimal = 10000.0
     for i: uint256 in range(4):
         x = x * inp
     return x
@@ -147,36 +147,36 @@
 @external
 def iarg() -> uint256:
     x: uint256 = as_wei_value(7, "wei")
     x *= 2
     return x
     """
 
-    c = get_contract_with_gas_estimation(harder_decimal_test)
+    c = get_contract(harder_decimal_test)
     assert c.phooey(decimal_to_int("1.2")) == decimal_to_int("20736.0")
     assert c.phooey(decimal_to_int("-1.2")) == decimal_to_int("20736.0")
     assert c.arg(decimal_to_int("-3.7")) == decimal_to_int("-3.7")
     assert c.arg(decimal_to_int("3.7")) == decimal_to_int("3.7")
     assert c.garg() == decimal_to_int("6.75")
     assert c.harg() == decimal_to_int("9.0")
     assert c.iarg() == 14
 
     print("Passed fractional multiplication test")
 
 
-def test_mul_overflow(tx_failed, get_contract_with_gas_estimation):
+def test_mul_overflow(tx_failed, get_contract):
     mul_code = """
 
 @external
 def _num_mul(x: decimal, y: decimal) -> decimal:
     return x * y
 
     """
 
-    c = get_contract_with_gas_estimation(mul_code)
+    c = get_contract(mul_code)
 
     x = decimal_to_int("85070591730234615865843651857942052864")
     y = decimal_to_int("136112946768375385385349842973")
 
     with tx_failed():
         c._num_mul(x, y)
 
@@ -243,40 +243,40 @@
     assert c.foo(decimal_to_int(x), decimal_to_int(1)) == decimal_to_int(x)
 
     assert c.foo(decimal_to_int(x), decimal_to_int(1 + DECIMAL_EPSILON)) == decimal_to_int(
         quantize(x / (1 + DECIMAL_EPSILON))
     )
 
 
-def test_decimal_min_max_literals(tx_failed, get_contract_with_gas_estimation):
+def test_decimal_min_max_literals(tx_failed, get_contract):
     code = """
 @external
 def maximum():
     a: decimal = 18707220957835557353007165858768422651595.9365500927
 @external
 def minimum():
     a: decimal = -18707220957835557353007165858768422651595.9365500928
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
-    assert c.maximum() == []
-    assert c.minimum() == []
+    assert c.maximum() is None
+    assert c.minimum() is None
 
 
-def test_scientific_notation(get_contract_with_gas_estimation):
+def test_scientific_notation(get_contract):
     code = """
 @external
 def foo() -> decimal:
     return 1e-10
 
 @external
 def bar(num: decimal) -> decimal:
     return num + -1e38
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.foo() == decimal_to_int("1e-10")  # Smallest possible decimal
     assert c.bar(decimal_to_int("1e37")) == decimal_to_int("-9e37")  # Math lines up
 
 
 def test_exponents():
     code = """
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_division.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_division.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_exponents.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_exponents.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,24 @@
 def f0():
     lv0: uint256 = max_value(int128) ** max_value(int128)
     """
     with pytest.raises(InvalidLiteral):
         compile_code(code)
 
 
+def test_fold_nonliteral(get_contract):
+    # test we can fold non-literal constants
+    code = """
+N: constant(uint256) = 3
+N2: public(constant(uint256)) = N**N
+    """
+    c = get_contract(code)
+    assert c.N2() == 3**3
+
+
 @pytest.mark.fuzzing
 @pytest.mark.parametrize("power", range(2, 255))
 def test_exp_uint256(get_contract, tx_failed, power):
     code = f"""
 @external
 def foo(a: uint256) -> uint256:
     return a ** {power}
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_isqrt.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_isqrt.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,111 +3,111 @@
 import hypothesis
 import pytest
 
 from vyper.utils import SizeLimits
 
 
 @pytest.fixture(scope="module")
-def isqrt_contract(get_contract_module):
+def isqrt_contract(get_contract):
     code = """
 @external
 def test(a: uint256) -> uint256:
     return isqrt(a)
     """
-    c = get_contract_module(code)
+    c = get_contract(code)
     return c
 
 
-def test_isqrt_literal(get_contract_with_gas_estimation):
+def test_isqrt_literal(get_contract):
     val = 2
     code = f"""
 @external
 def test() -> uint256:
     return isqrt({val})
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.test() == math.isqrt(val)
 
 
-def test_isqrt_variable(get_contract_with_gas_estimation):
+def test_isqrt_variable(get_contract):
     code = """
 @external
 def test(a: uint256) -> uint256:
     return isqrt(a)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     val = 3333
     assert c.test(val) == math.isqrt(val)
 
     val = 10**17
     assert c.test(val) == math.isqrt(val)
     assert c.test(0) == 0
 
 
-def test_isqrt_internal_variable(get_contract_with_gas_estimation):
+def test_isqrt_internal_variable(get_contract):
     val = 44001
     code = f"""
 @external
 def test2() -> uint256:
     a: uint256 = {val}
     return isqrt(a)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.test2() == math.isqrt(val)
 
 
-def test_isqrt_storage(get_contract_with_gas_estimation):
+def test_isqrt_storage(get_contract):
     code = """
 s_var: uint256
 
 @external
 def test(a: uint256) -> uint256:
     self.s_var = a + 1
     return isqrt(self.s_var)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     val = 1221
     assert c.test(val) == math.isqrt(val + 1)
     val = 10001
     assert c.test(val) == math.isqrt(val + 1)
 
 
-def test_isqrt_storage_internal_variable(get_contract_with_gas_estimation):
+def test_isqrt_storage_internal_variable(get_contract):
     val = 44444
     code = f"""
 s_var: uint256
 
 @external
 def test2() -> uint256:
     self.s_var = {val}
     return isqrt(self.s_var)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.test2() == math.isqrt(val)
 
 
-def test_isqrt_inline_memory_correct(get_contract_with_gas_estimation):
+def test_isqrt_inline_memory_correct(get_contract):
     code = """
 @external
 def test(a: uint256) -> (uint256, uint256, uint256, uint256, uint256, String[100]):
     x: uint256 = 1
     y: uint256 = 2
     z: uint256 = 3
     e: uint256 = isqrt(a)
     f: String[100] = 'hello world'
     return a, x, y, z, e, f
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     val = 21
-    assert c.test(val) == [val, 1, 2, 3, math.isqrt(val), "hello world"]
+    assert c.test(val) == (val, 1, 2, 3, math.isqrt(val), "hello world")
 
 
 @pytest.mark.fuzzing
 @hypothesis.given(
     value=hypothesis.strategies.integers(min_value=0, max_value=SizeLimits.MAX_UINT256)
 )
 @hypothesis.example(SizeLimits.MAX_UINT256)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_modulo.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_modulo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
 from tests.utils import decimal_to_int
 from vyper.exceptions import ZeroDivisionException
 
 
-def test_modulo(get_contract_with_gas_estimation):
+def test_modulo(get_contract):
     code = """
 @external
 def num_modulo_num() -> int128:
     return 1 % 2
 
 @external
 def decimal_modulo_decimal() -> decimal:
@@ -19,28 +19,28 @@
     return .5 % 1.0
 
 
 @external
 def num_modulo_decimal() -> decimal:
     return 1.5 % 1.0
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.num_modulo_num() == 1
     assert c.decimal_modulo_decimal() == decimal_to_int(".18")
     assert c.decimal_modulo_num() == decimal_to_int(".5")
     assert c.num_modulo_decimal() == decimal_to_int(".5")
 
 
-def test_modulo_with_input_of_zero(tx_failed, get_contract_with_gas_estimation):
+def test_modulo_with_input_of_zero(tx_failed, get_contract):
     code = """
 @external
 def foo(a: decimal, b: decimal) -> decimal:
     return a % b
 """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     with tx_failed():
         c.foo(decimal_to_int("1"), decimal_to_int("0"))
 
 
 def test_literals_vs_evm(get_contract):
     code = """
 @external
@@ -52,15 +52,15 @@
 @view
 def bar(a: int128) -> bool:
     assert -5%2 == a%2
     return True
 """
 
     c = get_contract(code)
-    assert c.foo() == [1, 1, -1, -1]
+    assert c.foo() == (1, 1, -1, -1)
     assert c.bar(-5) is True
 
 
 BAD_CODE = [
     """
 @external
 def foo() -> uint256:
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_signed_ints.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_signed_ints.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pytest
 
 from vyper import compile_code
 from vyper.exceptions import (
     InvalidOperation,
     OverflowException,
+    StaticAssertionException,
     TypeMismatch,
     ZeroDivisionException,
 )
 from vyper.semantics.types import IntegerT
 from vyper.utils import evm_div, evm_mod
 
 types = sorted(IntegerT.signeds())
@@ -69,26 +70,43 @@
     c = get_contract(code)
     for x in range(5):
         assert c.foo(x) == (-1) ** x
 
 
 # TODO: make this test pass
 @pytest.mark.parametrize("base", (0, 1))
-def test_exponent_negative_power(get_contract, tx_failed, base):
+def test_exponent_negative_power_runtime_check(get_contract, tx_failed, base, experimental_codegen):
     # #2985
     code = f"""
 @external
-def bar() -> int16:
-    x: int16 = -2
+def bar(negative:int16) -> int16:
+    x: int16 = negative
     return {base} ** x
     """
     c = get_contract(code)
     # known bug: 2985
     with tx_failed():
-        c.bar()
+        c.bar(-2)
+
+
+@pytest.mark.parametrize("base", (0, 1))
+def test_exponent_negative_power_compile_time_check(
+    get_contract, tx_failed, base, experimental_codegen
+):
+    # #2985
+    code = f"""
+@external
+def bar() -> int16:
+    x: int16 = -2
+    return {base} ** x
+    """
+    if not experimental_codegen:
+        return
+    with pytest.raises(StaticAssertionException):
+        get_contract(code)
 
 
 def test_exponent_min_int16(get_contract):
     # #2987
     code = """
 @external
 def foo() -> int16:
@@ -130,15 +148,15 @@
             with tx_failed():
                 c.foo(x)
         else:
             assert c.foo(x) == 4**x
 
 
 @pytest.mark.parametrize("typ", types)
-def test_negative_nums(get_contract_with_gas_estimation, typ):
+def test_negative_nums(get_contract, typ):
     negative_nums_code = f"""
 @external
 def negative_one() -> {typ}:
     return -1
 
 @external
 def negative_three() -> {typ}:
@@ -146,22 +164,22 @@
 
 @external
 def negative_four() -> {typ}:
     a: {typ} = 2
     return -(a+2)
     """
 
-    c = get_contract_with_gas_estimation(negative_nums_code)
+    c = get_contract(negative_nums_code)
     assert c.negative_one() == -1
     assert c.negative_three() == -3
     assert c.negative_four() == -4
 
 
 @pytest.mark.parametrize("typ", types)
-def test_num_bound(tx_failed, get_contract_with_gas_estimation, typ):
+def test_num_bound(tx_failed, get_contract, typ):
     lo, hi = typ.ast_bounds
 
     num_bound_code = f"""
 @external
 def _num(x: {typ}) -> {typ}:
     return x
 
@@ -182,15 +200,15 @@
     return {hi}
 
 @external
 def _num_min() -> {typ}:
     return {lo}
     """
 
-    c = get_contract_with_gas_estimation(num_bound_code)
+    c = get_contract(num_bound_code)
 
     assert c._num_add(hi, 0) == hi
     assert c._num_sub(lo, 0) == lo
     assert c._num_add(hi - 1, 1) == hi
     assert c._num_sub(lo + 1, 1) == lo
     with tx_failed():
         c._num_add(hi, 1)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_sqrt.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_sqrt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from decimal import ROUND_FLOOR, Decimal
 
 import hypothesis
 import pytest
-from eth_tester.exceptions import TransactionFailed
 
 from tests.utils import decimal_to_int
 from vyper.utils import SizeLimits
 
 DECIMAL_PLACES = 10
 DECIMAL_RANGE = [Decimal("0." + "0" * d + "2") for d in range(0, DECIMAL_PLACES)]
 
@@ -19,95 +18,95 @@
     return val.quantize(Decimal(q), rounding=rounding)
 
 
 def decimal_sqrt(val):
     return decimal_to_int(decimal_truncate(val.sqrt()))
 
 
-def test_sqrt_literal(get_contract_with_gas_estimation):
+def test_sqrt_literal(get_contract):
     code = """
 @external
 def test() -> decimal:
     return sqrt(2.0)
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.test() == decimal_sqrt(Decimal("2"))
 
 
 # TODO: use parametrization here
-def test_sqrt_variable(get_contract_with_gas_estimation):
+def test_sqrt_variable(get_contract):
     code = """
 @external
 def test(a: decimal) -> decimal:
     return sqrt(a)
 
 @external
 def test2() -> decimal:
     a: decimal = 44.001
     return sqrt(a)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     val = Decimal("33.33")
     assert c.test(decimal_to_int(val)) == decimal_sqrt(val)
 
     val = Decimal("0.1")
     assert c.test(decimal_to_int(val)) == decimal_sqrt(val)
 
     assert c.test(decimal_to_int("0.0")) == decimal_to_int("0.0")
     assert c.test2() == decimal_sqrt(Decimal("44.001"))
 
 
-def test_sqrt_storage(get_contract_with_gas_estimation):
+def test_sqrt_storage(get_contract):
     code = """
 s_var: decimal
 
 @external
 def test(a: decimal) -> decimal:
     self.s_var = a + 1.0
     return sqrt(self.s_var)
 
 @external
 def test2() -> decimal:
     self.s_var = 444.44
     return sqrt(self.s_var)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     val = Decimal("12.21")
     assert c.test(decimal_to_int(val)) == decimal_sqrt(val + 1)
     val = Decimal("100.01")
     assert c.test(decimal_to_int(val)) == decimal_sqrt(val + 1)
     assert c.test2() == decimal_sqrt(Decimal("444.44"))
 
 
-def test_sqrt_inline_memory_correct(get_contract_with_gas_estimation):
+def test_sqrt_inline_memory_correct(get_contract):
     code = """
 @external
 def test(a: decimal) -> (decimal, decimal, decimal, decimal, decimal, String[100]):
     x: decimal = 1.0
     y: decimal = 2.0
     z: decimal = 3.0
     e: decimal = sqrt(a)
     f: String[100] = 'hello world'
     return a, x, y, z, e, f
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     val = Decimal("2.1")
-    assert c.test(decimal_to_int(val)) == [
+    assert c.test(decimal_to_int(val)) == (
         decimal_to_int(val),
         decimal_to_int("1"),
         decimal_to_int("2"),
         decimal_to_int("3"),
         decimal_sqrt(val),
         "hello world",
-    ]
+    )
 
 
 @pytest.mark.parametrize("value", DECIMAL_RANGE)
 def test_sqrt_sub_decimal_places(value, get_contract):
     code = """
 @external
 def test(a: decimal) -> decimal:
@@ -118,21 +117,21 @@
 
     vyper_sqrt = c.test(decimal_to_int(value))
     actual_sqrt = decimal_sqrt(value)
     assert vyper_sqrt == actual_sqrt
 
 
 @pytest.fixture(scope="module")
-def sqrt_contract(get_contract_module):
+def sqrt_contract(get_contract):
     code = """
 @external
 def test(a: decimal) -> decimal:
     return sqrt(a)
     """
-    c = get_contract_module(code)
+    c = get_contract(code)
     return c
 
 
 @pytest.mark.parametrize("value", [Decimal(0), Decimal(SizeLimits.MAX_INT128)])
 def test_sqrt_bounds(sqrt_contract, value):
     vyper_sqrt = sqrt_contract.test(decimal_to_int(value))
     actual_sqrt = decimal_sqrt(value)
@@ -157,10 +156,10 @@
 @hypothesis.given(
     value=hypothesis.strategies.decimals(
         min_value=Decimal(SizeLimits.MIN_INT128), max_value=Decimal("-1E10"), places=DECIMAL_PLACES
     )
 )
 @hypothesis.example(value=Decimal(SizeLimits.MIN_INT128))
 @hypothesis.example(value=Decimal("-1E10"))
-def test_sqrt_invalid_range(sqrt_contract, value):
-    with pytest.raises(TransactionFailed):
+def test_sqrt_invalid_range(tx_failed, sqrt_contract, value):
+    with tx_failed():
         sqrt_contract.test(decimal_to_int(value))
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/numbers/test_unsigned_ints.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/numbers/test_unsigned_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_array_indexing.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_array_indexing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,70 @@
-import pytest
-from eth_tester.exceptions import TransactionFailed
-
 # TODO: rewrite the tests in type-centric way, parametrize array and indices types
 
 
-def test_negative_ix_access(get_contract):
+def test_negative_ix_access(get_contract, tx_failed):
     # Arrays can't be accessed with negative indices
     code = """
 arr: uint256[3]
 
 @external
 def foo(i: int128):
     self.arr[i] = 1
     """
 
     c = get_contract(code)
 
-    with pytest.raises(TransactionFailed):
+    with tx_failed():
         c.foo(-1)
+    with tx_failed():
         c.foo(-3)
+    with tx_failed():
         c.foo(-(2**127) + 1)
 
 
-def test_negative_ix_access_to_large_arr(get_contract):
+def test_negative_ix_access_to_large_arr(get_contract, tx_failed):
     # Arrays can't be accessed with negative indices
     code = """
 arr: public(uint256[max_value(uint256)-1])
 
 @external
 def set(idx: int256):
     self.arr[idx] = 1
     """
 
     c = get_contract(code)
-    with pytest.raises(TransactionFailed):
+    with tx_failed():
         c.set(-(2**255))
+    with tx_failed():
         c.set(-(2**255) + 5)
+    with tx_failed():
         c.set(-(2**128))
+    with tx_failed():
         c.set(-1)
 
 
-def test_oob_access_to_large_arr(get_contract):
+def test_oob_access_to_large_arr(get_contract, tx_failed):
     # Test OOB access to large array
     code = """
 arr: public(uint256[max_value(uint256)-1])
 
 @external
 def set(idx: int256):
     self.arr[idx] = 3
 
 @external
 def set2(idx: uint256):
     self.arr[idx] = 3
     """
     c = get_contract(code)
 
-    with pytest.raises(TransactionFailed):
-        c.set2(2**256 - 1, transact={})
-        c.set2(2**256 - 2, transact={})
+    with tx_failed():
+        c.set2(2**256 - 1)
+    with tx_failed():
+        c.set2(2**256 - 2)
 
 
 def test_boundary_access_to_arr(get_contract):
     # Test access to the boundary of the array
     code = """
 arr1: public(int256[max_value(int256)])
 
@@ -75,22 +78,22 @@
 
 @external
 def set2(idx: uint256):
     self.arr2[idx] = 3
     """
     c1 = get_contract(code)
 
-    c1.set1(2**255 - 2, transact={})
+    c1.set1(2**255 - 2)
     assert c1.arr1(2**255 - 2) == 3
-    c1.set1(0, transact={})
+    c1.set1(0)
     assert c1.arr1(0) == 3
 
     c2 = get_contract(code2)
 
-    c2.set2(2**256 - 3, transact={})
+    c2.set2(2**256 - 3)
     assert c2.arr2(2**256 - 3) == 3
 
 
 def test_valid_ix_access(get_contract):
     code = """
 arr: public(uint256[3])
 arr2: public(int256[3])
@@ -102,17 +105,17 @@
 @external
 def bar(i: uint256):
     self.arr[i] = 2
     """
 
     c = get_contract(code)
     for i in range(3):
-        c.foo(i, transact={})
+        c.foo(i)
         assert c.arr(i) == 1
-        c.bar(i, transact={})
+        c.bar(i)
         assert c.arr(i) == 2
 
 
 def test_for_loop_ix_access(get_contract):
     # Arrays can be accessed with for loop iterators of type int
     code = """
 arr: public(int256[10])
@@ -120,10 +123,10 @@
 @external
 def foo():
     for i: int256 in range(10):
         self.arr[i] = i
     """
 
     c = get_contract(code)
-    c.foo(transact={})
+    c.foo()
     for i in range(10):
         assert c.arr(i) == i
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pytest
 
 from vyper.exceptions import TypeMismatch
 
 
-def test_test_bytes(get_contract_with_gas_estimation, tx_failed):
+def test_test_bytes(get_contract, tx_failed):
     test_bytes = """
 @external
 def foo(x: Bytes[100]) -> Bytes[100]:
     return x
     """
 
-    c = get_contract_with_gas_estimation(test_bytes)
+    c = get_contract(test_bytes)
     moo_result = c.foo(b"cow")
     assert moo_result == b"cow"
 
     print("Passed basic bytes test")
 
     assert c.foo(b"\x35" * 100) == b"\x35" * 100
 
@@ -23,33 +23,33 @@
     # test for greater than 100 bytes, should raise exception
     with tx_failed():
         c.foo(b"\x35" * 101)
 
     print("Passed input-too-long test")
 
 
-def test_test_bytes2(get_contract_with_gas_estimation):
+def test_test_bytes2(get_contract):
     test_bytes2 = """
 @external
 def foo(x: Bytes[100]) -> Bytes[100]:
     y: Bytes[100] = x
     return y
     """
 
-    c = get_contract_with_gas_estimation(test_bytes2)
+    c = get_contract(test_bytes2)
     assert c.foo(b"cow") == b"cow"
     assert c.foo(b"") == b""
     assert c.foo(b"\x35" * 63) == b"\x35" * 63
     assert c.foo(b"\x35" * 64) == b"\x35" * 64
     assert c.foo(b"\x35" * 65) == b"\x35" * 65
 
     print("Passed string copying test")
 
 
-def test_test_bytes3(get_contract_with_gas_estimation):
+def test_test_bytes3(get_contract):
     test_bytes3 = """
 x: int128
 maa: Bytes[60]
 y: int128
 
 @deploy
 def __init__():
@@ -75,32 +75,32 @@
     return ay
 
 @external
 def get_xy() -> int128:
     return self.x * self.y
     """
 
-    c = get_contract_with_gas_estimation(test_bytes3)
-    c.set_maa(b"pig", transact={})
+    c = get_contract(test_bytes3)
+    c.set_maa(b"pig")
     assert c.get_maa() == b"pig"
     assert c.get_maa2() == b"pig"
-    c.set_maa2(b"", transact={})
+    c.set_maa2(b"")
     assert c.get_maa() == b""
     assert c.get_maa2() == b""
-    c.set_maa(b"\x44" * 60, transact={})
+    c.set_maa(b"\x44" * 60)
     assert c.get_maa() == b"\x44" * 60
     assert c.get_maa2() == b"\x44" * 60
-    c.set_maa2(b"mongoose", transact={})
+    c.set_maa2(b"mongoose")
     assert c.get_maa() == b"mongoose"
     assert c.get_xy() == 999
 
     print("Passed advanced string copying test")
 
 
-def test_test_bytes4(get_contract_with_gas_estimation):
+def test_test_bytes4(get_contract):
     test_bytes4 = """
 a: Bytes[60]
 @external
 def foo(inp: Bytes[60]) -> Bytes[60]:
     self.a = inp
     self.a = b""
     return self.a
@@ -108,22 +108,22 @@
 @external
 def bar(inp: Bytes[60]) -> Bytes[60]:
     b: Bytes[60] = inp
     b = b""
     return b
     """
 
-    c = get_contract_with_gas_estimation(test_bytes4)
+    c = get_contract(test_bytes4)
     assert c.foo(b"") == b"", c.foo()
     assert c.bar(b"") == b""
 
     print("Passed string deleting test")
 
 
-def test_test_bytes5(get_contract_with_gas_estimation):
+def test_test_bytes5(get_contract):
     test_bytes5 = """
 struct G:
     a: Bytes[50]
     b: Bytes[50]
 struct H:
     a: Bytes[40]
     b: Bytes[45]
@@ -155,28 +155,28 @@
 @external
 def quz(inp1: Bytes[40], inp2: Bytes[45]):
     h:  H = H(a=inp1, b=inp2)
     self.g.a = h.a
     self.g.b = h.b
     """
 
-    c = get_contract_with_gas_estimation(test_bytes5)
-    c.foo(b"cow", b"horse", transact={})
+    c = get_contract(test_bytes5)
+    c.foo(b"cow", b"horse")
     assert c.check1() == b"cow"
     assert c.check2() == b"horse"
     assert c.bar(b"pig", b"moose") == b"pig"
     assert c.bat(b"pig", b"moose") == b"moose"
-    c.quz(b"badminton", b"fluffysheep", transact={})
+    c.quz(b"badminton", b"fluffysheep")
     assert c.check1() == b"badminton"
     assert c.check2() == b"fluffysheep"
 
     print("Passed string struct test")
 
 
-def test_binary_literal(get_contract_with_gas_estimation):
+def test_binary_literal(get_contract):
     bytes_to_num_code = """
 r: Bytes[1]
 
 @external
 def get(a: Bytes[1]) -> Bytes[2]:
     return concat(a, 0b00000001)
 
@@ -190,39 +190,39 @@
 
 @external
 def testsome_storage(y: Bytes[1]) -> bool:
     self.r = 0b01100001
     return self.r == y
     """
 
-    c = get_contract_with_gas_estimation(bytes_to_num_code)
+    c = get_contract(bytes_to_num_code)
 
     assert c.getsome() == b"\x0e"
     assert c.testsome(b"a")
     assert c.testsome(b"\x61")
     assert c.testsome(0b1100001.to_bytes(1, "big"))
     assert not c.testsome(b"b")
     assert c.testsome_storage(b"a")
     assert not c.testsome_storage(b"x")
 
 
-def test_bytes_comparison(get_contract_with_gas_estimation):
+def test_bytes_comparison(get_contract):
     code = """
 @external
 def get_mismatch(a: Bytes[1]) -> bool:
     b: Bytes[2] = b'ab'
     return a == b
 
 @external
 def get_large(a: Bytes[100]) -> bool:
     b: Bytes[100] = b'ab'
     return a == b
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.get_mismatch(b"\x00") is False
     assert c.get_large(b"\x00") is False
     assert c.get_large(b"ab") is True
 
 
 def test_bytes32_literals(get_contract):
     code = """
@@ -282,19 +282,19 @@
 def get_count() -> Bytes[24]:
     return self.to_little_endian_64(self.counter)
     """
 
     c = get_contract(code)
 
     assert c.get_count() == b"\x00\x00\x00\x00\x00\x00\x00\x00"
-    c.set_count(1, transact={})
+    c.set_count(1)
     assert c.get_count() == b"\x01\x00\x00\x00\x00\x00\x00\x00"
-    c.set_count(0xF0F0F0, transact={})
+    c.set_count(0xF0F0F0)
     assert c.get_count() == b"\xf0\xf0\xf0\x00\x00\x00\x00\x00"
-    c.set_count(0x0101010101010101, transact={})
+    c.set_count(0x0101010101010101)
     assert c.get_count() == b"\x01\x01\x01\x01\x01\x01\x01\x01"
 
 
 cases_invalid_assignments = [
     (
         """
 @external
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes_literal.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes_literal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 
 import pytest
 
 
-def test_bytes_literal_code(get_contract_with_gas_estimation):
+def test_bytes_literal_code(get_contract):
     bytes_literal_code = """
 @external
 def foo() -> Bytes[5]:
     return b"horse"
 
 @external
 def bar() -> Bytes[10]:
@@ -27,27 +27,27 @@
 
 @external
 def baz4() -> Bytes[100]:
     return concat(b"01234567890123456789012345678901234567890123456789",
                   b"01234567890123456789012345678901234567890123456789")
     """
 
-    c = get_contract_with_gas_estimation(bytes_literal_code)
+    c = get_contract(bytes_literal_code)
     assert c.foo() == b"horse"
     assert c.bar() == b"badminton"
     assert c.baz() == b"012345678901234567890123456789012"
     assert c.baz2() == b"0123456789012345678901234567890112"
     assert c.baz3() == b"01234567890123456789012345678901"
     assert c.baz4() == b"0123456789" * 10
 
     print("Passed string literal test")
 
 
 @pytest.mark.parametrize("i,e,_s", itertools.product([95, 96, 97], [63, 64, 65], [31, 32, 33]))
-def test_bytes_literal_splicing_fuzz(get_contract_with_gas_estimation, i, e, _s):
+def test_bytes_literal_splicing_fuzz(get_contract, i, e, _s):
     kode = f"""
 moo: Bytes[100]
 
 @external
 def foo(s: uint256, L: uint256) -> Bytes[100]:
     x: int128 = 27
     r: Bytes[100] = slice(b"{("c" * i)}", s, L)
@@ -72,14 +72,14 @@
     self.moo = slice(b"{("c" * i)}", s, L)
     y: int128 = 37
     if x * y == 999:
         return self.moo
     return b"3434346667777"
     """
 
-    c = get_contract_with_gas_estimation(kode)
+    c = get_contract(kode)
     o1 = c.foo(_s, e - _s)
     o2 = c.bar(_s, e - _s)
     o3 = c.baz(_s, e - _s)
     assert o1 == o2 == o3 == b"c" * (e - _s), (i, _s, e - _s, o1, o2, o3)
 
     print("Passed string literal splicing fuzz-test")
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_bytes_zero_padding.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_bytes_zero_padding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hypothesis
 import pytest
 
 
 @pytest.fixture(scope="module")
-def little_endian_contract(get_contract_module):
+def little_endian_contract(get_contract):
     code = """
 @internal
 @view
 def to_little_endian_64(_value: uint256) -> Bytes[8]:
     y: uint256 = 0
     x: uint256 = _value
     for _: uint256 in range(8):
@@ -16,16 +16,15 @@
     return slice(convert(y, bytes32), 24, 8)
 
 @external
 @view
 def get_count(counter: uint256) -> Bytes[24]:
     return self.to_little_endian_64(counter)
     """
-    c = get_contract_module(code)
-    return c
+    return get_contract(code)
 
 
 @pytest.mark.fuzzing
 @hypothesis.given(value=hypothesis.strategies.integers(min_value=0, max_value=(2**64 - 1)))
 def test_zero_pad_range(little_endian_contract, value):
     actual_bytes = value.to_bytes(8, byteorder="little")
     contract_bytes = little_endian_contract.get_count(value)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_dynamic_array.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_dynamic_array.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import itertools
+from typing import Any, Callable
 
 import pytest
 
 from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import (
     ArgumentException,
@@ -11,15 +12,15 @@
     OverflowException,
     StackTooDeep,
     StateAccessViolation,
     TypeMismatch,
 )
 
 
-def test_list_tester_code(get_contract_with_gas_estimation):
+def test_list_tester_code(get_contract):
     list_tester_code = """
 z: DynArray[int128, 3]
 z2: DynArray[DynArray[int128, 2], 2]
 z3: DynArray[int128, 2]
 
 @external
 def foo(x: DynArray[int128, 3]) -> int128:
@@ -48,25 +49,24 @@
 @external
 def loo(x: DynArray[DynArray[int128, 2], 2]) -> int128:
     self.z2 = x
     self.z3 = x[1]
     return self.z2[0][0] + self.z2[0][1] + self.z3[0] * 10 + self.z3[1] * 10
     """
 
-    c = get_contract_with_gas_estimation(list_tester_code)
+    c = get_contract(list_tester_code)
     assert c.foo([3, 4, 5]) == 12
     assert c.goo([[1, 2], [3, 4]]) == 73
     assert c.hoo([3, 4, 5]) == 12
     assert c.joo([[1, 2], [3, 4]]) == 73
     assert c.koo([3, 4, 5]) == 12
     assert c.loo([[1, 2], [3, 4]]) == 73
     print("Passed list tests")
 
 
-@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_string_list(get_contract):
     code = """
 @external
 def foo1(x: DynArray[String[32], 2]) -> DynArray[String[32], 2]:
     return x
 
 @external
@@ -99,15 +99,15 @@
     assert c.foo2([["hello", "world"]]) == [["hello", "world"]]
     assert c.foo3([["hello", "world"]]) == ["hello", "world"]
     assert c.foo4([["hello", "world"]]) == "hello"
     assert c.foo5() == ["hello", "world"]
     assert c.foo6() == [["hello", "world"]]
 
 
-def test_list_output_tester_code(get_contract_with_gas_estimation):
+def test_list_output_tester_code(get_contract):
     list_output_tester_code = """
 flag Foobar:
     FOO
     BAR
 
 y: DynArray[Foobar, 2]
 z: DynArray[int128, 2]
@@ -200,15 +200,15 @@
     return self.y
 
 @external
 def uoo(inp: DynArray[Foobar, 2]) -> DynArray[DynArray[Foobar, 2], 2]:
     return [inp, [Foobar.BAR, Foobar.FOO]]
     """
 
-    c = get_contract_with_gas_estimation(list_output_tester_code)
+    c = get_contract(list_output_tester_code)
     assert c.foo() == [3, 5]
     assert c.goo() == [3, 5]
     assert c.hoo() == [3, 5]
     assert c.hoo1() == c.hoo2() == c.hoo3() == c.hoo4() == []
     assert c.hoo5() == []
     assert c.joo() == [3, 5]
     assert c.koo() == [[1, 2], [3, 4]]
@@ -228,49 +228,49 @@
     assert c.soo() == [1, 2]
     assert c.too() == [2, 1]
     assert c.uoo([1, 2]) == [[1, 2], [2, 1]]
 
     print("Passed list output tests")
 
 
-def test_array_accessor(get_contract_with_gas_estimation):
+def test_array_accessor(get_contract):
     array_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: DynArray[int128, 4] = [0, 0, 0, 0]
     a[0] = x
     a[1] = y
     a[2] = z
     a[3] = w
     return a[0] * 1000 + a[1] * 100 + a[2] * 10 + a[3]
     """
 
-    c = get_contract_with_gas_estimation(array_accessor)
+    c = get_contract(array_accessor)
     assert c.test_array(2, 7, 1, 8) == 2718
     print("Passed basic array accessor test")
 
 
-def test_two_d_array_accessor(get_contract_with_gas_estimation):
+def test_two_d_array_accessor(get_contract):
     two_d_array_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: DynArray[DynArray[int128, 2], 2] = [[0, 0], [0, 0]]
     a[0][0] = x
     a[0][1] = y
     a[1][0] = z
     a[1][1] = w
     return a[0][0] * 1000 + a[0][1] * 100 + a[1][0] * 10 + a[1][1]
     """
 
-    c = get_contract_with_gas_estimation(two_d_array_accessor)
+    c = get_contract(two_d_array_accessor)
     assert c.test_array(2, 7, 1, 8) == 2718
     print("Passed complex array accessor test")
 
 
-def test_three_d_array_accessor(get_contract_with_gas_estimation):
+def test_three_d_array_accessor(get_contract):
     three_d_array_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: DynArray[DynArray[DynArray[int128, 2], 2], 2] = [[[0, 0], [0, 0]], [[0, 0], [0, 0]]]
     a[0][0][0] = x
     a[0][0][1] = y
     a[0][1][0] = z
@@ -279,19 +279,19 @@
     a[1][0][1] = -y
     a[1][1][0] = -z
     a[1][1][1] = -w
     return a[0][0][0] * 1000 + a[0][0][1] * 100 + a[0][1][0] * 10 + a[0][1][1] + \\
         a[1][1][1] * 1000 + a[1][1][0] * 100 + a[1][0][1] * 10 + a[1][0][0]
     """
 
-    c = get_contract_with_gas_estimation(three_d_array_accessor)
+    c = get_contract(three_d_array_accessor)
     assert c.test_array(2, 7, 1, 8) == -5454
 
 
-def test_four_d_array_accessor(get_contract_with_gas_estimation):
+def test_four_d_array_accessor(get_contract):
     four_d_array_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: DynArray[DynArray[DynArray[DynArray[int128, 2], 2], 2], 2] = \\
         [[[[0, 0], [0, 0]], [[0, 0], [0, 0]]], [[[0, 0], [0, 0]], [[0, 0], [0, 0]]]]
     a[0][0][0][0] = x
     a[0][0][0][1] = y
@@ -312,19 +312,19 @@
     a[1][1][1][1] = - (w + 1)
     return a[0][0][0][0] * 1000 + a[0][0][0][1] * 100 + a[0][0][1][0] * 10 + a[0][0][1][1] + \\
         a[0][1][1][1] * 1000 + a[0][1][1][0] * 100 + a[0][1][0][1] * 10 + a[0][1][0][0] + \\
         a[1][0][0][0] * 1000 + a[1][0][0][1] * 100 + a[1][0][1][0] * 10 + a[1][0][1][1] + \\
         a[1][1][1][1] * 1000 + a[1][1][1][0] * 100 + a[1][1][0][1] * 10 + a[1][1][0][0]
     """
 
-    c = get_contract_with_gas_estimation(four_d_array_accessor)
+    c = get_contract(four_d_array_accessor)
     assert c.test_array(2, 7, 1, 8) == -10908
 
 
-def test_array_negative_accessor(get_contract_with_gas_estimation, assert_compile_failed):
+def test_array_negative_accessor(get_contract, assert_compile_failed):
     array_constant_negative_accessor = """
 FOO: constant(int128) = -1
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[4] = [0, 0, 0, 0]
     a[0] = x
     a[1] = y
@@ -343,32 +343,28 @@
     a[0] = x
     a[1] = y
     a[2] = z
     a[3] = w
     return a[-4] * 1000 + a[-3] * 100 + a[-2] * 10 + a[-1]
     """
 
-    assert_compile_failed(
-        lambda: get_contract_with_gas_estimation(array_negative_accessor), ArrayIndexException
-    )
+    assert_compile_failed(lambda: get_contract(array_negative_accessor), ArrayIndexException)
 
     two_d_array_negative_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: DynArray[DynArray[int128, 2], 2] = [[0, 0], [0, 0]]
     a[0][0] = x
     a[0][1] = y
     a[1][0] = z
     a[1][1] = w
     return a[-2][-2] * 1000 + a[-2][-1] * 100 + a[-1][-2] * 10 + a[-1][-1]
     """
 
-    assert_compile_failed(
-        lambda: get_contract_with_gas_estimation(two_d_array_negative_accessor), ArrayIndexException
-    )
+    assert_compile_failed(lambda: get_contract(two_d_array_negative_accessor), ArrayIndexException)
 
     three_d_array_negative_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: DynArray[DynArray[DynArray[int128, 2], 2], 2] = [[[0, 0], [0, 0]], [[0, 0], [0, 0]]]
     a[0][0][0] = x
     a[0][0][1] = y
@@ -379,16 +375,15 @@
     a[1][1][0] = -z
     a[1][1][1] = -w
     return a[-2][-2][-2] * 1000 + a[-2][-2][-1] * 100 + a[-2][-1][-2] * 10 + a[-2][-1][-1] + \\
         a[-1][-1][-1] * 1000 + a[-1][-1][-2] * 100 + a[-1][-2][-1] * 10 + a[-1][-2][-2]
     """
 
     assert_compile_failed(
-        lambda: get_contract_with_gas_estimation(three_d_array_negative_accessor),
-        ArrayIndexException,
+        lambda: get_contract(three_d_array_negative_accessor), ArrayIndexException
     )
 
     four_d_array_negative_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: DynArray[DynArray[DynArray[DynArray[int128, 2], 2], 2], 2] = \\
         [[[[0, 0], [0, 0]], [[0, 0], [0, 0]]], [[[0, 0], [0, 0]], [[0, 0], [0, 0]]]]
@@ -415,18 +410,15 @@
         100 + a[-2][-1][-2][-1] * 10 + a[-2][-1][-2][-2] + \\
         a[-1][-2][-2][-2] * 1000 + a[-1][-2][-2][-1] * \\
         100 + a[-1][-2][-1][-2] * 10 + a[-1][-2][-1][-1] + \\
         a[-1][-1][-1][-1] * 1000 + a[-1][-1][-1][-2] * \\
         100 + a[-1][-1][-2][-1] * 10 + a[-1][-1][-2][-2]
     """
 
-    assert_compile_failed(
-        lambda: get_contract_with_gas_estimation(four_d_array_negative_accessor),
-        ArrayIndexException,
-    )
+    assert_compile_failed(lambda: get_contract(four_d_array_negative_accessor), ArrayIndexException)
 
 
 @pytest.mark.parametrize(
     "type,values,false_value",
     [
         ("uint256", [3, 7], 4),
         (
@@ -444,78 +436,78 @@
                 "0x0000000000000000000000000000000000000000000000000000000080ac58cd",
                 "0x0000000000000000000000000000000000000000000000000000000080ac58ce",
             ],
             "0x0000000000000000000000000000000000000000000000000000000080ac58cf",
         ),
     ],
 )
-def test_member_in_list(get_contract_with_gas_estimation, type, values, false_value):
+def test_member_in_list(get_contract, type, values, false_value):
     code = f"""
 @external
 def check(a: {type}) -> bool:
     x: DynArray[{type}, 2] = [{values[0]}, {values[1]}]
     return a in x
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.check(values[0]) is True
     assert c.check(values[1]) is True
     assert c.check(false_value) is False
 
 
 @pytest.mark.parametrize("type_", ("uint256", "bytes32", "address"))
-def test_member_in_empty_list(get_contract_with_gas_estimation, type_):
+def test_member_in_empty_list(get_contract, type_):
     code = f"""
 @external
 def check_in(s: uint128) -> bool:
     a: {type_} = convert(s, {type_})
     x: DynArray[{type_}, 2] = []
     return a in x
 
 @external
 def check_not_in(s: uint128) -> bool:
     a: {type_} = convert(s, {type_})
     x: DynArray[{type_}, 2] = []
     return a not in x
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     for s in (0, 1, 2, 3):
         assert c.check_in(s) is False
         assert c.check_not_in(s) is True
 
 
 @pytest.mark.parametrize(
     "type,values,false_values",
     [
         ("uint256", [[3, 7], [9, 11]], [4, 10]),
         ("bool", [[True, True], [False, False]], [False, True]),
     ],
 )
-def test_member_in_nested_list(get_contract_with_gas_estimation, type, values, false_values):
+def test_member_in_nested_list(get_contract, type, values, false_values):
     code = f"""
 @external
 def check1(a: {type}) -> bool:
     x: DynArray[DynArray[{type}, 2], 2] = {values}
     return a in x[0]
 
 @external
 def check2(a: {type}) -> bool:
     x: DynArray[DynArray[{type}, 2], 2] = {values}
     return a in x[1]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.check1(values[0][0]) is True
     assert c.check1(values[0][1]) is True
     assert c.check1(false_values[0]) is False
 
     assert c.check2(values[1][0]) is True
     assert c.check2(values[1][1]) is True
     assert c.check2(false_values[1]) is False
 
 
-def test_member_in_nested_address_list(get_contract_with_gas_estimation):
+def test_member_in_nested_address_list(get_contract):
     code = """
 @external
 def check1(a: address) -> bool:
     x: DynArray[DynArray[address, 2], 2] = [
         [
             0x0000000000000000000000000000000000000012,
             0x0000000000000000000000000000000000000024,
@@ -537,25 +529,25 @@
         [
             0x0000000000000000000000000000000000000036,
             0x0000000000000000000000000000000000000048,
         ],
     ]
     return a in x[1]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.check1("0x0000000000000000000000000000000000000012") is True
     assert c.check1("0x0000000000000000000000000000000000000024") is True
     assert c.check1("0x0000000000000000000000000000000000000036") is False
 
     assert c.check2("0x0000000000000000000000000000000000000036") is True
     assert c.check2("0x0000000000000000000000000000000000000048") is True
     assert c.check2("0x0000000000000000000000000000000000000024") is False
 
 
-def test_member_in_nested_bytes32_list(get_contract_with_gas_estimation):
+def test_member_in_nested_bytes32_list(get_contract):
     code = """
 @external
 def check1(a: bytes32) -> bool:
     x: DynArray[DynArray[bytes32, 2], 2] = [
         [
             0x0000000000000000000000000000000000000000000000000000000080ac58ca,
             0x0000000000000000000000000000000000000000000000000000000080ac58cb,
@@ -577,38 +569,38 @@
         [
             0x0000000000000000000000000000000000000000000000000000000080ac58cc,
             0x0000000000000000000000000000000000000000000000000000000080ac58cd,
         ],
     ]
     return a in x[1]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.check1("0x0000000000000000000000000000000000000000000000000000000080ac58ca") is True
     assert c.check1("0x0000000000000000000000000000000000000000000000000000000080ac58cb") is True
     assert c.check1("0x0000000000000000000000000000000000000000000000000000000080ac58cc") is False
 
     assert c.check2("0x0000000000000000000000000000000000000000000000000000000080ac58cc") is True
     assert c.check2("0x0000000000000000000000000000000000000000000000000000000080ac58cd") is True
     assert c.check2("0x0000000000000000000000000000000000000000000000000000000080ac58ca") is False
 
 
-def test_member_in_updated_list(get_contract_with_gas_estimation):
+def test_member_in_updated_list(get_contract):
     code = """
 @external
 def foo() -> bool:
     xs: DynArray[uint256, 3] = [2, 2, 2]
     xs = [1, 1]
     y: uint256 = 2
     return y in xs
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() is False
 
 
-def test_member_in_updated_nested_list(get_contract_with_gas_estimation):
+def test_member_in_updated_nested_list(get_contract):
     code = """
 @external
 def foo() -> bool:
     xs: DynArray[DynArray[DynArray[uint256, 3], 3], 3] = [
         [[2, 2, 2], [2, 2, 2], [2, 2, 2]],
         [[2, 2, 2], [2, 2, 2], [2, 2, 2]],
         [[2, 2, 2], [2, 2, 2], [2, 2, 2]],
@@ -619,37 +611,37 @@
         [[1, 1], [1, 1], [1, 1]],
     ]
     y: uint256 = 2
     return y in xs[0][0] or y in xs[0][1] or y in xs[0][2] or \\
         y in xs[1][0] or y in xs[1][1] or y in xs[1][2] or \\
         y in xs[2][0] or y in xs[2][1] or y in xs[2][2]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() is False
 
 
-def test_member_in_list_lhs_side_effects(get_contract_with_gas_estimation):
+def test_member_in_list_lhs_side_effects(get_contract):
     code = """
 _counter: uint256
 
 @internal
 def counter() -> uint256:
     self._counter = 1
     return self._counter
 
 @external
 def bar() -> bool:
     x: DynArray[uint256, 4] = [2, 2, 2, 2]
     return self.counter() in x
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bar() is False
 
 
-def test_member_in_nested_list_lhs_side_effects(get_contract_with_gas_estimation):
+def test_member_in_nested_list_lhs_side_effects(get_contract):
     code = """
 _counter: uint256
 
 @internal
 def counter() -> uint256:
     self._counter = 1
     return self._counter
@@ -659,38 +651,38 @@
     x: DynArray[DynArray[DynArray[uint256, 4], 4], 4] = [
         [[2, 2, 2, 2], [2, 2, 2, 2], [2, 2, 2, 2]],
         [[2, 2, 2, 2], [2, 2, 2, 2], [2, 2, 2, 2]],
         [[2, 2, 2, 2], [2, 2, 2, 2], [2, 2, 2, 2]],
     ]
     return self.counter() in x[0][0]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bar() is False
 
 
-def test_member_in_list_rhs_side_effects(get_contract_with_gas_estimation):
+def test_member_in_list_rhs_side_effects(get_contract):
     code = """
 counter: uint256
 
 @internal
 def foo() -> DynArray[uint256, 3]:
     self.counter += 1
     return [0,0,0]
 
 @external
 def bar() -> uint256:
     self.counter = 0
     t: bool = self.counter in self.foo()
     return self.counter
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bar() == 1
 
 
-def test_member_in_nested_list_rhs_side_effects(get_contract_with_gas_estimation):
+def test_member_in_nested_list_rhs_side_effects(get_contract):
     code = """
 counter: uint256
 
 @internal
 def foo() -> DynArray[DynArray[DynArray[uint256, 3], 3], 3]:
     self.counter += 1
     return [
@@ -701,19 +693,19 @@
 
 @external
 def bar() -> uint256:
     self.counter = 0
     t: bool = self.counter in self.foo()[0][0]
     return self.counter
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bar() == 1
 
 
-def test_returns_lists(get_contract_with_gas_estimation):
+def test_returns_lists(get_contract):
     code = """
 @external
 def test_array_num_return() -> DynArray[DynArray[int128, 2], 2]:
     a: DynArray[DynArray[int128, 2], 2] = [empty(DynArray[int128, 2]), [3, 4]]
     return a
 
 @external
@@ -727,29 +719,29 @@
 
 @external
 def test_array_decimal_return3() -> DynArray[DynArray[decimal, 2], 2]:
     a: DynArray[DynArray[decimal, 2], 2] = [[1.0, 2.0], [3.0]]
     return a
 """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.test_array_num_return() == [[], [3, 4]]
     assert c.test_array_decimal_return1() == [
         [decimal_to_int(1)],
         [decimal_to_int(3), decimal_to_int(4)],
     ]
     assert c.test_array_decimal_return2() == [[decimal_to_int(1), decimal_to_int(2)]]
     assert c.test_array_decimal_return3() == [
         [decimal_to_int(1), decimal_to_int(2)],
         [decimal_to_int(3)],
     ]
 
 
 @pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
-def test_mult_list(get_contract_with_gas_estimation):
+def test_mult_list(get_contract):
     code = """
 nest3: DynArray[DynArray[DynArray[uint256, 2], 2], 2]
 nest4: DynArray[DynArray[DynArray[DynArray[uint256, 2], 2], 2], 2]
 
 @external
 def test_multi3_1() -> DynArray[DynArray[DynArray[uint256, 2], 2], 2]:
     l: DynArray[DynArray[DynArray[uint256, 2], 2], 2] = [[[0, 0], [0, 4]], [[0, 7], [0, 123]]]
@@ -773,31 +765,31 @@
 @external
 def test_multi4_2() -> DynArray[DynArray[DynArray[DynArray[uint256, 2], 2], 2], 2]:
     l: DynArray[DynArray[DynArray[DynArray[uint256, 2], 2], 2], 2] = [[[[1, 0], [0, 4]], [[0, 0], [0, 0]]], [[[444, 0], [0, 0]],[[1, 0], [0, 222]]]]  # noqa: E501
     self.nest4 = l
     return self.nest4
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     nest3 = [[[0, 0], [0, 4]], [[0, 7], [0, 123]]]
     assert c.test_multi3_1() == nest3
     assert c.test_multi3_2() == nest3
     nest4 = [[[[1, 0], [0, 4]], [[0, 0], [0, 0]]], [[[444, 0], [0, 0]], [[1, 0], [0, 222]]]]
     assert c.test_multi4_1() == nest4
     assert c.test_multi4_2() == nest4
 
 
-def test_uint256_accessor(get_contract_with_gas_estimation, tx_failed):
+def test_uint256_accessor(get_contract, tx_failed):
     code = """
 @external
 def bounds_check_uint256(xs: DynArray[uint256, 3], ix: uint256) -> uint256:
     return xs[ix]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     with tx_failed():
         c.bounds_check_uint256([], 0)
 
     assert c.bounds_check_uint256([1], 0) == 1
     with tx_failed():
         c.bounds_check_uint256([1], 1)
 
@@ -806,79 +798,79 @@
     with tx_failed():
         c.bounds_check_uint256([1, 2, 3], 3)
 
     # TODO do bounds checks for nested darrays
 
 
 @pytest.mark.parametrize("list_", ([], [11], [11, 12], [11, 12, 13]))
-def test_dynarray_len(get_contract_with_gas_estimation, tx_failed, list_):
+def test_dynarray_len(get_contract, tx_failed, list_):
     code = """
 @external
 def darray_len(xs: DynArray[uint256, 3]) -> uint256:
     return len(xs)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.darray_len(list_) == len(list_)
 
 
-def test_dynarray_too_large(get_contract_with_gas_estimation, tx_failed):
+def test_dynarray_too_large(get_contract, tx_failed):
     code = """
 @external
 def darray_len(xs: DynArray[uint256, 3]) -> uint256:
     return len(xs)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     with tx_failed():
         c.darray_len([1, 2, 3, 4])
 
 
-def test_int128_accessor(get_contract_with_gas_estimation, tx_failed):
+def test_int128_accessor(get_contract, tx_failed):
     code = """
 @external
 def bounds_check_int128(ix: int128) -> uint256:
     xs: DynArray[uint256, 3] = [1,2,3]
     return xs[ix]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bounds_check_int128(0) == 1
     assert c.bounds_check_int128(2) == 3
     with tx_failed():
         c.bounds_check_int128(3)
     with tx_failed():
         c.bounds_check_int128(-1)
 
 
-def test_index_exception(get_contract_with_gas_estimation, assert_compile_failed):
+def test_index_exception(get_contract, assert_compile_failed):
     code = """
 @external
 def fail() -> uint256:
     xs: DynArray[uint256, 3] = [1,2,3]
     return xs[3]
     """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), ArrayIndexException)
+    assert_compile_failed(lambda: get_contract(code), ArrayIndexException)
 
     code = """
 @external
 def fail() -> uint256:
     xs: DynArray[uint256, 3] = [1,2,3]
     return xs[-1]
     """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), ArrayIndexException)
+    assert_compile_failed(lambda: get_contract(code), ArrayIndexException)
 
 
-def test_compile_time_bounds_check(get_contract_with_gas_estimation, assert_compile_failed):
+def test_compile_time_bounds_check(get_contract, assert_compile_failed):
     code = """
 @external
 def parse_list_fail():
     xs: DynArray[uint256, 3] = [2**256, 1, 3]
     pass
     """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), OverflowException)
+    assert_compile_failed(lambda: get_contract(code), OverflowException)
 
 
 def test_2d_array_input_1(get_contract):
     code = """
 @internal
 def test_input(
     arr: DynArray[DynArray[int128, 2], 1], i: int128
@@ -889,15 +881,15 @@
 def test_values(
     arr: DynArray[DynArray[int128, 2], 1], i: int128
 ) -> (DynArray[DynArray[int128, 2], 1], int128):
     return self.test_input(arr, i)
     """
 
     c = get_contract(code)
-    assert c.test_values([[1, 2]], 3) == [[[1, 2]], 3]
+    assert c.test_values([[1, 2]], 3) == ([[1, 2]], 3)
 
 
 def test_2d_array_input_2(get_contract):
     code = """
 @internal
 def test_input(
     arr: DynArray[DynArray[int128, 2], 3],
@@ -910,15 +902,15 @@
     arr: DynArray[DynArray[int128, 2], 3],
     s: String[10]
 ) -> (DynArray[DynArray[int128, 2], 3], String[10]):
     return self.test_input(arr, s)
     """
 
     c = get_contract(code)
-    assert c.test_values([[1, 2], [3, 4], [5, 6]], "abcdef") == [[[1, 2], [3, 4], [5, 6]], "abcdef"]
+    assert c.test_values([[1, 2], [3, 4], [5, 6]], "abcdef") == ([[1, 2], [3, 4], [5, 6]], "abcdef")
 
 
 def test_nested_index_of_returned_array(get_contract):
     code = """
 @internal
 def inner() -> (int128, int128):
     return 1,2
@@ -945,15 +937,15 @@
 
 @external
 def foo() -> (uint256, uint256, uint256, uint256, uint256):
     return self._foo(2, [3, self._foo2()])
     """
 
     c = get_contract(code)
-    assert c.foo() == [1, 2, 3, 4, 5]
+    assert c.foo() == (1, 2, 3, 4, 5)
 
 
 def test_nested_calls_inside_arrays_with_index_access(get_contract):
     code = """
 @internal
 def _foo(
     a: DynArray[uint256, 2],
@@ -968,15 +960,15 @@
 
 @external
 def foo() -> (uint256, uint256, uint256, uint256, uint256):
     return self._foo([7, self._foo2()[0]], [11, self._foo2()[1]])
     """
 
     c = get_contract(code)
-    assert c.foo() == [1, 2, 3, 4, 5]
+    assert c.foo() == (1, 2, 3, 4, 5)
 
 
 append_pop_tests = [
     (
         """
 my_array: DynArray[uint256, 5]
 @external
@@ -1020,27 +1012,27 @@
 my_array: DynArray[uint256, 5]
 @external
 def foo(xs: DynArray[uint256, 5]) -> (DynArray[uint256, 5], uint256):
     for x: uint256 in xs:
         self.my_array.append(x)
     return self.my_array, self.my_array.pop()
     """,
-        lambda xs: None if len(xs) == 0 else [xs, xs[-1]],
+        lambda xs: None if len(xs) == 0 else (xs, xs[-1]),
     ),
     # check order of evaluation.
     (
         """
 my_array: DynArray[uint256, 5]
 @external
 def foo(xs: DynArray[uint256, 5]) -> (uint256, DynArray[uint256, 5]):
     for x: uint256 in xs:
         self.my_array.append(x)
     return self.my_array.pop(), self.my_array
     """,
-        lambda xs: None if len(xs) == 0 else [xs[-1], xs[:-1]],
+        lambda xs: None if len(xs) == 0 else (xs[-1], xs[:-1]),
     ),
     # test memory arrays
     (
         """
 @external
 def foo(xs: DynArray[uint256, 5]) -> DynArray[uint256, 5]:
     ys: DynArray[uint256, 5] = []
@@ -1205,15 +1197,15 @@
         # None is sentinel to indicate txn should revert
         with tx_failed():
             c.foo(test_data)
     else:
         assert c.foo(test_data) == expected_result
 
 
-append_pop_complex_tests = [
+append_pop_complex_tests: list[tuple[str, Callable[[Any], Any]]] = [
     (
         """
 @external
 def foo(x: {typ}) -> DynArray[{typ}, 2]:
     ys: DynArray[{typ}, 1] = []
     ys.append(x)
     return ys
@@ -1235,25 +1227,25 @@
         """
 my_array: DynArray[{typ}, 5]
 @external
 def foo(x: {typ}) -> (DynArray[{typ}, 5], {typ}):
     self.my_array.append(x)
     return self.my_array, self.my_array.pop()
     """,
-        lambda x: [[x], x],
+        lambda x: ([x], x),
     ),
     (
         """
 my_array: DynArray[{typ}, 5]
 @external
 def foo(x: {typ}) -> ({typ}, DynArray[{typ}, 5]):
     self.my_array.append(x)
     return self.my_array.pop(), self.my_array
     """,
-        lambda x: [x, []],
+        lambda x: (x, []),
     ),
     (
         """
 my_array: DynArray[{typ}, 5]
 @external
 def foo(x: {typ}) -> {typ}:
     return self.my_array.pop()
@@ -1319,15 +1311,15 @@
         1,
         14-self._foo2()[0],
         self._foo([7,self._foo2()[0]], [11,self._foo2()[1]])[2]
     ]
     return 666, x, [88, self._foo2()[0]]
     """
     c = get_contract(code)
-    assert c.foo() == [666, [1, 2, 3], [88, 12]]
+    assert c.foo() == (666, [1, 2, 3], [88, 12])
 
 
 def test_list_of_structs_arg(get_contract):
     code = """
 flag Foobar:
     FOO
     BAR
@@ -1487,15 +1479,14 @@
     return a[0][0][0] * a[1][1][1]
     """
     c = get_contract(code)
     assert c.bar(7) == [[[7, 14], [21, 28]], [[35, 42], [49, 56]]]
     assert c.foo(7) == 392
 
 
-@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_struct_of_lists(get_contract):
     code = """
 struct Foo:
     a1: DynArray[uint256, 2]
     a2: DynArray[DynArray[uint256, 2], 2]
     a3: DynArray[DynArray[DynArray[uint256, 2], 2], 2]
 
@@ -1576,15 +1567,14 @@
     f: Foo = self._foo(x)
     return f.a
     """
     c = get_contract(code)
     assert c.bar(7) == [7, 14]
 
 
-@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_nested_struct_of_lists(get_contract, assert_compile_failed, optimize):
     code = """
 struct nestedFoo:
     a1: DynArray[DynArray[DynArray[uint256, 2], 2], 2]
 
 struct Foo:
     b1: DynArray[DynArray[DynArray[nestedFoo, 2], 2], 2]
@@ -1706,17 +1696,15 @@
 @pytest.mark.parametrize(
     "typ,val",
     [
         ("DynArray[DynArray[uint256, 5], 5]", [[], []]),
         ("DynArray[DynArray[DynArray[uint256, 5], 5], 5]", [[[], []], []]),
     ],
 )
-def test_empty_nested_dynarray(get_contract, typ, val, venom_xfail):
-    if val == [[[], []], []]:
-        venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
+def test_empty_nested_dynarray(get_contract, typ, val):
     code = f"""
 @external
 def foo() -> {typ}:
     a: {typ} = {val}
     return a
     """
     c = get_contract(code)
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_flag.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_flag.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def set_and_get(a: Actions) -> Actions:
     self.action = a
     return self.action
     """
     c = get_contract(code)
     for i in range(5):
         assert c.set_and_get(i) == i
-        c.set_and_get(i, transact={})
+        c.set_and_get(i)
         assert c.action() == i
 
 
 def test_eq_neq(get_contract):
     code = """
 flag Roles:
     USER
@@ -148,15 +148,15 @@
         c.bor_arg(3, 32)
     with tx_failed():
         c.band_arg(3, 32)
     with tx_failed():
         c.bxor_arg(3, 32)
 
 
-def test_augassign_storage(get_contract, w3, tx_failed):
+def test_augassign_storage(get_contract, env, tx_failed):
     code = """
 flag Roles:
     ADMIN
     MINTER
 
 roles: public(HashMap[address, Roles])
 
@@ -182,53 +182,53 @@
 @external
 def checkMinter(minter: address):
     assert Roles.MINTER in self.roles[minter]
     """
     c = get_contract(code)
 
     # check admin
-    admin_address = w3.eth.accounts[0]
-    minter_address = w3.eth.accounts[1]
+    admin_address = env.deployer
+    minter_address = env.accounts[1]
 
     # add minter
-    c.addMinter(minter_address, transact={})
+    c.addMinter(minter_address)
     c.checkMinter(minter_address)
 
     assert c.roles(admin_address) == 0b01
     assert c.roles(minter_address) == 0b10
 
     # admin is not a minter
     with tx_failed():
         c.checkMinter(admin_address)
 
-    c.addMinter(admin_address, transact={})
+    c.addMinter(admin_address)
 
     # now, admin is a minter
     assert c.roles(admin_address) == 0b11
     c.checkMinter(admin_address)
 
     # revoke minter
-    c.revokeMinter(admin_address, transact={})
+    c.revokeMinter(admin_address)
     assert c.roles(admin_address) == 0b01
     with tx_failed():
         c.checkMinter(admin_address)
 
     # flip minter
-    c.flipMinter(admin_address, transact={})
+    c.flipMinter(admin_address)
     assert c.roles(admin_address) == 0b11
     c.checkMinter(admin_address)
 
     # flip minter
-    c.flipMinter(admin_address, transact={})
+    c.flipMinter(admin_address)
     assert c.roles(admin_address) == 0b01
     with tx_failed():
         c.checkMinter(admin_address)
 
 
-def test_in_flag(get_contract_with_gas_estimation):
+def test_in_flag(get_contract):
     code = """
 flag Roles:
     USER
     STAFF
     ADMIN
     MANAGER
     CEO
@@ -248,15 +248,15 @@
 @external
 def baz(a: Roles) -> bool:
     x: Roles = Roles.USER | Roles.ADMIN | Roles.CEO
     y: Roles = x ^ (Roles.MANAGER | Roles.CEO)  # flip off CEO, flip on MANAGER
     return a in (x & y)
 
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.foo() is True
 
     # CEO MANAGER ADMIN STAFF USER
     #   1       1     1     1    1
 
     assert c.bar(0b00001) is True  # Roles.USER should pass
     assert c.bar(0b00010) is False  # Roles.STAFF should fail
@@ -265,41 +265,41 @@
     assert c.bar2(0b00010) is True  # Roles.STAFF should pass
 
     assert c.baz(0b00001) is True  # Roles.USER should pass
     assert c.baz(0b00100) is True  # Roles.ADMIN should pass
     assert c.baz(0b01000) is False  # Roles.MANAGER should fail
 
 
-def test_struct_with_flag(get_contract_with_gas_estimation):
+def test_struct_with_flag(get_contract):
     code = """
 flag Foobar:
     FOO
     BAR
 
 struct Foo:
     a: uint256
     b: Foobar
 
 @external
 def get_flag_from_struct() -> Foobar:
     f: Foo = Foo(a=1, b=Foobar.BAR)
     return f.b
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.get_flag_from_struct() == 2
 
 
-def test_mapping_with_flag(get_contract_with_gas_estimation):
+def test_mapping_with_flag(get_contract):
     code = """
 flag Foobar:
     FOO
     BAR
 
 fb: HashMap[Foobar, uint256]
 
 @external
 def get_key(f: Foobar, i: uint256) -> uint256:
     self.fb[f] = i
     return self.fb[f]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.get_key(1, 777) == 777
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_identifier_naming.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_identifier_naming.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_lists.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_lists.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         if isinstance(x, list):
             ret.append(_map_nested(f, x))
         else:
             ret.append(f(x))
     return ret
 
 
-def test_list_tester_code(get_contract_with_gas_estimation):
+def test_list_tester_code(get_contract):
     list_tester_code = """
 z: int128[3]
 z2: int128[2][2]
 z3: int128[2]
 
 @external
 def foo(x: int128[3]) -> int128:
@@ -49,25 +49,25 @@
 @external
 def loo(x: int128[2][2]) -> int128:
     self.z2 = x
     self.z3 = x[1]
     return self.z2[0][0] + self.z2[0][1] + self.z3[0] * 10 + self.z3[1] * 10
     """
 
-    c = get_contract_with_gas_estimation(list_tester_code)
+    c = get_contract(list_tester_code)
     assert c.foo([3, 4, 5]) == 12
     assert c.goo([[1, 2], [3, 4]]) == 73
     assert c.hoo([3, 4, 5]) == 12
     assert c.joo([[1, 2], [3, 4]]) == 73
     assert c.koo([3, 4, 5]) == 12
     assert c.loo([[1, 2], [3, 4]]) == 73
     print("Passed list tests")
 
 
-def test_list_output_tester_code(get_contract_with_gas_estimation):
+def test_list_output_tester_code(get_contract):
     list_output_tester_code = """
 z: int128[2]
 
 @external
 def foo() -> int128[2]:
     return [3, 5]
 
@@ -114,15 +114,15 @@
     return [inp, [3,4]]
 
 @external
 def roo(inp: decimal[2]) -> decimal[2][2]:
     return [inp, [3.0, 4.0]]
     """
 
-    c = get_contract_with_gas_estimation(list_output_tester_code)
+    c = get_contract(list_output_tester_code)
     assert c.foo() == [3, 5]
     assert c.goo() == [3, 5]
     assert c.hoo() == [3, 5]
     assert c.joo() == [3, 5]
     assert c.koo() == [[1, 2], [3, 4]]
     assert c.loo() == [[1, 2], [3, 4]]
     assert c.moo() == [[1, 2], [3, 4]]
@@ -130,49 +130,49 @@
     assert c.poo([[1, 2], [3, 4]]) == [[1, 2], [3, 4]]
     assert c.qoo([1, 2]) == [[1, 2], [3, 4]]
     assert c.roo(_map_nested(decimal_to_int, [1.0, 2.0])) == _map_nested(
         decimal_to_int, [[1.0, 2.0], [3.0, 4.0]]
     )
 
 
-def test_array_accessor(get_contract_with_gas_estimation):
+def test_array_accessor(get_contract):
     array_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[4] = [0, 0, 0, 0]
     a[0] = x
     a[1] = y
     a[2] = z
     a[3] = w
     return a[0] * 1000 + a[1] * 100 + a[2] * 10 + a[3]
     """
 
-    c = get_contract_with_gas_estimation(array_accessor)
+    c = get_contract(array_accessor)
     assert c.test_array(2, 7, 1, 8) == 2718
     print("Passed basic array accessor test")
 
 
-def test_two_d_array_accessor(get_contract_with_gas_estimation):
+def test_two_d_array_accessor(get_contract):
     two_d_array_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[2][2] = [[0, 0], [0, 0]]
     a[0][0] = x
     a[0][1] = y
     a[1][0] = z
     a[1][1] = w
     return a[0][0] * 1000 + a[0][1] * 100 + a[1][0] * 10 + a[1][1]
     """
 
-    c = get_contract_with_gas_estimation(two_d_array_accessor)
+    c = get_contract(two_d_array_accessor)
     assert c.test_array(2, 7, 1, 8) == 2718
     print("Passed complex array accessor test")
 
 
-def test_three_d_array_accessor(get_contract_with_gas_estimation):
+def test_three_d_array_accessor(get_contract):
     three_d_array_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[2][2][2] = [[[0, 0], [0, 0]], [[0, 0], [0, 0]]]
     a[0][0][0] = x
     a[0][0][1] = y
     a[0][1][0] = z
@@ -181,19 +181,19 @@
     a[1][0][1] = -y
     a[1][1][0] = -z
     a[1][1][1] = -w
     return a[0][0][0] * 1000 + a[0][0][1] * 100 + a[0][1][0] * 10 + a[0][1][1] + \\
         a[1][1][1] * 1000 + a[1][1][0] * 100 + a[1][0][1] * 10 + a[1][0][0]
     """
 
-    c = get_contract_with_gas_estimation(three_d_array_accessor)
+    c = get_contract(three_d_array_accessor)
     assert c.test_array(2, 7, 1, 8) == -5454
 
 
-def test_four_d_array_accessor(get_contract_with_gas_estimation):
+def test_four_d_array_accessor(get_contract):
     four_d_array_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[2][2][2][2] = \\
         [[[[0, 0], [0, 0]], [[0, 0], [0, 0]]], [[[0, 0], [0, 0]], [[0, 0], [0, 0]]]]
     a[0][0][0][0] = x
     a[0][0][0][1] = y
@@ -214,48 +214,44 @@
     a[1][1][1][1] = - (w + 1)
     return a[0][0][0][0] * 1000 + a[0][0][0][1] * 100 + a[0][0][1][0] * 10 + a[0][0][1][1] + \\
         a[0][1][1][1] * 1000 + a[0][1][1][0] * 100 + a[0][1][0][1] * 10 + a[0][1][0][0] + \\
         a[1][0][0][0] * 1000 + a[1][0][0][1] * 100 + a[1][0][1][0] * 10 + a[1][0][1][1] + \\
         a[1][1][1][1] * 1000 + a[1][1][1][0] * 100 + a[1][1][0][1] * 10 + a[1][1][0][0]
     """
 
-    c = get_contract_with_gas_estimation(four_d_array_accessor)
+    c = get_contract(four_d_array_accessor)
     assert c.test_array(2, 7, 1, 8) == -10908
 
 
-def test_array_negative_accessor(get_contract_with_gas_estimation, assert_compile_failed):
+def test_array_negative_accessor(get_contract, assert_compile_failed):
     array_negative_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[4] = [0, 0, 0, 0]
     a[0] = x
     a[1] = y
     a[2] = z
     a[3] = w
     return a[-4] * 1000 + a[-3] * 100 + a[-2] * 10 + a[-1]
     """
 
-    assert_compile_failed(
-        lambda: get_contract_with_gas_estimation(array_negative_accessor), ArrayIndexException
-    )
+    assert_compile_failed(lambda: get_contract(array_negative_accessor), ArrayIndexException)
 
     two_d_array_negative_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[2][2] = [[0, 0], [0, 0]]
     a[0][0] = x
     a[0][1] = y
     a[1][0] = z
     a[1][1] = w
     return a[-2][-2] * 1000 + a[-2][-1] * 100 + a[-1][-2] * 10 + a[-1][-1]
     """
 
-    assert_compile_failed(
-        lambda: get_contract_with_gas_estimation(two_d_array_negative_accessor), ArrayIndexException
-    )
+    assert_compile_failed(lambda: get_contract(two_d_array_negative_accessor), ArrayIndexException)
 
     three_d_array_negative_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[2][2][2] = [[[0, 0], [0, 0]], [[0, 0], [0, 0]]]
     a[0][0][0] = x
     a[0][0][1] = y
@@ -266,16 +262,15 @@
     a[1][1][0] = -z
     a[1][1][1] = -w
     return a[-2][-2][-2] * 1000 + a[-2][-2][-1] * 100 + a[-2][-1][-2] * 10 + a[-2][-1][-1] + \\
         a[-1][-1][-1] * 1000 + a[-1][-1][-2] * 100 + a[-1][-2][-1] * 10 + a[-1][-2][-2]
     """
 
     assert_compile_failed(
-        lambda: get_contract_with_gas_estimation(three_d_array_negative_accessor),
-        ArrayIndexException,
+        lambda: get_contract(three_d_array_negative_accessor), ArrayIndexException
     )
 
     four_d_array_negative_accessor = """
 @external
 def test_array(x: int128, y: int128, z: int128, w: int128) -> int128:
     a: int128[2][2][2][2] = \\
         [[[[0, 0], [0, 0]], [[0, 0], [0, 0]]], [[[0, 0], [0, 0]], [[0, 0], [0, 0]]]]
@@ -302,21 +297,18 @@
         a[-2][-1][-2][-1] * 10 + a[-2][-1][-2][-2] + \\
         a[-1][-2][-2][-2] * 1000 + a[-1][-2][-2][-1] * 100 + \\
         a[-1][-2][-1][-2] * 10 + a[-1][-2][-1][-1] + \\
         a[-1][-1][-1][-1] * 1000 + a[-1][-1][-1][-2] * 100 + \\
         a[-1][-1][-2][-1] * 10 + a[-1][-1][-2][-2]
     """
 
-    assert_compile_failed(
-        lambda: get_contract_with_gas_estimation(four_d_array_negative_accessor),
-        ArrayIndexException,
-    )
+    assert_compile_failed(lambda: get_contract(four_d_array_negative_accessor), ArrayIndexException)
 
 
-def test_returns_lists(get_contract_with_gas_estimation):
+def test_returns_lists(get_contract):
     code = """
 @external
 def test_array_num_return() -> int128[2][2]:
     a: int128[2][2] = [[1, 2], [3, 4]]
     return a
 
 @external
@@ -330,130 +322,130 @@
 
 @external
 def test_array_decimal_return3() -> decimal[2][2]:
     a: decimal[2][2] = [[1.0, 2.0], [3.0, 4.0]]
     return a
 """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.test_array_num_return() == [[1, 2], [3, 4]]
     assert c.test_array_decimal_return1() == _map_nested(decimal_to_int, [[1.0, 2.0], [3.0, 4.0]])
     assert c.test_array_decimal_return2() == _map_nested(decimal_to_int, [[1.0, 2.0], [3.0, 4.0]])
     assert c.test_array_decimal_return3() == _map_nested(decimal_to_int, [[1.0, 2.0], [3.0, 4.0]])
 
 
-def test_mult_list(get_contract_with_gas_estimation):
+def test_mult_list(get_contract):
     code = """
 @external
 def test_multi3() -> uint256[2][2][2]:
     l: uint256[2][2][2] = [[[0, 0], [0, 4]], [[0, 0], [0, 123]]]
     return l
 
 @external
 def test_multi4() -> uint256[2][2][2][2]:
     l: uint256[2][2][2][2] = [[[[1, 0], [0, 4]], [[0, 0], [0, 0]]], [[[444, 0], [0, 0]],[[1, 0], [0, 222]]]]  # noqa: E501
     return l
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.test_multi3() == [[[0, 0], [0, 4]], [[0, 0], [0, 123]]]
     assert c.test_multi4() == [
         [[[1, 0], [0, 4]], [[0, 0], [0, 0]]],
         [[[444, 0], [0, 0]], [[1, 0], [0, 222]]],
     ]
 
 
 @pytest.mark.parametrize("type_", ["uint8", "uint256"])
-def test_unsigned_accessors(get_contract_with_gas_estimation, tx_failed, type_):
+def test_unsigned_accessors(get_contract, tx_failed, type_):
     code = f"""
 @external
 def bounds_check(ix: {type_}) -> uint256:
     xs: uint256[3] = [1,2,3]
     return xs[ix]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bounds_check(0) == 1
     assert c.bounds_check(2) == 3
     with tx_failed():
         c.bounds_check(3)
 
 
 @pytest.mark.parametrize("type_", ["int128", "int256"])
-def test_signed_accessors(get_contract_with_gas_estimation, tx_failed, type_):
+def test_signed_accessors(get_contract, tx_failed, type_):
     code = f"""
 @external
 def bounds_check(ix: {type_}) -> uint256:
     xs: uint256[3] = [1,2,3]
     return xs[ix]
     """
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.bounds_check(0) == 1
     assert c.bounds_check(2) == 3
     with tx_failed():
         c.bounds_check(3)
     with tx_failed():
         c.bounds_check(-1)
 
 
-def test_list_check_heterogeneous_types(get_contract_with_gas_estimation, assert_compile_failed):
+def test_list_check_heterogeneous_types(get_contract, assert_compile_failed):
     code = """
 @external
 def fail() -> uint256:
     xs: uint256[3] = [1,2,3]
     return xs[3]
     """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), ArrayIndexException)
+    assert_compile_failed(lambda: get_contract(code), ArrayIndexException)
     code = """
 @external
 def fail() -> uint256:
     xs: uint256[3] = [1,2,3]
     return xs[-1]
     """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), ArrayIndexException)
+    assert_compile_failed(lambda: get_contract(code), ArrayIndexException)
 
 
-def test_compile_time_bounds_check(get_contract_with_gas_estimation, assert_compile_failed):
+def test_compile_time_bounds_check(get_contract, assert_compile_failed):
     code = """
 @external
 def parse_list_fail():
     xs: uint256[3] = [2**256, 1, 3]
     pass
     """
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(code), OverflowException)
+    assert_compile_failed(lambda: get_contract(code), OverflowException)
 
 
 def test_2d_array_input_1(get_contract):
     code = """
 @internal
 def test_input(arr: int128[2][1], i: int128) -> (int128[2][1], int128):
     return arr, i
 
 @external
 def test_values(arr: int128[2][1], i: int128) -> (int128[2][1], int128):
     return self.test_input(arr, i)
     """
 
     c = get_contract(code)
-    assert c.test_values([[1, 2]], 3) == [[[1, 2]], 3]
+    assert c.test_values([[1, 2]], 3) == ([[1, 2]], 3)
 
 
 def test_2d_array_input_2(get_contract):
     code = """
 @internal
 def test_input(arr: int128[2][3], s: String[10]) -> (int128[2][3], String[10]):
     return arr, s
 
 @external
 def test_values(arr: int128[2][3], s: String[10]) -> (int128[2][3], String[10]):
     return self.test_input(arr, s)
     """
 
     c = get_contract(code)
-    assert c.test_values([[1, 2], [3, 4], [5, 6]], "abcdef") == [[[1, 2], [3, 4], [5, 6]], "abcdef"]
+    assert c.test_values([[1, 2], [3, 4], [5, 6]], "abcdef") == ([[1, 2], [3, 4], [5, 6]], "abcdef")
 
 
 def test_nested_index_of_returned_array(get_contract):
     code = """
 @internal
 def inner() -> (int128, int128):
     return 1,2
@@ -480,15 +472,15 @@
 
 @external
 def foo() -> (uint256, uint256, uint256, uint256, uint256):
     return self._foo(2, [3, self._foo2()])
     """
 
     c = get_contract(code)
-    assert c.foo() == [1, 2, 3, 4, 5]
+    assert c.foo() == (1, 2, 3, 4, 5)
 
 
 def test_nested_calls_inside_arrays_with_index_access(get_contract):
     code = """
 @internal
 def _foo(a: uint256[2], b: uint256[2]) -> (uint256, uint256, uint256, uint256, uint256):
     return a[1]-b[0], 2, a[0]-b[1], 8-b[1], 5
@@ -500,15 +492,15 @@
 
 @external
 def foo() -> (uint256, uint256, uint256, uint256, uint256):
     return self._foo([7, self._foo2()[0]], [11, self._foo2()[1]])
     """
 
     c = get_contract(code)
-    assert c.foo() == [1, 2, 3, 4, 5]
+    assert c.foo() == (1, 2, 3, 4, 5)
 
 
 def test_so_many_things_you_should_never_do(get_contract):
     code = """
 @internal
 def _foo(a: uint256[2], b: uint256[2]) -> uint256[5]:
     return [a[1]-b[0], 2, a[0]-b[1], 8-b[1], 5]
@@ -521,15 +513,15 @@
 
 @external
 def foo() -> (uint256, uint256[3], uint256[2]):
     x: uint256[3] = [1, 14-self._foo2()[0], self._foo([7,self._foo2()[0]], [11,self._foo2()[1]])[2]]
     return 666, x, [88, self._foo2()[0]]
     """
     c = get_contract(code)
-    assert c.foo() == [666, [1, 2, 3], [88, 12]]
+    assert c.foo() == (666, [1, 2, 3], [88, 12])
 
 
 def test_list_of_dynarray(get_contract):
     code = """
 @external
 def bar(x: int128) -> DynArray[int128, 2][2]:
     a: DynArray[int128, 2][2] = [[x, x * 2], [x * 3, x * 4]]
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_node_types.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_node_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_string.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_string.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,76 @@
 import pytest
 
-pytestmark = pytest.mark.usefixtures("memory_mocker")
 
-
-def test_string_return(get_contract_with_gas_estimation):
+def test_string_return(get_contract):
     code = """
 @external
 def testb() -> String[100]:
     a: String[100] = "test return"
     return a
 
 @external
 def testa(inp: String[100]) -> String[100]:
     return inp
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.testa("meh") == "meh"
     assert c.testb() == "test return"
 
 
-def test_string_concat(get_contract_with_gas_estimation):
+def test_string_concat(get_contract):
     code = """
 @external
 def testb(inp: String[10]) -> String[128]:
     a: String[100] = "return message:"
     b: String[128] = concat(a, " ", inp)
     return b
 
 @external
 def testa(inp: String[10]) -> String[160]:
     a: String[100] = "<-- return message"
     return concat("Funny ", inp, " ", inp, a)
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.testb("bob") == "return message: bob"
     assert c.testa("foo") == "Funny foo foo<-- return message"
 
 
-def test_basic_long_string_as_keys(get_contract, w3):
+def test_basic_long_string_as_keys(get_contract):
     code = """
 mapped_string: HashMap[String[34], int128]
 
 @external
 def set(k: String[34], v: int128):
     self.mapped_string[k] = v
 
 @external
 def get(k: String[34]) -> int128:
     return self.mapped_string[k]
     """
 
     c = get_contract(code)
 
-    c.set("a" * 34, 6789, transact={"gas": 10**6})
+    c.set("a" * 34, 6789, gas=10**6)
 
     assert c.get("a" * 34) == 6789
 
 
-def test_string_slice(get_contract_with_gas_estimation, tx_failed):
+def test_string_slice(get_contract, tx_failed):
     test_slice4 = """
 @external
 def foo(inp: String[10], start: uint256, _len: uint256) -> String[10]:
     return slice(inp, start, _len)
     """
 
-    c = get_contract_with_gas_estimation(test_slice4)
+    c = get_contract(test_slice4)
     assert c.foo("badminton", 3, 3) == "min"
     assert c.foo("badminton", 0, 9) == "badminton"
     assert c.foo("badminton", 1, 8) == "adminton"
     assert c.foo("badminton", 1, 7) == "adminto"
     assert c.foo("badminton", 1, 0) == ""
     assert c.foo("badminton", 9, 0) == ""
 
@@ -82,15 +80,15 @@
         c.foo("badminton", 1, 9)
     with tx_failed():
         c.foo("badminton", 9, 1)
     with tx_failed():
         c.foo("badminton", 10, 0)
 
 
-def test_private_string(get_contract_with_gas_estimation):
+def test_private_string(get_contract):
     private_test_code = """
 greeting: public(String[100])
 
 @deploy
 def __init__():
     self.greeting = "Hello "
 
@@ -100,40 +98,41 @@
 
 @external
 def hithere(name: String[100]) -> String[200]:
     d: String[200] = self.construct(name)
     return d
     """
 
-    c = get_contract_with_gas_estimation(private_test_code)
+    c = get_contract(private_test_code)
     assert c.hithere("bob") == "Hello bob"
     assert c.hithere("alice") == "Hello alice"
 
 
-def test_logging_extended_string(get_contract_with_gas_estimation, get_logs):
+def test_logging_extended_string(get_contract, get_logs):
     code = """
 event MyLog:
     arg1: int128
     arg2: String[64]
     arg3: int128
 
 @external
 def foo():
     log MyLog(667788, 'hellohellohellohellohellohellohellohellohello', 334455)
     """
 
-    c = get_contract_with_gas_estimation(code)
-    log = get_logs(c.foo(transact={}), c, "MyLog")
+    c = get_contract(code)
+    c.foo()
+    (log,) = get_logs(c, "MyLog")
 
-    assert log[0].args.arg1 == 667788
-    assert log[0].args.arg2 == "hello" * 9
-    assert log[0].args.arg3 == 334455
+    assert log.args.arg1 == 667788
+    assert log.args.arg2 == "hello" * 9
+    assert log.args.arg3 == 334455
 
 
-def test_tuple_return_external_contract_call_string(get_contract_with_gas_estimation):
+def test_tuple_return_external_contract_call_string(get_contract):
     contract_1 = """
 @external
 def out_literals() -> (int128, address, String[10]):
     return 1, 0x0000000000000000000000000000000000000123, "random"
     """
 
     contract_2 = """
@@ -144,32 +143,32 @@
 def test(addr: address) -> (int128, address, String[10]):
     a: int128 = 0
     b: address = empty(address)
     c: String[10] = ""
     (a, b, c) = staticcall Test(addr).out_literals()
     return a, b,c
     """
-    c1 = get_contract_with_gas_estimation(contract_1)
-    c2 = get_contract_with_gas_estimation(contract_2)
+    c1 = get_contract(contract_1)
+    c2 = get_contract(contract_2)
 
-    assert c1.out_literals() == [1, "0x0000000000000000000000000000000000000123", "random"]
-    assert c2.test(c1.address) == [1, "0x0000000000000000000000000000000000000123", "random"]
+    assert c1.out_literals() == (1, "0x0000000000000000000000000000000000000123", "random")
+    assert c2.test(c1.address) == (1, "0x0000000000000000000000000000000000000123", "random")
 
 
-def test_default_arg_string(get_contract_with_gas_estimation):
+def test_default_arg_string(get_contract):
     code = """
 @external
 def test(a: uint256, b: String[50] = "foo") -> Bytes[100]:
     return concat(
         convert(a, bytes32),
         convert(b, Bytes[50])
     )
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.test(12345)[-3:] == b"foo"
     assert c.test(12345, "bar")[-3:] == b"bar"
 
 
 string_equality_tests = [
     (
@@ -185,15 +184,15 @@
     (32, "", "\1"),
     (33, "", "\1"),
     (33, "", "\0"),
 ]
 
 
 @pytest.mark.parametrize("len_,a,b", string_equality_tests)
-def test_string_equality(get_contract_with_gas_estimation, len_, a, b):
+def test_string_equality(get_contract, len_, a, b):
     # fixtures to initialize strings with dirty bytes
     a_init = "\\1" * len_
     b_init = "\\2" * len_
     string1 = a.encode("unicode_escape").decode("utf-8")
     string2 = b.encode("unicode_escape").decode("utf-8")
     code = f"""
 a: String[{len_}]
@@ -328,15 +327,15 @@
     self.a = "{a_init}"
     b: String[{len_}] = "{b_init}"
     self.a = "{string1}"
     b = "{string1}"
     return self.a != b
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
     assert c.equal_true() is True
     assert c.equal_false() is False
     assert c.not_equal_true() is True
     assert c.not_equal_false() is False
     assert c.literal_equal_true() is True
     assert c.literal_equal_false() is False
     assert c.literal_not_equal_true() is True
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_string_literal.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_string_literal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-def test_string_literal_return(get_contract_with_gas_estimation):
+def test_string_literal_return(get_contract):
     code = """
 @external
 def test() -> String[100]:
     return "hello world!"
 
 
 @external
 def testb() -> Bytes[100]:
     return b"hello world!"
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.test() == "hello world!"
     assert c.testb() == b"hello world!"
 
 
-def test_string_convert(get_contract_with_gas_estimation):
+def test_string_convert(get_contract):
     code = """
 @external
 def testb() -> String[100]:
     return convert(b"hello world!", String[100])
 
 @external
 def testbb() -> String[100]:
     return convert(convert("hello world!", Bytes[100]), String[100])
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.testb() == "hello world!"
     assert c.testbb() == "hello world!"
 
 
-def test_str_assign(get_contract_with_gas_estimation):
+def test_str_assign(get_contract):
     code = """
 @external
 def test() -> String[100]:
     a: String[100] = "baba black sheep"
     return a
     """
 
-    c = get_contract_with_gas_estimation(code)
+    c = get_contract(code)
 
     assert c.test() == "baba black sheep"
```

### Comparing `vyper-0.4.0rc2/tests/functional/codegen/types/test_struct.py` & `vyper-0.4.0rc3/tests/functional/codegen/types/test_struct.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,18 +17,16 @@
     human.animal.fur = slice(concat(human.animal.fur, " is great"), 0, 13)
 
     return human
     """
     c = get_contract(code)
     addr1 = "0x1234567890123456789012345678901234567890"
     addr2 = "0x1234567890123456789012345678900000000000"
-    # assert c.modify_nested_tuple([addr1, 123], [addr2, 456]) == [[addr1, 124], [addr2, 457]]
-    assert c.modify_nested_struct(
-        {"location": addr1, "animal": {"location": addr2, "fur": "wool"}}
-    ) == (addr1, (addr2, "wool is great"))
+    # assert c.modify_nested_tuple([addr1, 123], [addr2, 456]) == ([addr1, 124], [addr2, 457])
+    assert c.modify_nested_struct((addr1, (addr2, "wool"))) == (addr1, (addr2, "wool is great"))
 
 
 def test_nested_single_struct(get_contract):
     code = """
 struct Animal:
     fur: String[32]
 
@@ -43,8 +41,8 @@
     # (13 is the length of the result)
     human.animal.fur = slice(concat(human.animal.fur, " is great"), 0, 13)
 
     return human
     """
     c = get_contract(code)
 
-    assert c.modify_nested_single_struct({"animal": {"fur": "wool"}}) == (("wool is great",),)
+    assert c.modify_nested_single_struct((("wool",),)) == (("wool is great",),)
```

### Comparing `vyper-0.4.0rc2/tests/functional/examples/auctions/test_simple_open_auction.py` & `vyper-0.4.0rc3/tests/functional/examples/auctions/test_simple_open_auction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,105 @@
 import pytest
 
+from tests.utils import ZERO_ADDRESS
+
 EXPIRY = 16
 
 
-@pytest.fixture
-def auction_start(w3):
-    return w3.eth.get_block("latest").timestamp + 1
+@pytest.fixture(scope="module")
+def auction_start(env):
+    return env.timestamp + 1
 
 
-@pytest.fixture
-def auction_contract(w3, get_contract, auction_start):
+@pytest.fixture(scope="module")
+def auction_contract(env, get_contract, auction_start):
     with open("examples/auctions/simple_open_auction.vy") as f:
         contract_code = f.read()
-        contract = get_contract(contract_code, *[w3.eth.accounts[0], auction_start, EXPIRY])
-    return contract
 
+    for acc in env.accounts[:5]:
+        env.set_balance(acc, 10**20)
+
+    env.timestamp += 1  # make sure auction has started
+    return get_contract(contract_code, *[env.accounts[0], auction_start, EXPIRY])
 
-def test_initial_state(w3, tester, auction_contract, auction_start):
+
+def test_initial_state(env, auction_contract, auction_start):
     # Check beneficiary is correct
-    assert auction_contract.beneficiary() == w3.eth.accounts[0]
+    assert auction_contract.beneficiary() == env.accounts[0]
     # Check start time is `auction_start`
     assert auction_contract.auctionStart() == auction_start
     # Check time difference between start time and end time is EXPIRY
     assert auction_contract.auctionEnd() == auction_contract.auctionStart() + EXPIRY
     # Check auction has not ended
     assert auction_contract.ended() is False
     # Check highest bidder is empty
-    assert auction_contract.highestBidder() is None
+    assert auction_contract.highestBidder() == ZERO_ADDRESS
     # Check highest bid is 0
     assert auction_contract.highestBid() == 0
     # Check end time is more than current block timestamp
-    assert auction_contract.auctionEnd() >= tester.get_block_by_number("latest")["timestamp"]
+    assert auction_contract.auctionEnd() >= env.timestamp
+
 
+def test_bid(env, auction_contract, tx_failed):
+    k1, k2, k3, k4, k5 = env.accounts[:5]
 
-def test_bid(w3, tester, auction_contract, tx_failed):
-    k1, k2, k3, k4, k5 = w3.eth.accounts[:5]
     # Bidder cannot bid 0
     with tx_failed():
-        auction_contract.bid(transact={"value": 0, "from": k1})
+        auction_contract.bid(value=0, sender=k1)
+
     # Bidder can bid
-    auction_contract.bid(transact={"value": 1, "from": k1})
+    auction_contract.bid(value=1, sender=k1)
     # Check that highest bidder and highest bid have changed accordingly
     assert auction_contract.highestBidder() == k1
     assert auction_contract.highestBid() == 1
     # Bidder bid cannot equal current highest bid
     with tx_failed():
-        auction_contract.bid(transact={"value": 1, "from": k1})
+        auction_contract.bid(value=1, sender=k1)
     # Higher bid can replace current highest bid
-    auction_contract.bid(transact={"value": 2, "from": k2})
+    auction_contract.bid(value=2, sender=k2)
     # Check that highest bidder and highest bid have changed accordingly
     assert auction_contract.highestBidder() == k2
     assert auction_contract.highestBid() == 2
     # Multiple bidders can bid
-    auction_contract.bid(transact={"value": 3, "from": k3})
-    auction_contract.bid(transact={"value": 4, "from": k4})
-    auction_contract.bid(transact={"value": 5, "from": k5})
+    auction_contract.bid(value=3, sender=k3)
+    auction_contract.bid(value=4, sender=k4)
+    auction_contract.bid(value=5, sender=k5)
     # Check that highest bidder and highest bid have changed accordingly
     assert auction_contract.highestBidder() == k5
     assert auction_contract.highestBid() == 5
-    auction_contract.bid(transact={"value": 1 * 10**10, "from": k1})
+    auction_contract.bid(value=1 * 10**10, sender=k1)
     pending_return_before_outbid = auction_contract.pendingReturns(k1)
-    auction_contract.bid(transact={"value": 2 * 10**10, "from": k2})
+    auction_contract.bid(value=2 * 10**10, sender=k2)
     pending_return_after_outbid = auction_contract.pendingReturns(k1)
     # Account has a greater pending return balance after being outbid
     assert pending_return_after_outbid > pending_return_before_outbid
 
-    balance_before_withdrawal = w3.eth.get_balance(k1)
-    auction_contract.withdraw(transact={"from": k1})
-    balance_after_withdrawal = w3.eth.get_balance(k1)
+    balance_before_withdrawal = env.get_balance(k1)
+    auction_contract.withdraw(sender=k1)
+    balance_after_withdrawal = env.get_balance(k1)
     # Balance increases after withdrawal
     assert balance_after_withdrawal > balance_before_withdrawal
     # Pending return balance is reset to 0
     assert auction_contract.pendingReturns(k1) == 0
 
 
-def test_end_auction(w3, tester, auction_contract, tx_failed):
-    k1, k2, k3, k4, k5 = w3.eth.accounts[:5]
+def test_end_auction(env, auction_contract, tx_failed):
+    k1, k2, k3, k4, k5 = env.accounts[:5]
+
     # Fails if auction end time has not been reached
     with tx_failed():
         auction_contract.endAuction()
-    auction_contract.bid(transact={"value": 1 * 10**10, "from": k2})
+
+    auction_contract.bid(value=1 * 10**10, sender=k2)
     # Move block timestamp forward to reach auction end time
-    # tester.time_travel(tester.get_block_by_number('latest')['timestamp'] + EXPIRY)
-    w3.testing.mine(EXPIRY)
-    balance_before_end = w3.eth.get_balance(k1)
-    auction_contract.endAuction(transact={"from": k2})
-    balance_after_end = w3.eth.get_balance(k1)
+    env.timestamp += EXPIRY
+    balance_before_end = env.get_balance(k1)
+    auction_contract.endAuction(sender=k2)
+    balance_after_end = env.get_balance(k1)
     # Beneficiary receives the highest bid
     assert balance_after_end == balance_before_end + 1 * 10**10
     # Bidder cannot bid after auction end time has been reached
     with tx_failed():
-        auction_contract.bid(transact={"value": 10, "from": k1})
+        auction_contract.bid(value=10, sender=k1)
     # Auction cannot be ended twice
     with tx_failed():
         auction_contract.endAuction()
```

### Comparing `vyper-0.4.0rc2/tests/functional/examples/market_maker/test_on_chain_market_maker.py` & `vyper-0.4.0rc3/tests/functional/examples/market_maker/test_on_chain_market_maker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,113 +1,114 @@
 import pytest
+from eth_utils import to_wei
 
-
-@pytest.fixture
-def market_maker(get_contract):
-    with open("examples/market_maker/on_chain_market_maker.vy") as f:
-        contract_code = f.read()
-    return get_contract(contract_code)
-
+from tests.utils import ZERO_ADDRESS
 
 TOKEN_NAME = "Vypercoin"
 TOKEN_SYMBOL = "FANG"
 TOKEN_DECIMALS = 18
 TOKEN_INITIAL_SUPPLY = 21 * 10**6
 TOKEN_TOTAL_SUPPLY = TOKEN_INITIAL_SUPPLY * (10**TOKEN_DECIMALS)
 
 
-@pytest.fixture
+@pytest.fixture(scope="module")
 def erc20(get_contract):
     with open("examples/tokens/ERC20.vy") as f:
         contract_code = f.read()
     return get_contract(
         contract_code, *[TOKEN_NAME, TOKEN_SYMBOL, TOKEN_DECIMALS, TOKEN_INITIAL_SUPPLY]
     )
 
 
+@pytest.fixture(scope="module")
+def market_maker(get_contract, erc20):
+    with open("examples/market_maker/on_chain_market_maker.vy") as f:
+        contract_code = f.read()
+    return get_contract(contract_code)
+
+
 def test_initial_state(market_maker):
     assert market_maker.totalEthQty() == 0
     assert market_maker.totalTokenQty() == 0
     assert market_maker.invariant() == 0
-    assert market_maker.owner() is None
+    assert market_maker.owner() == ZERO_ADDRESS
 
 
-def test_initiate(w3, market_maker, erc20, tx_failed):
-    a0 = w3.eth.accounts[0]
-    ether, ethers = w3.to_wei(1, "ether"), w3.to_wei(2, "ether")
-    erc20.approve(market_maker.address, ethers, transact={})
-    market_maker.initiate(erc20.address, ether, transact={"value": ethers})
+def test_initiate(env, market_maker, erc20, tx_failed):
+    a0 = env.accounts[0]
+    ether, ethers = to_wei(1, "ether"), to_wei(2, "ether")
+    env.set_balance(a0, ethers * 2)
+    erc20.approve(market_maker.address, ethers)
+    market_maker.initiate(erc20.address, ether, value=ethers)
     assert market_maker.totalEthQty() == ethers
     assert market_maker.totalTokenQty() == ether
     assert market_maker.invariant() == 2 * 10**36
     assert market_maker.owner() == a0
     assert erc20.name() == TOKEN_NAME
     assert erc20.decimals() == TOKEN_DECIMALS
 
     # Initiate cannot be called twice
     with tx_failed():
-        market_maker.initiate(erc20.address, ether, transact={"value": ethers})
+        market_maker.initiate(erc20.address, ether, value=ethers)
 
 
-def test_eth_to_tokens(w3, market_maker, erc20):
-    a1 = w3.eth.accounts[1]
-    erc20.approve(market_maker.address, w3.to_wei(2, "ether"), transact={})
-    market_maker.initiate(
-        erc20.address, w3.to_wei(1, "ether"), transact={"value": w3.to_wei(2, "ether")}
-    )
-    assert erc20.balanceOf(market_maker.address) == w3.to_wei(1, "ether")
+def test_eth_to_tokens(env, market_maker, erc20):
+    a0, a1 = env.accounts[:2]
+    env.set_balance(a0, to_wei(2, "ether"))
+    erc20.approve(market_maker.address, to_wei(2, "ether"))
+    market_maker.initiate(erc20.address, to_wei(1, "ether"), value=to_wei(2, "ether"))
+    assert erc20.balanceOf(market_maker.address) == to_wei(1, "ether")
     assert erc20.balanceOf(a1) == 0
-    assert market_maker.totalTokenQty() == w3.to_wei(1, "ether")
-    assert market_maker.totalEthQty() == w3.to_wei(2, "ether")
+    assert market_maker.totalTokenQty() == to_wei(1, "ether")
+    assert market_maker.totalEthQty() == to_wei(2, "ether")
 
-    market_maker.ethToTokens(transact={"value": 100, "from": a1})
+    env.set_balance(a1, 100)
+    market_maker.ethToTokens(value=100, sender=a1)
     assert erc20.balanceOf(market_maker.address) == 999999999999999950
     assert erc20.balanceOf(a1) == 50
     assert market_maker.totalTokenQty() == 999999999999999950
     assert market_maker.totalEthQty() == 2000000000000000100
 
 
-def test_tokens_to_eth(w3, market_maker, erc20):
-    a1 = w3.eth.accounts[1]
-    a1_balance_before = w3.eth.get_balance(a1)
-
-    erc20.transfer(a1, w3.to_wei(2, "ether"), transact={})
-    erc20.approve(market_maker.address, w3.to_wei(2, "ether"), transact={"from": a1})
-    market_maker.initiate(
-        erc20.address, w3.to_wei(1, "ether"), transact={"value": w3.to_wei(2, "ether"), "from": a1}
-    )
-    assert w3.eth.get_balance(market_maker.address) == w3.to_wei(2, "ether")
+def test_tokens_to_eth(env, market_maker, erc20):
+    a1 = env.accounts[1]
+    a1_balance_before = to_wei(2, "ether")
+    env.set_balance(a1, a1_balance_before)
+
+    erc20.transfer(a1, to_wei(2, "ether"))
+    erc20.approve(market_maker.address, to_wei(2, "ether"), sender=a1)
+    market_maker.initiate(erc20.address, to_wei(1, "ether"), value=to_wei(2, "ether"), sender=a1)
+    assert env.get_balance(market_maker.address) == to_wei(2, "ether")
     # sent 2 eth, with initiate.
-    assert w3.eth.get_balance(a1) == a1_balance_before - w3.to_wei(2, "ether")
-    assert market_maker.totalTokenQty() == w3.to_wei(1, "ether")
+    assert env.get_balance(a1) == a1_balance_before - to_wei(2, "ether")
+    assert market_maker.totalTokenQty() == to_wei(1, "ether")
 
-    erc20.approve(market_maker.address, w3.to_wei(1, "ether"), transact={"from": a1})
-    market_maker.tokensToEth(w3.to_wei(1, "ether"), transact={"from": a1})
+    erc20.approve(market_maker.address, to_wei(1, "ether"), sender=a1)
+    market_maker.tokensToEth(to_wei(1, "ether"), sender=a1)
     # 1 eth less in market.
-    assert w3.eth.get_balance(market_maker.address) == w3.to_wei(1, "ether")
+    assert env.get_balance(market_maker.address) == to_wei(1, "ether")
     # got 1 eth back, for trade.
-    assert w3.eth.get_balance(a1) == a1_balance_before - w3.to_wei(1, "ether")
+    assert env.get_balance(a1) == a1_balance_before - to_wei(1, "ether")
     # Tokens increased by 1
-    assert market_maker.totalTokenQty() == w3.to_wei(2, "ether")
-    assert market_maker.totalEthQty() == w3.to_wei(1, "ether")
+    assert market_maker.totalTokenQty() == to_wei(2, "ether")
+    assert market_maker.totalEthQty() == to_wei(1, "ether")
 
 
-def test_owner_withdraw(w3, market_maker, erc20, tx_failed):
-    a0, a1 = w3.eth.accounts[:2]
-    a0_balance_before = w3.eth.get_balance(a0)
+def test_owner_withdraw(env, market_maker, erc20, tx_failed):
+    a0, a1 = env.accounts[:2]
+    a0_balance_before = to_wei(10, "ether")
+    env.set_balance(a0, a0_balance_before)
     # Approve 2 eth transfers.
-    erc20.approve(market_maker.address, w3.to_wei(2, "ether"), transact={})
+    erc20.approve(market_maker.address, to_wei(2, "ether"))
     # Initiate market with 2 eth value.
-    market_maker.initiate(
-        erc20.address, w3.to_wei(1, "ether"), transact={"value": w3.to_wei(2, "ether")}
-    )
+    market_maker.initiate(erc20.address, to_wei(1, "ether"), value=to_wei(2, "ether"))
     # 2 eth was sent to market_maker contract.
-    assert w3.eth.get_balance(a0) == a0_balance_before - w3.to_wei(2, "ether")
+    assert env.get_balance(a0) == a0_balance_before - to_wei(2, "ether")
     # a0's balance is locked up in market_maker contract.
-    assert erc20.balanceOf(a0) == TOKEN_TOTAL_SUPPLY - w3.to_wei(1, "ether")
+    assert erc20.balanceOf(a0) == TOKEN_TOTAL_SUPPLY - to_wei(1, "ether")
 
     # Only owner can call ownerWithdraw
     with tx_failed():
-        market_maker.ownerWithdraw(transact={"from": a1})
-    market_maker.ownerWithdraw(transact={})
-    assert w3.eth.get_balance(a0) == a0_balance_before  # Eth balance restored.
+        market_maker.ownerWithdraw(sender=a1)
+    market_maker.ownerWithdraw()
+    assert env.get_balance(a0) == a0_balance_before  # Eth balance restored.
     assert erc20.balanceOf(a0) == TOKEN_TOTAL_SUPPLY  # Tokens returned to a0.
```

### Comparing `vyper-0.4.0rc2/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py` & `vyper-0.4.0rc3/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,110 +8,119 @@
 # (1.1. Seller can reclaim deposit and close the sale as long as nothing was purchased.)
 # 2. Buyer purchases item (value) plus posts an additional safety deposit (Item
 #    value). Balance is 4*value
 # 3. Seller ships item
 # 4. Buyer confirms receiving the item. Buyer's deposit (value) is returned.
 #    Seller's deposit (2*value) + items value is returned. Balance is 0.
 import pytest
+from eth_utils import to_wei
 
 
-@pytest.fixture
+@pytest.fixture(scope="module")
 def contract_code(get_contract):
     with open("examples/safe_remote_purchase/safe_remote_purchase.vy") as f:
         contract_code = f.read()
     return contract_code
 
 
-@pytest.fixture
-def get_balance(w3):
+@pytest.fixture(scope="module")
+def get_balance(env):
     def get_balance():
-        a0, a1 = w3.eth.accounts[:2]
+        a0, a1 = env.accounts[:2]
         # balance of a1 = seller, a2 = buyer
-        return w3.eth.get_balance(a0), w3.eth.get_balance(a1)
+        return env.get_balance(a0), env.get_balance(a1)
 
     return get_balance
 
 
-def test_initial_state(w3, tx_failed, get_contract, get_balance, contract_code):
+def test_initial_state(env, tx_failed, get_contract, get_balance, contract_code):
+    env.set_balance(env.deployer, to_wei(2, "ether"))
     # Initial deposit has to be divisible by two
     with tx_failed():
         get_contract(contract_code, value=13)
     # Seller puts item up for sale
     a0_pre_bal, a1_pre_bal = get_balance()
-    c = get_contract(contract_code, value_in_eth=2)
+    c = get_contract(contract_code, value=to_wei(2, "ether"))
     # Check that the seller is set correctly
-    assert c.seller() == w3.eth.accounts[0]
+    assert c.seller() == env.accounts[0]
     # Check if item value is set correctly (Half of deposit)
-    assert c.value() == w3.to_wei(1, "ether")
+    assert c.value() == to_wei(1, "ether")
     # Check if unlocked() works correctly after initialization
     assert c.unlocked() is True
     # Check that sellers (and buyers) balance is correct
-    assert get_balance() == ((a0_pre_bal - w3.to_wei(2, "ether")), a1_pre_bal)
+    assert get_balance() == ((a0_pre_bal - to_wei(2, "ether")), a1_pre_bal)
 
 
-def test_abort(w3, tx_failed, get_balance, get_contract, contract_code):
-    a0, a1, a2 = w3.eth.accounts[:3]
+def test_abort(env, tx_failed, get_balance, get_contract, contract_code):
+    a0, a1, a2 = env.accounts[:3]
+    for a in env.accounts[:3]:
+        env.set_balance(a, 10**20)
 
     a0_pre_bal, a1_pre_bal = get_balance()
-    c = get_contract(contract_code, value=w3.to_wei(2, "ether"))
-    assert c.value() == w3.to_wei(1, "ether")
+    c = get_contract(contract_code, value=to_wei(2, "ether"))
+    assert c.value() == to_wei(1, "ether")
     # Only sender can trigger refund
     with tx_failed():
-        c.abort(transact={"from": a2})
+        c.abort(sender=a2)
     # Refund works correctly
-    c.abort(transact={"from": a0})
+    c.abort(sender=a0)
     assert get_balance() == (a0_pre_bal, a1_pre_bal)
     # Purchase in process, no refund possible
     c = get_contract(contract_code, value=2)
-    c.purchase(transact={"value": 2, "from": a1})
+    c.purchase(value=2, sender=a1)
     with tx_failed():
-        c.abort(transact={"from": a0})
+        c.abort(sender=a0)
 
 
-def test_purchase(w3, get_contract, tx_failed, get_balance, contract_code):
-    a0, a1, a2, a3 = w3.eth.accounts[:4]
+def test_purchase(env, get_contract, tx_failed, get_balance, contract_code):
+    a0, a1, a2, a3 = env.accounts[:4]
+    for a in env.accounts[:4]:
+        env.set_balance(a, 10**18)
+
     init_bal_a0, init_bal_a1 = get_balance()
     c = get_contract(contract_code, value=2)
     # Purchase for too low/high price
     with tx_failed():
-        c.purchase(transact={"value": 1, "from": a1})
+        c.purchase(value=1, sender=a1)
     with tx_failed():
-        c.purchase(transact={"value": 3, "from": a1})
+        c.purchase(value=3, sender=a1)
     # Purchase for the correct price
-    c.purchase(transact={"value": 2, "from": a1})
+    c.purchase(value=2, sender=a1)
     # Check if buyer is set correctly
     assert c.buyer() == a1
     # Check if contract is locked correctly
     assert c.unlocked() is False
     # Check balances, both deposits should have been deducted
     assert get_balance() == (init_bal_a0 - 2, init_bal_a1 - 2)
     # Allow nobody else to purchase
     with tx_failed():
-        c.purchase(transact={"value": 2, "from": a3})
+        c.purchase(value=2, sender=a3)
 
 
-def test_received(w3, get_contract, tx_failed, get_balance, contract_code):
-    a0, a1 = w3.eth.accounts[:2]
+def test_received(env, get_contract, tx_failed, get_balance, contract_code):
+    a0, a1 = env.accounts[:2]
+    env.set_balance(a0, 10**18)
+    env.set_balance(a1, 10**18)
     init_bal_a0, init_bal_a1 = get_balance()
     c = get_contract(contract_code, value=2)
     # Can only be called after purchase
     with tx_failed():
-        c.received(transact={"from": a1})
+        c.received(sender=a1)
     # Purchase completed
-    c.purchase(transact={"value": 2, "from": a1})
+    c.purchase(value=2, sender=a1)
     # Check that e.g. sender cannot trigger received
     with tx_failed():
-        c.received(transact={"from": a0})
+        c.received(sender=a0)
     # Check if buyer can call receive
-    c.received(transact={"from": a1})
+    c.received(sender=a1)
     # Final check if everything worked. 1 value has been transferred
     assert get_balance() == (init_bal_a0 + 1, init_bal_a1 - 1)
 
 
-def test_received_reentrancy(w3, get_contract, tx_failed, get_balance, contract_code):
+def test_received_reentrancy(env, get_contract, tx_failed, get_balance, contract_code):
     buyer_contract_code = """
 interface PurchaseContract:
 
     def received(): nonpayable
     def purchase(): payable
     def unlocked() -> bool: view
 
@@ -138,28 +147,32 @@
 @external
 @payable
 def __default__():
     extcall self.purchase_contract.received()
 
     """
 
-    a0 = w3.eth.accounts[0]
+    a0, a1 = env.accounts[:2]
+    for a in env.accounts[:2]:
+        env.set_balance(a, 10**18)
+
     c = get_contract(contract_code, value=2)
     buyer_contract = get_contract(buyer_contract_code, *[c.address])
     buyer_contract_address = buyer_contract.address
     init_bal_a0, init_bal_buyer_contract = (
-        w3.eth.get_balance(a0),
-        w3.eth.get_balance(buyer_contract_address),
+        env.get_balance(a0),
+        env.get_balance(buyer_contract_address),
     )
     # Start purchase
-    buyer_contract.start_purchase(transact={"value": 4, "from": w3.eth.accounts[1], "gas": 100000})
+    buyer_contract.start_purchase(value=4, sender=a1, gas=100000)
     assert c.unlocked() is False
     assert c.buyer() == buyer_contract_address
 
     # Trigger "re-entry"
-    buyer_contract.start_received(transact={"from": w3.eth.accounts[1], "gas": 100000})
+    with tx_failed():
+        buyer_contract.start_received(sender=a1, gas=100000)
 
     # Final check if everything worked. 1 value has been transferred
-    assert w3.eth.get_balance(a0), w3.eth.get_balance(buyer_contract_address) == (
+    assert env.get_balance(a0), env.get_balance(buyer_contract_address) == (
         init_bal_a0 + 1,
         init_bal_buyer_contract - 1,
     )
```

### Comparing `vyper-0.4.0rc2/tests/functional/examples/storage/test_storage.py` & `vyper-0.4.0rc3/tests/functional/examples/storage/test_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import pytest
 
 INITIAL_VALUE = 4
 
 
-@pytest.fixture
-def storage_contract(w3, get_contract):
+@pytest.fixture(scope="module")
+def storage_contract(get_contract):
     with open("examples/storage/storage.vy") as f:
         contract_code = f.read()
         # Pass constructor variables directly to the contract
         contract = get_contract(contract_code, INITIAL_VALUE)
     return contract
 
 
 def test_initial_state(storage_contract):
     # Check if the constructor of the contract is set up properly
     assert storage_contract.storedData() == INITIAL_VALUE
 
 
-def test_set(w3, storage_contract):
-    k0 = w3.eth.accounts[0]
-
-    # Let k0 try to set the value to 10
-    storage_contract.set(10, transact={"from": k0})
+def test_set(storage_contract):
+    storage_contract.set(10)
     assert storage_contract.storedData() == 10  # Directly access storedData
 
-    # Let k0 try to set the value to -5
-    storage_contract.set(-5, transact={"from": k0})
+    storage_contract.set(-5)
     assert storage_contract.storedData() == -5
```

### Comparing `vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc4626.py` & `vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc4626.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,85 +3,85 @@
 AMOUNT = 100 * 10**18
 TOKEN_NAME = "Vypercoin"
 TOKEN_SYMBOL = "FANG"
 TOKEN_DECIMALS = 18
 TOKEN_INITIAL_SUPPLY = 0
 
 
-@pytest.fixture
+@pytest.fixture(scope="module")
 def token(get_contract):
     with open("examples/tokens/ERC20.vy") as f:
         return get_contract(
             f.read(), TOKEN_NAME, TOKEN_SYMBOL, TOKEN_DECIMALS, TOKEN_INITIAL_SUPPLY
         )
 
 
-@pytest.fixture
+@pytest.fixture(scope="module")
 def vault(get_contract, token):
     with open("examples/tokens/ERC4626.vy") as f:
         return get_contract(f.read(), token.address)
 
 
 def test_asset(vault, token):
     assert vault.asset() == token.address
 
 
-def test_max_methods(w3, vault):
-    a = w3.eth.accounts[0]
+def test_max_methods(env, vault):
+    a = env.accounts[0]
 
     assert vault.maxDeposit(a) == 2**256 - 1
     assert vault.maxMint(a) == 2**256 - 1
     assert vault.maxWithdraw(a) == 2**256 - 1
     assert vault.maxRedeem(a) == 2**256 - 1
 
 
-def test_preview_methods(w3, token, vault):
-    a = w3.eth.accounts[0]
+def test_preview_methods(env, token, vault):
+    a = env.accounts[0]
 
     assert vault.totalAssets() == 0
     assert vault.convertToAssets(10**18) == 0  # no assets
     assert vault.convertToShares(10**18) == 10**18  # 1:1 price
     assert vault.previewDeposit(AMOUNT) == AMOUNT  # 1:1 price
     assert vault.previewMint(AMOUNT) == AMOUNT  # 1:1 price
     assert vault.previewWithdraw(AMOUNT) == 0  # but no assets
     assert vault.previewRedeem(AMOUNT) == 0  # but no assets
 
-    token.mint(a, AMOUNT, transact={"from": a})
-    token.approve(vault.address, AMOUNT, transact={"from": a})
-    vault.deposit(AMOUNT, transact={"from": a})
+    token.mint(a, AMOUNT, sender=a)
+    token.approve(vault.address, AMOUNT, sender=a)
+    vault.deposit(AMOUNT, sender=a)
 
     assert vault.totalAssets() == AMOUNT
     assert vault.convertToAssets(10**18) == 10**18  # 1:1 price
     assert vault.convertToShares(10**18) == 10**18  # 1:1 price
     assert vault.previewDeposit(AMOUNT) == AMOUNT  # 1:1 price
     assert vault.previewMint(AMOUNT) == AMOUNT  # 1:1 price
     assert vault.previewWithdraw(AMOUNT) == AMOUNT  # 1:1 price
     assert vault.previewRedeem(AMOUNT) == AMOUNT  # 1:1 price
 
-    token.mint(vault.address, AMOUNT, transact={"from": a})
+    token.mint(vault.address, AMOUNT, sender=a)
 
     assert vault.totalAssets() == 2 * AMOUNT
     assert vault.convertToAssets(10**18) == 2 * 10**18  # 2:1 price
     assert vault.convertToShares(2 * 10**18) == 10**18  # 2:1 price
     assert vault.previewDeposit(AMOUNT) == AMOUNT // 2  # 2:1 price
     assert vault.previewMint(AMOUNT // 2) == AMOUNT  # 2:1 price
     assert vault.previewWithdraw(AMOUNT) == AMOUNT // 2  # 2:1 price
     assert vault.previewRedeem(AMOUNT // 2) == AMOUNT  # 2:1 price
 
-    vault.DEBUG_steal_tokens(AMOUNT, transact={"from": a})
+    vault.DEBUG_steal_tokens(AMOUNT, sender=a)
 
     assert vault.totalAssets() == AMOUNT
     assert vault.convertToAssets(10**18) == 10**18  # 1:1 price
     assert vault.convertToShares(10**18) == 10**18  # 1:1 price
     assert vault.previewDeposit(AMOUNT) == AMOUNT  # 1:1 price
     assert vault.previewMint(AMOUNT) == AMOUNT  # 1:1 price
     assert vault.previewWithdraw(AMOUNT) == AMOUNT  # 1:1 price
     assert vault.previewRedeem(AMOUNT) == AMOUNT  # 1:1 price
 
-    vault.DEBUG_steal_tokens(AMOUNT // 2, transact={"from": a})
+    vault.DEBUG_steal_tokens(AMOUNT // 2, sender=a)
 
     assert vault.totalAssets() == AMOUNT // 2
     assert vault.convertToAssets(10**18) == 10**18 // 2  # 1:2 price
     assert vault.convertToShares(10**18 // 2) == 10**18  # 1:2 price
     assert vault.previewDeposit(AMOUNT) == 2 * AMOUNT  # 1:2 price
     assert vault.previewMint(2 * AMOUNT) == AMOUNT  # 1:2 price
     assert vault.previewWithdraw(AMOUNT) == 2 * AMOUNT  # 1:2 price
```

### Comparing `vyper-0.4.0rc2/tests/functional/examples/tokens/test_erc721.py` & `vyper-0.4.0rc3/tests/functional/examples/tokens/test_erc721.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import pytest
 
+from tests.utils import ZERO_ADDRESS
+
 SOMEONE_TOKEN_IDS = [1, 2, 3]
 OPERATOR_TOKEN_ID = 10
 NEW_TOKEN_ID = 20
 INVALID_TOKEN_ID = 99
-ZERO_ADDRESS = "0x0000000000000000000000000000000000000000"
 ERC165_SIG = "0x01ffc9a7"
 ERC165_INVALID_SIG = "0xffffffff"
 ERC721_SIG = "0x80ac58cd"
 
 
-@pytest.fixture
-def c(get_contract, w3):
+@pytest.fixture(scope="module")
+def c(get_contract, env):
     with open("examples/tokens/ERC721.vy") as f:
         code = f.read()
     c = get_contract(code)
-    minter, someone, operator = w3.eth.accounts[:3]
+    minter, someone, operator = env.accounts[:3]
     # someone owns 3 tokens
     for i in SOMEONE_TOKEN_IDS:
-        c.mint(someone, i, transact={"from": minter})
+        c.mint(someone, i, sender=minter)
     # operator owns 1 tokens
-    c.mint(operator, OPERATOR_TOKEN_ID, transact={"from": minter})
+    c.mint(operator, OPERATOR_TOKEN_ID, sender=minter)
     return c
 
 
-def test_erc165(w3, c):
+def test_erc165(env, c):
     # From EIP-165:
     #   The source contract makes a STATICCALL to the destination address with input data:
     #       0x01ffc9a701ffc9a700000000000000000000000000000000000000000000000000000000
     #       and gas 30,000. This corresponds to `contract.supportsInterface(0x01ffc9a7)`
     assert c.supportsInterface(ERC165_SIG)
     #   If the call fails or return false, the destination contract does not implement ERC-165.
     #   If the call returns true, a second call is made with input data:
@@ -36,311 +37,279 @@
     assert not c.supportsInterface(ERC165_INVALID_SIG)
     #   If the second call fails or returns true, the destination contract does not implement
     #   ERC-165. Otherwise it implements ERC-165.
 
     assert c.supportsInterface(ERC721_SIG)
 
 
-def test_balanceOf(c, w3, tx_failed):
-    someone = w3.eth.accounts[1]
+def test_balanceOf(c, env, tx_failed):
+    someone = env.accounts[1]
     assert c.balanceOf(someone) == 3
     with tx_failed():
         c.balanceOf(ZERO_ADDRESS)
 
 
-def test_ownerOf(c, w3, tx_failed):
-    someone = w3.eth.accounts[1]
+def test_ownerOf(c, env, tx_failed):
+    someone = env.accounts[1]
     assert c.ownerOf(SOMEONE_TOKEN_IDS[0]) == someone
     with tx_failed():
         c.ownerOf(INVALID_TOKEN_ID)
 
 
-def test_getApproved(c, w3):
-    someone, operator = w3.eth.accounts[1:3]
+def test_getApproved(c, env):
+    someone, operator = env.accounts[1:3]
 
-    assert c.getApproved(SOMEONE_TOKEN_IDS[0]) is None
+    assert c.getApproved(SOMEONE_TOKEN_IDS[0]) == ZERO_ADDRESS
 
-    c.approve(operator, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
+    c.approve(operator, SOMEONE_TOKEN_IDS[0], sender=someone)
 
     assert c.getApproved(SOMEONE_TOKEN_IDS[0]) == operator
 
 
-def test_isApprovedForAll(c, w3):
-    someone, operator = w3.eth.accounts[1:3]
+def test_isApprovedForAll(c, env):
+    someone, operator = env.accounts[1:3]
 
     assert c.isApprovedForAll(someone, operator) == 0
 
-    c.setApprovalForAll(operator, True, transact={"from": someone})
+    c.setApprovalForAll(operator, True, sender=someone)
 
     assert c.isApprovedForAll(someone, operator) == 1
 
 
-def test_transferFrom_by_owner(c, w3, tx_failed, get_logs):
-    someone, operator = w3.eth.accounts[1:3]
+def test_transferFrom_by_owner(c, env, tx_failed, get_logs):
+    someone, operator = env.accounts[1:3]
 
     # transfer from zero address
     with tx_failed():
-        c.transferFrom(ZERO_ADDRESS, operator, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
+        c.transferFrom(ZERO_ADDRESS, operator, SOMEONE_TOKEN_IDS[0], sender=someone)
 
     # transfer to zero address
     with tx_failed():
-        c.transferFrom(someone, ZERO_ADDRESS, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
+        c.transferFrom(someone, ZERO_ADDRESS, SOMEONE_TOKEN_IDS[0], sender=someone)
 
     # transfer token without ownership
     with tx_failed():
-        c.transferFrom(someone, operator, OPERATOR_TOKEN_ID, transact={"from": someone})
+        c.transferFrom(someone, operator, OPERATOR_TOKEN_ID, sender=someone)
 
     # transfer invalid token
     with tx_failed():
-        c.transferFrom(someone, operator, INVALID_TOKEN_ID, transact={"from": someone})
+        c.transferFrom(someone, operator, INVALID_TOKEN_ID, sender=someone)
 
     # transfer by owner
-    tx_hash = c.transferFrom(someone, operator, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
-
-    logs = get_logs(tx_hash, c, "Transfer")
+    c.transferFrom(someone, operator, SOMEONE_TOKEN_IDS[0], sender=someone)
 
-    assert len(logs) > 0
-    args = logs[0].args
-    assert args.sender == someone
-    assert args.receiver == operator
-    assert args.token_id == SOMEONE_TOKEN_IDS[0]
+    (log,) = get_logs(c, "Transfer")
+    assert log.args.sender == someone
+    assert log.args.receiver == operator
+    assert log.args.token_id == SOMEONE_TOKEN_IDS[0]
     assert c.ownerOf(SOMEONE_TOKEN_IDS[0]) == operator
     assert c.balanceOf(someone) == 2
     assert c.balanceOf(operator) == 2
 
 
-def test_transferFrom_by_approved(c, w3, get_logs):
-    someone, operator = w3.eth.accounts[1:3]
+def test_transferFrom_by_approved(c, env, get_logs):
+    someone, operator = env.accounts[1:3]
 
     # transfer by approved
-    c.approve(operator, SOMEONE_TOKEN_IDS[1], transact={"from": someone})
-    tx_hash = c.transferFrom(someone, operator, SOMEONE_TOKEN_IDS[1], transact={"from": operator})
-
-    logs = get_logs(tx_hash, c, "Transfer")
+    c.approve(operator, SOMEONE_TOKEN_IDS[1], sender=someone)
+    c.transferFrom(someone, operator, SOMEONE_TOKEN_IDS[1], sender=operator)
 
-    assert len(logs) > 0
-    args = logs[0].args
-    assert args.sender == someone
-    assert args.receiver == operator
-    assert args.token_id == SOMEONE_TOKEN_IDS[1]
+    (log,) = get_logs(c, "Transfer")
+    assert log.args.sender == someone
+    assert log.args.receiver == operator
+    assert log.args.token_id == SOMEONE_TOKEN_IDS[1]
     assert c.ownerOf(SOMEONE_TOKEN_IDS[1]) == operator
     assert c.balanceOf(someone) == 2
     assert c.balanceOf(operator) == 2
 
 
-def test_transferFrom_by_operator(c, w3, get_logs):
-    someone, operator = w3.eth.accounts[1:3]
+def test_transferFrom_by_operator(c, env, get_logs):
+    someone, operator = env.accounts[1:3]
 
     # transfer by operator
-    c.setApprovalForAll(operator, True, transact={"from": someone})
-    tx_hash = c.transferFrom(someone, operator, SOMEONE_TOKEN_IDS[2], transact={"from": operator})
-
-    logs = get_logs(tx_hash, c, "Transfer")
+    c.setApprovalForAll(operator, True, sender=someone)
+    c.transferFrom(someone, operator, SOMEONE_TOKEN_IDS[2], sender=operator)
 
-    assert len(logs) > 0
-    args = logs[0].args
-    assert args.sender == someone
-    assert args.receiver == operator
-    assert args.token_id == SOMEONE_TOKEN_IDS[2]
+    (log,) = get_logs(c, "Transfer")
+    assert log.args.sender == someone
+    assert log.args.receiver == operator
+    assert log.args.token_id == SOMEONE_TOKEN_IDS[2]
     assert c.ownerOf(SOMEONE_TOKEN_IDS[2]) == operator
     assert c.balanceOf(someone) == 2
     assert c.balanceOf(operator) == 2
 
 
-def test_safeTransferFrom_by_owner(c, w3, tx_failed, get_logs):
-    someone, operator = w3.eth.accounts[1:3]
+def test_safeTransferFrom_by_owner(c, env, tx_failed, get_logs):
+    someone, operator = env.accounts[1:3]
 
     # transfer from zero address
     with tx_failed():
-        c.safeTransferFrom(ZERO_ADDRESS, operator, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
+        c.safeTransferFrom(ZERO_ADDRESS, operator, SOMEONE_TOKEN_IDS[0], sender=someone)
 
     # transfer to zero address
     with tx_failed():
-        c.safeTransferFrom(someone, ZERO_ADDRESS, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
+        c.safeTransferFrom(someone, ZERO_ADDRESS, SOMEONE_TOKEN_IDS[0], sender=someone)
 
     # transfer token without ownership
     with tx_failed():
-        c.safeTransferFrom(someone, operator, OPERATOR_TOKEN_ID, transact={"from": someone})
+        c.safeTransferFrom(someone, operator, OPERATOR_TOKEN_ID, sender=someone)
 
     # transfer invalid token
     with tx_failed():
-        c.safeTransferFrom(someone, operator, INVALID_TOKEN_ID, transact={"from": someone})
+        c.safeTransferFrom(someone, operator, INVALID_TOKEN_ID, sender=someone)
 
     # transfer by owner
-    tx_hash = c.safeTransferFrom(
-        someone, operator, SOMEONE_TOKEN_IDS[0], transact={"from": someone}
-    )
-
-    logs = get_logs(tx_hash, c, "Transfer")
+    c.safeTransferFrom(someone, operator, SOMEONE_TOKEN_IDS[0], sender=someone)
 
-    assert len(logs) > 0
-    args = logs[0].args
-    assert args.sender == someone
-    assert args.receiver == operator
-    assert args.token_id == SOMEONE_TOKEN_IDS[0]
+    (log,) = get_logs(c, "Transfer")
+    assert log.args.sender == someone
+    assert log.args.receiver == operator
+    assert log.args.token_id == SOMEONE_TOKEN_IDS[0]
     assert c.ownerOf(SOMEONE_TOKEN_IDS[0]) == operator
     assert c.balanceOf(someone) == 2
     assert c.balanceOf(operator) == 2
 
 
-def test_safeTransferFrom_by_approved(c, w3, get_logs):
-    someone, operator = w3.eth.accounts[1:3]
+def test_safeTransferFrom_by_approved(c, env, get_logs):
+    someone, operator = env.accounts[1:3]
 
     # transfer by approved
-    c.approve(operator, SOMEONE_TOKEN_IDS[1], transact={"from": someone})
-    tx_hash = c.safeTransferFrom(
-        someone, operator, SOMEONE_TOKEN_IDS[1], transact={"from": operator}
-    )
-
-    logs = get_logs(tx_hash, c, "Transfer")
+    c.approve(operator, SOMEONE_TOKEN_IDS[1], sender=someone)
+    c.safeTransferFrom(someone, operator, SOMEONE_TOKEN_IDS[1], sender=operator)
 
-    assert len(logs) > 0
-    args = logs[0].args
+    (log,) = get_logs(c, "Transfer")
+    args = log.args
     assert args.sender == someone
     assert args.receiver == operator
     assert args.token_id == SOMEONE_TOKEN_IDS[1]
     assert c.ownerOf(SOMEONE_TOKEN_IDS[1]) == operator
     assert c.balanceOf(someone) == 2
     assert c.balanceOf(operator) == 2
 
 
-def test_safeTransferFrom_by_operator(c, w3, get_logs):
-    someone, operator = w3.eth.accounts[1:3]
+def test_safeTransferFrom_by_operator(c, env, get_logs):
+    someone, operator = env.accounts[1:3]
 
     # transfer by operator
-    c.setApprovalForAll(operator, True, transact={"from": someone})
-    tx_hash = c.safeTransferFrom(
-        someone, operator, SOMEONE_TOKEN_IDS[2], transact={"from": operator}
-    )
+    c.setApprovalForAll(operator, True, sender=someone)
+    c.safeTransferFrom(someone, operator, SOMEONE_TOKEN_IDS[2], sender=operator)
 
-    logs = get_logs(tx_hash, c, "Transfer")
-
-    assert len(logs) > 0
-    args = logs[0].args
-    assert args.sender == someone
-    assert args.receiver == operator
-    assert args.token_id == SOMEONE_TOKEN_IDS[2]
+    (log,) = get_logs(c, "Transfer")
+    assert log.args.sender == someone
+    assert log.args.receiver == operator
+    assert log.args.token_id == SOMEONE_TOKEN_IDS[2]
     assert c.ownerOf(SOMEONE_TOKEN_IDS[2]) == operator
     assert c.balanceOf(someone) == 2
     assert c.balanceOf(operator) == 2
 
 
-def test_safeTransferFrom_to_contract(c, w3, tx_failed, get_logs, get_contract):
-    someone = w3.eth.accounts[1]
+def test_safeTransferFrom_to_contract(c, env, tx_failed, get_logs, get_contract):
+    someone = env.accounts[1]
 
     # Can't transfer to a contract that doesn't implement the receiver code
     with tx_failed():
-        c.safeTransferFrom(someone, c.address, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
+        c.safeTransferFrom(someone, c.address, SOMEONE_TOKEN_IDS[0], sender=someone)
 
     # Only to an address that implements that function
     receiver = get_contract(
         """
 @external
 def onERC721Received(
         _operator: address,
         _from: address,
         _tokenId: uint256,
         _data: Bytes[1024]
     ) -> bytes4:
     return method_id("onERC721Received(address,address,uint256,bytes)", output_type=bytes4)
     """
     )
-    tx_hash = c.safeTransferFrom(
-        someone, receiver.address, SOMEONE_TOKEN_IDS[0], transact={"from": someone}
-    )
+    c.safeTransferFrom(someone, receiver.address, SOMEONE_TOKEN_IDS[0], sender=someone)
 
-    logs = get_logs(tx_hash, c, "Transfer")
-
-    assert len(logs) > 0
-    args = logs[0].args
-    assert args.sender == someone
-    assert args.receiver == receiver.address
-    assert args.token_id == SOMEONE_TOKEN_IDS[0]
+    (log,) = get_logs(c, "Transfer")
+    assert log.args.sender == someone
+    assert log.args.receiver == receiver.address
+    assert log.args.token_id == SOMEONE_TOKEN_IDS[0]
     assert c.ownerOf(SOMEONE_TOKEN_IDS[0]) == receiver.address
     assert c.balanceOf(someone) == 2
     assert c.balanceOf(receiver.address) == 1
 
 
-def test_approve(c, w3, tx_failed, get_logs):
-    someone, operator = w3.eth.accounts[1:3]
+def test_approve(c, env, tx_failed, get_logs):
+    someone, operator = env.accounts[1:3]
 
     # approve myself
     with tx_failed():
-        c.approve(someone, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
+        c.approve(someone, SOMEONE_TOKEN_IDS[0], sender=someone)
 
     # approve token without ownership
     with tx_failed():
-        c.approve(operator, OPERATOR_TOKEN_ID, transact={"from": someone})
+        c.approve(operator, OPERATOR_TOKEN_ID, sender=someone)
 
     # approve invalid token
     with tx_failed():
-        c.approve(operator, INVALID_TOKEN_ID, transact={"from": someone})
+        c.approve(operator, INVALID_TOKEN_ID, sender=someone)
 
-    tx_hash = c.approve(operator, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
-    logs = get_logs(tx_hash, c, "Approval")
+    c.approve(operator, SOMEONE_TOKEN_IDS[0], sender=someone)
+    (log,) = get_logs(c, "Approval")
 
-    assert len(logs) > 0
-    args = logs[0].args
-    assert args.owner == someone
-    assert args.approved == operator
-    assert args.token_id == SOMEONE_TOKEN_IDS[0]
+    assert log.args.owner == someone
+    assert log.args.approved == operator
+    assert log.args.token_id == SOMEONE_TOKEN_IDS[0]
 
 
-def test_setApprovalForAll(c, w3, tx_failed, get_logs):
-    someone, operator = w3.eth.accounts[1:3]
+def test_setApprovalForAll(c, env, tx_failed, get_logs):
+    someone, operator = env.accounts[1:3]
     approved = True
 
     # setApprovalForAll myself
     with tx_failed():
-        c.setApprovalForAll(someone, approved, transact={"from": someone})
+        c.setApprovalForAll(someone, approved, sender=someone)
 
-    tx_hash = c.setApprovalForAll(operator, approved, transact={"from": someone})
-    logs = get_logs(tx_hash, c, "ApprovalForAll")
-
-    assert len(logs) > 0
-    args = logs[0].args
+    c.setApprovalForAll(operator, approved, sender=someone)
+    (log,) = get_logs(c, "ApprovalForAll")
+    args = log.args
     assert args.owner == someone
     assert args.operator == operator
     assert args.approved == approved
 
 
-def test_mint(c, w3, tx_failed, get_logs):
-    minter, someone = w3.eth.accounts[:2]
+def test_mint(c, env, tx_failed, get_logs):
+    minter, someone = env.accounts[:2]
 
     # mint by non-minter
     with tx_failed():
-        c.mint(someone, SOMEONE_TOKEN_IDS[0], transact={"from": someone})
+        c.mint(someone, SOMEONE_TOKEN_IDS[0], sender=someone)
 
     # mint to zero address
     with tx_failed():
-        c.mint(ZERO_ADDRESS, SOMEONE_TOKEN_IDS[0], transact={"from": minter})
+        c.mint(ZERO_ADDRESS, SOMEONE_TOKEN_IDS[0], sender=minter)
 
     # mint by minter
-    tx_hash = c.mint(someone, NEW_TOKEN_ID, transact={"from": minter})
-    logs = get_logs(tx_hash, c, "Transfer")
+    c.mint(someone, NEW_TOKEN_ID, sender=minter)
+    logs = get_logs(c, "Transfer")
 
     assert len(logs) > 0
     args = logs[0].args
     assert args.sender == ZERO_ADDRESS
     assert args.receiver == someone
     assert args.token_id == NEW_TOKEN_ID
     assert c.ownerOf(NEW_TOKEN_ID) == someone
     assert c.balanceOf(someone) == 4
 
 
-def test_burn(c, w3, tx_failed, get_logs):
-    someone, operator = w3.eth.accounts[1:3]
+def test_burn(c, env, tx_failed, get_logs):
+    someone, operator = env.accounts[1:3]
 
     # burn token without ownership
     with tx_failed():
-        c.burn(SOMEONE_TOKEN_IDS[0], transact={"from": operator})
+        c.burn(SOMEONE_TOKEN_IDS[0], sender=operator)
 
     # burn token by owner
-    tx_hash = c.burn(SOMEONE_TOKEN_IDS[0], transact={"from": someone})
-    logs = get_logs(tx_hash, c, "Transfer")
+    c.burn(SOMEONE_TOKEN_IDS[0], sender=someone)
+    logs = get_logs(c, "Transfer")
 
     assert len(logs) > 0
     args = logs[0].args
     assert args.sender == someone
     assert args.receiver == ZERO_ADDRESS
     assert args.token_id == SOMEONE_TOKEN_IDS[0]
     with tx_failed():
```

### Comparing `vyper-0.4.0rc2/tests/functional/examples/voting/test_ballot.py` & `vyper-0.4.0rc3/tests/functional/examples/voting/test_ballot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,247 +1,246 @@
 import pytest
 
+from tests.utils import ZERO_ADDRESS
+
 PROPOSAL_1_NAME = b"Clinton" + b"\x00" * 25
 PROPOSAL_2_NAME = b"Trump" + b"\x00" * 27
 
 
-@pytest.fixture
+@pytest.fixture(scope="module")
 def c(get_contract):
     with open("examples/voting/ballot.vy") as f:
         contract_code = f.read()
     return get_contract(contract_code, *[[PROPOSAL_1_NAME, PROPOSAL_2_NAME]])
 
 
-z0 = "0x0000000000000000000000000000000000000000"
+z0 = ZERO_ADDRESS
 
 
-def test_initial_state(w3, c):
-    a0 = w3.eth.accounts[0]
+def test_initial_state(env, c):
+    a0 = env.accounts[0]
     # Check chairperson is msg.sender
     assert c.chairperson() == a0
     # Check propsal names are correct
     assert c.proposals(0)[0][:7] == b"Clinton"  # Proposal.name
     assert c.proposals(1)[0][:5] == b"Trump"  # Proposal.name
     # Check proposal voteCount is 0
     assert c.proposals(0)[1] == 0  # Proposal.voteCount
     assert c.proposals(1)[1] == 0  # Proposal.voteCount
     # Check voterCount is 0
     assert c.voterCount() == 0
     # Check voter starts empty
-    assert c.voters(z0)[2] is None  # Voter.delegate
-    assert c.voters(z0)[3] == 0  # Voter.vote
-    assert c.voters(z0)[1] is False  # Voter.voted
-    assert c.voters(z0)[0] == 0  # Voter.weight
+    assert c.voters(z0) == (0, False, ZERO_ADDRESS, 0)
 
 
-def test_give_the_right_to_vote(w3, c, tx_failed):
-    a0, a1, a2, a3, a4, a5 = w3.eth.accounts[:6]
-    c.giveRightToVote(a1, transact={})
+def test_give_the_right_to_vote(env, c, tx_failed):
+    a0, a1, a2, a3, a4, a5 = env.accounts[:6]
+    c.giveRightToVote(a1)
     # Check voter given right has weight of 1
     assert c.voters(a1)[0] == 1  # Voter.weight
     # Check no other voter attributes have changed
-    assert c.voters(a1)[2] is None  # Voter.delegate
+    assert c.voters(a1)[2] == ZERO_ADDRESS  # Voter.delegate
     assert c.voters(a1)[3] == 0  # Voter.vote
     assert c.voters(a1)[1] is False  # Voter.voted
     # Chairperson can give themselves the right to vote
-    c.giveRightToVote(a0, transact={})
+    c.giveRightToVote(a0)
     # Check chairperson has weight of 1
     assert c.voters(a0)[0] == 1  # Voter.weight
     # Check voter_acount is 2
     assert c.voterCount() == 2
     # Check several giving rights to vote
-    c.giveRightToVote(a2, transact={})
-    c.giveRightToVote(a3, transact={})
-    c.giveRightToVote(a4, transact={})
-    c.giveRightToVote(a5, transact={})
+    c.giveRightToVote(a2)
+    c.giveRightToVote(a3)
+    c.giveRightToVote(a4)
+    c.giveRightToVote(a5)
     # Check voter_acount is now 6
     assert c.voterCount() == 6
     # Check chairperson cannot give the right to vote twice to the same voter
     with tx_failed():
-        c.giveRightToVote(a5, transact={})
+        c.giveRightToVote(a5)
     # Check voters weight didn't change
     assert c.voters(a5)[0] == 1  # Voter.weight
 
 
-def test_forward_weight(w3, c):
-    a0, a1, a2, a3, a4, a5, a6, a7, a8, a9 = w3.eth.accounts[:10]
-    c.giveRightToVote(a0, transact={})
-    c.giveRightToVote(a1, transact={})
-    c.giveRightToVote(a2, transact={})
-    c.giveRightToVote(a3, transact={})
-    c.giveRightToVote(a4, transact={})
-    c.giveRightToVote(a5, transact={})
-    c.giveRightToVote(a6, transact={})
-    c.giveRightToVote(a7, transact={})
-    c.giveRightToVote(a8, transact={})
-    c.giveRightToVote(a9, transact={})
+def test_forward_weight(env, c):
+    a0, a1, a2, a3, a4, a5, a6, a7, a8, a9 = env.accounts[:10]
+    c.giveRightToVote(a0)
+    c.giveRightToVote(a1)
+    c.giveRightToVote(a2)
+    c.giveRightToVote(a3)
+    c.giveRightToVote(a4)
+    c.giveRightToVote(a5)
+    c.giveRightToVote(a6)
+    c.giveRightToVote(a7)
+    c.giveRightToVote(a8)
+    c.giveRightToVote(a9)
 
     # aN(V) in these comments means address aN has vote weight V
 
-    c.delegate(a2, transact={"from": a1})
+    c.delegate(a2, sender=a1)
     # a1(0) -> a2(2)    a3(1)
-    c.delegate(a3, transact={"from": a2})
+    c.delegate(a3, sender=a2)
     # a1(0) -> a2(0) -> a3(3)
     assert c.voters(a1)[0] == 0  # Voter.weight
     assert c.voters(a2)[0] == 0  # Voter.weight
     assert c.voters(a3)[0] == 3  # Voter.weight
 
-    c.delegate(a9, transact={"from": a8})
+    c.delegate(a9, sender=a8)
     # a7(1)    a8(0) -> a9(2)
-    c.delegate(a8, transact={"from": a7})
+    c.delegate(a8, sender=a7)
     # a7(0) -> a8(0) -> a9(3)
     assert c.voters(a7)[0] == 0  # Voter.weight
     assert c.voters(a8)[0] == 0  # Voter.weight
     assert c.voters(a9)[0] == 3  # Voter.weight
-    c.delegate(a7, transact={"from": a6})
-    c.delegate(a6, transact={"from": a5})
-    c.delegate(a5, transact={"from": a4})
+    c.delegate(a7, sender=a6)
+    c.delegate(a6, sender=a5)
+    c.delegate(a5, sender=a4)
     # a4(0) -> a5(0) -> a6(0) -> a7(0) -> a8(0) -> a9(6)
     assert c.voters(a9)[0] == 6  # Voter.weight
     assert c.voters(a8)[0] == 0  # Voter.weight
 
     # a3(3)    a4(0) -> a5(0) -> a6(0) -> a7(0) -> a8(0) -> a9(6)
-    c.delegate(a4, transact={"from": a3})
+    c.delegate(a4, sender=a3)
     # a3(0) -> a4(0) -> a5(0) -> a6(0) -> a7(0) -> a8(3) -> a9(6)
     # a3's vote weight of 3 only makes it to a8 in the delegation chain:
     assert c.voters(a8)[0] == 3  # Voter.weight
     assert c.voters(a9)[0] == 6  # Voter.weight
 
     # call forward_weight again to move the vote weight the
     # rest of the way:
-    c.forwardWeight(a8, transact={})
+    c.forwardWeight(a8)
     # a3(0) -> a4(0) -> a5(0) -> a6(0) -> a7(0) -> a8(0) -> a9(9)
     assert c.voters(a8)[0] == 0  # Voter.weight
     assert c.voters(a9)[0] == 9  # Voter.weight
 
     # a0(1) -> a1(0) -> a2(0) -> a3(0) -> a4(0) -> a5(0) -> a6(0) -> a7(0) -> a8(0) -> a9(9)
-    c.delegate(a1, transact={"from": a0})
+    c.delegate(a1, sender=a0)
     # a0's vote weight of 1 only makes it to a5 in the delegation chain:
     # a0(0) -> a1(0) -> a2(0) -> a3(0) -> a4(0) -> a5(1) -> a6(0) -> a7(0) -> a8(0) -> a9(9)
     assert c.voters(a5)[0] == 1  # Voter.weight
     assert c.voters(a9)[0] == 9  # Voter.weight
 
     # once again call forward_weight to move the vote weight the
     # rest of the way:
-    c.forwardWeight(a5, transact={})
+    c.forwardWeight(a5)
     # a0(0) -> a1(0) -> a2(0) -> a3(0) -> a4(0) -> a5(0) -> a6(0) -> a7(0) -> a8(0) -> a9(10)
     assert c.voters(a5)[0] == 0  # Voter.weight
     assert c.voters(a9)[0] == 10  # Voter.weight
 
 
-def test_block_short_cycle(w3, c, tx_failed):
-    a0, a1, a2, a3, a4, a5, a6, a7, a8, a9 = w3.eth.accounts[:10]
-    c.giveRightToVote(a0, transact={})
-    c.giveRightToVote(a1, transact={})
-    c.giveRightToVote(a2, transact={})
-    c.giveRightToVote(a3, transact={})
-    c.giveRightToVote(a4, transact={})
-    c.giveRightToVote(a5, transact={})
-
-    c.delegate(a1, transact={"from": a0})
-    c.delegate(a2, transact={"from": a1})
-    c.delegate(a3, transact={"from": a2})
-    c.delegate(a4, transact={"from": a3})
+def test_block_short_cycle(env, c, tx_failed):
+    a0, a1, a2, a3, a4, a5, a6, a7, a8, a9 = env.accounts[:10]
+    c.giveRightToVote(a0)
+    c.giveRightToVote(a1)
+    c.giveRightToVote(a2)
+    c.giveRightToVote(a3)
+    c.giveRightToVote(a4)
+    c.giveRightToVote(a5)
+
+    c.delegate(a1, sender=a0)
+    c.delegate(a2, sender=a1)
+    c.delegate(a3, sender=a2)
+    c.delegate(a4, sender=a3)
     # would create a length 5 cycle:
     with tx_failed():
-        c.delegate(a0, transact={"from": a4})
+        c.delegate(a0, sender=a4)
 
-    c.delegate(a5, transact={"from": a4})
+    c.delegate(a5, sender=a4)
     # can't detect length 6 cycle, so this works:
-    c.delegate(a0, transact={"from": a5})
+    c.delegate(a0, sender=a5)
     # which is fine for the contract; those votes are simply spoiled.
     # but this is something the frontend should prevent for user friendliness
 
 
-def test_delegate(w3, c, tx_failed):
-    a0, a1, a2, a3, a4, a5, a6 = w3.eth.accounts[:7]
-    c.giveRightToVote(a0, transact={})
-    c.giveRightToVote(a1, transact={})
-    c.giveRightToVote(a2, transact={})
-    c.giveRightToVote(a3, transact={})
+def test_delegate(env, c, tx_failed):
+    a0, a1, a2, a3, a4, a5, a6 = env.accounts[:7]
+    c.giveRightToVote(a0)
+    c.giveRightToVote(a1)
+    c.giveRightToVote(a2)
+    c.giveRightToVote(a3)
     # Voter's weight is 1
     assert c.voters(a1)[0] == 1  # Voter.weight
     # Voter can delegate: a1 -> a0
-    c.delegate(a0, transact={"from": a1})
+    c.delegate(a0, sender=a1)
     # Voter's weight is now 0
     assert c.voters(a1)[0] == 0  # Voter.weight
     # Voter has voted
     assert c.voters(a1)[1] is True  # Voter.voted
     # Delegate's weight is 2
     assert c.voters(a0)[0] == 2  # Voter.weight
     # Voter cannot delegate twice
     with tx_failed():
-        c.delegate(a2, transact={"from": a1})
+        c.delegate(a2, sender=a1)
     # Voter cannot delegate to themselves
     with tx_failed():
-        c.delegate(a2, transact={"from": a2})
+        c.delegate(a2, sender=a2)
     # Voter CAN delegate to someone who hasn't been granted right to vote
     # Exercise: prevent that
-    c.delegate(a6, transact={"from": a2})
+    c.delegate(a6, sender=a2)
     # Voter's delegatation is passed up to final delegate, yielding:
     # a3 -> a1 -> a0
-    c.delegate(a1, transact={"from": a3})
+    c.delegate(a1, sender=a3)
     # Delegate's weight is 3
     assert c.voters(a0)[0] == 3  # Voter.weight
 
 
-def test_vote(w3, c, tx_failed):
-    a0, a1, a2, a3, a4, a5, a6, a7, a8, a9 = w3.eth.accounts[:10]
-    c.giveRightToVote(a0, transact={})
-    c.giveRightToVote(a1, transact={})
-    c.giveRightToVote(a2, transact={})
-    c.giveRightToVote(a3, transact={})
-    c.giveRightToVote(a4, transact={})
-    c.giveRightToVote(a5, transact={})
-    c.giveRightToVote(a6, transact={})
-    c.giveRightToVote(a7, transact={})
-    c.delegate(a0, transact={"from": a1})
-    c.delegate(a1, transact={"from": a3})
+def test_vote(env, c, tx_failed):
+    a0, a1, a2, a3, a4, a5, a6, a7, a8, a9 = env.accounts[:10]
+    c.giveRightToVote(a0)
+    c.giveRightToVote(a1)
+    c.giveRightToVote(a2)
+    c.giveRightToVote(a3)
+    c.giveRightToVote(a4)
+    c.giveRightToVote(a5)
+    c.giveRightToVote(a6)
+    c.giveRightToVote(a7)
+    c.delegate(a0, sender=a1)
+    c.delegate(a1, sender=a3)
     # Voter can vote
-    c.vote(0, transact={})
+    c.vote(0)
     # Vote count changes based on voters weight
     assert c.proposals(0)[1] == 3  # Proposal.voteCount
     # Voter cannot vote twice
     with tx_failed():
         c.vote(0)
     # Voter cannot vote if they've delegated
     with tx_failed():
-        c.vote(0, transact={"from": a1})
+        c.vote(0, sender=a1)
     # Several voters can vote
-    c.vote(1, transact={"from": a4})
-    c.vote(1, transact={"from": a2})
-    c.vote(1, transact={"from": a5})
-    c.vote(1, transact={"from": a6})
+    c.vote(1, sender=a4)
+    c.vote(1, sender=a2)
+    c.vote(1, sender=a5)
+    c.vote(1, sender=a6)
     assert c.proposals(1)[1] == 4  # Proposal.voteCount
     # Can't vote on a non-proposal
     with tx_failed():
-        c.vote(2, transact={"from": a7})
+        c.vote(2, sender=a7)
 
 
-def test_winning_proposal(w3, c):
-    a0, a1, a2 = w3.eth.accounts[:3]
-    c.giveRightToVote(a0, transact={})
-    c.giveRightToVote(a1, transact={})
-    c.giveRightToVote(a2, transact={})
-    c.vote(0, transact={})
+def test_winning_proposal(env, c):
+    a0, a1, a2 = env.accounts[:3]
+    c.giveRightToVote(a0)
+    c.giveRightToVote(a1)
+    c.giveRightToVote(a2)
+    c.vote(0)
     # Proposal 0 is now winning
     assert c.winningProposal() == 0
-    c.vote(1, transact={"from": a1})
+    c.vote(1, sender=a1)
     # Proposal 0 is still winning (the proposals are tied)
     assert c.winningProposal() == 0
-    c.vote(1, transact={"from": a2})
+    c.vote(1, sender=a2)
     # Proposal 2 is now winning
     assert c.winningProposal() == 1
 
 
-def test_winner_namer(w3, c):
-    a0, a1, a2 = w3.eth.accounts[:3]
-    c.giveRightToVote(a0, transact={})
-    c.giveRightToVote(a1, transact={})
-    c.giveRightToVote(a2, transact={})
-    c.delegate(a1, transact={"from": a2})
-    c.vote(0, transact={})
+def test_winner_namer(env, c):
+    a0, a1, a2 = env.accounts[:3]
+    c.giveRightToVote(a0)
+    c.giveRightToVote(a1)
+    c.giveRightToVote(a2)
+    c.delegate(a1, sender=a2)
+    c.vote(0)
     # Proposal 0 is now winning
     assert c.winnerName()[:7] == b"Clinton"
-    c.vote(1, transact={"from": a1})
+    c.vote(1, sender=a1)
     # Proposal 2 is now winning
     assert c.winnerName()[:5] == b"Trump"
```

### Comparing `vyper-0.4.0rc2/tests/functional/examples/wallet/test_wallet.py` & `vyper-0.4.0rc3/tests/functional/examples/wallet/test_wallet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,115 @@
 import pytest
 from eth_account import Account
 from eth_account.messages import encode_defunct
 from eth_keys import KeyAPI
-from eth_utils import is_same_address
+from eth_utils import is_same_address, to_bytes, to_checksum_address, to_int
 
+from tests.utils import ZERO_ADDRESS
+from vyper.utils import keccak256
 
-@pytest.fixture
-def c(w3, get_contract):
-    a0, a1, a2, a3, a4, a5, a6 = w3.eth.accounts[:7]
+
+@pytest.fixture(scope="module")
+def c(env, get_contract):
+    a0, a1, a2, a3, a4, a5, a6 = env.accounts[:7]
     with open("examples/wallet/wallet.vy") as f:
         code = f.read()
     # Sends wei to the contract for future transactions gas costs
     c = get_contract(code, *[[a1, a2, a3, a4, a5], 3])
-    w3.eth.send_transaction({"to": c.address, "value": 10**17})
+    env.set_balance(a0, 10**17)
+    env.message_call(c.address, value=10**17)
     return c
 
 
-@pytest.fixture
-def sign(keccak):
-    def _sign(seq, to, value, data, key):
-        keys = KeyAPI()
-        comb = seq.to_bytes(32, "big") + b"\x00" * 12 + to + value.to_bytes(32, "big") + data
-        h1 = keccak(comb)
-        h2 = keccak(b"\x19Ethereum Signed Message:\n32" + h1)
-        sig = keys.ecdsa_sign(h2, key)
-        return [28 if sig.v == 1 else 27, sig.r, sig.s]
-
-    return _sign
-
-
-def test_approve(w3, c, tester, tx_failed, sign):
-    a0, a1, a2, a3, a4, a5, a6 = w3.eth.accounts[:7]
-    k0, k1, k2, k3, k4, k5, k6, k7 = tester.backend.account_keys[:8]
+def sign(seq, to, value, data, key):
+    keys = KeyAPI()
+    comb = seq.to_bytes(32, "big") + b"\x00" * 12 + to + value.to_bytes(32, "big") + data
+    h1 = keccak256(comb)
+    h2 = keccak256(b"\x19Ethereum Signed Message:\n32" + h1)
+    sig = keys.ecdsa_sign(h2, key)
+    return [28 if sig.v == 1 else 27, sig.r, sig.s]
+
+
+def test_approve(env, c, tx_failed):
+    a0, a1, a2, a3, a4, a5, a6 = env.accounts[:7]
+    k0, k1, k2, k3, k4, k5, k6, k7 = env._keys[:8]
+    env.set_balance(a1, 10**18)
 
     to, value, data = b"\x35" * 20, 10**16, b""
-    to_address = w3.to_checksum_address(to)
+    to_address = to_checksum_address(to)
 
     def pack_and_sign(seq, *args):
         sigs = [sign(seq, to, value, data, k) if k else [0, 0, 0] for k in args]
         return sigs
 
     # Legitimate approval
     sigs = pack_and_sign(0, k1, 0, k3, 0, k5)
-    c.approve(0, "0x" + to.hex(), value, data, sigs, transact={"value": value, "from": a1})
+    c.approve(0, "0x" + to.hex(), value, data, sigs, value=value, sender=a1)
     # Approve fails if only 2 signatures are given
     sigs = pack_and_sign(1, k1, 0, k3, 0, 0)
     with tx_failed():
-        c.approve(1, to_address, value, data, sigs, transact={"value": value, "from": a1})
+        c.approve(1, to_address, value, data, sigs, value=value, sender=a1)
     # Approve fails if an invalid signature is given
     sigs = pack_and_sign(1, k1, 0, k7, 0, k5)
     with tx_failed():
-        c.approve(1, to_address, value, data, sigs, transact={"value": value, "from": a1})
+        c.approve(1, to_address, value, data, sigs, value=value, sender=a1)
     # Approve fails if transaction number is incorrect (the first argument should be 1)
     sigs = pack_and_sign(0, k1, 0, k3, 0, k5)
     with tx_failed():
-        c.approve(0, to_address, value, data, sigs, transact={"value": value, "from": a1})
+        c.approve(0, to_address, value, data, sigs, value=value, sender=a1)
     # Approve fails if not enough value is sent
     sigs = pack_and_sign(1, k1, 0, k3, 0, k5)
     with tx_failed():
-        c.approve(1, to_address, value, data, sigs, transact={"value": 0, "from": a1})
+        c.approve(1, to_address, value, data, sigs, value=0, sender=a1)
     sigs = pack_and_sign(1, k1, 0, k3, 0, k5)
 
     # this call should succeed
-    c.approve(1, to_address, value, data, sigs, call={"value": value, "from": a1})
+    c.approve(1, to_address, value, data, sigs, value=value, sender=a1)
 
     print("Basic tests passed")
 
 
-def test_javascript_signatures(w3, get_contract):
-    a3 = w3.eth.accounts[2]
+def test_javascript_signatures(env, get_contract, keccak):
+    a3 = env.accounts[2]
     # The zero address will cause `approve` to default to valid signatures
-    zero_address = "0x0000000000000000000000000000000000000000"
     accounts = [
         "0x776ba14735ff84789320718cf0aa43e91f7a8ce1",
         "0x095ce4e4240fa66ff90282c26847456e3f3b5002",
     ]
     # The address that will receive the transaction
     recipient = "0x776Ba14735FF84789320718cf0aa43e91F7A8Ce1"
     # These are the matching sigs to the accounts
     raw_sigs = [
         "0x4a89507bf71749fb338ed13fba623a683d9ecab0fb9c389a4298525c043e38281a00ab65628bb18a382eb8c8b4fb4dae95ccc993cf49f617c60d8051180778601c",  # noqa: E501
         "0xc84fe5d2a600e033930e0cf73f26e78f4c65b134f9c9992f60f08ce0863abdbe0548a6e8aa2d952659f29c67106b59fdfcd64d67df03c1df620c70c85578ae701b",  # noqa: E501
     ]
 
     # Turns the raw sigs into sigs
     sigs = [
-        (w3.to_int(x[64:]), w3.to_int(x[:32]), w3.to_int(x[32:64]))  # v  # r  # s
-        for x in map(lambda z: w3.to_bytes(hexstr=z[2:]), raw_sigs)
+        (to_int(x[64:]), to_int(x[:32]), to_int(x[32:64]))  # v  # r  # s
+        for x in map(lambda z: to_bytes(hexstr=z[2:]), raw_sigs)
     ]
 
-    h = w3.keccak(
+    h = keccak(
         (0).to_bytes(32, "big")
         + b"\x00" * 12
-        + w3.to_bytes(hexstr=recipient[2:])
+        + to_bytes(hexstr=recipient[2:])
         + (25).to_bytes(32, "big")
         + b""
     )  # noqa: E501
     h2 = encode_defunct(h)
 
     # Check to make sure the signatures are valid
     assert is_same_address(Account.recover_message(h2, sigs[0]), accounts[0])
     assert is_same_address(Account.recover_message(h2, sigs[1]), accounts[1])
 
     # Set the owners to zero addresses
     with open("examples/wallet/wallet.vy") as f:
-        owners = [w3.to_checksum_address(x) for x in accounts + [a3, zero_address, zero_address]]
+        owners = [to_checksum_address(x) for x in accounts + [a3, ZERO_ADDRESS, ZERO_ADDRESS]]
         x2 = get_contract(f.read(), *[owners, 2])
 
-    w3.eth.send_transaction({"to": x2.address, "value": 10**17})
+    env.set_balance(env.deployer, 10**18)
+    env.message_call(x2.address, value=10**17)
 
     # There's no need to pass in signatures because the owners are 0 addresses
     # causing them to default to valid signatures
-    x2.approve(
-        0, recipient, 25, b"", sigs + [[0, 0, 0]] * 3, call={"to": x2.address, "value": 10**17}
-    )
-
-    print("Javascript signature tests passed")
+    x2.approve(0, recipient, 25, b"", sigs + [[0, 0, 0]] * 3, value=10**17)
```

### Comparing `vyper-0.4.0rc2/tests/functional/grammar/test_grammar.py` & `vyper-0.4.0rc3/tests/functional/grammar/test_grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_argument_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_argument_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_call_violation.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_call_violation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_constancy_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_constancy_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_function_declaration_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_function_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_instantiation_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_instantiation_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_literal_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_literal_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_payable.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_reference.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_reference.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_invalid_type_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_invalid_type_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_namespace_collision.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_namespace_collision.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_overflow_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_overflow_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_structure_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_structure_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_syntax_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_type_mismatch_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_type_mismatch_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_undeclared_definition.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_undeclared_definition.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_variable_declaration_exception.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_variable_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/exceptions/test_vyper_exception_pos.py` & `vyper-0.4.0rc3/tests/functional/syntax/exceptions/test_vyper_exception_pos.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/modules/test_deploy_visibility.py` & `vyper-0.4.0rc3/tests/functional/syntax/modules/test_deploy_visibility.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/modules/test_exports.py` & `vyper-0.4.0rc3/tests/functional/syntax/modules/test_exports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/modules/test_implements.py` & `vyper-0.4.0rc3/tests/functional/syntax/modules/test_implements.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/modules/test_initializers.py` & `vyper-0.4.0rc3/tests/functional/syntax/modules/test_initializers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/names/test_event_names.py` & `vyper-0.4.0rc3/tests/functional/syntax/names/test_event_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/names/test_function_names.py` & `vyper-0.4.0rc3/tests/functional/syntax/names/test_function_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/names/test_variable_names.py` & `vyper-0.4.0rc3/tests/functional/syntax/names/test_variable_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/signatures/test_invalid_function_decorators.py` & `vyper-0.4.0rc3/tests/functional/syntax/signatures/test_invalid_function_decorators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/signatures/test_method_id_conflicts.py` & `vyper-0.4.0rc3/tests/functional/syntax/signatures/test_method_id_conflicts.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_abi_decode.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_abi_decode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_abi_encode.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_abs.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_addmulmod.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_addmulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_address_code.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_address_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,65 @@
+import json
 from typing import Type
 
 import pytest
-from eth_tester.exceptions import TransactionFailed
-from web3 import Web3
 
 from vyper import compiler
-from vyper.compiler.settings import Settings
 from vyper.exceptions import NamespaceCollision, StructureException, VyperException
 
 # For reproducibility, use precompiled data of `hello: public(uint256)` using vyper 0.3.1
-PRECOMPILED_ABI = """[{"stateMutability": "view", "type": "function", "name": "hello", "inputs": [], "outputs": [{"name": "", "type": "uint256"}], "gas": 2460}]"""  # noqa: E501
+PRECOMPILED_ABI = """[{"stateMutability": "view", "type": "function", "name": "hello", "inputs": [], "outputs": [{"name": "", "type": "uint256"}], "gas": 2460}]"""  # noqa: E501, FS003
 PRECOMPILED_BYTECODE = """0x61004456600436101561000d57610035565b60046000601c376000513461003b576319ff1d2181186100335760005460e052602060e0f35b505b60006000fd5b600080fd5b61000461004403610004600039610004610044036000f3"""  # noqa: E501
 PRECOMPILED_BYTECODE_RUNTIME = """0x600436101561000d57610035565b60046000601c376000513461003b576319ff1d2181186100335760005460e052602060e0f35b505b60006000fd5b600080fd"""  # noqa: E501
 PRECOMPILED = bytes.fromhex(PRECOMPILED_BYTECODE_RUNTIME[2:])
 
 
-def _deploy_precompiled_contract(w3: Web3):
-    Precompiled = w3.eth.contract(abi=PRECOMPILED_ABI, bytecode=PRECOMPILED_BYTECODE)
-    tx_hash = Precompiled.constructor().transact()
-    tx_receipt = w3.eth.wait_for_transaction_receipt(tx_hash)
-    address = tx_receipt["contractAddress"]
-    return w3.eth.contract(address=address, abi=PRECOMPILED_ABI)
+@pytest.fixture
+def precompiled_contract(env):
+    bytecode = bytes.fromhex(PRECOMPILED_BYTECODE.removeprefix("0x"))
+    return env.deploy(json.loads(PRECOMPILED_ABI), bytecode)
 
 
 @pytest.mark.parametrize(
     ("start", "length", "expected"), [(0, 5, PRECOMPILED[:5]), (5, 10, PRECOMPILED[5:][:10])]
 )
-def test_address_code_slice(start: int, length: int, expected: bytes, w3: Web3, get_contract):
+def test_address_code_slice(
+    start: int, length: int, expected: bytes, precompiled_contract, get_contract
+):
     code = f"""
 @external
 def code_slice(x: address) -> Bytes[{length}]:
     return slice(x.code, {start}, {length})
 """
     contract = get_contract(code)
-    precompiled_contract = _deploy_precompiled_contract(w3)
     actual = contract.code_slice(precompiled_contract.address)
     assert actual == expected
 
 
-def test_address_code_runtime_error_slice_too_long(w3: Web3, get_contract):
+def test_address_code_runtime_error_slice_too_long(precompiled_contract, get_contract, tx_failed):
     start = len(PRECOMPILED) - 5
     length = 10
     code = f"""
 @external
 def code_slice(x: address) -> Bytes[{length}]:
     return slice(x.code, {start}, {length})
 """
     contract = get_contract(code)
-    precompiled_contract = _deploy_precompiled_contract(w3)
-    with pytest.raises(TransactionFailed):
+    with tx_failed():
         contract.code_slice(precompiled_contract.address)
 
 
-def test_address_code_runtime_error_no_code(get_contract):
+def test_address_code_runtime_error_no_code(get_contract, tx_failed):
     code = """
 @external
 def code_slice(x: address) -> Bytes[4]:
     return slice(x.code, 0, 4)
 """
     contract = get_contract(code)
-    with pytest.raises(TransactionFailed):
+    with tx_failed():
         contract.code_slice(b"\x00" * 20)
 
 
 @pytest.mark.parametrize(
     ("bad_code", "error_type", "error_message"),
     [
         (
@@ -157,49 +153,46 @@
 """,
     ],
 )
 def test_address_code_compile_success(code: str):
     compiler.compile_code(code)
 
 
-def test_address_code_self_success(get_contract, optimize, experimental_codegen):
+def test_address_code_self_success(get_contract):
     code = """
 code_deployment: public(Bytes[32])
 
 @deploy
 def __init__():
     self.code_deployment = slice(self.code, 0, 32)
 
 @external
 def code_runtime() -> Bytes[32]:
     return slice(self.code, 0, 32)
 """
     contract = get_contract(code)
-    settings = Settings(optimize=optimize, experimental_codegen=experimental_codegen)
-    code_compiled = compiler.compile_code(
-        code, output_formats=["bytecode", "bytecode_runtime"], settings=settings
-    )
+    code_compiled = compiler.compile_code(code, output_formats=["bytecode", "bytecode_runtime"])
     assert contract.code_deployment() == bytes.fromhex(code_compiled["bytecode"][2:])[:32]
     assert contract.code_runtime() == bytes.fromhex(code_compiled["bytecode_runtime"][2:])[:32]
 
 
-def test_address_code_self_runtime_error_deployment(get_contract):
+def test_address_code_self_runtime_error_deployment(get_contract, tx_failed):
     code = """
 dummy: public(Bytes[1000000])
 
 @deploy
 def __init__():
     self.dummy = slice(self.code, 0, 1000000)
 """
-    with pytest.raises(TransactionFailed):
+    with tx_failed():
         get_contract(code)
 
 
-def test_address_code_self_runtime_error_runtime(get_contract):
+def test_address_code_self_runtime_error_runtime(get_contract, tx_failed):
     code = """
 @external
 def code_runtime() -> Bytes[1000000]:
     return slice(self.code, 0, 1000000)
 """
     contract = get_contract(code)
-    with pytest.raises(TransactionFailed):
+    with tx_failed():
         contract.code_runtime()
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_ann_assign.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_ann_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_as_uint256.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_as_uint256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_as_wei_value.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_as_wei_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,9 +123,9 @@
 def foo():
     a: uint256 = x
     """,
 ]
 
 
 @pytest.mark.parametrize("good_code", valid_list)
-def test_as_wei_success(good_code, get_contract_with_gas_estimation):
-    assert get_contract_with_gas_estimation(good_code) is not None
+def test_as_wei_success(good_code, get_contract):
+    assert get_contract(good_code) is not None
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_block.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,7 +149,35 @@
     """,
 ]
 
 
 @pytest.mark.parametrize("good_code", valid_list)
 def test_block_success(good_code):
     assert compiler.compile_code(good_code) is not None
+
+
+valid_list = [
+    """
+@external
+def foo() -> uint256:
+    return block.blobbasefee
+    """,
+    """
+@external
+def foo() -> uint256:
+    a: uint256 = 5
+    a = block.blobbasefee
+    return a
+    """,
+    """
+@external
+def foo() -> uint256:
+    a: uint256 = block.blobbasefee
+    return a
+    """,
+]
+
+
+@pytest.mark.requires_evm_version("cancun")
+@pytest.mark.parametrize("good_code", valid_list)
+def test_block_blob_success(good_code):
+    assert compiler.compile_code(good_code) is not None
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_blockscope.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_blockscope.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_bool.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_bool.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,21 +148,21 @@
         (8, "", True),
         (40, "a", False),
         (40, "hellohellohellohellohellohellohellohello", False),
         (40, "", True),
     ],
 )
 @pytest.mark.parametrize("op", ["==", "!="])
-def test_empty_string_comparison(get_contract_with_gas_estimation, length, value, result, op):
+def test_empty_string_comparison(get_contract, length, value, result, op):
     contract = f"""
 @external
 def foo(xs: String[{length}]) -> bool:
     return xs {op} ""
     """
-    c = get_contract_with_gas_estimation(contract)
+    c = get_contract(contract)
     if op == "==":
         assert c.foo(value) == result
     elif op == "!=":
         assert c.foo(value) != result
 
 
 @pytest.mark.parametrize(
@@ -175,18 +175,18 @@
         (8, b"", True),
         (40, b"a", False),
         (40, b"hellohellohellohellohellohellohellohello", False),
         (40, b"", True),
     ],
 )
 @pytest.mark.parametrize("op", ["==", "!="])
-def test_empty_bytes_comparison(get_contract_with_gas_estimation, length, value, result, op):
+def test_empty_bytes_comparison(get_contract, length, value, result, op):
     contract = f"""
 @external
 def foo(xs: Bytes[{length}]) -> bool:
     return b"" {op} xs
     """
-    c = get_contract_with_gas_estimation(contract)
+    c = get_contract(contract)
     if op == "==":
         assert c.foo(value) == result
     elif op == "!=":
         assert c.foo(value) != result
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_bytes.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_chainid.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_chainid.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,16 +77,16 @@
 
 
 @pytest.mark.parametrize("good_code", valid_list)
 def test_chain_success(good_code):
     assert compiler.compile_code(good_code) is not None
 
 
-def test_chainid_operation(get_contract_with_gas_estimation):
+def test_chainid_operation(get_contract, env):
     code = """
 @external
 @view
 def get_chain_id() -> uint256:
     return chain.id
     """
-    c = get_contract_with_gas_estimation(code)
-    assert c.get_chain_id() == 131277322940537  # Default value of py-evm
+    c = get_contract(code)
+    assert c.get_chain_id() == env.DEFAULT_CHAIN_ID
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_code_size.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_code_size.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_codehash.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_codehash.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from vyper.compiler import compile_code
-from vyper.compiler.settings import Settings
 from vyper.utils import keccak256
 
 
-def test_get_extcodehash(get_contract, optimize, experimental_codegen):
+def test_get_extcodehash(get_contract):
     code = """
 a: address
 
 @deploy
 def __init__():
     self.a = self
 
@@ -24,16 +23,15 @@
 def foo3() -> bytes32:
     return self.codehash
 
 @external
 def foo4() -> bytes32:
     return self.a.codehash
     """
-    settings = Settings(optimize=optimize, experimental_codegen=experimental_codegen)
-    compiled = compile_code(code, output_formats=["bytecode_runtime"], settings=settings)
+    compiled = compile_code(code, output_formats=["bytecode_runtime"])
     bytecode = bytes.fromhex(compiled["bytecode_runtime"][2:])
     hash_ = keccak256(bytecode)
 
     c = get_contract(code)
 
     assert c.foo(c.address) == hash_
     assert not int(c.foo("0xDeaDbeefdEAdbeefdEadbEEFdeadbeEFdEaDbeeF").hex(), 16)
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_concat.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_concat.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,16 +85,16 @@
     """,
         ArgumentException,
     ),
 ]
 
 
 @pytest.mark.parametrize("bad_code,exc", fail_list)
-def test_block_fail(assert_compile_failed, get_contract_with_gas_estimation, bad_code, exc):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(bad_code), exc)
+def test_block_fail(assert_compile_failed, get_contract, bad_code, exc):
+    assert_compile_failed(lambda: get_contract(bad_code), exc)
 
 
 valid_list = [
     """
 @external
 def cat(i1: Bytes[10], i2: Bytes[30]) -> Bytes[40]:
     return concat(i1, i2)
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_constants.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_create_with_code_of.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_create_with_code_of.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_dynamic_array.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_external_calls.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_external_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_extract32.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_extract32.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     """,
         InvalidType,  # output_type can't be bool
     ),
 ]
 
 
 @pytest.mark.parametrize("bad_code,exc", fail_list)
-def test_extract32_fail(assert_compile_failed, get_contract_with_gas_estimation, bad_code, exc):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(bad_code), exc)
+def test_extract32_fail(assert_compile_failed, get_contract, bad_code, exc):
+    assert_compile_failed(lambda: get_contract(bad_code), exc)
 
 
 valid_list = [
     """
 @external
 def foo() -> uint256:
     return extract32(
@@ -76,9 +76,9 @@
     self.x = b"cowcowcowcowcowccowcowcowcowcowccowcowcowcowcowccowcowcowcowcowc"
     return extract32(self.x, 1, output_type=uint256)
 """,
 ]
 
 
 @pytest.mark.parametrize("good_code", valid_list)
-def test_extract32_success(get_contract_with_gas_estimation, good_code):
-    assert get_contract_with_gas_estimation(good_code) is not None
+def test_extract32_success(get_contract, good_code):
+    assert get_contract(good_code) is not None
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_flag.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_for_range.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_functions_call.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_functions_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_immutables.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_immutables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_init.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_interfaces.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_invalids.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_invalids.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_keccak256.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_len.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_list.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_logging.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_method_id.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_minmax.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_minmax_value.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_msg_data.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_msg_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
-from eth_tester.exceptions import TransactionFailed
+from eth_utils import to_bytes
 
 from vyper import compiler
 from vyper.exceptions import StructureException, TypeMismatch
 from vyper.utils import method_id
 
 
-def test_variable_assignment(get_contract, keccak):
+def test_variable_assignment(get_contract):
     code = """
 @external
 def foo() -> Bytes[4]:
     bar: Bytes[4] = slice(msg.data, 0, 4)
     return bar
 """
 
@@ -27,27 +27,27 @@
 """
 
     contract = get_contract(code)
 
     assert contract.foo(42) == 42
 
 
-def test_get_full_calldata(get_contract, keccak, w3):
+def test_get_full_calldata(get_contract):
     code = """
 @external
 def foo(bar: uint256) -> Bytes[36]:
     data: Bytes[36] = slice(msg.data, 0, 36)
     return data
 """
     contract = get_contract(code)
 
     # 2fbebd38000000000000000000000000000000000000000000000000000000000000002a
-    selector_hex = method_id("foo(uint256)")  # 2fbebd38
-    encoded_42 = (42).to_bytes(32, "big")
-    expected_result = selector_hex + encoded_42
+    foo_method_id = method_id("foo(uint256)")  # 2fbebd38
+    encoded_42 = to_bytes(42)  # 2a
+    expected_result = foo_method_id + b"\0" * 31 + encoded_42
 
     assert contract.foo(42) == expected_result
 
 
 @pytest.mark.parametrize("bar", [0, 1, 42, 2**256 - 1])
 def test_calldata_private(get_contract, bar):
     code = """
@@ -69,29 +69,27 @@
     b: Bytes[4] = slice(msg.data, 0, 4)
     c: uint256 = max_value(uint256)
 
     return (a, b, c)
 """
     contract = get_contract(code)
 
-    assert contract.foo() == [2**256 - 1, method_id("foo()"), 2**256 - 1]
+    assert contract.foo() == (2**256 - 1, method_id("foo()"), 2**256 - 1)
 
 
-def test_assignment_to_storage(w3, get_contract, keccak):
+def test_assignment_to_storage(get_contract, keccak):
     code = """
 cache: public(Bytes[4])
 
 @external
 def foo():
     self.cache = slice(msg.data, 0, 4)
 """
-    acct = w3.eth.accounts[0]
     contract = get_contract(code)
-
-    contract.foo(transact={"from": acct})
+    contract.foo()
     assert contract.cache() == method_id("foo()")
 
 
 def test_get_len(get_contract):
     code = """
 @external
 def foo(bar: uint256) -> uint256:
@@ -154,19 +152,18 @@
 
 @pytest.mark.parametrize("bad_code", fail_list)
 def test_invalid_usages_compile_error(bad_code):
     with pytest.raises(bad_code[1]):
         compiler.compile_code(bad_code[0])
 
 
-def test_runtime_failure_bounds_check(get_contract):
+def test_runtime_failure_bounds_check(get_contract, tx_failed):
     code = """
 @external
 def foo(_value: uint256) -> uint256:
     val: Bytes[40] = slice(msg.data, 0, 40)
     return convert(slice(val, 4, 32), uint256)
 """
 
     contract = get_contract(code)
-
-    with pytest.raises(TransactionFailed):
+    with tx_failed():
         contract.foo(42)
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_nested_list.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_nested_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,9 +71,9 @@
 def foo():
     self.bar = [[1.0, 2.0, 3.0], [4.0, 5.0, 6.0], [7.0, 8.0, 9.0]]
     """,
 ]
 
 
 @pytest.mark.parametrize("good_code", valid_list)
-def test_nested_list_sucess(good_code):
+def test_nested_list_success(good_code):
     assert compiler.compile_code(good_code) is not None
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_no_none.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_no_none.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from vyper.exceptions import InvalidLiteral, SyntaxException
 
 
-def test_no_none_assign(assert_compile_failed, get_contract_with_gas_estimation):
+def test_no_none_assign(assert_compile_failed, get_contract):
     contracts = [  # noqa: E122
         """
 @external
 def foo():
     bar: int128 = 0
     bar = None
     """,
@@ -68,20 +68,18 @@
 @external
 def foo():
     bar: address = None
     """,
     ]
 
     for contract in contracts:
-        assert_compile_failed(
-            lambda c=contract: get_contract_with_gas_estimation(c), InvalidLiteral
-        )
+        assert_compile_failed(lambda c=contract: get_contract(c), InvalidLiteral)
 
 
-def test_no_is_none(assert_compile_failed, get_contract_with_gas_estimation):
+def test_no_is_none(assert_compile_failed, get_contract):
     contracts = [  # noqa: E122
         """
 @external
 def foo():
     bar: int128 = 0
     assert bar is None
     """,
@@ -114,20 +112,18 @@
 def foo():
     bar: address = empty(address)
     assert bar is None
     """,
     ]
 
     for contract in contracts:
-        assert_compile_failed(
-            lambda c=contract: get_contract_with_gas_estimation(c), SyntaxException
-        )
+        assert_compile_failed(lambda c=contract: get_contract(c), SyntaxException)
 
 
-def test_no_eq_none(assert_compile_failed, get_contract_with_gas_estimation):
+def test_no_eq_none(assert_compile_failed, get_contract):
     contracts = [  # noqa: E122
         """
 @external
 def foo():
     bar: int128 = 0
     assert bar == None
     """,
@@ -160,20 +156,18 @@
 def foo():
     bar: address = empty(address)
     assert bar == None
     """,
     ]
 
     for contract in contracts:
-        assert_compile_failed(
-            lambda c=contract: get_contract_with_gas_estimation(c), InvalidLiteral
-        )
+        assert_compile_failed(lambda c=contract: get_contract(c), InvalidLiteral)
 
 
-def test_struct_none(assert_compile_failed, get_contract_with_gas_estimation):
+def test_struct_none(assert_compile_failed, get_contract):
     contracts = [  # noqa: E122
         """
 struct Mom:
     a: uint256
     b: int128
 
 @external
@@ -197,10 +191,8 @@
 @external
 def foo():
     mom: Mom = Mom(a=None, b=None)
     """,
     ]
 
     for contract in contracts:
-        assert_compile_failed(
-            lambda c=contract: get_contract_with_gas_estimation(c), InvalidLiteral
-        )
+        assert_compile_failed(lambda c=contract: get_contract(c), InvalidLiteral)
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_powmod.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_print.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_print.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_public.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_raw_call.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_return_tuple.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_return_tuple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import pytest
 
 from vyper import compiler
 from vyper.exceptions import FunctionDeclarationException
 
-pytestmark = pytest.mark.usefixtures("memory_mocker")
-
 fail_list = [
     """
 @external
 def unmatched_tupl_length() -> (Bytes[8], int128, Bytes[8]):
     return "test", 123
     """
 ]
@@ -30,15 +28,15 @@
 @external
 def foo() -> (uint256, uint256, uint256, uint256, uint256):
     return 1, 2, self._foo(), 4, 5
     """
 
     c = get_contract(code)
 
-    assert c.foo() == [1, 2, 3, 4, 5]
+    assert c.foo() == (1, 2, 3, 4, 5)
 
 
 def test_call_in_call(get_contract):
     code = """
 @internal
 def _foo(a: uint256, b: uint256, c: uint256) -> (uint256, uint256, uint256, uint256, uint256):
     return 1, a, b, c, 5
@@ -51,15 +49,15 @@
 @external
 def foo() -> (uint256, uint256, uint256, uint256, uint256):
     return self._foo(2, 3, self._foo2())
     """
 
     c = get_contract(code)
 
-    assert c.foo() == [1, 2, 3, 4, 5]
+    assert c.foo() == (1, 2, 3, 4, 5)
 
 
 def test_nested_calls_in_tuple_return(get_contract):
     code = """
 @internal
 def _foo(a: uint256, b: uint256, c: uint256) -> (uint256, uint256):
     return 415, 3
@@ -82,15 +80,15 @@
 @external
 def foo() -> (uint256, uint256, uint256, uint256, uint256):
     return 1, 2, self._foo(6, 7, self._foo2(self._foo3(9, 11)))[1], self._foo4(), 5
     """
 
     c = get_contract(code)
 
-    assert c.foo() == [1, 2, 3, 4, 5]
+    assert c.foo() == (1, 2, 3, 4, 5)
 
 
 def test_external_call_in_return_tuple(get_contract):
     code = """
 @view
 @external
 def foo() -> (uint256, uint256):
@@ -105,15 +103,15 @@
 def foo(a: address) -> (uint256, uint256, uint256, uint256, uint256):
     return 1, 2, (staticcall Foo(a).foo())[0], 4, 5
     """
 
     c = get_contract(code)
     c2 = get_contract(code2)
 
-    assert c2.foo(c.address) == [1, 2, 3, 4, 5]
+    assert c2.foo(c.address) == (1, 2, 3, 4, 5)
 
 
 def test_nested_external_call_in_return_tuple(get_contract):
     code = """
 @view
 @external
 def foo() -> (uint256, uint256):
@@ -140,15 +138,15 @@
         staticcall Foo(a).bar((staticcall Foo(a).foo())[1])
     )
     """
 
     c = get_contract(code)
     c2 = get_contract(code2)
 
-    assert c2.foo(c.address) == [1, 2, 3, 4, 5]
+    assert c2.foo(c.address) == (1, 2, 3, 4, 5)
 
 
 def test_single_type_tuple_int(get_contract):
     code = """
 @view
 @external
 def foo() -> (uint256[3], uint256, uint256[2][2]):
@@ -158,16 +156,16 @@
 @external
 def foo2(a: int128, b: int128) -> (int128[5], int128, int128[2]):
     return [1,2,3,a,5], b, [7,8]
     """
 
     c = get_contract(code)
 
-    assert c.foo() == [[1, 2, 3], 4, [[5, 6], [7, 8]]]
-    assert c.foo2(4, 6) == [[1, 2, 3, 4, 5], 6, [7, 8]]
+    assert c.foo() == ([1, 2, 3], 4, [[5, 6], [7, 8]])
+    assert c.foo2(4, 6) == ([1, 2, 3, 4, 5], 6, [7, 8])
 
 
 def test_single_type_tuple_address(get_contract):
     code = """
 @view
 @external
 def foo() -> (address, address[2]):
@@ -175,27 +173,27 @@
         self,
         [0xF5D4020dCA6a62bB1efFcC9212AAF3c9819E30D7, 0xFFfFfFffFFfffFFfFFfFFFFFffFFFffffFfFFFfF]
     )
     """
 
     c = get_contract(code)
 
-    assert c.foo() == [
+    assert c.foo() == (
         c.address,
         [
             "0xF5D4020dCA6a62bB1efFcC9212AAF3c9819E30D7",
             "0xFFfFfFffFFfffFFfFFfFFFFFffFFFffffFfFFFfF",
         ],
-    ]
+    )
 
 
 def test_single_type_tuple_bytes(get_contract):
     code = """
 @view
 @external
 def foo() -> (Bytes[5], Bytes[5]):
     return b"hello", b"there"
     """
 
     c = get_contract(code)
 
-    assert c.foo() == [b"hello", b"there"]
+    assert c.foo() == (b"hello", b"there")
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_selfdestruct.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_send.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_slice.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_string.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_string.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,9 +50,9 @@
     """,
         StructureException,
     )
 ]
 
 
 @pytest.mark.parametrize("bad_code,exc", invalid_list)
-def test_string_fail(assert_compile_failed, get_contract_with_gas_estimation, bad_code, exc):
-    assert_compile_failed(lambda: get_contract_with_gas_estimation(bad_code), exc)
+def test_string_fail(assert_compile_failed, get_contract, bad_code, exc):
+    assert_compile_failed(lambda: get_contract(bad_code), exc)
```

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_structs.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_structs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_ternary.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_tuple_assign.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_tuple_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/functional/syntax/test_unbalanced_return.py` & `vyper-0.4.0rc3/tests/functional/syntax/test_unbalanced_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/abi_types/test_invalid_abi_types.py` & `vyper-0.4.0rc3/tests/unit/abi_types/test_invalid_abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_compare_nodes.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_compare_nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_binop_decimal.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_binop_decimal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_binop_int.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_binop_int.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_boolop.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_boolop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_compare.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_compare.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_subscript.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_subscript.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_fold_unaryop.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_fold_unaryop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_from_node.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_from_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_get_children.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_get_children.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_get_descendants.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_get_descendants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/nodes/test_hex.py` & `vyper-0.4.0rc3/tests/unit/ast/nodes/test_hex.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/test_annotate_and_optimize_ast.py` & `vyper-0.4.0rc3/tests/unit/ast/test_annotate_and_optimize_ast.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,9 +58,9 @@
 
 def test_it_rewrites_unary_subtractions():
     contract_ast, _ = get_contract_info(TEST_CONTRACT_SOURCE_CODE)
 
     function_def = contract_ast.body[2]
     return_stmt = function_def.body[0]
 
-    assert isinstance(return_stmt.value, python_ast.Num)
-    assert return_stmt.value.n == -1
+    assert isinstance(return_stmt.value, python_ast.Constant)
+    assert return_stmt.value.value == -1
```

### Comparing `vyper-0.4.0rc2/tests/unit/ast/test_ast_dict.py` & `vyper-0.4.0rc3/tests/unit/ast/test_ast_dict.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/test_metadata_journal.py` & `vyper-0.4.0rc3/tests/unit/ast/test_metadata_journal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/test_natspec.py` & `vyper-0.4.0rc3/tests/unit/ast/test_natspec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 from vyper import ast as vy_ast
+from vyper.compiler import compile_code
 from vyper.compiler.phases import CompilerData
 from vyper.exceptions import NatSpecSyntaxException
 
 test_code = """
 '''
 @title A simulator for Bug Bunny, the most famous Rabbit
 @license MIT
@@ -61,18 +62,18 @@
 
 def parse_natspec(code):
     vyper_ast = CompilerData(code).annotated_vyper_module
     return vy_ast.parse_natspec(vyper_ast)
 
 
 def test_documentation_example_output():
-    userdoc, devdoc = parse_natspec(test_code)
+    natspec = parse_natspec(test_code)
 
-    assert userdoc == expected_userdoc
-    assert devdoc == expected_devdoc
+    assert natspec.userdoc == expected_userdoc
+    assert natspec.devdoc == expected_devdoc
 
 
 def test_no_tags_implies_notice():
     code = """
 '''
 Because there is no tag, this docstring is handled as a notice.
 '''
@@ -80,21 +81,21 @@
 def foo():
     '''
     This one too!
     '''
     pass
     """
 
-    userdoc, devdoc = parse_natspec(code)
+    natspec = parse_natspec(code)
 
-    assert userdoc == {
+    assert natspec.userdoc == {
         "methods": {"foo()": {"notice": "This one too!"}},
         "notice": "Because there is no tag, this docstring is handled as a notice.",
     }
-    assert not devdoc
+    assert natspec.devdoc == {}
 
 
 def test_whitespace():
     code = """
 '''
         @dev
 
@@ -107,17 +108,17 @@
 
 
 We don't mind!
 
 @author Mr No-linter
                 '''
 """
-    _, devdoc = parse_natspec(code)
+    natspec = parse_natspec(code)
 
-    assert devdoc == {
+    assert natspec.devdoc == {
         "author": "Mr No-linter",
         "details": "Whitespace gets cleaned up, people can use awful formatting. We don't mind!",
     }
 
 
 def test_params():
     code = """
@@ -127,17 +128,17 @@
     @param bar a number
     @param baz also a number
     @dev we didn't document potato, but that's ok
     '''
     pass
     """
 
-    _, devdoc = parse_natspec(code)
+    natspec = parse_natspec(code)
 
-    assert devdoc == {
+    assert natspec.devdoc == {
         "methods": {
             "foo(int128,uint256,bytes32)": {
                 "details": "we didn't document potato, but that's ok",
                 "params": {"bar": "a number", "baz": "also a number"},
             }
         }
     }
@@ -150,17 +151,17 @@
     '''
     @return value of bar
     @return value of baz
     '''
     return bar, baz
     """
 
-    _, devdoc = parse_natspec(code)
+    natspec = parse_natspec(code)
 
-    assert devdoc == {
+    assert natspec.devdoc == {
         "methods": {
             "foo(int128,uint256)": {"returns": {"_0": "value of bar", "_1": "value of baz"}}
         }
     }
 
 
 def test_ignore_private_methods():
@@ -172,17 +173,17 @@
 
 @internal
 def notfoo(bar: int128, baz: uint256):
     '''@dev I will not be parsed.'''
     pass
     """
 
-    _, devdoc = parse_natspec(code)
+    natspec = parse_natspec(code)
 
-    assert devdoc["methods"] == {"foo(int128,uint256)": {"details": "I will be parsed."}}
+    assert natspec.devdoc["methods"] == {"foo(int128,uint256)": {"details": "I will be parsed."}}
 
 
 def test_partial_natspec():
     code = """
 @external
 def foo():
     '''
@@ -272,17 +273,17 @@
 @license {license}
 '''
 @external
 def foo():
     pass
     """
 
-    _, devdoc = parse_natspec(code)
+    natspec = parse_natspec(code)
 
-    assert devdoc == {"license": license}
+    assert natspec.devdoc == {"license": license}
 
 
 fields = ["title", "author", "license", "notice", "dev"]
 
 
 @pytest.mark.parametrize("field", fields)
 def test_empty_fields(field):
@@ -413,7 +414,25 @@
     return 1, 2
     """
 
     with pytest.raises(
         NatSpecSyntaxException, match="Number of documented return values exceeds actual number"
     ):
         parse_natspec(code)
+
+
+def test_natspec_parsed_implicitly():
+    # test natspec is parsed even if not explicitly requested
+    code = """
+'''
+@noticee x
+'''
+    """
+    with pytest.raises(NatSpecSyntaxException):
+        parse_natspec(code)
+
+    # check we can get ast
+    compile_code(code, output_formats=["ast_dict"])
+
+    # anything beyond ast is blocked
+    with pytest.raises(NatSpecSyntaxException):
+        compile_code(code, output_formats=["annotated_ast_dict"])
```

### Comparing `vyper-0.4.0rc2/tests/unit/ast/test_parser.py` & `vyper-0.4.0rc3/tests/unit/ast/test_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/test_pre_parser.py` & `vyper-0.4.0rc3/tests/unit/ast/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/ast/test_source_annotation.py` & `vyper-0.4.0rc3/tests/unit/ast/test_source_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/cli/storage_layout/test_storage_layout.py` & `vyper-0.4.0rc3/tests/unit/cli/storage_layout/test_storage_layout.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/cli/storage_layout/test_storage_layout_overrides.py` & `vyper-0.4.0rc3/tests/unit/cli/storage_layout/test_storage_layout_overrides.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/cli/vyper_compile/test_parse_args.py` & `vyper-0.4.0rc3/tests/unit/cli/vyper_compile/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_compile_json.py` & `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_compile_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,24 +68,29 @@
         "stateMutability": "nonpayable",
         "type": "function",
     }
 ]
 
 
 @pytest.fixture(scope="function")
-def input_json():
+def input_json(optimize, evm_version, experimental_codegen):
     return {
         "language": "Vyper",
         "sources": {
             "contracts/foo.vy": {"content": FOO_CODE},
             "contracts/library.vy": {"content": LIBRARY_CODE},
             "contracts/bar.vy": {"content": BAR_CODE},
         },
         "interfaces": {"contracts/ibar.json": {"abi": BAR_ABI}},
-        "settings": {"outputSelection": {"*": ["*"]}},
+        "settings": {
+            "outputSelection": {"*": ["*"]},
+            "optimize": optimize.name.lower(),
+            "evmVersion": evm_version,
+            "experimentalCodegen": experimental_codegen,
+        },
     }
 
 
 @pytest.fixture(scope="function")
 def input_bundle(input_json):
     # CMC 2023-12-11 maybe input_json -> JSONInputBundle should be a helper
     # function in `vyper_json.py`.
@@ -218,19 +223,14 @@
         contract_path="contracts/foo.vy",
         output_formats=["method_identifiers"],
         input_bundle=input_bundle,
     )["method_identifiers"]
     assert foo["evm"]["methodIdentifiers"] == method_identifiers
 
 
-def test_root_folder_not_exists(input_json):
-    with pytest.raises(FileNotFoundError):
-        compile_json(input_json, root_folder="/path/that/does/not/exist")
-
-
 def test_wrong_language():
     with pytest.raises(JSONError):
         compile_json({"language": "Solidity"})
 
 
 def test_exc_handler_raises_syntax(input_json):
     input_json["sources"]["badcode.vy"] = {"content": BAD_SYNTAX_CODE}
```

### Comparing `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_get_inputs.py` & `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_get_inputs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_get_settings.py` & `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_get_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_output_selection.py` & `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_output_selection.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py` & `vyper-0.4.0rc3/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/asm/test_asm_optimizer.py` & `vyper-0.4.0rc3/tests/unit/compiler/asm/test_asm_optimizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from vyper.compiler import compile_code
 from vyper.compiler.phases import CompilerData
 from vyper.compiler.settings import OptimizationLevel, Settings
+from vyper.ir.compile_ir import _merge_jumpdests
 
 codes = [
     """
 s: uint256
 
 @internal
 def ctor_only():
@@ -119,7 +120,13 @@
     input_bundle = make_input_bundle({"library.vy": library})
     res = compile_code(code, input_bundle=input_bundle, output_formats=["asm"])
     asm = res["asm"]
     assert "some_function()" in asm
 
     assert "unused1()" not in asm
     assert "unused2()" not in asm
+
+
+def test_merge_jumpdests():
+    asm = ["_sym_label_0", "JUMP", "PUSH0", "_sym_label_0", "JUMPDEST", "_sym_label_0", "JUMPDEST"]
+
+    assert _merge_jumpdests(asm) is False, "should not return True as no changes were made"
```

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/ir/test_compile_ir.py` & `vyper-0.4.0rc3/tests/unit/compiler/ir/test_compile_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/ir/test_optimize_ir.py` & `vyper-0.4.0rc3/tests/unit/compiler/ir/test_optimize_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/ir/test_with.py` & `vyper-0.4.0rc3/tests/unit/compiler/ir/test_with.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/test_abi.py` & `vyper-0.4.0rc3/tests/unit/compiler/test_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/test_bytecode_runtime.py` & `vyper-0.4.0rc3/tests/unit/compiler/test_bytecode_runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,20 +120,18 @@
     assert data_section_lengths == []
     assert immutables_len == 32
     assert compiler == {"vyper": list(vyper.version.version_tuple)}
 
 
 # check that deployed bytecode actually matches the cbor metadata
 @pytest.mark.parametrize("code", [simple_contract_code, has_immutables, many_functions])
-def test_bytecode_signature_deployed(code, get_contract, w3):
+def test_bytecode_signature_deployed(code, get_contract, env):
     c = get_contract(code)
-    deployed_code = w3.eth.get_code(c.address)
+    deployed_code = env.get_code(c.address)
 
-    initcode = c._classic_contract.bytecode
-
-    metadata = _parse_cbor_metadata(initcode)
+    metadata = _parse_cbor_metadata(c.bytecode)
     runtime_len, data_section_lengths, immutables_len, compiler = metadata
 
     assert compiler == {"vyper": list(vyper.version.version_tuple)}
 
     # runtime_len includes data sections but not immutables
     assert len(deployed_code) == runtime_len + immutables_len
```

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/test_compile_code.py` & `vyper-0.4.0rc3/tests/unit/compiler/test_compile_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/test_default_settings.py` & `vyper-0.4.0rc3/tests/unit/compiler/test_default_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/test_input_bundle.py` & `vyper-0.4.0rc3/tests/unit/compiler/test_input_bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,21 +69,21 @@
 def test_load_abi(make_file, input_bundle, tmp_path):
     contents = json.dumps("some string")
 
     path = make_file("foo.json", contents)
 
     file = input_bundle.load_file("foo.json")
     assert isinstance(file, ABIInput)
-    assert file == ABIInput(0, "foo.json", path, "some string")
+    assert file == ABIInput(0, "foo.json", path, contents, "some string")
 
     # suffix doesn't matter
     path = make_file("foo.txt", contents)
     file = input_bundle.load_file("foo.txt")
     assert isinstance(file, ABIInput)
-    assert file == ABIInput(1, "foo.txt", path, "some string")
+    assert file == ABIInput(1, "foo.txt", path, contents, "some string")
 
 
 # check that unique paths give unique source ids
 def test_source_id_file_input(make_file, input_bundle, tmp_path):
     foopath = make_file("foo.vy", "contents")
     barpath = make_file("bar.vy", "contents 2")
 
@@ -122,37 +122,39 @@
 
     foopath = make_file("foo.json", contents)
 
     barpath = make_file("bar.json", contents2)
 
     file = input_bundle.load_file("foo.json")
     assert isinstance(file, ABIInput)
-    assert file == ABIInput(0, "foo.json", foopath, "some string")
+    assert file == ABIInput(0, "foo.json", foopath, contents, "some string")
 
     file2 = input_bundle.load_file("bar.json")
     assert isinstance(file2, ABIInput)
-    assert file2 == ABIInput(1, "bar.json", barpath, ["some list"])
+    assert file2 == ABIInput(1, "bar.json", barpath, contents2, ["some list"])
 
     file3 = input_bundle.load_file("foo.json")
     assert file3.source_id == 0
-    assert file3 == ABIInput(0, "foo.json", foopath, "some string")
+    assert file3 == ABIInput(0, "foo.json", foopath, contents, "some string")
 
     # test source id is stable across different search paths
     with working_directory(tmp_path):
         with input_bundle.search_path(Path(".")):
             file4 = input_bundle.load_file("foo.json")
             assert file4.source_id == 0
-            assert file4 == ABIInput(0, "foo.json", foopath, "some string")
+            assert file4 == ABIInput(0, "foo.json", foopath, contents, "some string")
 
     # test source id is stable even when requested filename is different
     with working_directory(tmp_path.parent):
         with input_bundle.search_path(Path(".")):
             file5 = input_bundle.load_file(Path(tmp_path.stem) / "foo.json")
             assert file5.source_id == 0
-            assert file5 == ABIInput(0, Path(tmp_path.stem) / "foo.json", foopath, "some string")
+            assert file5 == ABIInput(
+                0, Path(tmp_path.stem) / "foo.json", foopath, contents, "some string"
+            )
 
 
 # test some pathological case where the file changes underneath
 def test_mutating_file_source_id(make_file, input_bundle, tmp_path):
     foopath = make_file("foo.vy", "contents")
 
     file = input_bundle.load_file("foo.vy")
@@ -234,11 +236,12 @@
     some_abi_str = json.dumps(some_abi)
     foopath = PurePath("foo.json")
     barpath = PurePath("bar.txt")
     files = {foopath: {"abi": some_abi}, barpath: {"content": some_abi_str}}
     input_bundle = JSONInputBundle(files, [PurePath(".")])
 
     file = input_bundle.load_file(foopath)
-    assert file == ABIInput(0, foopath, foopath, some_abi)
+    abi_contents = json.dumps({"abi": some_abi})
+    assert file == ABIInput(0, foopath, foopath, abi_contents, some_abi)
 
     file = input_bundle.load_file(barpath)
-    assert file == ABIInput(1, barpath, barpath, some_abi)
+    assert file == ABIInput(1, barpath, barpath, some_abi_str, some_abi)
```

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/test_opcodes.py` & `vyper-0.4.0rc3/tests/unit/compiler/test_opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/test_pre_parser.py` & `vyper-0.4.0rc3/tests/unit/compiler/test_pre_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from vyper.compiler import compile_code
 from vyper.compiler.settings import OptimizationLevel, Settings
-from vyper.exceptions import StructureException, SyntaxException
+from vyper.exceptions import SyntaxException
 
 
 def test_semicolon_prohibited(get_contract):
     code = """@external
 def test() -> int128:
     a: int128 = 1; b: int128 = 2
     return a + b
@@ -92,38 +92,38 @@
     code = """
 #pragma evm-version london
     """
     assert compile_code(code, settings=Settings(evm_version=None)) is not None
     assert compile_code(code, settings=Settings(evm_version="london")) is not None
     # should fail if compile options indicate different evm version
     # from source pragma
-    with pytest.raises(StructureException):
+    with pytest.raises(ValueError):
         compile_code(code, settings=Settings(evm_version="shanghai"))
 
 
 def test_optimization_mode_check():
     code = """
 #pragma optimize codesize
     """
     assert compile_code(code, settings=Settings(optimize=None))
     # should fail if compile options indicate different optimization mode
     # from source pragma
-    with pytest.raises(StructureException):
+    with pytest.raises(ValueError):
         compile_code(code, settings=Settings(optimize=OptimizationLevel.GAS))
-    with pytest.raises(StructureException):
+    with pytest.raises(ValueError):
         compile_code(code, settings=Settings(optimize=OptimizationLevel.NONE))
 
 
 def test_optimization_mode_check_none():
     code = """
 #pragma optimize none
     """
     assert compile_code(code, settings=Settings(optimize=None))
     # "none" conflicts with "gas"
-    with pytest.raises(StructureException):
+    with pytest.raises(ValueError):
         compile_code(code, settings=Settings(optimize=OptimizationLevel.GAS))
 
 
 def test_version_empty_version(assert_compile_failed, get_contract):
     code = """
 #@version
```

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/test_sha3_32.py` & `vyper-0.4.0rc3/tests/unit/compiler/test_sha3_32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/test_source_map.py` & `vyper-0.4.0rc3/tests/unit/compiler/test_source_map.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import namedtuple
 
 from vyper.compiler import compile_code
 from vyper.compiler.output import _compress_source_map
+from vyper.compiler.settings import OptimizationLevel
 from vyper.compiler.utils import expand_source_map
 
 TEST_CODE = """
 x: public(uint256)
 
 @internal
 def _baz(a: int128) -> int128:
@@ -27,28 +28,43 @@
     if self._bar(a):
         return self._baz(2)
     else:
         return 42
     """
 
 
-def test_jump_map():
+def test_jump_map(optimize, experimental_codegen):
     source_map = compile_code(TEST_CODE, output_formats=["source_map"])["source_map"]
     pos_map = source_map["pc_pos_map"]
     jump_map = source_map["pc_jump_map"]
 
-    assert len([v for v in jump_map.values() if v == "o"]) == 1
+    expected_jumps = 1
+    if optimize == OptimizationLevel.NONE:
+        # some jumps which don't get optimized out when optimizer is off
+        # (slightly different behavior depending if venom pipeline is enabled):
+        if not experimental_codegen:
+            expected_jumps = 3
+        else:
+            expected_jumps = 2
+
+    assert len([v for v in jump_map.values() if v == "o"]) == expected_jumps
     assert len([v for v in jump_map.values() if v == "i"]) == 2
 
     code_lines = [i + "\n" for i in TEST_CODE.split("\n")]
     for pc in [k for k, v in jump_map.items() if v == "o"]:
+        if pc not in pos_map:
+            assert optimize == OptimizationLevel.NONE
+            continue  # some jump is not being optimized out
         lineno, col_offset, _, end_col_offset = pos_map[pc]
         assert code_lines[lineno - 1][col_offset:end_col_offset].startswith("return")
 
     for pc in [k for k, v in jump_map.items() if v == "i"]:
+        if pc not in pos_map:
+            assert optimize == OptimizationLevel.NONE
+            continue  # some jump is not being optimized out
         lineno, col_offset, _, end_col_offset = pos_map[pc]
         assert code_lines[lineno - 1][col_offset:end_col_offset].startswith("self.")
 
 
 def test_pos_map_offsets():
     source_map = compile_code(TEST_CODE, output_formats=["source_map"])["source_map"]
     expanded = expand_source_map(source_map["pc_pos_map_compressed"])
```

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/venom/test_convert_basicblock_simple.py` & `vyper-0.4.0rc3/tests/unit/compiler/venom/test_convert_basicblock_simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 def test_simple():
     ir = IRnode.from_list(["calldatacopy", 32, 0, ["calldatasize"]])
     ir_node = IRnode.from_list(ir)
     venom = ir_node_to_venom(ir_node)
     assert venom is not None
 
-    bb = venom.basic_blocks[0]
+    fn = list(venom.functions.values())[0]
+
+    bb = fn.entry
     assert bb.instructions[0].opcode == "calldatasize"
     assert bb.instructions[1].opcode == "calldatacopy"
 
 
 def test_simple_2():
     ir = [
         "seq",
```

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/venom/test_duplicate_operands.py` & `vyper-0.4.0rc3/tests/unit/compiler/venom/test_duplicate_operands.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from vyper.compiler.settings import OptimizationLevel
 from vyper.venom import generate_assembly_experimental
-from vyper.venom.function import IRFunction
+from vyper.venom.context import IRContext
 
 
 def test_duplicate_operands():
     """
     Test the duplicate operands code generation.
     The venom code:
 
     %1 = 10
     %2 = add %1, %1
     %3 = mul %1, %2
     stop
 
     Should compile to: [PUSH1, 10, DUP1, DUP1, DUP1, ADD, MUL, STOP]
     """
-    ctx = IRFunction()
-    bb = ctx.get_basic_block()
+    ctx = IRContext()
+    fn = ctx.create_function("test")
+    bb = fn.get_basic_block()
     op = bb.append_instruction("store", 10)
     sum_ = bb.append_instruction("add", op, op)
     bb.append_instruction("mul", sum_, op)
     bb.append_instruction("stop")
 
     asm = generate_assembly_experimental(ctx, optimize=OptimizationLevel.GAS)
     assert asm == ["PUSH1", 10, "DUP1", "DUP1", "ADD", "MUL", "STOP"]
```

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/venom/test_make_ssa.py` & `vyper-0.4.0rc3/tests/unit/compiler/venom/test_make_ssa.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from vyper.venom.analysis import calculate_cfg, calculate_liveness
+from vyper.venom.analysis.analysis import IRAnalysesCache
 from vyper.venom.basicblock import IRBasicBlock, IRLabel
-from vyper.venom.function import IRFunction
+from vyper.venom.context import IRContext
 from vyper.venom.passes.make_ssa import MakeSSA
 
 
 def test_phi_case():
-    ctx = IRFunction(IRLabel("_global"))
+    ctx = IRContext()
+    fn = ctx.create_function("_global")
 
-    bb = ctx.get_basic_block()
+    bb = fn.get_basic_block()
 
-    bb_cont = IRBasicBlock(IRLabel("condition"), ctx)
-    bb_then = IRBasicBlock(IRLabel("then"), ctx)
-    bb_else = IRBasicBlock(IRLabel("else"), ctx)
-    bb_if_exit = IRBasicBlock(IRLabel("if_exit"), ctx)
-    ctx.append_basic_block(bb_cont)
-    ctx.append_basic_block(bb_then)
-    ctx.append_basic_block(bb_else)
-    ctx.append_basic_block(bb_if_exit)
+    bb_cont = IRBasicBlock(IRLabel("condition"), fn)
+    bb_then = IRBasicBlock(IRLabel("then"), fn)
+    bb_else = IRBasicBlock(IRLabel("else"), fn)
+    bb_if_exit = IRBasicBlock(IRLabel("if_exit"), fn)
+    fn.append_basic_block(bb_cont)
+    fn.append_basic_block(bb_then)
+    fn.append_basic_block(bb_else)
+    fn.append_basic_block(bb_if_exit)
 
     v = bb.append_instruction("mload", 64)
     bb_cont.append_instruction("jnz", v, bb_then.label, bb_else.label)
 
     bb_if_exit.append_instruction("add", v, 1, ret=v)
     bb_if_exit.append_instruction("jmp", bb_cont.label)
 
     bb_then.append_instruction("assert", bb_then.append_instruction("mload", 96))
     bb_then.append_instruction("jmp", bb_if_exit.label)
     bb_else.append_instruction("jmp", bb_if_exit.label)
 
     bb.append_instruction("jmp", bb_cont.label)
 
-    calculate_cfg(ctx)
-    MakeSSA().run_pass(ctx, ctx.basic_blocks[0])
-    calculate_liveness(ctx)
+    ac = IRAnalysesCache(fn)
+    MakeSSA(ac, fn).run_pass()
 
-    condition_block = ctx.get_basic_block("condition")
+    condition_block = fn.get_basic_block("condition")
     assert len(condition_block.instructions) == 2
 
     phi_inst = condition_block.instructions[0]
     assert phi_inst.opcode == "phi"
     assert phi_inst.operands[0].name == "_global"
     assert phi_inst.operands[1].name == "%1"
     assert phi_inst.operands[2].name == "if_exit"
```

### Comparing `vyper-0.4.0rc2/tests/unit/compiler/venom/test_multi_entry_block.py` & `vyper-0.4.0rc3/tests/unit/compiler/venom/test_multi_entry_block.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,138 +1,146 @@
-from vyper.venom.analysis import calculate_cfg
-from vyper.venom.function import IRBasicBlock, IRFunction, IRLabel
+from vyper.venom.analysis.analysis import IRAnalysesCache
+from vyper.venom.analysis.cfg import CFGAnalysis
+from vyper.venom.context import IRContext
+from vyper.venom.function import IRBasicBlock, IRLabel
 from vyper.venom.passes.normalization import NormalizationPass
 
 
 def test_multi_entry_block_1():
-    ctx = IRFunction()
+    ctx = IRContext()
+    fn = ctx.create_function("__global")
 
     finish_label = IRLabel("finish")
     target_label = IRLabel("target")
-    block_1_label = IRLabel("block_1", ctx)
+    block_1_label = IRLabel("block_1", fn)
 
-    bb = ctx.get_basic_block()
+    bb = fn.get_basic_block()
     op = bb.append_instruction("store", 10)
     acc = bb.append_instruction("add", op, op)
     bb.append_instruction("jnz", acc, finish_label, block_1_label)
 
-    block_1 = IRBasicBlock(block_1_label, ctx)
-    ctx.append_basic_block(block_1)
+    block_1 = IRBasicBlock(block_1_label, fn)
+    fn.append_basic_block(block_1)
     acc = block_1.append_instruction("add", acc, op)
     op = block_1.append_instruction("store", 10)
     block_1.append_instruction("mstore", acc, op)
     block_1.append_instruction("jnz", acc, finish_label, target_label)
 
-    target_bb = IRBasicBlock(target_label, ctx)
-    ctx.append_basic_block(target_bb)
+    target_bb = IRBasicBlock(target_label, fn)
+    fn.append_basic_block(target_bb)
     target_bb.append_instruction("mul", acc, acc)
     target_bb.append_instruction("jmp", finish_label)
 
-    finish_bb = IRBasicBlock(finish_label, ctx)
-    ctx.append_basic_block(finish_bb)
+    finish_bb = IRBasicBlock(finish_label, fn)
+    fn.append_basic_block(finish_bb)
     finish_bb.append_instruction("stop")
 
-    calculate_cfg(ctx)
-    assert not ctx.normalized, "CFG should not be normalized"
+    ac = IRAnalysesCache(fn)
+    ac.request_analysis(CFGAnalysis)
+    assert not fn.normalized, "CFG should not be normalized"
 
-    NormalizationPass().run_pass(ctx)
+    NormalizationPass(ac, fn).run_pass()
 
-    assert ctx.normalized, "CFG should be normalized"
+    assert fn.normalized, "CFG should be normalized"
 
-    finish_bb = ctx.get_basic_block(finish_label.value)
+    finish_bb = fn.get_basic_block(finish_label.value)
     cfg_in = list(finish_bb.cfg_in)
     assert cfg_in[0].label.value == "target", "Should contain target"
     assert cfg_in[1].label.value == "__global_split_finish", "Should contain __global_split_finish"
     assert cfg_in[2].label.value == "block_1_split_finish", "Should contain block_1_split_finish"
 
 
 # more complicated one
 def test_multi_entry_block_2():
-    ctx = IRFunction()
+    ctx = IRContext()
+    fn = ctx.create_function("__global")
 
     finish_label = IRLabel("finish")
     target_label = IRLabel("target")
-    block_1_label = IRLabel("block_1", ctx)
-    block_2_label = IRLabel("block_2", ctx)
+    block_1_label = IRLabel("block_1", fn)
+    block_2_label = IRLabel("block_2", fn)
 
-    bb = ctx.get_basic_block()
+    bb = fn.get_basic_block()
     op = bb.append_instruction("store", 10)
     acc = bb.append_instruction("add", op, op)
     bb.append_instruction("jnz", acc, finish_label, block_1_label)
 
-    block_1 = IRBasicBlock(block_1_label, ctx)
-    ctx.append_basic_block(block_1)
+    block_1 = IRBasicBlock(block_1_label, fn)
+    fn.append_basic_block(block_1)
     acc = block_1.append_instruction("add", acc, op)
     op = block_1.append_instruction("store", 10)
     block_1.append_instruction("mstore", acc, op)
     block_1.append_instruction("jnz", acc, target_label, finish_label)
 
-    block_2 = IRBasicBlock(block_2_label, ctx)
-    ctx.append_basic_block(block_2)
+    block_2 = IRBasicBlock(block_2_label, fn)
+    fn.append_basic_block(block_2)
     acc = block_2.append_instruction("add", acc, op)
     op = block_2.append_instruction("store", 10)
     block_2.append_instruction("mstore", acc, op)
     # switch the order of the labels, for fun and profit
     block_2.append_instruction("jnz", acc, finish_label, target_label)
 
-    target_bb = IRBasicBlock(target_label, ctx)
-    ctx.append_basic_block(target_bb)
+    target_bb = IRBasicBlock(target_label, fn)
+    fn.append_basic_block(target_bb)
     target_bb.append_instruction("mul", acc, acc)
     target_bb.append_instruction("jmp", finish_label)
 
-    finish_bb = IRBasicBlock(finish_label, ctx)
-    ctx.append_basic_block(finish_bb)
+    finish_bb = IRBasicBlock(finish_label, fn)
+    fn.append_basic_block(finish_bb)
     finish_bb.append_instruction("stop")
 
-    calculate_cfg(ctx)
-    assert not ctx.normalized, "CFG should not be normalized"
+    ac = IRAnalysesCache(fn)
+    ac.request_analysis(CFGAnalysis)
+    assert not fn.normalized, "CFG should not be normalized"
 
-    NormalizationPass().run_pass(ctx)
+    NormalizationPass(ac, fn).run_pass()
 
-    assert ctx.normalized, "CFG should be normalized"
+    assert fn.normalized, "CFG should be normalized"
 
-    finish_bb = ctx.get_basic_block(finish_label.value)
+    finish_bb = fn.get_basic_block(finish_label.value)
     cfg_in = list(finish_bb.cfg_in)
     assert cfg_in[0].label.value == "target", "Should contain target"
     assert cfg_in[1].label.value == "__global_split_finish", "Should contain __global_split_finish"
     assert cfg_in[2].label.value == "block_1_split_finish", "Should contain block_1_split_finish"
 
 
 def test_multi_entry_block_with_dynamic_jump():
-    ctx = IRFunction()
+    ctx = IRContext()
+    fn = ctx.create_function("__global")
 
     finish_label = IRLabel("finish")
     target_label = IRLabel("target")
-    block_1_label = IRLabel("block_1", ctx)
+    block_1_label = IRLabel("block_1", fn)
 
-    bb = ctx.get_basic_block()
+    bb = fn.get_basic_block()
     op = bb.append_instruction("store", 10)
     acc = bb.append_instruction("add", op, op)
     bb.append_instruction("djmp", acc, finish_label, block_1_label)
 
-    block_1 = IRBasicBlock(block_1_label, ctx)
-    ctx.append_basic_block(block_1)
+    block_1 = IRBasicBlock(block_1_label, fn)
+    fn.append_basic_block(block_1)
     acc = block_1.append_instruction("add", acc, op)
     op = block_1.append_instruction("store", 10)
     block_1.append_instruction("mstore", acc, op)
     block_1.append_instruction("jnz", acc, finish_label, target_label)
 
-    target_bb = IRBasicBlock(target_label, ctx)
-    ctx.append_basic_block(target_bb)
+    target_bb = IRBasicBlock(target_label, fn)
+    fn.append_basic_block(target_bb)
     target_bb.append_instruction("mul", acc, acc)
     target_bb.append_instruction("jmp", finish_label)
 
-    finish_bb = IRBasicBlock(finish_label, ctx)
-    ctx.append_basic_block(finish_bb)
+    finish_bb = IRBasicBlock(finish_label, fn)
+    fn.append_basic_block(finish_bb)
     finish_bb.append_instruction("stop")
 
-    calculate_cfg(ctx)
-    assert not ctx.normalized, "CFG should not be normalized"
+    ac = IRAnalysesCache(fn)
+    ac.request_analysis(CFGAnalysis)
+    assert not fn.normalized, "CFG should not be normalized"
 
-    NormalizationPass().run_pass(ctx)
-    assert ctx.normalized, "CFG should be normalized"
+    NormalizationPass(ac, fn).run_pass()
+    assert fn.normalized, "CFG should be normalized"
 
-    finish_bb = ctx.get_basic_block(finish_label.value)
+    finish_bb = fn.get_basic_block(finish_label.value)
     cfg_in = list(finish_bb.cfg_in)
     assert cfg_in[0].label.value == "target", "Should contain target"
     assert cfg_in[1].label.value == "__global_split_finish", "Should contain __global_split_finish"
     assert cfg_in[2].label.value == "block_1_split_finish", "Should contain block_1_split_finish"
```

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/analysis/test_array_index.py` & `vyper-0.4.0rc3/tests/unit/semantics/analysis/test_array_index.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/analysis/test_cyclic_function_calls.py` & `vyper-0.4.0rc3/tests/unit/semantics/analysis/test_cyclic_function_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/analysis/test_for_loop.py` & `vyper-0.4.0rc3/tests/unit/semantics/analysis/test_for_loop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/analysis/test_potential_types.py` & `vyper-0.4.0rc3/tests/unit/semantics/analysis/test_potential_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/conftest.py` & `vyper-0.4.0rc3/tests/unit/semantics/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/test_namespace.py` & `vyper-0.4.0rc3/tests/unit/semantics/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/test_storage_slots.py` & `vyper-0.4.0rc3/tests/unit/semantics/test_storage_slots.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/types/test_event.py` & `vyper-0.4.0rc3/tests/unit/semantics/types/test_event.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/types/test_pure_types.py` & `vyper-0.4.0rc3/tests/unit/semantics/types/test_pure_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/types/test_size_in_bytes.py` & `vyper-0.4.0rc3/tests/unit/semantics/types/test_size_in_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/types/test_type_from_abi.py` & `vyper-0.4.0rc3/tests/unit/semantics/types/test_type_from_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/unit/semantics/types/test_type_from_annotation.py` & `vyper-0.4.0rc3/tests/unit/semantics/types/test_type_from_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/tests/utils.py` & `vyper-0.4.0rc3/tests/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import decimal
 import os
 
 from vyper import ast as vy_ast
 from vyper.semantics.analysis.constant_folding import constant_fold
 from vyper.utils import DECIMAL_EPSILON, round_towards_zero
 
+ZERO_ADDRESS = "0x0000000000000000000000000000000000000000"
+
 
 @contextlib.contextmanager
 def working_directory(directory):
     tmp = os.getcwd()
     try:
         os.chdir(directory)
         yield
```

### Comparing `vyper-0.4.0rc2/vyper/__init__.py` & `vyper-0.4.0rc3/vyper/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,7 +17,10 @@
 else:
     __commit__ = "unknown"
 
 try:
     __version__ = _version(__name__)
 except PackageNotFoundError:
     from vyper.version import version as __version__
+
+# pep440 version with commit hash
+__long_version__ = f"{__version__}+commit.{__commit__}"
```

### Comparing `vyper-0.4.0rc2/vyper/__main__.py` & `vyper-0.4.0rc3/vyper/__main__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/abi_types.py` & `vyper-0.4.0rc3/vyper/abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ast/README.md` & `vyper-0.4.0rc3/vyper/ast/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ast/grammar.lark` & `vyper-0.4.0rc3/vyper/ast/grammar.lark`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ast/grammar.py` & `vyper-0.4.0rc3/vyper/ast/grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ast/identifiers.py` & `vyper-0.4.0rc3/vyper/ast/identifiers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ast/metadata.py` & `vyper-0.4.0rc3/vyper/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ast/natspec.py` & `vyper-0.4.0rc3/vyper/ast/natspec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import re
+from dataclasses import dataclass
 from typing import Optional, Tuple
 
 from asttokens import LineNumbers
 
 from vyper.ast import nodes as vy_ast
 from vyper.exceptions import NatSpecSyntaxException
 
 SINGLE_FIELDS = ("title", "author", "license", "notice", "dev")
 PARAM_FIELDS = ("param", "return")
 USERDOCS_FIELDS = ("notice",)
 
 
-def parse_natspec(annotated_vyper_module: vy_ast.Module) -> Tuple[dict, dict]:
+@dataclass
+class NatspecOutput:
+    userdoc: dict
+    devdoc: dict
+
+
+def parse_natspec(annotated_vyper_module: vy_ast.Module) -> NatspecOutput:
     """
     Parses NatSpec documentation from a contract.
 
     Arguments
     ---------
     annotated_vyper_module: Module
         Module-level vyper ast node.
@@ -59,15 +66,15 @@
         fn_natspec = _parse_docstring(source, docstring, invalid_fields, args, ret_len)
         for method_id in func_type.method_ids:
             if "notice" in fn_natspec:
                 userdoc.setdefault("methods", {})[method_id] = {"notice": fn_natspec.pop("notice")}
             if fn_natspec:
                 devdoc.setdefault("methods", {})[method_id] = fn_natspec
 
-    return userdoc, devdoc
+    return NatspecOutput(userdoc=userdoc, devdoc=devdoc)
 
 
 def _parse_docstring(
     source: str,
     docstring: str,
     invalid_fields: Tuple,
     params: Optional[Tuple] = None,
```

### Comparing `vyper-0.4.0rc2/vyper/ast/nodes.py` & `vyper-0.4.0rc3/vyper/ast/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -784,19 +784,14 @@
         return True
 
 
 class Num(Constant):
     # inherited class for all numeric constant node types
     __slots__ = ()
 
-    @property
-    def n(self):
-        # TODO phase out use of Num.n and remove this
-        return self.value
-
     def validate(self):
         if self.value < SizeLimits.MIN_INT256:
             raise OverflowException("Value is below lower bound for all numeric types", self)
         if self.value > SizeLimits.MAX_UINT256:
             raise OverflowException("Value exceeds upper bound for all numeric types", self)
 
 
@@ -890,19 +885,14 @@
     _translated_fields = {"s": "value"}
 
     def validate(self):
         for c in self.value:
             if ord(c) >= 256:
                 raise InvalidLiteral(f"'{c}' is not an allowed string literal character", self)
 
-    @property
-    def s(self):
-        # TODO phase out use of Str.s and remove this
-        return self.value
-
 
 class Bytes(Constant):
     __slots__ = ()
     _translated_fields = {"s": "value"}
 
     def __init__(self, parent: Optional["VyperNode"] = None, **kwargs: dict):
         super().__init__(parent, **kwargs)
@@ -1110,14 +1100,15 @@
         # the compiler to hang. the others will get caught during constant
         # folding or codegen.
         # l**r > 2**256
         # r * ln(l) > ln(2 ** 256)
         # r > ln(2 ** 256) / ln(l)
         if right > math.log(decimal.Decimal(2**257)) / math.log(decimal.Decimal(left)):
             raise InvalidLiteral("Out of bounds", self)
+
         return int(left**right)
 
 
 class BitAnd(Operator):
     __slots__ = ()
     _description = "bitwise and"
     _pretty = "&"
@@ -1389,15 +1380,15 @@
         self.is_transient = False
         self._expanded_getter = None
 
         def _check_args(annotation, call_name):
             # do the same thing as `validate_call_args`
             # (can't be imported due to cyclic dependency)
             if len(annotation.args) != 1:
-                raise ArgumentException("Invalid number of arguments to `{call_name}`:", self)
+                raise ArgumentException(f"Invalid number of arguments to `{call_name}`:", self)
 
         # the annotation is a "function" call, e.g.
         # `foo: public(constant(uint256))`
         # pretend we were parsing actual Vyper AST. annotation would be
         # TYPE | PUBLIC "(" TYPE | ((IMMUTABLE | CONSTANT) "(" TYPE ")") ")"
         if self.annotation.get("func.id") == "public":
             _check_args(self.annotation, "public")
```

### Comparing `vyper-0.4.0rc2/vyper/ast/nodes.pyi` & `vyper-0.4.0rc3/vyper/ast/nodes.pyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ast/parse.py` & `vyper-0.4.0rc3/vyper/ast/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,19 @@
         """
         Move a node docstring from body to `doc_string` and annotate it as `DocStr`.
         """
         self.generic_visit(node)
 
         if node.body:
             n = node.body[0]
-            if isinstance(n, python_ast.Expr) and isinstance(n.value, python_ast.Str):
+            if (
+                isinstance(n, python_ast.Expr)
+                and isinstance(n.value, python_ast.Constant)
+                and isinstance(n.value.value, str)
+            ):
                 self.generic_visit(n.value)
                 n.value.ast_type = "DocStr"
                 del node.body[0]
                 node.doc_string = n.value
 
         return node
 
@@ -466,19 +470,15 @@
         Adjust operand value and discard unary operations, where possible.
 
         This is done so that negative decimal literals are accurately represented.
         """
         self.generic_visit(node)
 
         is_sub = isinstance(node.op, python_ast.USub)
-        is_num = (
-            hasattr(node.operand, "n")
-            and not isinstance(node.operand.n, bool)
-            and isinstance(node.operand.n, (int, Decimal))
-        )
+        is_num = hasattr(node.operand, "value") and isinstance(node.operand.value, (int, Decimal))
         if is_sub and is_num:
-            node.operand.n = 0 - node.operand.n
+            node.operand.value = 0 - node.operand.value
             node.operand.col_offset = node.col_offset
             node.operand.node_source_code = node.node_source_code
             return node.operand
         else:
             return node
```

### Comparing `vyper-0.4.0rc2/vyper/ast/pre_parser.py` & `vyper-0.4.0rc3/vyper/ast/pre_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
                         except ValueError:
                             raise StructureException(f"Invalid optimization mode `{mode}`", start)
                     elif pragma.startswith("evm-version "):
                         if settings.evm_version is not None:
                             raise StructureException("pragma evm-version specified twice!", start)
                         evm_version = pragma.removeprefix("evm-version").strip()
                         if evm_version not in EVM_VERSIONS:
-                            raise StructureException("Invalid evm version: `{evm_version}`", start)
+                            raise StructureException(f"Invalid evm version: `{evm_version}`", start)
                         settings.evm_version = evm_version
                     elif pragma.startswith("experimental-codegen"):
                         if settings.experimental_codegen is not None:
                             raise StructureException(
                                 "pragma experimental-codegen specified twice!", start
                             )
                         settings.experimental_codegen = True
```

### Comparing `vyper-0.4.0rc2/vyper/ast/utils.py` & `vyper-0.4.0rc3/vyper/ast/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ast/validation.py` & `vyper-0.4.0rc3/vyper/ast/validation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/builtins/_convert.py` & `vyper-0.4.0rc3/vyper/builtins/_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/builtins/_signatures.py` & `vyper-0.4.0rc3/vyper/builtins/_signatures.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/builtins/_utils.py` & `vyper-0.4.0rc3/vyper/builtins/_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/builtins/functions.py` & `vyper-0.4.0rc3/vyper/builtins/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,19 @@
     shr,
     unwrap_location,
 )
 from vyper.codegen.expr import Expr
 from vyper.codegen.ir_node import Encoding, scope_multi
 from vyper.codegen.keccak256_helper import keccak256_helper
 from vyper.evm.address_space import MEMORY
+from vyper.evm.opcodes import version_check
 from vyper.exceptions import (
     ArgumentException,
     CompilerPanic,
+    EvmVersionException,
     InvalidLiteral,
     InvalidType,
     StateAccessViolation,
     StructureException,
     TypeMismatch,
     UnfoldableNode,
     ZeroDivisionException,
@@ -244,49 +246,49 @@
 
 def _build_adhoc_slice_node(sub: IRnode, start: IRnode, length: IRnode, context: Context) -> IRnode:
     assert length.is_literal, "typechecker failed"
     assert isinstance(length.value, int)  # mypy hint
 
     dst_typ = BytesT(length.value)
     # allocate a buffer for the return value
-    np = context.new_internal_variable(dst_typ)
+    buf = context.new_internal_variable(dst_typ)
 
     # `msg.data` by `calldatacopy`
     if sub.value == "~calldata":
         node = [
             "seq",
             _make_slice_bounds_check(start, length, "calldatasize"),
-            ["mstore", np, length],
-            ["calldatacopy", np + 32, start, length],
-            np,
+            ["mstore", buf, length],
+            ["calldatacopy", add_ofst(buf, 32), start, length],
+            buf,
         ]
 
     # `self.code` by `codecopy`
     elif sub.value == "~selfcode":
         node = [
             "seq",
             _make_slice_bounds_check(start, length, "codesize"),
-            ["mstore", np, length],
-            ["codecopy", np + 32, start, length],
-            np,
+            ["mstore", buf, length],
+            ["codecopy", add_ofst(buf, 32), start, length],
+            buf,
         ]
 
     # `<address>.code` by `extcodecopy`
     else:
         assert sub.value == "~extcode" and len(sub.args) == 1
         node = [
             "with",
             "_extcode_address",
             sub.args[0],
             [
                 "seq",
                 _make_slice_bounds_check(start, length, ["extcodesize", "_extcode_address"]),
-                ["mstore", np, length],
-                ["extcodecopy", "_extcode_address", np + 32, start, length],
-                np,
+                ["mstore", buf, length],
+                ["extcodecopy", "_extcode_address", add_ofst(buf, 32), start, length],
+                buf,
             ],
         ]
 
     assert isinstance(length.value, int)  # mypy hint
     return IRnode.from_list(node, typ=BytesT(length.value), location=MEMORY)
 
 
@@ -548,18 +550,16 @@
         if isinstance(args[0].typ, StringT):
             ret_typ = StringT(dst_maxlen)
         else:
             ret_typ = BytesT(dst_maxlen)
 
         # respect API of copy_bytes
         bufsize = dst_maxlen + 32
-        buf = context.new_internal_variable(BytesT(bufsize))
-
-        # Node representing the position of the output in memory
-        dst = IRnode.from_list(buf, typ=ret_typ, location=MEMORY, annotation="concat destination")
+        dst = context.new_internal_variable(BytesT(bufsize))
+        dst.annotation = "concat destination"
 
         ret = ["seq"]
         # stack item representing our current offset in the dst buffer
         ofst = "concat_ofst"
 
         # TODO: optimize for the case where all lengths are statically known.
         for arg in args:
@@ -779,33 +779,31 @@
         output_buf = context.new_internal_variable(get_type_for_exact_size(32))
         return IRnode.from_list(
             [
                 "seq",
                 # clear output memory first, ecrecover can return 0 bytes
                 ["mstore", output_buf, 0],
                 ["mstore", input_buf, args[0]],
-                ["mstore", input_buf + 32, args[1]],
-                ["mstore", input_buf + 64, args[2]],
-                ["mstore", input_buf + 96, args[3]],
+                ["mstore", add_ofst(input_buf, 32), args[1]],
+                ["mstore", add_ofst(input_buf, 64), args[2]],
+                ["mstore", add_ofst(input_buf, 96), args[3]],
                 ["staticcall", "gas", 1, input_buf, 128, output_buf, 32],
                 ["mload", output_buf],
             ],
             typ=AddressT(),
         )
 
 
 class _ECArith(BuiltinFunctionT):
     @process_inputs
     def build_IR(self, expr, _args, kwargs, context):
         args_tuple = ir_tuple_from_args(_args)
 
         args_t = args_tuple.typ
-        input_buf = IRnode.from_list(
-            context.new_internal_variable(args_t), typ=args_t, location=MEMORY
-        )
+        input_buf = context.new_internal_variable(args_t)
         ret_t = self._return_type
 
         ret = ["seq"]
         ret.append(make_setter(input_buf, args_tuple))
 
         output_buf = context.new_internal_variable(ret_t)
 
@@ -1099,17 +1097,15 @@
                 input_buf = IRnode.from_list("arg_buf")
             else:
                 call_ir = ["seq", eval_input_buf]
 
             args_ofst = add_ofst(input_buf, 32)
             args_len = ["mload", input_buf]
 
-        output_node = IRnode.from_list(
-            context.new_internal_variable(BytesT(outsize)), typ=BytesT(outsize), location=MEMORY
-        )
+        output_node = context.new_internal_variable(BytesT(outsize))
 
         bool_ty = BoolT()
 
         # build IR for call or delegatecall
         common_call_args = [
             args_ofst,
             args_len,
@@ -1215,14 +1211,26 @@
     def build_IR(self, expr, args, kwargs, contact):
         return IRnode.from_list(
             ["blockhash", clamp("lt", clamp("sge", args[0], ["sub", ["number"], 256]), "number")],
             typ=BYTES32_T,
         )
 
 
+class BlobHash(BuiltinFunctionT):
+    _id = "blobhash"
+    _inputs = [("index", UINT256_T)]
+    _return_type = BYTES32_T
+
+    @process_inputs
+    def build_IR(self, expr, args, kwargs, contact):
+        if not version_check(begin="cancun"):
+            raise EvmVersionException("`blobhash` is not available pre-cancun", expr)
+        return IRnode.from_list(["blobhash", args[0]], typ=BYTES32_T)
+
+
 class RawRevert(BuiltinFunctionT):
     _id = "raw_revert"
     _inputs = [("data", BytesT.any())]
     _return_type = None
     _is_terminus = True
 
     def fetch_call_return(self, node):
@@ -1654,16 +1662,16 @@
         "salt": KwargSettings(BYTES32_T, empty_value),
         "revert_on_failure": KwargSettings(BoolT(), True, require_literal=True),
     }
     _return_type = AddressT()
 
     @process_inputs
     def build_IR(self, expr, args, kwargs, context):
-        # errmsg something like "Cannot use {self._id} in pure fn"
-        context.check_is_not_constant("use {self._id}", expr)
+        # errmsg something like f"Cannot use {self._id} in pure fn"
+        context.check_is_not_constant(f"use {self._id}", expr)
 
         should_use_create2 = "salt" in [kwarg.arg for kwarg in expr.keywords]
 
         if not should_use_create2:
             kwargs["salt"] = CREATE2_SENTINEL
 
         ir_builder = self._build_create_IR(expr, args, context, **kwargs)
@@ -1708,16 +1716,16 @@
             aligned_target = shl(96, target_address)
 
         buf_len = preamble_length + 20 + len(forwarder_post_evm)
 
         return [
             "seq",
             ["mstore", buf, forwarder_preamble],
-            ["mstore", ["add", buf, preamble_length], aligned_target],
-            ["mstore", ["add", buf, preamble_length + 20], forwarder_post],
+            ["mstore", add_ofst(buf, preamble_length), aligned_target],
+            ["mstore", add_ofst(buf, preamble_length + 20), forwarder_post],
             _create_ir(value, buf, buf_len, salt, revert_on_failure),
         ]
 
 
 class CreateForwarderTo(CreateMinimalProxyTo):
     _warned = False
 
@@ -1818,17 +1826,15 @@
         else:
             # encode the varargs
             to_encode = ir_tuple_from_args(ctor_args)
 
             # pretend we allocated enough memory for the encoder
             # (we didn't, but we are clobbering unused memory so it's safe.)
             bufsz = to_encode.typ.abi_type.size_bound()
-            argbuf = IRnode.from_list(
-                context.new_internal_variable(get_type_for_exact_size(bufsz)), location=MEMORY
-            )
+            argbuf = context.new_internal_variable(get_type_for_exact_size(bufsz))
 
             # return a complex expression which writes to memory and returns
             # the length of the encoded data
             argslen = abi_encode(argbuf, to_encode, context, bufsz=bufsz, returns_len=True)
 
         # NOTE: we need to invoke the abi encoder before evaluating MSIZE,
         # then copy the abi encoded buffer to past-the-end of the initcode
@@ -2067,21 +2073,25 @@
                 "seq",
                 [
                     "if",
                     ["eq", val, 0],
                     # clobber val, and return it as a pointer
                     [
                         "seq",
-                        ["mstore", ["sub", buf + n_digits, i], i],
-                        ["set", val, ["sub", buf + n_digits, i]],
+                        ["mstore", ["sub", add_ofst(buf, n_digits), i], i],
+                        ["set", val, ["sub", add_ofst(buf, n_digits), i]],
                         "break",
                     ],
                     [
                         "seq",
-                        ["mstore", ["sub", buf + n_digits, i], ["add", 48, ["mod", val, 10]]],
+                        [
+                            "mstore",
+                            ["sub", add_ofst(buf, n_digits), i],
+                            ["add", 48, ["mod", val, 10]],
+                        ],
                         ["set", val, ["div", val, 10]],
                     ],
                 ],
             ]
             ret.append(body)
 
             # "0" has hex representation 0x00..0130..00
@@ -2089,15 +2099,15 @@
             #   return "0"
             # } else {
             #   do the loop
             # }
             ret = [
                 "if",
                 ["eq", val, 0],
-                ["seq", ["mstore", buf + 1, ord("0")], ["mstore", buf, 1], buf],
+                ["seq", ["mstore", add_ofst(buf, 1), ord("0")], ["mstore", buf, 1], buf],
                 ["seq", ret, val],
             ]
 
             return b1.resolve(IRnode.from_list(ret, location=MEMORY, typ=return_t))
 
 
 class Sqrt(BuiltinFunctionT):
@@ -2267,56 +2277,60 @@
             buflen = 32 + args_abi_t.size_bound()
 
             # 32 bytes extra space for the method id
             buf = context.new_internal_variable(get_type_for_exact_size(buflen))
 
             ret = ["seq"]
             ret.append(["mstore", buf, method_id])
-            encode = abi_encode(buf + 32, args_as_tuple, context, buflen, returns_len=True)
+            encode = abi_encode(add_ofst(buf, 32), args_as_tuple, context, buflen, returns_len=True)
 
         else:
             method_id = method_id_int("log(string,bytes)")
             schema = args_abi_t.selector_name().encode("utf-8")
             if len(schema) > 32:
-                raise CompilerPanic("print signature too long: {schema}")
+                raise CompilerPanic(f"print signature too long: {schema}")
 
             schema_t = StringT(len(schema))
             schema_buf = context.new_internal_variable(schema_t)
             ret = ["seq"]
             ret.append(["mstore", schema_buf, len(schema)])
 
             # TODO use Expr.make_bytelike, or better have a `bytestring` IRnode type
-            ret.append(["mstore", schema_buf + 32, bytes_to_int(schema.ljust(32, b"\x00"))])
+            ret.append(
+                ["mstore", add_ofst(schema_buf, 32), bytes_to_int(schema.ljust(32, b"\x00"))]
+            )
 
             payload_buflen = args_abi_t.size_bound()
             payload_t = BytesT(payload_buflen)
 
             # 32 bytes extra space for the method id
             payload_buf = context.new_internal_variable(payload_t)
             encode_payload = abi_encode(
-                payload_buf + 32, args_as_tuple, context, payload_buflen, returns_len=True
+                add_ofst(payload_buf, 32), args_as_tuple, context, payload_buflen, returns_len=True
             )
 
             ret.append(["mstore", payload_buf, encode_payload])
             args_as_tuple = ir_tuple_from_args(
                 [
                     IRnode.from_list(schema_buf, typ=schema_t, location=MEMORY),
                     IRnode.from_list(payload_buf, typ=payload_t, location=MEMORY),
                 ]
             )
 
             # add 32 for method id padding
             buflen = 32 + args_as_tuple.typ.abi_type.size_bound()
             buf = context.new_internal_variable(get_type_for_exact_size(buflen))
             ret.append(["mstore", buf, method_id])
-            encode = abi_encode(buf + 32, args_as_tuple, context, buflen, returns_len=True)
+            encode = abi_encode(add_ofst(buf, 32), args_as_tuple, context, buflen, returns_len=True)
 
         # debug address that tooling uses
         CONSOLE_ADDRESS = 0x000000000000000000636F6E736F6C652E6C6F67
-        ret.append(["staticcall", "gas", CONSOLE_ADDRESS, buf + 28, ["add", 4, encode], 0, 0])
+        ret.append(
+            ["staticcall", "gas", CONSOLE_ADDRESS, add_ofst(buf, 28), ["add", 4, encode], 0, 0]
+        )
 
         return IRnode.from_list(ret, annotation="print:" + sig)
 
 
 class ABIEncode(BuiltinFunctionT):
     _id = "_abi_encode"  # TODO prettier to rename this to abi.encode
     # signature: *, ensure_tuple=<literal_bool> -> Bytes[<calculated len>]
@@ -2411,23 +2425,27 @@
         buf = context.new_internal_variable(buf_t)
 
         ret = ["seq"]
         if method_id is not None:
             # <32 bytes length> | <4 bytes method_id> | <everything else>
             # write the unaligned method_id first, then we will
             # overwrite the 28 bytes of zeros with the bytestring length
-            ret += [["mstore", buf + 4, method_id]]
+            ret += [["mstore", add_ofst(buf, 4), method_id]]
             # abi encode, and grab length as stack item
-            length = abi_encode(buf + 36, encode_input, context, returns_len=True, bufsz=maxlen)
+            length = abi_encode(
+                add_ofst(buf, 36), encode_input, context, returns_len=True, bufsz=maxlen
+            )
             # write the output length to where bytestring stores its length
             ret += [["mstore", buf, ["add", length, 4]]]
 
         else:
             # abi encode and grab length as stack item
-            length = abi_encode(buf + 32, encode_input, context, returns_len=True, bufsz=maxlen)
+            length = abi_encode(
+                add_ofst(buf, 32), encode_input, context, returns_len=True, bufsz=maxlen
+            )
             # write the output length to where bytestring stores its length
             ret += [["mstore", buf, length]]
 
         # return the buf location
         # TODO location is statically known, optimize this out
         ret += [buf]
 
@@ -2504,21 +2522,20 @@
             )
             to_decode.encoding = Encoding.ABI
 
             # TODO optimization: skip make_setter when we don't need
             # input validation
 
             output_buf = context.new_internal_variable(wrapped_typ)
-            output = IRnode.from_list(output_buf, typ=wrapped_typ, location=MEMORY)
 
             # sanity check buffer size for wrapped output type will not buffer overflow
             assert wrapped_typ.memory_bytes_required == output_typ.memory_bytes_required
-            ret.append(make_setter(output, to_decode))
+            ret.append(make_setter(output_buf, to_decode))
 
-            ret.append(output)
+            ret.append(output_buf)
             # finalize. set the type and location for the return buffer.
             # (note: unwraps the tuple type if necessary)
             ret = IRnode.from_list(ret, typ=output_typ, location=MEMORY)
             return b1.resolve(ret)
 
 
 class _MinMaxValue(TypenameFoldedFunctionT):
@@ -2587,14 +2604,15 @@
     "ecrecover": ECRecover(),
     "ecadd": ECAdd(),
     "ecmul": ECMul(),
     "extract32": Extract32(),
     "as_wei_value": AsWeiValue(),
     "raw_call": RawCall(),
     "blockhash": BlockHash(),
+    "blobhash": BlobHash(),
     "bitwise_and": BitwiseAnd(),
     "bitwise_or": BitwiseOr(),
     "bitwise_xor": BitwiseXor(),
     "bitwise_not": BitwiseNot(),
     "uint256_addmod": AddMod(),
     "uint256_mulmod": MulMod(),
     "unsafe_add": UnsafeAdd(),
```

### Comparing `vyper-0.4.0rc2/vyper/builtins/interfaces/IERC20.vyi` & `vyper-0.4.0rc3/vyper/builtins/interfaces/IERC20.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/builtins/interfaces/IERC4626.vyi` & `vyper-0.4.0rc3/vyper/builtins/interfaces/IERC4626.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/builtins/interfaces/IERC721.vyi` & `vyper-0.4.0rc3/vyper/builtins/interfaces/IERC721.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/cli/vyper_compile.py` & `vyper-0.4.0rc3/vyper/cli/vyper_compile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 import argparse
 import json
+import os
 import sys
 import warnings
 from pathlib import Path
 from typing import Any, Iterable, Iterator, Optional, Set, TypeVar
 
 import vyper
 import vyper.codegen.ir_node as ir_node
 import vyper.evm.opcodes as evm
 from vyper.cli import vyper_json
+from vyper.cli.compile_archive import NotZipInput, compile_from_zip
 from vyper.compiler.input_bundle import FileInput, FilesystemInputBundle
 from vyper.compiler.settings import VYPER_TRACEBACK_LIMIT, OptimizationLevel, Settings
 from vyper.typing import ContractPath, OutputFormats
 
 T = TypeVar("T")
 
 format_options_help = """Format to print, one or more of:
@@ -35,14 +37,16 @@
 external_interface - External interface of a contract, used for outside contract calls
 opcodes            - List of opcodes as a string
 opcodes_runtime    - List of runtime opcodes as a string
 ir                 - Intermediate representation in list format
 ir_json            - Intermediate representation in JSON format
 ir_runtime         - Intermediate representation of runtime bytecode in list format
 asm                - Output the EVM assembly of the deployable bytecode
+archive            - Output the build as an archive file
+solc_json          - Output the build in solc json format
 """
 
 combined_json_outputs = [
     "bytecode",
     "bytecode_runtime",
     "blueprint_bytecode",
     "abi",
@@ -60,14 +64,28 @@
 
 def _cli_helper(f, output_formats, compiled):
     if output_formats == ("combined_json",):
         compiled = {str(path): v for (path, v) in compiled.items()}
         print(json.dumps(compiled), file=f)
         return
 
+    if output_formats == ("archive",):
+        for contract_data in compiled.values():
+            assert list(contract_data.keys()) == ["archive"]
+            out = contract_data["archive"]
+            if f.isatty() and isinstance(out, bytes):
+                raise RuntimeError(
+                    "won't write raw bytes to a tty! (if you want to base64"
+                    " encode the archive, you can try `-f archive` in"
+                    " conjunction with `--base64`)"
+                )
+            else:
+                f.write(out)
+        return
+
     for contract_data in compiled.values():
         for data in contract_data.values():
             if isinstance(data, (list, dict)):
                 print(json.dumps(data), file=f)
             else:
                 print(data, file=f)
 
@@ -81,17 +99,15 @@
         return
 
     parser = argparse.ArgumentParser(
         description="Pythonic Smart Contract Language for the EVM",
         formatter_class=argparse.RawTextHelpFormatter,
     )
     parser.add_argument("input_files", help="Vyper sourcecode to compile", nargs="+")
-    parser.add_argument(
-        "--version", action="version", version=f"{vyper.__version__}+commit.{vyper.__commit__}"
-    )
+    parser.add_argument("--version", action="version", version=vyper.__long_version__)
     parser.add_argument(
         "--show-gas-estimates",
         help="Show gas estimates in abi and ir output mode.",
         action="store_true",
     )
     parser.add_argument("-f", help=format_options_help, default="bytecode", dest="format")
     parser.add_argument(
@@ -105,14 +121,19 @@
         help=f"Select desired EVM version (default {evm.DEFAULT_EVM_VERSION}). "
         "note: cancun support is EXPERIMENTAL",
         choices=list(evm.EVM_VERSIONS),
         dest="evm_version",
     )
     parser.add_argument("--no-optimize", help="Do not optimize", action="store_true")
     parser.add_argument(
+        "--base64",
+        help="Base64 encode the output (only valid in conjunction with `-f archive`",
+        action="store_true",
+    )
+    parser.add_argument(
         "-O",
         "--optimize",
         help="Optimization flag (defaults to 'gas')",
         choices=["gas", "codesize", "none"],
     )
     parser.add_argument("--debug", help="Compile in debug mode", action="store_true")
     parser.add_argument(
@@ -132,26 +153,31 @@
         action="store_true",
     )
     parser.add_argument(
         "--standard-json",
         help="Switch to standard JSON mode. Use `--standard-json -h` for available options.",
         action="store_true",
     )
-    parser.add_argument("--hex-ir", action="store_true")
+    parser.add_argument(
+        "--hex-ir", help="Represent integers as hex values in the IR", action="store_true"
+    )
     parser.add_argument(
         "--path", "-p", help="Set the root path for contract imports", action="append", dest="paths"
     )
     parser.add_argument("-o", help="Set the output path", dest="output_path")
     parser.add_argument(
         "--experimental-codegen",
         help="The compiler use the new IR codegen. This is an experimental feature.",
         action="store_true",
         dest="experimental_codegen",
     )
     parser.add_argument("--enable-decimals", help="Enable decimals", action="store_true")
+    parser.add_argument(
+        "--disable-sys-path", help="Disable the use of sys.path", action="store_true"
+    )
 
     args = parser.parse_args(argv)
 
     if args.traceback_limit is not None:
         sys.tracebacklimit = args.traceback_limit
     elif VYPER_TRACEBACK_LIMIT is not None:
         sys.tracebacklimit = VYPER_TRACEBACK_LIMIT
@@ -164,14 +190,20 @@
         sys.tracebacklimit = 0
 
     if args.hex_ir:
         ir_node.AS_HEX_DEFAULT = True
 
     output_formats = tuple(uniq(args.format.split(",")))
 
+    if args.base64 and output_formats != ("archive",):
+        raise ValueError("Cannot use `--base64` except with `-f archive`")
+
+    if args.base64:
+        output_formats = ("archive_b64",)
+
     if args.no_optimize and args.optimize:
         raise ValueError("Cannot use `--no-optimize` and `--optimize` at the same time!")
 
     settings = Settings()
 
     if args.no_optimize:
         settings.optimize = OptimizationLevel.NONE
@@ -189,30 +221,38 @@
 
     if args.enable_decimals:
         settings.enable_decimals = args.enable_decimals
 
     if args.verbose:
         print(f"cli specified: `{settings}`", file=sys.stderr)
 
+    include_sys_path = not args.disable_sys_path
+
     compiled = compile_files(
         args.input_files,
         output_formats,
         args.paths,
+        include_sys_path,
         args.show_gas_estimates,
         settings,
         args.storage_layout,
         args.no_bytecode_metadata,
     )
 
+    mode = "w"
+    if output_formats == ("archive",):
+        mode = "wb"
+
     if args.output_path:
-        with open(args.output_path, "w") as f:
+        with open(args.output_path, mode) as f:
             _cli_helper(f, output_formats, compiled)
     else:
-        f = sys.stdout
-        _cli_helper(f, output_formats, compiled)
+        # https://stackoverflow.com/a/54073813
+        with os.fdopen(sys.stdout.fileno(), mode, closefd=False) as f:
+            _cli_helper(f, output_formats, compiled)
 
 
 def uniq(seq: Iterable[T]) -> Iterator[T]:
     """
     Yield unique items in ``seq`` in order.
     """
     seen: Set[T] = set()
@@ -226,24 +266,26 @@
 
 
 def exc_handler(contract_path: ContractPath, exception: Exception) -> None:
     print(f"Error compiling: {contract_path}")
     raise exception
 
 
-def get_search_paths(paths: list[str] = None) -> list[Path]:
+def get_search_paths(paths: list[str] = None, include_sys_path=True) -> list[Path]:
     # given `paths` input, get the full search path, including
     # the system search path.
     paths = paths or []
 
     # lowest precedence search path is always sys path
     # note python sys path uses opposite resolution order from us
     # (first in list is highest precedence; we give highest precedence
     # to the last in the list)
-    search_paths = [Path(p) for p in reversed(sys.path)]
+    search_paths = []
+    if include_sys_path:
+        search_paths = [Path(p) for p in reversed(sys.path)]
 
     if Path(".") not in search_paths:
         search_paths.append(Path("."))
 
     for p in paths:
         path = Path(p).resolve(strict=True)
         search_paths.append(path)
@@ -251,51 +293,74 @@
     return search_paths
 
 
 def compile_files(
     input_files: list[str],
     output_formats: OutputFormats,
     paths: list[str] = None,
+    include_sys_path: bool = True,
     show_gas_estimates: bool = False,
     settings: Optional[Settings] = None,
     storage_layout_paths: list[str] = None,
     no_bytecode_metadata: bool = False,
 ) -> dict:
-    search_paths = get_search_paths(paths)
+    search_paths = get_search_paths(paths, include_sys_path)
     input_bundle = FilesystemInputBundle(search_paths)
 
     show_version = False
     if "combined_json" in output_formats:
         if len(output_formats) > 1:
             raise ValueError("If using combined_json it must be the only output format requested")
         output_formats = combined_json_outputs
         show_version = True
 
+    # formats which can only be requested as a single output format
+    for c in ("solc_json", "archive"):
+        if c in output_formats and len(output_formats) > 1:
+            raise ValueError(f"If using {c} it must be the only output format requested")
+
     translate_map = {
         "abi_python": "abi",
         "json": "abi",
         "ast": "ast_dict",
         "annotated_ast": "annotated_ast_dict",
         "ir_json": "ir_dict",
     }
     final_formats = [translate_map.get(i, i) for i in output_formats]
 
     if storage_layout_paths:
         if len(storage_layout_paths) != len(input_files):
             raise ValueError(
-                "provided {len(storage_layout_paths)} storage "
-                "layouts, but {len(input_files)} source files"
+                f"provided {len(storage_layout_paths)} storage "
+                f"layouts, but {len(input_files)} source files"
             )
 
     ret: dict[Any, Any] = {}
     if show_version:
         ret["version"] = vyper.__version__
 
     for file_name in input_files:
         file_path = Path(file_name)
+
+        try:
+            # try to compile in zipfile mode if it's a zip file, falling back
+            # to regular mode if it's not.
+            # we allow this instead of requiring a different mode (like
+            # `--zip`) so that verifier pipelines do not need a different
+            # workflow for archive files and single-file contracts.
+            output = compile_from_zip(file_name, output_formats, settings, no_bytecode_metadata)
+            ret[file_path] = output
+            continue
+        except NotZipInput:
+            pass
+
+        # note compile_from_zip also reads the file contents, so this
+        # is slightly inefficient (and also maybe allows for some very
+        # rare, strange race conditions if the file changes in between
+        # the two reads).
         file = input_bundle.load_file(file_path)
         assert isinstance(file, FileInput)  # mypy hint
 
         storage_layout_override = None
         if storage_layout_paths:
             storage_file_path = storage_layout_paths.pop(0)
             with open(storage_file_path) as sfh:
```

### Comparing `vyper-0.4.0rc2/vyper/cli/vyper_ir.py` & `vyper-0.4.0rc3/vyper/cli/vyper_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/cli/vyper_json.py` & `vyper-0.4.0rc3/vyper/cli/vyper_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,20 +54,14 @@
     )
     parser.add_argument(
         "-o",
         help="Filename to save JSON output to. If the file exists it will be overwritten.",
         default=None,
         dest="output_file",
     )
-    parser.add_argument(
-        "-p",
-        help="Set a base import path. Vyper searches here if a file is not found in the JSON.",
-        default=None,
-        dest="root_folder",
-    )
     parser.add_argument("--pretty-json", help="Output JSON in pretty format.", action="store_true")
     parser.add_argument(
         "--traceback",
         help="Show python traceback on error instead of returning JSON",
         action="store_true",
     )
 
@@ -78,15 +72,15 @@
         json_path = Path(args.input_file).resolve().as_posix()
     else:
         input_json = "".join(sys.stdin.read()).strip()
         json_path = "<stdin>"
 
     exc_handler = exc_handler_raises if args.traceback else exc_handler_to_dict
     output_json = json.dumps(
-        compile_json(input_json, exc_handler, args.root_folder, json_path),
+        compile_json(input_json, exc_handler, json_path),
         indent=2 if args.pretty_json else None,
         sort_keys=True,
         default=str,
     )
 
     if args.output_file is not None:
         output_path = Path(args.output_file).resolve()
@@ -186,28 +180,28 @@
         if isinstance(value, list):
             # backwards compatibility - straight ABI with no "abi" key.
             # (should probably just reject these)
             value = {"abi": value}
 
         # some validation
         if not isinstance(value, dict):
-            raise JSONError("invalid interface (must be a dictionary):\n{json.dumps(value)}")
+            raise JSONError(f"invalid interface (must be a dictionary):\n{json.dumps(value)}")
         if "content" in value:
             if not isinstance(value["content"], str):
                 raise JSONError(f"invalid 'content' (expected string):\n{json.dumps(value)}")
         elif "abi" in value:
             if not isinstance(value["abi"], list):
                 raise JSONError(f"invalid 'abi' (expected list):\n{json.dumps(value)}")
         else:
             raise JSONError(
-                "invalid interface (must contain either 'content' or 'abi'):\n{json.dumps(value)}"
+                f"invalid interface (must contain either 'content' or 'abi'):\n{json.dumps(value)}"
             )
         if "content" in value and "abi" in value:
             raise JSONError(
-                "invalid interface (found both 'content' and 'abi'):\n{json.dumps(value)}"
+                f"invalid interface (found both 'content' and 'abi'):\n{json.dumps(value)}"
             )
 
         ret[path] = value
         seen[path.stem] = True
 
     return ret
 
@@ -246,60 +240,69 @@
 
         for output_path in output_paths:
             output_formats[output_path] = outputs
 
     return output_formats
 
 
+def get_search_paths(input_dict: dict) -> list[PurePath]:
+    ret = input_dict["settings"].get("search_paths", ".")
+    return [PurePath(p) for p in ret]
+
+
 def compile_from_input_dict(
-    input_dict: dict, exc_handler: Callable = exc_handler_raises, root_folder: Optional[str] = None
+    input_dict: dict, exc_handler: Callable = exc_handler_raises
 ) -> tuple[dict, dict]:
-    if root_folder is None:
-        root_folder = "."
-
     if input_dict["language"] != "Vyper":
         raise JSONError(f"Invalid language '{input_dict['language']}' - Only Vyper is supported.")
 
     evm_version = get_evm_version(input_dict)
 
     optimize = input_dict["settings"].get("optimize")
+    experimental_codegen = input_dict["settings"].get("experimentalCodegen", False)
     if isinstance(optimize, bool):
         # bool optimization level for backwards compatibility
         warnings.warn(
             "optimize: <bool> is deprecated! please use one of 'gas', 'codesize', 'none'.",
             stacklevel=2,
         )
         optimize = OptimizationLevel.default() if optimize else OptimizationLevel.NONE
     elif isinstance(optimize, str):
         optimize = OptimizationLevel.from_string(optimize)
     else:
         assert optimize is None
 
-    settings = Settings(evm_version=evm_version, optimize=optimize)
+    settings = Settings(
+        evm_version=evm_version, optimize=optimize, experimental_codegen=experimental_codegen
+    )
 
     no_bytecode_metadata = not input_dict["settings"].get("bytecodeMetadata", True)
 
+    integrity = input_dict.get("integrity")
+
     sources = get_inputs(input_dict)
     output_formats = get_output_formats(input_dict)
     compilation_targets = list(output_formats.keys())
+    search_paths = get_search_paths(input_dict)
 
-    input_bundle = JSONInputBundle(sources, search_paths=[Path(root_folder)])
+    input_bundle = JSONInputBundle(sources, search_paths=search_paths)
 
     res, warnings_dict = {}, {}
     warnings.simplefilter("always")
     for contract_path in compilation_targets:
         with warnings.catch_warnings(record=True) as caught_warnings:
             try:
                 # use load_file to get a unique source_id
                 file = input_bundle.load_file(contract_path)
                 assert isinstance(file, FileInput)  # mypy hint
                 data = vyper.compile_from_file_input(
                     file,
                     input_bundle=input_bundle,
                     output_formats=output_formats[contract_path],
+                    integrity_sum=integrity,
                     settings=settings,
                     no_bytecode_metadata=no_bytecode_metadata,
                 )
                 assert isinstance(data, dict)
                 data["source_id"] = file.source_id
             except Exception as exc:
                 return exc_handler(contract_path, exc, "compiler"), {}
@@ -374,29 +377,28 @@
             dict_out[key] = val
     return dict_out
 
 
 def compile_json(
     input_json: dict | str,
     exc_handler: Callable = exc_handler_raises,
-    root_folder: Optional[str] = None,
     json_path: Optional[str] = None,
 ) -> dict:
     try:
         if isinstance(input_json, str):
             try:
                 input_dict = json.loads(input_json, object_pairs_hook=_raise_on_duplicate_keys)
             except json.decoder.JSONDecodeError as exc:
                 new_exc = JSONError(str(exc), exc.lineno, exc.colno)
                 return exc_handler(json_path, new_exc, "json")
         else:
             input_dict = input_json
 
         try:
-            compiler_data, warn_data = compile_from_input_dict(input_dict, exc_handler, root_folder)
+            compiler_data, warn_data = compile_from_input_dict(input_dict, exc_handler)
             if "errors" in compiler_data:
                 return compiler_data
         except KeyError as exc:
             new_exc = JSONError(f"Input JSON missing required field: {str(exc)}")
             return exc_handler(json_path, new_exc, "json")
         except (FileNotFoundError, JSONError) as exc:
             return exc_handler(json_path, exc, "json")
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/abi_encoder.py` & `vyper-0.4.0rc3/vyper/codegen/abi_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,17 +155,17 @@
 # performance note: takes O(n^2) compilation time
 # where n is depth of data type, could be optimized but unlikely
 # that users will provide deeply nested data.
 # returns_len is a calling convention parameter; if set to true,
 # the abi_encode routine will push the output len onto the stack,
 # otherwise it will return 0 items to the stack.
 def abi_encode(dst, ir_node, context, bufsz, returns_len=False):
-    # TODO change dst to be an IRnode so it has type info to begin with.
-    # setting the typ of dst to ir_node.typ is a footgun.
+    # cast dst to the type of the input so that make_setter works
     dst = IRnode.from_list(dst, typ=ir_node.typ, location=MEMORY)
+
     abi_t = dst.typ.abi_type
     size_bound = abi_t.size_bound()
 
     assert isinstance(bufsz, int)
     if bufsz < size_bound:  # pragma: nocover
         raise CompilerPanic("buffer provided to abi_encode not large enough")
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/arithmetic.py` & `vyper-0.4.0rc3/vyper/codegen/arithmetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
     ok = [1]  # true
 
     if is_decimal_type(x.typ):
         lo, hi = typ.int_bounds
         if max(abs(lo), abs(hi)) * typ.divisor > 2**256 - 1:  # pragma: nocover
             # stub to prevent us from adding fixed point numbers we don't know
             # how to deal with
-            raise UnimplementedException("safe_mul for decimal{typ.bits}x{typ.decimals}")
+            raise UnimplementedException(f"safe_mul for decimal{typ.bits}x{typ.decimals}")
         x = ["mul", x, typ.divisor]
 
     DIV = "sdiv" if typ.is_signed else "div"
     res = IRnode.from_list([DIV, x, clamp("gt", y, 0)], typ=typ)
     with res.cache_when_complex("res") as (b1, res):
         # TODO: refactor this condition / push some things into the optimizer
         if typ.is_signed and typ.bits == 256:
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/context.py` & `vyper-0.4.0rc3/vyper/codegen/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 import contextlib
 import enum
 from dataclasses import dataclass
 from typing import Any, Optional
 
-from vyper.codegen.ir_node import Encoding
+from vyper.codegen.ir_node import Encoding, IRnode
+from vyper.compiler.settings import get_global_settings
 from vyper.evm.address_space import MEMORY, AddrSpace
 from vyper.exceptions import CompilerPanic, StateAccessViolation
 from vyper.semantics.types import VyperType
 
 
 class Constancy(enum.Enum):
     Mutable = 0
     Constant = 1
 
 
+@dataclass(frozen=True)
+class Alloca:
+    name: str
+    offset: int
+    typ: VyperType
+    size: int
+
+    def __post_init__(self):
+        assert self.typ.memory_bytes_required == self.size
+
+
 # Function variable
 @dataclass
 class VariableRecord:
     name: str
     pos: int
     typ: VyperType
     mutable: bool
     encoding: Encoding = Encoding.VYPER
     location: AddrSpace = MEMORY
     size: Optional[int] = None  # allocated size
     blockscopes: Optional[list] = None
     defined_at: Any = None
     is_internal: bool = False
+    alloca: Optional[Alloca] = None
+
+    # the following members are probably dead
     is_immutable: bool = False
     is_transient: bool = False
     data_offset: Optional[int] = None
 
     def __hash__(self):
         return hash(id(self))
 
@@ -39,14 +54,28 @@
             self.blockscopes = []
 
     def __repr__(self):
         ret = vars(self)
         ret["allocated"] = self.typ.memory_bytes_required
         return f"VariableRecord({ret})"
 
+    def as_ir_node(self):
+        ret = IRnode.from_list(
+            self.pos,
+            typ=self.typ,
+            annotation=self.name,
+            encoding=self.encoding,
+            mutable=self.mutable,
+            location=self.location,
+        )
+        ret._referenced_variables = {self}
+        if self.alloca is not None:
+            ret.passthrough_metadata["alloca"] = self.alloca
+        return ret
+
 
 # compilation context for a function
 class Context:
     def __init__(
         self,
         module_ctx,
         memory_allocator,
@@ -87,14 +116,16 @@
         # Incremented values, used for internal IDs
         self._internal_var_iter = 0
         self._scope_id_iter = 0
 
         # either the constructor, or called from the constructor
         self.is_ctor_context = is_ctor_context
 
+        self.settings = get_global_settings()
+
     def is_constant(self):
         return self.constancy is Constancy.Constant or self.in_range_expr
 
     def check_is_not_constant(self, err, expr):
         if self.is_constant():
             raise StateAccessViolation(f"Cannot {err} from {self.pp_constancy()}", expr)
 
@@ -136,18 +167,15 @@
         yield
 
         # Remove all variables that have specific scope_id attached
         released = [
             (k, v) for k, v in self.vars.items() if v.is_internal and scope_id in v.blockscopes
         ]
         for name, var in released:
-            n = var.typ.memory_bytes_required
-            assert n == var.size
-            self.memory_allocator.deallocate_memory(var.pos, n)
-            del self.vars[name]
+            self.deallocate_variable(name, var)
 
         # Remove block scopes
         self._scopes.remove(scope_id)
 
     @contextlib.contextmanager
     def block_scope(self):
         """
@@ -160,71 +188,103 @@
         self._scope_id_iter += 1
         self._scopes.add(scope_id)
         yield
 
         # Remove all variables that have specific scope_id attached
         released = [(k, v) for k, v in self.vars.items() if scope_id in v.blockscopes]
         for name, var in released:
-            n = var.typ.memory_bytes_required
-            # sanity check the type's size hasn't changed since allocation.
-            assert n == var.size
-            self.memory_allocator.deallocate_memory(var.pos, n)
-            del self.vars[name]
+            self.deallocate_variable(name, var)
 
         # Remove block scopes
         self._scopes.remove(scope_id)
 
-    def _new_variable(
-        self, name: str, typ: VyperType, var_size: int, is_internal: bool, is_mutable: bool = True
-    ) -> int:
-        var_pos = self.memory_allocator.allocate_memory(var_size)
+    def deallocate_variable(self, varname, var):
+        assert varname == var.name
+
+        # sanity check the type's size hasn't changed since allocation.
+        n = var.typ.memory_bytes_required
+        assert n == var.size
+
+        if self.settings.experimental_codegen:
+            # do not deallocate at this stage because this will break
+            # analysis in venom; venom will do its own alloc/dealloc/analysis.
+            pass
+        else:
+            self.memory_allocator.deallocate_memory(var.pos, var.size)
 
-        assert var_pos + var_size <= self.memory_allocator.size_of_mem, "function frame overrun"
+        del self.vars[var.name]
 
-        self.vars[name] = VariableRecord(
+    def _new_variable(
+        self,
+        name: str,
+        typ: VyperType,
+        is_internal: bool,
+        is_mutable: bool = True,
+        internal_function=False,
+    ) -> IRnode:
+        size = typ.memory_bytes_required
+
+        ofst = self.memory_allocator.allocate_memory(size)
+        assert ofst + size <= self.memory_allocator.size_of_mem, "function frame overrun"
+
+        pos = ofst
+        alloca = None
+        if self.settings.experimental_codegen:
+            # convert it into an abstract pointer
+            if internal_function:
+                pos = f"$palloca_{ofst}_{size}"
+            else:
+                pos = f"$alloca_{ofst}_{size}"
+            alloca = Alloca(name=name, offset=ofst, typ=typ, size=size)
+
+        var = VariableRecord(
             name=name,
-            pos=var_pos,
+            pos=pos,
             typ=typ,
-            size=var_size,
+            size=size,
             mutable=is_mutable,
             blockscopes=self._scopes.copy(),
             is_internal=is_internal,
+            alloca=alloca,
         )
-        return var_pos
+        self.vars[name] = var
+        return var.as_ir_node()
 
-    def new_variable(self, name: str, typ: VyperType, is_mutable: bool = True) -> int:
+    def new_variable(
+        self, name: str, typ: VyperType, is_mutable: bool = True, internal_function=False
+    ) -> IRnode:
         """
-        Allocate memory for a user-defined variable.
+        Allocate memory for a user-defined variable and return an IR node referencing it.
 
         Arguments
         ---------
         name : str
             Name of the variable
         typ : VyperType
             Variable type, used to determine the size of memory allocation
 
         Returns
         -------
         int
             Memory offset for the variable
         """
 
-        var_size = typ.memory_bytes_required
-        return self._new_variable(name, typ, var_size, False, is_mutable=is_mutable)
+        return self._new_variable(
+            name, typ, is_internal=False, is_mutable=is_mutable, internal_function=internal_function
+        )
 
     def fresh_varname(self, name: str) -> str:
         """
         return a unique variable name
         """
         t = self._internal_var_iter
         self._internal_var_iter += 1
         return f"{name}{t}"
 
-    # do we ever allocate immutable internal variables?
-    def new_internal_variable(self, typ: VyperType) -> int:
+    def new_internal_variable(self, typ: VyperType) -> IRnode:
         """
         Allocate memory for an internal variable.
 
         Arguments
         ---------
         typ : VyperType
             Variable type, used to determine the size of memory allocation
@@ -233,18 +293,17 @@
         -------
         int
             Memory offset for the variable
         """
         # internal variable names begin with a number sign so there is no chance for collision
         name = self.fresh_varname("#internal")
 
-        var_size = typ.memory_bytes_required
-        return self._new_variable(name, typ, var_size, True)
+        return self._new_variable(name, typ, is_internal=True)
 
-    def lookup_var(self, varname):
+    def lookup_var(self, varname) -> VariableRecord:
         return self.vars[varname]
 
     # Pretty print constancy for error messages
     def pp_constancy(self):
         if self.in_range_expr:
             return "a range expression"
         elif self.constancy == Constancy.Constant:
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/core.py` & `vyper-0.4.0rc3/vyper/codegen/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,15 +592,15 @@
 
 def _get_element_ptr_mapping(parent, key):
     assert isinstance(parent.typ, HashMapT)
     subtype = parent.typ.value_type
     key = unwrap_location(key)
 
     if parent.location not in (STORAGE, TRANSIENT):  # pragma: nocover
-        raise TypeCheckFailure("bad dereference on mapping {parent}[{key}]")
+        raise TypeCheckFailure(f"bad dereference on mapping {parent}[{key}]")
 
     return IRnode.from_list(["sha3_64", parent, key], typ=subtype, location=parent.location)
 
 
 # Take a value representing a memory or storage location, and descend down to
 # an element or member variable
 # This is analogous (but not necessarily equivalent to) getelementptr in LLVM.
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/events.py` & `vyper-0.4.0rc3/vyper/codegen/events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/codegen/expr.py` & `vyper-0.4.0rc3/vyper/codegen/expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from vyper.codegen.ir_node import IRnode
 from vyper.codegen.keccak256_helper import keccak256_helper
 from vyper.evm.address_space import MEMORY
 from vyper.evm.opcodes import version_check
 from vyper.exceptions import (
     CodegenPanic,
     CompilerPanic,
+    EvmVersionException,
     StructureException,
     TypeCheckFailure,
     TypeMismatch,
     UnimplementedException,
     tag_exceptions,
 )
 from vyper.semantics.types import (
@@ -84,15 +85,15 @@
             assert isinstance(self.ir_node, IRnode), self.ir_node
 
         self.ir_node.annotation = self.expr.get("node_source_code")
         self.ir_node.ast_source = self.expr
 
     def parse_Int(self):
         typ = self.expr._metadata["type"]
-        return IRnode.from_list(self.expr.n, typ=typ)
+        return IRnode.from_list(self.expr.value, typ=typ)
 
     def parse_Decimal(self):
         val = self.expr.value * DECIMAL_DIVISOR
 
         # sanity check that type checker did its job
         assert isinstance(val, decimal.Decimal)
         assert math.ceil(val) == math.floor(val)
@@ -128,16 +129,16 @@
     def parse_Str(self):
         bytez, bytez_length = string_to_bytes(self.expr.value)
         typ = StringT(bytez_length)
         return self._make_bytelike(typ, bytez, bytez_length)
 
     # Byte literals
     def parse_Bytes(self):
-        bytez = self.expr.s
-        bytez_length = len(self.expr.s)
+        bytez = self.expr.value
+        bytez_length = len(self.expr.value)
         typ = BytesT(bytez_length)
         return self._make_bytelike(typ, bytez, bytez_length)
 
     def _make_bytelike(self, btype, bytez, bytez_length):
         placeholder = self.context.new_internal_variable(btype)
         seq = []
         seq.append(["mstore", placeholder, bytez_length])
@@ -163,25 +164,15 @@
         return IRnode.from_list(val, typ=BoolT())
 
     # Variable names
     def parse_Name(self):
         if self.expr.id == "self":
             return IRnode.from_list(["address"], typ=AddressT())
         elif self.expr.id in self.context.vars:
-            var = self.context.vars[self.expr.id]
-            ret = IRnode.from_list(
-                var.pos,
-                typ=var.typ,
-                location=var.location,  # either 'memory' or 'calldata' storage is handled above.
-                encoding=var.encoding,
-                annotation=self.expr.id,
-                mutable=var.mutable,
-            )
-            ret._referenced_variables = {var}
-            return ret
+            return self.context.lookup_var(self.expr.id).as_ir_node()
 
         elif (varinfo := self.expr._expr_info.var_info) is not None:
             if varinfo.is_constant:
                 return Expr.parse_value_expr(varinfo.decl_node.value, self.context)
 
             assert varinfo.is_immutable, "not an immutable!"
 
@@ -282,14 +273,20 @@
                 return IRnode.from_list(["coinbase"], typ=AddressT())
             elif key == "block.number":
                 return IRnode.from_list(["number"], typ=UINT256_T)
             elif key == "block.gaslimit":
                 return IRnode.from_list(["gaslimit"], typ=UINT256_T)
             elif key == "block.basefee":
                 return IRnode.from_list(["basefee"], typ=UINT256_T)
+            elif key == "block.blobbasefee":
+                if not version_check(begin="cancun"):
+                    raise EvmVersionException(
+                        "`block.blobbasefee` is not available pre-cancun", self.expr
+                    )
+                return IRnode.from_list(["blobbasefee"], typ=UINT256_T)
             elif key == "block.prevhash":
                 return IRnode.from_list(["blockhash", ["sub", "number", 1]], typ=BYTES32_T)
             elif key == "tx.origin":
                 return IRnode.from_list(["origin"], typ=AddressT())
             elif key == "tx.gasprice":
                 return IRnode.from_list(["gasprice"], typ=UINT256_T)
             elif key == "chain.id":
@@ -344,15 +341,15 @@
 
         elif is_array_like(sub.typ):
             index = Expr.parse_value_expr(self.expr.slice, self.context)
 
         elif is_tuple_like(sub.typ):
             # should we annotate expr.slice in the frontend with the
             # folded value instead of calling reduced() here?
-            index = self.expr.slice.reduced().n
+            index = self.expr.slice.reduced().value
             # note: this check should also happen in get_element_ptr
             if not 0 <= index < len(sub.typ.member_types):
                 raise TypeCheckFailure("unreachable")
         else:
             raise TypeCheckFailure("unreachable")
 
         ir_node = get_element_ptr(sub, index)
@@ -490,15 +487,15 @@
             loop = ["repeat", i, 0, len_, right.typ.count, loop_body]
 
             ret.append(["seq", ["mstore", found_ptr, not_found], loop, ["mload", found_ptr]])
 
             return IRnode.from_list(b1.resolve(b2.resolve(ret)), typ=BoolT())
 
     @staticmethod
-    def _signed_to_unsigned_comparision_op(op):
+    def _signed_to_unsigned_comparison_op(op):
         translation_map = {"sgt": "gt", "sge": "ge", "sle": "le", "slt": "lt"}
         if op in translation_map:
             return translation_map[op]
         else:
             return op
 
     def parse_Compare(self):
@@ -550,15 +547,15 @@
                 return IRnode.from_list([op, left_keccak, right_keccak], typ=BoolT())
 
         # Compare other types.
         elif is_numeric_type(left.typ) and is_numeric_type(right.typ):
             if left.typ == right.typ and right.typ == UINT256_T:
                 # signed comparison ops work for any integer
                 # type BESIDES uint256
-                op = self._signed_to_unsigned_comparision_op(op)
+                op = self._signed_to_unsigned_comparison_op(op)
 
         elif left.typ._is_prim_word and right.typ._is_prim_word:
             if op not in ("eq", "ne"):
                 raise TypeCheckFailure("unreachable")
         else:
             # kludge to block behavior in #2638
             # TODO actually implement equality for complex types
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/external_call.py` & `vyper-0.4.0rc3/vyper/codegen/external_call.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import copy
 from dataclasses import dataclass
 
 import vyper.utils as util
 from vyper.codegen.abi_encoder import abi_encode
 from vyper.codegen.core import (
     _freshname,
+    add_ofst,
     calculate_type_for_external_return,
     check_assign,
     check_external_call,
     dummy_node_for_type,
     eval_once_check,
     get_type_for_exact_size,
     make_setter,
@@ -50,30 +52,30 @@
         buflen = args_abi_t.size_bound()
 
     buflen += 32  # padding for the method id
 
     buf_t = get_type_for_exact_size(buflen)
     buf = context.new_internal_variable(buf_t)
 
-    args_ofst = buf + 28
+    args_ofst = add_ofst(buf, 28)
     args_len = args_abi_t.size_bound() + 4
 
     abi_signature = fn_type.name + dst_tuple_t.abi_type.selector_name()
 
     # layout:
     # 32 bytes                 | args
     # 0x..00<method_id_4bytes> | args
     # the reason for the left padding is just so the alignment is easier.
     # XXX: we could align to buf (and also keep code size small) by using
     # (mstore buf (shl signature.method_id 224))
     pack_args = ["seq"]
     pack_args.append(["mstore", buf, util.method_id_int(abi_signature)])
 
     if len(args) != 0:
-        pack_args.append(abi_encode(buf + 32, args_as_tuple, context, bufsz=buflen))
+        pack_args.append(abi_encode(add_ofst(buf, 32), args_as_tuple, context, bufsz=buflen))
 
     return buf, pack_args, args_ofst, args_len
 
 
 def _unpack_returndata(buf, fn_type, call_kwargs, contract_address, context, expr):
     return_t = fn_type.return_type
 
@@ -89,21 +91,19 @@
     assert 0 < min_return_size <= max_return_size
 
     ret_ofst = buf
     ret_len = max_return_size
 
     encoding = Encoding.ABI
 
-    buf = IRnode.from_list(
-        buf,
-        typ=wrapped_return_t,
-        location=MEMORY,
-        encoding=encoding,
-        annotation=f"{expr.node_source_code} returndata buffer",
-    )
+    assert buf.location == MEMORY
+    buf = copy.copy(buf)
+    buf.typ = wrapped_return_t
+    buf.encoding = encoding
+    buf.annotation = f"{expr.node_source_code} returndata buffer"
 
     unpacker = ["seq"]
 
     # revert when returndatasize is not in bounds
     # (except when return_override is provided.)
     if not call_kwargs.skip_contract_check:
         assertion = IRnode.from_list(
@@ -113,15 +113,14 @@
         unpacker.append(assertion)
 
     assert isinstance(wrapped_return_t, TupleT)
 
     # unpack strictly
     if needs_clamp(wrapped_return_t, encoding):
         return_buf = context.new_internal_variable(wrapped_return_t)
-        return_buf = IRnode.from_list(return_buf, typ=wrapped_return_t, location=MEMORY)
 
         # note: make_setter does ABI decoding and clamps
         unpacker.append(make_setter(return_buf, buf))
     else:
         return_buf = buf
 
     if call_kwargs.default_return_value is not None:
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/function_definitions/common.py` & `vyper-0.4.0rc3/vyper/codegen/function_definitions/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/codegen/function_definitions/external_function.py` & `vyper-0.4.0rc3/vyper/codegen/function_definitions/external_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ExternalFuncIR,
     get_nonreentrant_lock,
     initialize_context,
     tag_frame_info,
 )
 from vyper.codegen.ir_node import Encoding, IRnode
 from vyper.codegen.stmt import parse_body
-from vyper.evm.address_space import CALLDATA, DATA, MEMORY
+from vyper.evm.address_space import CALLDATA, DATA
 from vyper.semantics.types import TupleT
 from vyper.semantics.types.function import ContractFunctionT
 from vyper.utils import calc_mem_gas
 
 
 # register function args with the local calling context.
 # also allocate the ones that live in memory (i.e. kwargs)
@@ -31,16 +31,15 @@
         base_args_ofst = IRnode(4, location=CALLDATA, typ=base_args_t, encoding=Encoding.ABI)
 
     for i, arg in enumerate(func_t.positional_args):
         arg_ir = get_element_ptr(base_args_ofst, i)
 
         if needs_clamp(arg.typ, Encoding.ABI):
             # allocate a memory slot for it and copy
-            p = context.new_variable(arg.name, arg.typ, is_mutable=False)
-            dst = IRnode(p, typ=arg.typ, location=MEMORY)
+            dst = context.new_variable(arg.name, arg.typ, is_mutable=False)
 
             copy_arg = make_setter(dst, arg_ir)
             copy_arg.ast_source = arg.ast_source
             ret.append(copy_arg)
         else:
             assert abi_encoding_matches_vyper(arg.typ)
             # leave it in place
@@ -90,27 +89,24 @@
         # TODO optimize make_setter by using
         # TupleT(list(arg.typ for arg in calldata_kwargs + default_kwargs))
         # (must ensure memory area is contiguous)
 
         for i, arg_meta in enumerate(calldata_kwargs):
             k = func_t.n_positional_args + i
 
-            dst = context.lookup_var(arg_meta.name).pos
-
-            lhs = IRnode(dst, location=MEMORY, typ=arg_meta.typ)
+            lhs = context.lookup_var(arg_meta.name).as_ir_node()
 
             rhs = get_element_ptr(calldata_kwargs_ofst, k, array_bounds_check=False)
 
             copy_arg = make_setter(lhs, rhs)
             copy_arg.ast_source = arg_meta.ast_source
             ret.append(copy_arg)
 
         for x in default_kwargs:
-            dst = context.lookup_var(x.name).pos
-            lhs = IRnode(dst, location=MEMORY, typ=x.typ)
+            lhs = context.lookup_var(x.name).as_ir_node()
             lhs.ast_source = x.ast_source
             kw_ast_val = func_t.default_values[x.name]  # e.g. `3` in x: int = 3
             rhs = Expr(kw_ast_val, context).ir_node
 
             copy_arg = make_setter(lhs, rhs)
             copy_arg.ast_source = x.ast_source
             ret.append(copy_arg)
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/function_definitions/internal_function.py` & `vyper-0.4.0rc3/vyper/codegen/function_definitions/internal_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     assert func_t.is_internal or func_t.is_constructor
 
     context = initialize_context(func_t, module_ctx, is_ctor_context)
 
     for arg in func_t.arguments:
         # allocate a variable for every arg, setting mutability
         # to True to allow internal function arguments to be mutable
-        context.new_variable(arg.name, arg.typ, is_mutable=True)
+        context.new_variable(arg.name, arg.typ, is_mutable=True, internal_function=True)
 
     # Get nonreentrant lock
     nonreentrant_pre, nonreentrant_post = get_nonreentrant_lock(func_t)
 
     function_entry_label = func_t._ir_info.internal_function_label(context.is_ctor_context)
     cleanup_label = func_t._ir_info.exit_sequence_label
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/ir_node.py` & `vyper-0.4.0rc3/vyper/codegen/ir_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/codegen/jumptable_utils.py` & `vyper-0.4.0rc3/vyper/codegen/jumptable_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/codegen/keccak256_helper.py` & `vyper-0.4.0rc3/vyper/codegen/keccak256_helper.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/codegen/memory_allocator.py` & `vyper-0.4.0rc3/vyper/codegen/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/codegen/module.py` & `vyper-0.4.0rc3/vyper/codegen/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/codegen/return_.py` & `vyper-0.4.0rc3/vyper/codegen/return_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/codegen/self_call.py` & `vyper-0.4.0rc3/vyper/codegen/self_call.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,17 +73,15 @@
     # if one of the arguments is a self call, the argument
     # buffer could get borked. to prevent against that,
     # write args to a temporary buffer until all the arguments
     # are fully evaluated.
     if args_as_tuple.contains_self_call:
         copy_args = ["seq"]
         # TODO deallocate me
-        tmp_args_buf = IRnode(
-            context.new_internal_variable(dst_tuple_t), typ=dst_tuple_t, location=MEMORY
-        )
+        tmp_args_buf = context.new_internal_variable(dst_tuple_t)
         copy_args.append(
             # --> args evaluate here <--
             make_setter(tmp_args_buf, args_as_tuple)
         )
 
         copy_args.append(make_setter(args_dst, tmp_args_buf))
```

### Comparing `vyper-0.4.0rc2/vyper/codegen/stmt.py` & `vyper-0.4.0rc3/vyper/codegen/stmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from vyper import ast as vy_ast
 from vyper.codegen.abi_encoder import abi_encode
 from vyper.codegen.context import Constancy, Context
 from vyper.codegen.core import (
     LOAD,
     STORE,
     IRnode,
+    add_ofst,
     clamp_le,
     get_dyn_array_count,
     get_element_ptr,
     get_type_for_exact_size,
     make_setter,
     wrap_value_for_external_return,
 )
@@ -132,22 +133,22 @@
         buf = self.context.new_internal_variable(get_type_for_exact_size(bufsz))
 
         # offset of bytes in (bytes,)
         method_id = util.method_id_int("Error(string)")
 
         # abi encode method_id + bytestring to `buf+32`, then
         # write method_id to `buf` and get out of here
-        payload_buf = buf + 32
+        payload_buf = add_ofst(buf, 32)
         bufsz -= 32  # reduce buffer by size of `method_id` slot
         encoded_length = abi_encode(payload_buf, msg_ir, self.context, bufsz, returns_len=True)
         with encoded_length.cache_when_complex("encoded_len") as (b1, encoded_length):
             revert_seq = [
                 "seq",
                 ["mstore", buf, method_id],
-                ["revert", buf + 28, ["add", 4, encoded_length]],
+                ["revert", add_ofst(buf, 28), ["add", 4, encoded_length]],
             ]
             revert_seq = b1.resolve(revert_seq)
 
         if is_raise:
             ir_node = revert_seq
         else:
             ir_node = ["if", ["iszero", test_expr], revert_seq]
```

### Comparing `vyper-0.4.0rc2/vyper/compiler/README.md` & `vyper-0.4.0rc3/vyper/compiler/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/compiler/__init__.py` & `vyper-0.4.0rc3/vyper/compiler/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from collections import OrderedDict
 from pathlib import Path
-from typing import Any, Callable, Dict, Optional, Sequence, Union
+from typing import Callable, Dict, Optional
 
-import vyper.ast as vy_ast  # break an import cycle
 import vyper.codegen.core as codegen
 import vyper.compiler.output as output
 from vyper.compiler.input_bundle import FileInput, InputBundle, PathLike
 from vyper.compiler.phases import CompilerData
-from vyper.compiler.settings import Settings, anchor_settings
-from vyper.typing import ContractPath, OutputFormats, StorageLayout
+from vyper.compiler.settings import Settings, anchor_settings, get_global_settings
+from vyper.typing import OutputFormats, StorageLayout
 
 OUTPUT_FORMATS = {
     # requires vyper_module
     "ast_dict": output.build_ast_dict,
     # requires annotated_vyper_module
     "annotated_ast_dict": output.build_annotated_ast_dict,
     "layout": output.build_layout_output,
-    # requires global_ctx
     "devdoc": output.build_devdoc,
     "userdoc": output.build_userdoc,
+    "archive": output.build_archive,
+    "archive_b64": output.build_archive_b64,
+    "integrity": output.build_integrity,
+    "solc_json": output.build_solc_json,
     # requires ir_node
     "external_interface": output.build_external_interface_output,
     "interface": output.build_interface_output,
     "bb": output.build_bb_output,
     "bb_runtime": output.build_bb_runtime_output,
     "cfg": output.build_cfg_output,
     "cfg_runtime": output.build_cfg_runtime_output,
@@ -49,14 +50,15 @@
 UNKNOWN_CONTRACT_NAME = "<unknown>"
 
 
 def compile_from_file_input(
     file_input: FileInput,
     input_bundle: InputBundle = None,
     settings: Settings = None,
+    integrity_sum: str = None,
     output_formats: Optional[OutputFormats] = None,
     storage_layout_override: Optional[StorageLayout] = None,
     no_bytecode_metadata: bool = False,
     show_gas_estimates: bool = False,
     exc_handler: Optional[Callable] = None,
 ) -> dict:
     """
@@ -91,31 +93,32 @@
         Use experimental codegen. Defaults to False
 
     Returns
     -------
     Dict
         Compiler output as `{'output key': "output data"}`
     """
-    settings = settings or Settings()
+    settings = settings or get_global_settings() or Settings()
 
     if output_formats is None:
         output_formats = ("bytecode",)
 
     # make IR output the same between runs
     codegen.reset_names()
 
     # TODO: maybe at this point we might as well just pass a `FileInput`
     # directly to `CompilerData`.
     compiler_data = CompilerData(
         file_input,
         input_bundle,
-        settings,
-        storage_layout_override,
-        show_gas_estimates,
-        no_bytecode_metadata,
+        settings=settings,
+        integrity_sum=integrity_sum,
+        storage_layout=storage_layout_override,
+        show_gas_estimates=show_gas_estimates,
+        no_bytecode_metadata=no_bytecode_metadata,
     )
 
     ret = {}
     with anchor_settings(compiler_data.settings):
         for output_format in output_formats:
             if output_format not in OUTPUT_FORMATS:
                 raise ValueError(f"Unsupported format type {repr(output_format)}")
@@ -145,12 +148,12 @@
     code. This was previously the main entry point into the compiler
     # (`compile_from_file_input()` is newer)
     """
     if isinstance(contract_path, str):
         contract_path = Path(contract_path)
     file_input = FileInput(
         source_id=source_id,
-        source_code=source_code,
+        contents=source_code,
         path=contract_path,
         resolved_path=resolved_path or contract_path,  # type: ignore
     )
     return compile_from_file_input(file_input, *args, **kwargs)
```

### Comparing `vyper-0.4.0rc2/vyper/compiler/input_bundle.py` & `vyper-0.4.0rc3/vyper/compiler/input_bundle.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 import contextlib
 import json
 import os
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass, field
 from functools import cached_property
 from pathlib import Path, PurePath
-from typing import Any, Iterator, Optional
+from typing import TYPE_CHECKING, Any, Iterator, Optional
 
 from vyper.exceptions import JSONError
 from vyper.utils import sha256sum
 
 # a type to make mypy happy
 PathLike = Path | PurePath
 
+if TYPE_CHECKING:
+    from zipfile import ZipFile
 
-@dataclass
+
+@dataclass(frozen=True)
 class CompilerInput:
     # an input to the compiler, basically an abstraction for file contents
+
     source_id: int
     path: PathLike  # the path that was asked for
 
     # resolved_path is the real path that was resolved to.
     # mainly handy for debugging at this point
     resolved_path: PathLike
+    contents: str
 
+    @cached_property
+    def sha256sum(self):
+        return sha256sum(self.contents)
 
-@dataclass
-class FileInput(CompilerInput):
-    source_code: str
 
+@dataclass(frozen=True)
+class FileInput(CompilerInput):
     @cached_property
-    def sha256sum(self):
-        return sha256sum(self.source_code)
+    def source_code(self):
+        return self.contents
 
 
-@dataclass
+@dataclass(frozen=True, unsafe_hash=True)
 class ABIInput(CompilerInput):
     # some json input, which has already been parsed into a dict or list
     # this is needed because json inputs present json interfaces as json
     # objects, not as strings. this class helps us avoid round-tripping
     # back to a string to pretend it's a file.
-    abi: Any  # something that json.load() returns
+    abi: Any = field(hash=False)  # something that json.load() returns
 
 
 def try_parse_abi(file_input: FileInput) -> CompilerInput:
     try:
         s = json.loads(file_input.source_code)
-        return ABIInput(file_input.source_id, file_input.path, file_input.resolved_path, s)
+        return ABIInput(**asdict(file_input), abi=s)
     except (ValueError, TypeError):
         return file_input
 
 
 class _NotFound(Exception):
     pass
 
@@ -181,17 +188,18 @@
 
 
 # wrap os.path.normpath, but return the same type as the input
 def _normpath(path):
     return path.__class__(os.path.normpath(path))
 
 
-# fake filesystem for JSON inputs. takes a base path, and `load_file()`
-# "reads" the file from the JSON input. Note that this input bundle type
-# never actually interacts with the filesystem -- it is guaranteed to be pure!
+# fake filesystem for "standard JSON" (aka solc-style) inputs. takes search
+# paths, and `load_file()` "reads" the file from the JSON input. Note that this
+# input bundle type never actually interacts with the filesystem -- it is
+# guaranteed to be pure!
 class JSONInputBundle(InputBundle):
     input_json: dict[PurePath, Any]
 
     def __init__(self, input_json, search_paths):
         super().__init__(search_paths)
         self.input_json = {}
         for path, item in input_json.items():
@@ -212,15 +220,46 @@
 
         source_id = super()._generate_source_id(resolved_path)
 
         if "content" in value:
             return FileInput(source_id, original_path, resolved_path, value["content"])
 
         if "abi" in value:
-            return ABIInput(source_id, original_path, resolved_path, value["abi"])
+            return ABIInput(
+                source_id, original_path, resolved_path, json.dumps(value), value["abi"]
+            )
 
         # TODO: ethPM support
         # if isinstance(contents, dict) and "contractTypes" in contents:
 
         # unreachable, based on how JSONInputBundle is constructed in
         # the codebase.
         raise JSONError(f"Unexpected type in file: '{resolved_path}'")  # pragma: nocover
+
+
+# input bundle for vyper archives. similar to JSONInputBundle, but takes
+# a zipfile as input.
+class ZipInputBundle(InputBundle):
+    def __init__(self, archive: "ZipFile"):
+        assert archive.testzip() is None
+        self.archive = archive
+
+        sp_str = archive.read("MANIFEST/searchpaths").decode("utf-8")
+        search_paths = [PurePath(p) for p in sp_str.splitlines()]
+
+        super().__init__(search_paths)
+
+    def _normalize_path(self, path: PurePath) -> PurePath:
+        return _normpath(path)
+
+    def _load_from_path(self, resolved_path: PurePath, original_path: PurePath) -> CompilerInput:
+        # zipfile.BadZipFile: File is not a zip file
+
+        try:
+            value = self.archive.read(str(resolved_path)).decode("utf-8")
+        except KeyError:
+            # zipfile literally raises KeyError if the file is not there
+            raise _NotFound(resolved_path)
+
+        source_id = super()._generate_source_id(resolved_path)
+
+        return FileInput(source_id, original_path, resolved_path, value)
```

### Comparing `vyper-0.4.0rc2/vyper/compiler/output.py` & `vyper-0.4.0rc3/vyper/compiler/output.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import base64
 import warnings
 from collections import deque
 from pathlib import PurePath
 
-from vyper.ast import ast_to_dict, parse_natspec
+from vyper.ast import ast_to_dict
 from vyper.codegen.ir_node import IRnode
+from vyper.compiler.output_bundle import SolcJSONWriter, VyperArchiveWriter
 from vyper.compiler.phases import CompilerData
 from vyper.compiler.utils import build_gas_estimates
 from vyper.evm import opcodes
+from vyper.exceptions import VyperException
 from vyper.ir import compile_ir
 from vyper.semantics.types.function import FunctionVisibility, StateMutability
 from vyper.typing import StorageLayout
+from vyper.utils import vyper_warn
 from vyper.warnings import ContractSizeLimitWarning
 
 
 def build_ast_dict(compiler_data: CompilerData) -> dict:
     ast_dict = {
         "contract_name": str(compiler_data.contract_path),
         "ast": ast_to_dict(compiler_data.vyper_module),
@@ -26,21 +30,57 @@
         "contract_name": str(compiler_data.contract_path),
         "ast": ast_to_dict(compiler_data.annotated_vyper_module),
     }
     return annotated_ast_dict
 
 
 def build_devdoc(compiler_data: CompilerData) -> dict:
-    userdoc, devdoc = parse_natspec(compiler_data.annotated_vyper_module)
-    return devdoc
+    return compiler_data.natspec.devdoc
 
 
 def build_userdoc(compiler_data: CompilerData) -> dict:
-    userdoc, devdoc = parse_natspec(compiler_data.annotated_vyper_module)
-    return userdoc
+    return compiler_data.natspec.userdoc
+
+
+def build_solc_json(compiler_data: CompilerData) -> str:
+    # request bytecode to ensure the input compiles through all the
+    # compilation passes, emit warnings if there are any issues
+    # (this allows use cases like sending a bug reproduction while
+    # still alerting the user in the common case that they didn't
+    # mean to have a bug)
+    try:
+        _ = compiler_data.bytecode
+    except VyperException as e:
+        vyper_warn(
+            f"Exceptions encountered during code generation (but producing output anyway): {e}"
+        )
+    writer = SolcJSONWriter(compiler_data)
+    writer.write()
+    return writer.output()
+
+
+def build_archive(compiler_data: CompilerData) -> bytes:
+    # ditto
+    try:
+        _ = compiler_data.bytecode
+    except VyperException as e:
+        vyper_warn(
+            f"Exceptions encountered during code generation (but producing archive anyway): {e}"
+        )
+    writer = VyperArchiveWriter(compiler_data)
+    writer.write()
+    return writer.output()
+
+
+def build_archive_b64(compiler_data: CompilerData) -> str:
+    return base64.b64encode(build_archive(compiler_data)).decode("ascii")
+
+
+def build_integrity(compiler_data: CompilerData) -> str:
+    return compiler_data.compilation_target._metadata["type"].integrity_sum
 
 
 def build_external_interface_output(compiler_data: CompilerData) -> str:
     interface = compiler_data.annotated_vyper_module._metadata["type"].interface
     stem = PurePath(compiler_data.contract_path).stem
     # capitalize words separated by '_'
     # ex: test_interface.vy -> TestInterface
```

### Comparing `vyper-0.4.0rc2/vyper/compiler/phases.py` & `vyper-0.4.0rc3/vyper/compiler/phases.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,30 @@
 import copy
 import warnings
 from functools import cached_property
 from pathlib import Path, PurePath
 from typing import Optional
 
 from vyper import ast as vy_ast
+from vyper.ast import natspec
 from vyper.codegen import module
 from vyper.codegen.ir_node import IRnode
 from vyper.compiler.input_bundle import FileInput, FilesystemInputBundle, InputBundle
-from vyper.compiler.settings import OptimizationLevel, Settings, anchor_settings
-from vyper.exceptions import StructureException
+from vyper.compiler.settings import OptimizationLevel, Settings, anchor_settings, merge_settings
 from vyper.ir import compile_ir, optimizer
 from vyper.semantics import analyze_module, set_data_positions, validate_compilation_target
 from vyper.semantics.types.function import ContractFunctionT
 from vyper.semantics.types.module import ModuleT
 from vyper.typing import StorageLayout
-from vyper.utils import ERC5202_PREFIX
+from vyper.utils import ERC5202_PREFIX, vyper_warn
 from vyper.venom import generate_assembly_experimental, generate_ir
 
 DEFAULT_CONTRACT_PATH = PurePath("VyperContract.vy")
 
 
-def _merge_one(lhs, rhs, helpstr):
-    if lhs is not None and rhs is not None and lhs != rhs:
-        raise StructureException(
-            f"compiler settings indicate {helpstr} {lhs}, " f"but source pragma indicates {rhs}."
-        )
-    return lhs if rhs is None else rhs
-
-
-# TODO: does this belong as a method under Settings?
-def _merge_settings(cli: Settings, pragma: Settings):
-    ret = Settings()
-    ret.evm_version = _merge_one(cli.evm_version, pragma.evm_version, "evm version")
-    ret.optimize = _merge_one(cli.optimize, pragma.optimize, "optimize")
-    ret.experimental_codegen = _merge_one(
-        cli.experimental_codegen, pragma.experimental_codegen, "experimental codegen"
-    )
-    ret.enable_decimals = _merge_one(cli.enable_decimals, pragma.enable_decimals, "enable-decimals")
-
-    return ret
-
-
 class CompilerData:
     """
     Object for fetching and storing compiler data for a Vyper contract.
 
     This object acts as a wrapper over the pure compiler functions, triggering
     compilation phases as needed and providing the data for use when generating
     the final compiler outputs.
@@ -73,14 +52,15 @@
     """
 
     def __init__(
         self,
         file_input: FileInput | str,
         input_bundle: InputBundle = None,
         settings: Settings = None,
+        integrity_sum: str = None,
         storage_layout: StorageLayout = None,
         show_gas_estimates: bool = False,
         no_bytecode_metadata: bool = False,
     ) -> None:
         """
         Initialization method.
 
@@ -96,27 +76,26 @@
             Show gas estimates for abi and ir output modes
         no_bytecode_metadata: bool, optional
             Do not add metadata to bytecode. Defaults to False
         """
 
         if isinstance(file_input, str):
             file_input = FileInput(
-                source_code=file_input,
+                contents=file_input,
                 source_id=-1,
                 path=DEFAULT_CONTRACT_PATH,
                 resolved_path=DEFAULT_CONTRACT_PATH,
             )
         self.file_input = file_input
         self.storage_layout_override = storage_layout
         self.show_gas_estimates = show_gas_estimates
         self.no_bytecode_metadata = no_bytecode_metadata
-        self.settings = settings or Settings()
+        self.original_settings = settings
         self.input_bundle = input_bundle or FilesystemInputBundle([Path(".")])
-
-        _ = self._generate_ast  # force settings to be calculated
+        self.expected_integrity_sum = integrity_sum
 
     @cached_property
     def source_code(self):
         return self.file_input.source_code
 
     @cached_property
     def source_id(self):
@@ -131,52 +110,88 @@
         settings, ast = vy_ast.parse_to_ast_with_settings(
             self.source_code,
             self.source_id,
             module_path=str(self.contract_path),
             resolved_path=str(self.file_input.resolved_path),
         )
 
-        self.settings = _merge_settings(self.settings, settings)
-        if self.settings.optimize is None:
-            self.settings.optimize = OptimizationLevel.default()
+        if self.original_settings:
+            og_settings = self.original_settings
+            settings = merge_settings(og_settings, settings)
+            assert self.original_settings == og_settings  # be paranoid
+        else:
+            # merge with empty Settings(), doesn't do much but it does
+            # remove the compiler version
+            settings = merge_settings(Settings(), settings)
+
+        if settings.optimize is None:
+            settings.optimize = OptimizationLevel.default()
+
+        if settings.experimental_codegen is None:
+            settings.experimental_codegen = False
+
+        return settings, ast
+
+    @cached_property
+    def settings(self):
+        settings, _ = self._generate_ast
+        return settings
 
-        if self.settings.experimental_codegen is None:
-            self.settings.experimental_codegen = False
-
-        # note self.settings.compiler_version is erased here as it is
-        # not used after pre-parsing
+    @cached_property
+    def vyper_module(self):
+        _, ast = self._generate_ast
         return ast
 
     @cached_property
-    def vyper_module(self):
-        return self._generate_ast
+    def _annotate(self) -> tuple[natspec.NatspecOutput, vy_ast.Module]:
+        module = generate_annotated_ast(self.vyper_module, self.input_bundle)
+        nspec = natspec.parse_natspec(module)
+        return nspec, module
+
+    @cached_property
+    def natspec(self) -> natspec.NatspecOutput:
+        return self._annotate[0]
 
     @cached_property
     def annotated_vyper_module(self) -> vy_ast.Module:
-        return generate_annotated_ast(self.vyper_module, self.input_bundle)
+        return self._annotate[1]
 
     @cached_property
     def compilation_target(self):
         """
         Get the annotated AST, and additionally run the global checks
         required for a compilation target.
         """
         module_t = self.annotated_vyper_module._metadata["type"]
+
+        expected = self.expected_integrity_sum
+
+        if expected is not None and module_t.integrity_sum != expected:
+            # warn for now. strict/relaxed mode was considered but it costs
+            # interface and testing complexity to add another feature flag.
+            vyper_warn(
+                f"Mismatched integrity sum! Expected {expected}"
+                f" but got {module_t.integrity_sum}."
+                " (This likely indicates a corrupted archive)"
+            )
+
         validate_compilation_target(module_t)
         return self.annotated_vyper_module
 
     @cached_property
     def storage_layout(self) -> StorageLayout:
         module_ast = self.compilation_target
         return set_data_positions(module_ast, self.storage_layout_override)
 
     @property
     def global_ctx(self) -> ModuleT:
         # ensure storage layout is computed
         _ = self.storage_layout
+        # ensure natspec is computed
+        _ = self.natspec
         return self.annotated_vyper_module._metadata["type"]
 
     @cached_property
     def _ir_output(self):
         # fetch both deployment and runtime IR
         return generate_ir_nodes(self.global_ctx, self.settings)
```

### Comparing `vyper-0.4.0rc2/vyper/compiler/utils.py` & `vyper-0.4.0rc3/vyper/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/evm/address_space.py` & `vyper-0.4.0rc3/vyper/evm/address_space.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/evm/opcodes.py` & `vyper-0.4.0rc3/vyper/evm/opcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,16 @@
     "NUMBER": (0x43, 0, 1, 2),
     "DIFFICULTY": (0x44, 0, 1, 2),
     "PREVRANDAO": (0x44, 0, 1, 2),
     "GASLIMIT": (0x45, 0, 1, 2),
     "CHAINID": (0x46, 0, 1, 2),
     "SELFBALANCE": (0x47, 0, 1, 5),
     "BASEFEE": (0x48, 0, 1, 2),
+    "BLOBHASH": (0x49, 1, 1, (None, None, None, 3)),
+    "BLOBBASEFEE": (0x4A, 0, 1, (None, None, None, 2)),
     "POP": (0x50, 1, 0, 2),
     "MLOAD": (0x51, 1, 1, 3),
     "MSTORE": (0x52, 2, 0, 3),
     "MSTORE8": (0x53, 2, 0, 3),
     "SLOAD": (0x54, 1, 1, 2100),
     "SSTORE": (0x55, 2, 0, 20000),
     "JUMP": (0x56, 1, 0, 8),
```

### Comparing `vyper-0.4.0rc2/vyper/exceptions.py` & `vyper-0.4.0rc3/vyper/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,14 +346,18 @@
         self.col_offset = col_offset
 
 
 class ParserException(Exception):
     """Contract source cannot be parsed."""
 
 
+class BadArchive(Exception):
+    """Bad archive"""
+
+
 class UnimplementedException(VyperException):
     """Some feature is known to be not implemented"""
 
 
 class FeatureException(VyperException):
     """Some feature flag is not enabled"""
```

### Comparing `vyper-0.4.0rc2/vyper/ir/README.md` & `vyper-0.4.0rc3/vyper/ir/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ir/compile_ir.py` & `vyper-0.4.0rc3/vyper/ir/compile_ir.py`

 * *Files 0% similar despite different names*

```diff
@@ -888,18 +888,19 @@
         if is_symbol(assembly[i]) and assembly[i + 1] == "JUMPDEST":
             current_symbol = assembly[i]
             if is_symbol(assembly[i + 2]) and assembly[i + 3] == "JUMPDEST":
                 # _sym_x JUMPDEST _sym_y JUMPDEST
                 # replace all instances of _sym_x with _sym_y
                 # (except for _sym_x JUMPDEST - don't want duplicate labels)
                 new_symbol = assembly[i + 2]
-                for j in range(len(assembly)):
-                    if assembly[j] == current_symbol and i != j:
-                        assembly[j] = new_symbol
-                        changed = True
+                if new_symbol != current_symbol:
+                    for j in range(len(assembly)):
+                        if assembly[j] == current_symbol and i != j:
+                            assembly[j] = new_symbol
+                            changed = True
             elif is_symbol(assembly[i + 2]) and assembly[i + 3] == "JUMP":
                 # _sym_x JUMPDEST _sym_y JUMP
                 # replace all instances of _sym_x with _sym_y
                 # (except for _sym_x JUMPDEST - don't want duplicate labels)
                 new_symbol = assembly[i + 2]
                 for j in range(len(assembly)):
                     if assembly[j] == current_symbol and i != j:
```

### Comparing `vyper-0.4.0rc2/vyper/ir/optimizer.py` & `vyper-0.4.0rc3/vyper/ir/optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/ir/s_expressions.py` & `vyper-0.4.0rc3/vyper/ir/s_expressions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/README.md` & `vyper-0.4.0rc3/vyper/semantics/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/base.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
 from dataclasses import dataclass
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, Union
 
 from vyper import ast as vy_ast
-from vyper.compiler.input_bundle import CompilerInput, FileInput
+from vyper.compiler.input_bundle import CompilerInput
 from vyper.exceptions import CompilerPanic, StructureException
 from vyper.semantics.data_locations import DataLocation
 from vyper.semantics.types.base import VyperType
 from vyper.semantics.types.primitives import SelfT
 from vyper.utils import OrderedSet, StringEnum
 
 if TYPE_CHECKING:
@@ -115,31 +115,29 @@
             )
         self.ownership = module_ownership
 
     def __hash__(self):
         return hash(id(self.module_t))
 
 
-@dataclass
+@dataclass(frozen=True)
 class ImportInfo(AnalysisResult):
     typ: Union[ModuleInfo, "InterfaceT"]
     alias: str  # the name in the namespace
     qualified_module_name: str  # for error messages
     compiler_input: CompilerInput  # to recover file info for ast export
     node: vy_ast.VyperNode
 
     def to_dict(self):
         ret = {"alias": self.alias, "qualified_module_name": self.qualified_module_name}
 
         ret["source_id"] = self.compiler_input.source_id
         ret["path"] = str(self.compiler_input.path)
         ret["resolved_path"] = str(self.compiler_input.resolved_path)
-
-        if isinstance(self.compiler_input, FileInput):
-            ret["file_sha256sum"] = self.compiler_input.sha256sum
+        ret["file_sha256sum"] = self.compiler_input.sha256sum
 
         return ret
 
 
 # analysis result of InitializesDecl
 @dataclass
 class InitializesInfo(AnalysisResult):
@@ -276,15 +274,15 @@
     attr: Optional[str] = None
 
     def __post_init__(self):
         should_match = ("typ", "location", "modifiability")
         if self.var_info is not None:
             for attr in should_match:
                 if getattr(self.var_info, attr) != getattr(self, attr):
-                    raise CompilerPanic("Bad analysis: non-matching {attr}: {self}")
+                    raise CompilerPanic(f"Bad analysis: non-matching {attr}: {self}")
 
         self._writes: OrderedSet[VarAccess] = OrderedSet()
         self._reads: OrderedSet[VarAccess] = OrderedSet()
 
     @classmethod
     def from_varinfo(cls, var_info: VarInfo, **kwargs) -> "ExprInfo":
         return cls(
```

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/common.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/constant_folding.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/constant_folding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/data_positions.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/data_positions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/getters.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/global_.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/global_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/import_graph.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/import_graph.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/levenshtein_utils.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/levenshtein_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/local.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/local.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/module.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from vyper import ast as vy_ast
 from vyper.compiler.input_bundle import (
     ABIInput,
     CompilerInput,
     FileInput,
     FilesystemInputBundle,
     InputBundle,
+    PathLike,
 )
 from vyper.evm.opcodes import version_check
 from vyper.exceptions import (
     BorrowException,
     CallViolation,
+    CompilerPanic,
     DuplicateImport,
     EvmVersionException,
     ExceptionList,
     ImmutableViolation,
     InitializerException,
     InterfaceViolation,
     InvalidLiteral,
@@ -394,15 +396,15 @@
 
     def _ast_from_file(self, file: FileInput) -> vy_ast.Module:
         # cache ast if we have seen it before.
         # this gives us the additional property of object equality on
         # two ASTs produced from the same source
         ast_of = self.input_bundle._cache._ast_of
         if file.source_id not in ast_of:
-            ast_of[file.source_id] = _parse_and_fold_ast(file)
+            ast_of[file.source_id] = _parse_ast(file)
 
         return ast_of[file.source_id]
 
     def visit_ImplementsDecl(self, node):
         type_ = type_from_annotation(node.annotation)
 
         if not isinstance(type_, InterfaceT):
@@ -866,15 +868,15 @@
             hint = "try renaming `vyper.interfaces` to `ethereum.ercs`"
 
         # copy search_paths, makes debugging a bit easier
         search_paths = self.input_bundle.search_paths.copy()  # noqa: F841
         raise ModuleNotFound(module_str, hint=hint) from err
 
 
-def _parse_and_fold_ast(file: FileInput) -> vy_ast.Module:
+def _parse_ast(file: FileInput) -> vy_ast.Module:
     module_path = file.resolved_path  # for error messages
     try:
         # try to get a relative path, to simplify the error message
         cwd = Path(".")
         if module_path.is_absolute():
             cwd = cwd.resolve()
         module_path = module_path.relative_to(cwd)
@@ -902,21 +904,25 @@
     return PurePath(f"{base_path}{module_str.replace('.','/')}/")
 
 
 # can add more, e.g. "vyper.builtins.interfaces", etc.
 BUILTIN_PREFIXES = ["ethereum.ercs"]
 
 
+# TODO: could move this to analysis/common.py or something
 def _is_builtin(module_str):
     return any(module_str.startswith(prefix) for prefix in BUILTIN_PREFIXES)
 
 
+_builtins_cache: dict[PathLike, tuple[CompilerInput, ModuleT]] = {}
+
+
 def _load_builtin_import(level: int, module_str: str) -> tuple[CompilerInput, InterfaceT]:
-    if not _is_builtin(module_str):
-        raise ModuleNotFound(module_str)
+    if not _is_builtin(module_str):  # pragma: nocover
+        raise CompilerPanic("unreachable!")
 
     builtins_path = vyper.builtins.interfaces.__path__[0]
     # hygiene: convert to relpath to avoid leaking user directory info
     # (note Path.relative_to cannot handle absolute to relative path
     # conversion, so we must use the `os` module).
     builtins_path = os.path.relpath(builtins_path)
 
@@ -929,26 +935,34 @@
     remapped_module = module_str
     if remapped_module.startswith("ethereum.ercs"):
         remapped_module = remapped_module.removeprefix("ethereum.ercs")
         remapped_module = vyper.builtins.interfaces.__package__ + remapped_module
 
     path = _import_to_path(level, remapped_module).with_suffix(".vyi")
 
+    # builtins are globally the same, so we can safely cache them
+    # (it is also *correct* to cache them, so that types defined in builtins
+    # compare correctly using pointer-equality.)
+    if path in _builtins_cache:
+        file, module_t = _builtins_cache[path]
+        return file, module_t.interface
+
     try:
         file = input_bundle.load_file(path)
         assert isinstance(file, FileInput)  # mypy hint
     except FileNotFoundError as e:
         hint = None
         components = module_str.split(".")
         # common issue for upgrading codebases from v0.3.x to v0.4.x -
         # hint: rename ERC20 to IERC20
         if components[-1].startswith("ERC"):
             module_prefix = components[-1]
             hint = f"try renaming `{module_prefix}` to `I{module_prefix}`"
         raise ModuleNotFound(module_str, hint=hint) from e
 
-    # TODO: it might be good to cache this computation
-    interface_ast = _parse_and_fold_ast(file)
+    interface_ast = _parse_ast(file)
 
     with override_global_namespace(Namespace()):
         module_t = _analyze_module_r(interface_ast, input_bundle, ImportGraph(), is_interface=True)
+
+    _builtins_cache[path] = file, module_t
     return file, module_t.interface
```

### Comparing `vyper-0.4.0rc2/vyper/semantics/analysis/utils.py` & `vyper-0.4.0rc3/vyper/semantics/analysis/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
                 # can be assigned to anything
                 if isinstance(t, VyperType):
                     ret.append(DArrayT(t, 1))
                 elif isinstance(t, type) and issubclass(t, VyperType):
                     # for typeclasses like bytestrings, use a generic type acceptor
                     ret.append(DArrayT(t.any(), 1))
                 else:
-                    raise CompilerPanic("busted type {t}", node)
+                    raise CompilerPanic(f"busted type {t}", node)
             return ret
 
         types_list = get_common_types(*node.elements)
 
         if len(types_list) > 0:
             count = len(node.elements)
             ret = []
```

### Comparing `vyper-0.4.0rc2/vyper/semantics/environment.py` & `vyper-0.4.0rc3/vyper/semantics/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     _type_members = {
         "coinbase": AddressT(),
         "difficulty": UINT256_T,
         "prevrandao": BYTES32_T,
         "number": UINT256_T,
         "gaslimit": UINT256_T,
         "basefee": UINT256_T,
+        "blobbasefee": UINT256_T,
         "prevhash": BYTES32_T,
         "timestamp": UINT256_T,
     }
 
 
 class _Chain(_EnvType):
     _id = "chain"
```

### Comparing `vyper-0.4.0rc2/vyper/semantics/namespace.py` & `vyper-0.4.0rc3/vyper/semantics/namespace.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         validate_identifier(attr)
 
         if attr in self:
             prev = super().__getitem__(attr)
             prev_decl = getattr(prev, "decl_node", None)
             msg = f"'{attr}' has already been declared"
             if prev_decl is None:
-                msg += " as a {prev}"
+                msg += f" as a {prev}"
             raise NamespaceCollision(msg, prev_decl=prev_decl)
 
 
 def get_namespace():
     """
     Get the global namespace object.
     """
```

### Comparing `vyper-0.4.0rc2/vyper/semantics/types/__init__.py` & `vyper-0.4.0rc3/vyper/semantics/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/types/base.py` & `vyper-0.4.0rc3/vyper/semantics/types/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         if location in (DataLocation.STORAGE, DataLocation.TRANSIENT):
             return self.storage_size_in_words
         if location == DataLocation.MEMORY:
             return self.memory_bytes_required
         if location == DataLocation.CODE:
             return self.memory_bytes_required
 
-        raise CompilerPanic("unreachable: invalid location {location}")  # pragma: nocover
+        raise CompilerPanic(f"unreachable: invalid location {location}")  # pragma: nocover
 
     @property
     def memory_bytes_required(self) -> int:
         # alias for API compatibility with codegen
         return self.size_in_bytes
 
     @property
```

### Comparing `vyper-0.4.0rc2/vyper/semantics/types/bytestrings.py` & `vyper-0.4.0rc3/vyper/semantics/types/bytestrings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/types/function.py` & `vyper-0.4.0rc3/vyper/semantics/types/function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/types/module.py` & `vyper-0.4.0rc3/vyper/semantics/types/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
     validate_unique_method_ids,
 )
 from vyper.semantics.data_locations import DataLocation
 from vyper.semantics.types.base import TYPE_T, VyperType, is_type_t
 from vyper.semantics.types.function import ContractFunctionT
 from vyper.semantics.types.primitives import AddressT
 from vyper.semantics.types.user import EventT, StructT, _UserType
-from vyper.utils import OrderedSet
+from vyper.utils import OrderedSet, sha256sum
 
 if TYPE_CHECKING:
-    from vyper.semantics.analysis.base import ModuleInfo
+    from vyper.semantics.analysis.base import ImportInfo, ModuleInfo
 
 
 class InterfaceT(_UserType):
     typeclass = "interface"
 
     _type_members = {"address": AddressT()}
     _is_prim_word = True
@@ -123,15 +123,15 @@
         # check for missing functions
         for name, type_ in self.functions.items():
             if not isinstance(type_, ContractFunctionT):
                 # ex. address
                 continue
 
             if not _is_function_implemented(name, type_):
-                unimplemented.append(name)
+                unimplemented.append(type_._pp_signature)
 
         if len(unimplemented) > 0:
             # TODO: improve the error message for cases where the
             # mismatch is small (like mutability, or just one argument
             # is off, etc).
             missing_str = ", ".join(sorted(unimplemented))
             raise InterfaceViolation(
@@ -408,14 +408,47 @@
             info = s._metadata["import_info"]
             module_info = info.typ
             if isinstance(module_info, InterfaceT):
                 continue
             ret[info.alias] = module_info
         return ret
 
+    @cached_property
+    def reachable_imports(self) -> list["ImportInfo"]:
+        """
+        Return (recursively) reachable imports from this module as a list in
+        depth-first (descendants-first) order.
+        """
+        ret = []
+        for s in self.import_stmts:
+            info = s._metadata["import_info"]
+
+            # NOTE: this needs to be redone if interfaces can import other interfaces
+            if not isinstance(info.typ, InterfaceT):
+                ret.extend(info.typ.typ.reachable_imports)
+
+            ret.append(info)
+
+        return ret
+
+    @cached_property
+    def integrity_sum(self) -> str:
+        acc = [sha256sum(self._module.full_source_code)]
+        for s in self.import_stmts:
+            info = s._metadata["import_info"]
+
+            if isinstance(info.typ, InterfaceT):
+                # NOTE: this needs to be redone if interfaces can import other interfaces
+                acc.append(info.compiler_input.sha256sum)
+            else:
+                assert isinstance(info.typ.typ, ModuleT)
+                acc.append(info.typ.typ.integrity_sum)
+
+        return sha256sum("".join(acc))
+
     def find_module_info(self, needle: "ModuleT") -> Optional["ModuleInfo"]:
         for s in self.imported_modules.values():
             if s.module_t == needle:
                 return s
         return None
 
     @property
```

### Comparing `vyper-0.4.0rc2/vyper/semantics/types/primitives.py` & `vyper-0.4.0rc3/vyper/semantics/types/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         super().validate_literal(node)
 
         assert isinstance(node, vy_ast.Hex)  # keep mypy happy
 
         val = node.value
 
         if node.n_bytes != self.m:
-            raise InvalidLiteral("Invalid literal for type {self}", node)
+            raise InvalidLiteral(f"Invalid literal for type {self}", node)
 
         nibbles = val[2:]  # strip leading 0x
         if nibbles not in (nibbles.lower(), nibbles.upper()):
             raise InvalidLiteral(f"Cannot mix uppercase and lowercase for {self} literal", node)
 
     def compare_type(self, other: VyperType) -> bool:
         if not super().compare_type(other):
@@ -147,17 +147,17 @@
         self, node: Union[vy_ast.UnaryOp, vy_ast.BinOp, vy_ast.AugAssign]
     ) -> None:
         if isinstance(node.op, self._invalid_ops):
             self._raise_invalid_op(node)
 
         def _get_lr():
             if isinstance(node, vy_ast.BinOp):
-                return node.left, node.right
+                return node.left.reduced(), node.right.reduced()
             elif isinstance(node, vy_ast.AugAssign):
-                return node.target, node.value
+                return node.target.reduced(), node.value.reduced()
             else:
                 raise CompilerPanic(f"Unexpected node type for numeric op: {type(node).__name__}")
 
         if isinstance(node.op, (vy_ast.LShift, vy_ast.RShift)):
             if self._bits != 256:
                 raise InvalidOperation(
                     f"Cannot perform {node.op.description} on non-int256/uint256 type!", node
```

### Comparing `vyper-0.4.0rc2/vyper/semantics/types/subscriptable.py` & `vyper-0.4.0rc3/vyper/semantics/types/subscriptable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/types/user.py` & `vyper-0.4.0rc3/vyper/semantics/types/user.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/semantics/types/utils.py` & `vyper-0.4.0rc3/vyper/semantics/types/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         # call from_annotation to produce a better error message.
         typ_.from_annotation(node)
 
     if hasattr(typ_, "module_t"):  # it's a ModuleInfo
         typ_ = typ_.module_t
 
     if not isinstance(typ_, VyperType):
-        raise CompilerPanic("Not a type: {typ_}", node)
+        raise CompilerPanic(f"Not a type: {typ_}", node)
 
     return typ_
 
 
 def get_index_value(node: vy_ast.VyperNode) -> int:
     """
     Return the literal value for a `Subscript` index.
```

### Comparing `vyper-0.4.0rc2/vyper/utils.py` & `vyper-0.4.0rc3/vyper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,20 @@
 
 
 @functools.lru_cache(maxsize=512)
 def sha256sum(s: str) -> str:
     return hashlib.sha256(s.encode("utf-8")).digest().hex()
 
 
+def get_long_version():
+    from vyper import __long_version__
+
+    return __long_version__
+
+
 # Converts four bytes to an integer
 def fourbytes_to_int(inp):
     return (inp[0] << 24) + (inp[1] << 16) + (inp[2] << 8) + inp[3]
 
 
 # Converts an integer to four bytes
 def int_to_fourbytes(n: int) -> bytes:
@@ -401,14 +407,15 @@
     MINDECIMAL = -(2**167)  # mindecimal as EVM value
     # min decimal allowed as Python value
     MIN_AST_DECIMAL = -decimal.Decimal(2**167) / DECIMAL_DIVISOR
     # max decimal allowed as Python value
     MAX_AST_DECIMAL = decimal.Decimal(2**167 - 1) / DECIMAL_DIVISOR
     MAX_UINT8 = 2**8 - 1
     MAX_UINT256 = 2**256 - 1
+    CEILING_UINT256 = 2**256
 
 
 def quantize(d: decimal.Decimal, places=MAX_DECIMAL_PLACES, rounding_mode=decimal.ROUND_DOWN):
     quantizer = decimal.Decimal(f"{1:0.{places}f}")
     return d.quantize(quantizer, rounding_mode)
 
 
@@ -573,29 +580,7 @@
     else:
         num_lines = end_offset - start_offset + 1
 
     cleanup_lines = [line.rstrip() for line in location_repr.splitlines()]
     cleanup_lines += [""] * (num_lines - len(cleanup_lines))
 
     return "\n".join(cleanup_lines)
-
-
-def ir_pass(func):
-    """
-    Decorator for IR passes. This decorator will run the pass repeatedly until
-    no more changes are made.
-    """
-
-    def wrapper(*args, **kwargs):
-        count = 0
-
-        while True:
-            changes = func(*args, **kwargs) or 0
-            if isinstance(changes, list) or isinstance(changes, set):
-                changes = len(changes)
-            count += changes
-            if changes == 0:
-                break
-
-        return count
-
-    return wrapper
```

### Comparing `vyper-0.4.0rc2/vyper/venom/README.md` & `vyper-0.4.0rc3/vyper/venom/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/venom/__init__.py` & `vyper-0.4.0rc3/vyper/venom/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,61 @@
 # maybe rename this `main.py` or `venom.py`
 # (can have an `__init__.py` which exposes the API).
 
-from typing import Any, Optional
+from typing import Optional
 
 from vyper.codegen.ir_node import IRnode
 from vyper.compiler.settings import OptimizationLevel
-from vyper.venom.analysis import DFG, calculate_cfg, calculate_liveness
-from vyper.venom.bb_optimizer import (
-    ir_pass_optimize_empty_blocks,
-    ir_pass_optimize_unused_variables,
-    ir_pass_remove_unreachable_blocks,
-)
-from vyper.venom.dominators import DominatorTree
+from vyper.venom.analysis.analysis import IRAnalysesCache
+from vyper.venom.analysis.liveness import LivenessAnalysis
+from vyper.venom.context import IRContext
 from vyper.venom.function import IRFunction
 from vyper.venom.ir_node_to_venom import ir_node_to_venom
-from vyper.venom.passes.constant_propagation import ir_pass_constant_propagation
 from vyper.venom.passes.dft import DFTPass
 from vyper.venom.passes.make_ssa import MakeSSA
-from vyper.venom.passes.normalization import NormalizationPass
+from vyper.venom.passes.mem2var import Mem2Var
+from vyper.venom.passes.remove_unused_variables import RemoveUnusedVariablesPass
+from vyper.venom.passes.sccp import SCCP
 from vyper.venom.passes.simplify_cfg import SimplifyCFGPass
 from vyper.venom.venom_to_assembly import VenomCompiler
 
 DEFAULT_OPT_LEVEL = OptimizationLevel.default()
 
 
 def generate_assembly_experimental(
-    runtime_code: IRFunction,
-    deploy_code: Optional[IRFunction] = None,
+    runtime_code: IRContext,
+    deploy_code: Optional[IRContext] = None,
     optimize: OptimizationLevel = DEFAULT_OPT_LEVEL,
 ) -> list[str]:
     # note: VenomCompiler is sensitive to the order of these!
     if deploy_code is not None:
         functions = [deploy_code, runtime_code]
     else:
         functions = [runtime_code]
 
     compiler = VenomCompiler(functions)
     return compiler.generate_evm(optimize == OptimizationLevel.NONE)
 
 
-def _run_passes(ctx: IRFunction, optimize: OptimizationLevel) -> None:
+def _run_passes(fn: IRFunction, optimize: OptimizationLevel) -> None:
     # Run passes on Venom IR
     # TODO: Add support for optimization levels
 
-    ir_pass_optimize_empty_blocks(ctx)
-    ir_pass_remove_unreachable_blocks(ctx)
+    ac = IRAnalysesCache(fn)
 
-    internals = [
-        bb
-        for bb in ctx.basic_blocks
-        if bb.label.value.startswith("internal") and len(bb.cfg_in) == 0
-    ]
+    SimplifyCFGPass(ac, fn).run_pass()
+    Mem2Var(ac, fn).run_pass()
+    MakeSSA(ac, fn).run_pass()
+    SCCP(ac, fn).run_pass()
 
-    SimplifyCFGPass().run_pass(ctx, ctx.basic_blocks[0])
-    for entry in internals:
-        SimplifyCFGPass().run_pass(ctx, entry)
+    SimplifyCFGPass(ac, fn).run_pass()
+    RemoveUnusedVariablesPass(ac, fn).run_pass()
+    DFTPass(ac, fn).run_pass()
 
-    make_ssa_pass = MakeSSA()
-    make_ssa_pass.run_pass(ctx, ctx.basic_blocks[0])
-    for entry in internals:
-        make_ssa_pass.run_pass(ctx, entry)
 
-    while True:
-        changes = 0
-
-        changes += ir_pass_optimize_empty_blocks(ctx)
-        changes += ir_pass_remove_unreachable_blocks(ctx)
-
-        calculate_liveness(ctx)
-
-        changes += ir_pass_optimize_unused_variables(ctx)
-
-        calculate_cfg(ctx)
-        calculate_liveness(ctx)
-
-        changes += DFTPass().run_pass(ctx)
-
-        calculate_cfg(ctx)
-        calculate_liveness(ctx)
-
-        if changes == 0:
-            break
-
-
-def generate_ir(ir: IRnode, optimize: OptimizationLevel) -> IRFunction:
+def generate_ir(ir: IRnode, optimize: OptimizationLevel) -> IRContext:
     # Convert "old" IR to "new" IR
     ctx = ir_node_to_venom(ir)
-    _run_passes(ctx, optimize)
+    for fn in ctx.functions.values():
+        _run_passes(fn, optimize)
 
     return ctx
```

### Comparing `vyper-0.4.0rc2/vyper/venom/analysis.py` & `vyper-0.4.0rc3/vyper/venom/passes/make_ssa.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,194 +1,172 @@
-from typing import Optional
-
-from vyper.exceptions import CompilerPanic
 from vyper.utils import OrderedSet
-from vyper.venom.basicblock import (
-    BB_TERMINATORS,
-    CFG_ALTERING_INSTRUCTIONS,
-    IRBasicBlock,
-    IRInstruction,
-    IRVariable,
-)
-from vyper.venom.function import IRFunction
-
-
-def calculate_cfg(ctx: IRFunction) -> None:
-    """
-    Calculate (cfg) inputs for each basic block.
-    """
-    for bb in ctx.basic_blocks:
-        bb.cfg_in = OrderedSet()
-        bb.cfg_out = OrderedSet()
-        bb.out_vars = OrderedSet()
-
-    for bb in ctx.basic_blocks:
-        assert len(bb.instructions) > 0, "Basic block should not be empty"
-        last_inst = bb.instructions[-1]
-        assert last_inst.opcode in BB_TERMINATORS, f"Last instruction should be a terminator {bb}"
-
-        for inst in bb.instructions:
-            if inst.opcode in CFG_ALTERING_INSTRUCTIONS:
-                ops = inst.get_label_operands()
-                for op in ops:
-                    ctx.get_basic_block(op.value).add_cfg_in(bb)
-
-    # Fill in the "out" set for each basic block
-    for bb in ctx.basic_blocks:
-        for in_bb in bb.cfg_in:
-            in_bb.add_cfg_out(bb)
-
-
-def _reset_liveness(ctx: IRFunction) -> None:
-    for bb in ctx.basic_blocks:
-        bb.out_vars = OrderedSet()
-        for inst in bb.instructions:
-            inst.liveness = OrderedSet()
+from vyper.venom.analysis.cfg import CFGAnalysis
+from vyper.venom.analysis.dominators import DominatorTreeAnalysis
+from vyper.venom.analysis.liveness import LivenessAnalysis
+from vyper.venom.basicblock import IRBasicBlock, IRInstruction, IROperand, IRVariable
+from vyper.venom.passes.base_pass import IRPass
 
 
-def _calculate_liveness(bb: IRBasicBlock) -> bool:
+class MakeSSA(IRPass):
     """
-    Compute liveness of each instruction in the basic block.
-    Returns True if liveness changed
+    This pass converts the function into Static Single Assignment (SSA) form.
     """
-    orig_liveness = bb.instructions[0].liveness.copy()
-    liveness = bb.out_vars.copy()
-    for instruction in reversed(bb.instructions):
-        ins = instruction.get_inputs()
-        outs = instruction.get_outputs()
 
-        if ins or outs:
-            # perf: only copy if changed
-            liveness = liveness.copy()
-            liveness.update(ins)
-            liveness.dropmany(outs)
+    dom: DominatorTreeAnalysis
+    defs: dict[IRVariable, OrderedSet[IRBasicBlock]]
 
-        instruction.liveness = liveness
+    def run_pass(self):
+        fn = self.function
 
-    return orig_liveness != bb.instructions[0].liveness
+        self.analyses_cache.request_analysis(CFGAnalysis)
+        self.dom = self.analyses_cache.request_analysis(DominatorTreeAnalysis)
+        self.analyses_cache.request_analysis(LivenessAnalysis)
 
+        self._add_phi_nodes()
 
-def _calculate_out_vars(bb: IRBasicBlock) -> bool:
-    """
-    Compute out_vars of basic block.
-    Returns True if out_vars changed
-    """
-    out_vars = bb.out_vars.copy()
-    for out_bb in bb.cfg_out:
-        target_vars = input_vars_from(bb, out_bb)
-        bb.out_vars = bb.out_vars.union(target_vars)
-    return out_vars != bb.out_vars
-
-
-def calculate_liveness(ctx: IRFunction) -> None:
-    _reset_liveness(ctx)
-    while True:
-        changed = False
-        for bb in ctx.basic_blocks:
-            changed |= _calculate_out_vars(bb)
-            changed |= _calculate_liveness(bb)
-
-        if not changed:
-            break
-
-
-def calculate_dup_requirements(ctx: IRFunction) -> None:
-    for bb in ctx.basic_blocks:
-        last_liveness = bb.out_vars
-        for inst in reversed(bb.instructions):
-            inst.dup_requirements = OrderedSet()
-            ops = inst.get_inputs()
-            for op in ops:
-                if op in last_liveness:
-                    inst.dup_requirements.add(op)
-            last_liveness = inst.liveness
-
-
-# calculate the input variables into self from source
-def input_vars_from(source: IRBasicBlock, target: IRBasicBlock) -> OrderedSet[IRVariable]:
-    liveness = target.instructions[0].liveness.copy()
-    assert isinstance(liveness, OrderedSet)
-
-    for inst in target.instructions:
-        if inst.opcode == "phi":
-            # we arbitrarily choose one of the arguments to be in the
-            # live variables set (dependent on how we traversed into this
-            # basic block). the argument will be replaced by the destination
-            # operand during instruction selection.
-            # for instance, `%56 = phi %label1 %12 %label2 %14`
-            # will arbitrarily choose either %12 or %14 to be in the liveness
-            # set, and then during instruction selection, after this instruction,
-            # %12 will be replaced by %56 in the liveness set
-
-            # bad path into this phi node
-            if source.label not in inst.operands:
-                raise CompilerPanic(f"unreachable: {inst} from {source.label}")
-
-            for label, var in inst.phi_operands:
-                if label == source.label:
-                    liveness.add(var)
-                else:
-                    if var in liveness:
-                        liveness.remove(var)
-
-    return liveness
-
-
-# DataFlow Graph
-# this could be refactored into its own file, but it's only used here
-# for now
-class DFG:
-    _dfg_inputs: dict[IRVariable, list[IRInstruction]]
-    _dfg_outputs: dict[IRVariable, IRInstruction]
-
-    def __init__(self):
-        self._dfg_inputs = dict()
-        self._dfg_outputs = dict()
-
-    # return uses of a given variable
-    def get_uses(self, op: IRVariable) -> list[IRInstruction]:
-        return self._dfg_inputs.get(op, [])
-
-    # the instruction which produces this variable.
-    def get_producing_instruction(self, op: IRVariable) -> Optional[IRInstruction]:
-        return self._dfg_outputs.get(op)
-
-    @classmethod
-    def build_dfg(cls, ctx: IRFunction) -> "DFG":
-        dfg = cls()
-
-        # Build DFG
-
-        # %15 = add %13 %14
-        # %16 = iszero %15
-        # dfg_outputs of %15 is (%15 = add %13 %14)
-        # dfg_inputs of %15 is all the instructions which *use* %15, ex. [(%16 = iszero %15), ...]
-        for bb in ctx.basic_blocks:
-            for inst in bb.instructions:
-                operands = inst.get_inputs()
-                res = inst.get_outputs()
+        self.var_name_counters = {var.name: 0 for var in self.defs.keys()}
+        self.var_name_stacks = {var.name: [0] for var in self.defs.keys()}
+        self._rename_vars(fn.entry)
+        self._remove_degenerate_phis(fn.entry)
 
-                for op in operands:
-                    inputs = dfg._dfg_inputs.setdefault(op, [])
-                    inputs.append(inst)
+    def _add_phi_nodes(self):
+        """
+        Add phi nodes to the function.
+        """
+        self._compute_defs()
+        work = {var: 0 for var in self.dom.dfs_walk}
+        has_already = {var: 0 for var in self.dom.dfs_walk}
+        i = 0
+
+        # Iterate over all variables
+        for var, d in self.defs.items():
+            i += 1
+            defs = list(d)
+            while len(defs) > 0:
+                bb = defs.pop()
+                for dom in self.dom.dominator_frontiers[bb]:
+                    if has_already[dom] >= i:
+                        continue
+
+                    self._place_phi(var, dom)
+                    has_already[dom] = i
+                    if work[dom] < i:
+                        work[dom] = i
+                        defs.append(dom)
+
+    def _place_phi(self, var: IRVariable, basic_block: IRBasicBlock):
+        if var not in basic_block.in_vars:
+            return
+
+        args: list[IROperand] = []
+        for bb in basic_block.cfg_in:
+            if bb == basic_block:
+                continue
+
+            args.append(bb.label)  # type: ignore
+            args.append(var)  # type: ignore
+
+        basic_block.insert_instruction(IRInstruction("phi", args, var), 0)
+
+    def _add_phi(self, var: IRVariable, basic_block: IRBasicBlock) -> bool:
+        for inst in basic_block.instructions:
+            if inst.opcode == "phi" and inst.output is not None and inst.output.name == var.name:
+                return False
+
+        args: list[IROperand] = []
+        for bb in basic_block.cfg_in:
+            if bb == basic_block:
+                continue
+
+            args.append(bb.label)
+            args.append(var)
 
-                for op in res:  # type: ignore
-                    dfg._dfg_outputs[op] = inst
+        phi = IRInstruction("phi", args, var)
+        basic_block.instructions.insert(0, phi)
 
-        return dfg
+        return True
 
-    def as_graph(self) -> str:
+    def _rename_vars(self, basic_block: IRBasicBlock):
         """
-        Generate a graphviz representation of the dfg
+        Rename variables. This follows the placement of phi nodes.
         """
-        lines = ["digraph dfg_graph {"]
-        for var, inputs in self._dfg_inputs.items():
-            for input in inputs:
-                for op in input.get_outputs():
-                    if isinstance(op, IRVariable):
-                        lines.append(f'    " {var.name} " -> " {op.name} "')
+        outs = []
 
-        lines.append("}")
-        return "\n".join(lines)
+        # Pre-action
+        for inst in basic_block.instructions:
+            new_ops: list[IROperand] = []
+            if inst.opcode != "phi":
+                for op in inst.operands:
+                    if not isinstance(op, IRVariable):
+                        new_ops.append(op)
+                        continue
 
-    def __repr__(self) -> str:
-        return self.as_graph()
+                    new_ops.append(IRVariable(op.name, version=self.var_name_stacks[op.name][-1]))
+
+                inst.operands = new_ops
+
+            if inst.output is not None:
+                v_name = inst.output.name
+                i = self.var_name_counters[v_name]
+
+                self.var_name_stacks[v_name].append(i)
+                self.var_name_counters[v_name] = i + 1
+
+                inst.output = IRVariable(v_name, version=i)
+                # note - after previous line, inst.output.name != v_name
+                outs.append(inst.output.name)
+
+        for bb in basic_block.cfg_out:
+            for inst in bb.instructions:
+                if inst.opcode != "phi":
+                    continue
+                assert inst.output is not None, "Phi instruction without output"
+                for i, op in enumerate(inst.operands):
+                    if op == basic_block.label:
+                        inst.operands[i + 1] = IRVariable(
+                            inst.output.name, version=self.var_name_stacks[inst.output.name][-1]
+                        )
+
+        for bb in self.dom.dominated[basic_block]:
+            if bb == basic_block:
+                continue
+            self._rename_vars(bb)
+
+        # Post-action
+        for op_name in outs:
+            # NOTE: each pop corresponds to an append in the pre-action above
+            self.var_name_stacks[op_name].pop()
+
+    def _remove_degenerate_phis(self, entry: IRBasicBlock):
+        for inst in entry.instructions.copy():
+            if inst.opcode != "phi":
+                continue
+
+            new_ops: list[IROperand] = []
+            for label, op in inst.phi_operands:
+                if op == inst.output:
+                    continue
+                new_ops.extend([label, op])
+            new_ops_len = len(new_ops)
+            if new_ops_len == 0:
+                entry.instructions.remove(inst)
+            elif new_ops_len == 2:
+                entry.instructions.remove(inst)
+            else:
+                inst.operands = new_ops
+
+        for bb in self.dom.dominated[entry]:
+            if bb == entry:
+                continue
+            self._remove_degenerate_phis(bb)
+
+    def _compute_defs(self):
+        """
+        Compute the definition points of variables in the function.
+        """
+        self.defs = {}
+        for bb in self.dom.dfs_walk:
+            assignments = bb.get_assignments()
+            for var in assignments:
+                if var not in self.defs:
+                    self.defs[var] = OrderedSet()
+                self.defs[var].add(bb)
```

### Comparing `vyper-0.4.0rc2/vyper/venom/basicblock.py` & `vyper-0.4.0rc3/vyper/venom/basicblock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import TYPE_CHECKING, Any, Generator, Iterator, Optional, Union
+from typing import TYPE_CHECKING, Any, Iterator, Optional, Union
 
+from vyper.codegen.ir_node import IRnode
 from vyper.utils import OrderedSet
 
 # instructions which can terminate a basic block
-BB_TERMINATORS = frozenset(["jmp", "djmp", "jnz", "ret", "return", "revert", "stop", "exit"])
+BB_TERMINATORS = frozenset(["jmp", "djmp", "jnz", "ret", "return", "stop", "exit"])
 
 VOLATILE_INSTRUCTIONS = frozenset(
     [
         "param",
-        "alloca",
         "call",
         "staticcall",
         "delegatecall",
         "invoke",
         "sload",
         "sstore",
         "iload",
@@ -186,63 +186,64 @@
         %1 = add %0, 1
     has opcode "add", operands ["%0", "1"], and return value "%1".
 
     Convention: the rightmost value is the top of the stack.
     """
 
     opcode: str
-    volatile: bool
     operands: list[IROperand]
     output: Optional[IROperand]
     # set of live variables at this instruction
     liveness: OrderedSet[IRVariable]
     dup_requirements: OrderedSet[IRVariable]
-    parent: Optional["IRBasicBlock"]
+    parent: "IRBasicBlock"
     fence_id: int
     annotation: Optional[str]
-    ast_source: Optional[int]
+    ast_source: Optional[IRnode]
     error_msg: Optional[str]
 
     def __init__(
         self,
         opcode: str,
         operands: list[IROperand] | Iterator[IROperand],
         output: Optional[IROperand] = None,
     ):
         assert isinstance(opcode, str), "opcode must be an str"
         assert isinstance(operands, list | Iterator), "operands must be a list"
         self.opcode = opcode
-        self.volatile = opcode in VOLATILE_INSTRUCTIONS
         self.operands = list(operands)  # in case we get an iterator
         self.output = output
         self.liveness = OrderedSet()
         self.dup_requirements = OrderedSet()
-        self.parent = None
         self.fence_id = -1
         self.annotation = None
         self.ast_source = None
         self.error_msg = None
 
-    def get_label_operands(self) -> list[IRLabel]:
+    @property
+    def volatile(self) -> bool:
+        return self.opcode in VOLATILE_INSTRUCTIONS
+
+    def get_label_operands(self) -> Iterator[IRLabel]:
         """
         Get all labels in instruction.
         """
-        return [op for op in self.operands if isinstance(op, IRLabel)]
+        return (op for op in self.operands if isinstance(op, IRLabel))
 
-    def get_non_label_operands(self) -> list[IROperand]:
+    def get_non_label_operands(self) -> Iterator[IROperand]:
         """
         Get input operands for instruction which are not labels
         """
-        return [op for op in self.operands if not isinstance(op, IRLabel)]
+        return (op for op in self.operands if not isinstance(op, IRLabel))
 
-    def get_inputs(self) -> list[IRVariable]:
+    def get_inputs(self) -> Iterator[IRVariable]:
         """
         Get all input operands for instruction.
         """
-        return [op for op in self.operands if isinstance(op, IRVariable)]
+        return (op for op in self.operands if isinstance(op, IRVariable))
 
     def get_outputs(self) -> list[IROperand]:
         """
         Get the output item for an instruction.
         (Currently all instructions output at most one item, but write
         it as a list to be generic for the future)
         """
@@ -264,26 +265,47 @@
         """
         replacements = {k.value: v for k, v in replacements.items()}
         for i, operand in enumerate(self.operands):
             if isinstance(operand, IRLabel) and operand.value in replacements:
                 self.operands[i] = replacements[operand.value]
 
     @property
-    def phi_operands(self) -> Generator[tuple[IRLabel, IRVariable], None, None]:
+    def phi_operands(self) -> Iterator[tuple[IRLabel, IROperand]]:
         """
         Get phi operands for instruction.
         """
         assert self.opcode == "phi", "instruction must be a phi"
         for i in range(0, len(self.operands), 2):
             label = self.operands[i]
             var = self.operands[i + 1]
             assert isinstance(label, IRLabel), "phi operand must be a label"
-            assert isinstance(var, IRVariable), "phi operand must be a variable"
+            assert isinstance(
+                var, (IRVariable, IRLiteral)
+            ), "phi operand must be a variable or literal"
             yield label, var
 
+    def remove_phi_operand(self, label: IRLabel) -> None:
+        """
+        Remove a phi operand from the instruction.
+        """
+        assert self.opcode == "phi", "instruction must be a phi"
+        for i in range(0, len(self.operands), 2):
+            if self.operands[i] == label:
+                del self.operands[i : i + 2]
+                return
+
+    def get_ast_source(self) -> Optional[IRnode]:
+        if self.ast_source:
+            return self.ast_source
+        idx = self.parent.instructions.index(self)
+        for inst in reversed(self.parent.instructions[:idx]):
+            if inst.ast_source:
+                return inst.ast_source
+        return self.parent.parent.ast_source
+
     def __repr__(self) -> str:
         s = ""
         if self.output:
             s += f"{self.output} = "
         opcode = f"{self.opcode} " if self.opcode != "store" else ""
         s += opcode
         operands = self.operands
@@ -447,14 +469,23 @@
 
     def get_assignments(self):
         """
         Get all assignments in basic block.
         """
         return [inst.output for inst in self.instructions if inst.output]
 
+    def get_uses(self) -> dict[IRVariable, OrderedSet[IRInstruction]]:
+        uses: dict[IRVariable, OrderedSet[IRInstruction]] = {}
+        for inst in self.instructions:
+            for op in inst.get_inputs():
+                if op not in uses:
+                    uses[op] = OrderedSet()
+                uses[op].add(inst)
+        return uses
+
     @property
     def is_empty(self) -> bool:
         """
         Check if the basic block is empty, i.e. it has no instructions.
         """
         return len(self.instructions) == 0
```

### Comparing `vyper-0.4.0rc2/vyper/venom/dominators.py` & `vyper-0.4.0rc3/vyper/venom/analysis/dominators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 from vyper.exceptions import CompilerPanic
 from vyper.utils import OrderedSet
+from vyper.venom.analysis.analysis import IRAnalysis
+from vyper.venom.analysis.cfg import CFGAnalysis
 from vyper.venom.basicblock import IRBasicBlock
 from vyper.venom.function import IRFunction
 
 
-class DominatorTree:
+class DominatorTreeAnalysis(IRAnalysis):
     """
     Dominator tree implementation. This class computes the dominator tree of a
     function and provides methods to query the tree. The tree is computed using
     the Lengauer-Tarjan algorithm.
     """
 
-    ctx: IRFunction
+    fn: IRFunction
     entry_block: IRBasicBlock
     dfs_order: dict[IRBasicBlock, int]
     dfs_walk: list[IRBasicBlock]
     dominators: dict[IRBasicBlock, OrderedSet[IRBasicBlock]]
     immediate_dominators: dict[IRBasicBlock, IRBasicBlock]
     dominated: dict[IRBasicBlock, OrderedSet[IRBasicBlock]]
     dominator_frontiers: dict[IRBasicBlock, OrderedSet[IRBasicBlock]]
 
-    @classmethod
-    def build_dominator_tree(cls, ctx, entry):
-        ret = DominatorTree()
-        ret.compute(ctx, entry)
-        return ret
-
-    def compute(self, ctx: IRFunction, entry: IRBasicBlock):
+    def analyze(self):
         """
         Compute the dominator tree.
         """
-        self.ctx = ctx
-        self.entry_block = entry
+        self.fn = self.function
+        self.entry_block = self.fn.entry
         self.dfs_order = {}
         self.dfs_walk = []
         self.dominators = {}
         self.immediate_dominators = {}
         self.dominated = {}
         self.dominator_frontiers = {}
 
+        self.analyses_cache.request_analysis(CFGAnalysis)
+
         self._compute_dfs(self.entry_block, OrderedSet())
         self._compute_dominators()
         self._compute_idoms()
         self._compute_df()
 
     def dominates(self, bb1, bb2):
         """
@@ -151,15 +149,15 @@
         self.dfs_order[entry] = len(self.dfs_walk)
 
     def as_graph(self) -> str:
         """
         Generate a graphviz representation of the dominator tree.
         """
         lines = ["digraph dominator_tree {"]
-        for bb in self.ctx.basic_blocks:
+        for bb in self.fn.get_basic_blocks():
             if bb == self.entry_block:
                 continue
             idom = self.immediate_dominator(bb)
             if idom is None:
                 continue
             lines.append(f'    " {idom.label} " -> " {bb.label} "')
         lines.append("}")
```

### Comparing `vyper-0.4.0rc2/vyper/venom/function.py` & `vyper-0.4.0rc3/vyper/venom/function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,214 +1,164 @@
 from typing import Iterator, Optional
 
 from vyper.codegen.ir_node import IRnode
 from vyper.utils import OrderedSet
-from vyper.venom.basicblock import (
-    CFG_ALTERING_INSTRUCTIONS,
-    IRBasicBlock,
-    IRInstruction,
-    IRLabel,
-    IROperand,
-    IRVariable,
-)
-
-GLOBAL_LABEL = IRLabel("__global")
+from vyper.venom.basicblock import CFG_ALTERING_INSTRUCTIONS, IRBasicBlock, IRLabel, IRVariable
 
 
 class IRFunction:
     """
     Function that contains basic blocks.
     """
 
     name: IRLabel  # symbol name
-    entry_points: list[IRLabel]  # entry points
+    ctx: "IRContext"  # type: ignore # noqa: F821
     args: list
-    ctor_mem_size: Optional[int]
-    immutables_len: Optional[int]
-    basic_blocks: list[IRBasicBlock]
-    data_segment: list[IRInstruction]
     last_label: int
     last_variable: int
+    _basic_block_dict: dict[str, IRBasicBlock]
 
     # Used during code generation
-    _ast_source_stack: list[int]
+    _ast_source_stack: list[IRnode]
     _error_msg_stack: list[str]
-    _bb_index: dict[str, int]
 
-    def __init__(self, name: IRLabel = None) -> None:
-        if name is None:
-            name = GLOBAL_LABEL
+    def __init__(self, name: IRLabel, ctx: "IRContext" = None) -> None:  # type: ignore # noqa: F821
+        self.ctx = ctx
         self.name = name
-        self.entry_points = []
         self.args = []
-        self.ctor_mem_size = None
-        self.immutables_len = None
-        self.basic_blocks = []
-        self.data_segment = []
-        self.last_label = 0
+        self._basic_block_dict = {}
+
         self.last_variable = 0
 
         self._ast_source_stack = []
         self._error_msg_stack = []
-        self._bb_index = {}
 
-        self.add_entry_point(name)
         self.append_basic_block(IRBasicBlock(name, self))
 
-    def add_entry_point(self, label: IRLabel) -> None:
-        """
-        Add entry point.
-        """
-        self.entry_points.append(label)
-
-    def remove_entry_point(self, label: IRLabel) -> None:
-        """
-        Remove entry point.
-        """
-        self.entry_points.remove(label)
+    @property
+    def entry(self) -> IRBasicBlock:
+        return next(self.get_basic_blocks())
 
-    def append_basic_block(self, bb: IRBasicBlock) -> IRBasicBlock:
+    def append_basic_block(self, bb: IRBasicBlock):
         """
         Append basic block to function.
         """
-        assert isinstance(bb, IRBasicBlock), f"append_basic_block takes IRBasicBlock, got '{bb}'"
-        self.basic_blocks.append(bb)
-
-        return self.basic_blocks[-1]
-
-    def _get_basicblock_index(self, label: str):
-        # perf: keep an "index" of labels to block indices to
-        # perform fast lookup.
-        # TODO: maybe better just to throw basic blocks in an ordered
-        # dict of some kind.
-        ix = self._bb_index.get(label, -1)
-        if 0 <= ix < len(self.basic_blocks) and self.basic_blocks[ix].label == label:
-            return ix
-        # do a reindex
-        self._bb_index = dict((bb.label.name, ix) for ix, bb in enumerate(self.basic_blocks))
-        # sanity check - no duplicate labels
-        assert len(self._bb_index) == len(self.basic_blocks)
-        return self._bb_index[label]
+        assert isinstance(bb, IRBasicBlock), bb
+        assert bb.label.name not in self._basic_block_dict
+        self._basic_block_dict[bb.label.name] = bb
+
+    def remove_basic_block(self, bb: IRBasicBlock):
+        assert isinstance(bb, IRBasicBlock), bb
+        del self._basic_block_dict[bb.label.name]
 
     def get_basic_block(self, label: Optional[str] = None) -> IRBasicBlock:
         """
         Get basic block by label.
         If label is None, return the last basic block.
         """
         if label is None:
-            return self.basic_blocks[-1]
-        ix = self._get_basicblock_index(label)
-        return self.basic_blocks[ix]
-
-    def get_basic_block_after(self, label: IRLabel) -> IRBasicBlock:
-        """
-        Get basic block after label.
-        """
-        ix = self._get_basicblock_index(label.value)
-        if 0 <= ix < len(self.basic_blocks) - 1:
-            return self.basic_blocks[ix + 1]
-        raise AssertionError(f"Basic block after '{label}' not found")
+            return next(reversed(self._basic_block_dict.values()))
+
+        return self._basic_block_dict[label]
+
+    def clear_basic_blocks(self):
+        self._basic_block_dict.clear()
+
+    def get_basic_blocks(self) -> Iterator[IRBasicBlock]:
+        """
+        Get an iterator over this function's basic blocks
+        """
+        return iter(self._basic_block_dict.values())
+
+    @property
+    def num_basic_blocks(self) -> int:
+        return len(self._basic_block_dict)
 
     def get_terminal_basicblocks(self) -> Iterator[IRBasicBlock]:
         """
         Get basic blocks that are terminal.
         """
-        for bb in self.basic_blocks:
+        for bb in self.get_basic_blocks():
             if bb.is_terminal:
                 yield bb
 
-    def get_basicblocks_in(self, basic_block: IRBasicBlock) -> list[IRBasicBlock]:
-        """
-        Get basic blocks that point to the given basic block
-        """
-        return [bb for bb in self.basic_blocks if basic_block.label in bb.cfg_in]
-
-    def get_next_label(self, suffix: str = "") -> IRLabel:
-        if suffix != "":
-            suffix = f"_{suffix}"
-        self.last_label += 1
-        return IRLabel(f"{self.last_label}{suffix}")
-
     def get_next_variable(self) -> IRVariable:
         self.last_variable += 1
         return IRVariable(f"%{self.last_variable}")
 
     def get_last_variable(self) -> str:
         return f"%{self.last_variable}"
 
     def remove_unreachable_blocks(self) -> int:
         self._compute_reachability()
 
         removed = []
-        new_basic_blocks = []
 
         # Remove unreachable basic blocks
-        for bb in self.basic_blocks:
+        for bb in self.get_basic_blocks():
             if not bb.is_reachable:
                 removed.append(bb)
-            else:
-                new_basic_blocks.append(bb)
-        self.basic_blocks = new_basic_blocks
+
+        for bb in removed:
+            self.remove_basic_block(bb)
 
         # Remove phi instructions that reference removed basic blocks
         for bb in removed:
             for out_bb in bb.cfg_out:
                 out_bb.remove_cfg_in(bb)
                 for inst in out_bb.instructions:
                     if inst.opcode != "phi":
                         continue
                     in_labels = inst.get_label_operands()
                     if bb.label in in_labels:
+                        inst.remove_phi_operand(bb.label)
+                    op_len = len(inst.operands)
+                    if op_len == 2:
+                        inst.opcode = "store"
+                        inst.operands = [inst.operands[1]]
+                    elif op_len == 0:
                         out_bb.remove_instruction(inst)
 
         return len(removed)
 
     def _compute_reachability(self) -> None:
         """
         Compute reachability of basic blocks.
         """
-        for bb in self.basic_blocks:
+        for bb in self.get_basic_blocks():
             bb.reachable = OrderedSet()
             bb.is_reachable = False
 
-        for entry in self.entry_points:
-            entry_bb = self.get_basic_block(entry.value)
-            self._compute_reachability_from(entry_bb)
+        self._compute_reachability_from(self.entry)
 
     def _compute_reachability_from(self, bb: IRBasicBlock) -> None:
         """
         Compute reachability of basic blocks from bb.
         """
         if bb.is_reachable:
             return
         bb.is_reachable = True
         for inst in bb.instructions:
-            if inst.opcode in CFG_ALTERING_INSTRUCTIONS or inst.opcode == "invoke":
+            if inst.opcode in CFG_ALTERING_INSTRUCTIONS:
                 for op in inst.get_label_operands():
                     out_bb = self.get_basic_block(op.value)
                     bb.reachable.add(out_bb)
                     self._compute_reachability_from(out_bb)
 
-    def append_data(self, opcode: str, args: list[IROperand]) -> None:
-        """
-        Append data
-        """
-        self.data_segment.append(IRInstruction(opcode, args))  # type: ignore
-
     @property
     def normalized(self) -> bool:
         """
         Check if function is normalized. A function is normalized if in the
         CFG, no basic block simultaneously has multiple inputs and outputs.
         That is, a basic block can be jumped to *from* multiple blocks, or it
         can jump *to* multiple blocks, but it cannot simultaneously do both.
         Having a normalized CFG makes calculation of stack layout easier when
         emitting assembly.
         """
-        for bb in self.basic_blocks:
+        for bb in self.get_basic_blocks():
             # Ignore if there are no multiple predecessors
             if len(bb.cfg_in) <= 1:
                 continue
 
             # Check if there is a branching jump at the end
             # of one of the predecessors
             for in_bb in bb.cfg_in:
@@ -226,25 +176,44 @@
     def pop_source(self):
         assert len(self._ast_source_stack) > 0, "Empty source stack"
         self._ast_source_stack.pop()
         assert len(self._error_msg_stack) > 0, "Empty error stack"
         self._error_msg_stack.pop()
 
     @property
-    def ast_source(self) -> Optional[int]:
+    def ast_source(self) -> Optional[IRnode]:
         return self._ast_source_stack[-1] if len(self._ast_source_stack) > 0 else None
 
     @property
     def error_msg(self) -> Optional[str]:
         return self._error_msg_stack[-1] if len(self._error_msg_stack) > 0 else None
 
+    def chain_basic_blocks(self) -> None:
+        """
+        Chain basic blocks together. If a basic block is not terminated, jump to the next one.
+        Otherwise, append a stop instruction. This is necessary for the IR to be valid, and is
+        done after the IR is generated.
+        """
+        bbs = list(self.get_basic_blocks())
+        for i, bb in enumerate(bbs):
+            if not bb.is_terminated:
+                if i < len(bbs) - 1:
+                    # TODO: revisit this. When contructor calls internal functions they
+                    # are linked to the last ctor block. Should separate them before this
+                    # so we don't have to handle this here
+                    if bbs[i + 1].label.value.startswith("internal"):
+                        bb.append_instruction("stop")
+                    else:
+                        bb.append_instruction("jmp", bbs[i + 1].label)
+                else:
+                    bb.append_instruction("exit")
+
     def copy(self):
         new = IRFunction(self.name)
-        new.basic_blocks = self.basic_blocks.copy()
-        new.data_segment = self.data_segment.copy()
+        new._basic_block_dict = self._basic_block_dict.copy()
         new.last_label = self.last_label
         new.last_variable = self.last_variable
         return new
 
     def as_graph(self) -> str:
         import html
 
@@ -256,27 +225,23 @@
             ret += "</table>>"
 
             return ret
             # return f"{bb.label.value}:\n" + "\n".join([f"    {inst}" for inst in bb.instructions])
 
         ret = "digraph G {\n"
 
-        for bb in self.basic_blocks:
+        for bb in self.get_basic_blocks():
             for out_bb in bb.cfg_out:
                 ret += f'    "{bb.label.value}" -> "{out_bb.label.value}"\n'
 
-        for bb in self.basic_blocks:
+        for bb in self.get_basic_blocks():
             ret += f'    "{bb.label.value}" [shape=plaintext, '
             ret += f'label={_make_label(bb)}, fontname="Courier" fontsize="8"]\n'
 
         ret += "}\n"
         return ret
 
     def __repr__(self) -> str:
         str = f"IRFunction: {self.name}\n"
-        for bb in self.basic_blocks:
+        for bb in self.get_basic_blocks():
             str += f"{bb}\n"
-        if len(self.data_segment) > 0:
-            str += "Data segment:\n"
-            for inst in self.data_segment:
-                str += f"{inst}\n"
         return str.strip()
```

### Comparing `vyper-0.4.0rc2/vyper/venom/ir_node_to_venom.py` & `vyper-0.4.0rc3/vyper/venom/ir_node_to_venom.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     IRBasicBlock,
     IRInstruction,
     IRLabel,
     IRLiteral,
     IROperand,
     IRVariable,
 )
+from vyper.venom.context import IRContext
 from vyper.venom.function import IRFunction
 
 # Instructions that are mapped to their inverse
 INVERSE_MAPPED_IR_INSTRUCTIONS = {"ne": "eq", "le": "gt", "sle": "sgt", "ge": "lt", "sge": "slt"}
 
 # Instructions that have a direct EVM opcode equivalent and can
 # be passed through to the EVM assembly without special handling
@@ -44,414 +45,402 @@
         "smod",
         "exp",
         "sha3",
         "sha3_64",
         "signextend",
         "chainid",
         "basefee",
+        "blobhash",
+        "blobbasefee",
         "timestamp",
         "blockhash",
         "caller",
         "selfbalance",
         "calldatasize",
         "callvalue",
         "address",
         "origin",
         "codesize",
         "gas",
         "gasprice",
         "gaslimit",
         "returndatasize",
+        "mload",
         "iload",
+        "istore",
         "sload",
+        "sstore",
         "tload",
+        "tstore",
         "coinbase",
         "number",
         "prevrandao",
         "difficulty",
         "iszero",
         "not",
         "calldataload",
         "extcodesize",
         "extcodehash",
         "balance",
         "msize",
-        "basefee",
         "invalid",
         "stop",
         "selfdestruct",
         "assert",
         "assert_unreachable",
         "exit",
         "calldatacopy",
         "mcopy",
         "extcodecopy",
         "codecopy",
         "returndatacopy",
         "revert",
-        "istore",
-        "sstore",
-        "tstore",
         "create",
         "create2",
         "addmod",
         "mulmod",
         "call",
         "delegatecall",
         "staticcall",
     ]
 )
 
 NOOP_INSTRUCTIONS = frozenset(["pass", "cleanup_repeat", "var_list", "unique_symbol"])
 
 SymbolTable = dict[str, Optional[IROperand]]
+_global_symbols: SymbolTable = {}
+MAIN_ENTRY_LABEL_NAME = "__main_entry"
 
 
 # convert IRnode directly to venom
-def ir_node_to_venom(ir: IRnode) -> IRFunction:
-    ctx = IRFunction()
-    _convert_ir_bb(ctx, ir, {})
-
-    # Patch up basic blocks. Connect unterminated blocks to the next with
-    # a jump. terminate final basic block with STOP.
-    for i, bb in enumerate(ctx.basic_blocks):
-        if not bb.is_terminated:
-            if len(ctx.basic_blocks) - 1 > i:
-                # TODO: revisit this. When contructor calls internal functions they
-                # are linked to the last ctor block. Should separate them before this
-                # so we don't have to handle this here
-                if ctx.basic_blocks[i + 1].label.value.startswith("internal"):
-                    bb.append_instruction("stop")
-                else:
-                    bb.append_instruction("jmp", ctx.basic_blocks[i + 1].label)
-            else:
-                bb.append_instruction("exit")
+def ir_node_to_venom(ir: IRnode) -> IRContext:
+    global _global_symbols
+    _global_symbols = {}
+
+    ctx = IRContext()
+    fn = ctx.create_function(MAIN_ENTRY_LABEL_NAME)
+
+    _convert_ir_bb(fn, ir, {})
+
+    ctx.chain_basic_blocks()
 
     return ctx
 
 
-def _append_jmp(ctx: IRFunction, label: IRLabel) -> None:
-    bb = ctx.get_basic_block()
+def _append_jmp(fn: IRFunction, label: IRLabel) -> None:
+    bb = fn.get_basic_block()
     if bb.is_terminated:
-        bb = IRBasicBlock(ctx.get_next_label("jmp_target"), ctx)
-        ctx.append_basic_block(bb)
+        bb = IRBasicBlock(fn.ctx.get_next_label("jmp_target"), fn)
+        fn.append_basic_block(bb)
 
     bb.append_instruction("jmp", label)
 
 
-def _new_block(ctx: IRFunction) -> IRBasicBlock:
-    bb = IRBasicBlock(ctx.get_next_label(), ctx)
-    bb = ctx.append_basic_block(bb)
-    return bb
+def _new_block(fn: IRFunction) -> None:
+    bb = IRBasicBlock(fn.ctx.get_next_label(), fn)
+    fn.append_basic_block(bb)
 
 
-def _append_return_args(ctx: IRFunction, ofst: int = 0, size: int = 0):
-    bb = ctx.get_basic_block()
+def _append_return_args(fn: IRFunction, ofst: int = 0, size: int = 0):
+    bb = fn.get_basic_block()
     if bb.is_terminated:
-        bb = IRBasicBlock(ctx.get_next_label("exit_to"), ctx)
-        ctx.append_basic_block(bb)
+        bb = IRBasicBlock(fn.ctx.get_next_label("exit_to"), fn)
+        fn.append_basic_block(bb)
     ret_ofst = IRVariable("ret_ofst")
     ret_size = IRVariable("ret_size")
     bb.append_instruction("store", ofst, ret=ret_ofst)
     bb.append_instruction("store", size, ret=ret_size)
 
 
-def _handle_self_call(ctx: IRFunction, ir: IRnode, symbols: SymbolTable) -> Optional[IRVariable]:
+def _handle_self_call(fn: IRFunction, ir: IRnode, symbols: SymbolTable) -> Optional[IRVariable]:
     setup_ir = ir.args[1]
     goto_ir = [ir for ir in ir.args if ir.value == "goto"][0]
     target_label = goto_ir.args[0].value  # goto
     return_buf_ir = goto_ir.args[1]  # return buffer
     ret_args: list[IROperand] = [IRLabel(target_label)]  # type: ignore
 
     if setup_ir != goto_ir:
-        _convert_ir_bb(ctx, setup_ir, symbols)
+        _convert_ir_bb(fn, setup_ir, symbols)
 
-    return_buf = _convert_ir_bb(ctx, return_buf_ir, symbols)
+    return_buf = _convert_ir_bb(fn, return_buf_ir, symbols)
 
-    bb = ctx.get_basic_block()
+    bb = fn.get_basic_block()
     if len(goto_ir.args) > 2:
         ret_args.append(return_buf)  # type: ignore
 
     bb.append_invoke_instruction(ret_args, returns=False)  # type: ignore
 
     return return_buf
 
 
 def _handle_internal_func(
-    ctx: IRFunction, ir: IRnode, does_return_data: bool, symbols: SymbolTable
-):
-    bb = IRBasicBlock(IRLabel(ir.args[0].args[0].value, True), ctx)  # type: ignore
-    bb = ctx.append_basic_block(bb)
+    fn: IRFunction, ir: IRnode, does_return_data: bool, symbols: SymbolTable
+) -> IRFunction:
+    fn = fn.ctx.create_function(ir.args[0].args[0].value)
+    bb = fn.get_basic_block()
 
     # return buffer
     if does_return_data:
         symbols["return_buffer"] = bb.append_instruction("param")
         bb.instructions[-1].annotation = "return_buffer"
 
     # return address
     symbols["return_pc"] = bb.append_instruction("param")
     bb.instructions[-1].annotation = "return_pc"
 
-    _convert_ir_bb(ctx, ir.args[0].args[2], symbols)
+    _convert_ir_bb(fn, ir.args[0].args[2], symbols)
+
+    return fn
 
 
 def _convert_ir_simple_node(
-    ctx: IRFunction, ir: IRnode, symbols: SymbolTable
+    fn: IRFunction, ir: IRnode, symbols: SymbolTable
 ) -> Optional[IRVariable]:
     # execute in order
-    args = _convert_ir_bb_list(ctx, ir.args, symbols)
+    args = _convert_ir_bb_list(fn, ir.args, symbols)
     # reverse output variables for stack
     args.reverse()
-    return ctx.get_basic_block().append_instruction(ir.value, *args)  # type: ignore
+    return fn.get_basic_block().append_instruction(ir.value, *args)  # type: ignore
 
 
 _break_target: Optional[IRBasicBlock] = None
 _continue_target: Optional[IRBasicBlock] = None
 
 
-def _convert_ir_bb_list(ctx, ir, symbols):
+def _convert_ir_bb_list(fn, ir, symbols):
     ret = []
     for ir_node in ir:
-        venom = _convert_ir_bb(ctx, ir_node, symbols)
+        venom = _convert_ir_bb(fn, ir_node, symbols)
         ret.append(venom)
     return ret
 
 
 current_func = None
 var_list: list[str] = []
 
 
 def pop_source_on_return(func):
     @functools.wraps(func)
     def pop_source(*args, **kwargs):
-        ctx = args[0]
+        fn = args[0]
         ret = func(*args, **kwargs)
-        ctx.pop_source()
+        fn.pop_source()
         return ret
 
     return pop_source
 
 
 @pop_source_on_return
-def _convert_ir_bb(ctx, ir, symbols):
+def _convert_ir_bb(fn, ir, symbols):
     assert isinstance(ir, IRnode), ir
-    global _break_target, _continue_target, current_func, var_list
+    global _break_target, _continue_target, current_func, var_list, _global_symbols
 
-    ctx.push_source(ir)
+    ctx = fn.ctx
+    fn.push_source(ir)
 
     if ir.value in INVERSE_MAPPED_IR_INSTRUCTIONS:
         org_value = ir.value
         ir.value = INVERSE_MAPPED_IR_INSTRUCTIONS[ir.value]
-        new_var = _convert_ir_simple_node(ctx, ir, symbols)
+        new_var = _convert_ir_simple_node(fn, ir, symbols)
         ir.value = org_value
-        return ctx.get_basic_block().append_instruction("iszero", new_var)
+        return fn.get_basic_block().append_instruction("iszero", new_var)
     elif ir.value in PASS_THROUGH_INSTRUCTIONS:
-        return _convert_ir_simple_node(ctx, ir, symbols)
+        return _convert_ir_simple_node(fn, ir, symbols)
     elif ir.value == "return":
-        ctx.get_basic_block().append_instruction(
+        fn.get_basic_block().append_instruction(
             "return", IRVariable("ret_size"), IRVariable("ret_ofst")
         )
     elif ir.value == "deploy":
         ctx.ctor_mem_size = ir.args[0].value
         ctx.immutables_len = ir.args[2].value
         return None
     elif ir.value == "seq":
         if len(ir.args) == 0:
             return None
         if ir.is_self_call:
-            return _handle_self_call(ctx, ir, symbols)
+            return _handle_self_call(fn, ir, symbols)
         elif ir.args[0].value == "label":
             current_func = ir.args[0].args[0].value
             is_external = current_func.startswith("external")
             is_internal = current_func.startswith("internal")
             if is_internal or len(re.findall(r"external.*__init__\(.*_deploy", current_func)) > 0:
                 # Internal definition
                 var_list = ir.args[0].args[1]
                 does_return_data = IRnode.from_list(["return_buffer"]) in var_list.args
+                _global_symbols = {}
                 symbols = {}
-                _handle_internal_func(ctx, ir, does_return_data, symbols)
+                new_fn = _handle_internal_func(fn, ir, does_return_data, symbols)
                 for ir_node in ir.args[1:]:
-                    ret = _convert_ir_bb(ctx, ir_node, symbols)
+                    ret = _convert_ir_bb(new_fn, ir_node, symbols)
 
                 return ret
             elif is_external:
-                ret = _convert_ir_bb(ctx, ir.args[0], symbols)
-                _append_return_args(ctx)
+                _global_symbols = {}
+                ret = _convert_ir_bb(fn, ir.args[0], symbols)
+                _append_return_args(fn)
         else:
-            bb = ctx.get_basic_block()
+            bb = fn.get_basic_block()
             if bb.is_terminated:
-                bb = IRBasicBlock(ctx.get_next_label("seq"), ctx)
-                ctx.append_basic_block(bb)
-            ret = _convert_ir_bb(ctx, ir.args[0], symbols)
+                bb = IRBasicBlock(ctx.get_next_label("seq"), fn)
+                fn.append_basic_block(bb)
+            ret = _convert_ir_bb(fn, ir.args[0], symbols)
 
         for ir_node in ir.args[1:]:
-            ret = _convert_ir_bb(ctx, ir_node, symbols)
+            ret = _convert_ir_bb(fn, ir_node, symbols)
 
         return ret
     elif ir.value == "if":
         cond = ir.args[0]
 
         # convert the condition
-        cont_ret = _convert_ir_bb(ctx, cond, symbols)
-        cond_block = ctx.get_basic_block()
+        cont_ret = _convert_ir_bb(fn, cond, symbols)
+        cond_block = fn.get_basic_block()
 
+        saved_global_symbols = _global_symbols.copy()
+
+        then_block = IRBasicBlock(ctx.get_next_label("then"), fn)
+        else_block = IRBasicBlock(ctx.get_next_label("else"), fn)
+
+        # convert "then"
         cond_symbols = symbols.copy()
+        fn.append_basic_block(then_block)
+        then_ret_val = _convert_ir_bb(fn, ir.args[1], cond_symbols)
+        if isinstance(then_ret_val, IRLiteral):
+            then_ret_val = fn.get_basic_block().append_instruction("store", then_ret_val)
 
-        else_block = IRBasicBlock(ctx.get_next_label("else"), ctx)
-        ctx.append_basic_block(else_block)
+        then_block_finish = fn.get_basic_block()
 
         # convert "else"
+        cond_symbols = symbols.copy()
+        _global_symbols = saved_global_symbols.copy()
+        fn.append_basic_block(else_block)
         else_ret_val = None
         if len(ir.args) == 3:
-            else_ret_val = _convert_ir_bb(ctx, ir.args[2], cond_symbols)
+            else_ret_val = _convert_ir_bb(fn, ir.args[2], cond_symbols)
             if isinstance(else_ret_val, IRLiteral):
                 assert isinstance(else_ret_val.value, int)  # help mypy
-                else_ret_val = ctx.get_basic_block().append_instruction("store", else_ret_val)
-
-        else_block_finish = ctx.get_basic_block()
-
-        # convert "then"
-        cond_symbols = symbols.copy()
-
-        then_block = IRBasicBlock(ctx.get_next_label("then"), ctx)
-        ctx.append_basic_block(then_block)
+                else_ret_val = fn.get_basic_block().append_instruction("store", else_ret_val)
 
-        then_ret_val = _convert_ir_bb(ctx, ir.args[1], cond_symbols)
-        if isinstance(then_ret_val, IRLiteral):
-            then_ret_val = ctx.get_basic_block().append_instruction("store", then_ret_val)
+        else_block_finish = fn.get_basic_block()
 
+        # finish the condition block
         cond_block.append_instruction("jnz", cont_ret, then_block.label, else_block.label)
 
-        then_block_finish = ctx.get_basic_block()
-
         # exit bb
-        exit_bb = IRBasicBlock(ctx.get_next_label("if_exit"), ctx)
-        exit_bb = ctx.append_basic_block(exit_bb)
+        exit_bb = IRBasicBlock(ctx.get_next_label("if_exit"), fn)
+        fn.append_basic_block(exit_bb)
 
-        if_ret = ctx.get_next_variable()
+        if_ret = fn.get_next_variable()
         if then_ret_val is not None and else_ret_val is not None:
             then_block_finish.append_instruction("store", then_ret_val, ret=if_ret)
             else_block_finish.append_instruction("store", else_ret_val, ret=if_ret)
 
         if not else_block_finish.is_terminated:
             else_block_finish.append_instruction("jmp", exit_bb.label)
 
         if not then_block_finish.is_terminated:
             then_block_finish.append_instruction("jmp", exit_bb.label)
 
+        _global_symbols = saved_global_symbols
+
         return if_ret
 
     elif ir.value == "with":
-        ret = _convert_ir_bb(ctx, ir.args[1], symbols)  # initialization
-
-        ret = ctx.get_basic_block().append_instruction("store", ret)
+        ret = _convert_ir_bb(fn, ir.args[1], symbols)  # initialization
 
-        # Handle with nesting with same symbol
-        with_symbols = symbols.copy()
+        ret = fn.get_basic_block().append_instruction("store", ret)
 
         sym = ir.args[0]
+        with_symbols = symbols.copy()
         with_symbols[sym.value] = ret
 
-        return _convert_ir_bb(ctx, ir.args[2], with_symbols)  # body
+        return _convert_ir_bb(fn, ir.args[2], with_symbols)  # body
+
     elif ir.value == "goto":
-        _append_jmp(ctx, IRLabel(ir.args[0].value))
+        _append_jmp(fn, IRLabel(ir.args[0].value))
     elif ir.value == "djump":
-        args = [_convert_ir_bb(ctx, ir.args[0], symbols)]
+        args = [_convert_ir_bb(fn, ir.args[0], symbols)]
         for target in ir.args[1:]:
             args.append(IRLabel(target.value))
-        ctx.get_basic_block().append_instruction("djmp", *args)
-        _new_block(ctx)
+        fn.get_basic_block().append_instruction("djmp", *args)
+        _new_block(fn)
     elif ir.value == "set":
         sym = ir.args[0]
-        arg_1 = _convert_ir_bb(ctx, ir.args[1], symbols)
-        ctx.get_basic_block().append_instruction("store", arg_1, ret=symbols[sym.value])
+        arg_1 = _convert_ir_bb(fn, ir.args[1], symbols)
+        fn.get_basic_block().append_instruction("store", arg_1, ret=symbols[sym.value])
     elif ir.value == "symbol":
         return IRLabel(ir.args[0].value, True)
     elif ir.value == "data":
         label = IRLabel(ir.args[0].value)
         ctx.append_data("dbname", [label])
         for c in ir.args[1:]:
             if isinstance(c, int):
                 assert 0 <= c <= 255, "data with invalid size"
                 ctx.append_data("db", [c])  # type: ignore
             elif isinstance(c.value, bytes):
                 ctx.append_data("db", [c.value])  # type: ignore
             elif isinstance(c, IRnode):
-                data = _convert_ir_bb(ctx, c, symbols)
+                data = _convert_ir_bb(fn, c, symbols)
                 ctx.append_data("db", [data])  # type: ignore
     elif ir.value == "label":
         label = IRLabel(ir.args[0].value, True)
-        bb = ctx.get_basic_block()
+        bb = fn.get_basic_block()
         if not bb.is_terminated:
             bb.append_instruction("jmp", label)
-        bb = IRBasicBlock(label, ctx)
-        ctx.append_basic_block(bb)
+        bb = IRBasicBlock(label, fn)
+        fn.append_basic_block(bb)
         code = ir.args[2]
         if code.value == "pass":
             bb.append_instruction("exit")
         else:
-            _convert_ir_bb(ctx, code, symbols)
+            _convert_ir_bb(fn, code, symbols)
     elif ir.value == "exit_to":
-        args = _convert_ir_bb_list(ctx, ir.args[1:], symbols)
+        args = _convert_ir_bb_list(fn, ir.args[1:], symbols)
         var_list = args
-        _append_return_args(ctx, *var_list)
-        bb = ctx.get_basic_block()
+        _append_return_args(fn, *var_list)
+        bb = fn.get_basic_block()
         if bb.is_terminated:
-            bb = IRBasicBlock(ctx.get_next_label("exit_to"), ctx)
-            ctx.append_basic_block(bb)
-        bb = ctx.get_basic_block()
+            bb = IRBasicBlock(ctx.get_next_label("exit_to"), fn)
+            fn.append_basic_block(bb)
+        bb = fn.get_basic_block()
 
         label = IRLabel(ir.args[0].value)
         if label.value == "return_pc":
             label = symbols.get("return_pc")
             bb.append_instruction("ret", label)
         else:
             bb.append_instruction("jmp", label)
 
     elif ir.value == "dload":
-        arg_0 = _convert_ir_bb(ctx, ir.args[0], symbols)
-        bb = ctx.get_basic_block()
+        arg_0 = _convert_ir_bb(fn, ir.args[0], symbols)
+        bb = fn.get_basic_block()
         src = bb.append_instruction("add", arg_0, IRLabel("code_end"))
 
         bb.append_instruction("dloadbytes", 32, src, MemoryPositions.FREE_VAR_SPACE)
         return bb.append_instruction("mload", MemoryPositions.FREE_VAR_SPACE)
 
     elif ir.value == "dloadbytes":
-        dst, src_offset, len_ = _convert_ir_bb_list(ctx, ir.args, symbols)
+        dst, src_offset, len_ = _convert_ir_bb_list(fn, ir.args, symbols)
 
-        bb = ctx.get_basic_block()
+        bb = fn.get_basic_block()
         src = bb.append_instruction("add", src_offset, IRLabel("code_end"))
         bb.append_instruction("dloadbytes", len_, src, dst)
         return None
 
-    elif ir.value == "mload":
-        arg_0 = _convert_ir_bb(ctx, ir.args[0], symbols)
-        bb = ctx.get_basic_block()
-        if isinstance(arg_0, IRVariable):
-            return bb.append_instruction("mload", arg_0)
-
-        if isinstance(arg_0, IRLiteral):
-            avar = symbols.get(f"%{arg_0.value}")
-            if avar is not None:
-                return bb.append_instruction("mload", avar)
-
-        return bb.append_instruction("mload", arg_0)
     elif ir.value == "mstore":
         # some upstream code depends on reversed order of evaluation --
         # to fix upstream.
-        arg_1, arg_0 = _convert_ir_bb_list(ctx, reversed(ir.args), symbols)
+        val, ptr = _convert_ir_bb_list(fn, reversed(ir.args), symbols)
 
-        if isinstance(arg_1, IRVariable):
-            symbols[f"&{arg_0.value}"] = arg_1
+        return fn.get_basic_block().append_instruction("mstore", val, ptr)
 
-        ctx.get_basic_block().append_instruction("mstore", arg_1, arg_0)
     elif ir.value == "ceil32":
         x = ir.args[0]
         expanded = IRnode.from_list(["and", ["add", x, 31], ["not", 31]])
-        return _convert_ir_bb(ctx, expanded, symbols)
+        return _convert_ir_bb(fn, expanded, symbols)
     elif ir.value == "select":
         cond, a, b = ir.args
         expanded = IRnode.from_list(
             [
                 "with",
                 "cond",
                 cond,
@@ -459,106 +448,117 @@
                     "with",
                     "a",
                     a,
                     ["with", "b", b, ["xor", "b", ["mul", "cond", ["xor", "a", "b"]]]],
                 ],
             ]
         )
-        return _convert_ir_bb(ctx, expanded, symbols)
+        return _convert_ir_bb(fn, expanded, symbols)
     elif ir.value == "repeat":
 
         def emit_body_blocks():
-            global _break_target, _continue_target
+            global _break_target, _continue_target, _global_symbols
             old_targets = _break_target, _continue_target
             _break_target, _continue_target = exit_block, incr_block
-            _convert_ir_bb(ctx, body, symbols.copy())
+            saved_global_symbols = _global_symbols.copy()
+            _convert_ir_bb(fn, body, symbols.copy())
             _break_target, _continue_target = old_targets
+            _global_symbols = saved_global_symbols
 
         sym = ir.args[0]
-        start, end, _ = _convert_ir_bb_list(ctx, ir.args[1:4], symbols)
+        start, end, _ = _convert_ir_bb_list(fn, ir.args[1:4], symbols)
 
         assert ir.args[3].is_literal, "repeat bound expected to be literal"
 
         bound = ir.args[3].value
         if (
             isinstance(end, IRLiteral)
             and isinstance(start, IRLiteral)
             and end.value + start.value <= bound
         ):
             bound = None
 
         body = ir.args[4]
 
-        entry_block = IRBasicBlock(ctx.get_next_label("repeat"), ctx)
-        cond_block = IRBasicBlock(ctx.get_next_label("condition"), ctx)
-        body_block = IRBasicBlock(ctx.get_next_label("body"), ctx)
-        incr_block = IRBasicBlock(ctx.get_next_label("incr"), ctx)
-        exit_block = IRBasicBlock(ctx.get_next_label("exit"), ctx)
+        entry_block = IRBasicBlock(ctx.get_next_label("repeat"), fn)
+        cond_block = IRBasicBlock(ctx.get_next_label("condition"), fn)
+        body_block = IRBasicBlock(ctx.get_next_label("body"), fn)
+        incr_block = IRBasicBlock(ctx.get_next_label("incr"), fn)
+        exit_block = IRBasicBlock(ctx.get_next_label("exit"), fn)
 
-        bb = ctx.get_basic_block()
+        bb = fn.get_basic_block()
         bb.append_instruction("jmp", entry_block.label)
-        ctx.append_basic_block(entry_block)
+        fn.append_basic_block(entry_block)
 
         counter_var = entry_block.append_instruction("store", start)
         symbols[sym.value] = counter_var
         end = entry_block.append_instruction("add", start, end)
         if bound:
             bound = entry_block.append_instruction("add", start, bound)
         entry_block.append_instruction("jmp", cond_block.label)
 
         xor_ret = cond_block.append_instruction("xor", counter_var, end)
         cont_ret = cond_block.append_instruction("iszero", xor_ret)
-        ctx.append_basic_block(cond_block)
+        fn.append_basic_block(cond_block)
 
-        ctx.append_basic_block(body_block)
+        fn.append_basic_block(body_block)
         if bound:
             xor_ret = body_block.append_instruction("xor", counter_var, bound)
             body_block.append_instruction("assert", xor_ret)
 
         emit_body_blocks()
-        body_end = ctx.get_basic_block()
+        body_end = fn.get_basic_block()
         if body_end.is_terminated is False:
             body_end.append_instruction("jmp", incr_block.label)
 
-        ctx.append_basic_block(incr_block)
+        fn.append_basic_block(incr_block)
         incr_block.insert_instruction(
             IRInstruction("add", [counter_var, IRLiteral(1)], counter_var)
         )
         incr_block.append_instruction("jmp", cond_block.label)
 
-        ctx.append_basic_block(exit_block)
+        fn.append_basic_block(exit_block)
 
         cond_block.append_instruction("jnz", cont_ret, exit_block.label, body_block.label)
     elif ir.value == "break":
         assert _break_target is not None, "Break with no break target"
-        ctx.get_basic_block().append_instruction("jmp", _break_target.label)
-        ctx.append_basic_block(IRBasicBlock(ctx.get_next_label(), ctx))
+        fn.get_basic_block().append_instruction("jmp", _break_target.label)
+        fn.append_basic_block(IRBasicBlock(ctx.get_next_label(), fn))
     elif ir.value == "continue":
         assert _continue_target is not None, "Continue with no contrinue target"
-        ctx.get_basic_block().append_instruction("jmp", _continue_target.label)
-        ctx.append_basic_block(IRBasicBlock(ctx.get_next_label(), ctx))
+        fn.get_basic_block().append_instruction("jmp", _continue_target.label)
+        fn.append_basic_block(IRBasicBlock(ctx.get_next_label(), fn))
     elif ir.value in NOOP_INSTRUCTIONS:
         pass
     elif isinstance(ir.value, str) and ir.value.startswith("log"):
-        args = reversed(_convert_ir_bb_list(ctx, ir.args, symbols))
+        args = reversed(_convert_ir_bb_list(fn, ir.args, symbols))
         topic_count = int(ir.value[3:])
         assert topic_count >= 0 and topic_count <= 4, "invalid topic count"
-        ctx.get_basic_block().append_instruction("log", topic_count, *args)
+        fn.get_basic_block().append_instruction("log", topic_count, *args)
     elif isinstance(ir.value, str) and ir.value.upper() in get_opcodes():
-        _convert_ir_opcode(ctx, ir, symbols)
-    elif isinstance(ir.value, str) and ir.value in symbols:
-        return symbols[ir.value]
+        _convert_ir_opcode(fn, ir, symbols)
+    elif isinstance(ir.value, str):
+        if ir.value.startswith("$alloca") and ir.value not in _global_symbols:
+            alloca = ir.passthrough_metadata["alloca"]
+            ptr = fn.get_basic_block().append_instruction("alloca", alloca.offset, alloca.size)
+            _global_symbols[ir.value] = ptr
+        elif ir.value.startswith("$palloca") and ir.value not in _global_symbols:
+            alloca = ir.passthrough_metadata["alloca"]
+            ptr = fn.get_basic_block().append_instruction("store", alloca.offset)
+            _global_symbols[ir.value] = ptr
+
+        return _global_symbols.get(ir.value) or symbols.get(ir.value)
     elif ir.is_literal:
         return IRLiteral(ir.value)
     else:
         raise Exception(f"Unknown IR node: {ir}")
 
     return None
 
 
-def _convert_ir_opcode(ctx: IRFunction, ir: IRnode, symbols: SymbolTable) -> None:
+def _convert_ir_opcode(fn: IRFunction, ir: IRnode, symbols: SymbolTable) -> None:
     opcode = ir.value.upper()  # type: ignore
     inst_args = []
     for arg in ir.args:
         if isinstance(arg, IRnode):
-            inst_args.append(_convert_ir_bb(ctx, arg, symbols))
-    ctx.get_basic_block().append_instruction(opcode, *inst_args)
+            inst_args.append(_convert_ir_bb(fn, arg, symbols))
+    fn.get_basic_block().append_instruction(opcode, *inst_args)
```

### Comparing `vyper-0.4.0rc2/vyper/venom/passes/dft.py` & `vyper-0.4.0rc3/vyper/venom/passes/dft.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from vyper.utils import OrderedSet
-from vyper.venom.analysis import DFG
+from vyper.venom.analysis.dfg import DFGAnalysis
 from vyper.venom.basicblock import BB_TERMINATORS, IRBasicBlock, IRInstruction, IRVariable
 from vyper.venom.function import IRFunction
 from vyper.venom.passes.base_pass import IRPass
 
 
 class DFTPass(IRPass):
+    function: IRFunction
     inst_order: dict[IRInstruction, int]
     inst_order_num: int
 
     def _process_instruction_r(self, bb: IRBasicBlock, inst: IRInstruction, offset: int = 0):
         for op in inst.get_outputs():
             assert isinstance(op, IRVariable), f"expected variable, got {op}"
             uses = self.dfg.get_uses(op)
@@ -18,21 +19,23 @@
                 if uses_this.parent != inst.parent or uses_this.fence_id != inst.fence_id:
                     # don't reorder across basic block or fence boundaries
                     continue
 
                 # if the instruction is a terminator, we need to place
                 # it at the end of the basic block
                 # along with all the instructions that "lead" to it
-                if uses_this.opcode in BB_TERMINATORS:
-                    offset = len(bb.instructions)
                 self._process_instruction_r(bb, uses_this, offset)
 
         if inst in self.visited_instructions:
             return
         self.visited_instructions.add(inst)
+        self.inst_order_num += 1
+
+        if inst.opcode in BB_TERMINATORS:
+            offset = len(bb.instructions)
 
         if inst.opcode == "phi":
             # phi instructions stay at the beginning of the basic block
             # and no input processing is needed
             # bb.instructions.append(inst)
             self.inst_order[inst] = 0
             return
@@ -41,19 +44,18 @@
             target = self.dfg.get_producing_instruction(op)
             assert target is not None, f"no producing instruction for {op}"
             if target.parent != inst.parent or target.fence_id != inst.fence_id:
                 # don't reorder across basic block or fence boundaries
                 continue
             self._process_instruction_r(bb, target, offset)
 
-        self.inst_order_num += 1
         self.inst_order[inst] = self.inst_order_num + offset
 
     def _process_basic_block(self, bb: IRBasicBlock) -> None:
-        self.ctx.append_basic_block(bb)
+        self.function.append_basic_block(bb)
 
         for inst in bb.instructions:
             inst.fence_id = self.fence_id
             if inst.volatile:
                 self.fence_id += 1
 
         # We go throught the instructions and calculate the order in which they should be executed
@@ -62,19 +64,18 @@
         self.inst_order = {}
         self.inst_order_num = 0
         for inst in bb.instructions:
             self._process_instruction_r(bb, inst)
 
         bb.instructions.sort(key=lambda x: self.inst_order[x])
 
-    def _run_pass(self, ctx: IRFunction) -> None:
-        self.ctx = ctx
-        self.dfg = DFG.build_dfg(ctx)
+    def run_pass(self) -> None:
+        self.dfg = self.analyses_cache.request_analysis(DFGAnalysis)
 
         self.fence_id = 0
         self.visited_instructions: OrderedSet[IRInstruction] = OrderedSet()
 
-        basic_blocks = ctx.basic_blocks
-        ctx.basic_blocks = []
+        basic_blocks = list(self.function.get_basic_blocks())
 
+        self.function.clear_basic_blocks()
         for bb in basic_blocks:
             self._process_basic_block(bb)
```

### Comparing `vyper-0.4.0rc2/vyper/venom/passes/normalization.py` & `vyper-0.4.0rc3/vyper/venom/passes/normalization.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from vyper.venom.analysis import calculate_cfg
+from vyper.exceptions import CompilerPanic
+from vyper.venom.analysis.cfg import CFGAnalysis
 from vyper.venom.basicblock import IRBasicBlock, IRLabel
-from vyper.venom.function import IRFunction
 from vyper.venom.passes.base_pass import IRPass
 
 
 class NormalizationPass(IRPass):
     """
     This pass splits basic blocks when there are multiple conditional predecessors.
     The code generator expect a normalized CFG, that has the property that
@@ -23,45 +23,56 @@
                 self.changes += 1
                 break
 
     def _insert_split_basicblock(self, bb: IRBasicBlock, in_bb: IRBasicBlock) -> IRBasicBlock:
         # Create an intermediary basic block and append it
         source = in_bb.label.value
         target = bb.label.value
+        fn = self.function
 
         split_label = IRLabel(f"{source}_split_{target}")
         in_terminal = in_bb.instructions[-1]
         in_terminal.replace_label_operands({bb.label: split_label})
 
-        split_bb = IRBasicBlock(split_label, self.ctx)
+        split_bb = IRBasicBlock(split_label, fn)
         split_bb.append_instruction("jmp", bb.label)
-        self.ctx.append_basic_block(split_bb)
+        fn.append_basic_block(split_bb)
 
         for inst in bb.instructions:
             if inst.opcode != "phi":
                 continue
             for i in range(0, len(inst.operands), 2):
                 if inst.operands[i] == in_bb.label:
                     inst.operands[i] = split_bb.label
 
         # Update the labels in the data segment
-        for inst in self.ctx.data_segment:
+        for inst in fn.ctx.data_segment:
             if inst.opcode == "db" and inst.operands[0] == bb.label:
                 inst.operands[0] = split_bb.label
 
         return split_bb
 
-    def _run_pass(self, ctx: IRFunction) -> int:
-        self.ctx = ctx
+    def _run_pass(self) -> int:
+        fn = self.function
         self.changes = 0
 
+        self.analyses_cache.request_analysis(CFGAnalysis)
+
         # Split blocks that need splitting
-        for bb in ctx.basic_blocks:
+        for bb in list(fn.get_basic_blocks()):
             if len(bb.cfg_in) > 1:
                 self._split_basic_block(bb)
 
         # If we made changes, recalculate the cfg
         if self.changes > 0:
-            calculate_cfg(ctx)
-            ctx.remove_unreachable_blocks()
+            self.analyses_cache.force_analysis(CFGAnalysis)
+            fn.remove_unreachable_blocks()
 
         return self.changes
+
+    def run_pass(self):
+        fn = self.function
+        for _ in range(fn.num_basic_blocks * 2):
+            if self._run_pass() == 0:
+                break
+        else:
+            raise CompilerPanic("Normalization pass did not converge")
```

### Comparing `vyper-0.4.0rc2/vyper/venom/passes/stack_reorder.py` & `vyper-0.4.0rc3/vyper/venom/passes/stack_reorder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from vyper.utils import OrderedSet
 from vyper.venom.basicblock import IRBasicBlock
-from vyper.venom.function import IRFunction
 from vyper.venom.passes.base_pass import IRPass
 
 
 class StackReorderPass(IRPass):
     visited: OrderedSet
 
-    def _reorder_stack(self, bb: IRBasicBlock):
+    def _reorder_stack(self):
         pass
 
     def _visit(self, bb: IRBasicBlock):
         if bb in self.visited:
             return
         self.visited.add(bb)
 
         for bb_out in bb.cfg_out:
             self._visit(bb_out)
 
-    def _run_pass(self, ctx: IRFunction, entry: IRBasicBlock):
-        self.ctx = ctx
+    def _run_pass(self):
+        entry = self.function.entry
         self.visited = OrderedSet()
         self._visit(entry)
```

### Comparing `vyper-0.4.0rc2/vyper/venom/stack_model.py` & `vyper-0.4.0rc3/vyper/venom/stack_model.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc2/vyper/venom/venom_to_assembly.py` & `vyper-0.4.0rc3/vyper/venom/venom_to_assembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,26 @@
     DataHeader,
     Instruction,
     RuntimeHeader,
     mksymbol,
     optimize_assembly,
 )
 from vyper.utils import MemoryPositions, OrderedSet
-from vyper.venom.analysis import (
-    calculate_cfg,
-    calculate_dup_requirements,
-    calculate_liveness,
-    input_vars_from,
-)
+from vyper.venom.analysis.analysis import IRAnalysesCache
+from vyper.venom.analysis.dup_requirements import DupRequirementsAnalysis
+from vyper.venom.analysis.liveness import LivenessAnalysis
 from vyper.venom.basicblock import (
     IRBasicBlock,
     IRInstruction,
     IRLabel,
     IRLiteral,
     IROperand,
     IRVariable,
 )
-from vyper.venom.function import IRFunction
+from vyper.venom.context import IRContext
 from vyper.venom.passes.normalization import NormalizationPass
 from vyper.venom.stack_model import StackModel
 
 # instructions which map one-to-one from venom to EVM
 _ONE_TO_ONE_INSTRUCTIONS = frozenset(
     [
         "revert",
@@ -93,14 +90,16 @@
         "msize",
         "balance",
         "call",
         "staticcall",
         "delegatecall",
         "codesize",
         "basefee",
+        "blobhash",
+        "blobbasefee",
         "prevrandao",
         "difficulty",
         "invalid",
     ]
 )
 
 _REVERT_POSTAMBLE = ["_sym___revert", "JUMPDEST", *PUSH(0), "DUP1", "REVERT"]
@@ -121,49 +120,45 @@
 # There, recursing into the deploy instruction was by design, and
 # made it easier to make the assembly generated "recursive" (i.e.
 # instructions being lists of instructions). We don't have this restriction
 # anymore, so we can probably refactor this to be iterative in coordination
 # with the assembler. My suggestion is to let this be for now, and we can
 # refactor it later when we are finished phasing out the old IR.
 class VenomCompiler:
-    ctxs: list[IRFunction]
+    ctxs: list[IRContext]
     label_counter = 0
     visited_instructions: OrderedSet  # {IRInstruction}
     visited_basicblocks: OrderedSet  # {IRBasicBlock}
+    liveness_analysis: LivenessAnalysis
 
-    def __init__(self, ctxs: list[IRFunction]):
+    def __init__(self, ctxs: list[IRContext]):
         self.ctxs = ctxs
         self.label_counter = 0
         self.visited_instructions = OrderedSet()
         self.visited_basicblocks = OrderedSet()
 
     def generate_evm(self, no_optimize: bool = False) -> list[str]:
         self.visited_instructions = OrderedSet()
         self.visited_basicblocks = OrderedSet()
         self.label_counter = 0
 
         asm: list[Any] = []
         top_asm = asm
 
-        # Before emitting the assembly, we need to make sure that the
-        # CFG is normalized. Calling calculate_cfg() will denormalize IR (reset)
-        # so it should not be called after calling NormalizationPass().run_pass().
-        # Liveness is then computed for the normalized IR, and we can proceed to
-        # assembly generation.
-        # This is a side-effect of how dynamic jumps are temporarily being used
-        # to support the O(1) dispatcher. -> look into calculate_cfg()
         for ctx in self.ctxs:
-            NormalizationPass().run_pass(ctx)
-            calculate_cfg(ctx)
-            calculate_liveness(ctx)
-            calculate_dup_requirements(ctx)
+            for fn in ctx.functions.values():
+                ac = IRAnalysesCache(fn)
+
+                NormalizationPass(ac, fn).run_pass()
+                self.liveness_analysis = ac.request_analysis(LivenessAnalysis)
+                ac.request_analysis(DupRequirementsAnalysis)
 
-            assert ctx.normalized, "Non-normalized CFG!"
+                assert fn.normalized, "Non-normalized CFG!"
 
-            self._generate_evm_for_basicblock_r(asm, ctx.basic_blocks[0], StackModel())
+                self._generate_evm_for_basicblock_r(asm, fn.entry, StackModel())
 
             # TODO make this property on IRFunction
             asm.extend(["_sym__ctor_exit", "JUMPDEST"])
             if ctx.immutables_len is not None and ctx.ctor_mem_size is not None:
                 asm.extend(
                     ["_sym_subcode_size", "_sym_runtime_begin", "_mem_deploy_start", "CODECOPY"]
                 )
@@ -315,15 +310,15 @@
     ) -> None:
         if len(basicblock.cfg_in) == 0:
             return
 
         to_pop = OrderedSet[IRVariable]()
         for in_bb in basicblock.cfg_in:
             # inputs is the input variables we need from in_bb
-            inputs = input_vars_from(in_bb, basicblock)
+            inputs = self.liveness_analysis.input_vars_from(in_bb, basicblock)
 
             # layout is the output stack layout for in_bb (which works
             # for all possible cfg_outs from the in_bb).
             layout = in_bb.out_vars
 
             # pop all the stack items which in_bb produced which we don't need.
             to_pop |= layout.difference(inputs)
@@ -348,17 +343,18 @@
         #
         # generate EVM for op
         #
 
         # Step 1: Apply instruction special stack manipulations
 
         if opcode in ["jmp", "djmp", "jnz", "invoke"]:
-            operands = inst.get_non_label_operands()
+            operands = list(inst.get_non_label_operands())
         elif opcode == "alloca":
-            operands = inst.operands[1:2]
+            offset, _size = inst.operands
+            operands = [offset]
 
         # iload and istore are special cases because they can take a literal
         # that is handled specialy with the _OFST macro. Look below, after the
         # stack reordering.
         elif opcode == "iload":
             addr = inst.operands[0]
             if isinstance(addr, IRLiteral):
@@ -376,15 +372,15 @@
             assert log_topic_count in [0, 1, 2, 3, 4], "Invalid topic count"
             operands = inst.operands[1:]
         else:
             operands = inst.operands
 
         if opcode == "phi":
             ret = inst.get_outputs()[0]
-            phis = inst.get_inputs()
+            phis = list(inst.get_inputs())
             depth = stack.get_phi_depth(phis)
             # collapse the arguments to the phi node in the stack.
             # example, for `%56 = %label1 %13 %label2 %14`, we will
             # find an instance of %13 *or* %14 in the stack and replace it with %56.
             to_be_replaced = stack.peek(depth)
             if to_be_replaced in inst.dup_requirements:
                 # %13/%14 is still live(!), so we make a copy of it
@@ -398,15 +394,15 @@
         self._emit_input_operands(assembly, inst, operands, stack)
 
         # Step 3: Reorder stack
         if opcode in ["jnz", "djmp", "jmp"]:
             # prepare stack for jump into another basic block
             assert inst.parent and isinstance(inst.parent.cfg_out, OrderedSet)
             b = next(iter(inst.parent.cfg_out))
-            target_stack = input_vars_from(inst.parent, b)
+            target_stack = self.liveness_analysis.input_vars_from(inst.parent, b)
             # TODO optimize stack reordering at entry and exit from basic blocks
             # NOTE: stack in general can contain multiple copies of the same variable,
             # however we are safe in the case of jmp/djmp/jnz as it's not going to
             # have multiples.
             target_stack_list = list(target_stack)
             self._stack_reorder(assembly, stack, target_stack_list)
 
@@ -518,14 +514,16 @@
             if isinstance(addr, IRLiteral):
                 assembly.extend(["_OFST", "_mem_deploy_end", addr.value])
             else:
                 assembly.extend(["_mem_deploy_end", "ADD"])
             assembly.append("MSTORE")
         elif opcode == "log":
             assembly.extend([f"LOG{log_topic_count}"])
+        elif opcode == "nop":
+            pass
         else:
             raise Exception(f"Unknown opcode: {opcode}")
 
         # Step 6: Emit instructions output operands (if any)
         if inst.output is not None:
             if "call" in inst.opcode and inst.output not in next_liveness:
                 self.pop(assembly, stack)
```

### Comparing `vyper-0.4.0rc2/vyper.egg-info/PKG-INFO` & `vyper-0.4.0rc3/vyper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0rc2
+Version: 0.4.0rc3
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0rc2/vyper.egg-info/SOURCES.txt` & `vyper-0.4.0rc3/vyper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -70,23 +70,28 @@
 examples/tokens/ERC721.vy
 examples/voting/ballot.vy
 examples/wallet/wallet.vy
 hooks/build
 tests/__init__.py
 tests/conftest.py
 tests/utils.py
-tests/fixtures/__init__.py
-tests/fixtures/memorymock.py
+tests/evm_backends/__init__.py
+tests/evm_backends/abi.py
+tests/evm_backends/abi_contract.py
+tests/evm_backends/base_env.py
+tests/evm_backends/pyevm_env.py
+tests/evm_backends/revm_env.py
 tests/functional/__init__.py
 tests/functional/builtins/codegen/__init__.py
 tests/functional/builtins/codegen/test_abi_decode.py
 tests/functional/builtins/codegen/test_abi_encode.py
 tests/functional/builtins/codegen/test_addmod.py
 tests/functional/builtins/codegen/test_as_wei_value.py
 tests/functional/builtins/codegen/test_bitwise.py
+tests/functional/builtins/codegen/test_blobhash.py
 tests/functional/builtins/codegen/test_ceil.py
 tests/functional/builtins/codegen/test_concat.py
 tests/functional/builtins/codegen/test_convert.py
 tests/functional/builtins/codegen/test_create_functions.py
 tests/functional/builtins/codegen/test_ec.py
 tests/functional/builtins/codegen/test_ecrecover.py
 tests/functional/builtins/codegen/test_empty.py
@@ -124,14 +129,15 @@
 tests/functional/codegen/calling_convention/test_default_function.py
 tests/functional/codegen/calling_convention/test_default_parameters.py
 tests/functional/codegen/calling_convention/test_erc20_abi.py
 tests/functional/codegen/calling_convention/test_external_contract_calls.py
 tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
 tests/functional/codegen/calling_convention/test_return.py
 tests/functional/codegen/calling_convention/test_self_call_struct.py
+tests/functional/codegen/environment_variables/test_blobbasefee.py
 tests/functional/codegen/environment_variables/test_block_number.py
 tests/functional/codegen/environment_variables/test_blockhash.py
 tests/functional/codegen/environment_variables/test_tx.py
 tests/functional/codegen/features/test_address_balance.py
 tests/functional/codegen/features/test_assert.py
 tests/functional/codegen/features/test_assert_unreachable.py
 tests/functional/codegen/features/test_assignment.py
@@ -199,15 +205,14 @@
 tests/functional/codegen/types/numbers/test_division.py
 tests/functional/codegen/types/numbers/test_exponents.py
 tests/functional/codegen/types/numbers/test_isqrt.py
 tests/functional/codegen/types/numbers/test_modulo.py
 tests/functional/codegen/types/numbers/test_signed_ints.py
 tests/functional/codegen/types/numbers/test_sqrt.py
 tests/functional/codegen/types/numbers/test_unsigned_ints.py
-tests/functional/examples/conftest.py
 tests/functional/examples/auctions/test_blind_auction.py
 tests/functional/examples/auctions/test_simple_open_auction.py
 tests/functional/examples/company/test_company.py
 tests/functional/examples/crowdfund/test_crowdfund_example.py
 tests/functional/examples/factory/test_factory.py
 tests/functional/examples/market_maker/test_on_chain_market_maker.py
 tests/functional/examples/name_registry/test_name_registry.py
@@ -358,14 +363,15 @@
 tests/unit/compiler/ir/test_with.py
 tests/unit/compiler/venom/test_convert_basicblock_simple.py
 tests/unit/compiler/venom/test_dominator_tree.py
 tests/unit/compiler/venom/test_duplicate_operands.py
 tests/unit/compiler/venom/test_liveness_simple_loop.py
 tests/unit/compiler/venom/test_make_ssa.py
 tests/unit/compiler/venom/test_multi_entry_block.py
+tests/unit/compiler/venom/test_sccp.py
 tests/unit/compiler/venom/test_stack_at_external_return.py
 tests/unit/compiler/venom/test_variables.py
 tests/unit/semantics/conftest.py
 tests/unit/semantics/test_namespace.py
 tests/unit/semantics/test_storage_slots.py
 tests/unit/semantics/analysis/test_array_index.py
 tests/unit/semantics/analysis/test_cyclic_function_calls.py
@@ -413,14 +419,15 @@
 vyper/builtins/functions.py
 vyper/builtins/interfaces/IERC165.vyi
 vyper/builtins/interfaces/IERC20.vyi
 vyper/builtins/interfaces/IERC20Detailed.vyi
 vyper/builtins/interfaces/IERC4626.vyi
 vyper/builtins/interfaces/IERC721.vyi
 vyper/cli/__init__.py
+vyper/cli/compile_archive.py
 vyper/cli/vyper_compile.py
 vyper/cli/vyper_ir.py
 vyper/cli/vyper_json.py
 vyper/codegen/__init__.py
 vyper/codegen/abi_encoder.py
 vyper/codegen/arithmetic.py
 vyper/codegen/context.py
@@ -440,14 +447,15 @@
 vyper/codegen/function_definitions/common.py
 vyper/codegen/function_definitions/external_function.py
 vyper/codegen/function_definitions/internal_function.py
 vyper/compiler/README.md
 vyper/compiler/__init__.py
 vyper/compiler/input_bundle.py
 vyper/compiler/output.py
+vyper/compiler/output_bundle.py
 vyper/compiler/phases.py
 vyper/compiler/settings.py
 vyper/compiler/utils.py
 vyper/evm/__init__.py
 vyper/evm/address_space.py
 vyper/evm/opcodes.py
 vyper/ir/README.md
@@ -480,22 +488,31 @@
 vyper/semantics/types/primitives.py
 vyper/semantics/types/shortcuts.py
 vyper/semantics/types/subscriptable.py
 vyper/semantics/types/user.py
 vyper/semantics/types/utils.py
 vyper/venom/README.md
 vyper/venom/__init__.py
-vyper/venom/analysis.py
 vyper/venom/basicblock.py
-vyper/venom/bb_optimizer.py
-vyper/venom/dominators.py
+vyper/venom/context.py
 vyper/venom/function.py
 vyper/venom/ir_node_to_venom.py
 vyper/venom/stack_model.py
 vyper/venom/venom_to_assembly.py
+vyper/venom/analysis/__init__.py
+vyper/venom/analysis/analysis.py
+vyper/venom/analysis/cfg.py
+vyper/venom/analysis/dfg.py
+vyper/venom/analysis/dominators.py
+vyper/venom/analysis/dup_requirements.py
+vyper/venom/analysis/liveness.py
 vyper/venom/passes/base_pass.py
-vyper/venom/passes/constant_propagation.py
 vyper/venom/passes/dft.py
 vyper/venom/passes/make_ssa.py
+vyper/venom/passes/mem2var.py
 vyper/venom/passes/normalization.py
+vyper/venom/passes/remove_unused_variables.py
 vyper/venom/passes/simplify_cfg.py
-vyper/venom/passes/stack_reorder.py
+vyper/venom/passes/stack_reorder.py
+vyper/venom/passes/sccp/__init__.py
+vyper/venom/passes/sccp/eval.py
+vyper/venom/passes/sccp/sccp.py
```

### Comparing `vyper-0.4.0rc2/vyper.egg-info/requires.txt` & `vyper-0.4.0rc3/vyper.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 pyinstaller
 twine
 pytest<9.0,>=8.0
 pytest-cov<5.0,>=4.1
 pytest-instafail<1.0,>=0.4
 pytest-xdist<3.4,>=3.0
 pytest-split<1.0,>=0.7.0
-eth-tester[py-evm]<0.11,>=0.10.0b4
-eth_abi<5.0.0,>=4.0.0
-py-evm<0.11,>=0.10.0b4
-web3==6.0.0
+eth_abi<6.0.0,>=5.0.0
+py-evm<0.11,>=0.10.1b1
 lark==1.1.9
 hypothesis[lark]<7.0,>=6.0
 eth-stdlib==0.2.7
+eth-account==0.12.2
 setuptools
 hexbytes>=1.2
+pyrevm>=0.3.2
 black==23.12.0
 flake8==6.1.0
 flake8-bugbear==23.12.2
 flake8-use-fstring==1.4
 isort==5.13.2
 mypy==1.5
 
@@ -41,16 +41,16 @@
 
 [test]
 pytest<9.0,>=8.0
 pytest-cov<5.0,>=4.1
 pytest-instafail<1.0,>=0.4
 pytest-xdist<3.4,>=3.0
 pytest-split<1.0,>=0.7.0
-eth-tester[py-evm]<0.11,>=0.10.0b4
-eth_abi<5.0.0,>=4.0.0
-py-evm<0.11,>=0.10.0b4
-web3==6.0.0
+eth_abi<6.0.0,>=5.0.0
+py-evm<0.11,>=0.10.1b1
 lark==1.1.9
 hypothesis[lark]<7.0,>=6.0
 eth-stdlib==0.2.7
+eth-account==0.12.2
 setuptools
 hexbytes>=1.2
+pyrevm>=0.3.2
```


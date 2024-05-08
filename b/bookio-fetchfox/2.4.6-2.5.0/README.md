# Comparing `tmp/bookio_fetchfox-2.4.6.tar.gz` & `tmp/bookio_fetchfox-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-2.4.6.tar", max compression
+gzip compressed data, was "bookio_fetchfox-2.5.0.tar", max compression
```

## Comparing `bookio_fetchfox-2.4.6.tar` & `bookio_fetchfox-2.5.0.tar`

### file list

```diff
@@ -1,79 +1,77 @@
--rw-r--r--   0        0        0     3734 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/README.md
--rw-r--r--   0        0        0        0 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2510 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0      609 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/algorand/algoxnftcom.py
--rw-r--r--   0        0        0     1427 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0     2156 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/algorand/nftexplorerapp.py
--rw-r--r--   0        0        0      605 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      262 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0      259 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/cardano/cexplorerio.py
--rw-r--r--   0        0        0      891 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/cardano/cnfttools.py
--rw-r--r--   0        0        0     1908 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/cardano/dexhunterio.py
--rw-r--r--   0        0        0     7006 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/cardano/gomaestroorg.py
--rw-r--r--   0        0        0     1798 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/cardano/jpgstore.py
--rw-r--r--   0        0        0      536 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/cardano/muesliswap.py
--rwxr-xr-x   0        0        0     1572 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0      988 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     5658 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     3037 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      228 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/pinatacloud.py
--rw-r--r--   0        0        0      228 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/apis/price.py
--rw-r--r--   0        0        0      120 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0    10494 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      689 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/algorand/exceptions.py
--rw-r--r--   0        0        0      502 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     3408 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    17568 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0      679 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/cardano/exceptions.py
--rw-r--r--   0        0        0     1060 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0     1696 2024-04-22 20:48:08.070615 bookio_fetchfox-2.4.6/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0    11892 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      753 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/blockchains/evm/exceptions.py
--rw-r--r--   0        0        0      617 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0      443 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/blockchains/exceptions.py
--rw-r--r--   0        0        0       32 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0     1706 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      146 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      299 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/beard.py
--rw-r--r--   0        0        0      158 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      399 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/book.py
--rw-r--r--   0        0        0       82 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/cardano.py
--rw-r--r--   0        0        0      163 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0       66 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/evm.py
--rw-r--r--   0        0        0      341 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0   453386 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/ranks.py
--rw-r--r--   0        0        0       95 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       62 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      329 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     3719 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     3666 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      495 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1572 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      948 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/order.py
--rw-r--r--   0        0        0     1203 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/pair_stats.py
--rw-r--r--   0        0        0      365 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     2023 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2024-04-22 20:48:08.074615 bookio_fetchfox-2.4.6/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0        0 2024-04-22 20:48:08.078615 bookio_fetchfox-2.4.6/fetchfox/pools/__init__.py
--rw-r--r--   0        0        0     1135 2024-04-22 20:48:08.078615 bookio_fetchfox-2.4.6/fetchfox/pools/book_pool.py
--rw-r--r--   0        0        0     5794 2024-04-22 20:48:08.078615 bookio_fetchfox-2.4.6/fetchfox/rest.py
--rw-r--r--   0        0        0      106 2024-04-22 20:48:08.078615 bookio_fetchfox-2.4.6/fetchfox/tokens/__init__.py
--rw-r--r--   0        0        0     4200 2024-04-22 20:48:08.078615 bookio_fetchfox-2.4.6/fetchfox/tokens/base.py
--rw-r--r--   0        0        0      744 2024-04-22 20:48:08.078615 bookio_fetchfox-2.4.6/fetchfox/tokens/beard_token.py
--rw-r--r--   0        0        0      811 2024-04-22 20:48:08.078615 bookio_fetchfox-2.4.6/fetchfox/tokens/book_token.py
--rw-r--r--   0        0        0      802 2024-04-22 20:48:08.078615 bookio_fetchfox-2.4.6/fetchfox/tokens/hosky_token.py
--rw-r--r--   0        0        0     1148 2024-04-22 20:48:08.090615 bookio_fetchfox-2.4.6/pyproject.toml
--rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 bookio_fetchfox-2.4.6/setup.py
--rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 bookio_fetchfox-2.4.6/PKG-INFO
+-rw-r--r--   0        0        0     3734 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2649 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0      694 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/algorand/algoxnftcom.py
+-rw-r--r--   0        0        0     1501 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0     2337 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/algorand/nftexplorerapp.py
+-rw-r--r--   0        0        0      686 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      317 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2289 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/cardano/dexhunterio.py
+-rw-r--r--   0        0        0     7351 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/cardano/gomaestroorg.py
+-rw-r--r--   0        0        0     1868 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/cardano/jpgstore.py
+-rw-r--r--   0        0        0      592 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/cardano/muesliswap.py
+-rwxr-xr-x   0        0        0     2197 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0     1089 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     5900 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     3215 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      285 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/pinatacloud.py
+-rw-r--r--   0        0        0      228 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/apis/price.py
+-rw-r--r--   0        0        0      120 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0    10494 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      689 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/algorand/exceptions.py
+-rw-r--r--   0        0        0      502 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     3408 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    17568 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0      679 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/cardano/exceptions.py
+-rw-r--r--   0        0        0     1060 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0     1696 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0    11880 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      753 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/evm/exceptions.py
+-rw-r--r--   0        0        0      617 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0      443 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/exceptions.py
+-rw-r--r--   0        0        0       32 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      146 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/constants/beard.py
+-rw-r--r--   0        0        0      158 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      399 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/constants/book.py
+-rw-r--r--   0        0        0       82 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/constants/cardano.py
+-rw-r--r--   0        0        0      163 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0       66 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/constants/evm.py
+-rw-r--r--   0        0        0      341 2024-05-08 17:43:54.232941 bookio_fetchfox-2.5.0/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0   453386 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/constants/ranks.py
+-rw-r--r--   0        0        0       95 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       62 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      329 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     3719 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3666 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      495 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1572 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      948 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/order.py
+-rw-r--r--   0        0        0     1203 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/pair_stats.py
+-rw-r--r--   0        0        0      365 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     2023 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0        0 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/pools/__init__.py
+-rw-r--r--   0        0        0     1177 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/pools/book_pool.py
+-rw-r--r--   0        0        0     5794 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/rest.py
+-rw-r--r--   0        0        0      106 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/tokens/__init__.py
+-rw-r--r--   0        0        0     4025 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/tokens/base.py
+-rw-r--r--   0        0        0      744 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/tokens/beard_token.py
+-rw-r--r--   0        0        0      811 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/tokens/book_token.py
+-rw-r--r--   0        0        0      802 2024-05-08 17:43:54.236941 bookio_fetchfox-2.5.0/fetchfox/tokens/hosky_token.py
+-rw-r--r--   0        0        0     1148 2024-05-08 17:43:54.244941 bookio_fetchfox-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 bookio_fetchfox-2.5.0/setup.py
+-rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 bookio_fetchfox-2.5.0/PKG-INFO
```

### Comparing `bookio_fetchfox-2.4.6/README.md` & `bookio_fetchfox-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/algorand/algonodecloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 import json
+import os
 from base64 import b64decode
 from functools import lru_cache
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = "https://mainnet-idx.algonode.cloud"
+BASE_URL = os.environ.get(
+    "ALGONODE_API_BASE_URL",
+    "https://mainnet-idx.algonode.cloud",
+)
 
 
 def get(service: str, params: dict = None, version: int = 2) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params,
     )
 
 
 def get_account_assets(address: str) -> Iterable[dict]:
     check_str(address, "algonodecloud.address")
     address = address.strip().upper()
 
-    response, status_code = get(f"accounts/{address}")
+    response, status_code = get(
+        service=f"accounts/{address}",
+    )
 
     account = response["account"]
 
     for asset in account.get("assets", []):
         yield asset
 
 
 def get_account_balance(address: str) -> Iterable[str]:
     check_str(address, "algonodecloud.address")
     address = address.strip().upper()
 
-    response, status_code = get(f"accounts/{address}")
+    response, status_code = get(
+        service=f"accounts/{address}",
+    )
 
     return int(response["account"]["amount"]) / 10**6
 
 
 @lru_cache(maxsize=None)
 def get_asset_data(asset_id: str) -> dict:
     check_str(asset_id, "algonodecloud.asset_id")
 
-    response, status_code = get(f"assets/{asset_id}")
+    response, status_code = get(
+        service=f"assets/{asset_id}",
+    )
 
     return response["asset"]["params"]
 
 
 @lru_cache(maxsize=None)
 def get_asset_metadata(asset_id: str) -> dict:
     check_str(asset_id, "algonodecloud.asset_id")
@@ -64,15 +74,15 @@
     return json.loads(note)
 
 
 def get_asset_owner(asset_id: str) -> dict:
     check_str(asset_id, "algonodecloud.asset_id")
 
     response, status_code = get(
-        f"assets/{asset_id}/balances",
+        service=f"assets/{asset_id}/balances",
         params={
             "currency-greater-than": "0",
         },
     )
 
     balances = response.get("balances", [])
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/algorand/algoxnftcom.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/algorand/algoxnftcom.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import os
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = "https://api.algoxnft.com"
+BASE_URL = os.environ.get(
+    "ALGOXNFT_API_BASE_URL",
+    "https://api.algoxnft.com",
+)
 
 
 def get(service: str, params: dict = None, version: int = 1) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params,
     )
 
 
 def get_collection_listings(creator_address: str) -> Iterable[dict]:
     check_str(creator_address, "algoxnftcom.creator_address")
     creator_address = creator_address.strip().upper()
 
-    response, status_code = get(f"nft-explorer/creator/{creator_address}")
+    response, status_code = get(
+        service=f"nft-explorer/creator/{creator_address}",
+    )
 
     yield from response
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/algorand/nfdomains.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import logging
+import os
 from functools import lru_cache
 from typing import Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = "https://api.nf.domains"
+BASE_URL = os.getenv(
+    "NFDOMAINS_API_BASE_URL",
+    "https://api.nf.domains",
+)
 
 logger = logging.getLogger(__name__)
 
 
 def get(service: str, params: dict = None) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/{service}",
@@ -18,15 +22,15 @@
 
 
 @lru_cache(maxsize=None)
 def resolve_nf_domain(nf_domain: str):
     check_str(nf_domain, "nfddomains.nf_domain")
 
     response, status_code = get(
-        "nfd",
+        service="nfd",
         params={
             "prefix": nf_domain,
             "limit": 1,
         },
     )
 
     if not response:
@@ -40,15 +44,15 @@
 
 @lru_cache(maxsize=None)
 def get_nf_domain(address: str):
     check_str(address, "nfddomains.address")
     address = address.strip().upper()
 
     response, status_code = get(
-        f"nfd/v2/address",
+        service=f"nfd/v2/address",
         params={
             "address": address,
         },
     )
 
     if status_code == 404:
         return None
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/algorand/nftexplorerapp.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/algorand/nftexplorerapp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import logging
+import os
 from functools import lru_cache
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = "https://api.nftexplorer.app"
+API_KEY = os.getenv("NFTEXPLORER_API_KEY")
+
+BASE_URL = os.getenv(
+    "NFTEXPLORER_API_BASE_URL",
+    "https://api.nftexplorer.app",
+)
 
 logger = logging.getLogger(__name__)
 
 
-def get(service: str, api_key: str, params: dict = None, version: int = 1) -> Tuple[dict, int]:
+def get(service: str, params: dict = None, version: int = 1, api_key: str = None) -> Tuple[dict, int]:
+    api_key = api_key or API_KEY
     check_str(api_key, "nftexplorerapp.api_key")
 
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         headers={
             "Authorization": api_key,
         },
         params=params,
-        sleep=1,
+        sleep=0.5,
     )
 
 
 @lru_cache(maxsize=None)
 def get_collection_id(creator_address: str, api_key: str) -> str:
-    check_str(creator_address, "randswap.creator_address")
+    check_str(creator_address, "nftexplorerapp.creator_address")
     creator_address = creator_address.strip().upper()
 
     response, status_code = get(
-        "collections/search",
+        service="collections/search",
         params={
             "q": creator_address,
         },
         api_key=api_key,
     )
 
     if response.get("error"):
@@ -49,28 +56,28 @@
 
     if recognized:
         return recognized[0]["collectionId"]
 
     return None
 
 
-def get_collection_sales(creator_address: str, api_key: str) -> Iterable[dict]:
-    check_str(creator_address, "randswap.creator_address")
+def get_collection_sales(creator_address: str, api_key: str = None) -> Iterable[dict]:
+    check_str(creator_address, "nftexplorerapp.creator_address")
     creator_address = creator_address.strip().upper()
 
     collection_id = get_collection_id(creator_address, api_key)
 
     if not collection_id:
         return
 
     next_token = ""
 
     while True:
         response, status_code = get(
-            "/collections/salesHistory",
+            service="/collections/salesHistory",
             params={
                 "collectionId": collection_id,
                 "nextToken": next_token,
             },
             api_key=api_key,
         )
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/algorand/randswapcom.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import os
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = "https://www.randswap.com"
+BASE_URL = os.environ.get(
+    "RANDSWAP_API_BASE_URL",
+    "https://randswap.com",
+)
 
 
 def get(service: str, params: dict = None, version: int = 1) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params,
     )
 
 
 def get_collection_listings(creator_address: str) -> Iterable[dict]:
     check_str(creator_address, "randswapcom.creator_address")
     creator_address = creator_address.strip().upper()
 
-    response, status_code = get(f"listings/creator/{creator_address}")
+    response, status_code = get(
+        service=f"listings/creator/{creator_address}",
+    )
 
     yield from response
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/cardano/dexhunterio.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/cardano/dexhunterio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,56 @@
+import os
 from typing import Iterable
 
 from fetchfox import rest
+from fetchfox.checks import check_str
+
+BASE_URL = os.getenv(
+    "DEXHUNTER_API_BASE_URL",
+    "https://dexhunter.sbase.ch/",
+)
+
+PARTNER_CODE = os.getenv("DEXHUNTER_PARTNER_CODE")
+
 
 ADA = "000000000000000000000000000000000000000000000000000000006c6f76656c616365"
-BASE_URL = "https://dexhunter.sbase.ch/"
 
 
-def get(service: str, partner_code: str, params: dict = None) -> dict:
-    url = f"{BASE_URL}/{service}"
+def get(service: str, params: dict = None, partner_code: str = None) -> dict:
+    partner_code = partner_code or PARTNER_CODE
+    check_str(partner_code, "dexhunterio.partner_code")
 
     response, _ = rest.get(
-        url=url,
+        url=f"{BASE_URL}/{service}",
         params=params,
         headers={
             "X-Partner-Id": partner_code,
         },
     )
 
     return response
 
 
-def post(service: str, body: dict, partner_code: str, params: dict = None) -> dict:
-    url = f"{BASE_URL}/{service}"
+def post(service: str, body: dict, params: dict = None, partner_code: str = None) -> dict:
+    partner_code = partner_code or PARTNER_CODE
+    check_str(partner_code, "dexhunterio.partner_code")
 
     response, _ = rest.post(
-        url=url,
+        url=f"{BASE_URL}/{service}",
         params=params,
         body=body,
         headers={
             "X-Partner-Id": partner_code,
         },
     )
 
     return response
 
 
-def get_asset_orders(asset_id: str, partner_code: str) -> Iterable[dict]:
+def get_asset_orders(asset_id: str, partner_code: str = None) -> Iterable[dict]:
     body = {
         "filters": [
             {
                 "filterType": "TOKENID",
                 "values": [asset_id],
             },
             {
@@ -67,21 +78,21 @@
 
         if not response.get("orders"):
             break
 
         yield from response["orders"]
 
 
-def get_asset_average_price(asset_id: str, partner_code: str) -> float:
+def get_asset_average_price(asset_id: str, partner_code: str = None) -> float:
     response = get(
-        f"swap/averagePrice/{asset_id}/ADA",
+        service=f"swap/averagePrice/{asset_id}/ADA",
         partner_code=partner_code,
     )
 
     return response["average_price"]
 
 
-def get_asset_pair_stats(asset_id: str, partner_code: str) -> dict:
+def get_asset_pair_stats(asset_id: str, partner_code: str = None) -> dict:
     return get(
-        f"swap/pairStats/{asset_id}/ADA",
+        service=f"swap/pairStats/{asset_id}/ADA",
         partner_code=partner_code,
     )
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/cardano/gomaestroorg.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/cardano/gomaestroorg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 import base64
+import os
 from functools import lru_cache
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 from fetchfox.constants.cardano import ADA_HANDLE_POLICY_ID
 
-BASE_URL = "https://mainnet.gomaestro-api.org"
+BASE_URL = os.getenv(
+    "GOMAESTRO_BASE_URL",
+    "https://mainnet.gomaestro-api.org",
+)
 
+API_KEY = os.getenv("GOMAESTRO_API_KEY")
 
-def get(service: str, api_key: str, params: dict = None, version: int = 1) -> Tuple[dict, int]:
-    check_str(api_key, "gomaestro.api_key")
+
+def get(service: str, params: dict = None, version: int = 1, api_key: str = None) -> Tuple[dict, int]:
+    api_key = api_key or API_KEY
+    check_str(api_key, "gomaestroorg.api_key")
 
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params,
         headers={
             "api-key": api_key,
         },
     )
 
 
-def get_account_assets(stake_address: str, api_key: str, policy_id: str = None) -> Iterable[Tuple[str, int]]:
-    check_str(stake_address, "gomaestro.stake_address")
+def get_account_assets(stake_address: str, policy_id: str = None, api_key: str = None) -> Iterable[Tuple[str, int]]:
+    check_str(stake_address, "gomaestroorg.stake_address")
     stake_address = stake_address.strip().lower()
 
     if policy_id:
         policy_id = policy_id.strip().lower()
 
     cursor = None
 
     while True:
         response, status_code = get(
-            f"accounts/{stake_address}/assets",
+            service=f"accounts/{stake_address}/assets",
             params={
                 "cursor": cursor,
                 "policy": policy_id,
             },
             api_key=api_key,
         )
 
@@ -44,56 +51,56 @@
 
         cursor = response.get("next_cursor")
 
         if not cursor:
             break
 
 
-def get_account_balance(stake_address: str, api_key: str) -> float:
-    check_str(stake_address, "gomaestro.stake_address")
+def get_account_balance(stake_address: str, api_key: str = None) -> float:
+    check_str(stake_address, "gomaestroorg.stake_address")
 
     response, status_code = get(
-        f"accounts/{stake_address}",
+        service=f"accounts/{stake_address}",
         api_key=api_key,
     )
 
     return response["data"]["total_balance"] / 10**6
 
 
-def get_collection_owners(policy_id: str, api_key: str) -> Iterable[dict]:
-    check_str(api_key, "gomaestro.api-key")
+def get_collection_owners(policy_id: str, api_key: str = None) -> Iterable[dict]:
+    check_str(policy_id, "gomaestroorg.policy_id")
     policy_id = policy_id.strip().lower()
 
     cursor = None
 
     while True:
         response, status_code = get(
-            f"policy/{policy_id}/accounts",
+            service=f"policy/{policy_id}/accounts",
             params={
                 "cursor": cursor,
             },
             api_key=api_key,
         )
 
         yield from response.get("data", [])
 
         cursor = response.get("next_cursor")
 
         if not cursor:
             break
 
 
-def get_asset_owners(asset_id: str, api_key: str) -> Iterable[dict]:
-    check_str(asset_id, "gomaestro.asset_id")
+def get_asset_owners(asset_id: str, api_key: str = None) -> Iterable[dict]:
+    check_str(asset_id, "gomaestroorg.asset_id")
 
     cursor = None
 
     while True:
         response, status_code = get(
-            f"assets/{asset_id}/accounts",
+            service=f"assets/{asset_id}/accounts",
             params={
                 "cursor": cursor,
             },
             api_key=api_key,
         )
 
         for item in response.get("data", []):
@@ -105,23 +112,23 @@
 
         cursor = response.get("next_cursor")
 
         if not cursor:
             break
 
 
-def get_collection_assets(policy_id: str, api_key: str) -> Iterable[dict]:
-    check_str(policy_id, "gomaestro.policy_id")
+def get_collection_assets(policy_id: str, api_key: str = None) -> Iterable[dict]:
+    check_str(policy_id, "gomaestroorg.policy_id")
     policy_id = policy_id.strip().lower()
 
     cursor = None
 
     while True:
         response, status_code = get(
-            f"policy/{policy_id}/assets",
+            service=f"policy/{policy_id}/assets",
             params={
                 "cursor": cursor,
             },
             api_key=api_key,
         )
 
         for item in response.get("data", []):
@@ -135,71 +142,71 @@
         cursor = response.get("next_cursor")
 
         if not cursor:
             break
 
 
 @lru_cache(maxsize=None)
-def get_asset_data(asset_id: str, api_key: str) -> dict:
-    check_str(asset_id, "gomaestro.asset_id")
+def get_asset_data(asset_id: str, api_key: str = None) -> dict:
+    check_str(asset_id, "gomaestroorg.asset_id")
 
     asset_id = asset_id.strip().lower()
 
     response, status_code = get(
-        f"assets/{asset_id}",
+        service=f"assets/{asset_id}",
         api_key=api_key,
     )
 
     cip25_metadata = response["data"]["asset_standards"].get("cip25_metadata")
     cip68_metadata = response["data"]["asset_standards"].get("cip68_metadata")
 
     metadata = cip68_metadata or cip25_metadata
     metadata["total_supply"] = response["data"].get("total_supply", "1")
 
     return metadata
 
 
 @lru_cache(maxsize=None)
-def get_stake_address(address: str, api_key: str) -> str:
-    check_str(address, "gomaestro.address")
+def get_stake_address(address: str, api_key: str = None) -> str:
+    check_str(address, "gomaestroorg.address")
 
     response, status_code = get(
-        f"addresses/{address}/decode",
+        service=f"addresses/{address}/decode",
         api_key=api_key,
     )
 
     try:
         return response["staking_cred"]["reward_address"]
     except:
         return address
 
 
-def get_pool_information(pool_id: str, api_key: str) -> dict:
-    check_str(pool_id, "gomaestro.pool_id")
+def get_pool_information(pool_id: str, api_key: str = None) -> dict:
+    check_str(pool_id, "gomaestroorg.pool_id")
 
     pool_id = pool_id.strip().lower()
 
     response, status_code = get(
-        f"pools/{pool_id}/info",
+        service=f"pools/{pool_id}/info",
         api_key=api_key,
     )
 
     return response["data"]
 
 
-def get_pool_delegators(pool_id: str, api_key: str) -> Iterable[Tuple[str, float]]:
-    check_str(pool_id, "gomaestro.pool_id")
+def get_pool_delegators(pool_id: str, api_key: str = None) -> Iterable[Tuple[str, float]]:
+    check_str(pool_id, "gomaestroorg.pool_id")
 
     pool_id = pool_id.strip().lower()
 
     cursor = None
 
     while True:
         response, status_code = get(
-            f"pools/{pool_id}/delegators",
+            service=f"pools/{pool_id}/delegators",
             params={
                 "cursor": cursor,
             },
             api_key=api_key,
         )
 
         for item in response.get("data", []):
@@ -213,16 +220,16 @@
         cursor = response.get("next_cursor")
 
         if not cursor:
             break
 
 
 @lru_cache(maxsize=None)
-def get_handle(stake_address: str, api_key: str) -> str:
-    check_str(stake_address, "gomaestro.stake_address")
+def get_handle(stake_address: str, api_key: str = None) -> str:
+    check_str(stake_address, "gomaestroorg.stake_address")
 
     handles = []
 
     for holding in get_account_assets(stake_address, api_key=api_key, policy_id=ADA_HANDLE_POLICY_ID):
         asset_id = holding["unit"]
         asset_id = asset_id.replace(f"{ADA_HANDLE_POLICY_ID}000de140", "")  # CIP-68
         asset_id = asset_id.replace(ADA_HANDLE_POLICY_ID, "")  # CIP-25
@@ -233,16 +240,16 @@
     if not handles:
         return None
 
     return sorted(handles, key=len)[0]
 
 
 @lru_cache(maxsize=None)
-def resolve_handle(handle: str, api_key: str) -> str:
-    check_str(handle, "gomaestro.handle")
+def resolve_handle(handle: str, api_key: str = None) -> str:
+    check_str(handle, "gomaestroorg.handle")
 
     if handle.startswith("$"):
         if handle.startswith("$"):
             handle = handle[1:]
 
     handle = handle.lower()
 
@@ -250,16 +257,16 @@
 
     if wallet:
         return wallet
 
     return resolve_cip68_handle(handle, api_key)
 
 
-def resolve_cip25_handle(handle: str, api_key: str) -> str:
-    check_str(handle, "gomaestro.handle")
+def resolve_cip25_handle(handle: str, api_key: str = None) -> str:
+    check_str(handle, "gomaestroorg.handle")
 
     encoded_name = base64.b16encode(handle.encode()).decode("utf-8")
 
     asset_id = f"{ADA_HANDLE_POLICY_ID}{encoded_name}".lower()
     owners = list(get_asset_owners(asset_id, api_key))
 
     if not owners:
@@ -267,16 +274,16 @@
 
     owner = owners[0]
     owner["cip"] = 25
 
     return owner
 
 
-def resolve_cip68_handle(handle: str, api_key: str) -> str:
-    check_str(handle, "gomaestro.handle")
+def resolve_cip68_handle(handle: str, api_key: str = None) -> str:
+    check_str(handle, "gomaestroorg.handle")
 
     encoded_name = base64.b16encode(handle.encode()).decode("utf-8")
 
     asset_id = f"{ADA_HANDLE_POLICY_ID}000de140{encoded_name}".lower()
     owners = list(get_asset_owners(asset_id, api_key))
 
     if not owners:
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/cardano/jpgstore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import logging
+import os
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = "https://server.jpgstoreapis.com"
+BASE_URL = os.getenv(
+    "JPGSTORE_BASE_URL",
+    "https://server.jpgstoreapis.com",
+)
+
 
 logger = logging.getLogger(__name__)
 
 
 def get(service: str, params: dict = None, headers: dict = None) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/{service}",
@@ -27,15 +32,15 @@
     while True:
         params = {}
 
         if cursor:
             params["cursor"] = cursor
 
         response, status_code = get(
-            f"policy/{policy_id}/listings",
+            service=f"policy/{policy_id}/listings",
             params=params,
         )
 
         cursor = response.get("nextPageCursor")
 
         if not cursor:  # pragma: no cover
             break
@@ -49,15 +54,15 @@
 
     txs = set()
 
     last_date = ""
 
     while True:
         response, status_code = get(
-            f"collection/{policy_id}/v2/transactions",
+            service=f"collection/{policy_id}/v2/transactions",
             params={
                 "lastDate": last_date,
                 "count": 50,
             },
             headers={
                 "x-jpgstore-csrf-protection": "1",
             },
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/coingeckocom.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,102 @@
 import logging
+import os
 import time
 from typing import Tuple
 
 from cachetools.func import ttl_cache
 
 from fetchfox import rest
 from fetchfox.constants.currencies import ALGO, ADA, BOOK, ETH, MATIC
 
-BASE_URL = "https://api.coingecko.com/api/v3"
-
 IDS = {
     ALGO: "algorand",
     ADA: "cardano",
     BOOK: "book-2",
     ETH: "ethereum",
     MATIC: "matic-network",
 }
 
+
+BASE_URL = os.environ.get(
+    "COINGECKOC_API_BASE_URL",
+    "https://api.coingecko.com/api/v3",
+)
+
+API_KEY = os.environ.get("COINGECKO_API_KEY")
+
 logger = logging.getLogger(__name__)
 
 
-def get(service: str, params: dict = None) -> Tuple[dict, int]:
+def get(service: str, params: dict = None, api_key: str = None) -> Tuple[dict, int]:
+    api_key = api_key or API_KEY
+
+    if api_key:
+        rate_limit = 30
+        headers = {
+            "x-cg-demo-api-key": api_key,
+        }
+    else:
+        rate_limit = 5
+        headers = {}
+
+    time.sleep(60 / rate_limit)
+
     return rest.get(
         url=f"{BASE_URL}/{service}",
+        headers=headers,
         params=params,
     )
 
 
 @ttl_cache(ttl=60 * 60)
-def get_currency_usd_exchange(currency: str):
-    time.sleep(5)
-
+def get_currency_usd_exchange(currency: str, api_key: str = None):
     currency = currency.strip().upper()
-
     id = IDS[currency]
 
     logger.info("fetching exchange for %s (%s)", currency, id)
 
     response, status_code = get(
         service="simple/price",
         params={
             "ids": id,
             "vs_currencies": "usd",
         },
+        api_key=api_key,
     )
 
     return response[id]["usd"]
 
 
 @ttl_cache(ttl=60 * 60)
-def get_currency_ath_usd(currency: str):
-    time.sleep(5)
-
+def get_currency_ath_usd(currency: str, api_key: str = None):
     currency = currency.strip().upper()
-
     id = IDS[currency]
 
     logger.info("fetching ath for %s (%s)", currency, id)
 
     response, status_code = get(
         service=f"coins/{id}",
+        api_key=api_key,
     )
 
     return response["market_data"]["ath"]["usd"]
 
 
-def get_currency_history(currency: str, days: int = 7):
+def get_currency_exchange_history(currency: str, days: int = 7, api_key: str = None):
     id = IDS[currency]
 
+    logger.info("fetching exchange history of %s (%s)", currency, id)
+
     response, status_code = get(
         service=f"coins/{id}/market_chart",
         params={
             "vs_currency": "usd",
             "days": days,
         },
+        api_key=api_key,
     )
 
     return response["prices"]
+
+
+get_currency_history = get_currency_exchange_history
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/evm/ensideascom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import logging
+import os
 from functools import lru_cache
 from typing import Tuple
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 
-BASE_URL = "https://api.ensideas.com"
+BASE_URL = os.getenv(
+    "ENSIDEAS_BASE_URL",
+    "https://api.ensideas.com",
+)
 
 logger = logging.getLogger(__name__)
 
 
 def get(service: str, params: dict = None) -> Tuple[dict, int]:
     return rest.get(
         url=f"{BASE_URL}/{service}",
@@ -17,31 +21,37 @@
     )
 
 
 @lru_cache(maxsize=None)
 def resolve_ens_domain(ens_domain: str):
     check_str(ens_domain)
 
-    response, status_code = get(f"ens/resolve/{ens_domain}")
+    response, status_code = get(
+        service=f"ens/resolve/{ens_domain}",
+    )
 
     address = response.get("address")
 
     if not address:
         return None
 
     logger.info("resolved %s to %s", ens_domain, address)
+
     return address
 
 
 @lru_cache(maxsize=None)
 def get_ens_domain(address: str):
     check_str(address)
 
-    response, status_code = get(f"ens/resolve/{address}")
+    response, status_code = get(
+        service=f"ens/resolve/{address}",
+    )
 
     ens_domain = response.get("name")
 
     if not ens_domain:
         return None
 
     logger.info("resolved %s to %s", address, ens_domain)
+
     return ens_domain
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/evm/moralisio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 import json
 import logging
+import os
 from functools import lru_cache
 from typing import Iterable, Tuple
 
 from fetchfox import rest
 from fetchfox.apis import pinatacloud
 from fetchfox.checks import check_str
 
-BASE_URL = "https://deep-index.moralis.io/api"
+BASE_URL = os.getenv(
+    "MORALIS_BASE_URL",
+    "https://deep-index.moralis.io/api",
+)
+
+API_KEY = os.getenv("MORALIS_API_KEY")
 
 logger = logging.getLogger(__name__)
 
 
-def get(service: str, blockchain: str, api_key: str, params: dict = None, version: int = 2) -> Tuple[dict, int]:
-    check_str(blockchain, "moralisio.blockchain")
+def get(service: str, blockchain: str, params: dict = None, version: int = 2, api_key: str = None) -> Tuple[dict, int]:
+    api_key = api_key or API_KEY
+
     check_str(api_key, "moralisio.api_key")
+    check_str(blockchain, "moralisio.blockchain")
 
     params = params or {}
     params["chain"] = "eth" if blockchain == "ethereum" else blockchain
 
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         params=params,
         headers={
             "X-API-Key": api_key,
             "Host": "deep-index.moralis.io",
         },
     )
 
 
-def get_account_balance(address: str, blockchain: str, api_key: str) -> Iterable[dict]:
+def get_account_balance(address: str, blockchain: str, api_key: str = None) -> Iterable[dict]:
     check_str(address, "moralisio.address")
     address = address.strip().lower()
 
     response, status_code = get(
-        f"{address}/balance",
+        service=f"{address}/balance",
         blockchain=blockchain,
         api_key=api_key,
     )
 
     return int(response["balance"]) / 10**18
 
 
-def get_account_assets(address: str, blockchain: str, api_key: str) -> Iterable[dict]:
+def get_account_assets(address: str, blockchain: str, api_key: str = None) -> Iterable[dict]:
     check_str(address, "moralisio.address")
     address = address.strip().lower()
 
     cursor = ""
 
     while True:
         response, status_code = get(
-            f"{address}/nft",
+            service=f"{address}/nft",
             params={
                 "cursor": cursor,
             },
             blockchain=blockchain,
             api_key=api_key,
         )
 
@@ -63,21 +71,21 @@
         if not response.get("cursor"):
             break
 
         cursor = response["cursor"]
 
 
 @lru_cache(maxsize=None)
-def get_asset_data(contract_address: str, asset_id: str, blockchain: str, api_key: str) -> dict:
+def get_asset_data(contract_address: str, asset_id: str, blockchain: str, api_key: str = None) -> dict:
     check_str(contract_address, "moralisio.contract_address")
     check_str(asset_id, "moralisio.asset_id")
     contract_address = contract_address.strip().lower()
 
     response, status_code = get(
-        f"nft/{contract_address}/{asset_id}",
+        service=f"nft/{contract_address}/{asset_id}",
         blockchain=blockchain,
         api_key=api_key,
     )
 
     if status_code == 404:
         raise Exception(f"{contract_address}/{asset_id} doesn't exist")
 
@@ -93,64 +101,67 @@
 
     metadata["attributes"].update(metadata["extraAttributes"])
     response["metadata"] = metadata
 
     return response
 
 
-def resync_asset_metadata(contract_address: str, asset_id: str, blockchain: str, api_key: str):
+def resync_asset_metadata(contract_address: str, asset_id: str, blockchain: str, api_key: str = None):
     check_str(contract_address, "moralisio.contract_address")
     check_str(asset_id, "moralisio.asset_id")
+
     contract_address = contract_address.strip().lower()
 
     response, status_code = get(
-        f"nft/{contract_address}/{asset_id}/metadata/resync",
+        service=f"nft/{contract_address}/{asset_id}/metadata/resync",
         params={
             "flag": "uri",
             "mode": "sync",
         },
         blockchain=blockchain,
         api_key=api_key,
     )
 
     if status_code == 404:
         raise ValueError(f"{contract_address}/{asset_id} doesn't exist")
 
     return response.get("status")
 
 
-def get_asset_owner(contract_address: str, asset_id: str, blockchain: str, api_key: str) -> dict:
+def get_asset_owner(contract_address: str, asset_id: str, blockchain: str, api_key: str = None) -> dict:
     check_str(contract_address, "moralisio.contract_address")
     check_str(asset_id, "moralisio.asset_id")
+
     contract_address = contract_address.strip().lower()
 
     response, status_code = get(
-        f"nft/{contract_address}/{asset_id}/owners",
+        service=f"nft/{contract_address}/{asset_id}/owners",
         blockchain=blockchain,
         api_key=api_key,
     )
 
     for holding in response["result"]:
         return {
             "contract_address": holding["token_address"],
             "asset_id": holding["token_id"],
             "address": holding["owner_of"],
             "amount": holding["amount"],
         }
 
 
-def get_collection_assets(contract_address: str, blockchain: str, api_key: str) -> Iterable[dict]:
+def get_collection_assets(contract_address: str, blockchain: str, api_key: str = None) -> Iterable[dict]:
     check_str(contract_address, "moralisio.contract_address")
+
     contract_address = contract_address.strip().lower()
 
     cursor = ""
 
     while True:
         response, status_code = get(
-            f"nft/{contract_address}",
+            service=f"nft/{contract_address}",
             params={
                 "cursor": cursor,
                 "format": "decimal",
                 "normalizeMetadata": "false",
             },
             blockchain=blockchain,
             api_key=api_key,
@@ -161,23 +172,24 @@
 
         if not response.get("cursor"):
             break
 
         cursor = response["cursor"]
 
 
-def get_collection_owners(contract_address: str, blockchain: str, api_key: str) -> Iterable[dict]:
+def get_collection_owners(contract_address: str, blockchain: str, api_key: str = None) -> Iterable[dict]:
     check_str(contract_address, "moralisio.contract_address")
+
     contract_address = contract_address.strip().lower()
 
     cursor = ""
 
     while True:
         response, status_code = get(
-            f"nft/{contract_address}/owners",
+            service=f"nft/{contract_address}/owners",
             params={
                 "cursor": cursor,
             },
             blockchain=blockchain,
             api_key=api_key,
         )
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-2.5.0/fetchfox/apis/evm/openseaio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import logging
+import os
 from functools import lru_cache
 from typing import Tuple, Iterable
 
 from fetchfox import rest
 from fetchfox.checks import check_str
 from fetchfox.constants.blockchains import ETHEREUM, POLYGON
 
-BASE_URL = "https://api.opensea.io"
+BASE_URL = os.getenv(
+    "OPENSEA_BASE_URL",
+    "https://api.opensea.io",
+)
+
+API_KEY = os.getenv("OPENSEA_API_KEY")
 
 BLOCKCHAINS = {
     ETHEREUM: "ethereum",
     POLYGON: "matic",
 }
 
 logger = logging.getLogger(__name__)
 
 
-def get(service: str, api_key: str, params: dict = None, version: int = 2, check: str = None) -> Tuple[dict, int]:
+def get(service: str, params: dict = None, version: int = 2, check: str = None, api_key: str = None) -> Tuple[dict, int]:
+    api_key = api_key or API_KEY
+
     check_str(api_key, "openseaio.api_key")
 
     if version == 1:
         url = f"{BASE_URL}/api/v{version}/{service}"
     else:
         url = f"{BASE_URL}/v{version}/{service}"
 
@@ -32,46 +40,46 @@
         params=params,
         sleep=2.5,
         check=check,
     )
 
 
 @lru_cache(maxsize=None)
-def get_collection_slug(contract_address: str, blockchain: str, api_key: str) -> str:
+def get_collection_slug(contract_address: str, blockchain: str, api_key: str = None) -> str:
     check_str(contract_address, "openseaio.contract_address")
     check_str(blockchain, "openseaio.blockchain")
 
     contract_address = contract_address.strip().lower()
     blockchain: str = BLOCKCHAINS.get(blockchain, blockchain)
 
     logger.info("fetching slug for %s (%s)", contract_address, blockchain)
 
     response, status_code = get(
-        f"chain/{blockchain}/contract/{contract_address}",
+        service=f"chain/{blockchain}/contract/{contract_address}",
         api_key=api_key,
         check="collection",
     )
 
     return response["collection"]
 
 
-def get_collection_sales(contract_address: str, blockchain: str, api_key: str, slug: str = None) -> Iterable[dict]:
+def get_collection_sales(contract_address: str, blockchain: str, slug: str = None, api_key: str = None) -> Iterable[dict]:
     check_str(contract_address, "openseaio.contract_address")
     check_str(blockchain, "openseaio.blockchain")
 
     contract_address = contract_address.strip().lower()
 
     if not slug:
         slug = get_collection_slug(contract_address, blockchain, api_key=api_key)
 
     cursor = ""
 
     while True:
         response, status_code = get(
-            f"events/collection/{slug}",
+            service=f"events/collection/{slug}",
             params={
                 "event_type": "sale",
                 "next": cursor,
             },
             api_key=api_key,
         )
 
@@ -83,28 +91,28 @@
 
         cursor = response.get("next")
 
         if not cursor:
             break
 
 
-def get_collection_listings(contract_address: str, blockchain: str, api_key: str, slug: str = None) -> Iterable[dict]:
+def get_collection_listings(contract_address: str, blockchain: str, slug: str = None, api_key: str = None) -> Iterable[dict]:
     check_str(contract_address, "openseaio.contract_address")
     check_str(blockchain, "openseaio.blockchain")
 
     contract_address = contract_address.strip().lower()
 
     if not slug:
         slug = get_collection_slug(contract_address, blockchain, api_key=api_key)
 
     cursor = ""
 
     while True:
         response, status_code = get(
-            f"listings/collection/{slug}/all",
+            service=f"listings/collection/{slug}/all",
             params={
                 "next": cursor,
             },
             api_key=api_key,
         )
 
         yield from response.get("listings", [])
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/algorand/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/algorand/exceptions.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/algorand/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/base.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/cardano/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/cardano/exceptions.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/cardano/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/ethereum/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/evm/blockchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import logging
 from datetime import datetime
 from typing import Iterable, Tuple, List
 
 import pytz
 
 from fetchfox.apis import bookio
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/evm/exceptions.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/evm/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/blockchains/polygon/blockchain.py` & `bookio_fetchfox-2.5.0/fetchfox/blockchains/polygon/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/constants/ranks.py` & `bookio_fetchfox-2.5.0/fetchfox/constants/ranks.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/dtos/asset.py` & `bookio_fetchfox-2.5.0/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/dtos/campaign.py` & `bookio_fetchfox-2.5.0/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/dtos/listing.py` & `bookio_fetchfox-2.5.0/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/dtos/order.py` & `bookio_fetchfox-2.5.0/fetchfox/dtos/order.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/dtos/pair_stats.py` & `bookio_fetchfox-2.5.0/fetchfox/dtos/pair_stats.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/dtos/sale.py` & `bookio_fetchfox-2.5.0/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/pools/book_pool.py` & `bookio_fetchfox-2.5.0/fetchfox/pools/book_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from fetchfox.constants.book import BOOK_POOL_TICKER, BOOK_POOL_ID
 
 
 class BookPool:
     id = BOOK_POOL_ID
     ticker = BOOK_POOL_TICKER
 
-    def __init__(self, maestro_api_key: str):
+    def __init__(self, maestro_api_key: str = None):
         self.maestro_api_key = maestro_api_key
 
     @property
     def delegated_amount(self) -> float:
         info = gomaestroorg.get_pool_information(
             self.id,
             api_key=self.maestro_api_key,
@@ -36,8 +36,11 @@
             api_key=self.maestro_api_key,
         )
 
         return float(info["live_saturation"])
 
     @property
     def delegators(self) -> Iterable[Tuple[str, float]]:
-        yield from gomaestroorg.get_pool_delegators(self.id, api_key=self.maestro_api_key)
+        yield from gomaestroorg.get_pool_delegators(
+            self.id,
+            api_key=self.maestro_api_key,
+        )
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/rest.py` & `bookio_fetchfox-2.5.0/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/tokens/base.py` & `bookio_fetchfox-2.5.0/fetchfox/tokens/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Iterable, List, Tuple
 
 from cachetools.func import ttl_cache
 
 from fetchfox.apis import coingeckocom
 from fetchfox.apis import price
-from fetchfox.apis.cardano import cexplorerio, dexhunterio
+from fetchfox.apis.cardano import dexhunterio
 from fetchfox.constants.currencies import ADA
 from fetchfox.dtos import CardanoOrderDTO, OrderType, PairStatsDTO, StatsDTO
 
 
 class CardanoToken:
     def __init__(
         self,
@@ -75,20 +75,14 @@
         return f"https://app.minswap.org/swap?currencySymbolA={self.policy_id}&tokenNameA={self.asset_name}&currencySymbolB=&tokenNameB="
 
     @property
     def taptools_url(self):
         return f"https://www.taptools.io/charts/token/0be55d262b29f564998ff81efe21bdc0022621c12f15af08d0f2ddb1.{self.taptools_pair_id}"
 
     @property
-    def owners(self) -> Tuple[int, int]:
-        tx = cexplorerio.get_asset_detail(self.fingerprint)
-
-        return tx["epoch"], tx["owners_acc"]
-
-    @property
     def pair_stats(self) -> PairStatsDTO:
         stats = dexhunterio.get_asset_pair_stats(
             self.asset_id,
             partner_code=self.dexhunter_partner_code,
         )
 
         stats_dto = StatsDTO(
```

### Comparing `bookio_fetchfox-2.4.6/fetchfox/tokens/beard_token.py` & `bookio_fetchfox-2.5.0/fetchfox/tokens/beard_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/tokens/book_token.py` & `bookio_fetchfox-2.5.0/fetchfox/tokens/book_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/fetchfox/tokens/hosky_token.py` & `bookio_fetchfox-2.5.0/fetchfox/tokens/hosky_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.4.6/pyproject.toml` & `bookio_fetchfox-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "2.4.6"
+version = "2.5.0"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-2.4.6/setup.py` & `bookio_fetchfox-2.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'asyncio>=3.4.3,<4.0.0',
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '2.4.6',
+    'version': '2.5.0',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand(\n    nftexplorerapp_api_key=os.getenv("NFTEXPLORER_API_KEY"),\n)\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    blockfrostio_project_id=os.getenv("BLOCKFROST_PROJECT_ID"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_collection_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([blockfrost.io²](https://blockfrost.io))\n* get_assets ([blockfrost.io²](https://blockfrost.io))\n* get_holdings ([blockfrost.io²](https://blockfrost.io))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([blockfrost.io²](https://blockfrost.io))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n* get_ranks ([cnft.tools](https://cnft.tools))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** services require an [api key](https://www.nftexplorer.app/nftx-api).\n> \n> ² **blockfrost.io** services require a [project id](https://blockfrost.dev/docs/overview/plans-and-billing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-2.4.6/PKG-INFO` & `bookio_fetchfox-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 2.4.6
+Version: 2.5.0
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```


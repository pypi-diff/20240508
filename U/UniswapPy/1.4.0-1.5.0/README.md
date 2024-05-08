# Comparing `tmp/uniswappy-1.4.0.tar.gz` & `tmp/uniswappy-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniswappy-1.4.0.tar", last modified: Wed May  1 19:05:50 2024, max compression
+gzip compressed data, was "uniswappy-1.5.0.tar", last modified: Wed May  8 21:49:24 2024, max compression
```

## Comparing `uniswappy-1.4.0.tar` & `uniswappy-1.5.0.tar`

### file list

```diff
@@ -1,133 +1,136 @@
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.539687 uniswappy-1.4.0/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 uniswappy-1.4.0/LICENSE.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-01 19:05:50.539627 uniswappy-1.4.0/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     4341 2024-05-01 19:05:23.000000 uniswappy-1.4.0/README.md
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.539382 uniswappy-1.4.0/UniswapPy.egg-info/
--rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     3635 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/SOURCES.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/dependency_links.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 uniswappy-1.4.0/UniswapPy.egg-info/not-zip-safe
--rw-r--r--   0 ian_moore   (501) staff       (20)       30 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/requires.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/top_level.txt
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.518165 uniswappy-1.4.0/python/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.524136 uniswappy-1.4.0/python/prod/
--rw-r--r--   0 ian_moore   (501) staff       (20)      917 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.518593 uniswappy-1.4.0/python/prod/cpt/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.525171 uniswappy-1.4.0/python/prod/cpt/exchg/
--rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/exchg/ChildUniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    21859 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/exchg/UniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    42515 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/exchg/UniswapV3Exchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      148 2024-04-23 22:24:39.000000 uniswappy-1.4.0/python/prod/cpt/exchg/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.525613 uniswappy-1.4.0/python/prod/cpt/factory/
--rw-r--r--   0 ian_moore   (501) staff       (20)     4208 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/factory/UniswapFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 uniswappy-1.4.0/python/prod/cpt/factory/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.526215 uniswappy-1.4.0/python/prod/cpt/index/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2508 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/index/RebaseIndexToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2485 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/index/SettlementLPToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/cpt/index/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.527111 uniswappy-1.4.0/python/prod/cpt/quote/
--rw-r--r--   0 ian_moore   (501) staff       (20)     6933 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/quote/IndexTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6973 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/quote/LPQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/quote/LPTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/quote/TreeAmountQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/cpt/quote/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.527574 uniswappy-1.4.0/python/prod/cpt/vault/
--rw-r--r--   0 ian_moore   (501) staff       (20)    15304 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/vault/IndexVault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/vault/Vault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/cpt/vault/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.527918 uniswappy-1.4.0/python/prod/cpt/wallet/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/wallet/Wallets.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/cpt/wallet/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.528874 uniswappy-1.4.0/python/prod/erc/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1664 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/erc/DOAERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1441 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/erc/ERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1088 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/erc/IndexERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1700 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/erc/LPERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/erc/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.519066 uniswappy-1.4.0/python/prod/math/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.529368 uniswappy-1.4.0/python/prod/math/basic/
--rw-r--r--   0 ian_moore   (501) staff       (20)      500 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/basic/IDGenerator.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/basic/RoundFloat.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/basic/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.529835 uniswappy-1.4.0/python/prod/math/interest/
--rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/interest/CompoundReturn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/interest/Yield.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.530272 uniswappy-1.4.0/python/prod/math/interest/ips/
--rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/ConstantIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/IPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.530584 uniswappy-1.4.0/python/prod/math/interest/ips/aggregate/
--rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/aggregate/AggregateIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/aggregate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.531421 uniswappy-1.4.0/python/prod/math/model/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/BrownianModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/EventSelectionModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/ModelQueue.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/TimeDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/TokenDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/model/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.531751 uniswappy-1.4.0/python/prod/math/risk/
--rw-r--r--   0 ian_moore   (501) staff       (20)     5551 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/math/risk/MaxDrop.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/risk/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.532020 uniswappy-1.4.0/python/prod/process/
--rw-r--r--   0 ian_moore   (501) staff       (20)      301 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/Process.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.532446 uniswappy-1.4.0/python/prod/process/burn/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2465 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/burn/IndexTokenBurn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/burn/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.532745 uniswappy-1.4.0/python/prod/process/deposit/
--rw-r--r--   0 ian_moore   (501) staff       (20)     5363 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/deposit/SwapDeposit.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/deposit/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.533020 uniswappy-1.4.0/python/prod/process/join/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1650 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/join/Join.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/join/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.533427 uniswappy-1.4.0/python/prod/process/liquidity/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3527 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/liquidity/AddLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3200 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/liquidity/RemoveLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/liquidity/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.533688 uniswappy-1.4.0/python/prod/process/mint/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2737 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/mint/SwapIndexMint.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/mint/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.534270 uniswappy-1.4.0/python/prod/process/swap/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2319 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/swap/RandomSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2566 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/swap/Swap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     5632 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/swap/WithdrawSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/swap/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.535795 uniswappy-1.4.0/python/prod/simulate/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/simulate/Arbitrage.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4185 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/simulate/CorrectReserves.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/simulate/MarkovState.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    15429 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/simulate/QuantTerminal.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/simulate/SimpleLPSimulation.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1850 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/simulate/SolveDeltas.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      244 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/simulate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.519920 uniswappy-1.4.0/python/prod/utils/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.536202 uniswappy-1.4.0/python/prod/utils/client/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2164 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/utils/client/API0x.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       24 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/utils/client/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.537019 uniswappy-1.4.0/python/prod/utils/data/
--rw-r--r--   0 ian_moore   (501) staff       (20)    10464 2024-04-25 01:17:59.000000 uniswappy-1.4.0/python/prod/utils/data/Chain0x.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/utils/data/ExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/utils/data/FactoryData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      628 2024-04-23 22:24:39.000000 uniswappy-1.4.0/python/prod/utils/data/UniswapExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/utils/data/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.537411 uniswappy-1.4.0/python/prod/utils/interfaces/
--rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/utils/interfaces/IExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/utils/interfaces/IExchangeFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 uniswappy-1.4.0/python/prod/utils/interfaces/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.519965 uniswappy-1.4.0/python/prod/utils/tools/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.539202 uniswappy-1.4.0/python/prod/utils/tools/v3/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1331 2024-04-25 02:27:11.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/FullMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      844 2024-04-25 02:27:11.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/LiquidityMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4659 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/Position.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1928 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/SafeMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6201 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/Shared.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    10496 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/SqrtPriceMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4961 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/SwapMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     7724 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/Tick.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6407 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/TickMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     7573 2024-04-25 02:27:11.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/UniV3Utils.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      266 2024-04-25 02:27:11.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/__init__.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-05-01 19:05:50.539978 uniswappy-1.4.0/setup.cfg
--rw-r--r--   0 ian_moore   (501) staff       (20)     1537 2024-05-01 19:05:23.000000 uniswappy-1.4.0/setup.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.811194 uniswappy-1.5.0/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 uniswappy-1.5.0/LICENSE.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-08 21:49:24.811128 uniswappy-1.5.0/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4341 2024-05-01 19:05:23.000000 uniswappy-1.5.0/README.md
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.810878 uniswappy-1.5.0/UniswapPy.egg-info/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3752 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/SOURCES.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/dependency_links.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 uniswappy-1.5.0/UniswapPy.egg-info/not-zip-safe
+-rw-r--r--   0 ian_moore   (501) staff       (20)       30 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/requires.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-05-08 21:49:24.000000 uniswappy-1.5.0/UniswapPy.egg-info/top_level.txt
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.770417 uniswappy-1.5.0/python/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.773645 uniswappy-1.5.0/python/prod/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      953 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.770841 uniswappy-1.5.0/python/prod/cpt/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.774871 uniswappy-1.5.0/python/prod/cpt/exchg/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/exchg/ChildUniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    21851 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/exchg/UniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    42402 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/exchg/UniswapV3Exchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      148 2024-04-23 22:24:39.000000 uniswappy-1.5.0/python/prod/cpt/exchg/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.775546 uniswappy-1.5.0/python/prod/cpt/factory/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4208 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/cpt/factory/UniswapFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 uniswappy-1.5.0/python/prod/cpt/factory/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.776015 uniswappy-1.5.0/python/prod/cpt/index/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3366 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/index/RebaseIndexToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3462 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/index/SettlementLPToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-05-07 01:41:36.000000 uniswappy-1.5.0/python/prod/cpt/index/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.777189 uniswappy-1.5.0/python/prod/cpt/quote/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6933 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/cpt/quote/IndexTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7081 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/cpt/quote/LPQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/quote/LPTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/quote/TreeAmountQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/cpt/quote/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.777726 uniswappy-1.5.0/python/prod/cpt/vault/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15304 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/cpt/vault/IndexVault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/vault/Vault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/cpt/vault/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.778077 uniswappy-1.5.0/python/prod/cpt/wallet/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/cpt/wallet/Wallets.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-05-07 02:47:23.000000 uniswappy-1.5.0/python/prod/cpt/wallet/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.779011 uniswappy-1.5.0/python/prod/erc/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1664 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/erc/DOAERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1441 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/erc/ERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1088 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/erc/IndexERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1700 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/erc/LPERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/erc/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.771321 uniswappy-1.5.0/python/prod/math/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.779878 uniswappy-1.5.0/python/prod/math/basic/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      494 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/math/basic/IDGenerator.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/basic/RoundFloat.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/basic/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.780571 uniswappy-1.5.0/python/prod/math/interest/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/interest/CompoundReturn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/interest/Yield.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.781689 uniswappy-1.5.0/python/prod/math/interest/ips/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/ConstantIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/IPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.800009 uniswappy-1.5.0/python/prod/math/interest/ips/aggregate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/aggregate/AggregateIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/interest/ips/aggregate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.801153 uniswappy-1.5.0/python/prod/math/model/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/BrownianModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/EventSelectionModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/ModelQueue.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/TimeDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/model/TokenDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/math/model/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.801674 uniswappy-1.5.0/python/prod/math/risk/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     5551 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/math/risk/MaxDrop.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/math/risk/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.801972 uniswappy-1.5.0/python/prod/process/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      301 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/Process.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.802361 uniswappy-1.5.0/python/prod/process/burn/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2465 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/burn/IndexTokenBurn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/burn/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.802879 uniswappy-1.5.0/python/prod/process/deposit/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7051 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/process/deposit/SwapDeposit.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/deposit/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.803280 uniswappy-1.5.0/python/prod/process/join/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1870 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/process/join/Join.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/join/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.803751 uniswappy-1.5.0/python/prod/process/liquidity/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3611 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/process/liquidity/AddLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3200 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/liquidity/RemoveLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/liquidity/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.804052 uniswappy-1.5.0/python/prod/process/mint/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2737 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/mint/SwapIndexMint.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/mint/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.804659 uniswappy-1.5.0/python/prod/process/swap/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2319 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/swap/RandomSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2566 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/process/swap/Swap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     5338 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/process/swap/WithdrawSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 uniswappy-1.5.0/python/prod/process/swap/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.806022 uniswappy-1.5.0/python/prod/simulate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/simulate/Arbitrage.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4973 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/simulate/CorrectReserves.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/simulate/MarkovState.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15429 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/simulate/QuantTerminal.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/simulate/SimpleLPSimulation.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2229 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/simulate/SolveDeltas.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      244 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/simulate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.772086 uniswappy-1.5.0/python/prod/utils/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.806343 uniswappy-1.5.0/python/prod/utils/client/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2164 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/utils/client/API0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       24 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/utils/client/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.807287 uniswappy-1.5.0/python/prod/utils/data/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    10464 2024-04-25 01:17:59.000000 uniswappy-1.5.0/python/prod/utils/data/Chain0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/utils/data/ExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/utils/data/FactoryData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      628 2024-04-23 22:24:39.000000 uniswappy-1.5.0/python/prod/utils/data/UniswapExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-04-10 18:17:44.000000 uniswappy-1.5.0/python/prod/utils/data/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.807819 uniswappy-1.5.0/python/prod/utils/interfaces/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/utils/interfaces/IExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 uniswappy-1.5.0/python/prod/utils/interfaces/IExchangeFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 uniswappy-1.5.0/python/prod/utils/interfaces/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.808254 uniswappy-1.5.0/python/prod/utils/tools/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      725 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/utils/tools/MockAddress.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/utils/tools/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-08 21:49:24.810674 uniswappy-1.5.0/python/prod/utils/tools/v3/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1331 2024-04-25 02:27:11.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/FullMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      844 2024-04-25 02:27:11.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/LiquidityMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4659 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/Position.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1928 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/SafeMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6201 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/Shared.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    10496 2024-05-01 19:05:23.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/SqrtPriceMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4961 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/SwapMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7724 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/Tick.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6407 2024-04-24 18:20:10.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/TickMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3208 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/UniV3Helper.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7573 2024-04-25 02:27:11.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/UniV3Utils.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      303 2024-05-08 21:48:13.000000 uniswappy-1.5.0/python/prod/utils/tools/v3/__init__.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-05-08 21:49:24.811432 uniswappy-1.5.0/setup.cfg
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1572 2024-05-08 21:48:13.000000 uniswappy-1.5.0/setup.py
```

### Comparing `uniswappy-1.4.0/LICENSE.txt` & `uniswappy-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/PKG-INFO` & `uniswappy-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniswapPy
-Version: 1.4.0
+Version: 1.5.0
 Summary: Uniswap Analytics with Python
 Home-page: https://github.com/defipy-devs/uniswappy
 Author: icmoore
 Author-email: defipy.devs@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `uniswappy-1.4.0/README.md` & `uniswappy-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/UniswapPy.egg-info/PKG-INFO` & `uniswappy-1.5.0/UniswapPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniswapPy
-Version: 1.4.0
+Version: 1.5.0
 Summary: Uniswap Analytics with Python
 Home-page: https://github.com/defipy-devs/uniswappy
 Author: icmoore
 Author-email: defipy.devs@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `uniswappy-1.4.0/UniswapPy.egg-info/SOURCES.txt` & `uniswappy-1.5.0/UniswapPy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,21 @@
 python/prod/utils/data/ExchangeData.py
 python/prod/utils/data/FactoryData.py
 python/prod/utils/data/UniswapExchangeData.py
 python/prod/utils/data/__init__.py
 python/prod/utils/interfaces/IExchange.py
 python/prod/utils/interfaces/IExchangeFactory.py
 python/prod/utils/interfaces/__init__.py
+python/prod/utils/tools/MockAddress.py
+python/prod/utils/tools/__init__.py
 python/prod/utils/tools/v3/FullMath.py
 python/prod/utils/tools/v3/LiquidityMath.py
 python/prod/utils/tools/v3/Position.py
 python/prod/utils/tools/v3/SafeMath.py
 python/prod/utils/tools/v3/Shared.py
 python/prod/utils/tools/v3/SqrtPriceMath.py
 python/prod/utils/tools/v3/SwapMath.py
 python/prod/utils/tools/v3/Tick.py
 python/prod/utils/tools/v3/TickMath.py
+python/prod/utils/tools/v3/UniV3Helper.py
 python/prod/utils/tools/v3/UniV3Utils.py
 python/prod/utils/tools/v3/__init__.py
```

### Comparing `uniswappy-1.4.0/python/prod/__init__.py` & `uniswappy-1.5.0/python/prod/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 from uniswappy.process.mint import *
 from uniswappy.process.swap import *
 from uniswappy.process.join import *
 from uniswappy.simulate import *
 from uniswappy.utils.interfaces import *
 from uniswappy.utils.data import *
 from uniswappy.utils.client import *
+from uniswappy.utils.tools import *
 from uniswappy.utils.tools.v3 import *
```

### Comparing `uniswappy-1.4.0/python/prod/cpt/exchg/ChildUniswapExchange.py` & `uniswappy-1.5.0/python/prod/cpt/exchg/ChildUniswapExchange.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/cpt/exchg/UniswapExchange.py` & `uniswappy-1.5.0/python/prod/cpt/exchg/UniswapExchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,15 +566,15 @@
             Get price of select token in the exchange pair
                 
             Parameters
             -----------------
             token : ERC20
                 ERC20 token                
         """          
-        
+
         if(token.token_name == self.token0):
             if(self.reserve0 == 0):
                 return None 
             else:
                 return self.reserve1/self.reserve0 
         elif(token.token_name == self.token1):
             if(self.reserve1 == 0):
```

### Comparing `uniswappy-1.4.0/python/prod/cpt/exchg/UniswapV3Exchange.py` & `uniswappy-1.5.0/python/prod/cpt/exchg/UniswapV3Exchange.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ...erc import LPERC20
 from ...utils.interfaces import IExchange
 from ...utils.data import FactoryData
 from ...utils.data import UniswapExchangeData
 from ...utils.tools.v3.Shared import *
 from ...utils.tools.v3 import Position, Tick, SqrtPriceMath, LiquidityMath
 from ...utils.tools.v3 import SwapMath, TickMath, SafeMath, FullMath, UniV3Utils
+from ...utils.tools.v3 import UniV3Helper
 
 MINIMUM_LIQUIDITY = 1e-15
 GWEI_PRECISION = 18
 
 @dataclass
 class Slot0:
     ## the current price
@@ -117,15 +118,14 @@
         self.collected_fee0 = 0
         self.collected_fee1 = 0              
         self.name =  f"{self.token0}-{self.token1}"
         self.symbol = exchg_struct.symbol
         self.precision = exchg_struct.precision
         self.last_liquidity_deposit = 0
         self.total_supply = 0
-        self.tick_spacing = 1000
         self.slot0 = Slot0(0, 0, 0)
         self.positions = {}
         self.ticks = {}
         self.feeGrowthGlobal0X128 = 0
         self.feeGrowthGlobal1X128 = 0  
         self.protocolFees = ProtocolFees(0, 0)
         self.tickSpacing = exchg_struct.tick_spacing
@@ -139,20 +139,20 @@
         
         tokens = self.factory.token_from_exchange[self.name] 
         
         print(f"Exchange {self.name} ({self.symbol})")
 
         if (self.precision == UniswapExchangeData.TYPE_GWEI):
             print(f"Real Reserves:   {self.token0} = {self.reserve0}, {self.token1} = {self.reserve1}")
-            print(f"Virual Reserves: {self.token0} = {self.get_virtual_reserve(tokens[self.token0])}, {self.token1} = {self.get_virtual_reserve(tokens[self.token1])}")
-            print(f"Liquidity: {self.total_supply} \n")
+            print(f"Gross Liquidity: {self.total_supply} \n")
         else:  
-            print(f"Real Reserves:   {self.token0} = {self.gwei2dec(self.reserve0)}, {self.token1} = {self.gwei2dec(self.reserve1)}")
-            #print(f"Virual Reserves: {self.token0} = {self.get_virtual_reserve(tokens[self.token0])}, {self.token1} = {self.get_virtual_reserve(tokens[self.token1])}")
-            print(f"Liquidity: {self.gwei2dec(self.total_supply)} \n")            
+            res0 = UniV3Helper().gwei2dec(self.reserve0)
+            res1 = UniV3Helper().gwei2dec(self.reserve1)
+            print(f"Real Reserves:   {self.token0} = {res0}, {self.token1} = {res1}")
+            print(f"Gross Liquidity: {UniV3Helper().gwei2dec(self.total_supply)} \n")            
 
     def initialize(self, sqrtPriceX96):
 
         """ initialize
 
             Sets the initial price for the pool
                 
@@ -196,16 +196,15 @@
             Returns
             -------
             amount0 : float
                 Amount of token0 that was paid to mint the given amount of liquidity.   
             amount1 : float
                 Amount of token1 that was paid to mint the given amount of liquidity.                   
         """          
-
-        amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
+        amount = self._convert_to_machine(amount)
         
         checkInputTypes(
             accounts=(recipient), int24=(tickLower, tickUpper), uint128=(amount)
         )
         assert amount > 0
 
         (_, amount0Int, amount1Int) = self._modifyPosition(
@@ -228,16 +227,16 @@
         balanceB = tokens.get(self.token1).token_total
 
         self._update(balanceA, balanceB)
     
         assert balance0Before + amount0 <= tokens.get(self.token0).token_total, 'UniswapV3: M0' 
         assert balance1Before + amount1 <= tokens.get(self.token1).token_total, 'UniswapV3: M0' 
  
-        amount0 = self.convert(amount0)
-        amount1 = self.convert(amount1)        
+        amount0 = self._convert_to_human(amount0)
+        amount1 = self._convert_to_human(amount1)        
               
         return (amount0, amount1)
         
 
     def collect(self, recipient, tickLower, tickUpper, amount0Requested, amount1Requested):
 
         """ collect
@@ -265,19 +264,16 @@
             -------
             amount0 : float
                 Amount of token0 that was paid to mint the given amount of liquidity.   
             amount1 : float
                 Amount of token1 that was paid to mint the given amount of liquidity.                   
         """ 
 
-        amount0Requested = amount0Requested if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount0Requested)
-        amount1Requested = amount1Requested if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount1Requested)
-
-        print(f'amount0Requested {amount0Requested}')
-        print(f'amount1Requested {amount1Requested}')
+        amount0Requested = self._convert_to_machine(amount0Requested)
+        amount1Requested = self._convert_to_machine(amount1Requested)
         
         checkInputTypes(
             accounts=(recipient),
             int24=(tickLower, tickUpper),
             uint128=(amount0Requested, amount1Requested),
         )
         # Add this check to prevent creating a new position if the position doesn't exist or it's empty
@@ -304,16 +300,16 @@
             tokens.get(self.token0).deposit(recipient, amount0)
             #self.ledger.transferToken(self, recipient, self.token0, amount0)
         if amount1 > 0:
             position.tokensOwed1 -= amount1
             tokens.get(self.token1).deposit(recipient, amount1) 
             #self.ledger.transferToken(self, recipient, self.token1, amount1)
   
-        amount0 = self.convert(amount0)
-        amount1 = self.convert(amount1)        
+        amount0 = self._convert_to_human(amount0)
+        amount1 = self._convert_to_human(amount1)        
 
         return (recipient, tickLower, tickUpper, amount0, amount1)   
         
 
     def burn(self, recipient, tickLower, tickUpper, amount):
 
         """ burn
@@ -340,16 +336,15 @@
             amount0 : int
                 Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
                 Delta of the balance of token1 of the pool, exact when negative, minimum when positive               
             amount : int
                 How much liquidity to burn                  
         """  
-        
-        amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
+        amount = self._convert_to_machine(amount)
         
         checkInputTypes(
             accounts=(recipient), int24=(tickLower, tickUpper), uint128=(amount)
         )
 
         # Add check if the position exists - when poking an uninitialized position it can be that
         # getFeeGrowthInside finds a non-initialized tick before Position.update reverts.
@@ -373,17 +368,17 @@
         amount0 = abs(-amount0Int) & (2**256 - 1)
         amount1 = abs(-amount1Int) & (2**256 - 1)        
 
         if amount0 > 0 or amount1 > 0:
             position.tokensOwed0 += amount0
             position.tokensOwed1 += amount1
 
-        amount = self.convert(amount)   
-        amount0 = self.convert(amount0)
-        amount1 = self.convert(amount1)
+        amount = self._convert_to_human(amount)   
+        amount0 = self._convert_to_human(amount0)
+        amount1 = self._convert_to_human(amount1)
              
         return (recipient, tickLower, tickUpper, amount, amount0, amount1)
 
 
 
     def swapExact0For1(self, recipient, amount, sqrtPriceLimit):
 
@@ -406,16 +401,15 @@
             recipient : str
                 Address for which the liquidity will be created 
             amount0 : int
                 Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
                 Delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
         """         
-
-        amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
+        amount = self._convert_to_machine(amount)
         sqrtPriceLimitX96 = (
             sqrtPriceLimit
             if sqrtPriceLimit != None
             else UniV3Utils.getSqrtPriceLimitX96('Token0')
         )
 
         return self._swap(UniV3Utils.TEST_TOKENS[0], [amount, 0], recipient, sqrtPriceLimitX96)  
@@ -442,15 +436,15 @@
                 Address for which the liquidity will be created 
             amount0 : int
                 Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
                 Delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
         """           
         
-        amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
+        amount = self._convert_to_machine(amount)
         sqrtPriceLimitX96 = (
             sqrtPriceLimit
             if sqrtPriceLimit != None
             else UniV3Utils.getSqrtPriceLimitX96(UniV3Utils.TEST_TOKENS[0])
         )
         return self._swap(UniV3Utils.TEST_TOKENS[0], [0, amount], recipient, sqrtPriceLimitX96)  
 
@@ -477,15 +471,15 @@
                 Address for which the liquidity will be created 
             amount0 : int
                 Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
                 Delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
         """          
         
-        amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
+        amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else UniV3Helper().dec2gwei(amount)
         sqrtPriceLimitX96 = (
             sqrtPriceLimit
             if sqrtPriceLimit != None
             else UniV3Utils.getSqrtPriceLimitX96(UniV3Utils.TEST_TOKENS[1])
         )
         return self._swap(UniV3Utils.TEST_TOKENS[1], [amount, 0], recipient, sqrtPriceLimitX96)
     
@@ -511,15 +505,15 @@
                 Address for which the liquidity will be created 
             amount0 : int
                 Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
                 Delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
         """         
 
-        amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
+        amount = self._convert_to_machine(amount)
         sqrtPriceLimitX96 = (
             sqrtPriceLimit
             if sqrtPriceLimit != None
             else UniV3Utils.getSqrtPriceLimitX96(UniV3Utils.TEST_TOKENS[1])
         )
         return self._swap(UniV3Utils.TEST_TOKENS[1], [0, amount], recipient, sqrtPriceLimitX96)     
 
@@ -630,14 +624,15 @@
             ) = SwapMath.computeSwapStep(
                 state.sqrtPriceX96,
                 sqrtRatioTargetX96,
                 state.liquidity,
                 state.amountSpecifiedRemaining,
                 self.fee,
             )
+
             if exactInput:
                 state.amountSpecifiedRemaining -= step.amountIn + step.feeAmount
                 state.amountCalculated = SafeMath.subInts(
                     state.amountCalculated, step.amountOut
                 )
             else:
                 state.amountSpecifiedRemaining += step.amountOut
@@ -726,17 +721,17 @@
         if zeroForOne: 
             tokens.get(self.token0).deposit(recipient, abs(amount0))
             self._swap_tokens(0, abs(amount1), recipient)            
         else: 
             tokens.get(self.token1).deposit(recipient, abs(amount1))
             self._swap_tokens(abs(amount0), 0, recipient)            
 
-        amount0 = self.convert(amount0)
-        amount1 = self.convert(amount1)
-        liquidity = self.convert(state.liquidity)
+        amount0 = self._convert_to_human(amount0)
+        amount1 = self._convert_to_human(amount1)
+        liquidity = self._convert_to_human(state.liquidity)
         
         return (
             recipient,
             amount0,
             amount1,
             state.sqrtPriceX96,
             liquidity,
@@ -837,42 +832,65 @@
                 # No tick to the right
                 return TickMath.MAX_TICK, False
             nextTick = sortedKeyList[indexCurrentTick + 1]
 
         # Return tick within the boundaries
         return nextTick, True  
 
-    def get_price(self, token): 
-        pass
-            
+    def get_price(self, token):  
+        
+        """ get_price
+
+            Get price of select token in the exchange pair
+                
+            Parameters
+            -----------------
+            token : ERC20
+                ERC20 token                
+        """          
+        sqrt_P = self.slot0.sqrtPriceX96/2**96
+        
+        if(token.token_name == self.token0):
+            if(self.reserve0 == 0):
+                return None 
+            else:
+                return sqrt_P**2 
+        elif(token.token_name == self.token1):
+            if(self.reserve1 == 0):
+                return None
+            else:
+                return 1/sqrt_P**2 
+        else:
+            assert False, 'UniswapV2: WRONG_INPUT_TOKEN'   
+                  
     def get_liquidity(self):  
         
         """ get_liquidity
 
             Get liquidity of exchange pool         
         """          
 
-        return self.gwei2dec(self.total_supply)        
+        return UniV3Helper().gwei2dec(self.total_supply)        
             
     def get_reserve(self, token):  
         
         """ get_reserve
 
             Get reserve amount of select token in the exchange pair
                 
             Parameters
             -----------------
             token : ERC20
                 ERC20 token                
         """         
         
         if(token.token_name == self.token0):
-            return self.gwei2dec(self.reserve0) 
+            return UniV3Helper().gwei2dec(self.reserve0) 
         elif(token.token_name == self.token1):
-            return self.gwei2dec(self.reserve1)
+            return UniV3Helper().gwei2dec(self.reserve1)
         else:
             assert False, 'UniswapV2: WRONG_INPUT_TOKEN'      
 
     def get_virtual_reserve(self, token):  
         
         """ get_virtual_reserve
 
@@ -890,28 +908,22 @@
         if(token.token_name == self.token0):
             return liq/sqrt_P
         elif(token.token_name == self.token1):
             return liq*sqrt_P
         else:
             assert False, 'UniswapV2: WRONG_INPUT_TOKEN'           
 
-    def convert(self, val): 
-        val = val if self.precision == UniswapExchangeData.TYPE_GWEI else self.gwei2dec(val)
+    def _convert_to_human(self, val): 
+        val = val if self.precision == UniswapExchangeData.TYPE_GWEI else UniV3Helper().gwei2dec(val)
         return val
-    
 
-    def dec2gwei(self, tkn_amt, precision=None):
-        precision = GWEI_PRECISION if precision == None else precision
-        return int(Decimal(str(tkn_amt))*Decimal(str(10**precision)))
-    
-    def gwei2dec(self, tkn_amt, precision=None):   
-        precision = GWEI_PRECISION if precision == None else precision
-        return float(Decimal(str(tkn_amt))/Decimal(str(10**precision)))  
+    def _convert_to_machine(self, val): 
+        val = val if self.precision == UniswapExchangeData.TYPE_GWEI else UniV3Helper().dec2gwei(val)
+        return val        
     
-
     def _swap(self, inputToken, amounts, recipient, sqrtPriceLimitX96):
         [amountIn, amountOut] = amounts
         exactInput = amountOut == 0
         amount = amountIn if exactInput else amountOut
 
         if inputToken == 'Token0':
             if exactInput:
```

### Comparing `uniswappy-1.4.0/python/prod/cpt/factory/UniswapFactory.py` & `uniswappy-1.5.0/python/prod/cpt/factory/UniswapFactory.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/cpt/index/RebaseIndexToken.py` & `uniswappy-1.5.0/python/prod/cpt/index/RebaseIndexToken.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright [2023] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ...erc import ERC20
-from ...process.swap import WithdrawSwap
 from ...utils.data import UniswapExchangeData
+from ...utils.tools.v3 import TickMath
 
 class RebaseIndexToken():
     
     """ 
         Determine rebase amount of index token given a certain amount of liquidity from LP (inverse of SettlementLPToken)  
     """      
 
     
     def __init__(self):
-        self.fac = ERC20("DAI", "0x09")
+        pass
      
-    def apply(self, lp, tkn, liq_amt): 
+    def apply(self, lp, tkn, liq_amt, lwr_tick = None, upr_tick = None): 
        
         """ apply
 
             Apply rebase token calculation settlement; given liquidity amount, what is the reserve amount
                 
             Parameters
             -----------------
@@ -33,42 +33,65 @@
 
             Returns
             -----------------
             rebase_amount: float
                 Reserve token amount, given liquidity amount
                    
         """        
+        if(lp.version == UniswapExchangeData.VERSION_V2):
+            settlement = self.calc_univ2_tkn_settlement(lp, tkn, liq_amt)
+        elif(lp.version == UniswapExchangeData.VERSION_V3):   
+            settlement = self.calc_univ3_tkn_settlement(lp, tkn, liq_amt, lwr_tick, upr_tick)
         
-        return self.calc_tkn_settlement(lp, tkn, liq_amt)
+        return settlement
     
-    def calc_tkn_settlement(self, lp, token_in, dL):
+    def calc_univ2_tkn_settlement(self, lp, token_in, dL):
             
         (x, y) = self.get_reserves(lp, token_in)
         L = lp.get_liquidity()
         a0 = dL*x/L
         a1 = dL*y/L
         gamma = 997/1000
 
         dy1 = a1
         dy2 = gamma*a0*(y - a1)/(x - a0 + gamma*a0)
         itkn_amt = dy1 + dy2
 
         return itkn_amt if itkn_amt > 0 else 0  
 
+    def calc_univ3_tkn_settlement(self, lp, token_in, dL, lwr_tick, upr_tick):
+                
+        L = lp.get_liquidity()
+        if(token_in.token_name == lp.token0):
+            sqrtp_cur = lp.slot0.sqrtPriceX96/2**96
+            sqrtp_pa = TickMath.getSqrtRatioAtTick(lwr_tick)/2**96
+            sqrtp_pb = TickMath.getSqrtRatioAtTick(upr_tick)/2**96 
+            dPy = (sqrtp_cur - sqrtp_pa)
+            dPx = (1/sqrtp_cur - 1/sqrtp_pb)          
+        elif(token_in.token_name == lp.token1):
+            sqrtp_cur = 2**96/lp.slot0.sqrtPriceX96
+            sqrtp_pa = 2**96/TickMath.getSqrtRatioAtTick(lwr_tick)
+            sqrtp_pb = 2**96/TickMath.getSqrtRatioAtTick(upr_tick)
+            dPx = (1/sqrtp_cur - 1/sqrtp_pa)
+            dPy = (sqrtp_cur - sqrtp_pb)
+    
+        dAmt = dL*dPx
+        
+        L_diff = (L - dL) 
+        sqrtp_next = sqrtp_cur + (997*dAmt)/(L_diff*1000) 
+        dy1 = dAmt
+        dy2 = L_diff * (1/sqrtp_cur - 1/sqrtp_next)
+        itkn_amt = dy1 + dy2
+
+        return itkn_amt if itkn_amt > 0 else 0 
+    
+
     def get_reserves(self, lp, token_in):
         tokens = lp.factory.token_from_exchange[lp.name]
-        if(lp.version == UniswapExchangeData.VERSION_V2):
-            if(token_in.token_name == lp.token1):
-                x = lp.get_reserve(tokens[lp.token0])
-                y = lp.get_reserve(tokens[lp.token1])
-            else: 
-                x = lp.get_reserve(tokens[lp.token1])
-                y = lp.get_reserve(tokens[lp.token0])
-        elif(lp.version == UniswapExchangeData.VERSION_V3):   
-            if(token_in.token_name == lp.token1):
-                x = lp.get_virtual_reserve(tokens[lp.token0])
-                y = lp.get_virtual_reserve(tokens[lp.token1])
-            else: 
-                x = lp.get_virtual_reserve(tokens[lp.token1])
-                y = lp.get_virtual_reserve(tokens[lp.token0]) 
+        if(token_in.token_name == lp.token1):
+            x = lp.get_reserve(tokens[lp.token0])
+            y = lp.get_reserve(tokens[lp.token1])
+        else: 
+            x = lp.get_reserve(tokens[lp.token1])
+            y = lp.get_reserve(tokens[lp.token0])
         return (x, y)
```

### Comparing `uniswappy-1.4.0/python/prod/cpt/quote/IndexTokenQuote.py` & `uniswappy-1.5.0/python/prod/cpt/quote/IndexTokenQuote.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/cpt/quote/LPQuote.py` & `uniswappy-1.5.0/python/prod/cpt/quote/LPQuote.py`

 * *Files 9% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         if(tkn.token_name == lp.token0):
             amt_out = (amount_in * lp.reserve1) / lp.reserve0
         else:
             amt_out = (amount_in * lp.reserve0) / lp.reserve1
     
         return amt_out if self.quote_opposing else amount_in 
     
-    def get_amount_from_lp(self, lp, tkn, amount_lp_in):
+    def get_amount_from_lp(self, lp, tkn, amount_lp_in, lwr_tick = None, upr_tick = None):
         
         """ get_amount_from_lp
 
             Get amount of opposing token, given an amount priced in liquidity
                 
             Parameters
             -----------------
@@ -186,22 +186,22 @@
             Returns
             -----------------
             amt_out: float
                 Amount of opposing token 
         """           
         
         if(amount_lp_in > 0):
-            itkn_amt = RebaseIndexToken().apply(lp, tkn, amount_lp_in)
+            itkn_amt = RebaseIndexToken().apply(lp, tkn, amount_lp_in, lwr_tick, upr_tick)
             amt_out = self.get_amount(lp, tkn, itkn_amt) if self.quote_opposing else itkn_amt
         else:
             amt_out = 0
         return amt_out   
     
     
-    def get_lp_from_amount(self, lp, tkn, amount_in):
+    def get_lp_from_amount(self, lp, tkn, amount_in, lwr_tick = None, upr_tick = None):
         
         """ get_lp_from_amount
 
             Get amount of liquidity, given an amount reserve token
                 
             Parameters
             -----------------
@@ -215,12 +215,12 @@
             Returns
             -----------------
             amt_out: float
                 Amount of liquidity 
         """         
         
         if(amount_in > 0):
-            lp_amt = SettlementLPToken().apply(lp, tkn, amount_in)
+            lp_amt = SettlementLPToken().apply(lp, tkn, amount_in, lwr_tick, upr_tick)
         else:
             lp_amt = 0
         return lp_amt
```

### Comparing `uniswappy-1.4.0/python/prod/cpt/quote/LPTokenQuote.py` & `uniswappy-1.5.0/python/prod/cpt/quote/LPTokenQuote.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/cpt/quote/TreeAmountQuote.py` & `uniswappy-1.5.0/python/prod/cpt/quote/TreeAmountQuote.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/cpt/vault/IndexVault.py` & `uniswappy-1.5.0/python/prod/cpt/vault/IndexVault.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/cpt/vault/Vault.py` & `uniswappy-1.5.0/python/prod/cpt/vault/Vault.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/cpt/wallet/Wallets.py` & `uniswappy-1.5.0/python/prod/cpt/wallet/Wallets.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/erc/DOAERC20.py` & `uniswappy-1.5.0/python/prod/erc/DOAERC20.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/erc/ERC20.py` & `uniswappy-1.5.0/python/prod/erc/ERC20.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/erc/IndexERC20.py` & `uniswappy-1.5.0/python/prod/erc/IndexERC20.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/erc/LPERC20.py` & `uniswappy-1.5.0/python/prod/erc/LPERC20.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/math/interest/Yield.py` & `uniswappy-1.5.0/python/prod/math/interest/Yield.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/math/interest/ips/ConstantIPS.py` & `uniswappy-1.5.0/python/prod/math/interest/ips/ConstantIPS.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/math/model/BrownianModel.py` & `uniswappy-1.5.0/python/prod/math/model/BrownianModel.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/math/model/ModelQueue.py` & `uniswappy-1.5.0/python/prod/math/model/ModelQueue.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/math/model/TimeDeltaModel.py` & `uniswappy-1.5.0/python/prod/math/model/TimeDeltaModel.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/math/model/TokenDeltaModel.py` & `uniswappy-1.5.0/python/prod/math/model/TokenDeltaModel.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/math/risk/MaxDrop.py` & `uniswappy-1.5.0/python/prod/math/risk/MaxDrop.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/process/burn/IndexTokenBurn.py` & `uniswappy-1.5.0/python/prod/process/burn/IndexTokenBurn.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/process/deposit/SwapDeposit.py` & `uniswappy-1.5.0/python/prod/process/swap/WithdrawSwap.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,102 +1,95 @@
 # Copyright [2023] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ..Process import Process
-from ..liquidity import AddLiquidity
-from ..swap import Swap
+from .Swap import Swap
+from ..liquidity import RemoveLiquidity
 from ...math.model import TokenDeltaModel
 from ...math.model import EventSelectionModel
 from ...utils.data import UniswapExchangeData
+from ...cpt.index import SettlementLPToken
 import math
 
-
-class SwapDeposit(Process):
+class WithdrawSwap(Process):
     
-    """ Process to swap approx. half of single token X for token Y (and vice verse) and deposit proceeds
-        plus remaining other approximated half
+    """ Process to withdraw liquidity from LP and swap opposing token which is added to specifed token to receive         
+        a single amount of specified token
 
         Parameters
         ----------
         ev : EventSelectionModel
             EventSelectionModel object to randomly generate buy vs sell events
         tDel : TokenDeltaModel
             TokenDeltaModel to randomly generate token amounts        
     """       
 
     def __init__(self, ev = None, tDel = None):
         self.ev = EventSelectionModel() if ev  == None else ev
         self.tDel = TokenDeltaModel(50) if tDel == None else tDel
             
-    def apply(self, lp, token_in, user_nm, amount_in, lwr_tick = None, upr_tick = None):   
+    def apply(self, lp, token_out, user_nm, amount_out, lwr_tick = None, upr_tick = None):    
         
         """ apply
 
-            Swap approx. half of single token X for token Y (and vice verse) and deposit proceeds
-            plus remaining other approximated half
+            Withdraw liquidity from LP and swap opposing token which is added to specifed token to receive                 
+            a single amount of specified token
                 
             Parameters
             -------
             lp : Exchange
                 LP exchange
-            token_in : ERC20
+            token_out : ERC20
                 specified ERC20 token               
             user_nm : str
                 account name
-            amount_in : float
+            amount_out : float
                 token amount to be swap 
             lwr_tick : int
                 lower tick of the position in which to add liquidity   
             upr_tick : int
-                upper tick of the position in which to add liquidity   
+                upper tick of the position in which to add liquidity                 
                 
             Returns
             -------
-            (amount_in, amount_out) : float, float
-                token swap amounts                
+            amount_out : float
+                amount of withdrawn token               
         """          
         
-        amount_in = tDel.delta() if amount_in == None else amount_in    
+        amount_out = tDel.delta() if amount_out == None else amount_out
+    
+        
+        if(lp.version == UniswapExchangeData.VERSION_V2):
+            # Step 1: withdrawal
+            p_out = self._calc_withdraw_portion(lp, token_out, amount_out, lwr_tick, upr_tick)
+            removeLiq = RemoveLiquidity()
+            res = removeLiq.apply(lp, token_out, user_nm, p_out*amount_out)
+    
+            # Step 2: swap
+            trading_token = self.get_trading_token(lp, token_out)
+            out = Swap().apply(lp, trading_token, user_nm, res[trading_token.token_name])  
+            withdrawn = out + p_out*amount_out 
+            #withdrawn = p_out*amount_out 
 
-        # Step 1: swap        
-        p_in = self._calc_deposit_portion(lp, token_in, amount_in)
-        amount_out = Swap().apply(lp, token_in, user_nm, p_in*amount_in)
-        trading_token = self.get_trading_token(lp, token_in)
+        elif(lp.version == UniswapExchangeData.VERSION_V3): 
 
-        # Step 2: deposit   
-        if(lp.version == UniswapExchangeData.VERSION_V2):
-            if(token_in.token_name == lp.token1):
-                balance0 = amount_out 
-                balance1 = lp.quote(balance0, lp.reserve0, lp.reserve1)
-                deposited = balance1 + p_in*amount_in
-            elif(token_in.token_name == lp.token0):
-                balance1 = amount_out
-                balance0 = lp.quote(balance1, lp.reserve1, lp.reserve0)
-                deposited = balance0 + p_in*amount_in
-            lp.add_liquidity(user_nm, balance0, balance1, balance0, balance1) 
+            p_out = self._calc_withdraw_portion(lp, token_out, amount_out, lwr_tick, upr_tick)
             
-        elif(lp.version == UniswapExchangeData.VERSION_V3):  
-            tot_liq = lp.get_liquidity()
-            sqrt_P = lp.slot0.sqrtPriceX96/2**96
-            tokens = lp.factory.token_from_exchange[lp.name] 
-
-            if(token_in.token_name == lp.token0):
-                balance1 = abs(amount_out[2]) 
-                liq = balance1/sqrt_P 
-                deposited = liq/sqrt_P + p_in*amount_in
-                                
-            elif(token_in.token_name == lp.token1): 
-                balance0 = abs(amount_out[1]) 
-                liq = balance0*sqrt_P 
-                deposited = liq*sqrt_P + p_in*amount_in
-                
-            lp.mint(user_nm, lwr_tick, upr_tick, liq)  
-                            
-        return deposited  
+             # Step 1: withdrawal
+            removeLiq = RemoveLiquidity()
+            res = removeLiq.apply(lp, token_out, user_nm, p_out*amount_out, lwr_tick, upr_tick)
+        
+            # Step 2: swap
+            trading_token = self.get_trading_token(lp, token_out)
+            out = Swap().apply(lp, trading_token, user_nm, res[trading_token.token_name]) 
+            withdrawn = abs(out[1])  + p_out*amount_out 
+
+        return withdrawn 
+
 
     def get_trading_token(self, lp, token):
         
         """ get_trading_token
 
             Get opposing token from specified token
                 
@@ -107,39 +100,45 @@
             token : ERC20
                 specified ERC20 token      
                 
             Returns
             -------
             trading_token : ERC20 
                 opposing ERC20 token                   
-        """         
+        """          
         
         tokens = lp.factory.token_from_exchange[lp.name]
         trading_token = tokens[lp.token1] if token.token_name == lp.token0 else tokens[lp.token0]
-        return trading_token       
-            
-    
-    def _calc_deposit_portion(self, lp, token_in, dx):
-
-        tkn_supply = self._get_tkn_supply(lp, token_in)
-        a = 997*(dx**2)/(1000*tkn_supply)
-        b = dx*(1997/1000)
-        c = -dx
+        return trading_token        
+ 
+    def _calc_withdraw_portion(self, lp, token_in, amt, lwr_tick, upr_tick):
+
+        (x, y) = self._get_reserves(lp, token_in)
+        L = lp.get_liquidity()
+        gamma = 997/1000
+
+        dL = SettlementLPToken().apply(lp, token_in, amt, lwr_tick, upr_tick)
+        dx = dL*x/L
+        dy = dL*y/L
+        aswap = (gamma*dx)*(y-dy)/(x-dx+gamma*dx)
 
-        alpha = -(b - math.sqrt(b*b - 4*a*c)) / (2*a)
-        return alpha 
+        return dy/amt 
 
-    def _get_tkn_supply(self, lp, token_in):
+    def _get_reserves(self, lp, token_in):
         tokens = lp.factory.token_from_exchange[lp.name]
         if(lp.version == UniswapExchangeData.VERSION_V2):
-            if(token_in.token_name == lp.token0):
-                tkn_supply = lp.get_reserve(tokens[lp.token0])
-            else:    
-                tkn_supply = lp.get_reserve(tokens[lp.token1])
+            if(token_in.token_name == lp.token1):
+                x = lp.get_reserve(tokens[lp.token0])
+                y = lp.get_reserve(tokens[lp.token1])
+            else: 
+                x = lp.get_reserve(tokens[lp.token1])
+                y = lp.get_reserve(tokens[lp.token0])
         elif(lp.version == UniswapExchangeData.VERSION_V3):   
-            if(token_in.token_name == lp.token0):
-                tkn_supply = lp.get_virtual_reserve(tokens[lp.token0])
-            else:    
-                tkn_supply = lp.get_virtual_reserve(tokens[lp.token1])
-        return tkn_supply        
+            if(token_in.token_name == lp.token1):
+                x = lp.get_virtual_reserve(tokens[lp.token0])
+                y = lp.get_virtual_reserve(tokens[lp.token1])
+            else: 
+                x = lp.get_virtual_reserve(tokens[lp.token1])
+                y = lp.get_virtual_reserve(tokens[lp.token0]) 
+        return (x, y)        
+    
         
-
```

### Comparing `uniswappy-1.4.0/python/prod/process/join/Join.py` & `uniswappy-1.5.0/python/prod/process/join/Join.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright [2024] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ...utils.data import UniswapExchangeData
 from ...utils.tools.v3 import UniV3Utils
+from ...utils.tools.v3 import UniV3Helper
 import math
 
 class Join():
     
     """ Process to join x and y amounts to pool              
     """       
 
@@ -40,13 +41,16 @@
                 join output               
         """ 
 
         if(lp.version == UniswapExchangeData.VERSION_V2):
             out = lp.add_liquidity(user_nm, amount0, amount1, amount0, amount1)
             
         elif(lp.version == UniswapExchangeData.VERSION_V3):
-            k = math.sqrt(amount0*amount1)
-            init_liquidity = UniV3Utils.encodePriceSqrt(amount1, amount0)
-            lp.initialize(init_liquidity)
-            out = lp.mint(user_nm, lwr_tick, upr_tick, k)
+            init_price = UniV3Utils.encodePriceSqrt(amount1, amount0)
+            sqrtP = init_price/2**96
+            Ly = UniV3Helper().calc_Ly(sqrtP, amount1, lwr_tick, upr_tick)
+            Lx = UniV3Helper().calc_Lx(sqrtP, amount0, lwr_tick, upr_tick)
+            L_mint = min(Ly, Lx)    
+            lp.initialize(init_price)
+            out = lp.mint(user_nm, lwr_tick, upr_tick, L_mint)
              
         return out
```

### Comparing `uniswappy-1.4.0/python/prod/process/liquidity/AddLiquidity.py` & `uniswappy-1.5.0/python/prod/process/liquidity/AddLiquidity.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ..Process import Process
 from ...math.model import TokenDeltaModel
 from ...math.model import EventSelectionModel
 from ...utils.data import UniswapExchangeData
+from ...utils.tools.v3 import UniV3Helper
 
 class AddLiquidity(Process):
      
     """ Add liquidity process
 
         Parameters
         ----------
@@ -76,21 +77,19 @@
                 else:
                     balance0 = self.init_price*balance1            
                 
                 lp.add_liquidity(user_nm, balance0, balance1, balance0, balance1) 
 
         elif(lp.version == UniswapExchangeData.VERSION_V3): 
 
-            tot_liq = lp.get_liquidity()
             sqrt_P = lp.slot0.sqrtPriceX96/2**96
-
             if(token_in.token_name == lp.token0):
-                liq = amount_in*sqrt_P
-                (balance0, balance1)  = lp.mint(user_nm, lwr_tick, upr_tick, liq)
+                Lx = UniV3Helper().calc_Lx(sqrt_P, amount_in, lwr_tick, upr_tick)
+                (balance0, balance1)  = lp.mint(user_nm, lwr_tick, upr_tick, Lx)
             elif(token_in.token_name == lp.token1): 
-                liq = amount_in/sqrt_P
-                (balance0, balance1) = lp.mint(user_nm, lwr_tick, upr_tick, liq)  
+                Ly = UniV3Helper().calc_Ly(sqrt_P, amount_in, lwr_tick, upr_tick)
+                (balance0, balance1) = lp.mint(user_nm, lwr_tick, upr_tick, Ly)  
 
         return {lp.token0:balance0, lp.token1:balance1}
```

### Comparing `uniswappy-1.4.0/python/prod/process/liquidity/RemoveLiquidity.py` & `uniswappy-1.5.0/python/prod/process/liquidity/RemoveLiquidity.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/process/mint/SwapIndexMint.py` & `uniswappy-1.5.0/python/prod/process/mint/SwapIndexMint.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/process/swap/RandomSwap.py` & `uniswappy-1.5.0/python/prod/process/swap/RandomSwap.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/process/swap/Swap.py` & `uniswappy-1.5.0/python/prod/process/swap/Swap.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/simulate/Arbitrage.py` & `uniswappy-1.5.0/python/prod/simulate/Arbitrage.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/simulate/CorrectReserves.py` & `uniswappy-1.5.0/python/prod/simulate/CorrectReserves.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright [2024] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ..simulate import SolveDeltas
 from ..process.deposit import SwapDeposit
 from ..process.swap import WithdrawSwap
+from ..utils.data import UniswapExchangeData
 import numpy as np
 
 X0 = 1
 FAC = 1
 MAX_ATTEMPTS = 5
 USER_NM = 'reserve_correction'
 
 class CorrectReserves:
     
     """ 
         Applies SolveDeltas to Correct x/y reserve amounts so that price reflects desired input price; 
-        in the case for the BUIDL week event, it would be the most recent market price returned from 
-        the 0x API 
+        in the marjority of cases, the input price would be the most recent outside market price 
         
         Parameters
         -----------------
         lp : UniswapExchange
             Uniswap Exchange class
         x0 : float
             Initial market price at the beginning of the simulation 
@@ -61,15 +61,15 @@
             -----------------
             swap_dy : float
                 Delta y reserve adjustment from SolveDeltas class                   
         """           
         
         return self.swap_dy    
     
-    def apply(self, p): 
+    def apply(self, p, lwr_tick = None, upr_tick = None): 
         
         """ apply
 
             Apply reserve correction of mock pool given external price (eg. market price from 0x API)
                 
             Parameters
             -----------------
@@ -78,21 +78,21 @@
         """         
         
         do_update = True  
         max_tries = 5; c = 0
         while(do_update and c <= MAX_ATTEMPTS):
             c=+1
             try: 
-                self._update(p)
+                self._update(p, lwr_tick, upr_tick)
                 do_update = False 
             except:
                 p = p + np.random.normal(0, 0.1)  
                 do_update = True 
                 
-        assert c != MAX_ATTEMPTS, 'UniswapV2: RESERVE_CORRECTION_FAILURE'   
+        assert c != MAX_ATTEMPTS, 'Uniswap: RESERVE_CORRECTION_FAILURE'   
         
     def get_x_tkn(self): 
         
         """ get_x_tkn
 
             Get x token from Uniswap mock pool
                 
@@ -114,22 +114,29 @@
             -----------------
             y_tkn : ERC20
                 y token from mock pool                   
         """           
         
         return self.lp.factory.token_from_exchange[self.lp.name][self.lp.token1]        
                 
-    def _update(self, p):  
+    def _update(self, p, lwr_tick, upr_tick):  
         tkn_x = self.get_x_tkn()
         tkn_y = self.get_y_tkn()
-        
-        self.swap_dx, self.swap_dy = self.sDel.calc(p, self.x0, self.fac)   
-        if(self.swap_dx >= 0):
-            expected_amount_dep = SwapDeposit().apply(self.lp, tkn_x, USER_NM, abs(self.swap_dx))
-            expected_amount_out = WithdrawSwap().apply(self.lp, tkn_y, USER_NM, abs(self.swap_dy))
-        elif(self.swap_dy >= 0):
-            expected_amount_dep = SwapDeposit().apply(self.lp, tkn_y, USER_NM, abs(self.swap_dy))
-            expected_amount_out = WithdrawSwap().apply(self.lp, tkn_x, USER_NM, abs(self.swap_dx))                   
-            
+        self.swap_dx, self.swap_dy = self.sDel.calc(p, self.x0, self.fac)
 
-        
-        
+        if(self.lp.version == UniswapExchangeData.VERSION_V2):
+            if(self.swap_dx >= 0):
+                expected_amount_dep = SwapDeposit().apply(self.lp, tkn_x, USER_NM, abs(self.swap_dx))
+                expected_amount_out = WithdrawSwap().apply(self.lp, tkn_y, USER_NM, abs(self.swap_dy))
+            elif(self.swap_dy >= 0):
+                expected_amount_dep = SwapDeposit().apply(self.lp, tkn_y, USER_NM, abs(self.swap_dy))
+                expected_amount_out = WithdrawSwap().apply(self.lp, tkn_x, USER_NM, abs(self.swap_dx)) 
+               
+        elif(self.lp.version == UniswapExchangeData.VERSION_V3):
+            if(self.swap_dx >= 0):
+                expected_amount_dep = SwapDeposit().apply(self.lp, tkn_x, USER_NM, abs(self.swap_dx), lwr_tick, upr_tick)
+                expected_amount_out = WithdrawSwap().apply(self.lp, tkn_y, USER_NM, abs(self.swap_dy), lwr_tick, upr_tick)
+            elif(self.swap_dy >= 0):
+                expected_amount_dep = SwapDeposit().apply(self.lp, tkn_y, USER_NM, abs(self.swap_dy), lwr_tick, upr_tick)
+                expected_amount_out = WithdrawSwap().apply(self.lp, tkn_x, USER_NM, abs(self.swap_dx), lwr_tick, upr_tick) 
+              
+
```

### Comparing `uniswappy-1.4.0/python/prod/simulate/MarkovState.py` & `uniswappy-1.5.0/python/prod/simulate/MarkovState.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/simulate/QuantTerminal.py` & `uniswappy-1.5.0/python/prod/simulate/QuantTerminal.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/simulate/SimpleLPSimulation.py` & `uniswappy-1.5.0/python/prod/simulate/SimpleLPSimulation.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/simulate/SolveDeltas.py` & `uniswappy-1.5.0/python/prod/simulate/SolveDeltas.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 # Copyright [2023] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from scipy.optimize import fsolve
+from ..utils.data import UniswapExchangeData
 import warnings
 warnings.filterwarnings("ignore")
 
 class SolveDeltas():
     
     def __init__(self, lp):
-        self.x = lp.reserve0
-        self.y = lp.reserve1
+        self.lp = lp
         self.tkn_x = lp.factory.token_from_exchange[lp.name][lp.token0]
         self.tkn_y = lp.factory.token_from_exchange[lp.name][lp.token1]      
+        self.x = self._get_reserve(self.tkn_x) 
+        self.y = self._get_reserve(self.tkn_y)       
         self.p = lp.get_price(self.tkn_x)
         self.p_prev = lp.get_price(self.tkn_x)
-        self.lp = lp
         self.dp = 0
               
     def get_lp(self):
         return self.lp   
                     
     def func_swap_yx(self, z):
         z[0] = 1 if z[0] == 0 else z[0]
         return [(self.x*abs(z[1]) + abs(z[0])*self.y)/(self.x**2 - abs(z[0])*self.x) - self.dp,
-                abs(z[1])/abs(z[0]) - self.p ]
+                abs(z[1])/abs(z[0]) - self.p]
 
     def func_swap_xy(self, z):
         z[0] = 1 if z[0] == 0 else z[0]
         return [-(self.x*abs(z[1]) + abs(z[0])*self.y)/(self.x**2 + abs(z[0])*self.x) - self.dp,
                 abs(z[1])/abs(z[0]) - self.p]
         
     def calc(self, p, x0 = None, fac = None):
         self.p = p
         self.p_prev = self.lp.get_price(self.tkn_x) 
         self.dp = p - self.p_prev
-        self.x = self.lp.reserve0
-        self.y = self.lp.reserve1
+        self.x = self._get_reserve(self.tkn_x)
+        self.y = self._get_reserve(self.tkn_y)   
         fac = 0.1 if fac == None else fac
         dx0 = 0.5 if x0 == None else x0/p
         dy0 = 0.5 if x0 == None else x0
         if(self.dp >= 0):
             dx, dy = fsolve(self.func_swap_yx, [dx0, dy0], xtol=1e-6, factor=fac, maxfev = 200)
             self.p_prev = p
             return -dx, dy
         else:
             dx, dy = fsolve(self.func_swap_xy, [dx0, dy0], xtol=1e-6, factor=fac, maxfev = 200)
             self.p_prev = p
-            return dx, -dy        
+            return dx, -dy  
+
+    def _get_reserve(self, tkn):
+        
+        if(self.lp.version == UniswapExchangeData.VERSION_V2):
+            return self.lp.get_reserve(tkn) 
+        elif(self.lp.version == UniswapExchangeData.VERSION_V3):
+            return self.lp.get_virtual_reserve(tkn)
```

### Comparing `uniswappy-1.4.0/python/prod/utils/client/API0x.py` & `uniswappy-1.5.0/python/prod/utils/client/API0x.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/data/Chain0x.py` & `uniswappy-1.5.0/python/prod/utils/data/Chain0x.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/data/UniswapExchangeData.py` & `uniswappy-1.5.0/python/prod/utils/data/UniswapExchangeData.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/FullMath.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/FullMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/LiquidityMath.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/LiquidityMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/Position.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/Position.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/SafeMath.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/SafeMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/Shared.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/Shared.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/SqrtPriceMath.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/SqrtPriceMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/SwapMath.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/SwapMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/Tick.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/Tick.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/TickMath.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/TickMath.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/python/prod/utils/tools/v3/UniV3Utils.py` & `uniswappy-1.5.0/python/prod/utils/tools/v3/UniV3Utils.py`

 * *Files identical despite different names*

### Comparing `uniswappy-1.4.0/setup.py` & `uniswappy-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='UniswapPy',
-      version='1.4.0',
+      version='1.5.0',
       description='Uniswap Analytics with Python',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/defipy-devs/uniswappy',
       author = "icmoore",
       author_email = "defipy.devs@gmail.com",
       license='MIT',
@@ -35,14 +35,15 @@
           'uniswappy.process.mint',
           'uniswappy.process.swap',
           'uniswappy.process.join',
           'uniswappy.simulate',
           'uniswappy.utils.interfaces',
           'uniswappy.utils.data',
           'uniswappy.utils.client',
+          'uniswappy.utils.tools',
           'uniswappy.utils.tools.v3'
       ],
       install_requires=[
           'scipy >= 1.7.3',
           'termcolor >= 2.4.0'
       ],
       zip_safe=False)
```


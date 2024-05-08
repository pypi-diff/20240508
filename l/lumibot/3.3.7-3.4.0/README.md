# Comparing `tmp/lumibot-3.3.7.tar.gz` & `tmp/lumibot-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumibot-3.3.7.tar", last modified: Thu Apr 11 20:50:56 2024, max compression
+gzip compressed data, was "lumibot-3.4.0.tar", last modified: Wed May  8 05:18:01 2024, max compression
```

## Comparing `lumibot-3.3.7.tar` & `lumibot-3.4.0.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.330601 lumibot-3.3.7/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.3.7/LICENSE
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-11 20:50:56.330516 lumibot-3.3.7/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.3.7/README.md
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.305146 lumibot-3.3.7/lumibot/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.307586 lumibot-3.3.7/lumibot/backtesting/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/backtesting/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/backtesting/alpaca_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/backtesting/alpha_vantage_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    31484 2024-04-10 21:16:31.000000 lumibot-3.3.7/lumibot/backtesting/backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/backtesting/ccxt_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/backtesting/pandas_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15345 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/backtesting/polygon_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/backtesting/yahoo_backtesting.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.309976 lumibot-3.3.7/lumibot/brokers/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/brokers/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/brokers/alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    42389 2024-04-11 19:45:49.000000 lumibot-3.3.7/lumibot/brokers/broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-03-27 23:07:04.000000 lumibot-3.3.7/lumibot/brokers/ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/brokers/interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    27001 2024-04-10 20:52:06.000000 lumibot-3.3.7/lumibot/brokers/tradier.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.313345 lumibot-3.3.7/lumibot/data_sources/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/data_sources/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/data_sources/alpaca_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/data_sources/alpha_vantage_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/data_sources/ccxt_backtesting_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/data_sources/ccxt_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.3.7/lumibot/data_sources/data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.3.7/lumibot/data_sources/data_source_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/data_sources/exceptions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/data_sources/interactive_brokers_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15700 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/data_sources/pandas_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.3.7/lumibot/data_sources/tradier_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.3.7/lumibot/data_sources/yahoo_data.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.315967 lumibot-3.3.7/lumibot/entities/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/entities/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.3.7/lumibot/entities/asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/entities/bar.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/entities/bars.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21354 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/entities/data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/entities/dataline.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    28434 2024-04-10 20:12:46.000000 lumibot-3.3.7/lumibot/entities/order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/entities/position.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/entities/trading_fee.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.318643 lumibot-3.3.7/lumibot/example_strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/ccxt_backtesting_example.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/crypto_important_functions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.3.7/lumibot/example_strategies/options_hold_to_expiry.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/simple_start_single_file.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/stock_bracket.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/stock_buy_and_hold.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/stock_diversified_leverage.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/stock_limit_and_trailing_stops.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/stock_momentum.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/stock_oco.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/example_strategies/strangle.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.320669 lumibot-3.3.7/lumibot/strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    53804 2024-04-11 19:46:06.000000 lumibot-3.3.7/lumibot/strategies/_strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)   149970 2024-04-11 19:46:06.000000 lumibot-3.3.7/lumibot/strategies/strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    39749 2024-04-10 20:12:46.000000 lumibot-3.3.7/lumibot/strategies/strategy_executor.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.324166 lumibot-3.3.7/lumibot/tools/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/tools/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/tools/black_scholes.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.3.7/lumibot/tools/ccxt_data_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/tools/debugers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/tools/decorators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/tools/helpers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    26195 2024-04-10 20:29:05.000000 lumibot-3.3.7/lumibot/tools/indicators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/tools/lumibot_time.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/tools/pandas.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.3.7/lumibot/tools/polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/tools/types.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15620 2024-04-10 20:12:46.000000 lumibot-3.3.7/lumibot/tools/yahoo_helper.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.324586 lumibot-3.3.7/lumibot/traders/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/traders/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7929 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/traders/trader.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.325303 lumibot-3.3.7/lumibot/trading_builtins/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/trading_builtins/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/trading_builtins/custom_stream.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.3.7/lumibot/trading_builtins/safe_list.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.330129 lumibot-3.3.7/lumibot.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-04-11 20:50:56.000000 lumibot-3.3.7/lumibot.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3233 2024-04-11 20:50:56.000000 lumibot-3.3.7/lumibot.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-04-11 20:50:56.000000 lumibot-3.3.7/lumibot.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-04-11 20:50:56.000000 lumibot-3.3.7/lumibot.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-04-11 20:50:56.000000 lumibot-3.3.7/lumibot.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.3.7/pyproject.toml
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-04-11 20:50:56.331065 lumibot-3.3.7/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1865 2024-04-11 20:49:22.000000 lumibot-3.3.7/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.328490 lumibot-3.3.7/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-04-11 20:50:56.329933 lumibot-3.3.7/tests/backtest/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/backtest/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/backtest/test_example_strategies.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/backtest/test_main_pandas_daily.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12830 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/backtest/test_polygon.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/backtest/test_strategy_executor.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1909 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/backtest/test_yahoo.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_alpaca_old.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_ccxt_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.3.7/tests/test_order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_strategy_methods.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.3.7/tests/test_tradier.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.3.7/tests/test_tradingfee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.778898 lumibot-3.4.0/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.4.0/LICENSE
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-08 05:18:01.778836 lumibot-3.4.0/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.4.0/README.md
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.765012 lumibot-3.4.0/lumibot/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.766736 lumibot-3.4.0/lumibot/backtesting/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/alpaca_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/alpha_vantage_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    31484 2024-04-10 21:16:31.000000 lumibot-3.4.0/lumibot/backtesting/backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/ccxt_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/pandas_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    14588 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/backtesting/polygon_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/backtesting/yahoo_backtesting.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.767959 lumibot-3.4.0/lumibot/brokers/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/brokers/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/brokers/alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    42389 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/brokers/broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-04-16 22:57:26.000000 lumibot-3.4.0/lumibot/brokers/ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/brokers/interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    27085 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/brokers/tradier.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.769849 lumibot-3.4.0/lumibot/data_sources/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/alpaca_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/alpha_vantage_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/ccxt_backtesting_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/ccxt_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15261 2024-04-03 02:08:33.000000 lumibot-3.4.0/lumibot/data_sources/data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.4.0/lumibot/data_sources/data_source_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/exceptions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/data_sources/interactive_brokers_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15512 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/data_sources/pandas_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9535 2024-04-07 08:26:01.000000 lumibot-3.4.0/lumibot/data_sources/tradier_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.4.0/lumibot/data_sources/yahoo_data.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.771091 lumibot-3.4.0/lumibot/entities/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9174 2024-04-07 08:26:01.000000 lumibot-3.4.0/lumibot/entities/asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/bar.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/bars.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21849 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/entities/data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/dataline.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    28373 2024-05-08 05:17:06.000000 lumibot-3.4.0/lumibot/entities/order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/position.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/entities/trading_fee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.772752 lumibot-3.4.0/lumibot/example_strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/ccxt_backtesting_example.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-04-16 22:57:26.000000 lumibot-3.4.0/lumibot/example_strategies/crypto_important_functions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.4.0/lumibot/example_strategies/options_hold_to_expiry.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/simple_start_single_file.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_bracket.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_buy_and_hold.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_diversified_leverage.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_limit_and_trailing_stops.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_momentum.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/stock_oco.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/example_strategies/strangle.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.773453 lumibot-3.4.0/lumibot/strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    53879 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/strategies/_strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)   149930 2024-04-16 01:12:34.000000 lumibot-3.4.0/lumibot/strategies/strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    39943 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/strategies/strategy_executor.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.774978 lumibot-3.4.0/lumibot/tools/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/black_scholes.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.4.0/lumibot/tools/ccxt_data_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/debugers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/decorators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/helpers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    26283 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/tools/indicators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/lumibot_time.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/pandas.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    19664 2024-04-07 08:25:48.000000 lumibot-3.4.0/lumibot/tools/polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/tools/types.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15762 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/tools/yahoo_helper.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.775319 lumibot-3.4.0/lumibot/traders/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/traders/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7995 2024-05-08 03:43:54.000000 lumibot-3.4.0/lumibot/traders/trader.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.775667 lumibot-3.4.0/lumibot/trading_builtins/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/trading_builtins/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/trading_builtins/custom_stream.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.4.0/lumibot/trading_builtins/safe_list.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.778519 lumibot-3.4.0/lumibot.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3260 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-05-08 05:18:01.000000 lumibot-3.4.0/lumibot.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.4.0/pyproject.toml
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-05-08 05:18:01.779197 lumibot-3.4.0/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1809 2024-05-08 05:17:27.000000 lumibot-3.4.0/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.777443 lumibot-3.4.0/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-08 05:18:01.778346 lumibot-3.4.0/tests/backtest/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/backtest/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      553 2024-05-08 03:43:54.000000 lumibot-3.4.0/tests/backtest/fixtures.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11425 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/backtest/test_example_strategies.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/backtest/test_main_pandas_daily.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    17600 2024-05-08 03:43:54.000000 lumibot-3.4.0/tests/backtest/test_polygon.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/backtest/test_strategy_executor.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1928 2024-05-08 03:43:54.000000 lumibot-3.4.0/tests/backtest/test_yahoo.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_alpaca_old.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_ccxt_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      125 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.4.0/tests/test_order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21416 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_strategy_methods.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    20786 2024-04-10 02:40:36.000000 lumibot-3.4.0/tests/test_tradier.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.4.0/tests/test_tradingfee.py
```

### Comparing `lumibot-3.3.7/LICENSE` & `lumibot-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/PKG-INFO` & `lumibot-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.3.7
+Version: 3.4.0
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lumibot-3.3.7/README.md` & `lumibot-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/__init__.py` & `lumibot-3.4.0/lumibot/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/backtesting/backtesting_broker.py` & `lumibot-3.4.0/lumibot/backtesting/backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/backtesting/polygon_backtesting.py` & `lumibot-3.4.0/lumibot/backtesting/polygon_backtesting.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         logging.info(f"{storage_used = :,} bytes for {len(pandas_data)} items")
         while storage_used > PolygonDataBacktesting.MAX_STORAGE_BYTES:
             k, d = pandas_data.popitem(last=False)
             mu = d.df.memory_usage().sum()
             storage_used -= mu
             logging.info(f"Storage limit exceeded. Evicted LRU data: {k} used {mu:,} bytes")
 
-    def _update_pandas_data(self, asset, quote, length, timestep, start_dt=None, update_data_store=False):
+    def _update_pandas_data(self, asset, quote, length, timestep, start_dt=None):
         """
         Get asset data and update the self.pandas_data dictionary.
 
         Parameters
         ----------
         asset : Asset
             The asset to get data for.
@@ -63,18 +63,14 @@
             The quote asset to use. For example, if asset is "SPY" and quote is "USD", the data will be for "SPY/USD".
         length : int
             The number of data points to get.
         timestep : str
             The timestep to use. For example, "1minute" or "1hour" or "1day".
         start_dt : datetime
             The start datetime to use. If None, the current self.start_datetime will be used.
-        update_data_store : bool
-            If True, the data will also be added to the self._data_store dictionary.
-            That update will not include the adjustments made by PandasData.load_data.
-            See https://github.com/Lumiwealth/lumibot/issues/391 and its PR for further discussion.
         """
         search_asset = asset
         asset_separated = asset
         quote_asset = quote if quote is not None else Asset("USD", "forex")
 
         if isinstance(search_asset, tuple):
             asset_separated, quote_asset = search_asset
@@ -198,36 +194,30 @@
         data = Data(asset_separated, df, timestep=ts_unit, quote=quote_asset)
         pandas_data_update = self._set_pandas_data_keys([data])
 
         # Add the keys to the self.pandas_data dictionary
         self.pandas_data.update(pandas_data_update)
         if PolygonDataBacktesting.MAX_STORAGE_BYTES:
             self._enforce_storage_limit(self.pandas_data)
-        if update_data_store:
-            # TODO: Why do we have both self.pandas_data and self._data_store?
-            self._data_store.update(pandas_data_update)
-            if PolygonDataBacktesting.MAX_STORAGE_BYTES:
-                self._enforce_storage_limit(self._data_store)
 
     def _pull_source_symbol_bars(
         self,
         asset: Asset,
         length: int,
         timestep: str = "day",
         timeshift: int = None,
         quote: Asset = None,
         exchange: str = None,
         include_after_hours: bool = True,
     ):
         # Get the current datetime and calculate the start datetime
         current_dt = self.get_datetime()
-        start_dt, ts_unit = self.get_start_datetime_and_ts_unit(length, timestep, current_dt, start_buffer=START_BUFFER)
 
         # Get data from Polygon
-        self._update_pandas_data(asset, quote, length, timestep, start_dt)
+        self._update_pandas_data(asset, quote, length, timestep, current_dt)
 
         return super()._pull_source_symbol_bars(
             asset, length, timestep, timeshift, quote, exchange, include_after_hours
         )
 
     # Get pricing data for an asset for the entire backtesting period
     def get_historical_prices_between_dates(
@@ -251,15 +241,15 @@
 
         bars = self._parse_source_symbol_bars(response, asset, quote=quote)
         return bars
 
     def get_last_price(self, asset, timestep="minute", quote=None, exchange=None, **kwargs):
         try:
             dt = self.get_datetime()
-            self._update_pandas_data(asset, quote, 1, timestep, dt, update_data_store=True)
+            self._update_pandas_data(asset, quote, 1, timestep, dt)
         except Exception as e:
             print(f"Error get_last_price from Polygon: {e}")
             print(f"Error get_last_price from Polygon: {asset=} {quote=} {timestep=} {dt=} {e}")
 
         return super().get_last_price(asset=asset, quote=quote, exchange=exchange)
 
     def get_chains(self, asset: Asset, quote: Asset = None, exchange: str = None):
```

### Comparing `lumibot-3.3.7/lumibot/brokers/alpaca.py` & `lumibot-3.4.0/lumibot/brokers/alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/brokers/broker.py` & `lumibot-3.4.0/lumibot/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/brokers/ccxt.py` & `lumibot-3.4.0/lumibot/brokers/ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/brokers/interactive_brokers.py` & `lumibot-3.4.0/lumibot/brokers/interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/brokers/tradier.py` & `lumibot-3.4.0/lumibot/brokers/tradier.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,14 +364,15 @@
             time_in_force=response["duration"],
             limit_price=response["price"] if "price" in response and response["price"] else None,
             stop_price=response["stop_price"] if "stop_price" in response and response["stop_price"] else None,
             tag=response["tag"] if "tag" in response and response["tag"] else None,
             date_created=response["create_date"],
         )
         order.status = response["status"]
+        order.avg_fill_price = response.get("avg_fill_price", order.avg_fill_price)
         order.update_raw(response)  # This marks order as 'transmitted'
         return order
 
     def _pull_broker_order(self, identifier):
         """
         This function pulls a single order from the broker by its identifier. Order is converted to a dictionary,
         and then returned. It is expected that the caller will convert the dictionary to an Order object by
```

### Comparing `lumibot-3.3.7/lumibot/data_sources/alpaca_data.py` & `lumibot-3.4.0/lumibot/data_sources/alpaca_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/data_sources/alpha_vantage_data.py` & `lumibot-3.4.0/lumibot/data_sources/alpha_vantage_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/data_sources/ccxt_backtesting_data.py` & `lumibot-3.4.0/lumibot/data_sources/ccxt_backtesting_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/data_sources/ccxt_data.py` & `lumibot-3.4.0/lumibot/data_sources/ccxt_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/data_sources/data_source.py` & `lumibot-3.4.0/lumibot/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/data_sources/data_source_backtesting.py` & `lumibot-3.4.0/lumibot/data_sources/data_source_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/data_sources/exceptions.py` & `lumibot-3.4.0/lumibot/data_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/data_sources/interactive_brokers_data.py` & `lumibot-3.4.0/lumibot/data_sources/interactive_brokers_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/data_sources/pandas_data.py` & `lumibot-3.4.0/lumibot/data_sources/pandas_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,18 @@
     ]
 
     def __init__(self, *args, pandas_data=None, auto_adjust=True, **kwargs):
         super().__init__(*args, **kwargs)
         self.name = "pandas"
         self.pandas_data = self._set_pandas_data_keys(pandas_data)
         self.auto_adjust = auto_adjust
-        self._data_store = OrderedDict()
+        self._data_store = self.pandas_data
         self._date_index = None
         self._date_supply = None
         self._timestep = "minute"
-        self._expiries_exist = False
 
     @staticmethod
     def _set_pandas_data_keys(pandas_data):
         # OrderedDict tracks the LRU dataframes for when it comes time to do evictions.
         new_pandas_data = OrderedDict()
 
         def _get_new_pandas_data_key(data):
@@ -61,17 +60,14 @@
                 key = _get_new_pandas_data_key(data)
                 new_pandas_data[key] = data
 
         return new_pandas_data
     
     def load_data(self):
         self._data_store = self.pandas_data
-        self._expiries_exist = (
-            len([v.asset.expiration for v in self._data_store.values() if v.asset.expiration is not None]) > 0
-        )
         self._date_index = self.update_date_index()
 
         if len(self._data_store.values()) > 0:
             self._timestep = list(self._data_store.values())[0].timestep
 
         pcal = self.get_trading_days_pandas()
         self._date_index = self.clean_trading_times(self._date_index, pcal)
```

### Comparing `lumibot-3.3.7/lumibot/data_sources/tradier_data.py` & `lumibot-3.4.0/lumibot/data_sources/tradier_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/data_sources/yahoo_data.py` & `lumibot-3.4.0/lumibot/data_sources/yahoo_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/entities/asset.py` & `lumibot-3.4.0/lumibot/entities/asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/entities/bar.py` & `lumibot-3.4.0/lumibot/entities/bar.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/entities/bars.py` & `lumibot-3.4.0/lumibot/entities/bars.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/entities/data.py` & `lumibot-3.4.0/lumibot/entities/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -492,14 +492,15 @@
         Returns
         -------
         pandas.DataFrame
 
         """
         # Parse the timestep
         quantity, timestep = parse_timestep_qty_and_unit(timestep)
+        num_periods = length
 
         if timestep == "minute" and self.timestep == "day":
             raise ValueError("You are requesting minute data from a daily data source. This is not supported.")
 
         if timestep != "minute" and timestep != "day":
             raise ValueError(f"Only minute and day are supported for timestep. You provided: {timestep}")
 
@@ -526,14 +527,22 @@
 
         df = pd.DataFrame(data).assign(datetime=lambda df: pd.to_datetime(df['datetime'])).set_index('datetime')
         df_result = df.resample(f"{quantity}{unit}").agg(agg_column_map)
 
         # Drop any rows that have NaN values (this can happen if the data is not complete, eg. weekends)
         df_result = df_result.dropna()
 
+        # Remove partial day data from the current day, which can happen if the data is in minute timestep.
+        if timestep == "day":
+            df_result = df_result[df_result.index < dt.replace(hour=0, minute=0, second=0, microsecond=0)]
+
+        # The original df_result may include more rows when timestep is day and self.timestep is minute.
+        # In this case, we only want to return the last n rows.
+        df_result = df_result.tail(n=num_periods)
+
         return df_result
 
     def get_bars_between_dates(self, timestep=MIN_TIMESTEP, exchange=None, start_date=None, end_date=None):
         """Returns a dataframe of all the data available between the start and end dates.
 
         Parameters
         ----------
```

### Comparing `lumibot-3.3.7/lumibot/entities/order.py` & `lumibot-3.4.0/lumibot/entities/order.py`

 * *Files 0% similar despite different names*

```diff
@@ -545,15 +545,15 @@
     def quantity(self, value):
         # All non-crypto assets must be of type 'int'.
         if not isinstance(value, Decimal):
             if isinstance(value, float):
                 value = Decimal(str(value))
 
         quantity = Decimal(value)
-        self._quantity = check_quantity(quantity, "Order quantity must be a positive Decimal")
+        self._quantity = quantity
 
     def __hash__(self):
         return hash(self.identifier)
 
     # Compares two order objects to see if they are the same.
     def __eq__(self, other):
         # If the other object is not an Order object, then they are not equal.
```

### Comparing `lumibot-3.3.7/lumibot/entities/position.py` & `lumibot-3.4.0/lumibot/entities/position.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/entities/trading_fee.py` & `lumibot-3.4.0/lumibot/entities/trading_fee.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/ccxt_backtesting_example.py` & `lumibot-3.4.0/lumibot/example_strategies/ccxt_backtesting_example.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/crypto_important_functions.py` & `lumibot-3.4.0/lumibot/example_strategies/crypto_important_functions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/options_hold_to_expiry.py` & `lumibot-3.4.0/lumibot/example_strategies/options_hold_to_expiry.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/simple_start_single_file.py` & `lumibot-3.4.0/lumibot/example_strategies/simple_start_single_file.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/stock_bracket.py` & `lumibot-3.4.0/lumibot/example_strategies/stock_bracket.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/stock_buy_and_hold.py` & `lumibot-3.4.0/lumibot/example_strategies/stock_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/stock_diversified_leverage.py` & `lumibot-3.4.0/lumibot/example_strategies/stock_diversified_leverage.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/stock_limit_and_trailing_stops.py` & `lumibot-3.4.0/lumibot/example_strategies/stock_limit_and_trailing_stops.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/stock_momentum.py` & `lumibot-3.4.0/lumibot/example_strategies/stock_momentum.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/stock_oco.py` & `lumibot-3.4.0/lumibot/example_strategies/stock_oco.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/example_strategies/strangle.py` & `lumibot-3.4.0/lumibot/example_strategies/strangle.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/strategies/_strategy.py` & `lumibot-3.4.0/lumibot/strategies/_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,14 +699,15 @@
             create_tearsheet(
                 self._strategy_returns_df,
                 strat_name,
                 tearsheet_file,
                 self._benchmark_returns_df,
                 self._benchmark_asset,
                 show_tearsheet,
+                save_tearsheet,
                 risk_free_rate=self.risk_free_rate,
                 strategy_parameters=strategy_parameters,
             )
 
     @classmethod
     def run_backtest(
         cls,
@@ -1003,14 +1004,15 @@
         start = datetime.datetime.now()
 
         result = trader.run_all(
             show_plot=show_plot,
             show_tearsheet=show_tearsheet,
             save_tearsheet=save_tearsheet,
             show_indicators=show_indicators,
+            tearsheet_file=tearsheet_file,
         )
 
         end = datetime.datetime.now()
         backtesting_length = backtesting_end - backtesting_start
         backtesting_run_time = end - start
         logger.info(
             f"Backtest took {backtesting_run_time} for a speed of {backtesting_run_time / backtesting_length:,.3f}"
```

### Comparing `lumibot-3.3.7/lumibot/strategies/strategy.py` & `lumibot-3.4.0/lumibot/strategies/strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,26 +323,21 @@
         return self._stats
 
     @property
     def analysis(self):
         return self._analysis
 
     @property
-    def risk_free_rate(self):
-        rfr = 0
+    def risk_free_rate(self) -> float:
         if self._risk_free_rate is not None:
-            rfr = self._risk_free_rate
+            return self._risk_free_rate
         else:
-            # Get the current datetime
+            # Use the yahoo data to get the risk free rate, or 0 if None is returned
             now = self.get_datetime()
-
-            # Use the yahoo data to get the risk free rate
-            rfr = get_risk_free_rate(now)
-        
-        return rfr
+            return get_risk_free_rate(now) or 0.0
 
     # ======= Helper Methods =======================
 
     def log_message(self, message, color=None, broadcast=False):
         """Logs an info message prefixed with the strategy name.
 
         Uses python logging to log the message at the `info` level.
```

### Comparing `lumibot-3.3.7/lumibot/strategies/strategy_executor.py` & `lumibot-3.4.0/lumibot/strategies/strategy_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -764,14 +764,18 @@
             if self.broker.IS_BACKTESTING_BROKER:
                 self.broker.process_pending_orders(strategy=self.strategy)
             return
 
         if not is_247:
             # Set date to the start date, but account for minutes_before_opening
             self.strategy.await_market_to_open()  # set new time and bar length. Check if hit bar max or date max.
+            # Check if we should continue to run when we are in a new day.
+            broker_continue = self.broker.should_continue()
+            if not broker_continue:
+                return
 
             if not has_data_source or (has_data_source and self.broker.data_source.SOURCE != "PANDAS"):
                 self.strategy._update_cash_with_dividends()
 
             if not self.broker.is_market_open():
                 self._before_market_opens()
```

### Comparing `lumibot-3.3.7/lumibot/tools/__init__.py` & `lumibot-3.4.0/lumibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/tools/black_scholes.py` & `lumibot-3.4.0/lumibot/tools/black_scholes.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/tools/ccxt_data_store.py` & `lumibot-3.4.0/lumibot/tools/ccxt_data_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/tools/decorators.py` & `lumibot-3.4.0/lumibot/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/tools/helpers.py` & `lumibot-3.4.0/lumibot/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/tools/indicators.py` & `lumibot-3.4.0/lumibot/tools/indicators.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,20 +635,22 @@
 def create_tearsheet(
     strategy_df: pd.DataFrame,
     strat_name: str,
     tearsheet_file: str,
     benchmark_df: pd.DataFrame,
     benchmark_asset,  # This is causing a circular import: Asset,
     show_tearsheet: bool,
+    save_tearsheet: bool,
     risk_free_rate: float,
     strategy_parameters: dict = None,
 ):
     # If show tearsheet is False, then we don't want to open the tearsheet in the browser
-    if not show_tearsheet:
-        print("show_tearsheet is False, not creating the tearsheet file.")
+    # IMS create the tearsheet even if we are not showinbg it
+    if not save_tearsheet:
+        print("save_tearsheet is False, not creating the tearsheet file.")
         return
 
     print("\nCreating tearsheet...")
 
     # Check if df1 or df2 are empty and return if they are
     if strategy_df is None or benchmark_df is None or strategy_df.empty or benchmark_df.empty:
         logging.error("No data to create tearsheet, skipping")
```

### Comparing `lumibot-3.3.7/lumibot/tools/lumibot_time.py` & `lumibot-3.4.0/lumibot/tools/lumibot_time.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/tools/pandas.py` & `lumibot-3.4.0/lumibot/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/tools/polygon_helper.py` & `lumibot-3.4.0/lumibot/tools/polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/tools/types.py` & `lumibot-3.4.0/lumibot/tools/types.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/tools/yahoo_helper.py` & `lumibot-3.4.0/lumibot/tools/yahoo_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,16 @@
             pickle_file_path = os.path.join(YahooHelper.LUMIBOT_YAHOO_CACHE_FOLDER, file_name)
             if os.path.exists(pickle_file_path):
                 try:
                     with open(pickle_file_path, "rb") as f:
                         return pickle.load(f)
                 except Exception as e:
                     logging.error("Error while loading pickle file %s: %s" % (pickle_file_path, e))
+                    # Remove the file because it is corrupted.  This will enable re-download.
+                    os.remove(pickle_file_path)
                     return None
 
         return None
 
     @staticmethod
     def dump_pickle_file(symbol, type, data):
         if YahooHelper.CACHING_ENABLED:
```

### Comparing `lumibot-3.3.7/lumibot/traders/trader.py` & `lumibot-3.4.0/lumibot/traders/trader.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             result = True
         return result
 
     def add_strategy(self, strategy):
         """Adds a strategy to the trader"""
         self._strategies.append(strategy)
 
-    def run_all(self, async_=False, show_plot=True, show_tearsheet=True, save_tearsheet=True, show_indicators=True):
+    def run_all(self, async_=False, show_plot=True, show_tearsheet=True, save_tearsheet=True, show_indicators=True, tearsheet_file=""):
         """
         run all strategies
 
         Parameters
         ----------
         async_: bool
             Whether to run the strategies asynchronously or not. This is not implemented yet.
@@ -121,14 +121,15 @@
             logging.info("Backtesting finished")
             strat.backtest_analysis(
                 logdir=self.logdir,
                 show_plot=show_plot,
                 show_tearsheet=show_tearsheet,
                 save_tearsheet=save_tearsheet,
                 show_indicators=show_indicators,
+                tearsheet_file=tearsheet_file,
             )
 
         return result
 
     # Async version of run_all
     def run_all_async(self, backtest=False):
         """run all strategies"""
```

### Comparing `lumibot-3.3.7/lumibot/trading_builtins/custom_stream.py` & `lumibot-3.4.0/lumibot/trading_builtins/custom_stream.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot/trading_builtins/safe_list.py` & `lumibot-3.4.0/lumibot/trading_builtins/safe_list.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/lumibot.egg-info/PKG-INFO` & `lumibot-3.4.0/lumibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.3.7
+Version: 3.4.0
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lumibot-3.3.7/lumibot.egg-info/SOURCES.txt` & `lumibot-3.4.0/lumibot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -88,12 +88,13 @@
 tests/test_interactive_brokers.py
 tests/test_order.py
 tests/test_polygon_helper.py
 tests/test_strategy_methods.py
 tests/test_tradier.py
 tests/test_tradingfee.py
 tests/backtest/__init__.py
+tests/backtest/fixtures.py
 tests/backtest/test_example_strategies.py
 tests/backtest/test_main_pandas_daily.py
 tests/backtest/test_polygon.py
 tests/backtest/test_strategy_executor.py
 tests/backtest/test_yahoo.py
```

### Comparing `lumibot-3.3.7/lumibot.egg-info/requires.txt` & `lumibot-3.4.0/lumibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/pyproject.toml` & `lumibot-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/setup.cfg` & `lumibot-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/setup.py` & `lumibot-3.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lumibot",
-    version="3.3.7",
+    version="3.4.0",
     author="Robert Grzesik",
     author_email="rob@lumiwealth.com",
     description="Backtesting and Trading Library, Made by Lumiwealth",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lumiwealth/lumibot",
     packages=setuptools.find_packages(),
@@ -31,15 +31,15 @@
         "flask-sqlalchemy",
         "flask-marshmallow",
         "flask-security",
         "marshmallow-sqlalchemy",
         "email_validator",
         "bcrypt",
         "pytest",
-        "scipy>=1.13.0",  # Newer versions of scipy are currently causing issues
+        "scipy>=1.13.0",
         "ipython",  # required for quantstats, but not in their dependency list for some reason
         "quantstats-lumi>=0.2.0",
         "python-dotenv",  # Secret Storage
         "ccxt==4.2.85",
         "termcolor",
         "jsonpickle",
         "apscheduler==3.10.4",
```

### Comparing `lumibot-3.3.7/tests/backtest/test_example_strategies.py` & `lumibot-3.4.0/tests/backtest/test_example_strategies.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/backtest/test_main_pandas_daily.py` & `lumibot-3.4.0/tests/backtest/test_main_pandas_daily.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/backtest/test_polygon.py` & `lumibot-3.4.0/tests/backtest/test_polygon.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import datetime
 import os
 from collections import defaultdict
+import pandas as pd
 
 import pandas_market_calendars as mcal
 
+from tests.backtest.fixtures import polygon_data_backtesting
+import pytz
 from lumibot.backtesting import BacktestingBroker, PolygonDataBacktesting
 from lumibot.entities import Asset
 from lumibot.strategies import Strategy
 from lumibot.traders import Trader
 
+from unittest.mock import MagicMock, patch
+from datetime import timedelta
+
 # Global parameters
 # API Key for testing Polygon.io
 POLYGON_API_KEY = os.environ.get("POLYGON_API_KEY")
 
 
 class PolygonBacktestStrat(Strategy):
     parameters = {"symbol": "AMZN"}
 
     # Set the initial values for the strategy
-    def initialize(self, parameters=None):
-        self.sleeptime = "1D"
+    def initialize(self, custom_sleeptime="1D"):
+        self.sleeptime = custom_sleeptime
         self.first_price = None
         self.first_option_price = None
         self.orders = []
         self.prices = {}
         self.chains = {}
         self.market_opens_called = False
         self.market_closes_called = False
@@ -211,19 +217,43 @@
         )
         broker = BacktestingBroker(data_source=data_source)
         poly_strat_obj = PolygonBacktestStrat(
             broker=broker,
         )
         trader = Trader(logfile="", backtest=True)
         trader.add_strategy(poly_strat_obj)
-        results = trader.run_all(show_plot=False, show_tearsheet=False, save_tearsheet=False)
+        results = trader.run_all(show_plot=False, show_tearsheet=False, save_tearsheet=False, tearsheet_file="")
 
         assert results
         self.verify_backtest_results(poly_strat_obj)
 
+    def test_intraday_daterange(self):
+        tzinfo = pytz.timezone("America/New_York")
+        backtesting_start = datetime.datetime(2024, 2, 7).astimezone(tzinfo)
+        backtesting_end = datetime.datetime(2024, 2, 10).astimezone(tzinfo)
+
+        data_source = PolygonDataBacktesting(
+            datetime_start=backtesting_start,
+            datetime_end=backtesting_end,
+            api_key=POLYGON_API_KEY,
+            has_paid_subscription=True,
+        )
+        broker = BacktestingBroker(data_source=data_source)
+        poly_strat_obj = PolygonBacktestStrat(
+            broker=broker,
+            custom_sleeptime="30m",  # Sleep time for intra-day trading.
+        )
+        trader = Trader(logfile="", backtest=True)
+        trader.add_strategy(poly_strat_obj)
+        results = trader.run_all(show_plot=False, show_tearsheet=False, save_tearsheet=False, tearsheet_file="")
+        # Assert the results are not empty
+        assert results
+        # Assert the end datetime is before the market open of the next trading day.
+        assert broker.datetime == datetime.datetime.fromisoformat("2024-02-12 08:30:00-05:00")
+
     def test_polygon_legacy_backtest(self):
         """
         Do the same backtest as test_polygon_restclient() but using the legacy backtest() function call instead of
         trader.run_all(backtest=True) (which is the new standard way to run backtests).
         """
 
         # Parameters: True = Live Trading | False = Backtest
@@ -268,7 +298,91 @@
             save_tearsheet=False,
             polygon_api_key=POLYGON_API_KEY,  # Testing the legacy parameter name while DeprecationWarning is active
             # Painfully slow with free subscription setting b/c lumibot is over querying and imposing a very
             # strict rate limit
             polygon_has_paid_subscription=True,
         )
         assert results
+
+    def test_pull_source_symbol_bars_with_api_call(self, polygon_data_backtesting, mocker):
+        """Test that polygon_helper.get_price_data_from_polygon() is called with the right parameters"""
+        
+        # Only simulate first date
+        mocker.patch.object(
+            polygon_data_backtesting,
+            'get_datetime',
+            return_value=polygon_data_backtesting.datetime_start
+        )
+
+        mocked_get_price_data = mocker.patch(
+            'lumibot.tools.polygon_helper.get_price_data_from_polygon',
+            return_value=MagicMock()
+        )
+        
+        asset = Asset(symbol="AAPL", asset_type="stock")
+        quote = Asset(symbol="USD", asset_type="forex")
+        length = 10
+        timestep = "day"
+        START_BUFFER = timedelta(days=5)
+
+        with patch('lumibot.backtesting.polygon_backtesting.START_BUFFER', new=START_BUFFER):
+            polygon_data_backtesting._pull_source_symbol_bars(
+                asset=asset,
+                length=length,
+                timestep=timestep,
+                quote=quote
+            )
+
+            mocked_get_price_data.assert_called_once()
+            call_args = mocked_get_price_data.call_args
+            
+            expected_start_date = polygon_data_backtesting.datetime_start - datetime.timedelta(days=length) - START_BUFFER
+            
+            assert call_args[0][0] == polygon_data_backtesting._api_key
+            assert call_args[0][1] == asset
+            assert call_args[0][2] == expected_start_date
+            assert call_args[0][3] == polygon_data_backtesting.datetime_end
+            assert call_args[1]["timespan"] == timestep
+            assert call_args[1]["quote_asset"] == quote
+            assert call_args[1]["has_paid_subscription"] == polygon_data_backtesting.has_paid_subscription
+
+
+class TestPolygonDataSource:
+
+    def test_get_historical_prices(self):
+        tzinfo = pytz.timezone("America/New_York")
+        start = datetime.datetime(2024, 2, 5).astimezone(tzinfo)
+        end = datetime.datetime(2024, 2, 10).astimezone(tzinfo)
+
+        data_source = PolygonDataBacktesting(
+            start, end, api_key=POLYGON_API_KEY, has_paid_subscription=True
+        )
+        data_source._datetime = datetime.datetime(2024, 2, 7, 10).astimezone(tzinfo)
+        # This call will set make the data source use minute bars.
+        prices = data_source.get_historical_prices("SPY", 2, "minute")
+        # The data source will aggregate day bars from the minute bars.
+        prices = data_source.get_historical_prices("SPY", 2, "day")
+
+        # The expected df contains 2 days of data. And it is most recent from the
+        # past of the requested date.
+        expected_df = pd.DataFrame.from_records([
+            {
+                "datetime": "2024-02-05 00:00:00-05:00",
+                "open": 493.65,
+                "high": 494.3778,
+                "low": 490.23,
+                "close": 492.57,
+                "volume": 74655145.0
+            },
+            {
+                "datetime": "2024-02-06 00:00:00-05:00",
+                "open": 492.99,
+                "high": 494.3200,
+                "low": 492.03,
+                "close": 493.82,
+                "volume": 54775803.0
+            },
+        ], index="datetime")
+        expected_df.index = pd.to_datetime(expected_df.index).tz_convert(tzinfo)
+
+        assert prices is not None
+        assert prices.df.equals(expected_df)
```

### Comparing `lumibot-3.3.7/tests/backtest/test_strategy_executor.py` & `lumibot-3.4.0/tests/backtest/test_strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/backtest/test_yahoo.py` & `lumibot-3.4.0/tests/backtest/test_yahoo.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             broker=broker,
             backtesting_start=backtesting_start,
             backtesting_end=backtesting_end,
         )
 
         trader = Trader(logfile="", backtest=True)
         trader.add_strategy(poly_strat_obj)
-        results = trader.run_all(show_plot=False, show_tearsheet=False, save_tearsheet=False)
+        results = trader.run_all(show_plot=False, show_tearsheet=False, save_tearsheet=False, tearsheet_file="")
 
         assert results
 
         last_price = poly_strat_obj.last_price
         # Round to 2 decimal places
         last_price = round(last_price, 2)
```

### Comparing `lumibot-3.3.7/tests/test_alpaca.py` & `lumibot-3.4.0/tests/test_alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_alpaca_old.py` & `lumibot-3.4.0/tests/test_alpaca_old.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_asset.py` & `lumibot-3.4.0/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_backtesting_broker.py` & `lumibot-3.4.0/tests/test_backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_ccxt.py` & `lumibot-3.4.0/tests/test_ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_ccxt_store.py` & `lumibot-3.4.0/tests/test_ccxt_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_interactive_brokers.py` & `lumibot-3.4.0/tests/test_interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_order.py` & `lumibot-3.4.0/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_polygon_helper.py` & `lumibot-3.4.0/tests/test_polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_strategy_methods.py` & `lumibot-3.4.0/tests/test_strategy_methods.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.3.7/tests/test_tradier.py` & `lumibot-3.4.0/tests/test_tradier.py`

 * *Files identical despite different names*


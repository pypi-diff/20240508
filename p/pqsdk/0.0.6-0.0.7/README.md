# Comparing `tmp/pqsdk-0.0.6.tar.gz` & `tmp/pqsdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqsdk-0.0.6.tar", last modified: Mon May  6 11:09:20 2024, max compression
+gzip compressed data, was "pqsdk-0.0.7.tar", last modified: Wed May  8 03:30:00 2024, max compression
```

## Comparing `pqsdk-0.0.6.tar` & `pqsdk-0.0.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 11:09:20.011438 pqsdk-0.0.6/
--rw-rw-rw-   0        0        0      766 2024-05-06 11:09:20.010438 pqsdk-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.885438 pqsdk-0.0.6/pqsdk/
--rw-rw-rw-   0        0        0      190 2024-05-06 11:07:04.000000 pqsdk-0.0.6/pqsdk/__init__.py
--rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.6/pqsdk/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.904438 pqsdk-0.0.6/pqsdk/api/
--rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.6/pqsdk/api/__init__.py
--rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.6/pqsdk/api/main.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.945437 pqsdk-0.0.6/pqsdk/backtest/
--rw-rw-rw-   0        0        0     3196 2024-04-10 08:16:12.000000 pqsdk-0.0.6/pqsdk/backtest/__init__.py
--rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/backtest/analyzer.py
--rw-rw-rw-   0        0        0    35704 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/context.py
--rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/current_data.py
--rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/instrument.py
--rw-rw-rw-   0        0        0    14082 2024-04-20 12:07:11.000000 pqsdk-0.0.6/pqsdk/backtest/main.py
--rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.6/pqsdk/backtest/order.py
--rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/portfolio.py
--rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/position.py
--rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/run_info.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.948438 pqsdk-0.0.6/pqsdk/enums/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/enums/__init__.py
--rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.6/pqsdk/enums/orderStatus.py
--rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/faxconstant.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.984437 pqsdk-0.0.6/pqsdk/interface/
--rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/__init__.py
--rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractInstrument.py
--rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.6/pqsdk/interface/abstractOrder.py
--rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractPortfolio.py
--rw-rw-rw-   0        0        0     1677 2024-04-20 13:04:56.000000 pqsdk-0.0.6/pqsdk/interface/abstractPosition.py
--rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractRunInfo.py
--rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractStrategyContext.py
--rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractTrader.py
--rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.6/pqsdk/interface/constant.py
--rw-rw-rw-   0        0        0     5757 2024-05-05 10:11:04.000000 pqsdk-0.0.6/pqsdk/logger.py
--rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.6/pqsdk/main.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:09:20.002437 pqsdk-0.0.6/pqsdk/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/__init__.py
--rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/dynamic_import.py
--rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/file_util.py
--rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/import_global_modules.py
--rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/utils/timer_factory.py
--rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/value_type_util.py
--rw-rw-rw-   0        0        0      441 2024-05-06 11:09:16.000000 pqsdk-0.0.6/pqsdk/version.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:09:20.010438 pqsdk-0.0.6/pqsdk.egg-info/
--rw-rw-rw-   0        0        0      766 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1193 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      183 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 11:09:20.011438 pqsdk-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1599 2024-04-12 14:22:50.000000 pqsdk-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 11:09:20.009438 pqsdk-0.0.6/tests/
--rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.6/tests/test_backtest.py
--rw-rw-rw-   0        0        0     2137 2024-05-05 08:03:23.000000 pqsdk-0.0.6/tests/test_pqsdk_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:30:00.636013 pqsdk-0.0.7/
+-rw-rw-rw-   0        0        0      766 2024-05-08 03:30:00.635507 pqsdk-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 03:30:00.464035 pqsdk-0.0.7/pqsdk/
+-rw-rw-rw-   0        0        0      190 2024-05-06 11:07:04.000000 pqsdk-0.0.7/pqsdk/__init__.py
+-rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.7/pqsdk/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:30:00.492625 pqsdk-0.0.7/pqsdk/api/
+-rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.7/pqsdk/api/__init__.py
+-rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.7/pqsdk/api/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:30:00.543733 pqsdk-0.0.7/pqsdk/backtest/
+-rw-rw-rw-   0        0        0     3196 2024-04-10 08:16:12.000000 pqsdk-0.0.7/pqsdk/backtest/__init__.py
+-rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/backtest/analyzer.py
+-rw-rw-rw-   0        0        0    35709 2024-05-07 11:11:40.000000 pqsdk-0.0.7/pqsdk/backtest/context.py
+-rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.7/pqsdk/backtest/current_data.py
+-rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.7/pqsdk/backtest/instrument.py
+-rw-rw-rw-   0        0        0    14065 2024-05-08 03:27:07.000000 pqsdk-0.0.7/pqsdk/backtest/main.py
+-rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.7/pqsdk/backtest/order.py
+-rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.7/pqsdk/backtest/portfolio.py
+-rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.7/pqsdk/backtest/position.py
+-rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.7/pqsdk/backtest/run_info.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:30:00.549257 pqsdk-0.0.7/pqsdk/enums/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/enums/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.7/pqsdk/enums/orderStatus.py
+-rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/faxconstant.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:30:00.603356 pqsdk-0.0.7/pqsdk/interface/
+-rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/interface/__init__.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/interface/abstractInstrument.py
+-rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.7/pqsdk/interface/abstractOrder.py
+-rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/interface/abstractPortfolio.py
+-rw-rw-rw-   0        0        0     1677 2024-04-20 13:04:56.000000 pqsdk-0.0.7/pqsdk/interface/abstractPosition.py
+-rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/interface/abstractRunInfo.py
+-rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/interface/abstractStrategyContext.py
+-rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/interface/abstractTrader.py
+-rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.7/pqsdk/interface/constant.py
+-rw-rw-rw-   0        0        0     5757 2024-05-05 10:11:04.000000 pqsdk-0.0.7/pqsdk/logger.py
+-rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.7/pqsdk/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:30:00.632778 pqsdk-0.0.7/pqsdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/utils/dynamic_import.py
+-rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/utils/file_util.py
+-rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/utils/import_global_modules.py
+-rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.7/pqsdk/utils/timer_factory.py
+-rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.7/pqsdk/utils/value_type_util.py
+-rw-rw-rw-   0        0        0      441 2024-05-08 03:28:15.000000 pqsdk-0.0.7/pqsdk/version.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:30:00.482694 pqsdk-0.0.7/pqsdk.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-05-08 03:30:00.000000 pqsdk-0.0.7/pqsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2024-05-08 03:30:00.000000 pqsdk-0.0.7/pqsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 03:30:00.000000 pqsdk-0.0.7/pqsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-08 03:30:00.000000 pqsdk-0.0.7/pqsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      183 2024-05-08 03:30:00.000000 pqsdk-0.0.7/pqsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 03:30:00.000000 pqsdk-0.0.7/pqsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 03:30:00.636520 pqsdk-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2024-04-12 14:22:50.000000 pqsdk-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 03:30:00.634425 pqsdk-0.0.7/tests/
+-rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.7/tests/test_backtest.py
+-rw-rw-rw-   0        0        0     2137 2024-05-05 08:03:23.000000 pqsdk-0.0.7/tests/test_pqsdk_api.py
```

### Comparing `pqsdk-0.0.6/PKG-INFO` & `pqsdk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.6/pqsdk/__main__.py` & `pqsdk-0.0.7/pqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/api/__init__.py` & `pqsdk-0.0.7/pqsdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/api/main.py` & `pqsdk-0.0.7/pqsdk/api/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/backtest/__init__.py` & `pqsdk-0.0.7/pqsdk/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/backtest/analyzer.py` & `pqsdk-0.0.7/pqsdk/backtest/analyzer.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/backtest/context.py` & `pqsdk-0.0.7/pqsdk/backtest/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,15 @@
         pass
 
     def get_blacklist(self) -> list:
         """
         TODO 获取租户下定义的股票列表黑名单，黑名单的股票不建议持仓
         :return:
         """
-        pass
+        return []
 
     def set_benchmark_value(self, value: float):
         """
         设置回测过程中当前日期的benchmark close价格
         :param value:
         :return:
         """
```

### Comparing `pqsdk-0.0.6/pqsdk/backtest/current_data.py` & `pqsdk-0.0.7/pqsdk/backtest/current_data.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/backtest/instrument.py` & `pqsdk-0.0.7/pqsdk/backtest/instrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/backtest/main.py` & `pqsdk-0.0.7/pqsdk/backtest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         file_path = f"{self.params.get('save_path', 'storage')}/logs/"
         fu.create_dir(path=file_path)
         file_name = f'run_backtest_'
         strat_run_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         file_name += "__time=" + strat_run_time.replace("-", "").replace(":", "").replace(" ", "_") + ".log"
         log_path = file_path + file_name
         # 配置log输出到文件
-        log.add_file_handler(name='strategy', file_name=log_path, level=log.DEBUG)
+        log.add_file_handler(file_name=log_path, level=log.DEBUG)
 
     def add_analyzer(self, name: str, analyzer: Callable):
         self.analyzers[name] = analyzer().set_context(self.context)
 
     def initialize(self, context):
         """
         初始化方法，在整个回测、模拟实盘中最开始执行一次，用于初始一些全局变量，全局变量会被持久化。重启策略不会再次执行。
```

### Comparing `pqsdk-0.0.6/pqsdk/backtest/order.py` & `pqsdk-0.0.7/pqsdk/backtest/order.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/backtest/portfolio.py` & `pqsdk-0.0.7/pqsdk/backtest/portfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/backtest/position.py` & `pqsdk-0.0.7/pqsdk/backtest/position.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/backtest/run_info.py` & `pqsdk-0.0.7/pqsdk/backtest/run_info.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/enums/orderStatus.py` & `pqsdk-0.0.7/pqsdk/enums/orderStatus.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/faxconstant.py` & `pqsdk-0.0.7/pqsdk/faxconstant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/interface/__init__.py` & `pqsdk-0.0.7/pqsdk/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/interface/abstractInstrument.py` & `pqsdk-0.0.7/pqsdk/interface/abstractInstrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/interface/abstractOrder.py` & `pqsdk-0.0.7/pqsdk/interface/abstractOrder.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/interface/abstractPortfolio.py` & `pqsdk-0.0.7/pqsdk/interface/abstractPortfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/interface/abstractPosition.py` & `pqsdk-0.0.7/pqsdk/interface/abstractPosition.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/interface/abstractRunInfo.py` & `pqsdk-0.0.7/pqsdk/interface/abstractRunInfo.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/interface/abstractStrategyContext.py` & `pqsdk-0.0.7/pqsdk/interface/abstractStrategyContext.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/interface/abstractTrader.py` & `pqsdk-0.0.7/pqsdk/interface/abstractTrader.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/interface/constant.py` & `pqsdk-0.0.7/pqsdk/interface/constant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/logger.py` & `pqsdk-0.0.7/pqsdk/logger.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/main.py` & `pqsdk-0.0.7/pqsdk/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/utils/dynamic_import.py` & `pqsdk-0.0.7/pqsdk/utils/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/utils/file_util.py` & `pqsdk-0.0.7/pqsdk/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/utils/timer_factory.py` & `pqsdk-0.0.7/pqsdk/utils/timer_factory.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk/utils/value_type_util.py` & `pqsdk-0.0.7/pqsdk/utils/value_type_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/pqsdk.egg-info/PKG-INFO` & `pqsdk-0.0.7/pqsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.6/pqsdk.egg-info/SOURCES.txt` & `pqsdk-0.0.7/pqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/setup.py` & `pqsdk-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.6/tests/test_pqsdk_api.py` & `pqsdk-0.0.7/tests/test_pqsdk_api.py`

 * *Files identical despite different names*


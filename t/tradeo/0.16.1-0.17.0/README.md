# Comparing `tmp/tradeo-0.16.1.tar.gz` & `tmp/tradeo-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradeo-0.16.1.tar", max compression
+gzip compressed data, was "tradeo-0.17.0.tar", max compression
```

## Comparing `tradeo-0.16.1.tar` & `tradeo-0.17.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rwxr-xr-x   0        0        0     1524 2024-04-16 16:51:11.931913 tradeo-0.16.1/LICENSE
--rwxr-xr-x   0        0        0     4282 2024-04-27 14:06:45.230649 tradeo-0.16.1/README.md
--rwxr-xr-x   0        0        0     1091 2024-04-27 14:33:09.872168 tradeo-0.16.1/pyproject.toml
--rwxr-xr-x   0        0        0     1208 2024-04-27 12:51:46.561193 tradeo-0.16.1/tradeo/__init__.py
--rwxr-xr-x   0        0        0      353 2024-04-27 12:51:46.576817 tradeo-0.16.1/tradeo/bash/launch-mt5.sh
--rwxr-xr-x   0        0        0      172 2024-04-27 12:51:46.576817 tradeo-0.16.1/tradeo/bash/stop-mt.sh
--rwxr-xr-x   0        0        0     2569 2024-04-27 12:51:46.592441 tradeo-0.16.1/tradeo/config.py
--rwxr-xr-x   0        0        0        0 2024-04-27 12:51:46.592441 tradeo-0.16.1/tradeo/context_managers/__init__.py
--rwxr-xr-x   0        0        0      677 2024-04-27 12:51:46.608066 tradeo-0.16.1/tradeo/context_managers/blocker.py
--rwxr-xr-x   0        0        0        1 2024-04-27 12:51:46.608066 tradeo-0.16.1/tradeo/data/consecutive_times_down.txt
--rwxr-xr-x   0        0        0        1 2024-04-27 12:51:46.608066 tradeo-0.16.1/tradeo/data/last_balance.txt
--rwxr-xr-x   0        0        0        0 2024-04-27 12:51:46.623692 tradeo-0.16.1/tradeo/event_handlers/__init__.py
--rwxr-xr-x   0        0        0     1106 2024-04-27 12:51:46.623692 tradeo-0.16.1/tradeo/event_handlers/basic_event_handler.py
--rwxr-xr-x   0        0        0     1699 2024-04-27 12:51:46.639316 tradeo-0.16.1/tradeo/event_handlers/event_handler.py
--rwxr-xr-x   0        0        0     5883 2024-04-27 12:51:46.654941 tradeo-0.16.1/tradeo/executable/basic_forex.py
--rwxr-xr-x   0        0        0     1087 2024-04-27 12:51:46.654941 tradeo-0.16.1/tradeo/executable/executable.py
--rwxr-xr-x   0        0        0     2129 2024-04-27 12:51:46.671274 tradeo-0.16.1/tradeo/files.py
--rwxr-xr-x   0        0        0     2389 2024-04-27 12:51:46.671274 tradeo-0.16.1/tradeo/log.py
--rwxr-xr-x   0        0        0    24061 2024-04-27 12:51:46.687557 tradeo-0.16.1/tradeo/mt_client.py
--rwxr-xr-x   0        0        0     1388 2024-04-27 12:51:46.694566 tradeo-0.16.1/tradeo/mt_message.py
--rwxr-xr-x   0        0        0    45319 2024-04-27 12:51:46.702566 tradeo-0.16.1/tradeo/mt_tb_expert.mq5
--rwxr-xr-x   0        0        0      427 2024-04-27 12:51:46.703097 tradeo-0.16.1/tradeo/ohlc.py
--rwxr-xr-x   0        0        0     4286 2024-04-27 12:51:46.703097 tradeo-0.16.1/tradeo/order.py
--rwxr-xr-x   0        0        0      268 2024-04-27 12:51:46.718722 tradeo-0.16.1/tradeo/order_operations.py
--rwxr-xr-x   0        0        0     2161 2024-04-27 12:51:46.718722 tradeo-0.16.1/tradeo/order_type.py
--rwxr-xr-x   0        0        0      750 2024-04-27 12:51:46.734347 tradeo-0.16.1/tradeo/paths.py
--rwxr-xr-x   0        0        0      319 2024-04-27 12:51:46.734347 tradeo-0.16.1/tradeo/singleton.py
--rwxr-xr-x   0        0        0        0 2024-04-27 12:51:46.749972 tradeo-0.16.1/tradeo/strategies/__init__.py
--rwxr-xr-x   0        0        0     2417 2024-04-27 12:51:46.749972 tradeo-0.16.1/tradeo/strategies/basic_strategy.py
--rwxr-xr-x   0        0        0     4551 2024-04-27 12:51:46.765597 tradeo-0.16.1/tradeo/strategies/strategy.py
--rwxr-xr-x   0        0        0     5847 2024-04-27 12:51:46.765597 tradeo-0.16.1/tradeo/trading_methods.py
--rwxr-xr-x   0        0        0     2000 2024-04-27 12:51:46.796952 tradeo-0.16.1/tradeo/utils.py
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 tradeo-0.16.1/PKG-INFO
+-rw-r--r--   0        0        0     1524 2024-05-08 15:51:10.507547 tradeo-0.17.0/LICENSE
+-rw-r--r--   0        0        0     4282 2024-05-08 15:51:10.507547 tradeo-0.17.0/README.md
+-rw-r--r--   0        0        0     1095 2024-05-08 15:51:10.511546 tradeo-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0     1208 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/__init__.py
+-rw-r--r--   0        0        0      353 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/bash/launch-mt5.sh
+-rw-r--r--   0        0        0      172 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/bash/stop-mt.sh
+-rw-r--r--   0        0        0     2569 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/config.py
+-rw-r--r--   0        0        0        0 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/context_managers/__init__.py
+-rw-r--r--   0        0        0      677 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/context_managers/blocker.py
+-rw-r--r--   0        0        0        1 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/data/consecutive_times_down.txt
+-rw-r--r--   0        0        0        1 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/data/last_balance.txt
+-rw-r--r--   0        0        0        0 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/event_handlers/__init__.py
+-rw-r--r--   0        0        0     1106 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/event_handlers/basic_event_handler.py
+-rw-r--r--   0        0        0     1699 2024-05-08 15:51:10.511546 tradeo-0.17.0/tradeo/event_handlers/event_handler.py
+-rw-r--r--   0        0        0     5899 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/executable/basic_forex.py
+-rw-r--r--   0        0        0     1087 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/executable/executable.py
+-rw-r--r--   0        0        0     2129 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/files.py
+-rw-r--r--   0        0        0     2389 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/log.py
+-rw-r--r--   0        0        0    24080 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/mt_client.py
+-rw-r--r--   0        0        0     1984 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/mt_message.py
+-rw-r--r--   0        0        0    45319 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/mt_tb_expert.mq5
+-rw-r--r--   0        0        0      427 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/ohlc.py
+-rw-r--r--   0        0        0     4286 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/order.py
+-rw-r--r--   0        0        0      268 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/order_operations.py
+-rw-r--r--   0        0        0     2471 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/order_type.py
+-rw-r--r--   0        0        0      750 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/paths.py
+-rw-r--r--   0        0        0      319 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/singleton.py
+-rw-r--r--   0        0        0        0 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/strategies/__init__.py
+-rw-r--r--   0        0        0     2417 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/strategies/basic_strategy.py
+-rw-r--r--   0        0        0     4551 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/strategies/strategy.py
+-rw-r--r--   0        0        0     5847 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/trading_methods.py
+-rw-r--r--   0        0        0     2000 2024-05-08 15:51:10.515546 tradeo-0.17.0/tradeo/utils.py
+-rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 tradeo-0.17.0/PKG-INFO
```

### Comparing `tradeo-0.16.1/LICENSE` & `tradeo-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/README.md` & `tradeo-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/pyproject.toml` & `tradeo-0.17.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "tradeo"
-version = "0.16.1"
+version = "0.17.0"
 description = ""
 authors = ["sorul <cromerovargas2d@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.8.1"
 python-dotenv = "^1.0.0"
 pytz = "^2023.3.post1"
 pandas = "1.5.3"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4.4"
 freezegun = "^1.4.0"
 flake8-bugbear = "^24.1.17"
 flake8-print = "^5.0.0"
 flake8-builtins = "^2.2.0"
 flake8-eradicate = "^1.5.0"
 flake8-pie = "^0.16.0"
 flake8-secure-coding-standard = "^1.4.1"
@@ -32,13 +31,14 @@
 flake8-cognitive-complexity = "^0.1.0"
 flake8-functions = "^0.0.8"
 flake8-docstrings = "^1.7.0"
 flake8-pytest-style = "^1.7.2"
 flake8-pytest = "^1.4"
 flake8-annotations = "^3.0.1"
 python-dotenv = "^1.0.1"
+pytest-cov = "^5.0.0"
 
 [tool.poetry.scripts]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tradeo-0.16.1/tradeo/__init__.py` & `tradeo-0.17.0/tradeo/__init__.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/config.py` & `tradeo-0.17.0/tradeo/config.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/context_managers/blocker.py` & `tradeo-0.17.0/tradeo/context_managers/blocker.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/event_handlers/basic_event_handler.py` & `tradeo-0.17.0/tradeo/event_handlers/basic_event_handler.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/event_handlers/event_handler.py` & `tradeo-0.17.0/tradeo/event_handlers/event_handler.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/executable/basic_forex.py` & `tradeo-0.17.0/tradeo/executable/basic_forex.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 class BasicForex(Executable):
   """Basic example of a forex bot."""
 
   def __init__(self):
     """Initialize the forex bot."""
     self.name = 'BasicForex'
 
-  def entry_point(self):
+  def entry_point(self) -> None:
     """Entry point of the forex bot."""
     if not self.is_locked() and self.check_time_viability():
       mt_client = MT_Client(event_handler=BasicEventHandler())
       try:
         # Lock the execution of the forex bot.
         # Another thread can not run at the same time.
         with Blocker(name=self.name):
           self.main(mt_client)
       except Exception:  # noqa
         # Finish the bot
         self.finish(mt_client)
         # Log the error
         log.error(traceback.format_exc())
 
-  def main(self, mt_client: MT_Client):
+  def main(self, mt_client: MT_Client) -> None:
     """Execute forex bot."""
     # First of all, we lock the execution of the forex bot.
     # To prevent another execution to run at the same time.
 
     # Start the MT Client
     mt_client.start()
```

### Comparing `tradeo-0.16.1/tradeo/executable/executable.py` & `tradeo-0.17.0/tradeo/executable/executable.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/files.py` & `tradeo-0.17.0/tradeo/files.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/log.py` & `tradeo-0.17.0/tradeo/log.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/mt_client.py` & `tradeo-0.17.0/tradeo/mt_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 from tradeo.order import (
     Order, MutableOrderDetails, ImmutableOrderDetails, OrderPrice)
 from tradeo.ohlc import OHLC
 from tradeo.trading_methods import get_pip
 from tradeo.utils import string_to_date_utc
 from tradeo.mt_message import MT_MessageError, MT_MessageInfo
 if TYPE_CHECKING:
-  from tradeo.event_handlers.event_handler import EventHandler
+  from tradeo.event_handlers.event_handler import (
+      EventHandler)  # pragma: no cover
 
 
 # Typing types
 attributes_data_type = Dict[str, Dict]
 messages_type = Dict[str, List[Union[MT_MessageInfo, MT_MessageError]]]
 account_info_type = Dict[str, Union[float, str]]
 historical_data_type = Dict[str, DataFrame]
@@ -68,31 +69,31 @@
     self.market_data: attributes_data_type = {}
     self.bar_data: attributes_data_type = {}
     self.historical_data: historical_data_type = {}
     self.historical_trades: attributes_data_type = {}
     self.successful_symbols: Set[str] = set()
 
     # State attributes
-    self.ACTIVE = True
+    self.activate()
 
   def set_agent_paths(self) -> None:
     """Set the paths to the files generated by MQL."""
     mt_files_path = Config.mt_files_path
     self.prefix_files_path = 'AgentFiles'
     if exists(mt_files_path):
       self.path_orders = Path(
           join(mt_files_path, self.prefix_files_path, 'Orders.json'))
       self.path_messages = Path(
           join(mt_files_path, self.prefix_files_path, 'Messages.json'))
       self.path_market_data = Path(
           join(mt_files_path, self.prefix_files_path, 'Market_Data.json'))
       self.path_bar_data = Path(
           join(mt_files_path, self.prefix_files_path, 'Bar_Data.json'))
-      self.path_historical_data = Path(
-          join(mt_files_path, self.prefix_files_path))
+      self.path_historical_data_prefix = Path(
+          join(mt_files_path, self.prefix_files_path, 'Historical_Data_'))
       self.path_historical_trades = Path(
           join(mt_files_path, self.prefix_files_path,
                'Historical_Trades.json'))
       self.path_orders_stored = Path(
           join(mt_files_path, self.prefix_files_path,
                'Orders_Stored.json'))
       self.path_messages_stored = Path(
@@ -368,16 +369,15 @@
     remaining_symbols = self.get_remaining_symbols()
     if len(remaining_symbols) == 0:
       return {}
     if symbol is None:
       symbol = remaining_symbols[randrange(len(remaining_symbols))]
 
     # We read the symbol file
-    file_path = self.path_historical_data.joinpath(
-        f'Historical_Data_{symbol}.json')
+    file_path = Path(f'{self.path_historical_data_prefix}{symbol}.json')
     data = try_load_json(file_path)
 
     if len(data) > 0:
       # The dataframe is built
       df = DataFrame.from_dict(
           data[f'{symbol}_{Config.timeframe}'], orient='index')
       self.historical_data[symbol] = df
@@ -512,15 +512,16 @@
 
     if order.order_type.pending:
       bid, ask = self.get_bid_ask(order.symbol)
       self._modify_pending_order(order, bid, ask)
 
     self.send_open_order_command(order)
 
-  def _modify_pending_order(self, order: Order, bid: float, ask: float) -> None:
+  @staticmethod
+  def _modify_pending_order(order: Order, bid: float, ask: float) -> None:
     """Modify the pending order based on the bid/ask."""
     if bid != 0 and ask != 0:
       ot = order.order_type
       if ot.buy and order.price > ask:
         ot.value = OrderOperations.BUYSTOP
       elif ot.buy and order.price < ask:
         ot.value = OrderOperations.BUYLIMIT
@@ -679,16 +680,15 @@
       file_path = Path(f'{self.path_commands_prefix}{i}.txt')
       if not try_remove_file(file_path):
         break
 
   def clean_all_historical_files(self) -> None:
     """Clean historical files."""
     for symbol in Config.symbols:
-      file_path = self.path_historical_data.joinpath(
-          f'Historical_Data_{symbol}.json')
+      file_path = Path(f'{self.path_historical_data_prefix}{symbol}.json')
       try_remove_file(file_path)
 
   def command_file_exist(self, symbol: str) -> List[Path]:
     """Return the command files that match request hist. data from symbol."""
     g = glob.glob(f'{self.path_commands_prefix}*')
     pattern = f'GET_HISTORICAL_DATA|{symbol}'
     return [
```

### Comparing `tradeo-0.16.1/tradeo/mt_tb_expert.mq5` & `tradeo-0.17.0/tradeo/mt_tb_expert.mq5`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/order.py` & `tradeo-0.17.0/tradeo/order.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/order_type.py` & `tradeo-0.17.0/tradeo/order_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,24 @@
     elif self.buy and not self.market:
       self.value = OrderOperations.BUYLIMIT
     elif not self.buy and self.market:
       self.value = OrderOperations.SELL
     elif not self.buy and not self.market:
       self.value = OrderOperations.SELLLIMIT
 
+  def __eq__(self, value: object) -> bool:
+    """Check if the object is equal to another object."""
+    return (
+        isinstance(value, OrderType)
+        and self.buy == value.buy
+        and self.sell == value.sell
+        and self.market == value.market
+        and self.pending == value.pending
+    )
+
 
 def get_order_type_from_str(order_type_str: str) -> OrderType:
   """Get the order type object from a string."""
   if order_type_str == OrderOperations.BUYLIMIT:
     ot = OrderType(buy=True, market=False)
     ot.value = OrderOperations.BUYLIMIT
   elif order_type_str == OrderOperations.BUYSTOP:
```

### Comparing `tradeo-0.16.1/tradeo/paths.py` & `tradeo-0.17.0/tradeo/paths.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/strategies/basic_strategy.py` & `tradeo-0.17.0/tradeo/strategies/basic_strategy.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/strategies/strategy.py` & `tradeo-0.17.0/tradeo/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/trading_methods.py` & `tradeo-0.17.0/tradeo/trading_methods.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/tradeo/utils.py` & `tradeo-0.17.0/tradeo/utils.py`

 * *Files identical despite different names*

### Comparing `tradeo-0.16.1/PKG-INFO` & `tradeo-0.17.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradeo
-Version: 0.16.1
+Version: 0.17.0
 Summary: 
 Author: sorul
 Author-email: cromerovargas2d@gmail.com
 Requires-Python: ==3.8.1
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```


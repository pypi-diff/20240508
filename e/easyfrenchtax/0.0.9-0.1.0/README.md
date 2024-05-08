# Comparing `tmp/easyfrenchtax-0.0.9.tar.gz` & `tmp/easyfrenchtax-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfrenchtax-0.0.9.tar", last modified: Fri May  3 18:10:49 2024, max compression
+gzip compressed data, was "easyfrenchtax-0.1.0.tar", last modified: Wed May  8 14:34:32 2024, max compression
```

## Comparing `easyfrenchtax-0.0.9.tar` & `easyfrenchtax-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.782119 easyfrenchtax-0.0.9/
--rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.0.9/LICENSE
--rw-r--r--   0 hadrien    (501) staff       (20)     2587 2024-05-03 18:10:49.782036 easyfrenchtax-0.0.9/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)     1821 2024-05-03 18:10:18.000000 easyfrenchtax-0.0.9/README.md
--rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.0.9/pyproject.toml
--rw-r--r--   0 hadrien    (501) staff       (20)      853 2024-05-03 18:10:49.782460 easyfrenchtax-0.0.9/setup.cfg
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.774028 easyfrenchtax-0.0.9/src/
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.777001 easyfrenchtax-0.0.9/src/easyfrenchtax/
--rw-r--r--   0 hadrien    (501) staff       (20)      125 2023-08-11 21:09:23.000000 easyfrenchtax-0.0.9/src/easyfrenchtax/__init__.py
--rw-r--r--   0 hadrien    (501) staff       (20)    22815 2023-08-11 21:09:23.000000 easyfrenchtax-0.0.9/src/easyfrenchtax/stock_helper.py
--rw-r--r--   0 hadrien    (501) staff       (20)    27996 2024-05-03 13:20:43.000000 easyfrenchtax-0.0.9/src/easyfrenchtax/tax_simulator.py
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.781718 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/
--rw-r--r--   0 hadrien    (501) staff       (20)     2587 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)      480 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/SOURCES.txt
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/dependency_links.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       18 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/requires.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       14 2024-05-03 18:10:49.000000 easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/top_level.txt
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-03 18:10:49.781170 easyfrenchtax-0.0.9/tests/
--rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.0.9/tests/test_capital_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.0.9/tests/test_fiscal_advantages.py
--rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.0.9/tests/test_income_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.0.9/tests/test_rental_tax.py
--rw-r--r--   0 hadrien    (501) staff       (20)    14179 2023-07-20 16:51:06.000000 easyfrenchtax-0.0.9/tests/test_stock_helper.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-08 14:34:32.333635 easyfrenchtax-0.1.0/
+-rw-r--r--   0 hadrien    (501) staff       (20)     1069 2021-12-17 08:32:37.000000 easyfrenchtax-0.1.0/LICENSE
+-rw-r--r--   0 hadrien    (501) staff       (20)     2718 2024-05-08 14:34:32.333576 easyfrenchtax-0.1.0/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)     1952 2024-05-03 18:11:52.000000 easyfrenchtax-0.1.0/README.md
+-rw-r--r--   0 hadrien    (501) staff       (20)      103 2021-12-17 08:19:56.000000 easyfrenchtax-0.1.0/pyproject.toml
+-rw-r--r--   0 hadrien    (501) staff       (20)      853 2024-05-08 14:34:32.333897 easyfrenchtax-0.1.0/setup.cfg
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-08 14:34:32.328389 easyfrenchtax-0.1.0/src/
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-08 14:34:32.330040 easyfrenchtax-0.1.0/src/easyfrenchtax/
+-rw-r--r--   0 hadrien    (501) staff       (20)      125 2023-08-11 21:09:23.000000 easyfrenchtax-0.1.0/src/easyfrenchtax/__init__.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    21358 2024-05-08 14:33:59.000000 easyfrenchtax-0.1.0/src/easyfrenchtax/stock_helper.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    27996 2024-05-03 13:20:43.000000 easyfrenchtax-0.1.0/src/easyfrenchtax/tax_simulator.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-08 14:34:32.333286 easyfrenchtax-0.1.0/src/easyfrenchtax.egg-info/
+-rw-r--r--   0 hadrien    (501) staff       (20)     2718 2024-05-08 14:34:32.000000 easyfrenchtax-0.1.0/src/easyfrenchtax.egg-info/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      480 2024-05-08 14:34:32.000000 easyfrenchtax-0.1.0/src/easyfrenchtax.egg-info/SOURCES.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2024-05-08 14:34:32.000000 easyfrenchtax-0.1.0/src/easyfrenchtax.egg-info/dependency_links.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       18 2024-05-08 14:34:32.000000 easyfrenchtax-0.1.0/src/easyfrenchtax.egg-info/requires.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       14 2024-05-08 14:34:32.000000 easyfrenchtax-0.1.0/src/easyfrenchtax.egg-info/top_level.txt
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-08 14:34:32.332913 easyfrenchtax-0.1.0/tests/
+-rw-r--r--   0 hadrien    (501) staff       (20)     5482 2022-06-10 11:22:52.000000 easyfrenchtax-0.1.0/tests/test_capital_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    11040 2022-11-27 06:14:06.000000 easyfrenchtax-0.1.0/tests/test_fiscal_advantages.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     5387 2022-06-09 13:40:59.000000 easyfrenchtax-0.1.0/tests/test_income_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)     8783 2022-06-10 11:29:26.000000 easyfrenchtax-0.1.0/tests/test_rental_tax.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    10470 2024-05-08 14:33:59.000000 easyfrenchtax-0.1.0/tests/test_stock_helper.py
```

### Comparing `easyfrenchtax-0.0.9/LICENSE` & `easyfrenchtax-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.9/PKG-INFO` & `easyfrenchtax-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
@@ -41,7 +41,14 @@
 - Typical retention plans like RSU or Stock Options, direct stocks
 - Currency conversion at acquisition/exercise/buying/selling dates
 - Weighted average price ("Prix moyen pondéré" or PMP in French tax lingo)
 - Outputs fields 3VG/3VH for form 2042C, and frame 5 (512-524) + fields 903/913 for form 2074
 
 # Contact and contributions
 If you want to chat about this project, don't hesitate to shoot an email at hadrien.hamel@gmail.com. Contributions and bug reports are welcome!
+
+# Build and upload a new version
+```commandline
+# in venv
+python3 -m build
+python3 -m twine upload dist/easyfrenchtax-x.y.z* 
+```
```

### Comparing `easyfrenchtax-0.0.9/README.md` & `easyfrenchtax-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,8 +19,15 @@
 This module helps to fill the tax statement regarding stock acquisition or capital gain. It takes as input the stocks received (RSU, Stock Options) or bought (ESPP, direct buying) and what has been exercised/sold; it outputs the fields to fill a form 2074 and parts of 2042C. More precisely, it supports the following:
 - Typical retention plans like RSU or Stock Options, direct stocks
 - Currency conversion at acquisition/exercise/buying/selling dates
 - Weighted average price ("Prix moyen pondéré" or PMP in French tax lingo)
 - Outputs fields 3VG/3VH for form 2042C, and frame 5 (512-524) + fields 903/913 for form 2074
 
 # Contact and contributions
-If you want to chat about this project, don't hesitate to shoot an email at hadrien.hamel@gmail.com. Contributions and bug reports are welcome!
+If you want to chat about this project, don't hesitate to shoot an email at hadrien.hamel@gmail.com. Contributions and bug reports are welcome!
+
+# Build and upload a new version
+```commandline
+# in venv
+python3 -m build
+python3 -m twine upload dist/easyfrenchtax-x.y.z* 
+```
```

### Comparing `easyfrenchtax-0.0.9/setup.cfg` & `easyfrenchtax-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easyfrenchtax
-version = 0.0.9
+version = 0.1.0
 author = Hadrien Hamel
 author_email = hadrien.hamel@gmail.com
 license = MIT
 description = A simulator of French taxes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/had/easyfrenchtax
```

### Comparing `easyfrenchtax-0.0.9/src/easyfrenchtax/stock_helper.py` & `easyfrenchtax-0.1.0/src/easyfrenchtax/stock_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,47 +66,14 @@
     def __init__(self):
         self.rsu_plans = {}
         self.rsus = defaultdict(list)
         self.espp_stocks = defaultdict(list)
         self.stock_options = defaultdict(list)
         self.stock_sales = defaultdict(list)
 
-    # TODO: this seems unused, consider removing
-    def reset(self, stock_types: list[StockType] = (StockType.RSU, StockType.ESPP, StockType.STOCKOPTIONS),
-              symbols: list[str] = None) -> None:
-        for sales in self.stock_sales.values():
-            sales[:] = [s for s in sales if
-                        (symbols and s.symbol not in symbols) or (s.stock_type not in stock_types)]
-        stock_types_mapping = {
-            StockType.ESPP: self.espp_stocks,
-            StockType.STOCKOPTIONS: self.stock_options,
-            StockType.RSU: self.rsus
-        }
-        for stock_type in [stock_types_mapping[st] for st in stock_types]:
-            if not symbols:
-                stocks_subset = stock_type.values()
-            else:
-                stocks_subset = [stock_type[symbol] for symbol in symbols]
-            for stocks in stocks_subset:
-                for i, s in enumerate(stocks):
-                    stocks[i].available = s.count
-
-    # TODO: this seems unused, consider removing
-    def summary(self) -> dict[str, dict[str, int]]:
-        summary = defaultdict(lambda: defaultdict(int))
-        for symbol, rsus in self.rsus.items():
-            for rsu in rsus:
-                summary[symbol]["RSU"] += rsu.count
-        for symbol, espps in self.espp_stocks.items():
-            for espp in espps:
-                summary[symbol]["ESPP"] += espp.count
-        for symbol, stockoptions in self.stock_options.items():
-            for stockoption in stockoptions:
-                summary[symbol]["StockOption"] += stockoption.count
-        return summary
 
     # ----- RSU related load functions ------
     @staticmethod
     def _determine_rsu_plans_type(approval_date: date) -> RsuTaxScheme:
         if approval_date <= date(2012, 9, 27):
             return RsuTaxScheme.NONQUALIFIED_RSU
         elif approval_date <= date(2015, 8, 8):
@@ -199,28 +166,28 @@
                     elif stock_type == "ESPP":
                         self.add_espp(symbol, acq_count, acq_date, acq_price, currency)
                     elif stock_type == "StockOption":
                         self.add_stockoptions(symbol, plan_name, acq_count, acq_date, acq_price, currency)
 
     ####### stock selling related load functions #######
 
-    def sell_stockoptions(self, owner: int, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
-                          currency: str = "EUR") -> int:
+    def sell_stockoptions_legacy(self, owner: int, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
+                                 currency: str = "EUR") -> int:
         if nb_stocks == 0:
             return 0
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
         stocks_before_sell_date = [r for r in self.stock_options[symbol] if r.acq_date < sell_date]
         for i, acq in enumerate(stocks_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
             strike_price_eur = acq.acq_price_eur if acq.acq_price_eur else cc.convert(acq.acq_price, currency, "EUR",
                                                                                       date=sell_date)
-            self.sell_stockoptions_2(
+            self.sell_stockoptions(
                 symbol=symbol,
                 nb_stocks_sold=sell_from_acq,
                 unit_acquisition_price=strike_price_eur,  # re-using this field to store the strike price
                 sell_date=sell_date,
                 sell_price_eur=sell_price_eur,
                 owner=owner
             )
@@ -229,67 +196,67 @@
             to_sell -= sell_from_acq
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have ({to_sell})")
         return nb_stocks - to_sell
 
-    def sell_stockoptions_2(self, symbol: str, nb_stocks_sold: int, unit_acquisition_price: float,
-                sell_date: date, sell_price_eur: float, owner: int):
+    def sell_stockoptions(self, symbol: str, nb_stocks_sold: int, unit_acquisition_price: float,
+                          sell_date: date, sell_price_eur: float, owner: int):
         self.stock_sales[sell_date.year].append(SaleEvent(
             symbol=symbol,
             stock_type=StockType.STOCKOPTIONS,
             nb_stocks_sold=nb_stocks_sold,
             unit_acquisition_price=round(unit_acquisition_price, 2),
             sell_date=sell_date,
             sell_price_eur=sell_price_eur,
             selling_fees=0,
             owner=owner,
         ))
-    def sell_espp(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
-                  currency: str = "EUR") -> int:
+    def sell_espp_legacy(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
+                         currency: str = "EUR") -> int:
         if nb_stocks == 0:
             return 0
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
         stocks_before_sell_date = [r for r in self.espp_stocks[symbol] if r.acq_date < sell_date]
         for i, acq in enumerate(stocks_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
             self.espp_stocks[symbol][i].available = acq.available - sell_from_acq
             to_sell -= sell_from_acq
-            self.sell_espp_2(
+            self.sell_espp(
                 symbol=symbol,
                 nb_stocks_sold=sell_from_acq,
                 unit_acquisition_price=acq.acq_price_eur,
                 sell_date=sell_date,
                 sell_price_eur=sell_price_eur
             )
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have")
         return nb_stocks - to_sell
 
-    def sell_espp_2(self, symbol: str, nb_stocks_sold: int, unit_acquisition_price: float,
-                sell_date: date, sell_price_eur: float):
+    def sell_espp(self, symbol: str, nb_stocks_sold: int, unit_acquisition_price: float,
+                  sell_date: date, sell_price_eur: float):
         self.stock_sales[sell_date.year].append(SaleEvent(
             symbol=symbol,
             stock_type=StockType.ESPP,
             nb_stocks_sold=nb_stocks_sold,
             unit_acquisition_price=round(unit_acquisition_price, 2),
             sell_date=sell_date,
             sell_price_eur=sell_price_eur,
             selling_fees=0,
         ))
 
 
-    def sell_rsus(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
-                  currency: str = "EUR") -> int:
+    def sell_rsus_legacy(self, symbol: str, nb_stocks: int, sell_date: date, sell_price: float, fees: float,
+                         currency: str = "EUR") -> int:
         if nb_stocks == 0:
             return 0
         sell_price_eur = round(cc.convert(sell_price, currency, "EUR", date=sell_date), 2)
         to_sell = nb_stocks
 
         # Acquisitions are sorted by date, this is the rule set by the tax office (FIFO, or PEPS="premier entré premier
         # sorti"); we only keep stocks acquired *before* the sell date, in case we input a sell event in the middle of
@@ -299,15 +266,15 @@
             # no rsu for that date
             return 0
         for i, acq in enumerate(rsu_before_sell_date):
             if acq.available == 0:
                 continue
             sell_from_acq = min(to_sell, acq.available)
             tax_scheme = self.rsu_plans[acq.plan_name].taxation_scheme
-            self.sell_rsus_2(
+            self.sell_rsus(
                 symbol=symbol,
                 nb_stocks_sold=sell_from_acq,
                 acq_date=acq.acq_date,
                 unit_acquisition_price=acq.acq_price_eur,
                 sell_date = sell_date,
                 sell_price_eur=sell_price_eur,
                 tax_scheme=tax_scheme
@@ -317,16 +284,16 @@
             to_sell -= sell_from_acq
             if to_sell == 0:
                 break
         if to_sell > 0:
             print(f"WARNING: You are trying to sell more stocks ({nb_stocks}) than you have ({to_sell})")
         return (nb_stocks - to_sell)
 
-    def sell_rsus_2(self, symbol: str, nb_stocks_sold: int, acq_date: date, unit_acquisition_price: float,
-                sell_date: date, sell_price_eur: float, tax_scheme: RsuTaxScheme):
+    def sell_rsus(self, symbol: str, nb_stocks_sold: int, acq_date: date, unit_acquisition_price: float,
+                  sell_date: date, sell_price_eur: float, tax_scheme: RsuTaxScheme):
         self.stock_sales[sell_date.year].append(SaleEvent(
             symbol=symbol,
             stock_type=StockType.RSU,
             nb_stocks_sold=nb_stocks_sold,
             unit_acquisition_price=round(unit_acquisition_price, 2),
             sell_date=sell_date,
             sell_price_eur=sell_price_eur,
@@ -407,14 +374,15 @@
         sell_events = self.stock_sales[year]
         total_capital_gain = 0
         for sale in sell_events:
             if sale.stock_type == StockType.STOCKOPTIONS:
                 # stock option is "exercise and sold" immediately so there is no capital gain
                 continue
             sell_event_report = {}
+            sell_event_report["title_name_511"] = sale.symbol + " " + sale.stock_type.name
             sell_event_report["selling_date_512"] = sale.sell_date
             sell_event_report["sell_price_514"] = sale.sell_price_eur
             sell_event_report["sold_stock_units_515"] = sale.nb_stocks_sold
             global_selling_proceeds = sale.sell_price_eur * sale.nb_stocks_sold
             sell_event_report["global_selling_proceeds_516"] = round(global_selling_proceeds)
             sell_event_report["selling_fees_517"] = round(sale.selling_fees)
             net_selling_proceeds = round(global_selling_proceeds - sale.selling_fees)
```

### Comparing `easyfrenchtax-0.0.9/src/easyfrenchtax/tax_simulator.py` & `easyfrenchtax-0.1.0/src/easyfrenchtax/tax_simulator.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.9/src/easyfrenchtax.egg-info/PKG-INFO` & `easyfrenchtax-0.1.0/src/easyfrenchtax.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfrenchtax
-Version: 0.0.9
+Version: 0.1.0
 Summary: A simulator of French taxes
 Home-page: https://github.com/had/easyfrenchtax
 Author: Hadrien Hamel
 Author-email: hadrien.hamel@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/had/easyfrenchtax/issues
 Classifier: Programming Language :: Python :: 3
@@ -41,7 +41,14 @@
 - Typical retention plans like RSU or Stock Options, direct stocks
 - Currency conversion at acquisition/exercise/buying/selling dates
 - Weighted average price ("Prix moyen pondéré" or PMP in French tax lingo)
 - Outputs fields 3VG/3VH for form 2042C, and frame 5 (512-524) + fields 903/913 for form 2074
 
 # Contact and contributions
 If you want to chat about this project, don't hesitate to shoot an email at hadrien.hamel@gmail.com. Contributions and bug reports are welcome!
+
+# Build and upload a new version
+```commandline
+# in venv
+python3 -m build
+python3 -m twine upload dist/easyfrenchtax-x.y.z* 
+```
```

### Comparing `easyfrenchtax-0.0.9/tests/test_capital_tax.py` & `easyfrenchtax-0.1.0/tests/test_capital_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.9/tests/test_fiscal_advantages.py` & `easyfrenchtax-0.1.0/tests/test_fiscal_advantages.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.9/tests/test_income_tax.py` & `easyfrenchtax-0.1.0/tests/test_income_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.9/tests/test_rental_tax.py` & `easyfrenchtax-0.1.0/tests/test_rental_tax.py`

 * *Files identical despite different names*

### Comparing `easyfrenchtax-0.0.9/tests/test_stock_helper.py` & `easyfrenchtax-0.1.0/tests/test_stock_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,94 +37,83 @@
 
 @pytest.fixture
 def convert_fn() -> Callable[[float, str, str, date], float]:
     cc = CurrencyConverter(fallback_on_wrong_date=True)
     return cc.convert
 
 
-def test_summary(stock_helper_with_plan):
-    summary = stock_helper_with_plan.summary()
-    assert set(summary.keys()) == {"CAKE", "BUD", "PZZA"}
-    assert set(summary["CAKE"].keys()) == {"RSU"}
-    assert summary["CAKE"]["RSU"] == 420
-    assert set(summary["BUD"].keys()) == {"ESPP"}
-    assert summary["BUD"]["ESPP"] == 500
-    assert set(summary["PZZA"].keys()) == {"StockOption", "RSU"}
-    assert summary["PZZA"]["StockOption"] == 150
-
-
 def test_rsu_sale(stock_helper_with_plan):
-    final_count_1 = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
-                                                     currency="USD")
+    final_count_1 = stock_helper_with_plan.sell_rsus_legacy("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
+                                                            currency="USD")
     assert final_count_1 == 200
     assert stock_helper_with_plan.rsus["CAKE"][0].available == 40
     assert all([r.available == 10 or r.acq_date > date(2019, 6, 3) for r in stock_helper_with_plan.rsus["CAKE"][1:]])
-    final_count_2 = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
-                                                     currency="USD")
+    final_count_2 = stock_helper_with_plan.sell_rsus_legacy("CAKE", 200, date(2019, 6, 3), sell_price=22, fees=0,
+                                                            currency="USD")
     assert final_count_2 == 120, "Cannot sell more than we have"
 
 def test_rsu_sell_available(stock_helper_with_plan):
     # check that we only consider RSUs available at the sale date, not afterwards
     # on 1-4-2021, only 313+312+398+133 are available
     available_before = 313+312+398+133
     available_after = 313
 
-    amount_sold = stock_helper_with_plan.sell_rsus("PZZA", available_before + available_after, date(2021, 4, 1), sell_price=22, fees=0)
+    amount_sold = stock_helper_with_plan.sell_rsus_legacy("PZZA", available_before + available_after, date(2021, 4, 1), sell_price=22, fees=0)
     assert amount_sold == available_before
-    amount_sold_2 = stock_helper_with_plan.sell_rsus("PZZA", available_after, date(2021, 12, 1), sell_price=22, fees=0)
+    amount_sold_2 = stock_helper_with_plan.sell_rsus_legacy("PZZA", available_after, date(2021, 12, 1), sell_price=22, fees=0)
     assert amount_sold_2 == available_after
 
 def test_rsu_fifo(stock_helper_with_plan):
-    stock_helper_with_plan.sell_rsus("PZZA", 800, date(2022,1,1), sell_price=22, fees=0)
+    stock_helper_with_plan.sell_rsus_legacy("PZZA", 800, date(2022, 1, 1), sell_price=22, fees=0)
     vestings = sorted(stock_helper_with_plan.rsus["PZZA"],key=lambda sg: sg.acq_date)
     assert vestings[0].available == 0
     assert vestings[0].count == 398
     assert vestings[1].available == 0
     assert vestings[1].count == 313
     assert vestings[2].available == 44
     assert vestings[2].count == 133
     assert vestings[3].available == 312
     assert vestings[3].count == 312
     assert vestings[4].available == 313
     assert vestings[4].count == 313
 
 
 def test_rsu_acquisition_gain_tax(stock_helper_with_plan):
-    stock_helper_with_plan.sell_rsus("CAKE", 200, date(2019, 1, 16),
-                                     sell_price=22, fees=0, currency="USD")
+    stock_helper_with_plan.sell_rsus_legacy("CAKE", 200, date(2019, 1, 16),
+                                            sell_price=22, fees=0, currency="USD")
     taxes = stock_helper_with_plan.compute_acquisition_gain_tax(2019)
     assert taxes["taxable_acquisition_gain_1TZ"] == 3432
     assert taxes["acquisition_gain_50p_rebates_1WZ"] == 0
     assert taxes["acquisition_gain_rebates_1UZ"] == 0
     assert taxes["exercise_gain_1_1TT"] == 0
     assert taxes["exercise_gain_2_1UT"] == 0
 
 
 def test_rsu_acquisition_gain_tax_rebates(stock_helper_with_plan):
-    stock_helper_with_plan.sell_rsus("CAKE", 200, date(2021, 8, 2),
-                                     sell_price=28, fees=0, currency="USD")
+    stock_helper_with_plan.sell_rsus_legacy("CAKE", 200, date(2021, 8, 2),
+                                            sell_price=28, fees=0, currency="USD")
     taxes = stock_helper_with_plan.compute_acquisition_gain_tax(2021)
     assert taxes["taxable_acquisition_gain_1TZ"] == 1716
     assert taxes["acquisition_gain_50p_rebates_1WZ"] == 0
     assert taxes["acquisition_gain_rebates_1UZ"] == 1716
     assert taxes["exercise_gain_1_1TT"] == 0
     assert taxes["exercise_gain_2_1UT"] == 0
 
 
 def test_rsu_capital_gain_simple(stock_helper_with_plan):
-    final_count = stock_helper_with_plan.sell_rsus("CAKE", 200, date(2021, 8, 2),
-                                                   sell_price=28, fees=0, currency="USD")
+    final_count = stock_helper_with_plan.sell_rsus_legacy("CAKE", 200, date(2021, 8, 2),
+                                                          sell_price=28, fees=0, currency="USD")
     assert final_count == 200
     report = stock_helper_with_plan.compute_capital_gain_tax(2021)
     assert True
 
 
 def test_rsu_example(stock_helper_with_plan):
-    final_count = stock_helper_with_plan.sell_rsus("PZZA", 844, date(2021, 2, 12),
-                                                   sell_price=31.52, fees=0, currency="USD")
+    final_count = stock_helper_with_plan.sell_rsus_legacy("PZZA", 844, date(2021, 2, 12),
+                                                          sell_price=31.52, fees=0, currency="USD")
     assert final_count == 844
     report_ag = stock_helper_with_plan.compute_acquisition_gain_tax(2021)
     assert report_ag['taxable_acquisition_gain_1TZ'] == 13556
     report_cg = stock_helper_with_plan.compute_capital_gain_tax(2021)
     report_2042C = report_cg['2042C']
     report_2074 = report_cg['2074']
     assert report_2042C['capital_gain_3VG'] == 8413
@@ -142,15 +131,15 @@
 
 
 def test_espp_sale(convert_fn):
     stock_helper = StockHelper()
     stock_helper.add_espp("BUD", 200, date(2019, 1, 15), 22, "USD")
     stock_helper.add_espp("BUD", 300, date(2019, 7, 15), 19, "USD")
     sell_price = 28
-    final_count = stock_helper.sell_espp("BUD", 300, date(2021, 8, 2), sell_price=sell_price, fees=0, currency="USD")
+    final_count = stock_helper.sell_espp_legacy("BUD", 300, date(2021, 8, 2), sell_price=sell_price, fees=0, currency="USD")
     assert final_count == 300
 
     report_ag = stock_helper.compute_acquisition_gain_tax(2021)
     assert not any(report_ag.values()), "ESPP should not yield acquisition gain (thus no acquisition gain tax)"
 
     report_cg = stock_helper.compute_capital_gain_tax(2021)
     report_2042C = report_cg['2042C']
@@ -169,16 +158,16 @@
     )
     assert report_2042C["capital_gain_3VG"] == expected_capital_gain, \
         "Capital gain tax should be compliant"
 
 
 def test_stockoptions_sale(stock_helper_with_plan, convert_fn):
     sell_price = 40
-    final_count = stock_helper_with_plan.sell_stockoptions(1, "PZZA", 50, date(2021, 8, 2), sell_price=sell_price,
-                                                                    fees=0, currency="USD")
+    final_count = stock_helper_with_plan.sell_stockoptions_legacy(1, "PZZA", 50, date(2021, 8, 2), sell_price=sell_price,
+                                                                  fees=0, currency="USD")
     agt = stock_helper_with_plan.compute_acquisition_gain_tax(2021)
     cgt = stock_helper_with_plan.compute_capital_gain_tax(2021)
 
     strike_price = stock_helper_with_plan.stock_options["PZZA"][0].acq_price
     assert final_count == 50
     ex_gain_usd = 50 * (sell_price - strike_price)
     assert agt["exercise_gain_1_1TT"] == round(convert_fn(ex_gain_usd, "USD", "EUR", date(2021, 8, 2))), \
@@ -186,65 +175,14 @@
     assert agt["exercise_gain_2_1UT"] == 0
     assert not any(cgt["2042C"].values()), \
         "Stock options 'exercise and sell' should not yield capital gain (thus no capital gain tax)"
     assert len(cgt["2074"]) == 0, \
         "Stock options 'exercise and sell' should not yield capital gain (thus no capital gain tax)"
 
 
-def test_reset_all(stock_helper_with_plan):
-    # CAKE=240 ; BUD=200 ; PZZA=150
-    stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.sell_stockoptions(1, "PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.reset()
-    assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
-    assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
-    assert len(stock_helper_with_plan.stock_sales[2021]) == 0
-
-
-def test_reset_by_stocktype(stock_helper_with_plan):
-    # CAKE=240 ; BUD=200 ; PZZA=150
-    stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.sell_stockoptions(1, "PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
-    assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
-    stock_helper_with_plan.reset(stock_types=[StockType.ESPP])
-    assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
-    assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
-    stock_helper_with_plan.reset(stock_types=[StockType.STOCKOPTIONS])
-    assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
-    assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
-    stock_helper_with_plan.reset(stock_types=[StockType.RSU])
-    assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
-    assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
-
-
-def test_reset_by_symbol(stock_helper_with_plan):
-    # CAKE=240 ; BUD=200 ; PZZA=150
-    stock_helper_with_plan.sell_rsus("CAKE", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.sell_espp("BUD", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    stock_helper_with_plan.sell_stockoptions(1, "PZZA", 50, date(2021, 8, 2), sell_price=123, fees=0, currency="USD")
-    assert stock_helper_with_plan.rsus["CAKE"][0].available == 190
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
-    assert stock_helper_with_plan.stock_options["PZZA"][0].available == 100
-    stock_helper_with_plan.reset(symbols=["CAKE", "PZZA"])
-    assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 150
-    assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
-    stock_helper_with_plan.reset(symbols=["BUD"])
-    assert stock_helper_with_plan.rsus["CAKE"][0].available == 240
-    assert stock_helper_with_plan.espp_stocks["BUD"][0].available == 200
-    assert stock_helper_with_plan.stock_options["PZZA"][0].available == 150
-
 def test_estimate_tax_rsu_acquisition_gain():
     agi = {
         "acquisition_gain_rebates_1UZ": 16000,
         "acquisition_gain_50p_rebates_1WZ": 32000,
         "taxable_acquisition_gain_1TZ": 8000
     }
     stock_helper = StockHelper()
```


# Comparing `tmp/vnpy_btse-2024.5.7.tar.gz` & `tmp/vnpy_btse-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_btse-2024.5.7.tar", last modified: Mon May  6 14:17:11 2024, max compression
+gzip compressed data, was "vnpy_btse-2024.5.8.tar", last modified: Wed May  8 08:19:44 2024, max compression
```

## Comparing `vnpy_btse-2024.5.7.tar` & `vnpy_btse-2024.5.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 14:17:11.594306 vnpy_btse-2024.5.7/
--rw-rw-rw-   0        0        0     1092 2024-04-26 07:05:39.000000 vnpy_btse-2024.5.7/LICENSE
--rw-rw-rw-   0        0        0     2725 2024-05-06 14:17:11.594306 vnpy_btse-2024.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     1732 2024-05-06 14:16:24.000000 vnpy_btse-2024.5.7/README.md
--rw-rw-rw-   0        0        0     1078 2024-05-06 14:17:11.600336 vnpy_btse-2024.5.7/setup.cfg
--rw-rw-rw-   0        0        0       43 2024-03-05 02:02:34.000000 vnpy_btse-2024.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:17:11.579186 vnpy_btse-2024.5.7/vnpy_btse/
--rw-rw-rw-   0        0        0     1212 2024-05-06 14:16:13.000000 vnpy_btse-2024.5.7/vnpy_btse/__init__.py
--rw-rw-rw-   0        0        0    54213 2024-05-06 14:16:02.000000 vnpy_btse-2024.5.7/vnpy_btse/btse_gateway.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:17:11.593232 vnpy_btse-2024.5.7/vnpy_btse.egg-info/
--rw-rw-rw-   0        0        0     2725 2024-05-06 14:17:11.000000 vnpy_btse-2024.5.7/vnpy_btse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-06 14:17:11.000000 vnpy_btse-2024.5.7/vnpy_btse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 14:17:11.000000 vnpy_btse-2024.5.7/vnpy_btse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 14:17:11.000000 vnpy_btse-2024.5.7/vnpy_btse.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2024-05-06 14:17:11.000000 vnpy_btse-2024.5.7/vnpy_btse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-06 14:17:11.000000 vnpy_btse-2024.5.7/vnpy_btse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 08:19:44.713090 vnpy_btse-2024.5.8/
+-rw-rw-rw-   0        0        0     1092 2024-04-26 07:05:39.000000 vnpy_btse-2024.5.8/LICENSE
+-rw-rw-rw-   0        0        0     2725 2024-05-08 08:19:44.714010 vnpy_btse-2024.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2024-05-08 08:18:55.000000 vnpy_btse-2024.5.8/README.md
+-rw-rw-rw-   0        0        0     1078 2024-05-08 08:19:44.722751 vnpy_btse-2024.5.8/setup.cfg
+-rw-rw-rw-   0        0        0       43 2024-03-05 02:02:34.000000 vnpy_btse-2024.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:19:44.686381 vnpy_btse-2024.5.8/vnpy_btse/
+-rw-rw-rw-   0        0        0     1212 2024-05-08 08:18:28.000000 vnpy_btse-2024.5.8/vnpy_btse/__init__.py
+-rw-rw-rw-   0        0        0    55034 2024-05-08 08:17:22.000000 vnpy_btse-2024.5.8/vnpy_btse/btse_gateway.py
+drwxrwxrwx   0        0        0        0 2024-05-08 08:19:44.711115 vnpy_btse-2024.5.8/vnpy_btse.egg-info/
+-rw-rw-rw-   0        0        0     2725 2024-05-08 08:19:44.000000 vnpy_btse-2024.5.8/vnpy_btse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-08 08:19:44.000000 vnpy_btse-2024.5.8/vnpy_btse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 08:19:44.000000 vnpy_btse-2024.5.8/vnpy_btse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-08 08:19:44.000000 vnpy_btse-2024.5.8/vnpy_btse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2024-05-08 08:19:44.000000 vnpy_btse-2024.5.8/vnpy_btse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 08:19:44.000000 vnpy_btse-2024.5.8/vnpy_btse.egg-info/top_level.txt
```

### Comparing `vnpy_btse-2024.5.7/LICENSE` & `vnpy_btse-2024.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_btse-2024.5.7/PKG-INFO` & `vnpy_btse-2024.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_btse
-Version: 2024.5.7
+Version: 2024.5.8
 Summary: BTSE trading gateway for VeighNa Evo.
 Home-page: https://www.github.com/veighna-global
 Author: VeighNa Global
 Author-email: veighna@hotmail.com
 Keywords: quant,quantitative,investment,trading,algotrading,btse,btc,crypto
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,15 +24,15 @@
 # BTSE trading gateway for VeighNa Evo
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-2024.5.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-2024.5.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## Introduction
```

### Comparing `vnpy_btse-2024.5.7/README.md` & `vnpy_btse-2024.5.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BTSE trading gateway for VeighNa Evo
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-2024.5.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-2024.5.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## Introduction
```

### Comparing `vnpy_btse-2024.5.7/setup.cfg` & `vnpy_btse-2024.5.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `vnpy_btse-2024.5.7/vnpy_btse/__init__.py` & `vnpy_btse-2024.5.8/vnpy_btse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .btse_gateway import BtseGateway
 
 
-__version__ = "2024.5.7"
+__version__ = "2024.5.8"
```

### Comparing `vnpy_btse-2024.5.7/vnpy_btse/btse_gateway.py` & `vnpy_btse-2024.5.8/vnpy_btse/btse_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             return
 
         if contract.product == Product.SPOT:
             self.spot_ws_api.subscribe_market_trade(req)
             self.spot_ob_api.subscribe_orderbook(req)
         else:
             self.futures_ws_api.subscribe_market_trade(req)
-            self.futures_ob_api.subscribe_orderbook(req)
+            self.futures_ob_api.subscribe_snapshot(req)
 
     def send_order(self, req: OrderRequest) -> str:
         """Send new order"""
         contract: ContractData = self.contracts.get(req.symbol, None)
         if not contract:
             return ""
 
@@ -245,22 +245,33 @@
 
     def query_position(self) -> None:
         """Not required since BTSE provides websocket update"""
         pass
 
     def query_history(self, req: HistoryRequest) -> list[BarData]:
         """Query kline history data"""
-        return self.spot_rest_api.query_history(req)
+        contract: ContractData = self.contracts.get(req.symbol, None)
+        if not contract:
+            return
+
+        if contract.product == Product.SPOT:
+            return self.spot_rest_api.query_history(req)
+        else:
+            return self.futures_rest_api.query_history(req)
 
     def close(self) -> None:
         """Close server connections"""
         self.spot_rest_api.stop()
         self.spot_ob_api.stop()
         self.spot_ws_api.stop()
 
+        self.futures_rest_api.stop()
+        self.futures_ob_api.stop()
+        self.futures_ws_api.stop()
+
     def on_contract(self, contract: ContractData) -> None:
         """Save a copy of contract"""
         self.contracts[contract.symbol] = contract
         super().on_contract(contract)
 
     def on_order(self, order: OrderData) -> None:
         """Save a copy of order and then push"""
@@ -457,15 +468,15 @@
             on_failed=self.on_cancel_failed,
             extra=order
         )
 
     def on_query_time(self, packet: dict, request: Request) -> None:
         """Callback of server time query"""
         timestamp: int = packet["epoch"]
-        server_time: datetime = datetime.fromtimestamp(timestamp / 1000)
+        server_time: datetime = datetime.fromtimestamp(timestamp)
         local_time: datetime = datetime.now()
 
         msg: str = f"Server time: {server_time}, local time: {local_time}"
         self.gateway.write_log(msg)
 
     def on_query_order(self, packet: dict, request: Request) -> None:
         """Callback of open orders query"""
@@ -581,72 +592,75 @@
         """Failed callback of cancel_order"""
         msg = f"Cancel spot order failed, status code: {status_code}, message: {request.response.text}, order: {request.extra} "
         self.gateway.write_log(msg)
 
     def query_history(self, req: HistoryRequest) -> list[BarData]:
         """Query kline history data"""
         buf: dict[datetime, BarData] = {}
-        end_time: str = ""
-        path: str = "/api/v5/market/candles"
 
-        for i in range(15):
-            # Create query params
+        start_time: int = int(datetime.timestamp(req.start)) * 1000
+
+        while True:
+            # Create query parameters
             params: dict = {
-                "instId": req.symbol,
-                "bar": INTERVAL_VT2BTSE[req.interval]
+                "symbol": req.symbol,
+                "resolution": INTERVAL_VT2BTSE[req.interval],
+                "start": start_time,
             }
 
-            if end_time:
-                params["after"] = end_time
-
-            # Get response from server
             resp: Response = self.request(
                 "GET",
-                path,
+                path="/api/v3.2/ohlcv",
                 params=params
             )
 
-            # Break loop if request is failed
+            # Break the loop if request failed
             if resp.status_code // 100 != 2:
-                msg = f"Query kline history failed, status code: {resp.status_code}, message: {resp.text}"
+                msg: str = f"Query kline history failed, status code: {resp.status_code}, message: {resp.text}"
                 self.gateway.write_log(msg)
                 break
             else:
                 data: dict = resp.json()
-
-                if not data["data"]:
-                    m = data["msg"]
-                    msg = f"No kline history data is received, {m}"
+                if not data:
+                    msg: str = f"No kline history data is received, start time: {start_time}"
+                    self.gateway.write_log(msg)
                     break
 
-                for bar_list in data["data"]:
-                    ts, o, h, l, c, vol, _ = bar_list
-                    dt = parse_timestamp(ts)
+                for bar_list in data:
+                    ts, o, h, l, c, vol = bar_list
+                    dt: datetime = parse_timestamp(ts, False)
+
                     bar: BarData = BarData(
                         symbol=req.symbol,
                         exchange=req.exchange,
                         datetime=dt,
                         interval=req.interval,
                         volume=float(vol),
                         open_price=float(o),
                         high_price=float(h),
                         low_price=float(l),
                         close_price=float(c),
                         gateway_name=self.gateway_name
                     )
                     buf[bar.datetime] = bar
 
-                begin: str = data["data"][-1][0]
-                end: str = data["data"][0][0]
-                msg: str = f"Query kline history finished, {req.symbol} - {req.interval.value}, {parse_timestamp(begin)} - {parse_timestamp(end)}"
+                start_time: int = data[-1][0]
+                end_time: int = data[0][0]
+
+                msg: str = f"Query kline history finished, {req.symbol} - {req.interval.value}, {parse_timestamp(start_time, False)} - {parse_timestamp(end_time, False)}"
                 self.gateway.write_log(msg)
 
-                # Update end time
-                end_time = begin
+                # Break the loop if the latest data received
+                if len(data) < 300:
+                    break
+
+                # Update query start time
+                start_time = end_time
 
+        # Sort by datetime and return bar list
         index: list[datetime] = list(buf.keys())
         index.sort()
 
         history: list[BarData] = [buf[i] for i in index]
         return history
 
 
@@ -679,18 +693,18 @@
         }
 
         host: str = server_hosts[server]
         self.init(host, proxy_host, proxy_port, 20)
 
         self.start()
 
-    def subscribe_orderbook(self, req: SubscribeRequest) -> None:
+    def subscribe_snapshot(self, req: SubscribeRequest) -> None:
         """Subscribe market data"""
         topic: str = f"snapshotL1:{req.symbol}_0"
-        self.callbacks[topic] = self.on_orderbook
+        self.callbacks[topic] = self.on_snapshot
 
         btse_req: dict = {
             "op": "subscribe",
             "args": [topic]
         }
         self.send_packet(btse_req)
 
@@ -732,15 +746,15 @@
         detail: str = self.exception_detail(exception_type, exception_value, tb)
 
         msg: str = f"Exception catched by spot orderbook API: {detail}"
         self.gateway.write_log(msg)
 
         print(detail)
 
-    def on_orderbook(self, packet: dict) -> None:
+    def on_snapshot(self, packet: dict) -> None:
         """Callback of market trade update"""
         data: dict = packet["data"]
 
         symbol: str = data["symbol"]
         tick: TickData = self.gateway.get_tick(symbol)
 
         bid_data: tuple = data["bids"][0]
@@ -1239,72 +1253,75 @@
         """Failed callback of cancel_order"""
         msg = f"Cancel futures order failed, status code: {status_code}, message: {request.response.text}, order: {request.extra} "
         self.gateway.write_log(msg)
 
     def query_history(self, req: HistoryRequest) -> list[BarData]:
         """Query kline history data"""
         buf: dict[datetime, BarData] = {}
-        end_time: str = ""
-        path: str = "/api/v5/market/candles"
 
-        for i in range(15):
-            # Create query params
+        start_time: int = int(datetime.timestamp(req.start)) * 1000
+
+        while True:
+            # Create query parameters
             params: dict = {
-                "instId": req.symbol,
-                "bar": INTERVAL_VT2BTSE[req.interval]
+                "symbol": req.symbol,
+                "resolution": INTERVAL_VT2BTSE[req.interval],
+                "start": start_time,
             }
 
-            if end_time:
-                params["after"] = end_time
-
-            # Get response from server
             resp: Response = self.request(
                 "GET",
-                path,
+                path="/api/v2.1/ohlcv",
                 params=params
             )
 
-            # Break loop if request is failed
+            # Break the loop if request failed
             if resp.status_code // 100 != 2:
-                msg = f"Query kline history failed, status code: {resp.status_code}, message: {resp.text}"
+                msg: str = f"Query kline history failed, status code: {resp.status_code}, message: {resp.text}"
                 self.gateway.write_log(msg)
                 break
             else:
                 data: dict = resp.json()
-
-                if not data["data"]:
-                    m = data["msg"]
-                    msg = f"No kline history data is received, {m}"
+                if not data:
+                    msg: str = f"No kline history data is received, start time: {start_time}"
+                    self.gateway.write_log(msg)
                     break
 
-                for bar_list in data["data"]:
-                    ts, o, h, l, c, vol, _ = bar_list
-                    dt = parse_timestamp(ts)
+                for bar_list in data:
+                    ts, o, h, l, c, vol = bar_list
+                    dt: datetime = parse_timestamp(ts, False)
+
                     bar: BarData = BarData(
                         symbol=req.symbol,
                         exchange=req.exchange,
                         datetime=dt,
                         interval=req.interval,
                         volume=float(vol),
                         open_price=float(o),
                         high_price=float(h),
                         low_price=float(l),
                         close_price=float(c),
                         gateway_name=self.gateway_name
                     )
                     buf[bar.datetime] = bar
 
-                begin: str = data["data"][-1][0]
-                end: str = data["data"][0][0]
-                msg: str = f"Query kline history finished, {req.symbol} - {req.interval.value}, {parse_timestamp(begin)} - {parse_timestamp(end)}"
+                start_time: int = data[-1][0]
+                end_time: int = data[0][0]
+
+                msg: str = f"Query kline history finished, {req.symbol} - {req.interval.value}, {parse_timestamp(start_time, False)} - {parse_timestamp(end_time, False)}"
                 self.gateway.write_log(msg)
 
-                # Update end time
-                end_time = begin
+                # Break the loop if the latest data received
+                if len(data) < 300:
+                    break
 
+                # Update query start time
+                start_time = end_time
+
+        # Sort by datetime and return bar list
         index: list[datetime] = list(buf.keys())
         index.sort()
 
         history: list[BarData] = [buf[i] for i in index]
         return history
 
 
@@ -1337,18 +1354,18 @@
         }
 
         host: str = server_hosts[server]
         self.init(host, proxy_host, proxy_port, 20)
 
         self.start()
 
-    def subscribe_orderbook(self, req: SubscribeRequest) -> None:
+    def subscribe_snapshot(self, req: SubscribeRequest) -> None:
         """Subscribe market data"""
         topic: str = f"snapshotL1:{req.symbol}_0"
-        self.callbacks[topic] = self.on_orderbook
+        self.callbacks[topic] = self.on_snapshot
 
         btse_req: dict = {
             "op": "subscribe",
             "args": [topic]
         }
         self.send_packet(btse_req)
 
@@ -1390,15 +1407,15 @@
         detail: str = self.exception_detail(exception_type, exception_value, tb)
 
         msg: str = f"Exception catched by futures orderbook API: {detail}"
         self.gateway.write_log(msg)
 
         print(detail)
 
-    def on_orderbook(self, packet: dict) -> None:
+    def on_snapshot(self, packet: dict) -> None:
         """Callback of market trade update"""
         data: dict = packet["data"]
 
         symbol: str = data["symbol"]
         tick: TickData = self.gateway.get_tick(symbol)
 
         bid_data: tuple = data["bids"][0]
@@ -1645,17 +1662,20 @@
 def generate_timestamp() -> str:
     """Generate current timestamp"""
     now: datetime = datetime.utcnow()
     timestamp: str = now.isoformat("T", "milliseconds")
     return timestamp + "Z"
 
 
-def parse_timestamp(timestamp: int) -> datetime:
+def parse_timestamp(timestamp: int, is_millisecond: bool = True) -> datetime:
     """Parse timestamp to datetime"""
-    dt: datetime = datetime.fromtimestamp(timestamp / 1000)
+    if is_millisecond:
+        timestamp = timestamp / 1000
+
+    dt: datetime = datetime.fromtimestamp(timestamp)
     return dt.replace(tzinfo=UTC_TZ)
 
 
 def get_float_value(data: dict, key: str) -> float:
     """Get decimal number from float value"""
     data_str: str = data.get(key, "")
     if not data_str:
```

### Comparing `vnpy_btse-2024.5.7/vnpy_btse.egg-info/PKG-INFO` & `vnpy_btse-2024.5.8/vnpy_btse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-btse
-Version: 2024.5.7
+Version: 2024.5.8
 Summary: BTSE trading gateway for VeighNa Evo.
 Home-page: https://www.github.com/veighna-global
 Author: VeighNa Global
 Author-email: veighna@hotmail.com
 Keywords: quant,quantitative,investment,trading,algotrading,btse,btc,crypto
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
@@ -24,15 +24,15 @@
 # BTSE trading gateway for VeighNa Evo
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-2024.5.7-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-2024.5.8-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## Introduction
```


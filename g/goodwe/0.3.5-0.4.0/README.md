# Comparing `tmp/goodwe-0.3.5.tar.gz` & `tmp/goodwe-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodwe-0.3.5.tar", last modified: Wed May  8 21:26:36 2024, max compression
+gzip compressed data, was "goodwe-0.4.0.tar", last modified: Sun May  5 09:52:08 2024, max compression
```

## Comparing `goodwe-0.3.5.tar` & `goodwe-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:26:36.622644 goodwe-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 21:26:29.000000 goodwe-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-08 21:26:36.622644 goodwe-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-08 21:26:29.000000 goodwe-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 21:26:33.000000 goodwe-0.3.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:26:36.622644 goodwe-0.3.5/goodwe/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    40084 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/et.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/inverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    36990 2024-05-08 21:26:29.000000 goodwe-0.3.5/goodwe/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:26:36.622644 goodwe-0.3.5/goodwe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-08 21:26:36.000000 goodwe-0.3.5/goodwe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-08 21:26:36.000000 goodwe-0.3.5/goodwe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 21:26:36.000000 goodwe-0.3.5/goodwe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 21:26:36.000000 goodwe-0.3.5/goodwe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 21:26:29.000000 goodwe-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-08 21:26:36.622644 goodwe-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 21:26:36.622644 goodwe-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20437 2024-05-08 21:26:29.000000 goodwe-0.3.5/tests/test_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-05-08 21:26:29.000000 goodwe-0.3.5/tests/test_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    67983 2024-05-08 21:26:29.000000 goodwe-0.3.5/tests/test_et.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-08 21:26:29.000000 goodwe-0.3.5/tests/test_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-08 21:26:29.000000 goodwe-0.3.5/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-08 21:26:29.000000 goodwe-0.3.5/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:52:08.155559 goodwe-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 09:52:01.000000 goodwe-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-05 09:52:08.155559 goodwe-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-05 09:52:01.000000 goodwe-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 09:52:05.000000 goodwe-0.4.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:52:08.151559 goodwe-0.4.0/goodwe/
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22545 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39676 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24873 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37054 2024-05-05 09:52:01.000000 goodwe-0.4.0/goodwe/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:52:08.155559 goodwe-0.4.0/goodwe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-05 09:52:08.000000 goodwe-0.4.0/goodwe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-05 09:52:08.000000 goodwe-0.4.0/goodwe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 09:52:08.000000 goodwe-0.4.0/goodwe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 09:52:08.000000 goodwe-0.4.0/goodwe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-05 09:52:01.000000 goodwe-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-05 09:52:08.155559 goodwe-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:52:08.155559 goodwe-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-05-05 09:52:01.000000 goodwe-0.4.0/tests/test_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29091 2024-05-05 09:52:01.000000 goodwe-0.4.0/tests/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66893 2024-05-05 09:52:01.000000 goodwe-0.4.0/tests/test_et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-05 09:52:01.000000 goodwe-0.4.0/tests/test_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-05-05 09:52:01.000000 goodwe-0.4.0/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13861 2024-05-05 09:52:01.000000 goodwe-0.4.0/tests/test_sensor.py
```

### Comparing `goodwe-0.3.5/LICENSE` & `goodwe-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.5/PKG-INFO` & `goodwe-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.3.5
+Version: 0.4.0
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,23 +28,29 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/goodwe.svg)](https://github.com/marcelblijleven/goodwe/)
 [![Build Status](https://github.com/marcelblijleven/goodwe/actions/workflows/publish.yaml/badge.svg)](https://github.com/marcelblijleven/goodwe/actions/workflows/publish.yaml)
 ![License](https://img.shields.io/github/license/marcelblijleven/goodwe.svg)
 
 Library for connecting to GoodWe inverter over local network and retrieving runtime sensor values and configuration
 parameters.
 
-It has been reported to work on GoodWe ET, EH, BT, BH, ES, EM, BP, DT, MS, D-NS, and XS families of inverters. It may
-work on other inverters as well, as long as they listen on UDP port 8899 and respond to one of supported communication
-protocols.
+It has been reported to work with GoodWe ET, EH, BT, BH, ES, EM, BP, DT, MS, D-NS, and XS families of inverters. It
+should work with other inverters as well, as long as they listen on UDP port 8899 and respond to one of supported
+communication protocols.
+In general, if you can connect to your inverter with the official mobile app (SolarGo/PvMaster) over Wi-Fi (not
+bluetooth), this library should work.
 
 (If you can't communicate with the inverter despite your model is listed above, it is possible you have old ARM firmware
 version. You should ask manufacturer support to upgrade your ARM firmware (not just inverter firmware) to be able to
-communicate with the inveter via UDP.)
+communicate with the inverter via UDP.)
 
-White-label (GoodWe manufactured) inverters may work as well, e.g. General Electric GEP (PSB, PSC) and GEH models.
+White-label (GoodWe manufactured) inverters may work as well, e.g. General Electric GEP (PSB, PSC) and GEH models are
+know to work properly.
+
+Since v0.4.x the library also supports standard Modbus/TCP over port 502.
+This protocol is supported by the V2.0 version of LAN+WiFi communication dongle (model WLA0000-01-00P).
 
 ## Usage
 
 1. Install this package `pip install goodwe`
 2. Write down your GoodWe inverter's IP address (or invoke `goodwe.search_inverters()`)
 3. Connect to inverter and read all runtime data, example below
 
@@ -68,8 +74,7 @@
 ```
 
 ## References and useful links
 
 - https://github.com/mletenay/home-assistant-goodwe-inverter
 - https://github.com/yasko-pv/modbus-log
 - https://github.com/tkubec/GoodWe
-- https://github.com/OpenEMS/openems
```

### Comparing `goodwe-0.3.5/README.md` & `goodwe-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/goodwe.svg)](https://github.com/marcelblijleven/goodwe/)
 [![Build Status](https://github.com/marcelblijleven/goodwe/actions/workflows/publish.yaml/badge.svg)](https://github.com/marcelblijleven/goodwe/actions/workflows/publish.yaml)
 ![License](https://img.shields.io/github/license/marcelblijleven/goodwe.svg)
 
 Library for connecting to GoodWe inverter over local network and retrieving runtime sensor values and configuration
 parameters.
 
-It has been reported to work on GoodWe ET, EH, BT, BH, ES, EM, BP, DT, MS, D-NS, and XS families of inverters. It may
-work on other inverters as well, as long as they listen on UDP port 8899 and respond to one of supported communication
-protocols.
+It has been reported to work with GoodWe ET, EH, BT, BH, ES, EM, BP, DT, MS, D-NS, and XS families of inverters. It
+should work with other inverters as well, as long as they listen on UDP port 8899 and respond to one of supported
+communication protocols.
+In general, if you can connect to your inverter with the official mobile app (SolarGo/PvMaster) over Wi-Fi (not
+bluetooth), this library should work.
 
 (If you can't communicate with the inverter despite your model is listed above, it is possible you have old ARM firmware
 version. You should ask manufacturer support to upgrade your ARM firmware (not just inverter firmware) to be able to
-communicate with the inveter via UDP.)
+communicate with the inverter via UDP.)
 
-White-label (GoodWe manufactured) inverters may work as well, e.g. General Electric GEP (PSB, PSC) and GEH models.
+White-label (GoodWe manufactured) inverters may work as well, e.g. General Electric GEP (PSB, PSC) and GEH models are
+know to work properly.
+
+Since v0.4.x the library also supports standard Modbus/TCP over port 502.
+This protocol is supported by the V2.0 version of LAN+WiFi communication dongle (model WLA0000-01-00P).
 
 ## Usage
 
 1. Install this package `pip install goodwe`
 2. Write down your GoodWe inverter's IP address (or invoke `goodwe.search_inverters()`)
 3. Connect to inverter and read all runtime data, example below
 
@@ -44,8 +50,7 @@
 ```
 
 ## References and useful links
 
 - https://github.com/mletenay/home-assistant-goodwe-inverter
 - https://github.com/yasko-pv/modbus-log
 - https://github.com/tkubec/GoodWe
-- https://github.com/OpenEMS/openems
```

### Comparing `goodwe-0.3.5/goodwe/__init__.py` & `goodwe-0.4.0/goodwe/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import logging
-from typing import Type
 
+from .const import GOODWE_TCP_PORT, GOODWE_UDP_PORT
 from .dt import DT
 from .es import ES
 from .et import ET
 from .exceptions import InverterError, RequestFailedException
 from .inverter import Inverter, OperationMode, Sensor, SensorKind
 from .model import DT_MODEL_TAGS, ES_MODEL_TAGS, ET_MODEL_TAGS
 from .protocol import ProtocolCommand, UdpInverterProtocol, Aa55ProtocolCommand
@@ -22,85 +22,90 @@
 # Initial discovery command
 DISCOVERY_COMMAND = Aa55ProtocolCommand("010200", "0182")
 
 # supported inverter protocols
 _SUPPORTED_PROTOCOLS = [ET, DT, ES]
 
 
-async def connect(host: str, family: str = None, comm_addr: int = 0, timeout: int = 1, retries: int = 3,
-                  do_discover: bool = True) -> Inverter:
+async def connect(host: str, port: int = GOODWE_UDP_PORT, family: str = None, comm_addr: int = 0, timeout: int = 1,
+                  retries: int = 3, do_discover: bool = True) -> Inverter:
     """Contact the inverter at the specified host/port and answer appropriate Inverter instance.
 
     The specific inverter family/type will be detected automatically, but it can be passed explicitly.
     Supported inverter family names are ET, EH, BT, BH, ES, EM, BP, DT, MS, D-NS and XS.
 
     Inverter communication address may be explicitly passed, if not the usual default value
     will be used (0xf7 for ET/EH/BT/BH/ES/EM/BP inverters, 0x7f for DT/MS/D-NS/XS inverters).
 
     Since the UDP communication is by definition unreliable, when no (valid) response is received by the specified
     timeout, it is considered lost and the command will be re-tried up to retries times.
 
     Raise InverterError if unable to contact or recognise supported inverter.
     """
-    if family in ET_FAMILY:
-        inv = ET(host, comm_addr, timeout, retries)
+    if family in ET_FAMILY or port == GOODWE_TCP_PORT:
+        inv = ET(host, port, comm_addr, timeout, retries)
     elif family in ES_FAMILY:
-        inv = ES(host, comm_addr, timeout, retries)
+        inv = ES(host, port, comm_addr, timeout, retries)
     elif family in DT_FAMILY:
-        inv = DT(host, comm_addr, timeout, retries)
+        inv = DT(host, port, comm_addr, timeout, retries)
     elif do_discover:
-        return await discover(host, timeout, retries)
+        return await discover(host, port, timeout, retries)
     else:
         raise InverterError("Specify either an inverter family or set do_discover True")
 
-    logger.debug("Connecting to %s family inverter at %s.", family, host)
+    logger.debug("Connecting to %s family inverter at %s:%s.", family, host, port)
     await inv.read_device_info()
     logger.debug("Connected to inverter %s, S/N:%s.", inv.model_name, inv.serial_number)
     return inv
 
 
-async def discover(host: str, timeout: int = 1, retries: int = 3) -> Inverter:
+async def discover(host: str, port: int = GOODWE_UDP_PORT, timeout: int = 1, retries: int = 3) -> Inverter:
     """Contact the inverter at the specified value and answer appropriate Inverter instance
 
     Raise InverterError if unable to contact or recognise supported inverter
     """
     failures = []
 
     # Try the common AA55C07F0102000241 command first and detect inverter type from serial_number
     try:
-        logger.debug("Probing inverter at %s.", host)
-        response = await DISCOVERY_COMMAND.execute(host, timeout, retries)
+        logger.debug("Probing inverter at %s:%s.", host, port)
+        response = await DISCOVERY_COMMAND.execute(UdpInverterProtocol(host, port, timeout, retries))
         response = response.response_data()
         model_name = response[5:15].decode("ascii").rstrip()
         serial_number = response[31:47].decode("ascii")
 
-        inverter_class: Type[Inverter] | None = None
+        i: Inverter | None = None
         for model_tag in ET_MODEL_TAGS:
             if model_tag in serial_number:
                 logger.debug("Detected ET/EH/BT/BH/GEH inverter %s, S/N:%s.", model_name, serial_number)
-                inverter_class = ET
-        for model_tag in ES_MODEL_TAGS:
-            if model_tag in serial_number:
-                logger.debug("Detected ES/EM/BP inverter %s, S/N:%s.", model_name, serial_number)
-                inverter_class = ES
-        for model_tag in DT_MODEL_TAGS:
-            if model_tag in serial_number:
-                logger.debug("Detected DT/MS/D-NS/XS/GEP inverter %s, S/N:%s.", model_name, serial_number)
-                inverter_class = DT
-        if inverter_class:
-            i = inverter_class(host, 0, timeout, retries)
+                i = ET(host, port, 0, timeout, retries)
+                break
+        if not i:
+            for model_tag in ES_MODEL_TAGS:
+                if model_tag in serial_number:
+                    logger.debug("Detected ES/EM/BP inverter %s, S/N:%s.", model_name, serial_number)
+                    i = ES(host, port, 0, timeout, retries)
+                    break
+        if not i:
+            for model_tag in DT_MODEL_TAGS:
+                if model_tag in serial_number:
+                    logger.debug("Detected DT/MS/D-NS/XS/GEP inverter %s, S/N:%s.", model_name, serial_number)
+                    i = DT(host, port, 0, timeout, retries)
+                    break
+        if i:
             await i.read_device_info()
+            logger.debug("Connected to inverter %s, S/N:%s.", i.model_name, i.serial_number)
             return i
 
     except InverterError as ex:
         failures.append(ex)
 
     # Probe inverter specific protocols
     for inv in _SUPPORTED_PROTOCOLS:
-        i = inv(host, 0, timeout, retries)
+        i = inv(host, port, 0, timeout, retries)
         try:
             logger.debug("Probing %s inverter at %s.", inv.__name__, host)
             await i.read_device_info()
             await i.read_runtime_data()
             logger.debug("Detected %s family inverter %s, S/N:%s.", inv.__name__, i.model_name, i.serial_number)
             return i
         except InverterError as ex:
@@ -115,26 +120,16 @@
 async def search_inverters() -> bytes:
     """Scan the network for inverters.
     Answer the inverter discovery response string (which includes it IP address)
 
     Raise InverterError if unable to contact any inverter
     """
     logger.debug("Searching inverters by broadcast to port 48899")
-    loop = asyncio.get_running_loop()
     command = ProtocolCommand("WIFIKIT-214028-READ".encode("utf-8"), lambda r: True)
-    response_future = loop.create_future()
-    transport, _ = await loop.create_datagram_endpoint(
-        lambda: UdpInverterProtocol(response_future, command, 1, 3),
-        remote_addr=("255.255.255.255", 48899),
-        allow_broadcast=True,
-    )
     try:
-        await response_future
-        result = response_future.result()
+        result = await command.execute(UdpInverterProtocol("255.255.255.255", 48899, 1, 0))
         if result is not None:
-            return result
+            return result.response_data()
         else:
             raise InverterError("No response received to broadcast request.")
     except asyncio.CancelledError:
         raise InverterError("No valid response received to broadcast request.") from None
-    finally:
-        transport.close()
```

### Comparing `goodwe-0.3.5/goodwe/const.py` & `goodwe-0.4.0/goodwe/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict
 
+GOODWE_TCP_PORT = 502
 GOODWE_UDP_PORT = 8899
 
 BATTERY_MODES: Dict[int, str] = {
     0: "No battery",
     1: "Standby",
     2: "Discharge",
     3: "Charge",
```

### Comparing `goodwe-0.3.5/goodwe/dt.py` & `goodwe-0.4.0/goodwe/dt.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Tuple
 
 from .exceptions import InverterError
 from .inverter import Inverter
 from .inverter import OperationMode
 from .inverter import SensorKind as Kind
 from .model import is_3_mppt, is_single_phase
-from .protocol import ProtocolCommand, ModbusReadCommand, ModbusWriteCommand, ModbusWriteMultiCommand
+from .protocol import ProtocolCommand
 from .sensor import *
 
 
 class DT(Inverter):
     """Class representing inverter of DT/MS/D-NS/XS or GE's GEP(PSB/PSC) families"""
 
     __all_sensors: Tuple[Sensor, ...] = (
@@ -118,21 +118,21 @@
     )
 
     # Settings for three phase inverters
     __settings_three_phase: Tuple[Sensor, ...] = (
         Integer("grid_export_limit", 40336, "Grid Export Limit", "%", Kind.GRID),
     )
 
-    def __init__(self, host: str, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
-        super().__init__(host, comm_addr, timeout, retries)
+    def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
+        super().__init__(host, port, comm_addr, timeout, retries)
         if not self.comm_addr:
             # Set the default inverter address
             self.comm_addr = 0x7f
-        self._READ_DEVICE_VERSION_INFO: ProtocolCommand = ModbusReadCommand(self.comm_addr, 0x7531, 0x0028)
-        self._READ_DEVICE_RUNNING_DATA: ProtocolCommand = ModbusReadCommand(self.comm_addr, 0x7594, 0x0049)
+        self._READ_DEVICE_VERSION_INFO: ProtocolCommand = self._read_command(0x7531, 0x0028)
+        self._READ_DEVICE_RUNNING_DATA: ProtocolCommand = self._read_command(0x7594, 0x0049)
         self._sensors = self.__all_sensors
         self._settings: dict[str, Sensor] = {s.id_: s for s in self.__all_settings}
 
     @staticmethod
     def _single_phase_only(s: Sensor) -> bool:
         """Filter to exclude phase2/3 sensors on single phase inverters"""
         return not ((s.id_.endswith('2') or s.id_.endswith('3')) and 'pv' not in s.id_)
@@ -176,27 +176,27 @@
         return data
 
     async def read_setting(self, setting_id: str) -> Any:
         setting = self._settings.get(setting_id)
         if not setting:
             raise ValueError(f'Unknown setting "{setting_id}"')
         count = (setting.size_ + (setting.size_ % 2)) // 2
-        response = await self._read_from_socket(ModbusReadCommand(self.comm_addr, setting.offset, count))
+        response = await self._read_from_socket(self._read_command(setting.offset, count))
         return setting.read_value(response)
 
     async def write_setting(self, setting_id: str, value: Any):
         setting = self._settings.get(setting_id)
         if not setting:
             raise ValueError(f'Unknown setting "{setting_id}"')
         raw_value = setting.encode_value(value)
         if len(raw_value) <= 2:
             value = int.from_bytes(raw_value, byteorder="big", signed=True)
-            await self._read_from_socket(ModbusWriteCommand(self.comm_addr, setting.offset, value))
+            await self._read_from_socket(self._write_command(setting.offset, value))
         else:
-            await self._read_from_socket(ModbusWriteMultiCommand(self.comm_addr, setting.offset, raw_value))
+            await self._read_from_socket(self._write_multi_command(setting.offset, raw_value))
 
     async def read_settings_data(self) -> Dict[str, Any]:
         data = {}
         for setting in self.settings():
             value = await self.read_setting(setting.id_)
             data[setting.id_] = value
         return data
```

### Comparing `goodwe-0.3.5/goodwe/es.py` & `goodwe-0.4.0/goodwe/es.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import logging
 from typing import Tuple
 
 from .exceptions import InverterError
 from .inverter import Inverter
 from .inverter import OperationMode
 from .inverter import SensorKind as Kind
-from .protocol import ProtocolCommand, Aa55ProtocolCommand, Aa55ReadCommand, Aa55WriteCommand, Aa55WriteMultiCommand, \
-    ModbusReadCommand, ModbusWriteCommand, ModbusWriteMultiCommand
+from .protocol import ProtocolCommand, Aa55ProtocolCommand, Aa55ReadCommand, Aa55WriteCommand, Aa55WriteMultiCommand
 from .sensor import *
 
 logger = logging.getLogger(__name__)
 
 
 class ES(Inverter):
     """Class representing inverter of ES/EM/BP family AKA platform 105"""
@@ -164,16 +163,16 @@
         ByteH("eco_mode_2_switch", 47555, "Eco Mode Group 2 Switch"),
         EcoModeV2("eco_mode_3", 47559, "Eco Mode Group 3"),
         ByteH("eco_mode_3_switch", 47561, "Eco Mode Group 3 Switch"),
         EcoModeV2("eco_mode_4", 47565, "Eco Mode Group 4"),
         ByteH("eco_mode_4_switch", 47567, "Eco Mode Group 4 Switch"),
     )
 
-    def __init__(self, host: str, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
-        super().__init__(host, comm_addr, timeout, retries)
+    def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
+        super().__init__(host, port, comm_addr, timeout, retries)
         if not self.comm_addr:
             # Set the default inverter address
             self.comm_addr = 0xf7
         self._settings: dict[str, Sensor] = {s.id_: s for s in self.__all_settings}
 
     def _supports_eco_mode_v2(self) -> bool:
         if self.arm_version < 14:
@@ -224,15 +223,15 @@
         else:
             all_settings = await self.read_settings_data()
             return all_settings.get(setting_id)
 
     async def _read_setting(self, setting: Sensor) -> Any:
         count = (setting.size_ + (setting.size_ % 2)) // 2
         if self._is_modbus_setting(setting):
-            response = await self._read_from_socket(ModbusReadCommand(self.comm_addr, setting.offset, count))
+            response = await self._read_from_socket(self._read_command(setting.offset, count))
             return setting.read_value(response)
         else:
             response = await self._read_from_socket(Aa55ReadCommand(setting.offset, count))
             return setting.read_value(response)
 
     async def write_setting(self, setting_id: str, value: Any):
         if setting_id == 'time':
@@ -245,30 +244,30 @@
                 raise ValueError(f'Unknown setting "{setting_id}"')
             await self._write_setting(setting, value)
 
     async def _write_setting(self, setting: Sensor, value: Any):
         if setting.size_ == 1:
             # modbus can address/store only 16 bit values, read the other 8 bytes
             if self._is_modbus_setting(setting):
-                response = await self._read_from_socket(ModbusReadCommand(self.comm_addr, setting.offset, 1))
+                response = await self._read_from_socket(self._read_command(setting.offset, 1))
                 raw_value = setting.encode_value(value, response.response_data()[0:2])
             else:
                 response = await self._read_from_socket(Aa55ReadCommand(setting.offset, 1))
                 raw_value = setting.encode_value(value, response.response_data()[2:4])
         else:
             raw_value = setting.encode_value(value)
         if len(raw_value) <= 2:
             value = int.from_bytes(raw_value, byteorder="big", signed=True)
             if self._is_modbus_setting(setting):
-                await self._read_from_socket(ModbusWriteCommand(self.comm_addr, setting.offset, value))
+                await self._read_from_socket(self._write_command(setting.offset, value))
             else:
                 await self._read_from_socket(Aa55WriteCommand(setting.offset, value))
         else:
             if self._is_modbus_setting(setting):
-                await self._read_from_socket(ModbusWriteMultiCommand(self.comm_addr, setting.offset, raw_value))
+                await self._read_from_socket(self._write_multi_command(setting.offset, raw_value))
             else:
                 await self._read_from_socket(Aa55WriteMultiCommand(setting.offset, raw_value))
 
     async def read_settings_data(self) -> Dict[str, Any]:
         response = await self._read_from_socket(self._READ_DEVICE_SETTINGS_DATA)
         data = self._map_response(response, self.settings())
         return data
@@ -287,15 +286,15 @@
         result.remove(OperationMode.PEAK_SHAVING)
         result.remove(OperationMode.SELF_USE)
         if not include_emulated:
             result.remove(OperationMode.ECO_CHARGE)
             result.remove(OperationMode.ECO_DISCHARGE)
         return tuple(result)
 
-    async def get_operation_mode(self) -> OperationMode:
+    async def get_operation_mode(self) -> OperationMode | None:
         mode_id = await self.read_setting('work_mode')
         try:
             mode = OperationMode(mode_id)
         except ValueError:
             logger.debug("Unknown work_mode value %d", mode_id)
             return None
         if OperationMode.ECO != mode:
```

### Comparing `goodwe-0.3.5/goodwe/et.py` & `goodwe-0.4.0/goodwe/et.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import logging
 from typing import Tuple
 
-from .exceptions import RequestFailedException, RequestRejectedException
+from .exceptions import RequestRejectedException
 from .inverter import Inverter
 from .inverter import OperationMode
 from .inverter import SensorKind as Kind
 from .model import is_2_battery, is_4_mppt, is_745_platform, is_single_phase
-from .protocol import ProtocolCommand, ModbusReadCommand, ModbusWriteCommand, ModbusWriteMultiCommand
+from .protocol import ProtocolCommand
 from .sensor import *
 
 logger = logging.getLogger(__name__)
 
 
 class ET(Inverter):
     """Class representing inverter of ET/EH/BT/BH or GE's GEH families AKA platform 205 or 745"""
@@ -148,14 +148,18 @@
                    read_bytes4(data, 35105, 0) +
                    read_bytes4(data, 35109, 0) +
                    read_bytes4(data, 35113, 0) +
                    read_bytes4(data, 35117, 0) +
                    read_bytes4_signed(data, 35182) -
                    read_bytes2_signed(data, 35140),
                    "House Consumption", "W", Kind.AC),
+
+        # Power4S("pbattery2", 35264, "Battery2 Power", Kind.BAT),
+        # Integer("battery2_mode", 35266, "Battery2 Mode code", "", Kind.BAT),
+        # Enum2("battery2_mode_label", 35184, BATTERY_MODES, "Battery2 Mode", Kind.BAT),
     )
 
     # Modbus registers from offset 0x9088 (37000)
     __all_sensors_battery: Tuple[Sensor, ...] = (
         Integer("battery_bms", 37000, "Battery BMS", "", Kind.BAT),
         Integer("battery_index", 37001, "Battery Index", "", Kind.BAT),
         Integer("battery_status", 37002, "Battery Status", "", Kind.BAT),
@@ -401,26 +405,26 @@
         Integer("dod_holding", 47602, "DoD Holding", "", Kind.BAT),
         Integer("backup_mode_enable", 47605, "Backup Mode Switch"),
         Integer("max_charge_power", 47606, "Max Charge Power"),
         Integer("smart_charging_enable", 47609, "Smart Charging Mode Switch"),
         Integer("eco_mode_enable", 47612, "Eco Mode Switch"),
     )
 
-    def __init__(self, host: str, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
-        super().__init__(host, comm_addr, timeout, retries)
+    def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
+        super().__init__(host, port, comm_addr, timeout, retries)
         if not self.comm_addr:
             # Set the default inverter address
             self.comm_addr = 0xf7
-        self._READ_DEVICE_VERSION_INFO: ProtocolCommand = ModbusReadCommand(self.comm_addr, 0x88b8, 0x0021)
-        self._READ_RUNNING_DATA: ProtocolCommand = ModbusReadCommand(self.comm_addr, 0x891c, 0x007d)
-        self._READ_METER_DATA: ProtocolCommand = ModbusReadCommand(self.comm_addr, 0x8ca0, 0x2d)
-        self._READ_METER_DATA_EXTENDED: ProtocolCommand = ModbusReadCommand(self.comm_addr, 0x8ca0, 0x3a)
-        self._READ_BATTERY_INFO: ProtocolCommand = ModbusReadCommand(self.comm_addr, 0x9088, 0x0018)
-        self._READ_BATTERY2_INFO: ProtocolCommand = ModbusReadCommand(self.comm_addr, 0x9858, 0x0016)
-        self._READ_MPPT_DATA: ProtocolCommand = ModbusReadCommand(self.comm_addr, 0x89e5, 0x3d)
+        self._READ_DEVICE_VERSION_INFO: ProtocolCommand = self._read_command(0x88b8, 0x0021)
+        self._READ_RUNNING_DATA: ProtocolCommand = self._read_command(0x891c, 0x007d)
+        self._READ_METER_DATA: ProtocolCommand = self._read_command(0x8ca0, 0x2d)
+        self._READ_METER_DATA_EXTENDED: ProtocolCommand = self._read_command(0x8ca0, 0x3a)
+        self._READ_BATTERY_INFO: ProtocolCommand = self._read_command(0x9088, 0x0018)
+        self._READ_BATTERY2_INFO: ProtocolCommand = self._read_command(0x9858, 0x0016)
+        self._READ_MPPT_DATA: ProtocolCommand = self._read_command(0x89e5, 0x3d)
         self._has_eco_mode_v2: bool = True
         self._has_peak_shaving: bool = True
         self._has_battery: bool = True
         self._has_battery2: bool = False
         self._has_meter_extended: bool = False
         self._has_mppt: bool = False
         self._sensors = self.__all_sensors
@@ -474,70 +478,64 @@
             self._has_mppt = True
             self._has_meter_extended = True
         else:
             self._sensors_meter = tuple(filter(self._not_extended_meter, self._sensors_meter))
 
         # Check and add EcoModeV2 settings added in (ETU fw 19)
         try:
-            await self._read_from_socket(ModbusReadCommand(self.comm_addr, 47547, 6))
+            await self._read_from_socket(self._read_command(47547, 6))
             self._settings.update({s.id_: s for s in self.__settings_arm_fw_19})
         except RequestRejectedException as ex:
             if ex.message == 'ILLEGAL DATA ADDRESS':
-                logger.debug("EcoModeV2 settings not supported, switching to EcoModeV1.")
+                logger.debug("Cannot read EcoModeV2 settings, using to EcoModeV1.")
                 self._has_eco_mode_v2 = False
-        except RequestFailedException as ex:
-            logger.debug("Cannot read EcoModeV2 settings, switching to EcoModeV1.")
-            self._has_eco_mode_v2 = False
 
         # Check and add Peak Shaving settings added in (ETU fw 22)
         try:
-            await self._read_from_socket(ModbusReadCommand(self.comm_addr, 47589, 6))
+            await self._read_from_socket(self._read_command(47589, 6))
             self._settings.update({s.id_: s for s in self.__settings_arm_fw_22})
         except RequestRejectedException as ex:
             if ex.message == 'ILLEGAL DATA ADDRESS':
-                logger.debug("PeakShaving setting not supported, disabling it.")
+                logger.debug("Cannot read PeakShaving setting, disabling it.")
                 self._has_peak_shaving = False
-        except RequestFailedException as ex:
-            logger.debug("Cannot read _has_peak_shaving settings, disabling it.")
-            self._has_peak_shaving = False
 
     async def read_runtime_data(self) -> Dict[str, Any]:
         response = await self._read_from_socket(self._READ_RUNNING_DATA)
         data = self._map_response(response, self._sensors)
 
         self._has_battery = data.get('battery_mode', 0) != 0
         if self._has_battery:
             try:
                 response = await self._read_from_socket(self._READ_BATTERY_INFO)
                 data.update(self._map_response(response, self._sensors_battery))
             except RequestRejectedException as ex:
                 if ex.message == 'ILLEGAL DATA ADDRESS':
-                    logger.warning("Battery values not supported, disabling further attempts.")
+                    logger.warning("Cannot read battery values, disabling further attempts.")
                     self._has_battery = False
                 else:
                     raise ex
         if self._has_battery2:
             try:
                 response = await self._read_from_socket(self._READ_BATTERY2_INFO)
                 data.update(
                     self._map_response(response, self._sensors_battery2))
             except RequestRejectedException as ex:
                 if ex.message == 'ILLEGAL DATA ADDRESS':
-                    logger.warning("Battery 2 values not supported, disabling further attempts.")
+                    logger.warning("Cannot read battery 2 values, disabling further attempts.")
                     self._has_battery2 = False
                 else:
                     raise ex
 
         if self._has_meter_extended:
             try:
                 response = await self._read_from_socket(self._READ_METER_DATA_EXTENDED)
                 data.update(self._map_response(response, self._sensors_meter))
             except RequestRejectedException as ex:
                 if ex.message == 'ILLEGAL DATA ADDRESS':
-                    logger.warning("Extended meter values not supported, disabling further attempts.")
+                    logger.warning("Cannot read extended meter values, disabling further attempts.")
                     self._has_meter_extended = False
                     self._sensors_meter = tuple(filter(self._not_extended_meter, self._sensors_meter))
                     response = await self._read_from_socket(self._READ_METER_DATA)
                     data.update(
                         self._map_response(response, self._sensors_meter))
                 else:
                     raise ex
@@ -547,50 +545,50 @@
 
         if self._has_mppt:
             try:
                 response = await self._read_from_socket(self._READ_MPPT_DATA)
                 data.update(self._map_response(response, self._sensors_mppt))
             except RequestRejectedException as ex:
                 if ex.message == 'ILLEGAL DATA ADDRESS':
-                    logger.warning("MPPT values not supported, disabling further attempts.")
+                    logger.warning("Cannot read MPPT values, disabling further attempts.")
                     self._has_mppt = False
                 else:
                     raise ex
 
         return data
 
     async def read_setting(self, setting_id: str) -> Any:
         setting = self._settings.get(setting_id)
         if not setting:
             raise ValueError(f'Unknown setting "{setting_id}"')
         return await self._read_setting(setting)
 
     async def _read_setting(self, setting: Sensor) -> Any:
         count = (setting.size_ + (setting.size_ % 2)) // 2
-        response = await self._read_from_socket(ModbusReadCommand(self.comm_addr, setting.offset, count))
+        response = await self._read_from_socket(self._read_command(setting.offset, count))
         return setting.read_value(response)
 
     async def write_setting(self, setting_id: str, value: Any):
         setting = self._settings.get(setting_id)
         if not setting:
             raise ValueError(f'Unknown setting "{setting_id}"')
         await self._write_setting(setting, value)
 
     async def _write_setting(self, setting: Sensor, value: Any):
         if setting.size_ == 1:
             # modbus can address/store only 16 bit values, read the other 8 bytes
-            response = await self._read_from_socket(ModbusReadCommand(self.comm_addr, setting.offset, 1))
+            response = await self._read_from_socket(self._read_command(setting.offset, 1))
             raw_value = setting.encode_value(value, response.response_data()[0:2])
         else:
             raw_value = setting.encode_value(value)
         if len(raw_value) <= 2:
             value = int.from_bytes(raw_value, byteorder="big", signed=True)
-            await self._read_from_socket(ModbusWriteCommand(self.comm_addr, setting.offset, value))
+            await self._read_from_socket(self._write_command(setting.offset, value))
         else:
-            await self._read_from_socket(ModbusWriteMultiCommand(self.comm_addr, setting.offset, raw_value))
+            await self._read_from_socket(self._write_multi_command(setting.offset, raw_value))
 
     async def read_settings_data(self) -> Dict[str, Any]:
         data = {}
         for setting in self.settings():
             try:
                 value = await self.read_setting(setting.id_)
                 data[setting.id_] = value
@@ -613,15 +611,15 @@
         if not is_745_platform(self):
             result.remove(OperationMode.SELF_USE)
         if not include_emulated:
             result.remove(OperationMode.ECO_CHARGE)
             result.remove(OperationMode.ECO_DISCHARGE)
         return tuple(result)
 
-    async def get_operation_mode(self) -> OperationMode:
+    async def get_operation_mode(self) -> OperationMode | None:
         mode_id = await self.read_setting('work_mode')
         try:
             mode = OperationMode(mode_id)
         except ValueError:
             logger.debug("Unknown work_mode value %d", mode_id)
             return None
         if OperationMode.ECO != mode:
@@ -701,12 +699,12 @@
             result = result + self._sensors_mppt
         return result
 
     def settings(self) -> Tuple[Sensor, ...]:
         return tuple(self._settings.values())
 
     async def _clear_battery_mode_param(self) -> None:
-        await self._read_from_socket(ModbusWriteCommand(self.comm_addr, 0xb9ad, 1))
+        await self._read_from_socket(self._write_command(0xb9ad, 1))
 
     async def _set_offline(self, mode: bool) -> None:
         value = bytes.fromhex('00070000') if mode else bytes.fromhex('00010000')
-        await self._read_from_socket(ModbusWriteMultiCommand(self.comm_addr, 0xb997, value))
+        await self._read_from_socket(self._write_multi_command(0xb997, value))
```

### Comparing `goodwe-0.3.5/goodwe/exceptions.py` & `goodwe-0.4.0/goodwe/exceptions.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.5/goodwe/inverter.py` & `goodwe-0.4.0/goodwe/inverter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
-import asyncio
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum, IntEnum
 from typing import Any, Callable, Dict, Tuple, Optional
 
 from .exceptions import MaxRetriesException, RequestFailedException
-from .protocol import ProtocolCommand, ProtocolResponse
+from .protocol import InverterProtocol, ProtocolCommand, ProtocolResponse, TcpInverterProtocol, UdpInverterProtocol
 
 logger = logging.getLogger(__name__)
 
 
 class SensorKind(Enum):
     """
     Enumeration of sensor kinds.
@@ -83,66 +82,57 @@
 
 class Inverter(ABC):
     """
     Common superclass for various inverter models implementations.
     Represents the inverter state and its basic behavior
     """
 
-    def __init__(self, host: str, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
-        self.host: str = host
-        self.comm_addr: int = comm_addr
-        self.timeout: int = timeout
-        self.retries: int = retries
-        self._running_loop: asyncio.AbstractEventLoop | None = None
-        self._lock: asyncio.Lock | None = None
+    def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
+        self._protocol: InverterProtocol = self._create_protocol(host, port, timeout, retries)
         self._consecutive_failures_count: int = 0
 
+        self.comm_addr: int = comm_addr
+
         self.model_name: str | None = None
         self.serial_number: str | None = None
         self.rated_power: int = 0
         self.ac_output_type: int | None = None
         self.firmware: str | None = None
         self.arm_firmware: str | None = None
         self.modbus_version: int | None = None
         self.dsp1_version: int = 0
         self.dsp2_version: int = 0
         self.dsp_svn_version: int | None = None
         self.arm_version: int = 0
         self.arm_svn_version: int | None = None
 
-    def _ensure_lock(self) -> asyncio.Lock:
-        """Validate (or create) asyncio Lock.
-
-           The asyncio.Lock must always be created from within's asyncio loop,
-           so it cannot be eagerly created in constructor.
-           Additionally, since asyncio.run() creates and closes its own loop,
-           the lock's scope (its creating loop) mus be verified to support proper
-           behavior in subsequent asyncio.run() invocations.
-        """
-        if self._lock and self._running_loop == asyncio.get_event_loop():
-            return self._lock
-        else:
-            logger.debug("Creating lock instance for current event loop.")
-            self._lock = asyncio.Lock()
-            self._running_loop = asyncio.get_event_loop()
-            return self._lock
+    def _read_command(self, offset: int, count: int) -> ProtocolCommand:
+        """Create read protocol command."""
+        return self._protocol.read_command(self.comm_addr, offset, count)
+
+    def _write_command(self, register: int, value: int) -> ProtocolCommand:
+        """Create write protocol command."""
+        return self._protocol.write_command(self.comm_addr, register, value)
+
+    def _write_multi_command(self, offset: int, values: bytes) -> ProtocolCommand:
+        """Create write multiple protocol command."""
+        return self._protocol.write_multi_command(self.comm_addr, offset, values)
 
     async def _read_from_socket(self, command: ProtocolCommand) -> ProtocolResponse:
-        async with self._ensure_lock():
-            try:
-                result = await command.execute(self.host, self.timeout, self.retries)
-                self._consecutive_failures_count = 0
-                return result
-            except MaxRetriesException:
-                self._consecutive_failures_count += 1
-                raise RequestFailedException(f'No valid response received even after {self.retries} retries',
-                                             self._consecutive_failures_count)
-            except RequestFailedException as ex:
-                self._consecutive_failures_count += 1
-                raise RequestFailedException(ex.message, self._consecutive_failures_count)
+        try:
+            result = await command.execute(self._protocol)
+            self._consecutive_failures_count = 0
+            return result
+        except MaxRetriesException:
+            self._consecutive_failures_count += 1
+            raise RequestFailedException(f'No valid response received even after {self._protocol.retries} retries',
+                                         self._consecutive_failures_count) from None
+        except RequestFailedException as ex:
+            self._consecutive_failures_count += 1
+            raise RequestFailedException(ex.message, self._consecutive_failures_count) from None
 
     @abstractmethod
     async def read_device_info(self):
         """
         Request the device information from the inverter.
         The inverter instance variables will be loaded with relevant data.
         """
@@ -186,16 +176,16 @@
         """
         raise NotImplementedError()
 
     async def send_command(
             self, command: bytes, validator: Callable[[bytes], bool] = lambda x: True
     ) -> ProtocolResponse:
         """
-        Send low level udp command (as bytes).
-        Answer command's raw response data.
+        Send low level command (as bytes).
+        Answer ProtocolResponse with command's raw response data.
         """
         return await self._read_from_socket(ProtocolCommand(command, validator))
 
     @abstractmethod
     async def get_grid_export_limit(self) -> int:
         """
         Get the current grid export limit in W
@@ -274,14 +264,21 @@
     def settings(self) -> Tuple[Sensor, ...]:
         """
         Return tuple of settings definitions
         """
         raise NotImplementedError()
 
     @staticmethod
+    def _create_protocol(host: str, port: int, timeout: int, retries: int) -> InverterProtocol:
+        if port == 502:
+            return TcpInverterProtocol(host, port, timeout, retries)
+        else:
+            return UdpInverterProtocol(host, port, timeout, retries)
+
+    @staticmethod
     def _map_response(response: ProtocolResponse, sensors: Tuple[Sensor, ...]) -> Dict[str, Any]:
         """Process the response data and return dictionary with runtime values"""
         result = {}
         for sensor in sensors:
             try:
                 result[sensor.id_] = sensor.read(response)
             except ValueError:
```

### Comparing `goodwe-0.3.5/goodwe/modbus.py` & `goodwe-0.4.0/goodwe/modbus.py`

 * *Files 22% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     """
     crc = 0xFFFF
     for ch in data:
         crc = (crc >> 8) ^ _CRC_16_TABLE[(crc ^ ch) & 0xFF]
     return crc
 
 
-def create_modbus_request(comm_addr: int, cmd: int, offset: int, value: int) -> bytes:
+def create_modbus_rtu_request(comm_addr: int, cmd: int, offset: int, value: int) -> bytes:
     """
-    Create modbus request.
+    Create modbus RTU request.
     data[0] is inverter address
     data[1] is modbus command
     data[2:3] is command offset parameter
     data[4:5] is command value parameter
     data[6:7] is crc-16 checksum
     """
     data: bytearray = bytearray(6)
@@ -70,17 +70,44 @@
     data[5] = value & 0xFF
     checksum = _modbus_checksum(data)
     data.append(checksum & 0xFF)
     data.append((checksum >> 8) & 0xFF)
     return bytes(data)
 
 
-def create_modbus_multi_request(comm_addr: int, cmd: int, offset: int, values: bytes) -> bytes:
+def create_modbus_tcp_request(comm_addr: int, cmd: int, offset: int, value: int) -> bytes:
     """
-    Create modbus (multi value) request.
+    Create modbus TCP request.
+    data[0:1] is transaction identifier
+    data[2:3] is protocol identifier (0)
+    data[4:5] message length
+    data[6] is inverter address
+    data[7] is modbus command
+    data[8:9] is command offset parameter
+    data[10:11] is command value parameter
+    """
+    data: bytearray = bytearray(12)
+    data[0] = 0
+    data[1] = 1  # Not transaction ID support yet
+    data[2] = 0
+    data[3] = 0
+    data[4] = 0
+    data[5] = 6
+    data[6] = comm_addr
+    data[7] = cmd
+    data[8] = (offset >> 8) & 0xFF
+    data[9] = offset & 0xFF
+    data[10] = (value >> 8) & 0xFF
+    data[11] = value & 0xFF
+    return bytes(data)
+
+
+def create_modbus_rtu_multi_request(comm_addr: int, cmd: int, offset: int, values: bytes) -> bytes:
+    """
+    Create modbus RTU (multi value) request.
     data[0] is inverter address
     data[1] is modbus command
     data[2:3] is command offset parameter
     data[4:5] is number of registers
     data[6] is number of bytes
     data[7-n] is data payload
     data[n+1:n+2] is crc-16 checksum
@@ -96,17 +123,48 @@
     data.extend(values)
     checksum = _modbus_checksum(data)
     data.append(checksum & 0xFF)
     data.append((checksum >> 8) & 0xFF)
     return bytes(data)
 
 
-def validate_modbus_response(data: bytes, cmd: int, offset: int, value: int) -> bool:
+def create_modbus_tcp_multi_request(comm_addr: int, cmd: int, offset: int, values: bytes) -> bytes:
+    """
+    Create modbus TCP (multi value) request.
+    data[0:1] is transaction identifier
+    data[2:3] is protocol identifier (0)
+    data[4:5] message length
+    data[6] is inverter address
+    data[7] is modbus command
+    data[8:9] is command offset parameter
+    data[10:11] is number of registers
+    data[12] is number of bytes
+    data[13-n] is data payload
+    """
+    data: bytearray = bytearray(13)
+    data[0] = 0
+    data[1] = 1  # Not transaction ID support yet
+    data[2] = 0
+    data[3] = 0
+    data[4] = 0
+    data[5] = 7 + len(values)
+    data[6] = comm_addr
+    data[7] = cmd
+    data[8] = (offset >> 8) & 0xFF
+    data[9] = offset & 0xFF
+    data[10] = 0
+    data[11] = len(values) // 2
+    data[12] = len(values)
+    data.extend(values)
+    return bytes(data)
+
+
+def validate_modbus_rtu_response(data: bytes, cmd: int, offset: int, value: int) -> bool:
     """
-    Validate the modbus response.
+    Validate the modbus RTU response.
     data[0:1] is header
     data[2] is source address
     data[3] is command return type
     data[4] is response payload length (for read commands)
     data[-2:] is crc-16 checksum
     """
     if len(data) <= 4:
@@ -143,7 +201,49 @@
 
     if data[3] != cmd:
         failure_code = FAILURE_CODES.get(data[4], "UNKNOWN")
         logger.debug("Response is command failure: %s.", FAILURE_CODES.get(data[4], "UNKNOWN"))
         raise RequestRejectedException(failure_code)
 
     return True
+
+
+def validate_modbus_tcp_response(data: bytes, cmd: int, offset: int, value: int) -> bool:
+    """
+    Validate the modbus TCP response.
+    data[0:1] is transaction identifier
+    data[2:3] is protocol identifier (0)
+    data[4:5] message length
+    data[6] is source address
+    data[7] is command return type
+    data[8] is response payload length (for read commands)
+    """
+    if len(data) <= 8:
+        logger.debug("Response is too short.")
+        return False
+    if data[7] == MODBUS_READ_CMD:
+        if data[8] != value * 2:
+            logger.debug("Response has unexpected length: %d, expected %d.", data[8], value * 2)
+            return False
+        expected_length = data[8] + 9
+        if len(data) < expected_length:
+            logger.debug("Response is too short: %d, expected %d.", len(data), expected_length)
+            return False
+    elif data[7] in (MODBUS_WRITE_CMD, MODBUS_WRITE_MULTI_CMD):
+        if len(data) < 12:
+            logger.debug("Response has unexpected length: %d, expected %d.", len(data), 14)
+            return False
+        response_offset = int.from_bytes(data[8:10], byteorder='big', signed=False)
+        if response_offset != offset:
+            logger.debug("Response has wrong offset: %X, expected %X.", response_offset, offset)
+            return False
+        response_value = int.from_bytes(data[10:12], byteorder='big', signed=True)
+        if response_value != value:
+            logger.debug("Response has wrong value: %X, expected %X.", response_value, value)
+            return False
+
+    if data[7] != cmd:
+        failure_code = FAILURE_CODES.get(data[8], "UNKNOWN")
+        logger.debug("Response is command failure: %s.", FAILURE_CODES.get(data[8], "UNKNOWN"))
+        raise RequestRejectedException(failure_code)
+
+    return True
```

### Comparing `goodwe-0.3.5/goodwe/model.py` & `goodwe-0.4.0/goodwe/model.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.5/goodwe/sensor.py` & `goodwe-0.4.0/goodwe/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -877,20 +877,23 @@
     """Retrieve frequency [Hz] value (2 bytes) from buffer"""
     if offset is not None:
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(2), byteorder="big", signed=True)
     return float(value) / 100
 
 
-def read_temp(buffer: ProtocolResponse, offset: int = None) -> float:
+def read_temp(buffer: ProtocolResponse, offset: int = None) -> float | None:
     """Retrieve temperature [C] value (2 bytes) from buffer"""
     if offset is not None:
         buffer.seek(offset)
     value = int.from_bytes(buffer.read(2), byteorder="big", signed=True)
-    return float(value) / 10
+    if value == 32767:
+        return None
+    else:
+        return float(value) / 10
 
 
 def read_datetime(buffer: ProtocolResponse, offset: int = None) -> datetime:
     """Retrieve datetime value (6 bytes) from buffer"""
     if offset is not None:
         buffer.seek(offset)
     year = 2000 + int.from_bytes(buffer.read(1), byteorder='big')
```

### Comparing `goodwe-0.3.5/goodwe.egg-info/PKG-INFO` & `goodwe-0.4.0/goodwe.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.3.5
+Version: 0.4.0
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,23 +28,29 @@
 [![Python Versions](https://img.shields.io/pypi/pyversions/goodwe.svg)](https://github.com/marcelblijleven/goodwe/)
 [![Build Status](https://github.com/marcelblijleven/goodwe/actions/workflows/publish.yaml/badge.svg)](https://github.com/marcelblijleven/goodwe/actions/workflows/publish.yaml)
 ![License](https://img.shields.io/github/license/marcelblijleven/goodwe.svg)
 
 Library for connecting to GoodWe inverter over local network and retrieving runtime sensor values and configuration
 parameters.
 
-It has been reported to work on GoodWe ET, EH, BT, BH, ES, EM, BP, DT, MS, D-NS, and XS families of inverters. It may
-work on other inverters as well, as long as they listen on UDP port 8899 and respond to one of supported communication
-protocols.
+It has been reported to work with GoodWe ET, EH, BT, BH, ES, EM, BP, DT, MS, D-NS, and XS families of inverters. It
+should work with other inverters as well, as long as they listen on UDP port 8899 and respond to one of supported
+communication protocols.
+In general, if you can connect to your inverter with the official mobile app (SolarGo/PvMaster) over Wi-Fi (not
+bluetooth), this library should work.
 
 (If you can't communicate with the inverter despite your model is listed above, it is possible you have old ARM firmware
 version. You should ask manufacturer support to upgrade your ARM firmware (not just inverter firmware) to be able to
-communicate with the inveter via UDP.)
+communicate with the inverter via UDP.)
 
-White-label (GoodWe manufactured) inverters may work as well, e.g. General Electric GEP (PSB, PSC) and GEH models.
+White-label (GoodWe manufactured) inverters may work as well, e.g. General Electric GEP (PSB, PSC) and GEH models are
+know to work properly.
+
+Since v0.4.x the library also supports standard Modbus/TCP over port 502.
+This protocol is supported by the V2.0 version of LAN+WiFi communication dongle (model WLA0000-01-00P).
 
 ## Usage
 
 1. Install this package `pip install goodwe`
 2. Write down your GoodWe inverter's IP address (or invoke `goodwe.search_inverters()`)
 3. Connect to inverter and read all runtime data, example below
 
@@ -68,8 +74,7 @@
 ```
 
 ## References and useful links
 
 - https://github.com/mletenay/home-assistant-goodwe-inverter
 - https://github.com/yasko-pv/modbus-log
 - https://github.com/tkubec/GoodWe
-- https://github.com/OpenEMS/openems
```

### Comparing `goodwe-0.3.5/setup.cfg` & `goodwe-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.5/tests/test_dt.py` & `goodwe-0.4.0/tests/test_dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from goodwe.protocol import ProtocolCommand, ProtocolResponse
 
 
 class DtMock(TestCase, DT):
 
     def __init__(self, methodName='runTest'):
         TestCase.__init__(self, methodName)
-        DT.__init__(self, "localhost")
+        DT.__init__(self, "localhost", 8899)
         self.sensor_map = {s.id_: s.unit for s in self.sensors()}
         self._mock_responses = {}
 
     def mock_response(self, command: ProtocolCommand, filename: str):
         self._mock_responses[command] = filename
 
     async def _read_from_socket(self, command: ProtocolCommand) -> ProtocolResponse:
```

### Comparing `goodwe-0.3.5/tests/test_es.py` & `goodwe-0.4.0/tests/test_es.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from goodwe.protocol import ProtocolCommand, ProtocolResponse
 
 
 class EsMock(TestCase, ES):
 
     def __init__(self, methodName='runTest'):
         TestCase.__init__(self, methodName)
-        ES.__init__(self, "localhost")
+        ES.__init__(self, "localhost", 8899)
         self.sensor_map = {s.id_: s.unit for s in self.sensors()}
         self._mock_responses = {}
 
     def mock_response(self, command: ProtocolCommand, filename: str):
         self._mock_responses[command] = filename
 
     async def _read_from_socket(self, command: ProtocolCommand) -> ProtocolResponse:
```

### Comparing `goodwe-0.3.5/tests/test_et.py` & `goodwe-0.4.0/tests/test_et.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,38 +2,36 @@
 import os
 from datetime import datetime
 from unittest import TestCase
 
 from goodwe.et import ET
 from goodwe.exceptions import RequestRejectedException, RequestFailedException
 from goodwe.inverter import OperationMode
-from goodwe.protocol import ModbusReadCommand, ProtocolCommand, ProtocolResponse
+from goodwe.protocol import ModbusRtuReadCommand, ProtocolCommand, ProtocolResponse
 
 
 class EtMock(TestCase, ET):
 
     def __init__(self, methodName='runTest'):
         TestCase.__init__(self, methodName)
-        ET.__init__(self, "localhost")
+        ET.__init__(self, "localhost", 8899)
         self.sensor_map = {s.id_: s.unit for s in self.sensors()}
         self._mock_responses = {}
         self._list_of_requests = []
 
     def mock_response(self, command: ProtocolCommand, filename: str):
         self._mock_responses[command] = filename
 
     async def _read_from_socket(self, command: ProtocolCommand) -> ProtocolResponse:
         """Mock UDP communication"""
         root_dir = os.path.dirname(os.path.abspath(__file__))
         filename = self._mock_responses.get(command)
         if filename is not None:
             if 'ILLEGAL DATA ADDRESS' == filename:
                 raise RequestRejectedException('ILLEGAL DATA ADDRESS')
-            if 'NO RESPONSE' == filename:
-                raise RequestFailedException()
             with open(root_dir + '/sample/et/' + filename, 'r') as f:
                 response = bytes.fromhex(f.read())
                 if not command.validator(response):
                     raise RequestFailedException
                 return ProtocolResponse(response, command)
         else:
             self.request = command.request
@@ -54,17 +52,17 @@
 
     def __init__(self, methodName='runTest'):
         EtMock.__init__(self, methodName)
         self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW10K-ET_device_info_fw617.hex')
         self.mock_response(self._READ_RUNNING_DATA, 'GW10K-ET_running_data.hex')
         self.mock_response(self._READ_METER_DATA, 'GW10K-ET_meter_data.hex')
         self.mock_response(self._READ_BATTERY_INFO, 'GW10K-ET_battery_info.hex')
-        self.mock_response(ModbusReadCommand(self.comm_addr, 47547, 6), 'ILLEGAL DATA ADDRESS')
-        self.mock_response(ModbusReadCommand(self.comm_addr, 47589, 6), 'ILLEGAL DATA ADDRESS')
-        self.mock_response(ModbusReadCommand(self.comm_addr, 47515, 4), 'eco_mode_v1.hex')
+        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47547, 6), 'ILLEGAL DATA ADDRESS')
+        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47589, 6), 'ILLEGAL DATA ADDRESS')
+        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47515, 4), 'eco_mode_v1.hex')
 
     def test_GW10K_ET_device_info(self):
         self.loop.run_until_complete(self.read_device_info())
         self.assertEqual('GW10K-ET', self.model_name)
         self.assertEqual('9010KETU000W0000', self.serial_number)
         self.assertEqual(10000, self.rated_power)
         self.assertEqual(1, self.modbus_version)
@@ -308,16 +306,16 @@
 
 
 class GW10K_ET_fw819_Test(EtMock):
 
     def __init__(self, methodName='runTest'):
         EtMock.__init__(self, methodName)
         self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW10K-ET_device_info_fw819.hex')
-        self.mock_response(ModbusReadCommand(self.comm_addr, 47547, 6), 'eco_mode_v2.hex')
-        self.mock_response(ModbusReadCommand(self.comm_addr, 47589, 6), 'ILLEGAL DATA ADDRESS')
+        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47547, 6), 'eco_mode_v2.hex')
+        self.mock_response(ModbusRtuReadCommand(self.comm_addr, 47589, 6), 'ILLEGAL DATA ADDRESS')
         asyncio.get_event_loop().run_until_complete(self.read_device_info())
 
     def test_GW10K_ET_fw819_device_info(self):
         self.assertEqual('0GW10K-ET', self.model_name)
         self.assertEqual('9010KETU00000000', self.serial_number)
         self.assertEqual(10000, self.rated_power)
         self.assertEqual(1, self.modbus_version)
@@ -432,15 +430,15 @@
         self.assertSensor('load_mode1', 0, '', data)
         self.assertSensor('backup_p1', 0, 'W', data)
         self.assertSensor('load_p1', 1724, 'W', data)
         self.assertSensor('load_ptotal', 1725, 'W', data)
         self.assertSensor('backup_ptotal', 0, 'W', data)
         self.assertSensor('ups_load', 0, '%', data)
         self.assertSensor('temperature_air', 60.4, 'C', data)
-        self.assertSensor('temperature_module', 3276.7, 'C', data)
+        self.assertSensor('temperature_module', None, 'C', data)
         self.assertSensor('temperature', 38.6, 'C', data)
         self.assertSensor('function_bit', 256, '', data)
         self.assertSensor('bus_voltage', 380.6, 'V', data)
         self.assertSensor('nbus_voltage', 0, 'V', data)
         self.assertSensor('vbattery1', 0.0, 'V', data)
         self.assertSensor('ibattery1', 0.1, 'A', data)
         self.assertSensor('pbattery1', 0, 'W', data)
@@ -1194,30 +1192,7 @@
         self.assertSensor('reactive_power2', 0, 'var', data)
         self.assertSensor('reactive_power3', 0, 'var', data)
         self.assertSensor('apparent_power1', 0, 'VA', data)
         self.assertSensor('apparent_power2', 0, 'VA', data)
         self.assertSensor('apparent_power3', 0, 'VA', data)
 
         self.assertFalse(self.sensor_map, f"Some sensors were not tested {self.sensor_map}")
-
-
-class GW5K_BT_Test(EtMock):
-
-    def __init__(self, methodName='runTest'):
-        EtMock.__init__(self, methodName)
-        self.mock_response(self._READ_DEVICE_VERSION_INFO, 'GW5K-BT_device_info.hex')
-        self.mock_response(ModbusReadCommand(self.comm_addr, 47547, 6), 'NO RESPONSE')
-
-    def test_GW5K_BT_device_info(self):
-        self.loop.run_until_complete(self.read_device_info())
-        self.assertEqual('GW5K-BT', self.model_name)
-        self.assertEqual('95000BTU203W0000', self.serial_number)
-        self.assertEqual(5000, self.rated_power)
-        self.assertEqual(0, self.modbus_version)
-        self.assertEqual(254, self.ac_output_type)
-        self.assertEqual(3, self.dsp1_version)
-        self.assertEqual(3, self.dsp2_version)
-        self.assertEqual(124, self.dsp_svn_version)
-        self.assertEqual(11, self.arm_version)
-        self.assertEqual(147, self.arm_svn_version)
-        self.assertEqual('04029-03-S10', self.firmware)
-        self.assertEqual('02041-11-S00', self.arm_firmware)
```

### Comparing `goodwe-0.3.5/tests/test_protocol.py` & `goodwe-0.4.0/tests/test_protocol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-from typing import Callable
 from unittest import TestCase, mock
 
-from goodwe.exceptions import MaxRetriesException
-from goodwe.protocol import Aa55ReadCommand, Aa55WriteCommand, Aa55WriteMultiCommand, ModbusReadCommand, \
-    ModbusWriteCommand, ModbusWriteMultiCommand, ProtocolCommand, UdpInverterProtocol
+from goodwe.protocol import *
 
 
 class TestUDPClientProtocol(TestCase):
     def setUp(self) -> None:
-        self.command = ProtocolCommand(bytes.fromhex('636f666665650d0a'), lambda x: True)
-        self.response_future = mock.Mock()
-        #        self.processor = mock.Mock()
-        self.protocol = UdpInverterProtocol(self.response_future, self.command, 1, 3)
+        self.protocol = UdpInverterProtocol('127.0.0.1', 1337, 1, 3)
+        self.protocol.command = ProtocolCommand(bytes.fromhex('636f666665650d0a'), lambda x: True)
+        self.protocol.response_future = mock.Mock()
 
     def test_datagram_received(self):
         data = b'this is mock data'
         self.protocol.datagram_received(data, ('127.0.0.1', 1337))
-        self.response_future.set_result.assert_called_once()
+        self.protocol.response_future.set_result.assert_called_once()
 
     #        self.processor.assert_called_once_with(data)
 
     #    def test_datagram_received_process_exception(self):
     #        data = b'this is mock data'
 
     #        self.protocol.processor.side_effect = TypeError
@@ -28,92 +24,105 @@
     #        self.processor.assert_called_once_with(data)
     #        self.future.set_result.assert_not_called()
     #        self.future.set_exception.assert_called_once_with(ProcessingException)
 
     def test_error_received(self):
         exc = Exception('something went wrong')
         self.protocol.error_received(exc)
-        self.response_future.set_exception.assert_called_once_with(exc)
+        self.protocol.response_future.set_exception.assert_called_once_with(exc)
 
-    @mock.patch('goodwe.protocol.asyncio.get_event_loop')
+    @mock.patch('goodwe.protocol.asyncio.get_running_loop')
     def test_connection_made(self, mock_get_event_loop):
         transport = mock.Mock()
         mock_loop = mock.Mock()
         mock_get_event_loop.return_value = mock_loop
 
         mock_retry_mechanism = mock.Mock()
         self.protocol._retry_mechanism = mock_retry_mechanism
         self.protocol.connection_made(transport)
+        self.protocol._send_request(self.protocol.command, self.protocol.response_future)
 
         transport.sendto.assert_called_with(self.protocol.command.request)
         mock_get_event_loop.assert_called()
         mock_loop.call_later.assert_called_with(1, mock_retry_mechanism)
 
     def test_connection_lost(self):
-        self.response_future.done.return_value = True
+        self.protocol.response_future.done.return_value = True
         self.protocol.connection_lost(None)
-        self.response_future.cancel.assert_not_called()
+        self.protocol.response_future.cancel.assert_not_called()
 
     def test_connection_lost_not_done(self):
-        self.response_future.done.return_value = False
+        self.protocol.response_future.done.return_value = False
         self.protocol.connection_lost(None)
-        self.response_future.cancel.assert_called()
+        self.protocol.response_future.cancel.assert_called()
 
     def test_retry_mechanism(self):
         self.protocol._transport = mock.Mock()
-        self.protocol._send_message = mock.Mock()
-        self.response_future.done.return_value = True
+        self.protocol._send_request = mock.Mock()
+        self.protocol.response_future.done.return_value = True
         self.protocol._retry_mechanism()
 
-        self.protocol._transport.close.assert_called()
-        self.protocol._send_message.assert_not_called()
+        # self.protocol._transport.close.assert_called()
+        self.protocol._send_request.assert_not_called()
 
-    @mock.patch('goodwe.protocol.asyncio.get_event_loop')
+    @mock.patch('goodwe.protocol.asyncio.get_running_loop')
     def test_retry_mechanism_two_retries(self, mock_get_event_loop):
         def call_later(_: int, retry_func: Callable):
             retry_func()
 
         mock_loop = mock.Mock()
         mock_get_event_loop.return_value = mock_loop
         mock_loop.call_later = call_later
 
         self.protocol._transport = mock.Mock()
-        self.response_future.done.side_effect = [False, False, True]
+        self.protocol.response_future.done.side_effect = [False, False, True, False]
         self.protocol._retry_mechanism()
 
-        self.protocol._transport.close.assert_called()
-        self.assertEqual(self.protocol._retries, 2)
+        # self.protocol._transport.close.assert_called()
+        self.assertEqual(self.protocol._retry, 2)
 
-    @mock.patch('goodwe.protocol.asyncio.get_event_loop')
+    @mock.patch('goodwe.protocol.asyncio.get_running_loop')
     def test_retry_mechanism_max_retries(self, mock_get_event_loop):
         def call_later(_: int, retry_func: Callable):
             retry_func()
 
         mock_loop = mock.Mock()
         mock_get_event_loop.return_value = mock_loop
         mock_loop.call_later = call_later
 
         self.protocol._transport = mock.Mock()
-        self.response_future.done.side_effect = [False, False, False, False, False]
+        self.protocol.response_future.done.side_effect = [False, False, False, False, False]
         self.protocol._retry_mechanism()
-        self.response_future.set_exception.assert_called_once_with(MaxRetriesException)
-        self.assertEqual(self.protocol._retries, 3)
+        self.protocol.response_future.set_exception.assert_called_once_with(MaxRetriesException)
+        self.assertEqual(self.protocol._retry, 3)
 
-    def test_modbus_read_command(self):
-        command = ModbusReadCommand(0xf7, 0x88b8, 0x0021)
+    def test_modbus_rtu_read_command(self):
+        command = ModbusRtuReadCommand(0xf7, 0x88b8, 0x0021)
         self.assertEqual(bytes.fromhex('f70388b800213ac1'), command.request)
 
-    def test_modbus_write_command(self):
-        command = ModbusWriteCommand(0xf7, 0xb798, 0x0002)
+    def test_modbus_rtu_write_command(self):
+        command = ModbusRtuWriteCommand(0xf7, 0xb798, 0x0002)
         self.assertEqual(bytes.fromhex('f706b7980002bac6'), command.request)
 
-    def test_modbus_write_multi_command(self):
-        command = ModbusWriteMultiCommand(0xf7, 0xb798, bytes.fromhex('08070605'))
+    def test_modbus_rtu_write_multi_command(self):
+        command = ModbusRtuWriteMultiCommand(0xf7, 0xb798, bytes.fromhex('08070605'))
         self.assertEqual(bytes.fromhex('f710b79800020408070605851b'), command.request)
 
+    def test_modbus_tcp_read_command(self):
+        command = ModbusTcpReadCommand(180, 310, 2)
+        self.assertEqual(bytes.fromhex('000100000006b40301360002'), command.request)
+
+    def test_modbus_tcp_write_command(self):
+        command = ModbusTcpWriteCommand(180, 310, 0x4556)
+        self.assertEqual(bytes.fromhex('000100000006B40601364556'), command.request)
+
+    def test_modbus_tcp_write_multi_command(self):
+        command = ModbusTcpWriteMultiCommand(0xf7, 0xb798, bytes.fromhex('08070605'))
+        self.assertEqual(bytes.fromhex('00010000000bf710b79800020408070605'), command.request)
+
     def test_aa55_read_command(self):
         command = Aa55ReadCommand(0x0701, 16)
         self.assertEqual(bytes.fromhex('AA55C07F011A030701100274'), command.request)
 
     def test_aa55_write_command(self):
         command = Aa55WriteCommand(0x0560, 0x0002)
         self.assertEqual(bytes.fromhex('AA55C07F023905056001000202E6'), command.request)
```

### Comparing `goodwe-0.3.5/tests/test_sensor.py` & `goodwe-0.4.0/tests/test_sensor.py`

 * *Files identical despite different names*


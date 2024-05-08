# Comparing `tmp/yoto_api-1.7.9.tar.gz` & `tmp/yoto_api-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.7.9.tar", last modified: Sun May  5 21:37:00 2024, max compression
+gzip compressed data, was "yoto_api-1.8.0.tar", last modified: Wed May  8 01:58:49 2024, max compression
```

## Comparing `yoto_api-1.7.9.tar` & `yoto_api-1.8.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:37:00.541927 yoto_api-1.7.9/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-05 21:36:39.000000 yoto_api-1.7.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-05 21:36:39.000000 yoto_api-1.7.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 21:36:39.000000 yoto_api-1.7.9/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 21:36:39.000000 yoto_api-1.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 21:36:39.000000 yoto_api-1.7.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-05 21:37:00.541927 yoto_api-1.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-05 21:36:39.000000 yoto_api-1.7.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 21:36:39.000000 yoto_api-1.7.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 21:37:00.541927 yoto_api-1.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-05 21:36:54.000000 yoto_api-1.7.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:37:00.537927 yoto_api-1.7.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 21:36:39.000000 yoto_api-1.7.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-05 21:36:39.000000 yoto_api-1.7.9/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:37:00.537927 yoto_api-1.7.9/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    27730 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-05 21:36:39.000000 yoto_api-1.7.9/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 21:37:00.541927 yoto_api-1.7.9/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 21:37:00.000000 yoto_api-1.7.9/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:49.033391 yoto_api-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 01:58:28.000000 yoto_api-1.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-08 01:58:28.000000 yoto_api-1.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 01:58:28.000000 yoto_api-1.8.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 01:58:28.000000 yoto_api-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-08 01:58:28.000000 yoto_api-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-08 01:58:49.033391 yoto_api-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-08 01:58:28.000000 yoto_api-1.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 01:58:28.000000 yoto_api-1.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:58:49.033391 yoto_api-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-08 01:58:43.000000 yoto_api-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:49.029391 yoto_api-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:28.000000 yoto_api-1.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 01:58:28.000000 yoto_api-1.8.0/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:49.033391 yoto_api-1.8.0/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23967 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/YotoMQTTClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 01:58:28.000000 yoto_api-1.8.0/yoto_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:58:49.033391 yoto_api-1.8.0/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:58:48.000000 yoto_api-1.8.0/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 01:58:49.000000 yoto_api-1.8.0/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.7.9/CONTRIBUTING.rst` & `yoto_api-1.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.9/LICENSE` & `yoto_api-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.9/PKG-INFO` & `yoto_api-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.9
+Version: 1.8.0
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.7.9/README.rst` & `yoto_api-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.9/setup.py` & `yoto_api-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.7.9",
+    version="1.8.0",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.7.9/yoto_api/Card.py` & `yoto_api-1.8.0/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.7.9/yoto_api/YotoAPI.py` & `yoto_api-1.8.0/yoto_api/YotoAPI.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 """API Methods"""
 
 import requests
 import logging
 import datetime
-import re
-import paho.mqtt.client as mqtt
 
 from datetime import timedelta
 import pytz
 from .const import DOMAIN, LIGHT_COLORS, POWER_SOURCE
 from .Token import Token
 from .Card import Card
 from .YotoPlayer import YotoPlayer
+from .utils import get_child_value, parse_datetime
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class YotoAPI:
     def __init__(self) -> None:
         self.BASE_URL: str = "https://api.yotoplay.com"
         self.CLIENT_ID: str = "4P2do5RhHDXvCDZDZ6oti27Ft2XdRrzr"
         self.LOGIN_URL: str = "login.yotoplay.com"
         self.TOKEN_URL: str = "https://api.yotoplay.com/auth/token"
-        self.SCOPE: str = "YOUR_SCOPE"
-        self.MQTT_AUTH_NAME: str = "JwtAuthorizer_mGDDmvLsocFY"
-        self.MQTT_URL: str = "aqrphjqbp3u2z-ats.iot.eu-west-2.amazonaws.com"
 
     def login(self, username: str, password: str) -> Token:
         url = self.TOKEN_URL
         payload = {}
         payload["audience"] = self.BASE_URL
         payload["client_id"] = self.CLIENT_ID
         payload["grant_type"] = "password"
@@ -70,105 +66,103 @@
 
     # pass='audience=https%3A//api.yotoplay.com&client_id=FILL_THIS_IN&grant_type=password&password=FILL_THIS_IN&scope=openid%20email%20profile%20offline_access&username=FILL_THIS_IN%40gmail.com'
     # curl -d "$pass" https://api.yotoplay.com/auth/token | jq '.access_token'
 
     def update_players(self, token: Token, players: list[YotoPlayer]) -> None:
         response = self._get_devices(token)
         for item in response["devices"]:
-            if self.get_child_value(item, "deviceId") not in players:
+            if get_child_value(item, "deviceId") not in players:
                 player: YotoPlayer = YotoPlayer(
-                    id=self.get_child_value(item, "deviceId"),
+                    id=get_child_value(item, "deviceId"),
                 )
                 players[player.id] = player
-            deviceId = self.get_child_value(item, "deviceId")
-            players[deviceId].name = self.get_child_value(item, "name")
-            players[deviceId].device_type = self.get_child_value(item, "deviceType")
-            players[deviceId].online = self.get_child_value(item, "online")
+            deviceId = get_child_value(item, "deviceId")
+            players[deviceId].name = get_child_value(item, "name")
+            players[deviceId].device_type = get_child_value(item, "deviceType")
+            players[deviceId].online = get_child_value(item, "online")
 
             # Should we call here or make this a separate call from YM?  This could help us reduce API calls.
             player_status_response = self._get_device_status(token, deviceId)
-            players[deviceId].last_updated_at = self._parse_datetime(
-                self.get_child_value(player_status_response, "updatedAt"), pytz.utc
+            players[deviceId].last_updated_at = parse_datetime(
+                get_child_value(player_status_response, "updatedAt"), pytz.utc
             )
-            if self.get_child_value(player_status_response, "activeCard") != "none":
+            if get_child_value(player_status_response, "activeCard") != "none":
                 players[deviceId].is_playing = True
             else:
                 players[deviceId].is_playing = False
-            players[deviceId].active_card = self.get_child_value(
+            players[deviceId].active_card = get_child_value(
                 player_status_response, "activeCard"
             )
-            players[deviceId].ambient_light_sensor_reading = self.get_child_value(
+            players[deviceId].ambient_light_sensor_reading = get_child_value(
                 player_status_response, "ambientLightSensorReading"
             )
-            players[deviceId].battery_level_percentage = self.get_child_value(
+            players[deviceId].battery_level_percentage = get_child_value(
                 player_status_response, "batteryLevelPercentage"
             )
-            players[deviceId].day_mode_on = self.get_child_value(
+            players[deviceId].day_mode_on = get_child_value(
                 player_status_response, "dayMode"
             )
-            players[deviceId].user_volume = self.get_child_value(
+            players[deviceId].user_volume = get_child_value(
                 player_status_response, "userVolumePercentage"
             )
-            players[deviceId].system_volume = self.get_child_value(
+            players[deviceId].system_volume = get_child_value(
                 player_status_response, "systemVolumePercentage"
             )
-            players[deviceId].temperature_celcius = self.get_child_value(
+            players[deviceId].temperature_celcius = get_child_value(
                 player_status_response, "temperatureCelcius"
             )
-            players[deviceId].bluetooth_audio_connected = self.get_child_value(
+            players[deviceId].bluetooth_audio_connected = get_child_value(
                 player_status_response, "isBluetoothAudioConnected"
             )
-            players[deviceId].charging = self.get_child_value(
+            players[deviceId].charging = get_child_value(
                 player_status_response, "isCharging"
             )
-            players[deviceId].audio_device_connected = self.get_child_value(
+            players[deviceId].audio_device_connected = get_child_value(
                 player_status_response, "isAudioDeviceConnected"
             )
-            players[deviceId].firmware_version = self.get_child_value(
+            players[deviceId].firmware_version = get_child_value(
                 player_status_response, "firmwareVersion"
             )
-            players[deviceId].wifi_strength = self.get_child_value(
+            players[deviceId].wifi_strength = get_child_value(
                 player_status_response, "wifiStrength"
             )
-            players[deviceId].playing_source = self.get_child_value(
+            players[deviceId].playing_source = get_child_value(
                 player_status_response, "playingSource"
             )
             players[deviceId].night_light_mode = LIGHT_COLORS[
-                self.get_child_value(player_status_response, "nightlightMode")
+                get_child_value(player_status_response, "nightlightMode")
             ]
             players[deviceId].power_source = POWER_SOURCE[
-                self.get_child_value(player_status_response, "powerSource")
+                get_child_value(player_status_response, "powerSource")
             ]
 
     def update_library(self, token: Token, library: dict[Card]) -> list[Card]:
         response = self._get_cards(token)
         for item in response["cards"]:
-            if self.get_child_value(item, "cardId") not in library:
+            if get_child_value(item, "cardId") not in library:
                 card: Card = Card(
-                    id=self.get_child_value(item, "cardId"),
+                    id=get_child_value(item, "cardId"),
                 )
                 library[card.id] = card
-            cardId = self.get_child_value(item, "cardId")
-            library[cardId].title = self.get_child_value(item, "card.title")
-            library[cardId].description = self.get_child_value(
+            cardId = get_child_value(item, "cardId")
+            library[cardId].title = get_child_value(item, "card.title")
+            library[cardId].description = get_child_value(
                 item, "card.metadata.description"
             )
-            library[self.get_child_value(item, "cardId")].author = self.get_child_value(
+            library[get_child_value(item, "cardId")].author = get_child_value(
                 item, "card.metadata.author"
             )
-            library[cardId].category = self.get_child_value(
-                item, "card.metadata.stories"
-            )
-            library[cardId].coverImageL = self.get_child_value(
+            library[cardId].category = get_child_value(item, "card.metadata.stories")
+            library[cardId].coverImageL = get_child_value(
                 item, "card.metadata.cover.imageL"
             )
-            library[cardId].seriesOrder = self.get_child_value(
+            library[cardId].seriesOrder = get_child_value(
                 item, "card.metadata.cover.seriesorder"
             )
-            library[cardId].seriesTitle = self.get_child_value(
+            library[cardId].seriesTitle = get_child_value(
                 item, "card.metadata.cover.seriestitle"
             )
 
     def refresh_token(self, token: Token) -> Token:
         # audience=https%3A//api.yotoplay.com&client_id=FILL_THIS_IN&grant_type=refresh_token&refresh_token=FILL_THIS_IN&scope=openid%20email%20profile%20offline_access
         url = self.TOKEN_URL
         payload = {}
@@ -340,71 +334,14 @@
         #       "updatedAt": "2024-04-05T04:03:55.198Z",
         #       "createdAt": "2023-03-16T17:32:34.249Z",
         #       "lastPlayedAt": "2024-04-05T06:15:11.308Z",
         #       "masterUid": "04dedd46720000"
         #     }
         # }
 
-    def connect_mqtt(self, token: Token, deviceId: str):
-        def on_message(client, userdata, message):
-            # Process MQTT Message
-            _LOGGER.debug(
-                f"{DOMAIN} - MQTT Message: {str(message.payload.decode('utf-8'))}"
-            )
-            _LOGGER.debug(f"{DOMAIN} - MQTT Topic: {message.topic}")
-            _LOGGER.debug(f"{DOMAIN} - MQTT QOS: {message.qos}")
-            _LOGGER.debug(f"{DOMAIN} - MQTT Retain: {message.retain}")
-            parts = message.topic.split("/")
-            base, device, topic = parts
-            if topic == "status":
-                self._parse_status_message(
-                    str(message.payload.decode("utf-8")),
-                )
-
-        #             mqtt.CallbackAPIVersion.VERSION1,
-        client = mqtt.Client(
-            client_id="DASH" + deviceId,
-            transport="websockets",
-        )
-        client.username_pw_set(
-            username=deviceId + "?x-amz-customauthorizer-name=" + self.MQTT_AUTH_NAME,
-            password=token.access_token,
-        )
-        # client.on_connect = on_message
-        client.on_message = on_message
-        client.tls_set()
-        client.connect(host=self.MQTT_URL, port=443)
-        client.loop_start()
-        client.subscribe("device/" + deviceId + "/events")
-        client.subscribe("device/" + deviceId + "/status")
-        client.subscribe("device/" + deviceId + "/response")
-        # Command not needed but helps sniffing traffic
-        client.subscribe("device/" + deviceId + "/command")
-
-        # time.sleep(60)
-        # client.loop_stop()
-        return client
-
-    def card_pause(self, client, deviceId):
-        topic = "device/" + deviceId + "/command/card-pause"
-        payload = ""
-        self._publish_command(client, topic, payload)
-        # MQTT Message: {"status":{"card-pause":"OK","req_body":""}}
-
-    def card_play(self, client, deviceId):
-        topic = "device/" + deviceId + "/command/card-play"
-        self._publish_command(self, client, topic, "card-play")
-        # MQTT Message: {"status":{"card-play":"OK","req_body":"{\"uri\":\"https://yoto.io/7JtVV\",\"secondsIn\":0,\"cutOff\":0,\"chapterKey\":\"01\",\"trackKey\":\"01\",\"requestId\":\"5385910e-f853-4f34-99a4-d2ed94f02f6d\"}"}}
-
-    def _publish_command(self, client, topic, payload):
-        client.publish(topic, payload)
-
-    def _parse_status_message(self, message, player):
-        pass
-
     def _get_card_detail(self, token: Token, cardid: str) -> dict:
         ############## Details below from snooping JSON requests of the app ######################
 
         url = self.BASE_URL + "/card/details/" + cardid
         headers = self._get_authenticated_headers(token)
 
         response = requests.post(url, headers=headers).json()
@@ -545,44 +482,14 @@
     def _get_authenticated_headers(self, token: Token) -> dict:
         return {
             "User-Agent": "Yoto/2.73 (com.yotoplay.Yoto; build:10405; iOS 17.4.0) Alamofire/5.6.4",
             "Content-Type": "application/json",
             "Authorization": token.token_type + " " + token.access_token,
         }
 
-    def get_child_value(self, data, key):
-        value = data
-        for x in key.split("."):
-            try:
-                value = value[x]
-            except Exception:
-                try:
-                    value = value[int(x)]
-                except Exception:
-                    value = None
-        return value
-
-    def _parse_datetime(self, value, timezone) -> datetime.datetime:
-        if value is None:
-            return datetime.datetime(2000, 1, 1, tzinfo=timezone)
-
-        value = (
-            value.replace("-", "").replace("T", "").replace(":", "").replace("Z", "")
-        )
-        m = re.match(r"(\d{4})(\d{2})(\d{2})(\d{2})(\d{2})(\d{2})", value)
-        return datetime.datetime(
-            year=int(m.group(1)),
-            month=int(m.group(2)),
-            day=int(m.group(3)),
-            hour=int(m.group(4)),
-            minute=int(m.group(5)),
-            second=int(m.group(6)),
-            tzinfo=timezone,
-        )
-
 
 ######Endpoints:
 
 # api.yotoplay.com/device-v2/devices/mine
 # api.yotoplay.com/device-v2/$deviceid/status
 # api.yotoplay.com/media/displayIcons/user/me
 # api.yotoplay.com/user/details
```

### Comparing `yoto_api-1.7.9/yoto_api/YotoManager.py` & `yoto_api-1.8.0/yoto_api/YotoManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """YotoManager.py"""
 
 import datetime
 import logging
 import pytz
 
 from .YotoAPI import YotoAPI
+from .YotoMQTTClient import YotoMQTTClient
 from .Token import Token
 from .const import DOMAIN
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class YotoManager:
@@ -30,15 +31,16 @@
     def update_players_status(self) -> None:
         # Updates the data with current player data.
         self.api.update_players(self.token, self.players)
 
     def connect_to_events(self) -> None:
         for player in self.players.values():
             # Needs to be correct to handle multiple devices. 1 client per device
-            self.mqtt_client = self.api.connect_mqtt(self.token, player.id)
+            self.mqtt_client: YotoMQTTClient = YotoMQTTClient()
+            self.mqtt_client.connect_mqtt(self.token, player)
 
     def update_cards(self) -> None:
         # Updates library and all card data.  Typically only required on startup.
         # TODO: Should update the self.library object with a current dict of players. Should it do details for all cards too or separate?
         self.api.update_library(self.token, self.library)
 
     def pause_player(self, player_id: str):
```

### Comparing `yoto_api-1.7.9/yoto_api/YotoPlayer.py` & `yoto_api-1.8.0/yoto_api/YotoPlayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     bluetooth_audio_connected: bool = None
     charging: bool = None
     audio_device_connected: bool = None
     firmware_version: str = None
     wifi_strength: int = None
     power_source: str = None
 
+    # MQTT
+    repeat_all: bool = None
+
 
 # {'devices': [{'deviceId': 'XXXX', 'name': 'Yoto Player', 'description': 'nameless.limit', 'online': False, 'releaseChannel': 'general', 'deviceType': 'v3', 'deviceFamily': 'v3', 'deviceGroup': '', 'hasUserGivenName': False}]}
 # Device Status API: {'activeCard': 'none', 'ambientLightSensorReading': 0, 'averageDownloadSpeedBytesSecond': 0, 'batteryLevelPercentage': 100, 'buzzErrors': 0, 'cardInsertionState': 2, 'dayMode': 0, 'deviceId': 'XXXX', 'errorsLogged': 210, 'firmwareVersion': 'v2.17.5', 'freeDiskSpaceBytes': 30250544, 'isAudioDeviceConnected': False, 'isBackgroundDownloadActive': False, 'isBluetoothAudioConnected': False, 'isCharging': False, 'isOnline': True, 'networkSsid': 'XXXX', 'nightlightMode': '0x000000', 'playingSource': 0, 'powerCapabilities': '0x02', 'powerSource': 2, 'systemVolumePercentage': 47, 'taskWatchdogTimeoutCount': 0, 'temperatureCelcius': '20', 'totalDiskSpaceBytes': 31385600, 'updatedAt': '2024-04-23T01:26:19.927Z', 'uptime': 252342, 'userVolumePercentage': 50, 'utcOffsetSeconds': -21600, 'utcTime': 1713835609, 'wifiStrength': -61}
 # Mqtt response:
 
 {
     "status": {
```

### Comparing `yoto_api-1.7.9/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.8.0/yoto_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.7.9
+Version: 1.8.0
 Summary: A python package that makes it a bit easier to work with the yoto play API. Not associated with Yoto in any way.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```


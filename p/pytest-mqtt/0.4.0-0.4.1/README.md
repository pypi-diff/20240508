# Comparing `tmp/pytest-mqtt-0.4.0.tar.gz` & `tmp/pytest_mqtt-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-mqtt-0.4.0.tar", last modified: Sun Mar 31 17:07:23 2024, max compression
+gzip compressed data, was "pytest_mqtt-0.4.1.tar", last modified: Wed May  8 21:01:12 2024, max compression
```

## Comparing `pytest-mqtt-0.4.0.tar` & `pytest_mqtt-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-31 17:07:23.539394 pytest-mqtt-0.4.0/
--rw-r--r--   0 amo        (501) staff       (20)     1161 2022-09-20 10:04:35.000000 pytest-mqtt-0.4.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)     7910 2024-03-31 17:07:23.538830 pytest-mqtt-0.4.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     4920 2024-03-29 03:37:41.000000 pytest-mqtt-0.4.0/README.rst
--rw-r--r--   0 amo        (501) staff       (20)     4208 2024-03-31 17:07:13.000000 pytest-mqtt-0.4.0/pyproject.toml
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-31 17:07:23.534561 pytest-mqtt-0.4.0/pytest_mqtt/
--rw-r--r--   0 amo        (501) staff       (20)      358 2022-09-20 10:04:35.000000 pytest-mqtt-0.4.0/pytest_mqtt/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     5341 2024-03-29 03:52:16.000000 pytest-mqtt-0.4.0/pytest_mqtt/capmqtt.py
--rw-r--r--   0 amo        (501) staff       (20)      324 2024-03-29 02:22:41.000000 pytest-mqtt-0.4.0/pytest_mqtt/model.py
--rw-r--r--   0 amo        (501) staff       (20)     2989 2024-03-29 02:22:41.000000 pytest-mqtt-0.4.0/pytest_mqtt/mosquitto.py
--rw-r--r--   0 amo        (501) staff       (20)      576 2024-03-29 02:22:38.000000 pytest-mqtt-0.4.0/pytest_mqtt/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-03-31 17:07:23.536945 pytest-mqtt-0.4.0/pytest_mqtt.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     7910 2024-03-31 17:07:23.000000 pytest-mqtt-0.4.0/pytest_mqtt.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      367 2024-03-31 17:07:23.000000 pytest-mqtt-0.4.0/pytest_mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2024-03-31 17:07:23.000000 pytest-mqtt-0.4.0/pytest_mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       75 2024-03-31 17:07:23.000000 pytest-mqtt-0.4.0/pytest_mqtt.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      311 2024-03-31 17:07:23.000000 pytest-mqtt-0.4.0/pytest_mqtt.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       12 2024-03-31 17:07:23.000000 pytest-mqtt-0.4.0/pytest_mqtt.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)       38 2024-03-31 17:07:23.539462 pytest-mqtt-0.4.0/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)      210 2022-09-20 10:04:35.000000 pytest-mqtt-0.4.0/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-08 21:01:12.540969 pytest_mqtt-0.4.1/
+-rw-r--r--   0 amo        (501) staff       (20)     1161 2022-09-20 10:04:35.000000 pytest_mqtt-0.4.1/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)     7910 2024-05-08 21:01:12.540242 pytest_mqtt-0.4.1/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     4920 2024-03-29 03:37:41.000000 pytest_mqtt-0.4.1/README.rst
+-rw-r--r--   0 amo        (501) staff       (20)     4207 2024-05-08 21:01:06.000000 pytest_mqtt-0.4.1/pyproject.toml
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-08 21:01:12.533647 pytest_mqtt-0.4.1/pytest_mqtt/
+-rw-r--r--   0 amo        (501) staff       (20)      358 2022-09-20 10:04:35.000000 pytest_mqtt-0.4.1/pytest_mqtt/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     5341 2024-03-29 03:52:16.000000 pytest_mqtt-0.4.1/pytest_mqtt/capmqtt.py
+-rw-r--r--   0 amo        (501) staff       (20)      324 2024-03-29 02:22:41.000000 pytest_mqtt-0.4.1/pytest_mqtt/model.py
+-rw-r--r--   0 amo        (501) staff       (20)     3455 2024-05-08 20:59:25.000000 pytest_mqtt-0.4.1/pytest_mqtt/mosquitto.py
+-rw-r--r--   0 amo        (501) staff       (20)      576 2024-03-29 02:22:38.000000 pytest_mqtt-0.4.1/pytest_mqtt/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2024-05-08 21:01:12.537207 pytest_mqtt-0.4.1/pytest_mqtt.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     7910 2024-05-08 21:01:12.000000 pytest_mqtt-0.4.1/pytest_mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      367 2024-05-08 21:01:12.000000 pytest_mqtt-0.4.1/pytest_mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2024-05-08 21:01:12.000000 pytest_mqtt-0.4.1/pytest_mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       75 2024-05-08 21:01:12.000000 pytest_mqtt-0.4.1/pytest_mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      311 2024-05-08 21:01:12.000000 pytest_mqtt-0.4.1/pytest_mqtt.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       12 2024-05-08 21:01:12.000000 pytest_mqtt-0.4.1/pytest_mqtt.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)       38 2024-05-08 21:01:12.541119 pytest_mqtt-0.4.1/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)      210 2022-09-20 10:04:35.000000 pytest_mqtt-0.4.1/setup.py
```

### Comparing `pytest-mqtt-0.4.0/LICENSE` & `pytest_mqtt-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-mqtt-0.4.0/PKG-INFO` & `pytest_mqtt-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mqtt
-Version: 0.4.0
+Version: 0.4.1
 Summary: pytest-mqtt supports testing systems based on MQTT
 Author-email: Andreas Motl <andreas.motl@panodata.org>, Richard Pobering <richard.pobering@panodata.org>
 License: MIT
 Project-URL: homepage, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: documentation, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: repository, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: changelog, https://github.com/mqtt-tools/pytest-mqtt/blob/main/CHANGES.rst
@@ -48,15 +48,15 @@
 License-File: LICENSE
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: paho-mqtt<3
 Requires-Dist: pytest-docker-fixtures<2
 Provides-Extra: test
 Requires-Dist: coverage<8; extra == "test"
-Requires-Dist: pytest<8; extra == "test"
+Requires-Dist: pytest<9; extra == "test"
 Requires-Dist: pytest-fixture-order<1; extra == "test"
 Requires-Dist: pytest-ordering<1; extra == "test"
 Provides-Extra: develop
 Requires-Dist: isort<6; extra == "develop"
 Requires-Dist: black<25; extra == "develop"
 Requires-Dist: poethepoet<1; extra == "develop"
 Requires-Dist: ruff; extra == "develop"
```

### Comparing `pytest-mqtt-0.4.0/README.rst` & `pytest_mqtt-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-mqtt-0.4.0/pyproject.toml` & `pytest_mqtt-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Project definition
 # ==================
 
 # Derived from https://peps.python.org/pep-0621/
 
 [project]
 name = "pytest-mqtt"
-version = "0.4.0"
+version = "0.4.1"
 description = "pytest-mqtt supports testing systems based on MQTT"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {text = "MIT"}
 keywords = ["mqtt", "pytest", "testing", "mosquitto", "paho"]
 authors = [
   {name = "Andreas Motl", email = "andreas.motl@panodata.org"},
@@ -63,15 +63,15 @@
 [project.entry-points.pytest11]
 capmqtt = "pytest_mqtt.capmqtt"
 mosquitto = "pytest_mqtt.mosquitto"
 
 [project.optional-dependencies]
 test = [
   "coverage<8",
-  "pytest<8",
+  "pytest<9",
   "pytest-fixture-order<1",
   "pytest-ordering<1",
 ]
 develop = [
   "isort<6",
   "black<25",
   "poethepoet<1",
@@ -163,11 +163,11 @@
 test = [
   {cmd="coverage run -m pytest"},
   {cmd="coverage report"},
   {cmd="coverage xml"},
 ]
 
 release = [
-  #{cmd="minibump bump --relax minor"},
+  {cmd="minibump bump --relax patch"},
   {cmd="python -m build"},
   {cmd="twine upload --skip-existing dist/*.tar.gz dist/*.whl"},
 ]
```

### Comparing `pytest-mqtt-0.4.0/pytest_mqtt/capmqtt.py` & `pytest_mqtt-0.4.1/pytest_mqtt/capmqtt.py`

 * *Files identical despite different names*

### Comparing `pytest-mqtt-0.4.0/pytest_mqtt/mosquitto.py` & `pytest_mqtt-0.4.1/pytest_mqtt/mosquitto.py`

 * *Files 13% similar despite different names*

```diff
@@ -76,14 +76,27 @@
 mosquitto_image = Mosquitto()
 
 
 def is_mosquitto_running(host: str, port: int) -> bool:
     return probe_tcp_connect(host, port)
 
 
+def pytest_addoption(parser) -> None:
+    parser.addoption("--mqtt-host", action="store", type=str, default="localhost", help="MQTT host name")
+    parser.addoption("--mqtt-port", action="store", type=int, default=1883, help="MQTT port number")
+
+
+@pytest.fixture(scope="session")
+def mqtt_settings(pytestconfig) -> MqttSettings:
+    return MqttSettings(
+        host=pytestconfig.getoption("--mqtt-host"),
+        port=pytestconfig.getoption("--mqtt-port"),
+    )
+
+
 @pytest.fixture(scope="session")
 def mosquitto(mqtt_settings: MqttSettings):
 
     host, port = mqtt_settings.host, mqtt_settings.port
 
     # Gracefully skip spinning up the Docker container if Mosquitto is already running.
     if is_mosquitto_running(host, port):
```

### Comparing `pytest-mqtt-0.4.0/pytest_mqtt/util.py` & `pytest_mqtt-0.4.1/pytest_mqtt/util.py`

 * *Files identical despite different names*

### Comparing `pytest-mqtt-0.4.0/pytest_mqtt.egg-info/PKG-INFO` & `pytest_mqtt-0.4.1/pytest_mqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mqtt
-Version: 0.4.0
+Version: 0.4.1
 Summary: pytest-mqtt supports testing systems based on MQTT
 Author-email: Andreas Motl <andreas.motl@panodata.org>, Richard Pobering <richard.pobering@panodata.org>
 License: MIT
 Project-URL: homepage, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: documentation, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: repository, https://github.com/mqtt-tools/pytest-mqtt
 Project-URL: changelog, https://github.com/mqtt-tools/pytest-mqtt/blob/main/CHANGES.rst
@@ -48,15 +48,15 @@
 License-File: LICENSE
 Requires-Dist: dataclasses; python_version < "3.7"
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: paho-mqtt<3
 Requires-Dist: pytest-docker-fixtures<2
 Provides-Extra: test
 Requires-Dist: coverage<8; extra == "test"
-Requires-Dist: pytest<8; extra == "test"
+Requires-Dist: pytest<9; extra == "test"
 Requires-Dist: pytest-fixture-order<1; extra == "test"
 Requires-Dist: pytest-ordering<1; extra == "test"
 Provides-Extra: develop
 Requires-Dist: isort<6; extra == "develop"
 Requires-Dist: black<25; extra == "develop"
 Requires-Dist: poethepoet<1; extra == "develop"
 Requires-Dist: ruff; extra == "develop"
```


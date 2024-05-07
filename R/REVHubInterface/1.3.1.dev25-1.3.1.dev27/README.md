# Comparing `tmp/revhubinterface-1.3.1.dev25.tar.gz` & `tmp/revhubinterface-1.3.1.dev27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.1.dev25.tar", last modified: Tue May  7 20:23:06 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.1.dev27.tar", last modified: Tue May  7 20:27:52 2024, max compression
```

## Comparing `revhubinterface-1.3.1.dev25.tar` & `revhubinterface-1.3.1.dev27.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.753077 revhubinterface-1.3.1.dev25/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.757077 revhubinterface-1.3.1.dev25/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.757077 revhubinterface-1.3.1.dev25/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73547 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 20:23:06.000000 revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/flatpak/flatpak-pip-generator
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 20:23:02.000000 revhubinterface-1.3.1.dev25/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:23:06.761077 revhubinterface-1.3.1.dev25/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:27:52.490742 revhubinterface-1.3.1.dev27/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:27:52.482742 revhubinterface-1.3.1.dev27/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:27:52.486742 revhubinterface-1.3.1.dev27/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-07 20:27:52.490742 revhubinterface-1.3.1.dev27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:27:52.486742 revhubinterface-1.3.1.dev27/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73547 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:27:52.490742 revhubinterface-1.3.1.dev27/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-07 20:27:52.000000 revhubinterface-1.3.1.dev27/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-07 20:27:52.000000 revhubinterface-1.3.1.dev27/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:27:52.000000 revhubinterface-1.3.1.dev27/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 20:27:52.000000 revhubinterface-1.3.1.dev27/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 20:27:52.000000 revhubinterface-1.3.1.dev27/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 20:27:52.000000 revhubinterface-1.3.1.dev27/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:27:52.490742 revhubinterface-1.3.1.dev27/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/flatpak/flatpak-pip-generator
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 20:27:47.000000 revhubinterface-1.3.1.dev27/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 20:27:52.490742 revhubinterface-1.3.1.dev27/setup.cfg
```

### Comparing `revhubinterface-1.3.1.dev25/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.1.dev27/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/.github/workflows/python-publish.yml` & `revhubinterface-1.3.1.dev27/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/LICENSE.txt` & `revhubinterface-1.3.1.dev27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/PKG-INFO` & `revhubinterface-1.3.1.dev27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.1.dev25
-Summary: Manual control of REV Robotics Expansion Hub from a PC. Unofficial "community edition". 
+Version: 1.3.1.dev27
+Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
 
-# Rev Hardware Client (Community version)
+# Rev Hardware Client (Community Edition)
 
 The REV Hub Interface is a piece of software allowing for a direct connection from a REV Expansion Hub and its peripherals to a PC. 
 
 This interface provides a method for teams to prototype with motors, servos, and sensors in a way that is faster and easier than setting up an entire robot control system. It is also a valuable troubleshooting tool that can help isolate the cause of an issue and determine if it is electrical or software related. The REV Hub Firmware can also be updated and recovered through this interface in addition to the Robot Controller Application.
 
 This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows).
```

### Comparing `revhubinterface-1.3.1.dev25/README.md` & `revhubinterface-1.3.1.dev27/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Rev Hardware Client (Community version)
+# Rev Hardware Client (Community Edition)
 
 The REV Hub Interface is a piece of software allowing for a direct connection from a REV Expansion Hub and its peripherals to a PC. 
 
 This interface provides a method for teams to prototype with motors, servos, and sensors in a way that is faster and easier than setting up an entire robot control system. It is also a valuable troubleshooting tool that can help isolate the cause of an issue and determine if it is electrical or software related. The REV Hub Firmware can also be updated and recovered through this interface in addition to the Robot Controller Application.
 
 This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows).
```

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVADC.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVModule.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVServo.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface/__main__.py` & `revhubinterface-1.3.1.dev27/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.1.dev27/REVHubInterface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.1.dev25
-Summary: Manual control of REV Robotics Expansion Hub from a PC. Unofficial "community edition". 
+Version: 1.3.1.dev27
+Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
 
-# Rev Hardware Client (Community version)
+# Rev Hardware Client (Community Edition)
 
 The REV Hub Interface is a piece of software allowing for a direct connection from a REV Expansion Hub and its peripherals to a PC. 
 
 This interface provides a method for teams to prototype with motors, servos, and sensors in a way that is faster and easier than setting up an entire robot control system. It is also a valuable troubleshooting tool that can help isolate the cause of an issue and determine if it is electrical or software related. The REV Hub Firmware can also be updated and recovered through this interface in addition to the Robot Controller Application.
 
 This is a community continuation of the software, updating to newer underlying technologies (e.g. porting from Python 2 to Python 3), adding features, and porting to more platforms (Linux and macOS, in addition to Windows).
```

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.1.dev27/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/REVHubInterface.spec` & `revhubinterface-1.3.1.dev27/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.1.dev27/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.1.dev27/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/flatpak/python3-requirements.json` & `revhubinterface-1.3.1.dev27/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev25/pyproject.toml` & `revhubinterface-1.3.1.dev27/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>69", "setuptools-scm>8"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "REVHubInterface"
 dynamic = ["dependencies", "version"] # TODO make dynamic https://pypi.org/project/setuptools-scm/
-description = "Manual control of REV Robotics Expansion Hub from a PC. Unofficial \"community edition\". "
+description = "GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial \"Community Edition\". "
 readme = "README.md"
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 [tool.setuptools]
 packages = ["REVHubInterface"]
 [project.gui-scripts]
 revhubinterface = "REVHubInterface.__main__:initwindow"
```


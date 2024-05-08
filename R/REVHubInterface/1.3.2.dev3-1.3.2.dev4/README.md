# Comparing `tmp/revhubinterface-1.3.2.dev3.tar.gz` & `tmp/revhubinterface-1.3.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.2.dev3.tar", last modified: Tue May  7 23:37:50 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.2.dev4.tar", last modified: Tue May  7 23:38:53 2024, max compression
```

## Comparing `revhubinterface-1.3.2.dev3.tar` & `revhubinterface-1.3.2.dev4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.797992 revhubinterface-1.3.2.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.801992 revhubinterface-1.3.2.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.801992 revhubinterface-1.3.2.dev3/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface-mac.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/flatpak/flatpak-pip-generator
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.019075 revhubinterface-1.3.2.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.019075 revhubinterface-1.3.2.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface-mac.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-07 23:38:53.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/flatpak/flatpak-pip-generator
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/setup.cfg
```

### Comparing `revhubinterface-1.3.2.dev3/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.2.dev4/.github/workflows/pyinstaller.yml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     runs-on: macos-latest
     steps:
       - name: Create Executable
         uses: sayyid5416/pyinstaller@v1
         with:
           python_ver: '3.12'
           pyinstaller_ver: '==6.6.0'
-          spec: 'REVHubInterface.spec'
+          spec: 'REVHubInterface-mac.spec'
           requirements: 'requirements.txt'
           upload_exe_with_name: 'REVHubInterface Mac'
           options: --onefile, --name "REVHubInterface", --windowed,
   pyinstaller-build-win:
     runs-on: windows-latest
     steps:
       - name: Create Executable
```

### Comparing `revhubinterface-1.3.2.dev3/.github/workflows/python-publish.yml` & `revhubinterface-1.3.2.dev4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/LICENSE.txt` & `revhubinterface-1.3.2.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/PKG-INFO` & `revhubinterface-1.3.2.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.2.dev3
+Version: 1.3.2.dev4
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.2.dev3/README.md` & `revhubinterface-1.3.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVADC.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVModule.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVServo.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface/__main__.py` & `revhubinterface-1.3.2.dev4/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface-mac.spec` & `revhubinterface-1.3.2.dev4/REVHubInterface-mac.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.2.dev3
+Version: 1.3.2.dev4
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/REVHubInterface.spec` & `revhubinterface-1.3.2.dev4/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.2.dev4/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.2.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/flatpak/python3-requirements.json` & `revhubinterface-1.3.2.dev4/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev3/pyproject.toml` & `revhubinterface-1.3.2.dev4/pyproject.toml`

 * *Files identical despite different names*


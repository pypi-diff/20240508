# Comparing `tmp/revhubinterface-1.3.2.dev4.tar.gz` & `tmp/revhubinterface-1.3.2.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.2.dev4.tar", last modified: Tue May  7 23:38:53 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.2.dev5.tar", last modified: Wed May  8 01:46:36 2024, max compression
```

## Comparing `revhubinterface-1.3.2.dev4.tar` & `revhubinterface-1.3.2.dev5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.019075 revhubinterface-1.3.2.dev4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.019075 revhubinterface-1.3.2.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface-mac.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-07 23:38:53.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 23:38:52.000000 revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/flatpak/flatpak-pip-generator
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 23:38:48.000000 revhubinterface-1.3.2.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:38:53.023075 revhubinterface-1.3.2.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:46:36.958295 revhubinterface-1.3.2.dev5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:46:36.954295 revhubinterface-1.3.2.dev5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:46:36.954295 revhubinterface-1.3.2.dev5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 01:46:36.958295 revhubinterface-1.3.2.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:46:36.958295 revhubinterface-1.3.2.dev5/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface-mac.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:46:36.958295 revhubinterface-1.3.2.dev5/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-08 01:46:36.000000 revhubinterface-1.3.2.dev5/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 01:46:36.000000 revhubinterface-1.3.2.dev5/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:46:36.000000 revhubinterface-1.3.2.dev5/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 01:46:36.000000 revhubinterface-1.3.2.dev5/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 01:46:36.000000 revhubinterface-1.3.2.dev5/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 01:46:36.000000 revhubinterface-1.3.2.dev5/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:46:36.958295 revhubinterface-1.3.2.dev5/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/flatpak/flatpak-pip-generator
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 01:46:31.000000 revhubinterface-1.3.2.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:46:36.958295 revhubinterface-1.3.2.dev5/setup.cfg
```

### Comparing `revhubinterface-1.3.2.dev4/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.2.dev5/.github/workflows/pyinstaller.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,19 @@
         with:
           python_ver: '3.12'
           pyinstaller_ver: '==6.6.0'
           spec: 'REVHubInterface-mac.spec'
           requirements: 'requirements.txt'
           upload_exe_with_name: 'REVHubInterface Mac'
           options: --onefile, --name "REVHubInterface", --windowed,
+      - name: Make DMG
+        uses: QQxiaoming/create-dmg-action@v0.0.2
+        with:
+          name: 'REVHubInterface DMG'
+          srcdir: './dist'
   pyinstaller-build-win:
     runs-on: windows-latest
     steps:
       - name: Create Executable
         uses: sayyid5416/pyinstaller@v1
         with:
           python_ver: '3.12'
```

### Comparing `revhubinterface-1.3.2.dev4/.github/workflows/python-publish.yml` & `revhubinterface-1.3.2.dev5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/LICENSE.txt` & `revhubinterface-1.3.2.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/PKG-INFO` & `revhubinterface-1.3.2.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.2.dev4
+Version: 1.3.2.dev5
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.2.dev4/README.md` & `revhubinterface-1.3.2.dev5/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVADC.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVModule.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVServo.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface/__main__.py` & `revhubinterface-1.3.2.dev5/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface-mac.spec` & `revhubinterface-1.3.2.dev5/REVHubInterface-mac.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.2.dev5/REVHubInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.2.dev4
+Version: 1.3.2.dev5
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.2.dev5/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/REVHubInterface.spec` & `revhubinterface-1.3.2.dev5/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.2.dev5/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.2.dev5/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/flatpak/python3-requirements.json` & `revhubinterface-1.3.2.dev5/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.2.dev4/pyproject.toml` & `revhubinterface-1.3.2.dev5/pyproject.toml`

 * *Files identical despite different names*


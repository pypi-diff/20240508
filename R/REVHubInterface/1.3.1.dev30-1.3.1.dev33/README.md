# Comparing `tmp/revhubinterface-1.3.1.dev30.tar.gz` & `tmp/revhubinterface-1.3.1.dev33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.1.dev30.tar", last modified: Tue May  7 22:04:16 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.1.dev33.tar", last modified: Tue May  7 22:23:56 2024, max compression
```

## Comparing `revhubinterface-1.3.1.dev30.tar` & `revhubinterface-1.3.1.dev33.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:16.478302 revhubinterface-1.3.1.dev30/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:16.474302 revhubinterface-1.3.1.dev30/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:16.474302 revhubinterface-1.3.1.dev30/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-07 22:04:16.478302 revhubinterface-1.3.1.dev30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:16.478302 revhubinterface-1.3.1.dev30/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73736 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:16.478302 revhubinterface-1.3.1.dev30/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-07 22:04:16.000000 revhubinterface-1.3.1.dev30/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-07 22:04:16.000000 revhubinterface-1.3.1.dev30/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:04:16.000000 revhubinterface-1.3.1.dev30/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 22:04:16.000000 revhubinterface-1.3.1.dev30/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 22:04:16.000000 revhubinterface-1.3.1.dev30/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 22:04:16.000000 revhubinterface-1.3.1.dev30/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:16.478302 revhubinterface-1.3.1.dev30/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/flatpak/flatpak-pip-generator
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 22:04:11.000000 revhubinterface-1.3.1.dev30/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:04:16.478302 revhubinterface-1.3.1.dev30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.024170 revhubinterface-1.3.1.dev33/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.028170 revhubinterface-1.3.1.dev33/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.028170 revhubinterface-1.3.1.dev33/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/flatpak/flatpak-pip-generator
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/setup.cfg
```

### Comparing `revhubinterface-1.3.1.dev30/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.1.dev33/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/.github/workflows/python-publish.yml` & `revhubinterface-1.3.1.dev33/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/LICENSE.txt` & `revhubinterface-1.3.1.dev33/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/PKG-INFO` & `revhubinterface-1.3.1.dev33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.1.dev30
+Version: 1.3.1.dev33
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.1.dev30/README.md` & `revhubinterface-1.3.1.dev33/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVADC.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVModule.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVServo.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface/__main__.py` & `revhubinterface-1.3.1.dev33/REVHubInterface/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1416,22 +1416,21 @@
 
 
 def initwindow():
 
     mp.freeze_support()
 
     xroot = tk.Tk()
-    # Try to load nicer-looking interface on Linux if possible.  On Windows/macOS, the default Tk themes look reasonably-native.
-    if platform.system() != "Darwin" and platform.system() != "Windows":
-        try:
-            import sv_ttk
-            print('Loaded Tk theme: Sun Valley')
-            sv_ttk.set_theme("dark")
-        except:
-            pass
+    #attempt to import the theme, fallack to default if fails
+    try:
+        import sv_ttk
+        print('Loaded Tk theme: Sun Valley')
+        sv_ttk.set_theme("dark")
+    except:
+        pass
 
     xroot.title('REV Hub Interface - Community Edition - v1.3.1')
     try:
         xroot.iconbitmap('resource\\\\favicon.ico')
     except:
         try:
             xroot.iconbitmap('favicon.ico')
```

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.1.dev30
+Version: 1.3.1.dev33
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/REVHubInterface.spec` & `revhubinterface-1.3.1.dev33/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.1.dev33/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.1.dev33/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/flatpak/python3-requirements.json` & `revhubinterface-1.3.1.dev33/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev30/pyproject.toml` & `revhubinterface-1.3.1.dev33/pyproject.toml`

 * *Files identical despite different names*


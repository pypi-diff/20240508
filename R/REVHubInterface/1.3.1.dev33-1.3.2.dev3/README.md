# Comparing `tmp/revhubinterface-1.3.1.dev33.tar.gz` & `tmp/revhubinterface-1.3.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.1.dev33.tar", last modified: Tue May  7 22:23:56 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.2.dev3.tar", last modified: Tue May  7 23:37:50 2024, max compression
```

## Comparing `revhubinterface-1.3.1.dev33.tar` & `revhubinterface-1.3.2.dev3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.024170 revhubinterface-1.3.1.dev33/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.028170 revhubinterface-1.3.1.dev33/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.028170 revhubinterface-1.3.1.dev33/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 22:23:56.000000 revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/flatpak/flatpak-pip-generator
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 22:23:47.000000 revhubinterface-1.3.1.dev33/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:23:56.032170 revhubinterface-1.3.1.dev33/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.797992 revhubinterface-1.3.2.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.801992 revhubinterface-1.3.2.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.801992 revhubinterface-1.3.2.dev3/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73572 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface-mac.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 23:37:50.000000 revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/flatpak/flatpak-pip-generator
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 23:37:37.000000 revhubinterface-1.3.2.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:37:50.805992 revhubinterface-1.3.2.dev3/setup.cfg
```

### Comparing `revhubinterface-1.3.1.dev33/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.2.dev3/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/.github/workflows/python-publish.yml` & `revhubinterface-1.3.2.dev3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/LICENSE.txt` & `revhubinterface-1.3.2.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/PKG-INFO` & `revhubinterface-1.3.2.dev3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.1.dev33
+Version: 1.3.2.dev3
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
 
@@ -19,42 +19,60 @@
 ## Installing the software
 
 Start by downloading the latest version of the software from [the Releases page](https://github.com/unofficial-rev-port/REVHubInterface/releases).  An `.exe` is provided for Windows systems, a Flatpak for Linux systems (soon to be published on Flathub), and a `.DMG` for macOS.
 Alternately, you can download it from PyPi:
 
 1. Install Python 3
 2. Run `pip install REVHubInterface` to install
-3. Finally, run `python3 -m REVHubInterface` to run the app
+3. Finally, run `python3 -m REVHubInterface` to run the app (it should also be runnable as `revhubinterface`)
 
-Firmware updates require installing a driver.
+To avoid needing to run with root privileges on Ubuntu based platforms (and possibly other distributions) you need to add your user to the `dialout` group:
+
+1. Run ```sudo usermod `whoami` -a -G dialout```
+2. Reboot
+
+Firmware updates may require installing a driver.
+
+> [!WARNING]
+> Firmware update functionality has been ommited from the initial release.
+
+<details>
+  <summary>Driver installation</summary>
 
 - Windows: The newest versions of Windows should automatically install the required USB drivers. Alternatively, you can download the latest drivers from the [FTDI VCP website](https://www.ftdichip.com/Drivers/VCP.htm).
 - Linux: The latest `libftdi` is provided in the Flatpak.  If installing via PyPI instead, you will need to install `libftdi` yourself.  On Ubuntu and derivitaves, this can be installed with `sudo apt install libftdi1`.  The package name may be similar on other distributions.
-- macOS: (TODO: figure out; ~~`brew install libftdi` doesn't seem to make the error go away.~~ UPDATE: https://github.com/lsgunth/pyft232/pull/22 is merged but not yet published, in the mean time we should manually apply the change in our releases that have the library bundled.  Also, should we bundle `libftdi1.dylib` and its dependencies, or request users install it via Homebrew themselves?)
+- macOS: (TODO: figure out; `brew install libftdi` doesn't seem to make the error go away. UPDATE: https://github.com/lsgunth/pyft232/pull/22 is merged but not yet published, in the mean time we should manually apply the change in our releases that have the library bundled.  Also, should we bundle `libftdi1.dylib` and its dependencies, or request users install it via Homebrew themselves?
+
+</details>
 
 ## Connecting and Controlling an Expansion Hub
 
 1. Connect your Expansion Hub to the computer with a USB A to USB Mini-B cable.
 2. Run the REV Hub Interface Software.
 3. Press Connect.  The software will scan and connect to the Expansion Hub. The various peripheral tabs will populate with controls once connected.
 
 ## Running the development version
-If you want to run the development version from this repository rather than using a pre-packaged version, you will need to install a few additional dependencies:
+
+Early binaries are availiable from the Actions tab, or from the pre-releases section of https://pypi.org/project/REVHubInterface/#history.
+
+If you want to compile yourself rather than using a pre-packaged version, you will need to install a few additional dependencies:
 
 - Python 3
 - Tkinter
   - Windows: This is included in the Python 3 installer, just make sure sure it is selected to be installed at install time.
   - Linux: On Ubuntu and derivatives, this is instaled with `sudo apt install python3-tk`.  The package name will likely be similar on other distributions.
   - macOS: If using Homebrew, it can be install via `brew install python-tk`.
 - On Linux, you will need to install `libftdi`.  On Ubuntu and derivitaves, this can be installed with `sudo apt install libftdi1`.  The package name may be similar on other distributions.
 - The remaining Python dependencies (currently `pyft232` and `pyserial`, subject to future changes) can be installed via `pip3 install -r requirements.txt`
 - Finally, run `python3 REVHubInterface` while in the base folder of the repo.
 - Alternately, you can install onto your system from source using `pip install .` from the base folder of the repo, then using `python3 -m REVHubInterface` from anywhere.
 
 ## Compiling and publishing binaries
+<details>
+  <summary>Directions for developers</summary>
 
 ### PyPi
 PyPi builds *should* be automated by simply updating the trigger-actions branch, however, if you want to do it manually:
 
 1. Install build (`pip install build`) and twine (`pip install twine`)
 2. Create a Github release with a tag with the proper version number (if you want a dev release just skip this step; see https://packaging.python.org/en/latest/specifications/version-specifiers/ for proper version numbering)
 3. Run `python3 -m build `
@@ -69,7 +87,9 @@
 2. Run `pyinstaller REVHubInterface.spec`
 3. The binary should be available in the `dist` folder
 
 ### Flatpak
 Install Flatpak and flatpak-builder  
 TODO: finish this with Flathub directions
 
+</details>
+
```

### Comparing `revhubinterface-1.3.1.dev33/README.md` & `revhubinterface-1.3.2.dev3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,42 +9,60 @@
 ## Installing the software
 
 Start by downloading the latest version of the software from [the Releases page](https://github.com/unofficial-rev-port/REVHubInterface/releases).  An `.exe` is provided for Windows systems, a Flatpak for Linux systems (soon to be published on Flathub), and a `.DMG` for macOS.
 Alternately, you can download it from PyPi:
 
 1. Install Python 3
 2. Run `pip install REVHubInterface` to install
-3. Finally, run `python3 -m REVHubInterface` to run the app
+3. Finally, run `python3 -m REVHubInterface` to run the app (it should also be runnable as `revhubinterface`)
 
-Firmware updates require installing a driver.
+To avoid needing to run with root privileges on Ubuntu based platforms (and possibly other distributions) you need to add your user to the `dialout` group:
+
+1. Run ```sudo usermod `whoami` -a -G dialout```
+2. Reboot
+
+Firmware updates may require installing a driver.
+
+> [!WARNING]
+> Firmware update functionality has been ommited from the initial release.
+
+<details>
+  <summary>Driver installation</summary>
 
 - Windows: The newest versions of Windows should automatically install the required USB drivers. Alternatively, you can download the latest drivers from the [FTDI VCP website](https://www.ftdichip.com/Drivers/VCP.htm).
 - Linux: The latest `libftdi` is provided in the Flatpak.  If installing via PyPI instead, you will need to install `libftdi` yourself.  On Ubuntu and derivitaves, this can be installed with `sudo apt install libftdi1`.  The package name may be similar on other distributions.
-- macOS: (TODO: figure out; ~~`brew install libftdi` doesn't seem to make the error go away.~~ UPDATE: https://github.com/lsgunth/pyft232/pull/22 is merged but not yet published, in the mean time we should manually apply the change in our releases that have the library bundled.  Also, should we bundle `libftdi1.dylib` and its dependencies, or request users install it via Homebrew themselves?)
+- macOS: (TODO: figure out; `brew install libftdi` doesn't seem to make the error go away. UPDATE: https://github.com/lsgunth/pyft232/pull/22 is merged but not yet published, in the mean time we should manually apply the change in our releases that have the library bundled.  Also, should we bundle `libftdi1.dylib` and its dependencies, or request users install it via Homebrew themselves?
+
+</details>
 
 ## Connecting and Controlling an Expansion Hub
 
 1. Connect your Expansion Hub to the computer with a USB A to USB Mini-B cable.
 2. Run the REV Hub Interface Software.
 3. Press Connect.  The software will scan and connect to the Expansion Hub. The various peripheral tabs will populate with controls once connected.
 
 ## Running the development version
-If you want to run the development version from this repository rather than using a pre-packaged version, you will need to install a few additional dependencies:
+
+Early binaries are availiable from the Actions tab, or from the pre-releases section of https://pypi.org/project/REVHubInterface/#history.
+
+If you want to compile yourself rather than using a pre-packaged version, you will need to install a few additional dependencies:
 
 - Python 3
 - Tkinter
   - Windows: This is included in the Python 3 installer, just make sure sure it is selected to be installed at install time.
   - Linux: On Ubuntu and derivatives, this is instaled with `sudo apt install python3-tk`.  The package name will likely be similar on other distributions.
   - macOS: If using Homebrew, it can be install via `brew install python-tk`.
 - On Linux, you will need to install `libftdi`.  On Ubuntu and derivitaves, this can be installed with `sudo apt install libftdi1`.  The package name may be similar on other distributions.
 - The remaining Python dependencies (currently `pyft232` and `pyserial`, subject to future changes) can be installed via `pip3 install -r requirements.txt`
 - Finally, run `python3 REVHubInterface` while in the base folder of the repo.
 - Alternately, you can install onto your system from source using `pip install .` from the base folder of the repo, then using `python3 -m REVHubInterface` from anywhere.
 
 ## Compiling and publishing binaries
+<details>
+  <summary>Directions for developers</summary>
 
 ### PyPi
 PyPi builds *should* be automated by simply updating the trigger-actions branch, however, if you want to do it manually:
 
 1. Install build (`pip install build`) and twine (`pip install twine`)
 2. Create a Github release with a tag with the proper version number (if you want a dev release just skip this step; see https://packaging.python.org/en/latest/specifications/version-specifiers/ for proper version numbering)
 3. Run `python3 -m build `
@@ -59,7 +77,9 @@
 2. Run `pyinstaller REVHubInterface.spec`
 3. The binary should be available in the `dist` folder
 
 ### Flatpak
 Install Flatpak and flatpak-builder  
 TODO: finish this with Flathub directions
 
+</details>
+
```

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVADC.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVModule.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVServo.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface/__main__.py` & `revhubinterface-1.3.2.dev3/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.1.dev33
+Version: 1.3.2.dev3
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
 
@@ -19,42 +19,60 @@
 ## Installing the software
 
 Start by downloading the latest version of the software from [the Releases page](https://github.com/unofficial-rev-port/REVHubInterface/releases).  An `.exe` is provided for Windows systems, a Flatpak for Linux systems (soon to be published on Flathub), and a `.DMG` for macOS.
 Alternately, you can download it from PyPi:
 
 1. Install Python 3
 2. Run `pip install REVHubInterface` to install
-3. Finally, run `python3 -m REVHubInterface` to run the app
+3. Finally, run `python3 -m REVHubInterface` to run the app (it should also be runnable as `revhubinterface`)
 
-Firmware updates require installing a driver.
+To avoid needing to run with root privileges on Ubuntu based platforms (and possibly other distributions) you need to add your user to the `dialout` group:
+
+1. Run ```sudo usermod `whoami` -a -G dialout```
+2. Reboot
+
+Firmware updates may require installing a driver.
+
+> [!WARNING]
+> Firmware update functionality has been ommited from the initial release.
+
+<details>
+  <summary>Driver installation</summary>
 
 - Windows: The newest versions of Windows should automatically install the required USB drivers. Alternatively, you can download the latest drivers from the [FTDI VCP website](https://www.ftdichip.com/Drivers/VCP.htm).
 - Linux: The latest `libftdi` is provided in the Flatpak.  If installing via PyPI instead, you will need to install `libftdi` yourself.  On Ubuntu and derivitaves, this can be installed with `sudo apt install libftdi1`.  The package name may be similar on other distributions.
-- macOS: (TODO: figure out; ~~`brew install libftdi` doesn't seem to make the error go away.~~ UPDATE: https://github.com/lsgunth/pyft232/pull/22 is merged but not yet published, in the mean time we should manually apply the change in our releases that have the library bundled.  Also, should we bundle `libftdi1.dylib` and its dependencies, or request users install it via Homebrew themselves?)
+- macOS: (TODO: figure out; `brew install libftdi` doesn't seem to make the error go away. UPDATE: https://github.com/lsgunth/pyft232/pull/22 is merged but not yet published, in the mean time we should manually apply the change in our releases that have the library bundled.  Also, should we bundle `libftdi1.dylib` and its dependencies, or request users install it via Homebrew themselves?
+
+</details>
 
 ## Connecting and Controlling an Expansion Hub
 
 1. Connect your Expansion Hub to the computer with a USB A to USB Mini-B cable.
 2. Run the REV Hub Interface Software.
 3. Press Connect.  The software will scan and connect to the Expansion Hub. The various peripheral tabs will populate with controls once connected.
 
 ## Running the development version
-If you want to run the development version from this repository rather than using a pre-packaged version, you will need to install a few additional dependencies:
+
+Early binaries are availiable from the Actions tab, or from the pre-releases section of https://pypi.org/project/REVHubInterface/#history.
+
+If you want to compile yourself rather than using a pre-packaged version, you will need to install a few additional dependencies:
 
 - Python 3
 - Tkinter
   - Windows: This is included in the Python 3 installer, just make sure sure it is selected to be installed at install time.
   - Linux: On Ubuntu and derivatives, this is instaled with `sudo apt install python3-tk`.  The package name will likely be similar on other distributions.
   - macOS: If using Homebrew, it can be install via `brew install python-tk`.
 - On Linux, you will need to install `libftdi`.  On Ubuntu and derivitaves, this can be installed with `sudo apt install libftdi1`.  The package name may be similar on other distributions.
 - The remaining Python dependencies (currently `pyft232` and `pyserial`, subject to future changes) can be installed via `pip3 install -r requirements.txt`
 - Finally, run `python3 REVHubInterface` while in the base folder of the repo.
 - Alternately, you can install onto your system from source using `pip install .` from the base folder of the repo, then using `python3 -m REVHubInterface` from anywhere.
 
 ## Compiling and publishing binaries
+<details>
+  <summary>Directions for developers</summary>
 
 ### PyPi
 PyPi builds *should* be automated by simply updating the trigger-actions branch, however, if you want to do it manually:
 
 1. Install build (`pip install build`) and twine (`pip install twine`)
 2. Create a Github release with a tag with the proper version number (if you want a dev release just skip this step; see https://packaging.python.org/en/latest/specifications/version-specifiers/ for proper version numbering)
 3. Run `python3 -m build `
@@ -69,7 +87,9 @@
 2. Run `pyinstaller REVHubInterface.spec`
 3. The binary should be available in the `dist` folder
 
 ### Flatpak
 Install Flatpak and flatpak-builder  
 TODO: finish this with Flathub directions
 
+</details>
+
```

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.2.dev3/REVHubInterface.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 LICENSE.txt
 README.md
+REVHubInterface-mac.spec
 REVHubInterface.sh
 REVHubInterface.spec
 pyproject.toml
 requirements.txt
 .github/workflows/pyinstaller.yml
 .github/workflows/python-publish.yml
 REVHubInterface/REV2mSensor.py
```

### Comparing `revhubinterface-1.3.1.dev33/REVHubInterface.spec` & `revhubinterface-1.3.2.dev3/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.2.dev3/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.2.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/flatpak/python3-requirements.json` & `revhubinterface-1.3.2.dev3/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.1.dev33/pyproject.toml` & `revhubinterface-1.3.2.dev3/pyproject.toml`

 * *Files identical despite different names*


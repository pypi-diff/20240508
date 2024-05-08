# Comparing `tmp/pifcap-1.0.4.tar.gz` & `tmp/pifcap-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pifcap-1.0.4.tar", last modified: Thu May  2 12:51:06 2024, max compression
+gzip compressed data, was "pifcap-1.0.5.tar", last modified: Wed May  8 09:50:34 2024, max compression
```

## Comparing `pifcap-1.0.4.tar` & `pifcap-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-02 12:51:06.563800 pifcap-1.0.4/
--rw-r--r--   0 cam       (1000) cam       (1000)       26 2024-03-27 14:09:27.000000 pifcap-1.0.4/CHANGELOG
--rw-r--r--   0 cam       (1000) cam       (1000)     1068 2024-03-27 14:09:27.000000 pifcap-1.0.4/LICENSE
--rw-r--r--   0 cam       (1000) cam       (1000)     4762 2024-05-02 12:51:06.563800 pifcap-1.0.4/PKG-INFO
--rw-r--r--   0 cam       (1000) cam       (1000)     3317 2024-05-02 12:29:53.000000 pifcap-1.0.4/README.md
--rw-r--r--   0 cam       (1000) cam       (1000)       84 2024-03-27 14:09:27.000000 pifcap-1.0.4/pyproject.toml
--rw-r--r--   0 cam       (1000) cam       (1000)      723 2024-05-02 12:51:06.563800 pifcap-1.0.4/setup.cfg
--rw-r--r--   0 cam       (1000) cam       (1000)       45 2024-03-27 14:09:27.000000 pifcap-1.0.4/setup.py
-drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-02 12:51:06.555801 pifcap-1.0.4/src/
-drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-02 12:51:06.559800 pifcap-1.0.4/src/pifcap/
--rw-r--r--   0 cam       (1000) cam       (1000)        0 2024-04-28 13:45:36.000000 pifcap-1.0.4/src/pifcap/__init__.py
--rw-r--r--   0 cam       (1000) cam       (1000)     3804 2024-04-28 14:17:53.000000 pifcap-1.0.4/src/pifcap/autoexposure.py
--rw-r--r--   0 cam       (1000) cam       (1000)    24134 2024-04-28 14:17:53.000000 pifcap-1.0.4/src/pifcap/camera.py
--rw-r--r--   0 cam       (1000) cam       (1000)    16728 2024-04-28 14:44:04.000000 pifcap-1.0.4/src/pifcap/pifcap.py
--rw-r--r--   0 cam       (1000) cam       (1000)     8538 2024-04-21 09:54:15.000000 pifcap-1.0.4/src/pifcap/pifcap2fits.py
--rw-r--r--   0 cam       (1000) cam       (1000)      668 2024-04-05 13:43:54.000000 pifcap-1.0.4/src/pifcap/pifcap_image.py
--rw-r--r--   0 cam       (1000) cam       (1000)    18652 2024-04-14 12:33:51.000000 pifcap-1.0.4/src/pifcap/pifcap_ui.py
--rw-r--r--   0 cam       (1000) cam       (1000)     3803 2024-04-28 14:01:49.000000 pifcap-1.0.4/src/pifcap/settings.py
--rw-r--r--   0 cam       (1000) cam       (1000)     1690 2024-04-21 08:04:25.000000 pifcap-1.0.4/src/pifcap/settings_ui.py
-drwxr-xr-x   0 cam       (1000) cam       (1000)        0 2024-05-02 12:51:06.563800 pifcap-1.0.4/src/pifcap.egg-info/
--rw-r--r--   0 cam       (1000) cam       (1000)     4762 2024-05-02 12:51:06.000000 pifcap-1.0.4/src/pifcap.egg-info/PKG-INFO
--rw-r--r--   0 cam       (1000) cam       (1000)      485 2024-05-02 12:51:06.000000 pifcap-1.0.4/src/pifcap.egg-info/SOURCES.txt
--rw-r--r--   0 cam       (1000) cam       (1000)        1 2024-05-02 12:51:06.000000 pifcap-1.0.4/src/pifcap.egg-info/dependency_links.txt
--rw-r--r--   0 cam       (1000) cam       (1000)       99 2024-05-02 12:51:06.000000 pifcap-1.0.4/src/pifcap.egg-info/entry_points.txt
--rw-r--r--   0 cam       (1000) cam       (1000)       56 2024-05-02 12:51:06.000000 pifcap-1.0.4/src/pifcap.egg-info/requires.txt
--rw-r--r--   0 cam       (1000) cam       (1000)        7 2024-05-02 12:51:06.000000 pifcap-1.0.4/src/pifcap.egg-info/top_level.txt
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 09:50:34.536939 pifcap-1.0.5/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       64 2024-05-08 08:49:55.000000 pifcap-1.0.5/CHANGELOG
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1068 2024-05-03 06:52:46.000000 pifcap-1.0.5/LICENSE
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     5642 2024-05-08 09:50:34.536939 pifcap-1.0.5/PKG-INFO
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     4301 2024-05-08 09:50:04.000000 pifcap-1.0.5/README.md
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       84 2024-05-03 06:52:46.000000 pifcap-1.0.5/pyproject.toml
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      643 2024-05-08 09:50:34.540273 pifcap-1.0.5/setup.cfg
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       45 2024-05-03 06:52:46.000000 pifcap-1.0.5/setup.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 09:50:34.533606 pifcap-1.0.5/src/
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 09:50:34.536939 pifcap-1.0.5/src/pifcap/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)        0 2024-05-03 06:52:46.000000 pifcap-1.0.5/src/pifcap/__init__.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     3804 2024-05-03 06:52:46.000000 pifcap-1.0.5/src/pifcap/autoexposure.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    24134 2024-05-03 06:52:46.000000 pifcap-1.0.5/src/pifcap/camera.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    16728 2024-05-03 06:52:46.000000 pifcap-1.0.5/src/pifcap/pifcap.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     8538 2024-05-03 06:52:46.000000 pifcap-1.0.5/src/pifcap/pifcap2fits.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      668 2024-05-03 06:52:46.000000 pifcap-1.0.5/src/pifcap/pifcap_image.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    18652 2024-05-03 06:52:46.000000 pifcap-1.0.5/src/pifcap/pifcap_ui.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     3803 2024-05-03 06:52:46.000000 pifcap-1.0.5/src/pifcap/settings.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1690 2024-05-03 06:52:46.000000 pifcap-1.0.5/src/pifcap/settings_ui.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 09:50:34.536939 pifcap-1.0.5/src/pifcap.egg-info/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     5642 2024-05-08 09:50:34.000000 pifcap-1.0.5/src/pifcap.egg-info/PKG-INFO
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      452 2024-05-08 09:50:34.000000 pifcap-1.0.5/src/pifcap.egg-info/SOURCES.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)        1 2024-05-08 09:50:34.000000 pifcap-1.0.5/src/pifcap.egg-info/dependency_links.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       99 2024-05-08 09:50:34.000000 pifcap-1.0.5/src/pifcap.egg-info/entry_points.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)        7 2024-05-08 09:50:34.000000 pifcap-1.0.5/src/pifcap.egg-info/top_level.txt
```

### Comparing `pifcap-1.0.4/LICENSE` & `pifcap-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pifcap-1.0.4/PKG-INFO` & `pifcap-1.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: pifcap
-Version: 1.0.4
+Version: 1.0.5
 Summary: A GUI for fast RAW image capture on Raspberry Pi
 Home-page: https://github.com/scriptorron/pifcap
 Author: Ronald Schreiber
 Author-email: ronald.schreiber01@gmx.de
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.24
-Requires-Dist: astropy>=5.2
-Requires-Dist: picamera2>=0.3
-Requires-Dist: pyqtgraph>=0.13
 
 # pifcap - A GUI for fast RAW image capture on Raspberry Pi
 This software allows you to capture RAW images on Raspberry Pi in a fast way. Typical application is Lucky Imaging in astro photography.
 
 ***This software is still in development. It may not be functional. Please wait for the released version before you send issue reports.***
 
 ## Installation
 The software is made for raspberry Pi with a recent OS (Bullseye or Bookworm). 
 
-Some packages need to be installed with apt-get:
+Some packages need to be installed with `sudo apt`:
 - `libcamera` and `libcamera-apps` (if not already installed). You can test libcamera and the support
 for your camera with: 
   ```commandline
   libcamera-hello --list-cameras
   ```
   You must be able to make RAW pictures in all modes. For instance `libcamera-hello` shows for the HQ camera:
   ```
@@ -39,29 +35,52 @@
   ```commandline
   libcamera-still -r --mode 1332:990 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1080 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1520 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 4056:3040 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   ```
   Something with your libcamera or kernel driver installation will be wrong if this does not work.
-- The Python packages `PyQt5`, `picamera2` and `numpy` must be installed. Typically they are already installed. If not you can install them with:
+- Some Python packages require matching versions of system libraries. They must be installed with `sudo apt`:
 ```commandline
-sudo apt-get install python3-picamera2 python3-pyqt5 python3-numpy
+sudo apt install python3-pip libcamera-apps python3-picamera2 python3-pyqt5 python3-pyqtgraph python3-astropy python3-numpy python3-venv
 ```
 
-The Raspberry PI OS requires a virtual environment to install non-system Python packages. Trying to install `pifcap` without a virtual environment will fail with `error: externally-managed-environment`. 
+The Raspberry Pi OS "Bullseye" still allowed to install system wide with `sudo pip install pifcap`.
+Since "Bookworm" a virtual environment is required to install non-system Python packages. Trying to install
+`pifcap` without a virtual environment will fail with `error: externally-managed-environment`.
 
 Run the following on a command line to install `pifcap`in a virtual environment called `venv_pifcap`:
 ```commandline
 python3 -m venv --system-site-packages ~/venv_pifcap
 source ~/venv_pifcap/bin/activate
 pip install --upgrade pip
 pip install pifcap
 ```
 
+
+## Some hints when you get trouble
+The Python packages `picamera2`, `numpy`, and ` astropy` MUST be installed with `sudo apt install`.
+You MUST NOT update them with `pip`. When you get errors related to these packages you can:
+  1. Check directory `~/.local/lib/python3.9/site-packages` if it contains one of these packages. If yes delete them!
+  2. Check if `pip list` shows different version numbers than `apt list` for these packages:
+     ```commandline
+     pip list | grep numpy
+     apt list | grep numpy
+
+     pip list | grep astropy
+     apt list | grep astropy
+
+     pip list | grep picamera2
+     apt list | grep picamera2
+     ```
+     If you see different versions for a package remove it with `pip uninstall` and reinstall it with
+     `sudo apt reinstall`.
+  3. Remove and recreate the virtual environment.
+
+
 ## Uninstall
 To remove `pifcap` from your Pi just delete the virtual environment:
 ```commandline
 rm -rf ~/venv_pifcap
 ```
 
 ## Running
@@ -82,15 +101,18 @@
 pifcap2fits "*.pfc"
 ```
 Different to linux commands the file name specifier must be quoted!
 
 
 
 
-0.1.0
+1.0.5
+- fixed installation issues
+
+1.0.4
 initial release
 
 
 MIT License
 
 Copyright (c) 2024 scriptorron
```

### Comparing `pifcap-1.0.4/README.md` & `pifcap-1.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This software allows you to capture RAW images on Raspberry Pi in a fast way. Typical application is Lucky Imaging in astro photography.
 
 ***This software is still in development. It may not be functional. Please wait for the released version before you send issue reports.***
 
 ## Installation
 The software is made for raspberry Pi with a recent OS (Bullseye or Bookworm). 
 
-Some packages need to be installed with apt-get:
+Some packages need to be installed with `sudo apt`:
 - `libcamera` and `libcamera-apps` (if not already installed). You can test libcamera and the support
 for your camera with: 
   ```commandline
   libcamera-hello --list-cameras
   ```
   You must be able to make RAW pictures in all modes. For instance `libcamera-hello` shows for the HQ camera:
   ```
@@ -24,29 +24,52 @@
   ```commandline
   libcamera-still -r --mode 1332:990 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1080 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1520 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 4056:3040 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   ```
   Something with your libcamera or kernel driver installation will be wrong if this does not work.
-- The Python packages `PyQt5`, `picamera2` and `numpy` must be installed. Typically they are already installed. If not you can install them with:
+- Some Python packages require matching versions of system libraries. They must be installed with `sudo apt`:
 ```commandline
-sudo apt-get install python3-picamera2 python3-pyqt5 python3-numpy
+sudo apt install python3-pip libcamera-apps python3-picamera2 python3-pyqt5 python3-pyqtgraph python3-astropy python3-numpy python3-venv
 ```
 
-The Raspberry PI OS requires a virtual environment to install non-system Python packages. Trying to install `pifcap` without a virtual environment will fail with `error: externally-managed-environment`. 
+The Raspberry Pi OS "Bullseye" still allowed to install system wide with `sudo pip install pifcap`.
+Since "Bookworm" a virtual environment is required to install non-system Python packages. Trying to install
+`pifcap` without a virtual environment will fail with `error: externally-managed-environment`.
 
 Run the following on a command line to install `pifcap`in a virtual environment called `venv_pifcap`:
 ```commandline
 python3 -m venv --system-site-packages ~/venv_pifcap
 source ~/venv_pifcap/bin/activate
 pip install --upgrade pip
 pip install pifcap
 ```
 
+
+## Some hints when you get trouble
+The Python packages `picamera2`, `numpy`, and ` astropy` MUST be installed with `sudo apt install`.
+You MUST NOT update them with `pip`. When you get errors related to these packages you can:
+  1. Check directory `~/.local/lib/python3.9/site-packages` if it contains one of these packages. If yes delete them!
+  2. Check if `pip list` shows different version numbers than `apt list` for these packages:
+     ```commandline
+     pip list | grep numpy
+     apt list | grep numpy
+
+     pip list | grep astropy
+     apt list | grep astropy
+
+     pip list | grep picamera2
+     apt list | grep picamera2
+     ```
+     If you see different versions for a package remove it with `pip uninstall` and reinstall it with
+     `sudo apt reinstall`.
+  3. Remove and recreate the virtual environment.
+
+
 ## Uninstall
 To remove `pifcap` from your Pi just delete the virtual environment:
 ```commandline
 rm -rf ~/venv_pifcap
 ```
 
 ## Running
```

### Comparing `pifcap-1.0.4/setup.cfg` & `pifcap-1.0.5/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 [metadata]
 name = pifcap
-version = 1.0.4
+version = 1.0.5
 author = Ronald Schreiber
 author_email = ronald.schreiber01@gmx.de
 description = A GUI for fast RAW image capture on Raspberry Pi
 long_description = file: README.md, CHANGELOG, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/scriptorron/pifcap
 license_files = LICENSE
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 python_requires = >=3.7
-install_requires = 
-	numpy>=1.24
-	astropy>=5.2
-	picamera2>=0.3
-	pyqtgraph>=0.13
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 gui_scripts = 
 	pifcap = pifcap.pifcap:main
```

### Comparing `pifcap-1.0.4/src/pifcap/autoexposure.py` & `pifcap-1.0.5/src/pifcap/autoexposure.py`

 * *Files identical despite different names*

### Comparing `pifcap-1.0.4/src/pifcap/camera.py` & `pifcap-1.0.5/src/pifcap/camera.py`

 * *Files identical despite different names*

### Comparing `pifcap-1.0.4/src/pifcap/pifcap.py` & `pifcap-1.0.5/src/pifcap/pifcap.py`

 * *Files identical despite different names*

### Comparing `pifcap-1.0.4/src/pifcap/pifcap2fits.py` & `pifcap-1.0.5/src/pifcap/pifcap2fits.py`

 * *Files identical despite different names*

### Comparing `pifcap-1.0.4/src/pifcap/pifcap_image.py` & `pifcap-1.0.5/src/pifcap/pifcap_image.py`

 * *Files identical despite different names*

### Comparing `pifcap-1.0.4/src/pifcap/pifcap_ui.py` & `pifcap-1.0.5/src/pifcap/pifcap_ui.py`

 * *Files identical despite different names*

### Comparing `pifcap-1.0.4/src/pifcap/settings.py` & `pifcap-1.0.5/src/pifcap/settings.py`

 * *Files identical despite different names*

### Comparing `pifcap-1.0.4/src/pifcap/settings_ui.py` & `pifcap-1.0.5/src/pifcap/settings_ui.py`

 * *Files identical despite different names*

### Comparing `pifcap-1.0.4/src/pifcap.egg-info/PKG-INFO` & `pifcap-1.0.5/src/pifcap.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: pifcap
-Version: 1.0.4
+Version: 1.0.5
 Summary: A GUI for fast RAW image capture on Raspberry Pi
 Home-page: https://github.com/scriptorron/pifcap
 Author: Ronald Schreiber
 Author-email: ronald.schreiber01@gmx.de
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.24
-Requires-Dist: astropy>=5.2
-Requires-Dist: picamera2>=0.3
-Requires-Dist: pyqtgraph>=0.13
 
 # pifcap - A GUI for fast RAW image capture on Raspberry Pi
 This software allows you to capture RAW images on Raspberry Pi in a fast way. Typical application is Lucky Imaging in astro photography.
 
 ***This software is still in development. It may not be functional. Please wait for the released version before you send issue reports.***
 
 ## Installation
 The software is made for raspberry Pi with a recent OS (Bullseye or Bookworm). 
 
-Some packages need to be installed with apt-get:
+Some packages need to be installed with `sudo apt`:
 - `libcamera` and `libcamera-apps` (if not already installed). You can test libcamera and the support
 for your camera with: 
   ```commandline
   libcamera-hello --list-cameras
   ```
   You must be able to make RAW pictures in all modes. For instance `libcamera-hello` shows for the HQ camera:
   ```
@@ -39,29 +35,52 @@
   ```commandline
   libcamera-still -r --mode 1332:990 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1080 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1520 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 4056:3040 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   ```
   Something with your libcamera or kernel driver installation will be wrong if this does not work.
-- The Python packages `PyQt5`, `picamera2` and `numpy` must be installed. Typically they are already installed. If not you can install them with:
+- Some Python packages require matching versions of system libraries. They must be installed with `sudo apt`:
 ```commandline
-sudo apt-get install python3-picamera2 python3-pyqt5 python3-numpy
+sudo apt install python3-pip libcamera-apps python3-picamera2 python3-pyqt5 python3-pyqtgraph python3-astropy python3-numpy python3-venv
 ```
 
-The Raspberry PI OS requires a virtual environment to install non-system Python packages. Trying to install `pifcap` without a virtual environment will fail with `error: externally-managed-environment`. 
+The Raspberry Pi OS "Bullseye" still allowed to install system wide with `sudo pip install pifcap`.
+Since "Bookworm" a virtual environment is required to install non-system Python packages. Trying to install
+`pifcap` without a virtual environment will fail with `error: externally-managed-environment`.
 
 Run the following on a command line to install `pifcap`in a virtual environment called `venv_pifcap`:
 ```commandline
 python3 -m venv --system-site-packages ~/venv_pifcap
 source ~/venv_pifcap/bin/activate
 pip install --upgrade pip
 pip install pifcap
 ```
 
+
+## Some hints when you get trouble
+The Python packages `picamera2`, `numpy`, and ` astropy` MUST be installed with `sudo apt install`.
+You MUST NOT update them with `pip`. When you get errors related to these packages you can:
+  1. Check directory `~/.local/lib/python3.9/site-packages` if it contains one of these packages. If yes delete them!
+  2. Check if `pip list` shows different version numbers than `apt list` for these packages:
+     ```commandline
+     pip list | grep numpy
+     apt list | grep numpy
+
+     pip list | grep astropy
+     apt list | grep astropy
+
+     pip list | grep picamera2
+     apt list | grep picamera2
+     ```
+     If you see different versions for a package remove it with `pip uninstall` and reinstall it with
+     `sudo apt reinstall`.
+  3. Remove and recreate the virtual environment.
+
+
 ## Uninstall
 To remove `pifcap` from your Pi just delete the virtual environment:
 ```commandline
 rm -rf ~/venv_pifcap
 ```
 
 ## Running
@@ -82,15 +101,18 @@
 pifcap2fits "*.pfc"
 ```
 Different to linux commands the file name specifier must be quoted!
 
 
 
 
-0.1.0
+1.0.5
+- fixed installation issues
+
+1.0.4
 initial release
 
 
 MIT License
 
 Copyright (c) 2024 scriptorron
```


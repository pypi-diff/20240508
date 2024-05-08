# Comparing `tmp/indi_pylibcamera-2.6.2.tar.gz` & `tmp/indi_pylibcamera-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indi_pylibcamera-2.6.2.tar", last modified: Fri May  3 11:56:20 2024, max compression
+gzip compressed data, was "indi_pylibcamera-2.6.3.tar", last modified: Wed May  8 08:10:33 2024, max compression
```

## Comparing `indi_pylibcamera-2.6.2.tar` & `indi_pylibcamera-2.6.3.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:56:20.931551 indi_pylibcamera-2.6.2/
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2388 2024-05-03 11:38:08.000000 indi_pylibcamera-2.6.2/CHANGELOG
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1074 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/LICENSE
--rw-r--r--   0 sbr       (1000) sbr       (1000)      187 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/MANIFEST.in
--rw-r--r--   0 sbr       (1000) sbr       (1000)    22119 2024-05-03 11:56:20.931551 indi_pylibcamera-2.6.2/PKG-INFO
--rw-r--r--   0 sbr       (1000) sbr       (1000)    18228 2024-05-03 11:36:48.000000 indi_pylibcamera-2.6.2/README.md
--rw-r--r--   0 sbr       (1000) sbr       (1000)       81 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/pyproject.toml
--rw-r--r--   0 sbr       (1000) sbr       (1000)      920 2024-05-03 11:56:20.931551 indi_pylibcamera-2.6.2/setup.cfg
--rw-r--r--   0 sbr       (1000) sbr       (1000)       40 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/setup.py
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:56:20.924884 indi_pylibcamera-2.6.2/src/
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:56:20.928218 indi_pylibcamera-2.6.2/src/indi_pylibcamera/
--rw-r--r--   0 sbr       (1000) sbr       (1000)    48830 2024-04-21 18:26:02.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraControl.py
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:56:20.931551 indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1397 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1903 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/IMX290.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2074 2024-02-23 15:06:38.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2654 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1960 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2621 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)     3244 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/SnoopingManager.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)       75 2024-05-03 11:37:23.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/__init__.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2472 2024-02-27 18:59:44.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/indi_pylibcamera.ini
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)    60404 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/indi_pylibcamera.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)      216 2024-05-03 11:37:23.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/indi_pylibcamera.xml
--rw-r--r--   0 sbr       (1000) sbr       (1000)     2825 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/indi_pylibcamera_postinstall.py
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)    28758 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/indidevice.py
--rw-r--r--   0 sbr       (1000) sbr       (1000)      902 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/make_driver_xml.py
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)     1944 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/print_camera_information.py
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:56:20.931551 indi_pylibcamera-2.6.2/src/indi_pylibcamera/testpattern/
--rwxr-xr-x   0 sbr       (1000) sbr       (1000)    19253 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera/testpattern/RBG_testpattern.png
-drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-03 11:56:20.931551 indi_pylibcamera-2.6.2/src/indi_pylibcamera.egg-info/
--rw-r--r--   0 sbr       (1000) sbr       (1000)    22119 2024-05-03 11:56:20.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera.egg-info/PKG-INFO
--rw-r--r--   0 sbr       (1000) sbr       (1000)     1134 2024-05-03 11:56:20.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera.egg-info/SOURCES.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)        1 2024-05-03 11:56:20.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera.egg-info/dependency_links.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)      249 2024-05-03 11:56:20.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera.egg-info/entry_points.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)       40 2024-05-03 11:56:20.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera.egg-info/requires.txt
--rw-r--r--   0 sbr       (1000) sbr       (1000)       17 2024-05-03 11:56:20.000000 indi_pylibcamera-2.6.2/src/indi_pylibcamera.egg-info/top_level.txt
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2423 2024-05-08 07:52:04.000000 indi_pylibcamera-2.6.3/CHANGELOG
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1074 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/LICENSE
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      187 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/MANIFEST.in
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    23165 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/PKG-INFO
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    19324 2024-05-08 08:08:34.000000 indi_pylibcamera-2.6.3/README.md
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       81 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/pyproject.toml
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      857 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/setup.cfg
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       40 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/setup.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.049916 indi_pylibcamera-2.6.3/src/
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.053250 indi_pylibcamera-2.6.3/src/indi_pylibcamera/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    48830 2024-04-21 18:26:02.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraControl.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1397 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1903 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/IMX290.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2074 2024-02-23 15:06:38.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2654 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1960 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2621 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     3244 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/SnoopingManager.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       75 2024-05-08 07:49:47.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/__init__.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2472 2024-02-27 18:59:44.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.ini
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)    60404 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      216 2024-05-08 07:49:47.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.xml
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     2825 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera_postinstall.py
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)    28758 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/indidevice.py
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      902 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/make_driver_xml.py
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)     1944 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/print_camera_information.py
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/src/indi_pylibcamera/testpattern/
+-rwxr-xr-x   0 sbr       (1000) sbr       (1000)    19253 2024-01-14 16:09:36.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera/testpattern/RBG_testpattern.png
+drwxr-xr-x   0 sbr       (1000) sbr       (1000)        0 2024-05-08 08:10:33.056583 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/
+-rw-r--r--   0 sbr       (1000) sbr       (1000)    23165 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/PKG-INFO
+-rw-r--r--   0 sbr       (1000) sbr       (1000)     1091 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/SOURCES.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)        1 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/dependency_links.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)      249 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/entry_points.txt
+-rw-r--r--   0 sbr       (1000) sbr       (1000)       17 2024-05-08 08:10:33.000000 indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/top_level.txt
```

### Comparing `indi_pylibcamera-2.6.2/CHANGELOG` & `indi_pylibcamera-2.6.3/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2.6.3
+- fixed installation issues
+
 2.6.2
 - fixed ROWORDER attribute in FITS files (KStars/EKOS ignores this but some postprocessing tools need this fix to
   have the Bayer pattern in the correct order)
 - more details in install_requires of the wheel
 - adapted install instructions in README.md to meet newer OS versions (installation in virtual environment)
 - removed indi_pylibcamera_postinstall from installation: does not work from virtual environment
```

### Comparing `indi_pylibcamera-2.6.2/LICENSE` & `indi_pylibcamera-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/PKG-INFO` & `indi_pylibcamera-2.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: indi_pylibcamera
-Version: 2.6.2
+Version: 2.6.3
 Summary: An INDI driver for Raspberry Pi cameras supported by libcamera
 Home-page: https://github.com/scriptorron/indi_pylibcamera
 Author: Ronald Schreiber
 Author-email: ronald.schreiber01@gmx.de
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.24
-Requires-Dist: astropy>=5.2
-Requires-Dist: picamera2>=0.3
 
 # indi_pylibcamera
 This project implements a Raspberry Pi camera driver for INDI (https://indilib.org/). 
 
 Raspberry Pi cameras allow the amateur astronomer to make astonishing pictures with small budget. Especially the
 Raspberry Pi HQ camera can compete with expensive astro cameras.
 
@@ -36,15 +33,15 @@
                         --> kernel driver
 ```
 It can not work when the versions of `libcamera` and `picamera2` are too old (both are in a dynamic development).
 And it can not work when the libcamera-tools (like `libcamera-hello` and `libcamera-still`) have issues with your
 camera.
 
 ## Requirements and installation
-Some packages need to be installed with apt-get:
+Some packages need to be installed with `apt`:
 - `libcamera` and `libcamera-apps` (if not already installed). You can test libcamera and the support
 for your camera with: 
   ```commandline
   libcamera-hello --list-cameras
   ```
   You must be able to make RAW pictures in all modes. For instance `libcamera-hello` shows for the HQ camera:
   ```
@@ -59,34 +56,55 @@
   libcamera-still -r --mode 1332:990 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1080 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1520 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 4056:3040 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   ```
   Something with your libcamera or kernel driver installation will be wrong if this does not work.
 - Install INDI core library. If there is no pre-compiled package for your hardware you will need to compile it
-by yourself. Instructions can be found here: https://github.com/indilib/indi. A Raspberry Pi Zero does not
-have enough RAM to compile with 4 threads in parallel: you need to do `make -j1` instead of `make -j4`. 
+by yourself. Instructions can be found here: https://github.com/indilib/indi. 
+The scripts on https://gitea.nouspiro.space/nou/astro-soft-build automate compilation and installation.
+  A Raspberry Pi Zero does not have enough RAM to compile with 4 threads in parallel: you need to do `make -j1` instead of `make -j4`. 
 Finally, after installation, you need to have a working INDI server: `indiserver -v indi_simulator_telescope`
-- The Python packages `PyQt5`, `picamera2` and `numpy` must be installed with `apt-get`. Typically they are already
-installed. If not you can install them with:
+- Some Python packages require matching versions of system libraries. They must be installed with `apt`:
 ```commandline
-sudo apt-get install python3-picamera2 python3-pyqt5 python3-numpy
+sudo apt install python3-pip libcamera-apps python3-picamera2 python3-lxml python3-astropy python3-numpy python3-venv
 ```
 
-The Raspberry PI OS requires a virtual environment to install non-system Python packages. Trying to install
+The Raspberry Pi OS "Bullseye" still allowed to install system wide with `sudo pip install indi_pylibcamera`. 
+Since "Bookworm" a virtual environment is required to install non-system Python packages. Trying to install
 `indi_pylibcamera` without a virtual environment will fail with `error: externally-managed-environment`. 
 
-Run the following on a command line to install `indi_pylibcamera`in a virtual environment called `venv_indi_pylibcamera`:
+Run the following on a command line to install `indi_pylibcamera`in a virtual environment called `venv_indi_pylibcamera`
+(you can name the virtual environment as you want):
 ```commandline
 python3 -m venv --system-site-packages ~/venv_indi_pylibcamera
 source ~/venv_indi_pylibcamera/bin/activate
 pip install --upgrade pip
 pip install indi_pylibcamera
 ```
 
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
 ## Uninstall
 For uninstalling the driver do:
 ```commandline
 sudo rm -f /usr/share/indi/indi_pylibcamera.xml
 rm -rf ~/venv_indi_pylibcamera
 ```
 
@@ -333,14 +351,17 @@
 - Simon Šander
 - Aaron W Morris
 - Caden Gobat
 - anjok
 
 I hope I did not forget someone. If so please do not be angry and tell me.
 
+2.6.3
+- fixed installation issues
+
 2.6.2
 - fixed ROWORDER attribute in FITS files (KStars/EKOS ignores this but some postprocessing tools need this fix to
   have the Bayer pattern in the correct order)
 - more details in install_requires of the wheel
 - adapted install instructions in README.md to meet newer OS versions (installation in virtual environment)
 - removed indi_pylibcamera_postinstall from installation: does not work from virtual environment
```

### Comparing `indi_pylibcamera-2.6.2/README.md` & `indi_pylibcamera-2.6.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                         --> kernel driver
 ```
 It can not work when the versions of `libcamera` and `picamera2` are too old (both are in a dynamic development).
 And it can not work when the libcamera-tools (like `libcamera-hello` and `libcamera-still`) have issues with your
 camera.
 
 ## Requirements and installation
-Some packages need to be installed with apt-get:
+Some packages need to be installed with `apt`:
 - `libcamera` and `libcamera-apps` (if not already installed). You can test libcamera and the support
 for your camera with: 
   ```commandline
   libcamera-hello --list-cameras
   ```
   You must be able to make RAW pictures in all modes. For instance `libcamera-hello` shows for the HQ camera:
   ```
@@ -45,34 +45,55 @@
   libcamera-still -r --mode 1332:990 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1080 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1520 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 4056:3040 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   ```
   Something with your libcamera or kernel driver installation will be wrong if this does not work.
 - Install INDI core library. If there is no pre-compiled package for your hardware you will need to compile it
-by yourself. Instructions can be found here: https://github.com/indilib/indi. A Raspberry Pi Zero does not
-have enough RAM to compile with 4 threads in parallel: you need to do `make -j1` instead of `make -j4`. 
+by yourself. Instructions can be found here: https://github.com/indilib/indi. 
+The scripts on https://gitea.nouspiro.space/nou/astro-soft-build automate compilation and installation.
+  A Raspberry Pi Zero does not have enough RAM to compile with 4 threads in parallel: you need to do `make -j1` instead of `make -j4`. 
 Finally, after installation, you need to have a working INDI server: `indiserver -v indi_simulator_telescope`
-- The Python packages `PyQt5`, `picamera2` and `numpy` must be installed with `apt-get`. Typically they are already
-installed. If not you can install them with:
+- Some Python packages require matching versions of system libraries. They must be installed with `apt`:
 ```commandline
-sudo apt-get install python3-picamera2 python3-pyqt5 python3-numpy
+sudo apt install python3-pip libcamera-apps python3-picamera2 python3-lxml python3-astropy python3-numpy python3-venv
 ```
 
-The Raspberry PI OS requires a virtual environment to install non-system Python packages. Trying to install
+The Raspberry Pi OS "Bullseye" still allowed to install system wide with `sudo pip install indi_pylibcamera`. 
+Since "Bookworm" a virtual environment is required to install non-system Python packages. Trying to install
 `indi_pylibcamera` without a virtual environment will fail with `error: externally-managed-environment`. 
 
-Run the following on a command line to install `indi_pylibcamera`in a virtual environment called `venv_indi_pylibcamera`:
+Run the following on a command line to install `indi_pylibcamera`in a virtual environment called `venv_indi_pylibcamera`
+(you can name the virtual environment as you want):
 ```commandline
 python3 -m venv --system-site-packages ~/venv_indi_pylibcamera
 source ~/venv_indi_pylibcamera/bin/activate
 pip install --upgrade pip
 pip install indi_pylibcamera
 ```
 
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
 ## Uninstall
 For uninstalling the driver do:
 ```commandline
 sudo rm -f /usr/share/indi/indi_pylibcamera.xml
 rm -rf ~/venv_indi_pylibcamera
 ```
```

### Comparing `indi_pylibcamera-2.6.2/setup.cfg` & `indi_pylibcamera-2.6.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 
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
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	indi_pylibcamera = indi_pylibcamera.indi_pylibcamera:main
```

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraControl.py` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraControl.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/IMX290.txt` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/IMX290.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/SnoopingManager.py` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/SnoopingManager.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/indi_pylibcamera.ini` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.ini`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/indi_pylibcamera.py` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/indi_pylibcamera_postinstall.py` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/indi_pylibcamera_postinstall.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/indidevice.py` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/indidevice.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/make_driver_xml.py` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/make_driver_xml.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/print_camera_information.py` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/print_camera_information.py`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera/testpattern/RBG_testpattern.png` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera/testpattern/RBG_testpattern.png`

 * *Files identical despite different names*

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera.egg-info/PKG-INFO` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: indi_pylibcamera
-Version: 2.6.2
+Version: 2.6.3
 Summary: An INDI driver for Raspberry Pi cameras supported by libcamera
 Home-page: https://github.com/scriptorron/indi_pylibcamera
 Author: Ronald Schreiber
 Author-email: ronald.schreiber01@gmx.de
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.24
-Requires-Dist: astropy>=5.2
-Requires-Dist: picamera2>=0.3
 
 # indi_pylibcamera
 This project implements a Raspberry Pi camera driver for INDI (https://indilib.org/). 
 
 Raspberry Pi cameras allow the amateur astronomer to make astonishing pictures with small budget. Especially the
 Raspberry Pi HQ camera can compete with expensive astro cameras.
 
@@ -36,15 +33,15 @@
                         --> kernel driver
 ```
 It can not work when the versions of `libcamera` and `picamera2` are too old (both are in a dynamic development).
 And it can not work when the libcamera-tools (like `libcamera-hello` and `libcamera-still`) have issues with your
 camera.
 
 ## Requirements and installation
-Some packages need to be installed with apt-get:
+Some packages need to be installed with `apt`:
 - `libcamera` and `libcamera-apps` (if not already installed). You can test libcamera and the support
 for your camera with: 
   ```commandline
   libcamera-hello --list-cameras
   ```
   You must be able to make RAW pictures in all modes. For instance `libcamera-hello` shows for the HQ camera:
   ```
@@ -59,34 +56,55 @@
   libcamera-still -r --mode 1332:990 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1080 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 2028:1520 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   libcamera-still -r --mode 4056:3040 --shutter 100000 --gain 1 --awbgains 1,1 --immediate -o test.jpg
   ```
   Something with your libcamera or kernel driver installation will be wrong if this does not work.
 - Install INDI core library. If there is no pre-compiled package for your hardware you will need to compile it
-by yourself. Instructions can be found here: https://github.com/indilib/indi. A Raspberry Pi Zero does not
-have enough RAM to compile with 4 threads in parallel: you need to do `make -j1` instead of `make -j4`. 
+by yourself. Instructions can be found here: https://github.com/indilib/indi. 
+The scripts on https://gitea.nouspiro.space/nou/astro-soft-build automate compilation and installation.
+  A Raspberry Pi Zero does not have enough RAM to compile with 4 threads in parallel: you need to do `make -j1` instead of `make -j4`. 
 Finally, after installation, you need to have a working INDI server: `indiserver -v indi_simulator_telescope`
-- The Python packages `PyQt5`, `picamera2` and `numpy` must be installed with `apt-get`. Typically they are already
-installed. If not you can install them with:
+- Some Python packages require matching versions of system libraries. They must be installed with `apt`:
 ```commandline
-sudo apt-get install python3-picamera2 python3-pyqt5 python3-numpy
+sudo apt install python3-pip libcamera-apps python3-picamera2 python3-lxml python3-astropy python3-numpy python3-venv
 ```
 
-The Raspberry PI OS requires a virtual environment to install non-system Python packages. Trying to install
+The Raspberry Pi OS "Bullseye" still allowed to install system wide with `sudo pip install indi_pylibcamera`. 
+Since "Bookworm" a virtual environment is required to install non-system Python packages. Trying to install
 `indi_pylibcamera` without a virtual environment will fail with `error: externally-managed-environment`. 
 
-Run the following on a command line to install `indi_pylibcamera`in a virtual environment called `venv_indi_pylibcamera`:
+Run the following on a command line to install `indi_pylibcamera`in a virtual environment called `venv_indi_pylibcamera`
+(you can name the virtual environment as you want):
 ```commandline
 python3 -m venv --system-site-packages ~/venv_indi_pylibcamera
 source ~/venv_indi_pylibcamera/bin/activate
 pip install --upgrade pip
 pip install indi_pylibcamera
 ```
 
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
 ## Uninstall
 For uninstalling the driver do:
 ```commandline
 sudo rm -f /usr/share/indi/indi_pylibcamera.xml
 rm -rf ~/venv_indi_pylibcamera
 ```
 
@@ -333,14 +351,17 @@
 - Simon Šander
 - Aaron W Morris
 - Caden Gobat
 - anjok
 
 I hope I did not forget someone. If so please do not be angry and tell me.
 
+2.6.3
+- fixed installation issues
+
 2.6.2
 - fixed ROWORDER attribute in FITS files (KStars/EKOS ignores this but some postprocessing tools need this fix to
   have the Bayer pattern in the correct order)
 - more details in install_requires of the wheel
 - adapted install instructions in README.md to meet newer OS versions (installation in virtual environment)
 - removed indi_pylibcamera_postinstall from installation: does not work from virtual environment
```

### Comparing `indi_pylibcamera-2.6.2/src/indi_pylibcamera.egg-info/SOURCES.txt` & `indi_pylibcamera-2.6.3/src/indi_pylibcamera.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 src/indi_pylibcamera/indidevice.py
 src/indi_pylibcamera/make_driver_xml.py
 src/indi_pylibcamera/print_camera_information.py
 src/indi_pylibcamera.egg-info/PKG-INFO
 src/indi_pylibcamera.egg-info/SOURCES.txt
 src/indi_pylibcamera.egg-info/dependency_links.txt
 src/indi_pylibcamera.egg-info/entry_points.txt
-src/indi_pylibcamera.egg-info/requires.txt
 src/indi_pylibcamera.egg-info/top_level.txt
 src/indi_pylibcamera/CameraInfos/Arducam_Pivariety_IMX462.txt
 src/indi_pylibcamera/CameraInfos/IMX290.txt
 src/indi_pylibcamera/CameraInfos/Raspi_GlobalShutter_IMX296.txt
 src/indi_pylibcamera/CameraInfos/Raspi_HQ_IMX477.txt
 src/indi_pylibcamera/CameraInfos/Raspi_M3_IMX708.txt
 src/indi_pylibcamera/CameraInfos/Raspi_V1_OV5647.txt
```


# Comparing `tmp/DFRobotUPS-0.4.5.tar.gz` & `tmp/DFRobotUPS-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DFRobotUPS-0.4.5.tar", last modified: Mon May  6 11:13:59 2024, max compression
+gzip compressed data, was "DFRobotUPS-0.4.6.tar", last modified: Wed May  8 00:00:03 2024, max compression
```

## Comparing `DFRobotUPS-0.4.5.tar` & `DFRobotUPS-0.4.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 11:13:59.724898 DFRobotUPS-0.4.5/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 11:13:59.720898 DFRobotUPS-0.4.5/DFRobotUPS/
--rw-r--r--   0 pi        (1000) pi        (1000)      365 2024-05-06 11:12:04.000000 DFRobotUPS-0.4.5/DFRobotUPS/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6412 2024-05-06 11:08:00.000000 DFRobotUPS-0.4.5/DFRobotUPS/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5350 2024-05-06 11:11:33.000000 DFRobotUPS-0.4.5/DFRobotUPS/ups.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 11:13:59.724898 DFRobotUPS-0.4.5/DFRobotUPS.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-05-06 11:13:59.000000 DFRobotUPS-0.4.5/DFRobotUPS.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-05-06 11:13:59.000000 DFRobotUPS-0.4.5/DFRobotUPS.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-06 11:13:59.000000 DFRobotUPS-0.4.5/DFRobotUPS.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-05-06 11:13:59.000000 DFRobotUPS-0.4.5/DFRobotUPS.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-05-06 11:13:59.000000 DFRobotUPS-0.4.5/DFRobotUPS.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.5/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-05-06 11:13:59.724898 DFRobotUPS-0.4.5/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.5/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-05-06 11:13:59.724898 DFRobotUPS-0.4.5/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.5/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-08 00:00:03.498325 DFRobotUPS-0.4.6/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-08 00:00:03.490324 DFRobotUPS-0.4.6/DFRobotUPS/
+-rw-r--r--   0 pi        (1000) pi        (1000)      365 2024-05-07 23:57:41.000000 DFRobotUPS-0.4.6/DFRobotUPS/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6430 2024-05-06 13:37:19.000000 DFRobotUPS-0.4.6/DFRobotUPS/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5613 2024-05-06 11:36:34.000000 DFRobotUPS-0.4.6/DFRobotUPS/ups.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-08 00:00:03.498325 DFRobotUPS-0.4.6/DFRobotUPS.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     3462 2024-05-08 00:00:02.000000 DFRobotUPS-0.4.6/DFRobotUPS.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-05-08 00:00:03.000000 DFRobotUPS-0.4.6/DFRobotUPS.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-08 00:00:02.000000 DFRobotUPS-0.4.6/DFRobotUPS.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-05-08 00:00:02.000000 DFRobotUPS-0.4.6/DFRobotUPS.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-05-08 00:00:02.000000 DFRobotUPS-0.4.6/DFRobotUPS.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.6/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     3462 2024-05-08 00:00:03.498325 DFRobotUPS-0.4.6/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     2312 2024-05-06 11:20:42.000000 DFRobotUPS-0.4.6/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-05-08 00:00:03.502326 DFRobotUPS-0.4.6/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-05-06 10:29:19.000000 DFRobotUPS-0.4.6/setup.py
```

### Comparing `DFRobotUPS-0.4.5/DFRobotUPS/__main__.py` & `DFRobotUPS-0.4.6/DFRobotUPS/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,16 @@
 
 
 
 # --- main ---
 
 
 
-logger.info(
-    f"DFRobotUPS HAT on bus {args.bus} at I2C address 0x{args.addr:02x}")
+logger.info(f"searching for UPS HAT on bus {args.bus} at I2C address"
+            f" 0x{args.addr:02x}")
 
 
 # try to detect the UPS
 
 tries = 0
 while True:
     tries += 1
```

### Comparing `DFRobotUPS-0.4.5/DFRobotUPS/ups.py` & `DFRobotUPS-0.4.6/DFRobotUPS/ups.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,18 @@
 
 PID = 0xdf
 
 
 # status codes for DFRobotUPS.detect
 
 DETECT_OK         = 0   # detected OK
-DETECT_NOSMBUS    = 1   # error opening smbus
-DETECT_NODEVICE   = 2   # no device at I2C address
-DETECT_INVALIDPID = 3   # PID does not match UPS HAT
+DETECT_NOSMBUS    = 1   # not found error opening smbus
+DETECT_SMBUSPERM  = 2   # permission error opening smbus
+DETECT_NODEVICE   = 3   # no device at I2C address
+DETECT_INVALIDPID = 4   # PID does not match UPS HAT
 
 
 # the numbers of registers for UPS information, as read using
 # smbus.SMBus.read_byte_data()
 
 REG_ADDR     = 0x00
 REG_PID      = 0x01
@@ -79,14 +80,17 @@
 
         self.addr = addr
         try:
             self.bus = smbus.SMBus(bus)
         except FileNotFoundError:
             self.detect = DETECT_NOSMBUS
             return
+        except PermissionError:
+            self.detect = DETECT_SMBUSPERM
+            return
 
         # probe the device at the I2C address and set the 'detect'
         # attribute accordingly
         try:
             pid = self._get_pid()
         except OSError:
             # no device responded at the I2C address
@@ -181,14 +185,16 @@
         to detect the UPS HAT.
         """
 
         if self.detect == DETECT_OK:
             return "OK"
         elif self.detect == DETECT_NOSMBUS:
             return "I2C smbus not found"
+        elif self.detect == DETECT_SMBUSPERM:
+            return "permission error opening I2C smbus"
         elif self.detect == DETECT_NODEVICE:
             return "no device at I2C address"
         elif self.detect == DETECT_INVALIDPID:
             return "device at I2C address has incorrect PID"
         else:
             return "unknown error"
```

### Comparing `DFRobotUPS-0.4.5/LICENSE` & `DFRobotUPS-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4.5/setup.py` & `DFRobotUPS-0.4.6/setup.py`

 * *Files identical despite different names*


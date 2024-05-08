# Comparing `tmp/python-sscma-0.5.3.tar.gz` & `tmp/python-sscma-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sscma-0.5.3.tar", last modified: Thu Apr 18 02:28:13 2024, max compression
+gzip compressed data, was "python-sscma-0.5.4.tar", last modified: Wed May  8 07:48:57 2024, max compression
```

## Comparing `python-sscma-0.5.3.tar` & `python-sscma-0.5.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.830465 python-sscma-0.5.3/
--rw-rw-rw-   0        0        0     2888 2024-04-18 02:28:13.830465 python-sscma-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2370 2024-04-18 02:26:49.000000 python-sscma-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.801664 python-sscma-0.5.3/python_sscma.egg-info/
--rw-rw-rw-   0        0        0     2888 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-18 02:28:13.000000 python-sscma-0.5.3/python_sscma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 02:28:13.830465 python-sscma-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1310 2024-04-16 09:12:35.000000 python-sscma-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.802661 python-sscma-0.5.3/sscma/
--rw-rw-rw-   0        0        0       87 2024-04-18 02:26:20.000000 python-sscma-0.5.3/sscma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.806662 python-sscma-0.5.3/sscma/cli/
--rw-rw-rw-   0        0        0        0 2024-04-16 06:11:20.000000 python-sscma-0.5.3/sscma/cli/__init__.py
--rw-rw-rw-   0        0        0      253 2024-04-18 01:46:33.000000 python-sscma-0.5.3/sscma/cli/cli.py
--rw-rw-rw-   0        0        0     4547 2024-04-18 02:07:12.000000 python-sscma-0.5.3/sscma/cli/client.py
--rw-rw-rw-   0        0        0     3008 2024-04-18 02:25:18.000000 python-sscma-0.5.3/sscma/cli/flahser.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.809662 python-sscma-0.5.3/sscma/flashers/
--rw-rw-rw-   0        0        0       73 2024-04-16 06:11:41.000000 python-sscma-0.5.3/sscma/flashers/__init__.py
--rw-rw-rw-   0        0        0      941 2024-04-18 02:20:10.000000 python-sscma-0.5.3/sscma/flashers/base.py
--rw-rw-rw-   0        0        0     5256 2024-04-18 02:26:00.000000 python-sscma-0.5.3/sscma/flashers/core.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.810661 python-sscma-0.5.3/sscma/fonts/
--rw-rw-rw-   0        0        0  1580784 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/fonts/Arial.ttf
-drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.820627 python-sscma-0.5.3/sscma/micro/
--rw-rw-rw-   0        0        0      341 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/__init__.py
--rw-rw-rw-   0        0        0    13707 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/client.py
--rw-rw-rw-   0        0        0     4730 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/const.py
--rw-rw-rw-   0        0        0    24553 2024-04-16 06:21:15.000000 python-sscma-0.5.3/sscma/micro/device.py
--rw-rw-rw-   0        0        0     1231 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/exceptions.py
--rw-rw-rw-   0        0        0    10869 2024-04-16 05:34:06.000000 python-sscma-0.5.3/sscma/micro/info.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.822627 python-sscma-0.5.3/sscma/utils/
--rw-rw-rw-   0        0        0        0 2024-01-11 03:24:44.000000 python-sscma-0.5.3/sscma/utils/__init__.py
--rw-rw-rw-   0        0        0      844 2024-01-11 03:24:44.000000 python-sscma-0.5.3/sscma/utils/image.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:28:13.828630 python-sscma-0.5.3/tests/
--rw-rw-rw-   0        0        0      122 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/__init__.py
--rw-rw-rw-   0        0        0     2239 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/test_mqtt.py
--rw-rw-rw-   0        0        0     2039 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/test_mqttclient.py
--rw-rw-rw-   0        0        0     2135 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/test_serial.py
--rw-rw-rw-   0        0        0     1540 2024-04-16 05:34:06.000000 python-sscma-0.5.3/tests/test_serialclient.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:48:57.507488 python-sscma-0.5.4/
+-rw-rw-rw-   0        0        0     3033 2024-05-08 07:48:57.506487 python-sscma-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2515 2024-05-08 07:47:49.000000 python-sscma-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 07:48:57.477165 python-sscma-0.5.4/python_sscma.egg-info/
+-rw-rw-rw-   0        0        0     3033 2024-05-08 07:48:57.000000 python-sscma-0.5.4/python_sscma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2024-05-08 07:48:57.000000 python-sscma-0.5.4/python_sscma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 07:48:57.000000 python-sscma-0.5.4/python_sscma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-08 07:48:57.000000 python-sscma-0.5.4/python_sscma.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2024-05-08 07:48:57.000000 python-sscma-0.5.4/python_sscma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-08 07:48:57.000000 python-sscma-0.5.4/python_sscma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 07:48:57.507488 python-sscma-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1310 2024-04-16 09:12:35.000000 python-sscma-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:48:57.478163 python-sscma-0.5.4/sscma/
+-rw-rw-rw-   0        0        0       87 2024-05-08 07:48:35.000000 python-sscma-0.5.4/sscma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:48:57.483164 python-sscma-0.5.4/sscma/cli/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:02:34.000000 python-sscma-0.5.4/sscma/cli/__init__.py
+-rw-rw-rw-   0        0        0      253 2024-05-08 06:33:24.000000 python-sscma-0.5.4/sscma/cli/cli.py
+-rw-rw-rw-   0        0        0     4547 2024-04-18 02:07:12.000000 python-sscma-0.5.4/sscma/cli/client.py
+-rw-rw-rw-   0        0        0     3383 2024-05-08 07:45:25.000000 python-sscma-0.5.4/sscma/cli/flahser.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:48:57.486165 python-sscma-0.5.4/sscma/flashers/
+-rw-rw-rw-   0        0        0       73 2024-04-16 06:11:41.000000 python-sscma-0.5.4/sscma/flashers/__init__.py
+-rw-rw-rw-   0        0        0     1132 2024-05-08 07:45:44.000000 python-sscma-0.5.4/sscma/flashers/base.py
+-rw-rw-rw-   0        0        0     5698 2024-05-08 07:46:31.000000 python-sscma-0.5.4/sscma/flashers/core.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:48:57.487165 python-sscma-0.5.4/sscma/fonts/
+-rw-rw-rw-   0        0        0  1580784 2024-04-16 05:34:06.000000 python-sscma-0.5.4/sscma/fonts/Arial.ttf
+drwxrwxrwx   0        0        0        0 2024-05-08 07:48:57.497828 python-sscma-0.5.4/sscma/micro/
+-rw-rw-rw-   0        0        0      341 2024-04-16 05:34:06.000000 python-sscma-0.5.4/sscma/micro/__init__.py
+-rw-rw-rw-   0        0        0    13707 2024-04-16 05:34:06.000000 python-sscma-0.5.4/sscma/micro/client.py
+-rw-rw-rw-   0        0        0     4730 2024-04-16 05:34:06.000000 python-sscma-0.5.4/sscma/micro/const.py
+-rw-rw-rw-   0        0        0    24553 2024-04-16 06:21:15.000000 python-sscma-0.5.4/sscma/micro/device.py
+-rw-rw-rw-   0        0        0     1231 2024-04-16 05:34:06.000000 python-sscma-0.5.4/sscma/micro/exceptions.py
+-rw-rw-rw-   0        0        0    10869 2024-04-16 05:34:06.000000 python-sscma-0.5.4/sscma/micro/info.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:48:57.500481 python-sscma-0.5.4/sscma/utils/
+-rw-rw-rw-   0        0        0        0 2024-01-11 03:24:44.000000 python-sscma-0.5.4/sscma/utils/__init__.py
+-rw-rw-rw-   0        0        0      844 2024-01-11 03:24:44.000000 python-sscma-0.5.4/sscma/utils/image.py
+drwxrwxrwx   0        0        0        0 2024-05-08 07:48:57.505491 python-sscma-0.5.4/tests/
+-rw-rw-rw-   0        0        0      122 2024-04-16 05:34:06.000000 python-sscma-0.5.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2239 2024-04-16 05:34:06.000000 python-sscma-0.5.4/tests/test_mqtt.py
+-rw-rw-rw-   0        0        0     2039 2024-04-16 05:34:06.000000 python-sscma-0.5.4/tests/test_mqttclient.py
+-rw-rw-rw-   0        0        0     2135 2024-04-16 05:34:06.000000 python-sscma-0.5.4/tests/test_serial.py
+-rw-rw-rw-   0        0        0     1540 2024-04-16 05:34:06.000000 python-sscma-0.5.4/tests/test_serialclient.py
```

### Comparing `python-sscma-0.5.3/PKG-INFO` & `python-sscma-0.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sscma
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python library for sscma
 Home-page: https://github.com/Seeed-Studio/python-sscma
 Author: Seeed Studio
 Author-email: lht856@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -92,21 +92,26 @@
 Usage: sscma.cli flasher [OPTIONS]
 
 Options:
   -p, --port TEXT         Port to connect to
   -f, --file TEXT         File to write to the device
   -b, --baudrate INTEGER  Baud rate for the serial connection
   -o, --offset TEXT       Offset to write the file to
-  --help 
+  -s, --sn                Write serial number
+  --help                  Show this message and exit.
 ```
 
 ```bash
 sscma.cli flasher -p /dev/ttyUSB0 -f firmware.bin 
 ```
 
+```bash
+sscma.cli flasher -p /dev/ttyUSB0 -s
+```
+
 ## Contributing
 
 If you have any idea or suggestion, please open an issue first.
 
 If you want to contribute code, please fork this repository and submit a pull
 request.
```

### Comparing `python-sscma-0.5.3/README.md` & `python-sscma-0.5.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -77,21 +77,26 @@
 Usage: sscma.cli flasher [OPTIONS]
 
 Options:
   -p, --port TEXT         Port to connect to
   -f, --file TEXT         File to write to the device
   -b, --baudrate INTEGER  Baud rate for the serial connection
   -o, --offset TEXT       Offset to write the file to
-  --help 
+  -s, --sn                Write serial number
+  --help                  Show this message and exit.
 ```
 
 ```bash
 sscma.cli flasher -p /dev/ttyUSB0 -f firmware.bin 
 ```
 
+```bash
+sscma.cli flasher -p /dev/ttyUSB0 -s
+```
+
 ## Contributing
 
 If you have any idea or suggestion, please open an issue first.
 
 If you want to contribute code, please fork this repository and submit a pull
 request.
```

### Comparing `python-sscma-0.5.3/python_sscma.egg-info/PKG-INFO` & `python-sscma-0.5.4/python_sscma.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sscma
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python library for sscma
 Home-page: https://github.com/Seeed-Studio/python-sscma
 Author: Seeed Studio
 Author-email: lht856@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -92,21 +92,26 @@
 Usage: sscma.cli flasher [OPTIONS]
 
 Options:
   -p, --port TEXT         Port to connect to
   -f, --file TEXT         File to write to the device
   -b, --baudrate INTEGER  Baud rate for the serial connection
   -o, --offset TEXT       Offset to write the file to
-  --help 
+  -s, --sn                Write serial number
+  --help                  Show this message and exit.
 ```
 
 ```bash
 sscma.cli flasher -p /dev/ttyUSB0 -f firmware.bin 
 ```
 
+```bash
+sscma.cli flasher -p /dev/ttyUSB0 -s
+```
+
 ## Contributing
 
 If you have any idea or suggestion, please open an issue first.
 
 If you want to contribute code, please fork this repository and submit a pull
 request.
```

### Comparing `python-sscma-0.5.3/python_sscma.egg-info/SOURCES.txt` & `python-sscma-0.5.4/python_sscma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/setup.py` & `python-sscma-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/sscma/cli/client.py` & `python-sscma-0.5.4/sscma/cli/client.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/sscma/cli/flahser.py` & `python-sscma-0.5.4/sscma/cli/flahser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import traceback
 import click
 from sscma.flashers import FLASHERS
 
+
 def get_flasher_by_port(com=None):
     
     import os
 
     if os.name == 'nt':  # sys.platform == 'win32':
         from serial.tools.list_ports_windows import comports
     elif os.name == 'posix':
@@ -50,28 +52,40 @@
     return selected_flasher, selected_port.device
 
 @click.command()
 @click.option('--port', '-p', default=None, help='Port to connect to')
 @click.option('--file', '-f', default=None, help='File to write to the device')
 @click.option('--baudrate',  '-b', default=921600, help='Baud rate for the serial connection')
 @click.option('--offset', '-o', default='0x00', help='Offset to write the file to')
-def flasher(port, baudrate, file, offset):
+@click.option('--sn', '-s', is_flag=True, default=False, help='Write serial number')
+def flasher(port, baudrate, file, offset, sn):
+    
+    if sn is False and file is None:
+        click.echo("No operation specified. Exiting.")
+        exit(0)
+    
     try:
         Flasher, device = get_flasher_by_port(port)
         
         if Flasher is None or device is None:
             click.echo("No device found. Exiting.")
             return
         
         flasher = Flasher(device, baudrate=baudrate)
-        if file:
+        
+        if file is not None:
             with open(file, 'rb') as file:
                 data = file.read()
                 click.echo(("Found device {}. Writing file to device...").format(device))
                 click.echo(("File: {}").format(file.name))
                 click.echo(("Offset: {}").format(offset))
                 flasher.write(data, offset=int(offset, 16))
-        else:
-            click.echo("No operation specified. Exiting.")
+        
+        if sn:            
+            number = flasher.write_sn()
+            click.echo(("Serial number: {}").format(number))
+            
+       
     except Exception as e:
         click.echo("Error: {}".format(e))
+        traceback.print_exc()
         return
```

### Comparing `python-sscma-0.5.3/sscma/flashers/base.py` & `python-sscma-0.5.4/sscma/flashers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,7 +35,15 @@
     @abstractmethod
     def write(self, data, offset=0):
         """Write data to the programmer.
 
         This method should be overridden by the subclass.
         """
         pass
+    
+    @abstractmethod
+    def write_sn(self):
+        """Write serial number to the programmer.
+
+        This method should be overridden by the subclass.
+        """
+        pass
```

### Comparing `python-sscma-0.5.3/sscma/flashers/core.py` & `python-sscma-0.5.4/sscma/flashers/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 import io
 import time
 import serial 
 import logging
+import secrets
 
 from tqdm import tqdm
 from xmodem import XMODEM
 
 from sscma.flashers.base import BaseFlasher
 
+def fnv_hash(id_full):
+    hash_value = 0x811c9dc5
+    prime = 0x1000193
+    for value in id_full:
+        hash_value ^= value
+        hash_value *= prime
+    return hash_value & 0xFFFFFFFF 
+
 
 class HimaxFlasher(BaseFlasher):
     
     _NAME = "Himax Flasher"
     
     _USB = [{"vid": 0x1A86, "pid": 0x55D2},
             {"vid": 0x1A86, "pid": 0x55D3}]
@@ -162,13 +171,21 @@
         self.serial.close()
         time.sleep(0.5)
         self.serial.open()
         time.sleep(0.5)
         self.serial.close()
         
         progress_bar.close()
+        
+        
+    def write_sn(self):
+        random_bytes = secrets.token_bytes(4 * 1024)
+        sn = str(hex(fnv_hash(random_bytes[:16])))
+        self.write(random_bytes, 0x003DF000)
+        return sn
+
```

### Comparing `python-sscma-0.5.3/sscma/fonts/Arial.ttf` & `python-sscma-0.5.4/sscma/fonts/Arial.ttf`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/sscma/micro/client.py` & `python-sscma-0.5.4/sscma/micro/client.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/sscma/micro/const.py` & `python-sscma-0.5.4/sscma/micro/const.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/sscma/micro/device.py` & `python-sscma-0.5.4/sscma/micro/device.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/sscma/micro/exceptions.py` & `python-sscma-0.5.4/sscma/micro/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/sscma/micro/info.py` & `python-sscma-0.5.4/sscma/micro/info.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/sscma/utils/image.py` & `python-sscma-0.5.4/sscma/utils/image.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/tests/test_mqtt.py` & `python-sscma-0.5.4/tests/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/tests/test_mqttclient.py` & `python-sscma-0.5.4/tests/test_mqttclient.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/tests/test_serial.py` & `python-sscma-0.5.4/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `python-sscma-0.5.3/tests/test_serialclient.py` & `python-sscma-0.5.4/tests/test_serialclient.py`

 * *Files identical despite different names*


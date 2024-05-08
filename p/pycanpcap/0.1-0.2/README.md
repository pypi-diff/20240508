# Comparing `tmp/pycanpcap-0.1.tar.gz` & `tmp/pycanpcap-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycanpcap-0.1.tar", last modified: Fri Feb 23 21:08:01 2024, max compression
+gzip compressed data, was "pycanpcap-0.2.tar", last modified: Wed May  8 15:02:19 2024, max compression
```

## Comparing `pycanpcap-0.1.tar` & `pycanpcap-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 21:08:01.075188 pycanpcap-0.1/
--rw-rw-rw-   0        0        0     1088 2024-02-23 20:52:51.000000 pycanpcap-0.1/LICENSE
--rw-rw-rw-   0        0        0     1276 2024-02-23 21:08:01.074182 pycanpcap-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      789 2024-02-23 21:04:50.000000 pycanpcap-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-23 21:08:01.064179 pycanpcap-0.1/pycanpcap/
--rw-rw-rw-   0        0        0        0 2024-02-23 19:44:37.000000 pycanpcap-0.1/pycanpcap/__init__.py
--rw-rw-rw-   0        0        0     3158 2024-02-23 21:04:26.000000 pycanpcap-0.1/pycanpcap/log.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:08:01.072182 pycanpcap-0.1/pycanpcap.egg-info/
--rw-rw-rw-   0        0        0     1276 2024-02-23 21:08:00.000000 pycanpcap-0.1/pycanpcap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-02-23 21:08:00.000000 pycanpcap-0.1/pycanpcap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 21:08:00.000000 pycanpcap-0.1/pycanpcap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-02-23 21:08:00.000000 pycanpcap-0.1/pycanpcap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-23 21:08:00.000000 pycanpcap-0.1/pycanpcap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-23 21:08:01.075188 pycanpcap-0.1/setup.cfg
--rw-rw-rw-   0        0        0      678 2024-02-23 20:54:18.000000 pycanpcap-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:02:19.736405 pycanpcap-0.2/
+-rw-rw-rw-   0        0        0     2182 2024-05-08 03:42:18.000000 pycanpcap-0.2/LICENSE
+-rw-rw-rw-   0        0        0     1300 2024-05-08 15:02:19.733400 pycanpcap-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2024-05-08 03:42:18.000000 pycanpcap-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:02:19.705279 pycanpcap-0.2/pycanpcap/
+-rw-rw-rw-   0        0        0        0 2024-05-08 03:42:18.000000 pycanpcap-0.2/pycanpcap/__init__.py
+-rw-rw-rw-   0        0        0     3467 2024-05-08 03:50:46.000000 pycanpcap-0.2/pycanpcap/log.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:02:19.731414 pycanpcap-0.2/pycanpcap.egg-info/
+-rw-rw-rw-   0        0        0     1300 2024-05-08 15:02:19.000000 pycanpcap-0.2/pycanpcap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-08 15:02:19.000000 pycanpcap-0.2/pycanpcap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:02:19.000000 pycanpcap-0.2/pycanpcap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-08 15:02:19.000000 pycanpcap-0.2/pycanpcap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 15:02:19.000000 pycanpcap-0.2/pycanpcap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:02:19.736405 pycanpcap-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      679 2024-05-08 15:01:12.000000 pycanpcap-0.2/setup.py
```

### Comparing `pycanpcap-0.1/PKG-INFO` & `pycanpcap-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pycanpcap
-Version: 0.1
+Version: 0.2
 Summary: candump and write a pcap using scapy (and python-can)
 Home-page: https://github.com/BenGardiner/pycanpcap
 Author: Ben Gardiner
 Author-email: ben.l.gardiner@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scapy>=2.4.5
+Requires-Dist: python-can~=4.3.1
 
 candump and write a pcap using scapy (and python-can)
 
 ```cmd.exe
  > python -m pip install pycanpcap
  > python -m pycanpcap.log -i cantact -c 0 -w can.pcap
 WARNING: No libpcap provider available ! pcap won't be used
@@ -30,8 +30,7 @@
 ^C
 ```
 
 1. ignore the warnings on windows
 2. Ctrl-C when ready
 3. open can.pcap in wireshark
 4. grep the output as usual
-
```

### Comparing `pycanpcap-0.1/pycanpcap/log.py` & `pycanpcap-0.2/pycanpcap/log.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,116 @@
-import argparse
-import re
-
-from ast import literal_eval
-
-from scapy.all import sniff, wrpcap
-import scapy.libs.six as six
-from scapy.config import conf
-from scapy.consts import LINUX
-
-if six.PY2 or not LINUX or conf.use_pypy:
-    conf.contribs['CANSocket'] = {'use-python-can': True}
-
-from scapy.contrib.cansocket import CANSocket, PYTHON_CAN  # noqa: E402
-
-
-def create_socket(python_can_args, interface, channel):
-    if PYTHON_CAN:
-        if python_can_args:
-            interface_string = "PythonCANSocket(bustype=" \
-                               "'%s', channel='%s', %s)" % \
-                               (interface, channel, python_can_args)
-            arg_dict = dict((k, literal_eval(v)) for k, v in
-                            (pair.split('=') for pair in
-                             re.split(', | |,', python_can_args)))
-            sock = CANSocket(bustype=interface, channel=channel,
-                             **arg_dict)
-        else:
-            interface_string = "PythonCANSocket(bustype=" \
-                               "'%s', channel='%s')" % \
-                               (interface, channel)
-            sock = CANSocket(bustype=interface, channel=channel)
-    else:
-        sock = CANSocket(channel=channel)
-        interface_string = "\"%s\"" % channel
-
-    return sock, interface_string
-
-
-def sanitize_string(input_string):
-    s = input_string.replace('bustype', '').replace('channel','')
-    s = ''.join(ch if ch.isalnum() else '_' for ch in s)
-    s = re.sub('_+', '_', s)  # replace multiple underscores with a single one
-    s = re.sub('_+$', '', s)  # remove trailing underscores
-    return s
-
-
-def main():
-    parser = argparse.ArgumentParser(description='print a canlog and capture to a pcap using scapy')
-    parser.add_argument('-i', '--interface', type=str, required=False, help='''python-can interface for the scan.
-                          Depends on used interpreter and system,
-                          see examples below. Any python-can interface can
-                          be provided. Please see:
-                          https://python-can.readthedocs.io for
-                          further interface examples.''')
-    parser.add_argument('-c', '--channel', type=int, required=True,
-                        help='Additional arguments for a python-can Bus object.')
-    parser.add_argument('-a', '--python-can_args', type=str, required=False,
-                        help='python-can channel or Linux SocketCAN interface name')
-    parser.add_argument('-w', '--write', type=str, required=False, help='Output pcap file')
-
-    args = parser.parse_args()
-
-    sock, interface_string = \
-        create_socket(args.python_can_args, args.interface, args.channel)
-
-    pretty_iface_name = sanitize_string(interface_string)
-    def packet_handler(pkt):
-        print(f'({pkt.time:010.06f}) {pretty_iface_name} {pkt.identifier:03x}#{pkt.data.hex()}')
-        if args.write is not None:
-            wrpcap(args.write, pkt, append=True)
-
-    sniff(opened_socket=sock, prn=packet_handler)
-
-
-if __name__ == '__main__':
-    main()
+import argparse
+import re
+
+from ast import literal_eval
+
+from scapy.all import sniff, wrpcap
+import scapy.libs.six as six
+from scapy.config import conf
+from scapy.consts import LINUX
+
+if six.PY2 or not LINUX or conf.use_pypy:
+    conf.contribs["CANSocket"] = {"use-python-can": True}
+
+from scapy.contrib.cansocket import CANSocket, PYTHON_CAN  # noqa: E402
+
+
+def create_socket(python_can_args, interface, channel, bitrate):
+    if PYTHON_CAN:
+        if python_can_args:
+            interface_string = "PythonCANSocket(interface=" "'%s', channel='%s', %s)" % (
+                interface,
+                channel,
+                python_can_args,
+            )
+            arg_dict = dict(
+                (k, literal_eval(v))
+                for k, v in (
+                    pair.split("=") for pair in re.split(", | |,", python_can_args)
+                )
+            )
+            sock = CANSocket(
+                interface=interface, channel=channel, bitrate=bitrate, **arg_dict
+            )
+        else:
+            interface_string = "PythonCANSocket(interface=" "'%s', channel='%s')" % (
+                interface,
+                channel,
+            )
+            sock = CANSocket(interface=interface, channel=channel, bitrate=bitrate)
+    else:
+        sock = CANSocket(channel=channel)
+        interface_string = '"%s"' % channel
+
+    return sock, interface_string
+
+
+def sanitize_string(input_string):
+    s = input_string.replace("interface", "").replace("channel", "")
+    s = "".join(ch if ch.isalnum() else "_" for ch in s)
+    s = re.sub("_+", "_", s)  # replace multiple underscores with a single one
+    s = re.sub("_+$", "", s)  # remove trailing underscores
+    return s
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description="print a canlog and capture to a pcap using scapy"
+    )
+    parser.add_argument(
+        "-i",
+        "--interface",
+        type=str,
+        required=False,
+        help="""python-can interface for the scan.
+                          Depends on used interpreter and system,
+                          see examples below. Any python-can interface can
+                          be provided. Please see:
+                          https://python-can.readthedocs.io for
+                          further interface examples.""",
+    )
+    parser.add_argument(
+        "-c",
+        "--channel",
+        type=str,
+        required=True,
+        help="Additional arguments for a python-can Bus object.",
+    )
+    parser.add_argument(
+        "-b",
+        "--bitrate",
+        type=int,
+        required=False,
+        default=500_000,
+        help="Bits per second.",
+    )
+    parser.add_argument(
+        "-a",
+        "--python-can_args",
+        type=str,
+        required=False,
+        help="python-can channel or Linux SocketCAN interface name",
+    )
+    parser.add_argument(
+        "-w", "--write", type=str, required=False, help="Output pcap file"
+    )
+
+    args = parser.parse_args()
+
+    sock, interface_string = create_socket(
+        args.python_can_args, args.interface, args.channel, args.bitrate
+    )
+
+    pretty_iface_name = sanitize_string(interface_string)
+
+    def packet_handler(pkt):
+        print(
+            f"({pkt.time:010.06f}) {pretty_iface_name} {pkt.identifier:03x}#{pkt.data.hex()}"
+        )
+        if args.write is not None:
+            wrpcap(args.write, pkt, append=True)
+
+    sniff(opened_socket=sock, prn=packet_handler)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pycanpcap-0.1/pycanpcap.egg-info/PKG-INFO` & `pycanpcap-0.2/pycanpcap.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pycanpcap
-Version: 0.1
+Version: 0.2
 Summary: candump and write a pcap using scapy (and python-can)
 Home-page: https://github.com/BenGardiner/pycanpcap
 Author: Ben Gardiner
 Author-email: ben.l.gardiner@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: scapy>=2.4.5
+Requires-Dist: python-can~=4.3.1
 
 candump and write a pcap using scapy (and python-can)
 
 ```cmd.exe
  > python -m pip install pycanpcap
  > python -m pycanpcap.log -i cantact -c 0 -w can.pcap
 WARNING: No libpcap provider available ! pcap won't be used
@@ -30,8 +30,7 @@
 ^C
 ```
 
 1. ignore the warnings on windows
 2. Ctrl-C when ready
 3. open can.pcap in wireshark
 4. grep the output as usual
-
```


# Comparing `tmp/openobd_protocol-0.0.45.tar.gz` & `tmp/openobd_protocol-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd_protocol-0.0.45.tar", last modified: Tue May  7 14:21:50 2024, max compression
+gzip compressed data, was "openobd_protocol-0.0.46.tar", last modified: Tue May  7 14:32:34 2024, max compression
```

## Comparing `openobd_protocol-0.0.45.tar` & `openobd_protocol-0.0.46.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:21:50.395592 openobd_protocol-0.0.45/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-07 14:21:50.395592 openobd_protocol-0.0.45/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 14:21:50.396592 openobd_protocol-0.0.45/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:21:50.381591 openobd_protocol-0.0.45/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:21:50.387592 openobd_protocol-0.0.45/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1359 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:21:50.390592 openobd_protocol-0.0.45/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     1978 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      462 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2565 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2349 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      405 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8395 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:21:50.392592 openobd_protocol-0.0.45/src/openobd_protocol/SessionController/
--rw-r--r--   0 root         (0) root         (0)     2466 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/SessionController/SessionServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    10384 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2512 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/SessionController/Session_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2494 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/SessionController/Session_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1712 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:21:50.394592 openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     1748 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2973 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-07 14:21:46.000000 openobd_protocol-0.0.45/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:21:50.395592 openobd_protocol-0.0.45/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-07 14:21:50.000000 openobd_protocol-0.0.45/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1610 2024-05-07 14:21:50.000000 openobd_protocol-0.0.45/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 14:21:50.000000 openobd_protocol-0.0.45/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-05-07 14:21:50.000000 openobd_protocol-0.0.45/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 14:21:50.000000 openobd_protocol-0.0.45/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.531825 openobd_protocol-0.0.46/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-07 14:32:34.531825 openobd_protocol-0.0.46/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 14:32:34.531825 openobd_protocol-0.0.46/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.516825 openobd_protocol-0.0.46/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.522825 openobd_protocol-0.0.46/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.525825 openobd_protocol-0.0.46/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      462 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8395 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.527825 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    10384 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/Session_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/SessionController/Session_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.530825 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-07 14:32:29.000000 openobd_protocol-0.0.46/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 14:32:34.530825 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 14:32:34.000000 openobd_protocol-0.0.46/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd_protocol-0.0.45/LICENSE` & `openobd_protocol-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/PKG-INFO` & `openobd_protocol-0.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.45
+Version: 0.0.46
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.45/pyproject.toml` & `openobd_protocol-0.0.46/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/Authentication_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/Authentication_pb2.pyi` & `openobd_protocol-0.0.46/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/BasicResponse_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/BasicResponse_pb2.pyi` & `openobd_protocol-0.0.46/src/openobd_protocol/BasicResponse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd_protocol-0.0.46/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd_protocol-0.0.46/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd_protocol-0.0.46/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd_protocol-0.0.46/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/SessionController/SessionServices_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py` & `openobd_protocol-0.0.46/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/SessionController/Session_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/SessionController/Session_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/SessionController/Session_pb2.pyi` & `openobd_protocol-0.0.46/src/openobd_protocol/SessionController/Session_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/Status_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/Status_pb2.pyi` & `openobd_protocol-0.0.46/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd_protocol-0.0.46/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol.egg-info/PKG-INFO` & `openobd_protocol-0.0.46/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.45
+Version: 0.0.46
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.45/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd_protocol-0.0.46/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*


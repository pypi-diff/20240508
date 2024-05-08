# Comparing `tmp/asyncio-dgram-2.1.2.tar.gz` & `tmp/asyncio-dgram-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio-dgram-2.1.2.tar", last modified: Fri Feb  4 17:50:09 2022, max compression
+gzip compressed data, was "asyncio-dgram-2.2.0.tar", last modified: Wed May  8 19:21:47 2024, max compression
```

## Comparing `asyncio-dgram-2.1.2.tar` & `asyncio-dgram-2.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jbronder  (1000) jbronder  (1000)        0 2022-02-04 17:50:09.716645 asyncio-dgram-2.1.2/
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)     1071 2019-09-18 04:10:15.000000 asyncio-dgram-2.1.2/LICENSE
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)      166 2021-07-21 14:33:27.000000 asyncio-dgram-2.1.2/MANIFEST.in
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)     1796 2021-07-21 14:33:27.000000 asyncio-dgram-2.1.2/Makefile
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)     3245 2022-02-04 17:50:09.716645 asyncio-dgram-2.1.2/PKG-INFO
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)     2397 2021-02-12 20:43:50.000000 asyncio-dgram-2.1.2/README.md
-drwxr-xr-x   0 jbronder  (1000) jbronder  (1000)        0 2022-02-04 17:50:09.715645 asyncio-dgram-2.1.2/asyncio_dgram/
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)       27 2021-07-21 14:33:27.000000 asyncio-dgram-2.1.2/asyncio_dgram/__init__.py
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)     9955 2022-02-04 17:36:19.000000 asyncio-dgram-2.1.2/asyncio_dgram/aio.py
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)     1756 2021-12-23 20:59:58.000000 asyncio-dgram-2.1.2/asyncio_dgram/aio.pyi
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)        0 2021-07-21 14:33:27.000000 asyncio-dgram-2.1.2/asyncio_dgram/py.typed
-drwxr-xr-x   0 jbronder  (1000) jbronder  (1000)        0 2022-02-04 17:50:09.716645 asyncio-dgram-2.1.2/asyncio_dgram.egg-info/
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)     3245 2022-02-04 17:50:09.000000 asyncio-dgram-2.1.2/asyncio_dgram.egg-info/PKG-INFO
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)      400 2022-02-04 17:50:09.000000 asyncio-dgram-2.1.2/asyncio_dgram.egg-info/SOURCES.txt
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)        1 2022-02-04 17:50:09.000000 asyncio-dgram-2.1.2/asyncio_dgram.egg-info/dependency_links.txt
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)      153 2022-02-04 17:50:09.000000 asyncio-dgram-2.1.2/asyncio_dgram.egg-info/requires.txt
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)       14 2022-02-04 17:50:09.000000 asyncio-dgram-2.1.2/asyncio_dgram.egg-info/top_level.txt
--rwxr-xr-x   0 jbronder  (1000) jbronder  (1000)      882 2019-09-18 04:10:15.000000 asyncio-dgram-2.1.2/dev-env.sh
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)      145 2021-07-21 14:33:27.000000 asyncio-dgram-2.1.2/requirements-test.txt
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)        0 2019-09-18 04:10:15.000000 asyncio-dgram-2.1.2/requirements.txt
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)       98 2022-02-04 17:50:09.717645 asyncio-dgram-2.1.2/setup.cfg
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)     1455 2022-02-04 17:37:54.000000 asyncio-dgram-2.1.2/setup.py
-drwxr-xr-x   0 jbronder  (1000) jbronder  (1000)        0 2022-02-04 17:50:09.716645 asyncio-dgram-2.1.2/test/
--rw-r--r--   0 jbronder  (1000) jbronder  (1000)    15674 2021-02-12 20:38:08.000000 asyncio-dgram-2.1.2/test/test_aio.py
+drwxr-xr-x   0 jbronder  (1000) jbronder  (1000)        0 2024-05-08 19:21:47.579092 asyncio-dgram-2.2.0/
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)     1071 2022-07-01 15:11:16.000000 asyncio-dgram-2.2.0/LICENSE
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)      166 2022-07-01 15:11:16.000000 asyncio-dgram-2.2.0/MANIFEST.in
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)     1796 2023-09-05 15:59:23.000000 asyncio-dgram-2.2.0/Makefile
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)     3278 2024-05-08 19:21:47.579092 asyncio-dgram-2.2.0/PKG-INFO
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)     2397 2022-07-01 15:11:16.000000 asyncio-dgram-2.2.0/README.md
+drwxr-xr-x   0 jbronder  (1000) jbronder  (1000)        0 2024-05-08 19:21:47.579092 asyncio-dgram-2.2.0/asyncio_dgram/
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)       27 2022-07-01 15:11:16.000000 asyncio-dgram-2.2.0/asyncio_dgram/__init__.py
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)    10448 2022-07-05 20:52:48.000000 asyncio-dgram-2.2.0/asyncio_dgram/aio.py
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)     2130 2023-09-26 18:42:44.000000 asyncio-dgram-2.2.0/asyncio_dgram/aio.pyi
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)        0 2022-07-01 15:11:16.000000 asyncio-dgram-2.2.0/asyncio_dgram/py.typed
+drwxr-xr-x   0 jbronder  (1000) jbronder  (1000)        0 2024-05-08 19:21:47.579092 asyncio-dgram-2.2.0/asyncio_dgram.egg-info/
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)     3278 2024-05-08 19:21:47.000000 asyncio-dgram-2.2.0/asyncio_dgram.egg-info/PKG-INFO
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)      400 2024-05-08 19:21:47.000000 asyncio-dgram-2.2.0/asyncio_dgram.egg-info/SOURCES.txt
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)        1 2024-05-08 19:21:47.000000 asyncio-dgram-2.2.0/asyncio_dgram.egg-info/dependency_links.txt
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)      164 2024-05-08 19:21:47.000000 asyncio-dgram-2.2.0/asyncio_dgram.egg-info/requires.txt
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)       14 2024-05-08 19:21:47.000000 asyncio-dgram-2.2.0/asyncio_dgram.egg-info/top_level.txt
+-rwxr-xr-x   0 jbronder  (1000) jbronder  (1000)      882 2022-07-01 15:11:16.000000 asyncio-dgram-2.2.0/dev-env.sh
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)      145 2023-07-18 20:58:12.000000 asyncio-dgram-2.2.0/requirements-test.txt
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)       11 2023-07-18 20:53:58.000000 asyncio-dgram-2.2.0/requirements.txt
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)      120 2024-05-08 19:21:47.579092 asyncio-dgram-2.2.0/setup.cfg
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)     1506 2024-05-08 18:23:57.000000 asyncio-dgram-2.2.0/setup.py
+drwxr-xr-x   0 jbronder  (1000) jbronder  (1000)        0 2024-05-08 19:21:47.579092 asyncio-dgram-2.2.0/test/
+-rw-r--r--   0 jbronder  (1000) jbronder  (1000)    17746 2023-09-26 18:41:44.000000 asyncio-dgram-2.2.0/test/test_aio.py
```

### Comparing `asyncio-dgram-2.1.2/LICENSE` & `asyncio-dgram-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio-dgram-2.1.2/Makefile` & `asyncio-dgram-2.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `asyncio-dgram-2.1.2/PKG-INFO` & `asyncio-dgram-2.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: asyncio-dgram
-Version: 2.1.2
+Version: 2.2.0
 Summary: Higher level Datagram support for Asyncio
 Home-page: https://github.com/jsbronder/asyncio-dgram
 Author: Justin Bronder
 Author-email: jsbronder@cold-front.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 [![Build Status](https://github.com/jsbronder/asyncio-dgram/workflows/ci/badge.svg)](https://github.com/jsbronder/asyncio-dgram/actions)
 
 # Higher level Datagram support for Asyncio
@@ -85,8 +85,7 @@
     loop = asyncio.get_event_loop()
     loop.run_until_complete(asyncio.gather(udp_echo_server(), udp_echo_client()))
 
 
 if __name__ == "__main__":
     main()
 ```
-
```

### Comparing `asyncio-dgram-2.1.2/README.md` & `asyncio-dgram-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `asyncio-dgram-2.1.2/asyncio_dgram/aio.py` & `asyncio-dgram-2.2.0/asyncio_dgram/aio.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,23 +209,28 @@
         super().pause_writing()
 
     def resume_writing(self):
         self._drained.set()
         super().resume_writing()
 
 
-async def bind(addr):
+async def bind(addr, reuse_port=None):
     """
     Bind a socket to a local address for datagrams.  The socket will be either
     AF_INET, AF_INET6 or AF_UNIX depending upon the type of address specified.
-
     @param addr - For AF_INET or AF_INET6, a tuple with the the host and port to
                   to bind; port may be set to 0 to get any free port.
                   For AF_UNIX the path at which to bind (with a leading \0 for
                   abstract sockets).
+    @param reuse_port - Tells the kernel to allow this endpoint to be bound to
+                    the same port as other existing endpoints are bound to, so long as
+                    they all set this flag when being created. This option is not
+                    supported on Windows and some UNIX's. If the
+                    :py:data:`~socket.SO_REUSEPORT` constant is not defined then this
+                    capability is unsupported.
     @return     - A DatagramServer instance
     """
     loop = asyncio.get_event_loop()
     recvq = asyncio.Queue()
     excq = asyncio.Queue()
     drained = asyncio.Event()
 
@@ -236,14 +241,15 @@
     else:
         family = 0
 
     transport, protocol = await loop.create_datagram_endpoint(
         lambda: Protocol(recvq, excq, drained),
         local_addr=addr,
         family=family,
+        reuse_port=reuse_port,
     )
 
     return DatagramServer(transport, recvq, excq, drained)
 
 
 async def connect(addr):
     """
```

### Comparing `asyncio-dgram-2.1.2/asyncio_dgram/aio.pyi` & `asyncio-dgram-2.2.0/asyncio_dgram/aio.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 import asyncio
+import asyncio.trsock
 import pathlib
 import socket
 import sys
-from socket import _Address
+from socket import _Address, _RetAddress
 from typing import Any, Optional, Tuple, Union
 
+class TransportClosed(Exception):
+    pass
+
 class DatagramStream:
+    # Support type-checking in unittests which mock this
+    _drained: asyncio.Event
+
     def __init__(
         self,
         transport: asyncio.DatagramProtocol,
-        recvq: asyncio.Queue,
-        excq: asyncio.Queue,
+        recvq: asyncio.Queue[tuple[Optional[bytes], Optional[_Address]]],
+        excq: asyncio.Queue[Exception],
         drained: asyncio.Event,
     ) -> None: ...
+    @property
     def exception(self) -> None: ...
-    def sockname(self) -> str: ...
-    def peername(self) -> str: ...
-
-    # TODO: If upstream ever does better then Any, do so here. It's
-    # socket.socket in <3.8 and asyncio.TransportSocket thereafter.
-    def socket(self) -> Any: ...
+    @property
+    def sockname(self) -> _RetAddress: ...
+    @property
+    def peername(self) -> _RetAddress: ...
+    @property
+    def socket(self) -> socket.socket | asyncio.trsock.TransportSocket: ...
 
     def close(self) -> None: ...
     async def _send(self, data: bytes, addr: Optional[_Address]) -> None: ...
     async def recv(self) -> Tuple[bytes, _Address]: ...
 
 class DatagramServer(DatagramStream):
     async def send(self, data: bytes, addr: _Address) -> None: ...
 
 class DatagramClient(DatagramStream):
     async def send(self, data: bytes) -> None: ...
 
 class Protocol(asyncio.DatagramProtocol):
+    # Support type-checking in unittests which mock this
+    _drained: asyncio.Event
+
     def __init__(
-        self, recvq: asyncio.Queue, excq: asyncio.Queue, drained: asyncio.Event
+        self, recvq: asyncio.Queue[tuple[Optional[bytes], Optional[_Address]]], excq: asyncio.Queue[Exception], drained: asyncio.Event
     ) -> None: ...
     def connection_made(self, transport: asyncio.BaseTransport) -> None: ...
     def connection_lost(self, exc: Optional[Exception]) -> None: ...
     def datagram_received(self, data: bytes, addr: _Address) -> None: ...
     def error_received(self, exc: Exception) -> None: ...
     def pause_writing(self) -> None: ...
     def resume_writing(self) -> None: ...
 
-async def bind(addr: Union[_Address, pathlib.Path, str]) -> DatagramServer: ...
+async def bind(addr: Union[_Address, pathlib.Path, str], reuse_port: Optional[bool] = None) -> DatagramServer: ...
 async def connect(addr: Union[_Address, pathlib.Path, str]) -> DatagramClient: ...
 async def from_socket(sock: socket.socket) -> Union[DatagramServer, DatagramClient]: ...
```

### Comparing `asyncio-dgram-2.1.2/asyncio_dgram.egg-info/PKG-INFO` & `asyncio-dgram-2.2.0/asyncio_dgram.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: asyncio-dgram
-Version: 2.1.2
+Version: 2.2.0
 Summary: Higher level Datagram support for Asyncio
 Home-page: https://github.com/jsbronder/asyncio-dgram
 Author: Justin Bronder
 Author-email: jsbronder@cold-front.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 [![Build Status](https://github.com/jsbronder/asyncio-dgram/workflows/ci/badge.svg)](https://github.com/jsbronder/asyncio-dgram/actions)
 
 # Higher level Datagram support for Asyncio
@@ -85,8 +85,7 @@
     loop = asyncio.get_event_loop()
     loop.run_until_complete(asyncio.gather(udp_echo_server(), udp_echo_client()))
 
 
 if __name__ == "__main__":
     main()
 ```
-
```

### Comparing `asyncio-dgram-2.1.2/dev-env.sh` & `asyncio-dgram-2.2.0/dev-env.sh`

 * *Files identical despite different names*

### Comparing `asyncio-dgram-2.1.2/setup.py` & `asyncio-dgram-2.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,34 +14,35 @@
 extra_options = {}
 
 if sys.version_info.major == 3 and sys.version_info.minor >= 7:
     extra_options["long_description_content_type"] = "text/markdown"
 
 setuptools.setup(
     name="asyncio-dgram",
-    version="2.1.2",
+    version="2.2.0",
     description="Higher level Datagram support for Asyncio",
     long_description=readfile("README.md"),
     url="https://github.com/jsbronder/asyncio-dgram",
     author="Justin Bronder",
     author_email="jsbronder@cold-front.org",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Framework :: AsyncIO",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     package_data={"asyncio_dgram": ["*.pyi", "py.typed"]},
     include_package_data=True,
     packages=["asyncio_dgram"],
-    python_requires=">=3.5",
+    python_requires=">=3.6",
     install_requires=readfile("requirements.txt").split(),
     extras_require={"test": readfile("requirements-test.txt").split()},
     **extra_options,
 )
```

### Comparing `asyncio-dgram-2.1.2/test/test_aio.py` & `asyncio-dgram-2.2.0/test/test_aio.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 import asyncio
 import contextlib
 import os
+import pathlib
 import socket
 import sys
+import typing
 import unittest.mock
 
 import pytest
 
 import asyncio_dgram
 
+if typing.TYPE_CHECKING:
+    from socket import _Address
+else:
+    _Address = None
+
+if sys.version_info < (3, 9):
+    from typing import Generator
+else:
+    from collections.abc import Generator
+
 
 if sys.version_info < (3, 7):
     asyncio.create_task = asyncio.ensure_future
 
 
-@pytest.fixture
-def mock_socket():
-    s = unittest.mock.create_autospec(socket.socket)
-    s.family = socket.AF_INET
-    s.type = socket.SOCK_DGRAM
-
-    return s
-
-
 @contextlib.contextmanager
-def loop_exception_handler():
+def loop_exception_handler() -> Generator["asyncio.base_events._Context", None, None]:
     """
     Replace the current event loop exception handler with one that
     simply stores exceptions in the returned dictionary.
 
     @return - dictionary that is updated with the last loop exception
     """
     context = {}
 
-    def handler(self, c):
+    def handler(
+        loop: asyncio.AbstractEventLoop, c: "asyncio.base_events._Context"
+    ) -> None:
         context.update(c)
 
     loop = asyncio.get_event_loop()
     orig_handler = loop.get_exception_handler()
     loop.set_exception_handler(handler)
     yield context
 
@@ -50,19 +55,24 @@
     [
         (("127.0.0.1", 0), socket.AF_INET),
         (("::1", 0), socket.AF_INET6),
         ("socket", socket.AF_UNIX),
     ],
     ids=["INET", "INET6", "UNIX"],
 )
-async def test_connect_sync(addr, family, tmp_path):
+async def test_connect_sync(
+    addr: typing.Union[_Address, str],
+    family: socket.AddressFamily,
+    tmp_path: pathlib.Path,
+) -> None:
     # Bind a regular socket, asyncio_dgram connect, then check asyncio send and
     # receive.
 
     if family == socket.AF_UNIX:
+        assert isinstance(addr, str)
         if sys.version_info < (3, 7):
             pytest.skip()
         addr = str(tmp_path / addr)
 
     with socket.socket(family, socket.SOCK_DGRAM) as sock:
         sock.bind(addr)
         dest = addr if family == socket.AF_UNIX else sock.getsockname()[:2]
@@ -72,14 +82,15 @@
 
         await client.send(b"hi")
         got, client_addr = sock.recvfrom(4)
         assert got == b"hi"
         assert client.peername == sock.getsockname()
 
         if family == socket.AF_UNIX:
+            assert isinstance(addr, str)
             # AF_UNIX doesn't automatically bind
             assert client_addr is None
             os.unlink(addr)
         else:
             assert client_addr == client.sockname
 
             sock.sendto(b"bye", client.sockname)
@@ -125,19 +136,24 @@
     [
         (("127.0.0.1", 0), socket.AF_INET),
         (("::1", 0), socket.AF_INET6),
         ("socket", socket.AF_UNIX),
     ],
     ids=["INET", "INET6", "UNIX"],
 )
-async def test_bind_sync(addr, family, tmp_path):
+async def test_bind_sync(
+    addr: typing.Union[_Address, str],
+    family: socket.AddressFamily,
+    tmp_path: pathlib.Path,
+) -> None:
     # Bind an asyncio_dgram, regular socket connect, then check asyncio send and
     # receive.
 
     if family == socket.AF_UNIX:
+        assert isinstance(addr, str)
         if sys.version_info < (3, 7):
             pytest.skip()
         addr = str(tmp_path / addr)
 
     with socket.socket(family, socket.SOCK_DGRAM) as sock:
         server = await asyncio_dgram.bind(addr)
         sock.connect(server.sockname)
@@ -200,16 +216,21 @@
     [
         (("127.0.0.1", 0), socket.AF_INET),
         (("::1", 0), socket.AF_INET6),
         ("socket", socket.AF_UNIX),
     ],
     ids=["INET", "INET6", "UNIX"],
 )
-async def test_from_socket_streamtype(addr, family, tmp_path):
+async def test_from_socket_streamtype(
+    addr: typing.Union[_Address, str],
+    family: socket.AddressFamily,
+    tmp_path: pathlib.Path,
+) -> None:
     if family == socket.AF_UNIX:
+        assert isinstance(addr, str)
         if sys.version_info < (3, 7):
             pytest.skip()
         addr = str(tmp_path / addr)
 
     with socket.socket(family, socket.SOCK_DGRAM) as sock:
         sock.bind(addr)
         stream = await asyncio_dgram.from_socket(sock)
@@ -218,14 +239,15 @@
         assert sock.getsockname() == stream.sockname
         assert stream.peername is None
         assert stream.socket.fileno() == sock.fileno()
         assert isinstance(stream, asyncio_dgram.aio.DatagramServer)
 
     with socket.socket(family, socket.SOCK_DGRAM) as sock:
         if family == socket.AF_UNIX:
+            assert isinstance(addr, str)
             os.unlink(addr)
 
         sock.bind(addr)
 
         with socket.socket(family, socket.SOCK_DGRAM) as tsock:
             tsock.connect(sock.getsockname())
             stream = await asyncio_dgram.from_socket(tsock)
@@ -244,36 +266,41 @@
             # Make sure that the transport stored the peername
             with loop_exception_handler() as context:
                 await stream.send(b"abc")
                 assert context == {}
 
 
 @pytest.mark.asyncio
-async def test_from_socket_bad_socket(monkeypatch):
+async def test_from_socket_bad_socket(monkeypatch: pytest.MonkeyPatch) -> None:
     class MockSocket:
         family = socket.AF_PACKET
 
     with monkeypatch.context() as m:
         m.setattr(socket, "socket", lambda _, __: MockSocket())
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_DGRAM)
         with pytest.raises(TypeError, match="socket family not one of"):
             await asyncio_dgram.from_socket(sock)
 
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
-        with pytest.raises(TypeError, match="must be SocketKind.SOCK_DGRAM"):
+        if sys.version_info < (3, 11):
+            msg = "must be SocketKind.SOCK_DGRAM"
+        else:
+            msg = "socket type must be 2"
+
+        with pytest.raises(TypeError, match=msg):
             await asyncio_dgram.from_socket(sock)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "addr,family",
     [(("127.0.0.1", 0), socket.AF_INET), (("::1", 0), socket.AF_INET6)],
     ids=["INET", "INET6"],
 )
-async def test_no_server(addr, family):
+async def test_no_server(addr: _Address, family: socket.AddressFamily) -> None:
     with socket.socket(family, socket.SOCK_DGRAM) as sock:
         sock.bind(addr)
         free_addr = sock.getsockname()
 
     client = await asyncio_dgram.connect(free_addr[:2])
     await client.send(b"hi")
 
@@ -288,15 +315,15 @@
 
     assert client.peername == free_addr
     client.close()
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("addr", [("127.0.0.1", 0), ("::1", 0)], ids=["INET", "INET6"])
-async def test_echo(addr):
+async def test_echo(addr: _Address) -> None:
     server = await asyncio_dgram.bind(addr)
     client = await asyncio_dgram.connect(server.sockname[:2])
 
     await client.send(b"hi")
     data, client_addr = await server.recv()
     assert data == b"hi"
     assert client_addr == client.sockname
@@ -319,21 +346,26 @@
     [
         (("127.0.0.1", 0), socket.AF_INET),
         (("::1", 0), socket.AF_INET6),
         (None, socket.AF_UNIX),
     ],
     ids=["INET", "INET6", "UNIX"],
 )
-async def test_echo_bind(addr, family, tmp_path):
+async def test_echo_bind(
+    addr: typing.Optional[_Address],
+    family: socket.AddressFamily,
+    tmp_path: pathlib.Path,
+) -> None:
     if family == socket.AF_UNIX:
         if sys.version_info < (3, 7):
             pytest.skip()
         server = await asyncio_dgram.bind(tmp_path / "socket1")
         client = await asyncio_dgram.bind(tmp_path / "socket2")
     else:
+        assert addr is not None
         server = await asyncio_dgram.bind(addr)
         client = await asyncio_dgram.bind(addr)
 
     await client.send(b"hi", server.sockname)
     data, client_addr = await server.recv()
     assert data == b"hi"
     assert client_addr == client.sockname
@@ -348,15 +380,15 @@
 
     server.close()
     client.close()
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("addr", [("127.0.0.1", 0), ("::1", 0)], ids=["INET", "INET6"])
-async def test_unconnected_sender(addr):
+async def test_unconnected_sender(addr: _Address) -> None:
     # Bind two endpoints and connect to one.  Ensure that only the endpoint
     # that was connected to can send.
     ep1 = await asyncio_dgram.bind(addr)
     ep2 = await asyncio_dgram.bind(addr)
     connected = await asyncio_dgram.connect(ep1.sockname[:2])
 
     await ep1.send(b"from-ep1", connected.sockname)
@@ -370,15 +402,18 @@
 
     ep1.close()
     ep2.close()
     connected.close()
 
 
 @pytest.mark.asyncio
-async def test_protocol_pause_resume(monkeypatch, mock_socket, tmp_path):
+async def test_protocol_pause_resume(
+    monkeypatch: pytest.MonkeyPatch,
+    tmp_path: pathlib.Path,
+) -> None:
     # This is a little involved, but necessary to make sure that the Protocol
     # is correctly noticing when writing as been paused and resumed.  In
     # summary:
     #
     # - Mock the Protocol with one that sets the write buffer limits to 0 and
     # records when pause and resume writing are called.
     #
@@ -389,62 +424,65 @@
     # writing.
 
     class TestableProtocol(asyncio_dgram.aio.Protocol):
         pause_writing_called = 0
         resume_writing_called = 0
         instance = None
 
-        def __init__(self, *args, **kwds):
+        def __init__(self, *args, **kwds) -> None:  # type: ignore
             TestableProtocol.instance = self
             super().__init__(*args, **kwds)
 
-        def connection_made(self, transport):
+        def connection_made(self, transport: asyncio.BaseTransport) -> None:
+            assert isinstance(transport, asyncio.WriteTransport)
             transport.set_write_buffer_limits(low=0, high=0)
             super().connection_made(transport)
 
-        def pause_writing(self):
+        def pause_writing(self) -> None:
             self.pause_writing_called += 1
             super().pause_writing()
 
-        def resume_writing(self):
+        def resume_writing(self) -> None:
             self.resume_writing_called += 1
             super().resume_writing()
 
-    async def passthrough():
+    async def passthrough() -> None:
         """
         Used to mock the wait method on the asyncio.Event tracking if the write
         buffer is past the high water mark or not.  Given we're testing how
         that case is handled, we know it's safe locally to mock it.
         """
         pass
 
-    # Python 3.5 os.open doesn't like pathlib
-    cast = lambda x: x  # noqa: E731
-    if sys.version_info < (3, 6):
-        cast = lambda x: str(x)  # noqa: E731
+    mock_socket = unittest.mock.create_autospec(socket.socket)
+    mock_socket.family = socket.AF_INET
+    mock_socket.type = socket.SOCK_DGRAM
 
     with monkeypatch.context() as ctx:
         ctx.setattr(asyncio_dgram.aio, "Protocol", TestableProtocol)
 
         client = await asyncio_dgram.from_socket(mock_socket)
+        assert isinstance(client, asyncio_dgram.aio.DatagramClient)
+        assert TestableProtocol.instance is not None
+
         mock_socket.send.side_effect = BlockingIOError
         mock_socket.fileno.return_value = os.open(
-            cast(tmp_path / "socket"), os.O_RDONLY | os.O_CREAT
+            tmp_path / "socket", os.O_RDONLY | os.O_CREAT
         )
 
         with monkeypatch.context() as ctx2:
             ctx2.setattr(client._drained, "wait", passthrough)
             await client.send(b"foo")
 
         assert TestableProtocol.instance.pause_writing_called == 1
         assert TestableProtocol.instance.resume_writing_called == 0
         assert not TestableProtocol.instance._drained.is_set()
 
         mock_socket.send.side_effect = None
-        fd = os.open(cast(tmp_path / "socket"), os.O_WRONLY)
+        fd = os.open(tmp_path / "socket", os.O_WRONLY)
         os.write(fd, b"\n")
         os.close(fd)
 
         with monkeypatch.context() as ctx2:
             ctx2.setattr(client._drained, "wait", passthrough)
             await client.send(b"foo")
         await asyncio.sleep(0.1)
@@ -453,15 +491,15 @@
         assert TestableProtocol.instance.resume_writing_called == 1
         assert TestableProtocol.instance._drained.is_set()
 
         os.close(mock_socket.fileno.return_value)
 
 
 @pytest.mark.asyncio
-async def test_transport_closed():
+async def test_transport_closed() -> None:
     stream = await asyncio_dgram.bind(("127.0.0.1", 0))
 
     # Two tasks, both receiving.  This is a bit weird and we don't handle it at
     # this level on purpose.  The test is here to make that clear.  If having
     # multiple recv() calls racing against each other on a single event loop is
     # desired, one can wrap the DatagramStream with some sort of
     # dispatcher/adapter.
@@ -488,7 +526,29 @@
     # No recv after transport closed
     with pytest.raises(asyncio_dgram.TransportClosed):
         await stream.recv()
 
     # No send after transport closed
     with pytest.raises(asyncio_dgram.TransportClosed):
         await stream.send(b"junk", ("127.0.0.1", 0))
+
+
+@pytest.mark.asyncio
+async def test_bind_reuse_port() -> None:
+    async def use_socket(
+        addr: _Address, reuse_port: typing.Optional[bool] = None
+    ) -> None:
+        sock = await asyncio_dgram.bind(addr, reuse_port=reuse_port)
+        # give gather time to move to the other uses after the bind
+        await asyncio.sleep(0.1)
+        sock.close()
+
+    addr = ("127.0.0.1", 53001)
+    clients_count = 10
+    with pytest.raises(OSError, match="Address already in use"):
+        await asyncio.gather(*[use_socket(addr) for _ in range(clients_count)])
+
+    # We use another port in case the prev socket is still active (/ is still closing)
+    addr_2 = ("127.0.0.1", 53002)
+    await asyncio.gather(
+        *[use_socket(addr_2, reuse_port=True) for _ in range(clients_count)]
+    )
```


# Comparing `tmp/kaiju_scheduler-0.1.3-py3-none-any.whl.zip` & `tmp/kaiju_scheduler-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11404 bytes, number of entries: 11
--rw-r--r--  2.0 unx      273 b- defN 24-Apr-27 14:18 kaiju_scheduler/__init__.py
--rw-r--r--  2.0 unx      267 b- defN 24-Apr-27 14:18 kaiju_scheduler/interfaces.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-27 14:18 kaiju_scheduler/py.typed
--rw-r--r--  2.0 unx    10228 b- defN 24-Apr-27 14:18 kaiju_scheduler/scheduler.py
--rw-r--r--  2.0 unx    11381 b- defN 24-Apr-27 14:18 kaiju_scheduler/server.py
--rw-r--r--  2.0 unx     2733 b- defN 24-Apr-27 14:18 kaiju_scheduler/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5546 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      922 b- defN 24-Apr-27 14:18 kaiju_scheduler-0.1.3.dist-info/RECORD
-11 files, 32527 bytes uncompressed, 9834 bytes compressed:  69.8%
+Zip file size: 12231 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      273 b- defN 24-May-08 10:20 kaiju_scheduler/__init__.py
+-rw-r--r--  2.0 unx      291 b- defN 24-May-08 10:20 kaiju_scheduler/interfaces.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-08 10:20 kaiju_scheduler/py.typed
+-rw-r--r--  2.0 unx    10228 b- defN 24-May-08 10:20 kaiju_scheduler/scheduler.py
+-rw-r--r--  2.0 unx    18087 b- defN 24-May-08 10:20 kaiju_scheduler/server.py
+-rw-r--r--  2.0 unx     2733 b- defN 24-May-08 10:20 kaiju_scheduler/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-08 10:20 kaiju_scheduler-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5575 b- defN 24-May-08 10:20 kaiju_scheduler-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-08 10:20 kaiju_scheduler-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-08 10:20 kaiju_scheduler-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      922 b- defN 24-May-08 10:20 kaiju_scheduler-0.1.4.dist-info/RECORD
+11 files, 39286 bytes uncompressed, 10661 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: kaiju_scheduler/server.py
 Comment: 
 
 Filename: kaiju_scheduler/utils.py
 Comment: 
 
-Filename: kaiju_scheduler-0.1.3.dist-info/LICENSE
+Filename: kaiju_scheduler-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_scheduler-0.1.3.dist-info/METADATA
+Filename: kaiju_scheduler-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_scheduler-0.1.3.dist-info/WHEEL
+Filename: kaiju_scheduler-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_scheduler-0.1.3.dist-info/top_level.txt
+Filename: kaiju_scheduler-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_scheduler-0.1.3.dist-info/RECORD
+Filename: kaiju_scheduler-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_scheduler/__init__.py

```diff
@@ -3,8 +3,8 @@
 from kaiju_scheduler.scheduler import *
 from kaiju_scheduler.server import *
 from kaiju_scheduler.utils import *
 
 __python_version__ = "3.8"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

## kaiju_scheduler/interfaces.py

```diff
@@ -3,12 +3,12 @@
 from typing import Protocol
 
 __all__ = ["Logger"]
 
 
 class Logger(Protocol):
 
-    def error(self, msg, *args, **kwargs) -> None: ...
+    def error(self, msg: str, /, *args, **kwargs) -> None: ...
 
-    def info(self, msg, *args, **kwargs) -> None: ...
+    def info(self, msg: str, /, *args, **kwargs) -> None: ...
 
-    def debug(self, msg, *args, **kwargs) -> None: ...
+    def debug(self, msg: str, /, *args, **kwargs) -> None: ...
```

## kaiju_scheduler/server.py

```diff
@@ -1,21 +1,25 @@
 """Simple asyncio server implementation."""
 
 import asyncio
+from contextvars import ContextVar
 from dataclasses import dataclass, field
 from types import MappingProxyType
 from typing import Any, Awaitable, Callable, Collection, Iterable, Final, List, Mapping, Optional, Tuple
 
+from template_dict import Template
+
 from kaiju_scheduler.interfaces import Logger
 from kaiju_scheduler.utils import retry, timeout
 
 __all__ = ["Server", "Aborted", "ServerClosed"]
 
 _RequestBatch = Collection[Tuple[Callable[..., Awaitable], Iterable[Any], Mapping[str, Any]]]
 _Callback = Optional[Callable[..., Awaitable]]
+_Context = Optional[Mapping[str, Any]]
 
 
 class Aborted(RuntimeError):
     """The request was aborted by the server."""
 
 
 class ServerClosed(RuntimeError):
@@ -25,14 +29,16 @@
 @dataclass
 class Server:
     """Simple asyncio server for internal function calls.
 
     Provides a mechanism for request limiting, timeouts and retries.
     """
 
+    context: ContextVar[_Context] = ContextVar("Server", default=None)
+
     max_parallel_tasks: int = 256
     """Maximum number of parallel calls."""
 
     logger: Optional[Logger] = None
     """Optional logger instance."""
 
     full: bool = field(init=False, default=False)
@@ -57,14 +63,15 @@
         kws: Mapping[str, Any] = MappingProxyType({}),
         *,
         request_timeout_s: float = 300,
         callback: _Callback = None,
         retries: int = 0,
         retry_interval_s: float = 0,
         task_name: Optional[str] = None,
+        ctx: Optional[_Context] = None,
     ) -> asyncio.Task:
         """Create a new task and return immediately.
 
         .. note::
 
             The method is designed so the task doesn't raise errors. It returns them instead in its result and
             passes them to the callback function if it was provided.
@@ -74,39 +81,41 @@
         :param kws: Keyword arguments
         :param request_timeout_s: total max request time, the request will return `asyncio.TimeoutError`
             once the timeout is reached
         :param callback: The callback function which will be called with the result
         :param retries: How many times to retry the call
         :param retry_interval_s: How long to wait before retries
         :param task_name: custom asyncio task name
+        :param ctx: context variable with the context for this call
 
         :returns: an asyncio task wrapper around the request
         :raises asyncio.QueueFull: if the server is full, use :py:attr:`~kaiju_scheduler.server.Server.full` or
             :py:attr:`~kaiju_scheduler.server.Server.server_not_full` event to check before submitting a request
         :raises ServerClosed: if the server is closed and cannot accept a request
         """
         if self.closed:
             raise ServerClosed("Server is closed")
         if self.full:
             raise asyncio.QueueFull("Server is full")
         self._increment_counter()
         return asyncio.create_task(
-            self._call(func, args, kws, request_timeout_s, callback, retries, retry_interval_s), name=task_name
+            self._call(func, args, kws, request_timeout_s, callback, retries, retry_interval_s, ctx), name=task_name
         )
 
     def call_many_nowait(
         self,
         batch: _RequestBatch,
         *,
         request_timeout_s: float = 300,
         abort_batch_on_error: bool = False,
         callback: _Callback = None,
         retries: int = 0,
         retry_interval_s: float = 0,
         task_name: Optional[str] = None,
+        ctx: _Context = None,
     ) -> asyncio.Task:
         """Create a new task batch and return immediately.
 
         When batch will be called its requests will be executed in order which allows request chaining.
 
         .. note::
 
@@ -118,86 +127,186 @@
             will return `asyncio.TimeoutError`
         :param abort_batch_on_error: abort the whole batch on a first exception, all subsequent requests in the batch
             will return an :py:class:`~kaiju_scheduler.server.Server.Aborted` exceptions
         :param callback: The callback function which will be called with the result
         :param retries: How many times to retry the call
         :param retry_interval_s: How long to wait before retries
         :param task_name: custom asyncio task name
+        :param ctx: context variable with the context for this call
 
         :returns: an asyncio task wrapper around the request
         :raises asyncio.QueueFull: if the server is full, use :py:attr:`~kaiju_scheduler.server.Server.full` or
             :py:attr:`~kaiju_scheduler.server.Server.server_not_full` event to check before submitting a request
         :raises ServerClosed: if the server is closed and cannot accept a request
         """
         if self.closed:
             raise ServerClosed("Server is closed")
         if self.full:
             raise asyncio.QueueFull("Server is full")
         self._increment_counter()
         return asyncio.create_task(
-            self._call_many(batch, request_timeout_s, abort_batch_on_error, callback, retries, retry_interval_s),
+            self._call_many(batch, request_timeout_s, abort_batch_on_error, callback, retries, retry_interval_s, ctx),
             name=task_name,
         )
 
     async def call(
         self,
         func: Callable[..., Awaitable],
         args: Iterable[Any] = tuple(),
         kws: Mapping[str, Any] = MappingProxyType({}),
         *,
         request_timeout_s: float = 300,
         callback: _Callback = None,
         retries: int = 0,
         retry_interval_s: float = 0,
         task_name: Optional[str] = None,
+        ctx: _Context = None,
     ) -> asyncio.Task:
         """Same as :py:meth:`~kaiju_scheduler.server.Server.call_nowait` but would wait for the server counter
         instead of raising a `asyncio.QueueFull` error."""
         if self.closed:
             raise ServerClosed("Server is closed")
         if self.full:
             await self.server_not_full.wait()
         self._increment_counter()
         return asyncio.create_task(
-            self._call(func, args, kws, request_timeout_s, callback, retries, retry_interval_s), name=task_name
+            self._call(func, args, kws, request_timeout_s, callback, retries, retry_interval_s, ctx), name=task_name
         )
 
     async def call_many(
         self,
         batch: _RequestBatch,
         *,
         request_timeout_s: float = 300,
         abort_batch_on_error: bool = False,
         callback: _Callback = None,
         retries: int = 0,
         retry_interval_s: float = 0,
         task_name: Optional[str] = None,
+        ctx: _Context = None,
     ) -> asyncio.Task:
         """Same as :py:meth:`~kaiju_scheduler.server.Server.call_many_nowait` but would wait for the server counter
         instead of raising a `asyncio.QueueFull` error."""
         if self.closed:
             raise ServerClosed("Server is closed")
         if self.full:
             await self.server_not_full.wait()
         self._increment_counter()
         return asyncio.create_task(
-            self._call_many(batch, request_timeout_s, abort_batch_on_error, callback, retries, retry_interval_s),
+            self._call_many(batch, request_timeout_s, abort_batch_on_error, callback, retries, retry_interval_s, ctx),
+            name=task_name,
+        )
+
+    def call_template_nowait(
+        self,
+        batch: _RequestBatch,
+        *,
+        request_timeout_s: float = 300,
+        callback: _Callback = None,
+        retries: int = 0,
+        retry_interval_s: float = 0,
+        task_name: Optional[str] = None,
+        env: dict = None,
+        ctx: _Context = None,
+    ) -> asyncio.Task:
+        """Create a new task batch with templates and return immediately.
+
+        When batch will be called its requests will be executed in order which allows request chaining.
+
+        The difference from :py:meth:`~kaiju_scheduler.server.Server.call_many_nowait` is that this method executes
+        requests inside a template engine. This means you can pass results between requests before returning
+        the results.
+
+        For example, you have a method what returns a list of users and another which requires a list of user ids
+        to send notifications. With the `template syntax <https://template-dict.readthedocs.io/guide.html>`_
+        you ask the server to pass the results from the first method to the next one
+        using `[result.<request_id>.*]` placeholder. Request ids always start from zero.
+
+        .. code-block:: python
+
+            server.call_template_nowait([
+                (get_users, [], {'where': {'blocked': '[env.user_condition]'}}),
+                (notify_users, [], {'user_ids': '[result.0.id]'}),
+            ], env={'user_condition': {'blocked': True}})
+
+        This method is a bit slower than :py:meth:`~kaiju_scheduler.server.Server.call_many_nowait` for obvious
+        reasons. Use the other one if you don't need templates.
+
+        .. note::
+
+            The method is designed so the task doesn't raise errors. It returns them instead in its result and
+            passes them to the callback function if it was provided.
+
+        :param batch: batch of requests i.e. a collection of (func, args, kws) tuples
+        :param request_timeout_s: total max request time for the whole batch, each request in a batch after the timeout
+            will return `asyncio.TimeoutError`
+        :param callback: The callback function which will be called with the result
+        :param retries: How many times to retry the call
+        :param retry_interval_s: How long to wait before retries
+        :param task_name: custom asyncio task name
+        :param env: shared environment variables between requests, accessible with `[env.*]` template placeholder
+        :param ctx: context variable with context for this request
+
+        :returns: an asyncio task wrapper around the request
+        :raises asyncio.QueueFull: if the server is full, use :py:attr:`~kaiju_scheduler.server.Server.full` or
+            :py:attr:`~kaiju_scheduler.server.Server.server_not_full` event to check before submitting a request
+        :raises ServerClosed: if the server is closed and cannot accept a request
+        """
+        if self.closed:
+            raise ServerClosed("Server is closed")
+        if self.full:
+            raise asyncio.QueueFull("Server is full")
+        self._increment_counter()
+        if env is None:
+            env = {}
+        self._increment_counter()
+        return asyncio.create_task(
+            self._call_template(batch, request_timeout_s, callback, retries, retry_interval_s, env, ctx),
+            name=task_name,
+        )
+
+    async def call_template(
+        self,
+        batch: _RequestBatch,
+        *,
+        request_timeout_s: float = 300,
+        callback: _Callback = None,
+        retries: int = 0,
+        retry_interval_s: float = 0,
+        task_name: Optional[str] = None,
+        env: dict = None,
+        ctx: _Context = None,
+    ) -> asyncio.Task:
+        """Same as :py:meth:`~kaiju_scheduler.server.Server.call_template_nowait` but would wait for the server counter
+        instead of raising a `asyncio.QueueFull` error."""
+        if self.closed:
+            raise ServerClosed("Server is closed")
+        if self.full:
+            await self.server_not_full.wait()
+        if env is None:
+            env = {}
+        self._increment_counter()
+        return asyncio.create_task(
+            self._call_template(batch, request_timeout_s, callback, retries, retry_interval_s, env, ctx),
             name=task_name,
         )
 
     async def _call(
         self,
         func: Callable[..., Awaitable],
         args: Iterable[Any],
         kws: Mapping[str, Any],
         request_timeout_s: float,
         callback: _Callback,
         retries: int,
         retry_interval_s: float,
+        ctx: _Context,
     ) -> Any:
+        if ctx:
+            self.context.set(ctx)
         result = None
         try:
             async with timeout(request_timeout_s):
                 if retries:
                     result = await retry(
                         func,
                         args=args,
@@ -216,20 +325,23 @@
             if callback is not None:
                 await callback(result)
         return result
 
     async def _call_many(
         self,
         batch: _RequestBatch,
-        request_timeout_s: float = 300,
-        abort_batch_on_error: bool = False,
-        callback: _Callback = None,
-        retries: int = 0,
-        retry_interval_s: float = 0,
+        request_timeout_s,
+        abort_batch_on_error: bool,
+        callback: _Callback,
+        retries: int,
+        retry_interval_s: float,
+        ctx: _Context,
     ) -> List[Any]:
+        if ctx:
+            self.context.set(ctx)
         n, results = 0, []
         try:
             async with timeout(request_timeout_s):
                 for n, (func, args, kws) in enumerate(batch):
                     try:
                         if retries:
                             result = await retry(
@@ -252,14 +364,61 @@
         except asyncio.TimeoutError:
             results.extend([asyncio.TimeoutError("Timeout")] * (len(batch) - n))
         except asyncio.CancelledError:
             results.extend([Aborted("Request aborted")] * (len(batch) - n))
         finally:
             self._decrement_counter()
             if callback is not None:
+                await callback(results)
+        return results
+
+    async def _call_template(
+        self,
+        batch: _RequestBatch,
+        request_timeout_s: float,
+        callback: _Callback,
+        retries: int,
+        retry_interval_s: float,
+        env: dict,
+        ctx: _Context,
+    ) -> List[Any]:
+        if ctx:
+            self.context.set(ctx)
+        n, results = 0, []
+        template_env = {"env": env, "result": {}}
+        try:
+            async with timeout(request_timeout_s):
+                for n, (func, args, kws) in enumerate(batch):
+                    try:
+                        kws = Template(kws).eval(template_env)
+                        if retries:
+                            result = await retry(
+                                func,
+                                args=args,
+                                kws=kws,
+                                retries=retries,
+                                interval_s=retry_interval_s,
+                                timeout_s=request_timeout_s,
+                                logger=self.logger,
+                            )
+                        else:
+                            result = await func(*args, **kws)
+                        results.append(result)
+                        template_env["result"][str(n)] = result
+                    except Exception as exc:
+                        results.append(exc)
+                        results.extend([Aborted("Request aborted")] * (len(batch) - n - 1))
+                        break
+        except asyncio.TimeoutError:
+            results.extend([asyncio.TimeoutError("Timeout")] * (len(batch) - n))
+        except asyncio.CancelledError:
+            results.extend([Aborted("Request aborted")] * (len(batch) - n))
+        finally:
+            self._decrement_counter()
+            if callback is not None:
                 await callback(results)
         return results
 
     async def start(self):
         self._reset_counter()
         self.closed = False
```

## Comparing `kaiju_scheduler-0.1.3.dist-info/LICENSE` & `kaiju_scheduler-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_scheduler-0.1.3.dist-info/METADATA` & `kaiju_scheduler-0.1.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-scheduler
-Version: 0.1.3
+Version: 0.1.4
 Summary: Asynchronous tasks scheduler and executor
 Home-page: https://github.com/violet-black/kaiju-scheduler
 Author: violetblackdev@gmail.com
 License: MIT
 Keywords: scheduler,asyncio,tasks
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: template-dict
 Provides-Extra: dev
 Requires-Dist: pip-tools ; extra == 'dev'
 Requires-Dist: tox ; extra == 'dev'
 Requires-Dist: coverage ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
```


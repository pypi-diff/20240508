# Comparing `tmp/aio-celery-0.9.1.tar.gz` & `tmp/aio-celery-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-celery-0.9.1.tar", last modified: Tue Feb 13 13:07:51 2024, max compression
+gzip compressed data, was "aio-celery-0.9.2.tar", last modified: Wed Feb 21 06:50:22 2024, max compression
```

## Comparing `aio-celery-0.9.1.tar` & `aio-celery-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 owl        (502) staff       (20)        0 2024-02-13 13:07:51.001021 aio-celery-0.9.1/
--rw-r--r--   0 owl        (502) staff       (20)     9333 2024-02-13 13:07:51.000897 aio-celery-0.9.1/PKG-INFO
--rw-r--r--   0 owl        (502) staff       (20)     8082 2024-02-10 10:19:14.000000 aio-celery-0.9.1/README.md
-drwxr-xr-x   0 owl        (502) staff       (20)        0 2024-02-13 13:07:50.999499 aio-celery-0.9.1/aio_celery/
--rw-r--r--   0 owl        (502) staff       (20)      143 2024-02-13 13:07:35.000000 aio-celery-0.9.1/aio_celery/__init__.py
--rw-r--r--   0 owl        (502) staff       (20)     2467 2024-01-17 10:46:01.000000 aio-celery-0.9.1/aio_celery/__main__.py
--rw-r--r--   0 owl        (502) staff       (20)     2040 2023-11-06 09:35:42.000000 aio-celery-0.9.1/aio_celery/amqp.py
--rw-r--r--   0 owl        (502) staff       (20)     1590 2024-02-13 10:18:44.000000 aio-celery-0.9.1/aio_celery/annotated_task.py
--rw-r--r--   0 owl        (502) staff       (20)     7168 2024-02-13 10:18:44.000000 aio-celery-0.9.1/aio_celery/app.py
--rw-r--r--   0 owl        (502) staff       (20)      967 2023-11-05 17:48:48.000000 aio-celery-0.9.1/aio_celery/backend.py
--rw-r--r--   0 owl        (502) staff       (20)     1654 2023-11-23 16:12:53.000000 aio-celery-0.9.1/aio_celery/broker.py
--rw-r--r--   0 owl        (502) staff       (20)     1091 2023-11-23 16:40:41.000000 aio-celery-0.9.1/aio_celery/config.py
--rw-r--r--   0 owl        (502) staff       (20)      313 2023-11-05 17:59:49.000000 aio-celery-0.9.1/aio_celery/context.py
--rw-r--r--   0 owl        (502) staff       (20)      722 2023-11-05 17:48:48.000000 aio-celery-0.9.1/aio_celery/exceptions.py
--rw-r--r--   0 owl        (502) staff       (20)     2457 2023-11-06 15:18:05.000000 aio-celery-0.9.1/aio_celery/request.py
--rw-r--r--   0 owl        (502) staff       (20)     1793 2023-11-05 18:17:52.000000 aio-celery-0.9.1/aio_celery/result.py
--rw-r--r--   0 owl        (502) staff       (20)     3333 2024-02-13 10:13:12.000000 aio-celery-0.9.1/aio_celery/task.py
--rw-r--r--   0 owl        (502) staff       (20)      193 2023-11-05 17:35:30.000000 aio-celery-0.9.1/aio_celery/utils.py
--rw-r--r--   0 owl        (502) staff       (20)    11270 2024-02-13 10:18:44.000000 aio-celery-0.9.1/aio_celery/worker.py
-drwxr-xr-x   0 owl        (502) staff       (20)        0 2024-02-13 13:07:51.000532 aio-celery-0.9.1/aio_celery.egg-info/
--rw-r--r--   0 owl        (502) staff       (20)     9333 2024-02-13 13:07:50.000000 aio-celery-0.9.1/aio_celery.egg-info/PKG-INFO
--rw-r--r--   0 owl        (502) staff       (20)      566 2024-02-13 13:07:50.000000 aio-celery-0.9.1/aio_celery.egg-info/SOURCES.txt
--rw-r--r--   0 owl        (502) staff       (20)        1 2024-02-13 13:07:50.000000 aio-celery-0.9.1/aio_celery.egg-info/dependency_links.txt
--rw-r--r--   0 owl        (502) staff       (20)       56 2024-02-13 13:07:50.000000 aio-celery-0.9.1/aio_celery.egg-info/entry_points.txt
--rw-r--r--   0 owl        (502) staff       (20)       38 2024-02-13 13:07:50.000000 aio-celery-0.9.1/aio_celery.egg-info/requires.txt
--rw-r--r--   0 owl        (502) staff       (20)       11 2024-02-13 13:07:50.000000 aio-celery-0.9.1/aio_celery.egg-info/top_level.txt
--rw-r--r--   0 owl        (502) staff       (20)      351 2024-02-10 10:00:35.000000 aio-celery-0.9.1/pyproject.toml
--rw-r--r--   0 owl        (502) staff       (20)     1332 2024-02-13 13:07:51.001543 aio-celery-0.9.1/setup.cfg
+drwxr-xr-x   0 owl        (502) staff       (20)        0 2024-02-21 06:50:22.530418 aio-celery-0.9.2/
+-rw-r--r--   0 owl        (502) staff       (20)     9333 2024-02-21 06:50:22.530330 aio-celery-0.9.2/PKG-INFO
+-rw-r--r--   0 owl        (502) staff       (20)     8082 2024-02-10 10:19:14.000000 aio-celery-0.9.2/README.md
+drwxr-xr-x   0 owl        (502) staff       (20)        0 2024-02-21 06:50:22.528985 aio-celery-0.9.2/aio_celery/
+-rw-r--r--   0 owl        (502) staff       (20)      143 2024-02-21 06:49:56.000000 aio-celery-0.9.2/aio_celery/__init__.py
+-rw-r--r--   0 owl        (502) staff       (20)     2467 2024-01-17 10:46:01.000000 aio-celery-0.9.2/aio_celery/__main__.py
+-rw-r--r--   0 owl        (502) staff       (20)     2040 2023-11-06 09:35:42.000000 aio-celery-0.9.2/aio_celery/amqp.py
+-rw-r--r--   0 owl        (502) staff       (20)     1582 2024-02-13 16:17:07.000000 aio-celery-0.9.2/aio_celery/annotated_task.py
+-rw-r--r--   0 owl        (502) staff       (20)     7327 2024-02-13 16:25:40.000000 aio-celery-0.9.2/aio_celery/app.py
+-rw-r--r--   0 owl        (502) staff       (20)      967 2023-11-05 17:48:48.000000 aio-celery-0.9.2/aio_celery/backend.py
+-rw-r--r--   0 owl        (502) staff       (20)     1654 2023-11-23 16:12:53.000000 aio-celery-0.9.2/aio_celery/broker.py
+-rw-r--r--   0 owl        (502) staff       (20)     1091 2023-11-23 16:40:41.000000 aio-celery-0.9.2/aio_celery/config.py
+-rw-r--r--   0 owl        (502) staff       (20)      313 2023-11-05 17:59:49.000000 aio-celery-0.9.2/aio_celery/context.py
+-rw-r--r--   0 owl        (502) staff       (20)      722 2023-11-05 17:48:48.000000 aio-celery-0.9.2/aio_celery/exceptions.py
+-rw-r--r--   0 owl        (502) staff       (20)     2443 2024-02-21 06:44:42.000000 aio-celery-0.9.2/aio_celery/request.py
+-rw-r--r--   0 owl        (502) staff       (20)     1793 2023-11-05 18:17:52.000000 aio-celery-0.9.2/aio_celery/result.py
+-rw-r--r--   0 owl        (502) staff       (20)     3334 2024-02-21 06:48:56.000000 aio-celery-0.9.2/aio_celery/task.py
+-rw-r--r--   0 owl        (502) staff       (20)      193 2023-11-05 17:35:30.000000 aio-celery-0.9.2/aio_celery/utils.py
+-rw-r--r--   0 owl        (502) staff       (20)    11287 2024-02-13 13:17:20.000000 aio-celery-0.9.2/aio_celery/worker.py
+drwxr-xr-x   0 owl        (502) staff       (20)        0 2024-02-21 06:50:22.529998 aio-celery-0.9.2/aio_celery.egg-info/
+-rw-r--r--   0 owl        (502) staff       (20)     9333 2024-02-21 06:50:22.000000 aio-celery-0.9.2/aio_celery.egg-info/PKG-INFO
+-rw-r--r--   0 owl        (502) staff       (20)      566 2024-02-21 06:50:22.000000 aio-celery-0.9.2/aio_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 owl        (502) staff       (20)        1 2024-02-21 06:50:22.000000 aio-celery-0.9.2/aio_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 owl        (502) staff       (20)       56 2024-02-21 06:50:22.000000 aio-celery-0.9.2/aio_celery.egg-info/entry_points.txt
+-rw-r--r--   0 owl        (502) staff       (20)       38 2024-02-21 06:50:22.000000 aio-celery-0.9.2/aio_celery.egg-info/requires.txt
+-rw-r--r--   0 owl        (502) staff       (20)       11 2024-02-21 06:50:22.000000 aio-celery-0.9.2/aio_celery.egg-info/top_level.txt
+-rw-r--r--   0 owl        (502) staff       (20)      382 2024-02-21 06:46:17.000000 aio-celery-0.9.2/pyproject.toml
+-rw-r--r--   0 owl        (502) staff       (20)     1332 2024-02-21 06:50:22.530672 aio-celery-0.9.2/setup.cfg
```

### Comparing `aio-celery-0.9.1/PKG-INFO` & `aio-celery-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-celery
-Version: 0.9.1
+Version: 0.9.2
 Summary: Celery worker for running asyncio coroutine tasks
 Home-page: https://github.com/earlgreyness/aio-celery
 Author: Kirill Kondratenko
 Author-email: earlgreatness@gmail.com
 Keywords: asyncio,celery
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `aio-celery-0.9.1/README.md` & `aio-celery-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `aio-celery-0.9.1/aio_celery/__main__.py` & `aio-celery-0.9.2/aio_celery/__main__.py`

 * *Files identical despite different names*

### Comparing `aio-celery-0.9.1/aio_celery/amqp.py` & `aio-celery-0.9.2/aio_celery/amqp.py`

 * *Files identical despite different names*

### Comparing `aio-celery-0.9.1/aio_celery/annotated_task.py` & `aio-celery-0.9.2/aio_celery/annotated_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from .utils import first_not_null
 
 if TYPE_CHECKING:
     from .app import Celery
     from .result import AsyncResult
 
 
-@dataclass(frozen=True)
+@dataclass
 class AnnotatedTask:
     fn: Callable[..., Awaitable[Any]]
     bind: bool
     ignore_result: bool | None
     max_retries: int | None
     default_retry_delay: int
-    autoretry_for: tuple[type[Exception]]
+    autoretry_for: tuple[type[Exception], ...]
     app: Celery
     name: str
     queue: str | None
     priority: int | None
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         if self.bind:
```

### Comparing `aio-celery-0.9.1/aio_celery/app.py` & `aio-celery-0.9.2/aio_celery/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
-import dataclasses
 import logging
 import sys
 import uuid
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
+    Optional,
 )
 
 import aio_pika
 
 from .amqp import create_task_message
 from .annotated_task import AnnotatedTask
 from .backend import create_redis_connection_pool
@@ -28,27 +28,31 @@
 if TYPE_CHECKING:
     import redis.asyncio
 
 logger = logging.getLogger(__name__)
 
 
 class Celery:
-    def __init__(self) -> None:
+    def __init__(self, name: Optional[str] = None) -> None:
+        self.name = name
         self.conf = DefaultConfig()
         self._tasks_registry: dict[str, AnnotatedTask] = {}
         self._app_context: Any = None
         self._result_backend_connection_pool: (
             redis.asyncio.BlockingConnectionPool | None
         ) = None
         self._broker: Broker | None = None
         self._setup_app_context: Callable[
             [],
             contextlib.AbstractAsyncContextManager[Any],
         ] = _setup_nothing
 
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__} {self.name} at {hex(id(self))}>"
+
     def define_app_context(
         self,
         fn: Callable[[], contextlib.AbstractAsyncContextManager[Any]],
     ) -> None:
         self._setup_app_context = fn
 
     @property
@@ -103,15 +107,15 @@
         self,
         *args: Callable[..., Awaitable[Any]],
         bind: bool = False,
         name: str | None = None,
         ignore_result: bool | None = None,
         max_retries: int | None = 3,
         default_retry_delay: int = 180,
-        autoretry_for: tuple[type[Exception]] = (),
+        autoretry_for: tuple[type[Exception], ...] = (),
         queue: str | None = None,
         priority: int | None = None,
     ) -> AnnotatedTask | Callable[[Callable[..., Awaitable[Any]]], AnnotatedTask]:
         """Create a task class out of any callable."""
 
         def decorator(fn: Callable[..., Awaitable[Any]]) -> AnnotatedTask:
             if name is None:
@@ -146,15 +150,16 @@
             return decorator(func)
         msg = "@task() takes exactly 1 argument"
         raise TypeError(msg)
 
     def _construct_extended_task_registry(self) -> dict[str, AnnotatedTask]:
         registry: dict[str, AnnotatedTask] = {}
         for name, task in _SHARED_APP._tasks_registry.items():  # noqa: SLF001
-            registry[name] = dataclasses.replace(task, app=self)
+            task.app = self
+            registry[name] = task
         registry.update(self._tasks_registry)
         return registry
 
     def get_annotated_task(self, task_name: str) -> AnnotatedTask:
         return self._construct_extended_task_registry()[task_name]
 
     def list_registered_task_names(self) -> list[str]:
```

### Comparing `aio-celery-0.9.1/aio_celery/backend.py` & `aio-celery-0.9.2/aio_celery/backend.py`

 * *Files identical despite different names*

### Comparing `aio-celery-0.9.1/aio_celery/broker.py` & `aio-celery-0.9.2/aio_celery/broker.py`

 * *Files identical despite different names*

### Comparing `aio-celery-0.9.1/aio_celery/config.py` & `aio-celery-0.9.2/aio_celery/config.py`

 * *Files identical despite different names*

### Comparing `aio-celery-0.9.1/aio_celery/exceptions.py` & `aio-celery-0.9.2/aio_celery/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio-celery-0.9.1/aio_celery/request.py` & `aio-celery-0.9.2/aio_celery/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from aio_pika import IncomingMessage, Message
 
 
 @dataclass(frozen=True)
 class Request:
     message: IncomingMessage
 
-    id: str  # noqa: A003
+    id: str
     task: str
     args: tuple[Any, ...]
     kwargs: dict[str, Any]
     retries: int
     eta: datetime.datetime | None
     parent_id: str | None
     group: str | None
```

### Comparing `aio-celery-0.9.1/aio_celery/result.py` & `aio-celery-0.9.2/aio_celery/result.py`

 * *Files identical despite different names*

### Comparing `aio-celery-0.9.1/aio_celery/task.py` & `aio-celery-0.9.2/aio_celery/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,17 +51,17 @@
             "result": meta,
             "traceback": None,
             "children": [],
             "date_done": None,
             "task_id": self.request.id,
         }
         if _finalize:
-            payload["date_done"] = (
-                datetime.datetime.utcnow().isoformat()  # noqa: DTZ003
-            )
+            payload["date_done"] = datetime.datetime.now(
+                datetime.timezone.utc,
+            ).isoformat()
         if self.request.group is not None:
             payload["group_id"] = self.request.group
         if self.request.parent_id is not None:
             payload["parent_id"] = self.request.parent_id
         await result_backend.set(
             f"celery-task-meta-{self.request.id}",
             json.dumps(payload).encode(),
```

### Comparing `aio-celery-0.9.1/aio_celery/worker.py` & `aio-celery-0.9.2/aio_celery/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         raise MaxRetriesExceededError(msg)
     await app.broker.publish_message(
         exc.message,
         routing_key=(message.routing_key or app.conf.task_default_queue),
     )
 
 
-async def on_message_received(
+async def on_message_received(  # noqa: PLR0915
     message: IncomingMessage,
     *,
     app: Celery,
     semaphore: asyncio.Semaphore,
 ) -> None:
     task_id: str | None = None
     task_name: str | None = None
```

### Comparing `aio-celery-0.9.1/aio_celery.egg-info/PKG-INFO` & `aio-celery-0.9.2/aio_celery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-celery
-Version: 0.9.1
+Version: 0.9.2
 Summary: Celery worker for running asyncio coroutine tasks
 Home-page: https://github.com/earlgreyness/aio-celery
 Author: Kirill Kondratenko
 Author-email: earlgreatness@gmail.com
 Keywords: asyncio,celery
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `aio-celery-0.9.1/aio_celery.egg-info/SOURCES.txt` & `aio-celery-0.9.2/aio_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio-celery-0.9.1/setup.cfg` & `aio-celery-0.9.2/setup.cfg`

 * *Files identical despite different names*


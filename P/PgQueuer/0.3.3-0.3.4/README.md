# Comparing `tmp/pgqueuer-0.3.3.tar.gz` & `tmp/pgqueuer-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgqueuer-0.3.3.tar", last modified: Sun May  5 13:49:03 2024, max compression
+gzip compressed data, was "pgqueuer-0.3.4.tar", last modified: Wed May  8 07:44:15 2024, max compression
```

## Comparing `pgqueuer-0.3.3.tar` & `pgqueuer-0.3.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:49:03.984204 pgqueuer-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:49:03.972204 pgqueuer-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:49:03.976204 pgqueuer-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-05 13:49:03.980204 pgqueuer-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 13:49:03.984204 pgqueuer-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:49:03.976204 pgqueuer-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:49:03.980204 pgqueuer-0.3.3/src/PgQueuer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/qm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16206 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/src/PgQueuer/tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:49:03.980204 pgqueuer-0.3.3/src/PgQueuer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-05 13:49:03.000000 pgqueuer-0.3.3/src/PgQueuer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-05 13:49:03.000000 pgqueuer-0.3.3/src/PgQueuer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 13:49:03.000000 pgqueuer-0.3.3/src/PgQueuer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-05 13:49:03.000000 pgqueuer-0.3.3/src/PgQueuer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 13:49:03.000000 pgqueuer-0.3.3/src/PgQueuer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 13:49:03.000000 pgqueuer-0.3.3/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:49:03.980204 pgqueuer-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:49:03.980204 pgqueuer-0.3.3/test/db/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/test/db/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/test/db/init_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/test/test_qm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/test/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/test/test_tm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:49:03.980204 pgqueuer-0.3.3/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-05 13:48:55.000000 pgqueuer-0.3.3/tools/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.798206 pgqueuer-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.786206 pgqueuer-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.790207 pgqueuer-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:44:15.798206 pgqueuer-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.790207 pgqueuer-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/src/PgQueuer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/src/PgQueuer/tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/src/PgQueuer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/PgQueuer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 07:44:15.000000 pgqueuer-0.3.4/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/test/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/db/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/db/init_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/test_qm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/test/test_tm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:44:15.794206 pgqueuer-0.3.4/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-08 07:44:07.000000 pgqueuer-0.3.4/tools/benchmark.py
```

### Comparing `pgqueuer-0.3.3/.github/workflows/ci.yml` & `pgqueuer-0.3.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/.github/workflows/linting.yml` & `pgqueuer-0.3.4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/.github/workflows/release.yml` & `pgqueuer-0.3.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/.gitignore` & `pgqueuer-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/LICENSE` & `pgqueuer-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/pyproject.toml` & `pgqueuer-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/src/PgQueuer/cli.py` & `pgqueuer-0.3.4/src/PgQueuer/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import argparse
 import asyncio
 import os
 from datetime import timedelta
 
 import asyncpg
 from tabulate import tabulate, tabulate_formats
@@ -36,25 +38,24 @@
                 "Priority",
             ],
             tablefmt=tablefmt,
         )
     )
 
 
-async def fetch_and_dispay(
+async def fetch_and_display(
     queries: Queries,
     interval: timedelta | None,
     tail: int,
     tablefmt: str,
 ) -> None:
     clear_and_home = "\033[2J\033[H"
     while True:
         print(clear_and_home, end="")
-        stats = await queries.log_statistics(tail)  # Fetch stats once and reuse
-        await display_stats(stats, tablefmt)
+        await display_stats(await queries.log_statistics(tail), tablefmt)
         if interval is None:
             return
         await asyncio.sleep(interval.total_seconds())
 
 
 def cliparser() -> argparse.Namespace:
     common_arguments = argparse.ArgumentParser(
@@ -223,13 +224,13 @@
                 if not parsed.dry_run:
                     await queries.install()
             case "uninstall":
                 print(QueryBuilder().create_uninstall_query())
                 if not parsed.dry_run:
                     await queries.uninstall()
             case "dashboard":
-                await fetch_and_dispay(
+                await fetch_and_display(
                     queries,
                     parsed.interval,
                     parsed.tail,
                     parsed.table_format,
                 )
```

### Comparing `pgqueuer-0.3.3/src/PgQueuer/models.py` & `pgqueuer-0.3.4/src/PgQueuer/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from datetime import timedelta
 from typing import Literal
 
 from pydantic import AwareDatetime, BaseModel
 
 STATUS = Literal[
     "queued",
```

### Comparing `pgqueuer-0.3.3/src/PgQueuer/qm.py` & `pgqueuer-0.3.4/src/PgQueuer/qm.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,19 +111,19 @@
         dequeue_timeout: timedelta = timedelta(seconds=30),
     ) -> None:
         """
         Continuously listens for events and dispatches jobs. Manages connections and
         tasks, logs timeouts, and resets connections upon termination.
         """
         async with (
-            self.pool.acquire() as conn,
+            self.pool.acquire() as connection,
             TaskManager() as tm,
         ):
             listener = PGEventQueue()
-            await listener.connect(conn, self.channel)
+            await listener.connect(connection, self.channel)
 
             while self.alive:
                 while self.alive and (job := await self.queries.dequeue()):
                     tm.add(asyncio.create_task(self._dispatch(job)))
 
                 try:
                     await asyncio.wait_for(
@@ -132,16 +132,16 @@
                     )
                 except asyncio.TimeoutError:
                     logger.debug(
                         "Timeout after %r without receiving an event.",
                         dequeue_timeout,
                     )
 
-            conn.remove_termination_listener(_critical_termination_listener)
-            await conn.reset()
+            connection.remove_termination_listener(_critical_termination_listener)
+            await connection.reset()
 
     async def _dispatch(self, job: Job) -> None:
         """
         Handles asynchronous job dispatch. Logs exceptions, updates job status,
         and adapts execution method based on whether the job's function is asynchronous.
         """
```

### Comparing `pgqueuer-0.3.3/src/PgQueuer/queries.py` & `pgqueuer-0.3.4/src/PgQueuer/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import dataclasses
 import os
 from typing import Final
 
 import asyncpg
 
 from . import models
```

### Comparing `pgqueuer-0.3.3/src/PgQueuer/tm.py` & `pgqueuer-0.3.4/src/PgQueuer/tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/src/PgQueuer.egg-info/SOURCES.txt` & `pgqueuer-0.3.4/src/PgQueuer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+CONTRIBUTING.md
 LICENSE
 README.md
 docker-compose.yml
 pyproject.toml
 .github/workflows/ci.yml
 .github/workflows/linting.yml
 .github/workflows/release.yml
```

### Comparing `pgqueuer-0.3.3/test/conftest.py` & `pgqueuer-0.3.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/test/db/Dockerfile` & `pgqueuer-0.3.4/test/db/Dockerfile`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/test/test_qm.py` & `pgqueuer-0.3.4/test/test_qm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/test/test_queries.py` & `pgqueuer-0.3.4/test/test_queries.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/test/test_tm.py` & `pgqueuer-0.3.4/test/test_tm.py`

 * *Files identical despite different names*

### Comparing `pgqueuer-0.3.3/tools/benchmark.py` & `pgqueuer-0.3.4/tools/benchmark.py`

 * *Files identical despite different names*


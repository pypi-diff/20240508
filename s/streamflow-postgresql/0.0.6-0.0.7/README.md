# Comparing `tmp/streamflow-postgresql-0.0.6.tar.gz` & `tmp/streamflow_postgresql-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamflow-postgresql-0.0.6.tar", last modified: Tue Sep 12 08:59:34 2023, max compression
+gzip compressed data, was "streamflow_postgresql-0.0.7.tar", last modified: Wed May  8 15:39:25 2024, max compression
```

## Comparing `streamflow-postgresql-0.0.6.tar` & `streamflow_postgresql-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 08:59:34.475479 streamflow-postgresql-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2023-09-12 08:59:34.475479 streamflow-postgresql-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/bandit-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 08:59:34.475479 streamflow-postgresql-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 08:59:34.475479 streamflow-postgresql-0.0.6/streamflow_postgresql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/streamflow_postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20985 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/streamflow_postgresql/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/streamflow_postgresql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 08:59:34.475479 streamflow-postgresql-0.0.6/streamflow_postgresql/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/streamflow_postgresql/schemas/postgresql.json
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/streamflow_postgresql/schemas/postgresql.sql
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/streamflow_postgresql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 08:59:34.475479 streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2023-09-12 08:59:34.000000 streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-09-12 08:59:34.000000 streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 08:59:34.000000 streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-09-12 08:59:34.000000 streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-09-12 08:59:34.000000 streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-12 08:59:34.000000 streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 08:59:34.000000 streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 08:59:34.475479 streamflow-postgresql-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2023-09-12 08:59:24.000000 streamflow-postgresql-0.0.6/tests/test_persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:25.138555 streamflow_postgresql-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-08 15:39:25.134555 streamflow_postgresql-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/bandit-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:39:25.138555 streamflow_postgresql-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:25.134555 streamflow_postgresql-0.0.7/streamflow_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/streamflow_postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23917 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/streamflow_postgresql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/streamflow_postgresql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:25.134555 streamflow_postgresql-0.0.7/streamflow_postgresql/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/streamflow_postgresql/schemas/postgresql.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/streamflow_postgresql/schemas/postgresql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/streamflow_postgresql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:25.134555 streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-08 15:39:25.000000 streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 15:39:25.000000 streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:39:25.000000 streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:39:25.000000 streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 15:39:25.000000 streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 15:39:25.000000 streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:39:24.000000 streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:39:25.134555 streamflow_postgresql-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/tests/test_cwl_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10963 2024-05-08 15:39:20.000000 streamflow_postgresql-0.0.7/tests/test_persistence.py
```

### Comparing `streamflow-postgresql-0.0.6/LICENSE` & `streamflow_postgresql-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.6/PKG-INFO` & `streamflow_postgresql-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow-postgresql
-Version: 0.0.6
+Version: 0.0.7
 Summary: StreamFlow PostgreSQL plugin
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Package, https://pypi.org/project/streamflow-postgresql
 Project-URL: Repository, https://github.com/alpha-unito/streamflow-postgresql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -19,28 +19,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asyncpg==0.28.0
-Requires-Dist: streamflow==0.2.0.dev9
+Requires-Dist: asyncpg==0.29.0
+Requires-Dist: streamflow==0.2.0.dev11
 Provides-Extra: bandit
-Requires-Dist: bandit==1.7.5; extra == "bandit"
+Requires-Dist: bandit==1.7.8; extra == "bandit"
 Provides-Extra: lint
-Requires-Dist: black==23.9.1; extra == "lint"
-Requires-Dist: codespell==2.2.5; extra == "lint"
-Requires-Dist: flake8-bugbear==23.7.10; extra == "lint"
-Requires-Dist: pyupgrade==3.10.1; extra == "lint"
+Requires-Dist: black==24.4.2; extra == "lint"
+Requires-Dist: codespell==2.2.6; extra == "lint"
+Requires-Dist: flake8-bugbear==24.4.26; extra == "lint"
+Requires-Dist: pyupgrade==3.15.2; extra == "lint"
 Provides-Extra: test
-Requires-Dist: pytest==7.4.2; extra == "test"
+Requires-Dist: pytest==8.0.1; extra == "test"
 Requires-Dist: pytest-asyncio==0.21.1; extra == "test"
-Requires-Dist: pytest-cov==4.1.0; extra == "test"
-Requires-Dist: pytest-xdist==3.3.1; extra == "test"
+Requires-Dist: pytest-cov==5.0.0; extra == "test"
+Requires-Dist: pytest-xdist==3.6.1; extra == "test"
 
 # PostgreSQL Plugin for StreamFlow
 
 ## Installation
 
 Simply install the package directory from [PyPI](https://pypi.org/project/streamflow-postgresql/) using [pip](https://pip.pypa.io/en/stable/). StreamFlow will automatically recognise it as a plugin and load it at each workflow execution.
```

### Comparing `streamflow-postgresql-0.0.6/README.md` & `streamflow_postgresql-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.6/pyproject.toml` & `streamflow_postgresql-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.6/streamflow_postgresql/database.py` & `streamflow_postgresql-0.0.7/streamflow_postgresql/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,27 +87,14 @@
 
     @classmethod
     def get_schema(cls) -> str:
         return pkg_resources.resource_filename(
             __name__, os.path.join("schemas", "postgresql.json")
         )
 
-    async def add_command(self, step_id: int, tag: str, cmd: str) -> int:
-        async with self.pool as pool:
-            async with pool.acquire() as conn:
-                async with conn.transaction():
-                    return await conn.fetchval(
-                        "INSERT INTO command(step, tag, cmd) "
-                        "VALUES($1, $2, $3) "
-                        "RETURNING id",
-                        step_id,
-                        tag,
-                        cmd.encode("utf-8"),
-                    )
-
     async def add_dependency(
         self, step: int, port: int, type: DependencyType, name: str
     ) -> None:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 async with conn.transaction():
                     await conn.execute(
@@ -124,28 +111,56 @@
         self,
         name: str,
         type: str,
         config: str,
         external: bool,
         lazy: bool,
         workdir: str | None,
+        wraps: MutableMapping[str, Any] | None,
     ) -> int:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 async with conn.transaction():
                     return await conn.fetchval(
-                        "INSERT INTO deployment(name, type, config, external, lazy, workdir) "
-                        "VALUES ($1, $2, $3, $4, $5, $6) "
+                        "INSERT INTO deployment(name, type, config, external, lazy, workdir, wraps) "
+                        "VALUES ($1, $2, $3, $4, $5, $6, $7) "
                         "RETURNING id",
                         name,
                         type,
                         config,
                         external,
                         lazy,
                         workdir,
+                        json.dumps(wraps),
+                    )
+
+    async def add_execution(self, step_id: int, tag: str, cmd: str) -> int:
+        async with self.pool as pool:
+            async with pool.acquire() as conn:
+                async with conn.transaction():
+                    return await conn.fetchval(
+                        "INSERT INTO execution(step, tag, cmd) "
+                        "VALUES($1, $2, $3) "
+                        "RETURNING id",
+                        step_id,
+                        tag,
+                        cmd.encode("utf-8"),
+                    )
+
+    async def add_filter(self, name: str, type: str, config: str) -> int:
+        async with self.pool as pool:
+            async with pool.acquire() as conn:
+                async with conn.transaction():
+                    return await conn.fetchval(
+                        "INSERT INTO filter(name, type, config) "
+                        "VALUES($1, $2, $3) "
+                        "RETURNING id",
+                        name,
+                        type,
+                        config,
                     )
 
     async def add_port(
         self, name: str, workflow_id: int, type: type[Port], params: str
     ) -> int:
         async with self.pool as pool:
             async with pool.acquire() as conn:
@@ -238,124 +253,164 @@
                         "RETURNING id",
                         name,
                         json.dumps(params),
                         status,
                         type,
                     )
 
-    async def get_command(self, command_id: int) -> MutableMapping[str, Any]:
+    async def get_dependees(
+        self, token_id: int
+    ) -> MutableSequence[MutableMapping[str, Any]]:
+        async with self.pool as pool:
+            async with pool.acquire() as conn:
+                return await conn.fetch(
+                    "SELECT * FROM provenance WHERE depender = $1",
+                    token_id,
+                )
+
+    async def get_dependers(
+        self, token_id: int
+    ) -> MutableSequence[MutableMapping[str, Any]]:
+        async with self.pool as pool:
+            async with pool.acquire() as conn:
+                return await conn.fetch(
+                    "SELECT * FROM provenance WHERE dependee = $1",
+                    token_id,
+                )
+
+    async def get_deployment(self, deplyoment_id: int) -> MutableMapping[str, Any]:
+        async with self.pool as pool:
+            async with pool.acquire() as conn:
+                return await conn.fetchrow(
+                    "SELECT * FROM deployment WHERE id = $1",
+                    deplyoment_id,
+                )
+
+    async def get_execution(self, execution_id: int) -> MutableMapping[str, Any]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 row = await conn.fetchrow(
-                    "SELECT * FROM command WHERE id = $1", command_id
+                    "SELECT * FROM execution WHERE id = $1", execution_id
                 )
                 return {
                     k: bytearray(v) if isinstance(v, memoryview) else v
                     for k, v in row.items()
                 }
 
-    async def get_commands_by_step(
+    async def get_executions_by_step(
         self, step_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 rows = await conn.fetch(
-                    "SELECT * FROM command WHERE step = $1", step_id
+                    "SELECT * FROM execution WHERE step = $1", step_id
                 )
                 return [
                     {
                         k: bytearray(v) if isinstance(v, memoryview) else v
                         for k, v in row.items()
                     }
                     for row in rows
                 ]
 
-    async def get_dependees(
-        self, token_id: int
-    ) -> MutableSequence[MutableMapping[str, Any]]:
+    async def get_filter(self, filter_id: int) -> MutableMapping[str, Any]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
-                return await conn.fetch(
-                    "SELECT * FROM provenance WHERE depender = $1",
-                    token_id,
+                return await conn.fetchrow(
+                    "SELECT * FROM filter WHERE id = $1",
+                    filter_id,
                 )
 
-    async def get_dependers(
-        self, token_id: int
+    async def get_input_ports(
+        self, step_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 return await conn.fetch(
-                    "SELECT * FROM provenance WHERE dependee = $1",
-                    token_id,
+                    "SELECT * FROM dependency WHERE step = $1 AND type = $2",
+                    step_id,
+                    DependencyType.INPUT.value,
                 )
 
-    async def get_deployment(self, deplyoment_id: int) -> MutableMapping[str, Any]:
+    async def get_input_steps(
+        self, port_id: int
+    ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
-                return await conn.fetchrow(
-                    "SELECT * FROM deployment WHERE id = $1",
-                    deplyoment_id,
+                return await conn.fetch(
+                    "SELECT * FROM dependency WHERE port = $1 AND type = $2",
+                    port_id,
+                    DependencyType.OUTPUT.value,
                 )
 
-    async def get_input_ports(
+    async def get_output_ports(
         self, step_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 return await conn.fetch(
                     "SELECT * FROM dependency WHERE step = $1 AND type = $2",
                     step_id,
-                    DependencyType.INPUT.value,
+                    DependencyType.OUTPUT.value,
                 )
 
-    async def get_output_ports(
-        self, step_id: int
+    async def get_output_steps(
+        self, port_id: int
     ) -> MutableSequence[MutableMapping[str, Any]]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 return await conn.fetch(
-                    "SELECT * FROM dependency WHERE step = $1 AND type = $2",
-                    step_id,
-                    DependencyType.OUTPUT.value,
+                    "SELECT * FROM dependency WHERE port = $1 AND type = $2",
+                    port_id,
+                    DependencyType.INPUT.value,
                 )
 
     async def get_port(self, port_id: int) -> MutableMapping[str, Any]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 return await conn.fetchrow("SELECT * FROM port WHERE id = $1", port_id)
 
+    async def get_port_from_token(self, token_id: int) -> MutableMapping[str, Any]:
+        async with self.pool as pool:
+            async with pool.acquire() as conn:
+                return await conn.fetchrow(
+                    "SELECT port.* "
+                    "FROM token JOIN port ON token.port = port.id"
+                    "WHERE token.id = $1",
+                    token_id,
+                )
+
     async def get_port_tokens(self, port_id: int) -> MutableSequence[int]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 rows = await conn.fetch("SELECT * FROM port WHERE id = $1", port_id)
                 return [row["id"] for row in rows]
 
     async def get_reports(
         self, workflow: str, last_only: bool = False
     ) -> MutableSequence[MutableSequence[MutableMapping[str, Any]]]:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 if last_only:
                     rows = await conn.fetch(
                         "SELECT c.id, s.name, c.start_time, c.end_time "
-                        "FROM step AS s, command AS c "
+                        "FROM step AS s, execution AS c "
                         "WHERE s.id = c.step "
                         "AND s.workflow = ("
                         "SELECT id FROM workflow "
                         "WHERE name = $1 "
                         "ORDER BY id DESC LIMIT 1)",
                         workflow,
                     )
                     return [[dict(r) for r in rows]]
                 else:
                     async with conn.transaction():
                         cursor = conn.cursor(
                             "SELECT s.workflow, c.id, s.name, c.start_time, c.end_time "
-                            "FROM step AS s, command AS c "
+                            "FROM step AS s, execution AS c "
                             "WHERE s.id = c.step "
                             "AND s.workflow IN (SELECT id FROM workflow WHERE name = $1) "
                             "ORDER BY s.workflow DESC",
                             workflow,
                         )
                         result = {}
                         async for row in cursor:
@@ -442,45 +497,63 @@
                 async with pool.acquire() as conn:
                     return await conn.fetch(
                         "SELECT name, type, COUNT(*) AS num "
                         "FROM workflow GROUP BY name, type "
                         "ORDER BY name DESC"
                     )
 
-    async def update_command(
-        self, command_id: int, updates: MutableMapping[str, Any]
+    async def update_deployment(
+        self, deployment_id: int, updates: MutableMapping[str, Any]
     ) -> int:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 async with conn.transaction():
                     await conn.execute(
-                        "UPDATE command SET {} WHERE id = $1".format(  # nosec
+                        "UPDATE deployment SET {} WHERE id = $1".format(  # nosec
                             ", ".join([f"{k} = ${i+2}" for i, k in enumerate(updates)])
                         ),
-                        command_id,
+                        deployment_id,
                         *updates.values(),
                     )
-                    self.port_cache.pop(command_id, None)
-                    return command_id
+                    self.port_cache.pop(deployment_id, None)
+                    return deployment_id
 
-    async def update_deployment(
-        self, deployment_id: int, updates: MutableMapping[str, Any]
+    async def update_execution(
+        self, execution_id: int, updates: MutableMapping[str, Any]
     ) -> int:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 async with conn.transaction():
                     await conn.execute(
-                        "UPDATE deployment SET {} WHERE id = $1".format(  # nosec
+                        "UPDATE execution SET {} WHERE id = $1".format(  # nosec
                             ", ".join([f"{k} = ${i+2}" for i, k in enumerate(updates)])
                         ),
-                        deployment_id,
+                        execution_id,
                         *updates.values(),
                     )
-                    self.port_cache.pop(deployment_id, None)
-                    return deployment_id
+                    self.port_cache.pop(execution_id, None)
+                    return execution_id
+
+    async def update_filter(
+        self, filter_id: int, updates: MutableMapping[str, Any]
+    ) -> int:
+        async with self.pool as pool:
+            async with pool.acquire() as conn:
+                async with conn.transaction():
+                    await conn.execute(
+                        "UPDATE filter SET {} WHERE id = $1".format(  # nosec
+                            ", ".join(
+                                [f"{k} = ${i + 2}" for i, k in enumerate(updates)]
+                            )
+                        ),
+                        filter_id,
+                        *updates.values(),
+                    )
+                    self.filter_cache.pop(filter_id, None)
+                    return filter_id
 
     async def update_port(self, port_id: int, updates: MutableMapping[str, Any]) -> int:
         async with self.pool as pool:
             async with pool.acquire() as conn:
                 async with conn.transaction():
                     await conn.execute(
                         "UPDATE port SET {} WHERE id = $1".format(  # nosec
```

### Comparing `streamflow-postgresql-0.0.6/streamflow_postgresql/schemas/postgresql.json` & `streamflow_postgresql-0.0.7/streamflow_postgresql/schemas/postgresql.json`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.6/streamflow_postgresql/schemas/postgresql.sql` & `streamflow_postgresql-0.0.7/streamflow_postgresql/schemas/postgresql.sql`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     name TEXT,
     PRIMARY KEY (step, port, type, name),
     FOREIGN KEY (step) REFERENCES step (id),
     FOREIGN KEY (port) REFERENCES port (id)
 );
 
 
-CREATE TABLE IF NOT EXISTS command
+CREATE TABLE IF NOT EXISTS execution
 (
     id         SERIAL PRIMARY KEY,
     step       INTEGER,
     tag        TEXT,
     cmd        TEXT,
     output     BYTEA,
     status     INTEGER,
@@ -82,22 +82,31 @@
 (
     id       SERIAL PRIMARY KEY,
     name     TEXT,
     type     TEXT,
     config   TEXT,
     external BOOLEAN,
     lazy     BOOLEAN,
-    workdir  TEXT
+    workdir  TEXT,
+    wraps    TEXT
 );
 
 
 CREATE TABLE IF NOT EXISTS target
 (
     id         SERIAL PRIMARY KEY,
     deployment INTEGER,
     type       TEXT,
     locations  INTEGER,
     service    TEXT,
     workdir    TEXT,
     params     TEXT,
     FOREIGN KEY (deployment) REFERENCES deployment (id)
 );
+
+CREATE TABLE IF NOT EXISTS filter
+(
+    id          SERIAL PRIMARY KEY,
+    name        TEXT,
+    type        TEXT,
+    config      TEXT
+);
```

### Comparing `streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/PKG-INFO` & `streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow-postgresql
-Version: 0.0.6
+Version: 0.0.7
 Summary: StreamFlow PostgreSQL plugin
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Package, https://pypi.org/project/streamflow-postgresql
 Project-URL: Repository, https://github.com/alpha-unito/streamflow-postgresql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -19,28 +19,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asyncpg==0.28.0
-Requires-Dist: streamflow==0.2.0.dev9
+Requires-Dist: asyncpg==0.29.0
+Requires-Dist: streamflow==0.2.0.dev11
 Provides-Extra: bandit
-Requires-Dist: bandit==1.7.5; extra == "bandit"
+Requires-Dist: bandit==1.7.8; extra == "bandit"
 Provides-Extra: lint
-Requires-Dist: black==23.9.1; extra == "lint"
-Requires-Dist: codespell==2.2.5; extra == "lint"
-Requires-Dist: flake8-bugbear==23.7.10; extra == "lint"
-Requires-Dist: pyupgrade==3.10.1; extra == "lint"
+Requires-Dist: black==24.4.2; extra == "lint"
+Requires-Dist: codespell==2.2.6; extra == "lint"
+Requires-Dist: flake8-bugbear==24.4.26; extra == "lint"
+Requires-Dist: pyupgrade==3.15.2; extra == "lint"
 Provides-Extra: test
-Requires-Dist: pytest==7.4.2; extra == "test"
+Requires-Dist: pytest==8.0.1; extra == "test"
 Requires-Dist: pytest-asyncio==0.21.1; extra == "test"
-Requires-Dist: pytest-cov==4.1.0; extra == "test"
-Requires-Dist: pytest-xdist==3.3.1; extra == "test"
+Requires-Dist: pytest-cov==5.0.0; extra == "test"
+Requires-Dist: pytest-xdist==3.6.1; extra == "test"
 
 # PostgreSQL Plugin for StreamFlow
 
 ## Installation
 
 Simply install the package directory from [PyPI](https://pypi.org/project/streamflow-postgresql/) using [pip](https://pip.pypa.io/en/stable/). StreamFlow will automatically recognise it as a plugin and load it at each workflow execution.
```

### Comparing `streamflow-postgresql-0.0.6/streamflow_postgresql.egg-info/SOURCES.txt` & `streamflow_postgresql-0.0.7/streamflow_postgresql.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,8 +15,10 @@
 streamflow_postgresql.egg-info/dependency_links.txt
 streamflow_postgresql.egg-info/entry_points.txt
 streamflow_postgresql.egg-info/requires.txt
 streamflow_postgresql.egg-info/top_level.txt
 streamflow_postgresql.egg-info/zip-safe
 streamflow_postgresql/schemas/postgresql.json
 streamflow_postgresql/schemas/postgresql.sql
+tests/test_cwl_persistence.py
+tests/test_database.py
 tests/test_persistence.py
```

### Comparing `streamflow-postgresql-0.0.6/tests/test_persistence.py` & `streamflow_postgresql-0.0.7/tests/test_persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 import posixpath
 
 import pytest
 
 from tests.conftest import get_docker_deployment_config, save_load_and_test
 
 from streamflow.core import utils
-from streamflow.core.context import StreamFlowContext
 from streamflow.core.config import BindingConfig
-from streamflow.core.deployment import Target, LocalTarget
+from streamflow.core.context import StreamFlowContext
+from streamflow.core.deployment import LocalTarget, Target, FilterConfig
 from streamflow.core.workflow import Job, Token, Workflow
-
-from streamflow.workflow.port import JobPort, ConnectorPort
+from streamflow.workflow.combinator import (
+    CartesianProductCombinator,
+    DotProductCombinator,
+    LoopCombinator,
+    LoopTerminationCombinator,
+)
+from streamflow.workflow.port import ConnectorPort, JobPort
 from streamflow.workflow.step import (
     CombinatorStep,
     DeployStep,
     ExecuteStep,
     GatherStep,
-    ScheduleStep,
-    ScatterStep,
     LoopCombinatorStep,
-)
-from streamflow.workflow.combinator import (
-    CartesianProductCombinator,
-    DotProductCombinator,
-    LoopCombinator,
-    LoopTerminationCombinator,
+    ScatterStep,
+    ScheduleStep,
 )
 from streamflow.workflow.token import (
+    IterationTerminationToken,
     JobToken,
     ListToken,
     ObjectToken,
     TerminationToken,
-    IterationTerminationToken,
 )
 
 
-# Testing Workflow
 @pytest.mark.asyncio
 async def test_workflow(context: StreamFlowContext):
     """Test saving and loading Workflow from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await save_load_and_test(workflow, context)
 
 
-# Testing Port and its extension classes
 @pytest.mark.asyncio
 async def test_port(context: StreamFlowContext):
     """Test saving and loading Port from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await workflow.save(context)
@@ -75,15 +72,14 @@
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await workflow.save(context)
     port = workflow.create_port(ConnectorPort)
     await save_load_and_test(port, context)
 
 
-# Testing Step and its extension classes
 @pytest.mark.asyncio
 async def test_combinator_step(context: StreamFlowContext):
     """Test saving and loading CombinatorStep with CartesianProductCombinator from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await workflow.save(context)
@@ -176,18 +172,22 @@
 
 @pytest.mark.asyncio
 async def test_gather_step(context: StreamFlowContext):
     """Test saving and loading GatherStep from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
+    size_port = workflow.create_port()
     await workflow.save(context)
 
     step = workflow.create_step(
-        cls=GatherStep, name=utils.random_name() + "-gather", depth=1
+        cls=GatherStep,
+        name=utils.random_name() + "-gather",
+        depth=1,
+        size_port=size_port,
     )
     await save_load_and_test(step, context)
 
 
 @pytest.mark.asyncio
 async def test_scatter_step(context: StreamFlowContext):
     """Test saving and loading ScatterStep from database"""
@@ -196,15 +196,14 @@
     )
     await workflow.save(context)
 
     step = workflow.create_step(cls=ScatterStep, name=utils.random_name() + "-scatter")
     await save_load_and_test(step, context)
 
 
-# Subtest - Step param combinator
 @pytest.mark.asyncio
 async def test_dot_product_combinator(context: StreamFlowContext):
     """Test saving and loading CombinatorStep with DotProductCombinator from database"""
     workflow = Workflow(
         context=context, type="cwl", name=utils.random_name(), config={}
     )
     await workflow.save(context)
@@ -250,15 +249,14 @@
         combinator=LoopTerminationCombinator(
             name=utils.random_name(), workflow=workflow
         ),
     )
     await save_load_and_test(step, context)
 
 
-# Testing the Target and its extension classes
 @pytest.mark.asyncio
 async def test_target(context: StreamFlowContext):
     """Test saving and loading Target from database"""
     target = Target(
         deployment=get_docker_deployment_config(),
         service="test-persistence",
         workdir=utils.random_name(),
@@ -269,15 +267,14 @@
 @pytest.mark.asyncio
 async def test_local_target(context: StreamFlowContext):
     """Test saving and loading LocalTarget from database"""
     target = LocalTarget(workdir=utils.random_name())
     await save_load_and_test(target, context)
 
 
-# Testing the Token and its extension classes
 @pytest.mark.asyncio
 async def test_token(context: StreamFlowContext):
     """Test saving and loading Token from database"""
     token = Token(value=["test", "token"])
     await save_load_and_test(token, context)
 
 
@@ -321,13 +318,19 @@
 @pytest.mark.asyncio
 async def test_iteration_termination_token(context: StreamFlowContext):
     """Test saving and loading IterationTerminationToken from database"""
     token = IterationTerminationToken("1")
     await save_load_and_test(token, context)
 
 
-# Deployment test
+@pytest.mark.asyncio
+async def test_filter_config(context: StreamFlowContext):
+    """Test saving and loading filter configuration from database"""
+    config = FilterConfig(config={}, name=utils.random_name(), type="shuffle")
+    await save_load_and_test(config, context)
+
+
 @pytest.mark.asyncio
 async def test_deployment(context: StreamFlowContext):
     """Test saving and loading deployment configuration from database"""
     config = get_docker_deployment_config()
     await save_load_and_test(config, context)
```


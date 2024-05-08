# Comparing `tmp/tilekiln-0.4.0.tar.gz` & `tmp/tilekiln-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Fri Mar 15 22:04:25 2024, max compression
+gzip compressed data, last modified: Mon Apr 29 23:38:30 2024, max compression
```

## Comparing `tilekiln-0.4.0.tar` & `tilekiln-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,24 @@
--rw-r--r--   0        0        0      468 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/__init__.py
--rw-r--r--   0        0        0     3681 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/config.py
--rw-r--r--   0        0        0     2023 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/definition.py
--rw-r--r--   0        0        0     1094 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/kiln.py
--rw-r--r--   0        0        0      241 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/metric.py
--rw-r--r--   0        0        0     2891 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/prometheus.py
--rw-r--r--   0        0        0    17811 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/storage.py
--rw-r--r--   0        0        0      775 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/tile.py
--rw-r--r--   0        0        0     1842 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/tileset.py
--rw-r--r--   0        0        0     2255 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/dev/__init__.py
--rw-r--r--   0        0        0    16051 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/scripts/__init__.py
--rw-r--r--   0        0        0     6261 2024-03-15 22:04:25.000000 tilekiln-0.4.0/tilekiln/server/__init__.py
--rw-r--r--   0        0        0       97 2024-03-15 22:04:25.000000 tilekiln-0.4.0/.gitignore
--rw-r--r--   0        0        0    35147 2024-03-15 22:04:25.000000 tilekiln-0.4.0/LICENSE
--rw-r--r--   0        0        0     7328 2024-03-15 22:04:25.000000 tilekiln-0.4.0/README.md
--rw-r--r--   0        0        0     1425 2024-03-15 22:04:25.000000 tilekiln-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8410 2024-03-15 22:04:25.000000 tilekiln-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      494 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/__init__.py
+-rw-r--r--   0        0        0     3695 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/config.py
+-rw-r--r--   0        0        0     2055 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/definition.py
+-rwxr-xr-x   0        0        0     1240 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/generator.py
+-rw-r--r--   0        0        0     1094 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/kiln.py
+-rw-r--r--   0        0        0     2029 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/main.py
+-rw-r--r--   0        0        0      241 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/metric.py
+-rw-r--r--   0        0        0     2891 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/prometheus.py
+-rw-r--r--   0        0        0    16801 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/storage.py
+-rw-r--r--   0        0        0     1356 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/tile.py
+-rw-r--r--   0        0        0      358 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/tilerange.py
+-rw-r--r--   0        0        0     1842 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/tileset.py
+-rw-r--r--   0        0        0     2255 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/dev/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/scripts/__init__.py
+-rw-r--r--   0        0        0     1851 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/scripts/config.py
+-rw-r--r--   0        0        0     3547 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/scripts/generate.py
+-rw-r--r--   0        0        0     5964 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/scripts/serve.py
+-rw-r--r--   0        0        0     4998 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/scripts/storage.py
+-rw-r--r--   0        0        0     6222 2024-04-29 23:38:30.000000 tilekiln-0.5.0/tilekiln/server/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-29 23:38:30.000000 tilekiln-0.5.0/.gitignore
+-rw-r--r--   0        0        0    35147 2024-04-29 23:38:30.000000 tilekiln-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7445 2024-04-29 23:38:30.000000 tilekiln-0.5.0/README.md
+-rw-r--r--   0        0        0     1427 2024-04-29 23:38:30.000000 tilekiln-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8540 2024-04-29 23:38:30.000000 tilekiln-0.5.0/PKG-INFO
```

### Comparing `tilekiln-0.4.0/tilekiln/config.py` & `tilekiln-0.5.0/tilekiln/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         self.__definitions = set()
         for definition in layer_yaml.get("sql", []):
             self.__definitions.add(Definition(id, definition, filesystem))
 
         self.minzoom = min({d.minzoom for d in self.__definitions})
         self.maxzoom = max({d.maxzoom for d in self.__definitions})
 
-    def render_sql(self, tile):
+    def render_sql(self, tile) -> str | None:
         '''Returns the SQL for a layer, given a tile, or None if it is outside the zoom range
            of the definitions
         '''
         if tile.zoom > self.maxzoom or tile.zoom < self.minzoom:
             return None
 
         for d in self.__definitions:
```

### Comparing `tilekiln-0.4.0/tilekiln/definition.py` & `tilekiln-0.5.0/tilekiln/definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 
 DEFAULT_EXTENT = 4096
 DEFAULT_BUFFER = 0
 
 # Invariants of web mercator
 HALF_WORLD = 20037508.34
 
-j2Environment = j2.Environment(loader=j2.BaseLoader())
+j2Environment = j2.Environment(loader=j2.BaseLoader(), lstrip_blocks=True, trim_blocks=True)
 
 
 class Definition:
     def __init__(self, id, definition_yaml, filesystem):
         self.id = id
         self.minzoom = definition_yaml["minzoom"]
         self.maxzoom = definition_yaml["maxzoom"]
         self.extent = definition_yaml.get("extent", DEFAULT_EXTENT)
         self.buffer = definition_yaml.get("buffer", DEFAULT_BUFFER)
 
         # TODO: Let is use directories so one file can include others.
         self.__template = j2Environment.from_string(filesystem.readtext(definition_yaml["file"]))
 
-    def render_sql(self, tile):
+    def render_sql(self, tile) -> str:
         '''Generate the SQL for a layer
         '''
 
         # Tile validity constraints. x/y are checked by Tile class
         assert tile.zoom >= self.minzoom
         assert tile.zoom <= self.maxzoom
 
@@ -38,15 +38,15 @@
                                        tile_length=tile_length(tile),
                                        tile_area=tile_length(tile)**2,
                                        coordinate_length=tile_length(tile)/self.extent,
                                        coordinate_area=(tile_length(tile)/self.extent)**2)
 
         # TODO: Use proper escaping for self.id in SQL
         return ('''WITH mvtgeom AS\n(\n''' + inner + '''\n)\n''' +
-                f'''SELECT ST_AsMVT(mvtgeom.*, '{self.id}', {self.extent}, 'way', NULL)\n''' +
+                f'''SELECT ST_AsMVT(mvtgeom.*, '{self.id}', {self.extent})\n''' +
                 '''FROM mvtgeom;''')
 
 
 def tile_length(tile):
     '''Returns the length of a tile, in projected units
     '''
     # -1 for half vs full world
```

### Comparing `tilekiln-0.4.0/tilekiln/kiln.py` & `tilekiln-0.5.0/tilekiln/kiln.py`

 * *Files identical despite different names*

### Comparing `tilekiln-0.4.0/tilekiln/prometheus.py` & `tilekiln-0.5.0/tilekiln/prometheus.py`

 * *Files identical despite different names*

### Comparing `tilekiln-0.4.0/tilekiln/storage.py` & `tilekiln-0.5.0/tilekiln/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import gzip
 import json
 import sys
 from collections.abc import Iterator
 
 import click
 import psycopg.rows
-from psycopg_pool import ConnectionPool
+from psycopg import Connection
 
 from tilekiln.metric import Metric
 from tilekiln.tile import Tile
 from tilekiln.tileset import Tileset
 
 METADATA_TABLE = "metadata"
 GENERATE_STATS_TABLE = "generate_stats"
@@ -25,233 +25,215 @@
 class Storage:
     '''
     Storage is an object representing a tile storage, backed by a PostgreSQL database
 
     A Storage contains tiles and metadata about tilesets, and has functions to update
     tiles and metadata based on the ID
     '''
-    def __init__(self, dbpool: ConnectionPool, schema="tilekiln"):
-        self.__pool = dbpool
+    def __init__(self, conn: Connection, schema="tilekiln"):
+        self.__conn = conn
+        self.__conn.execute("SET TIMEZONE TO 'GMT'")
+        self.__conn.commit()
         self.__schema = schema
 
     '''
     Methods that manipulate schema-related stuff and don't involve any tiles
     '''
     def create_schema(self) -> None:
-        with self.__pool.connection() as conn:
-            with conn.cursor() as cur:
-                # Perform one-time setup using CREATE ... IF NOT EXISTS
-                # This is safe to rerun multiple times
-                cur.execute(f'''CREATE SCHEMA IF NOT EXISTS "{self.__schema}"''')
-                self.__setup_stats(cur)
-                self.__setup_metadata(cur)
-                conn.commit()
+        with self.__conn.cursor() as cur:
+            # Perform one-time setup using CREATE ... IF NOT EXISTS
+            # This is safe to rerun multiple times
+            cur.execute(f'''CREATE SCHEMA IF NOT EXISTS "{self.__schema}"''')
+            self.__setup_stats(cur)
+            self.__setup_metadata(cur)
+            self.__conn.commit()
 
     '''
     Methods for tilesets
     '''
     def create_tileset(self, id: str, minzoom: int, maxzoom: int, tilejson: str) -> None:
-        with self.__pool.connection() as conn:
-            with conn.cursor() as cur:
-                self.__set_metadata(cur, id, minzoom, maxzoom, tilejson)
+        with self.__conn.cursor() as cur:
+            self.__set_metadata(cur, id, minzoom, maxzoom, tilejson)
 
-                self.__setup_tables(cur, id, minzoom, maxzoom)
+            self.__setup_tables(cur, id, minzoom, maxzoom)
 
-                conn.commit()
+            self.__conn.commit()
 
     def remove_tileset(self, id: str) -> None:
-        with self.__pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(f'''DELETE FROM "{self.__schema}"."{METADATA_TABLE}" WHERE id = %s''',
-                            (id,))
-                cur.execute(f'''DROP TABLE "{self.__schema}"."{id}" CASCADE''')
-                cur.execute(f'''DELETE FROM "{self.__schema}"."{TILE_STATS_TABLE}" WHERE id = %s''',
-                            (id,))
-                conn.commit()
+        with self.__conn.cursor() as cur:
+            cur.execute(f'''DELETE FROM "{self.__schema}"."{METADATA_TABLE}" WHERE id = %s''',
+                        (id,))
+            cur.execute(f'''DROP TABLE "{self.__schema}"."{id}" CASCADE''')
+            cur.execute(f'''DELETE FROM "{self.__schema}"."{TILE_STATS_TABLE}" WHERE id = %s''',
+                        (id,))
+            self.__conn.commit()
 
     def get_tilesets(self) -> Iterator[Tileset]:
         '''
         Gets all tilesets in the storage
         '''
-        with self.__pool.connection() as conn:
-            conn.read_only = True
-            with conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
-                cur.execute(f'''SELECT id, minzoom, maxzoom, tilejson
-                             FROM "{self.__schema}"."{METADATA_TABLE}"''')
-                for record in cur:
-                    yield Tileset(self, record["id"], record["minzoom"], record["maxzoom"],
-                                  json.dumps(record["tilejson"]))
+
+        with self.__conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
+            cur.execute(f'''SELECT id, minzoom, maxzoom, tilejson
+                            FROM "{self.__schema}"."{METADATA_TABLE}"''')
+            for record in cur:
+                yield Tileset(self, record["id"], record["minzoom"], record["maxzoom"],
+                              json.dumps(record["tilejson"]))
 
     def get_tileset_ids(self) -> Iterator[str]:
         '''
         Get only the tileset IDs
         '''
-        with self.__pool.connection() as conn:
-            conn.read_only = True
-            with conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
-                cur.execute(f'''SELECT id
-                             FROM "{self.__schema}"."{METADATA_TABLE}"''')
-                for record in cur:
-                    yield record["id"]
+
+        with self.__conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
+            cur.execute(f'''SELECT id
+                            FROM "{self.__schema}"."{METADATA_TABLE}"''')
+            for record in cur:
+                yield record["id"]
 
     ''' Methods for metrics'''
     def metrics(self) -> Iterator[Metric]:
-        with self.__pool.connection() as conn:
-            conn.read_only = True
-            with conn.cursor(row_factory=psycopg.rows.class_row(Metric)) as cur:
-                cur.execute(f'''SELECT id, zoom, num_tiles, size, percentiles
-                             FROM "{self.__schema}"."{TILE_STATS_TABLE}"''')
-                for record in cur:
-                    yield record
+        with self.__conn.cursor(row_factory=psycopg.rows.class_row(Metric)) as cur:
+            cur.execute(f'''SELECT id, zoom, num_tiles, size, percentiles
+                            FROM "{self.__schema}"."{TILE_STATS_TABLE}"''')
+            for record in cur:
+                yield record
 
     def update_metrics(self) -> None:
-        with self.__pool.connection() as conn:
-            with conn.cursor() as cur:
-                for id in self.get_tileset_ids():
-                    minzoom = self.get_minzoom(id)
-                    maxzoom = self.get_maxzoom(id)
-                    self.__update_tileset_metrics(cur, id, minzoom, maxzoom)
-                conn.commit()
+        with self.__conn.cursor() as cur:
+            for id in self.get_tileset_ids():
+                minzoom = self.get_minzoom(id)
+                maxzoom = self.get_maxzoom(id)
+                self.__update_tileset_metrics(cur, id, minzoom, maxzoom)
+            self.__conn.commit()
 
     '''Methods that set/get metadata'''
     def set_metadata(self, id, minzoom, maxzoom, tilejson):
         '''
         Saves metadata into storage
 
         This just wraps __set_metadata, which requires a cursor
         '''
-        with self.__pool.connection() as conn:
-            with conn.cursor() as cur:
-                self.__set_metadata(cur, id, minzoom, maxzoom, tilejson)
-                conn.commit()
+        with self.__conn.cursor() as cur:
+            self.__set_metadata(cur, id, minzoom, maxzoom, tilejson)
+            self.__conn.commit()
 
     # TODO: Should the various get_* functions be separate? The query has to fetch from the
     # DB each time, but only tilejson needs URL. Not an urgent issue.
     def get_tilejson(self, id, url) -> str:
         '''Gets the tilejson for a layer from storage.'''
-        with self.__pool.connection() as conn:
-            conn.read_only = True
-            with conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
-                cur.execute(f'''SELECT tilejson
-                                FROM "{self.__schema}"."{METADATA_TABLE}"
-                                WHERE id = %s''', (id,))
-                result = cur.fetchone()
-                if result is None:
-                    # TODO: raise exception and handle it at the calling level
-                    click.echo(f"Failed to retrieve tilejson for id {id}, "
-                               f"does it exist in storage DB?",
-                               err=True)
-                    sys.exit(1)
-                tilejson = result["tilejson"]
-                tilejson["tiles"] = [f"{url}" + "/{z}/{x}/{y}.mvt"]
-                return json.dumps(tilejson)
+        with self.__conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
+            cur.execute(f'''SELECT tilejson
+                            FROM "{self.__schema}"."{METADATA_TABLE}"
+                            WHERE id = %s''', (id,))
+            result = cur.fetchone()
+            if result is None:
+                # TODO: raise exception and handle it at the calling level
+                click.echo(f"Failed to retrieve tilejson for id {id}, "
+                           f"does it exist in storage DB?",
+                           err=True)
+                sys.exit(1)
+            tilejson = result["tilejson"]
+            tilejson["tiles"] = [f"{url}" + "/{z}/{x}/{y}.mvt"]
+            return json.dumps(tilejson)
 
     def get_minzoom(self, id):
         '''Gets the minzoom for a layer from storage.'''
-        with self.__pool.connection() as conn:
-            conn.read_only = True
-            with conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
-                cur.execute(f'''SELECT minzoom
-                                FROM "{self.__schema}"."{METADATA_TABLE}"
-                                WHERE id = %s''', (id,))
-                result = cur.fetchone()
-                if result is None:
-                    # TODO: raise exception and handle it at the calling level
-                    click.echo(f"Failed to retrieve minzoom for id {id}, "
-                               f"does it exist in storage DB?",
-                               err=True)
-                    sys.exit(1)
-                return result["minzoom"]
+        with self.__conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
+            cur.execute(f'''SELECT minzoom
+                            FROM "{self.__schema}"."{METADATA_TABLE}"
+                            WHERE id = %s''', (id,))
+            result = cur.fetchone()
+            if result is None:
+                # TODO: raise exception and handle it at the calling level
+                click.echo(f"Failed to retrieve minzoom for id {id}, "
+                           f"does it exist in storage DB?",
+                           err=True)
+                sys.exit(1)
+            return result["minzoom"]
 
     def get_maxzoom(self, id):
         '''Gets the minzoom for a layer from storage.'''
-        with self.__pool.connection() as conn:
-            conn.read_only = True
-            with conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
-                cur.execute(f'''SELECT maxzoom
-                                FROM "{self.__schema}"."{METADATA_TABLE}"
-                                WHERE id = %s''', (id,))
-                result = cur.fetchone()
-                if result is None:
-                    # TODO: raise exception and handle it at the calling level
-                    click.echo(f"Failed to retrieve minzoom for id {id}, "
-                               f"does it exist in storage DB?",
-                               err=True)
-                    sys.exit(1)
-                return result["maxzoom"]
+        with self.__conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
+            cur.execute(f'''SELECT maxzoom
+                            FROM "{self.__schema}"."{METADATA_TABLE}"
+                            WHERE id = %s''', (id,))
+            result = cur.fetchone()
+            if result is None:
+                # TODO: raise exception and handle it at the calling level
+                click.echo(f"Failed to retrieve minzoom for id {id}, "
+                           "does it exist in storage DB?", err=True)
+                sys.exit(1)
+            return result["maxzoom"]
 
     '''
     Methods that involve saving, fetching, and deleting tiles
     '''
-    def delete_tiles(self, id: str, tiles: Iterator[Tile]):
-        with self.__pool.connection() as conn:
-            with conn.cursor() as cur:
-                for tile in tiles:
-                    self.__delete_tile(cur, id, tile)
-            conn.commit()
+    def delete_tiles(self, id: str, tiles: set[Tile]):
+        with self.__conn.cursor() as cur:
+            for tile in tiles:
+                self.__delete_tile(cur, id, tile)
+        self.__conn.commit()
 
     def truncate_tables(self, id: str, zooms=None):
-        with self.__pool.connection() as conn:
-            with conn.cursor() as cur:
-                if zooms is None:
-                    zooms = range(self.get_minzoom(id), self.get_maxzoom(id)+1)
-                for zoom in zooms:
-                    self.__truncate_table(cur, id, zoom)
-                conn.commit()
+        with self.__conn.cursor() as cur:
+            if zooms is None:
+                zooms = range(self.get_minzoom(id), self.get_maxzoom(id)+1)
+            for zoom in zooms:
+                self.__truncate_table(cur, id, zoom)
+            self.__conn.commit()
 
     def get_tile(self, id: str, tile: Tile) -> tuple[bytes | None, datetime.datetime | None]:
-        with self.__pool.connection() as conn:
-            conn.execute("SET TIMEZONE TO 'GMT'")
-            with conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
-                cur.execute(f'''SELECT generated, tile FROM "{self.__schema}"."{id}"
-                                WHERE zoom = %s AND x = %s AND y = %s''',
-                            (tile.zoom, tile.x, tile.y), binary=True)
-                result = cur.fetchone()
-                if result is None:
-                    return None, None
-                return gzip.decompress(result["tile"]), result["generated"]
+
+        with self.__conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
+            cur.execute(f'''SELECT generated, tile FROM "{self.__schema}"."{id}"
+                            WHERE zoom = %s AND x = %s AND y = %s''',
+                        (tile.zoom, tile.x, tile.y), binary=True)
+            result = cur.fetchone()
+            if result is None:
+                return None, None
+            return gzip.decompress(result["tile"]), result["generated"]
 
     # TODO: Needs to return timestamp written to the DB
     def save_tile(self, id: str, tile: Tile,
                   tiledata: bytes, render_time=0) -> datetime.datetime | None:
-        with self.__pool.connection() as conn:
-            conn.execute("SET TIMEZONE TO 'GMT'")
-            with conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
-                # TODO: This statement unconditionally writes the row even if it's unchanged. It
-                # shouldn't. Adding WHERE tile != EXCLUDED.tile would help, but then it would
-                # return zero rows if the contents are the same. The method here instead results
-                # in extra writes but does preserve the datetime.
-                tablename = f"{id}_z{tile.zoom}"
-                cur.execute(f'''INSERT INTO "{self.__schema}"."{tablename}" AS store
-(zoom, x, y, tile)
-VALUES (%s, %s, %s, %s)
-ON CONFLICT (zoom, x, y)
-DO UPDATE SET tile = EXCLUDED.tile,
-generated = CASE WHEN store.tile != EXCLUDED.tile
-    THEN statement_timestamp()
-    ELSE store.generated END
-RETURNING generated''',
-                            (tile.zoom, tile.x, tile.y, gzip.compress(tiledata, mtime=0)))
-                result = cur.fetchone()
-                if result is None:
-                    return None
-                return result["generated"]
+        with self.__conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
+            # TODO: This statement unconditionally writes the row even if it's unchanged. It
+            # shouldn't. Adding WHERE tile != EXCLUDED.tile would help, but then it would
+            # return zero rows if the contents are the same. The method here instead results
+            # in extra writes but does preserve the datetime.
+            tablename = f"{id}_z{tile.zoom}"
+            cur.execute(f'''INSERT INTO "{self.__schema}"."{tablename}" AS store\n'''
+                        '''(zoom, x, y, tile)\n'''
+                        '''VALUES (%s, %s, %s, %s)\n'''
+                        '''ON CONFLICT (zoom, x, y)\n'''
+                        '''DO UPDATE SET tile = EXCLUDED.tile,\n'''
+                        '''generated = CASE WHEN store.tile != EXCLUDED.tile\n'''
+                        '''    THEN statement_timestamp()\n'''
+                        '''    ELSE store.generated END\n'''
+                        '''RETURNING generated''',
+                        (tile.zoom, tile.x, tile.y, gzip.compress(tiledata, mtime=0)))
+            result = cur.fetchone()
+            self.__conn.commit()
+            if result is None:
+                return None
+            return result["generated"]
 
     def __setup_metadata(self, cur):
         ''' Create the metadata table in storage. This is safe to rerun
         '''
         # TODO: Updating metadata table schema??
         # Probably can only be done on a major version upgrade
 
-        cur.execute(f'''CREATE TABLE IF NOT EXISTS "{self.__schema}"."{METADATA_TABLE}" (
-            id text PRIMARY KEY,
-            active boolean NOT NULL DEFAULT TRUE,
-            minzoom smallint NOT NULL,
-            maxzoom smallint NOT NULL,
-            tilejson jsonb NOT NULL)''')
+        cur.execute(f'''CREATE TABLE IF NOT EXISTS "{self.__schema}"."{METADATA_TABLE}" (\n'''
+                    '''id text PRIMARY KEY,\n'''
+                    '''active boolean NOT NULL DEFAULT TRUE,\n'''
+                    '''minzoom smallint NOT NULL,\n'''
+                    '''maxzoom smallint NOT NULL,\n'''
+                    '''tilejson jsonb NOT NULL)''')
 
     def __set_metadata(self, cur, id, minzoom, maxzoom, tilejson):
         '''
         Sets metadata using a cursor
 
         This is separate from set_metadata because sometimes it needs
         calling within a transaction
@@ -357,29 +339,27 @@
                             ALTER COLUMN tile SET STORAGE EXTERNAL''')
 
     def __load_metadata(self):
         '''Load the stored metadata.
 
         This allows serving a TileJSON without having access to the config
         '''
-        with self.__pool.connection() as conn:
-            with conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
-                cur.execute(f'''SELECT minzoom, maxzoom, tilejson
-                                FROM "{self.__schema}"."{METADATA_TABLE}"
-                                WHERE id = %s''', (self.id,))
-                result = cur.fetchone()
-                if result is None:
-                    # TODO: raise exception and handle it at the calling level
-                    click.echo(f"Failed to retrieve metadata for id {self.id}, "
-                               f"does it exist in storage DB?",
-                               err=True)
-                    sys.exit(1)
-                self.minzoom = result["minzoom"]
-                self.maxzoom = result["maxzoom"]
-                self.__rawtilejson = result["tilejson"]
+        with self.__conn.cursor(row_factory=psycopg.rows.dict_row) as cur:
+            cur.execute(f'''SELECT minzoom, maxzoom, tilejson
+                            FROM "{self.__schema}"."{METADATA_TABLE}"
+                            WHERE id = %s''', (self.id,))
+            result = cur.fetchone()
+            if result is None:
+                # TODO: raise exception and handle it at the calling level
+                click.echo(f"Failed to retrieve metadata for id {self.id}, "
+                           "does it exist in storage DB?", err=True)
+                sys.exit(1)
+            self.minzoom = result["minzoom"]
+            self.maxzoom = result["maxzoom"]
+            self.__rawtilejson = result["tilejson"]
 
     def __truncate_table(self, cur, id: str, zoom: int) -> None:
         '''Remove every tile from a particular tileset and zoom'''
         tablename = f"{id}_z{zoom}"
         cur.execute(f'''TRUNCATE TABLE "{self.__schema}"."{tablename}"''')
 
     def __delete_tile(self, cur, id: str, tile: Tile):
```

### Comparing `tilekiln-0.4.0/tilekiln/tileset.py` & `tilekiln-0.5.0/tilekiln/tileset.py`

 * *Files identical despite different names*

### Comparing `tilekiln-0.4.0/tilekiln/dev/__init__.py` & `tilekiln-0.5.0/tilekiln/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `tilekiln-0.4.0/tilekiln/server/__init__.py` & `tilekiln-0.5.0/tilekiln/server/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import os
 
 import psycopg
-import psycopg_pool
 from fastapi import FastAPI, Response, HTTPException
 
 import tilekiln
 from tilekiln.config import Config
 from tilekiln.kiln import Kiln
 from tilekiln.tile import Tile
 from tilekiln.tileset import Tileset
@@ -31,32 +30,35 @@
 storage: Storage
 tilesets: dict[str, Tileset] = {}
 
 # Two types of server are defined - one for static tiles, the other for live generated tiles.
 server = FastAPI()
 live = FastAPI()
 
+# TODO: Set up middleware for CORS
+
 
 # TODO: Move elsewhere
 def change_tilejson_url(tilejson: str, baseurl: str) -> str:
     modified_tilejson = json.loads(tilejson)
     modified_tilejson["tiles"] = [baseurl + "/{z}/{x}/{y}.mvt"]
     return json.dumps(modified_tilejson)
 
 
 @server.on_event("startup")
 def load_server_config():
     '''Load the config for the server with static pre-rendered tiles'''
     global storage
     global tilesets
     # Because the DB connection variables are passed as standard PG* vars,
-    # a plain ConnectionPool() will connect to the right DB
-    pool = psycopg_pool.ConnectionPool(min_size=1, max_size=1)
+    # a plain connect() will connect to the right DB
+    conn = psycopg.connect()
+    # TODO: Make readonly?
 
-    storage = Storage(pool)
+    storage = Storage(conn)
     for tileset in storage.get_tilesets():
         tilesets[tileset.id] = tileset
 
 
 @live.on_event("startup")
 def load_live_config():
     global config
@@ -80,16 +82,16 @@
     if "STORAGE_PGHOST" in os.environ:
         storage_args["host"] = os.environ["STORAGE_PGHOST"]
     if "STORAGE_PGPORT" in os.environ:
         storage_args["port"] = os.environ["STORAGE_PGPORT"]
     if "STORAGE_PGUSER" in os.environ:
         storage_args["username"] = os.environ["STORAGE_PGUSER"]
 
-    storage_pool = psycopg_pool.ConnectionPool(min_size=1, max_size=1, kwargs=storage_args)
-    storage = Storage(storage_pool)
+    storage_conn = psycopg.connect(**storage_args)
+    storage = Storage(storage_conn)
 
     # Storing the tileset in the dict allows some commonalities in code later
     tilesets[config.id] = Tileset.from_config(storage, config)
     conn = psycopg.connect(**generate_args)
     global kiln
     kiln = Kiln(config, conn)
```

### Comparing `tilekiln-0.4.0/LICENSE` & `tilekiln-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tilekiln-0.4.0/README.md` & `tilekiln-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ##### `config test`
 Tests a config for validity.
 
 The process will exit with exit code 0 if tilekiln can load the config.
 
 This is intended for build and CI scripts used by configs.
 
-#### `sql`
+##### `config sql`
 Print the SQL for a tile or layer.
 
 Prints the SQL that would be issued to generate a particular tile layer,
 or if no layer is given, the entire tile. This allows manual debugging of
 a tile query.
 
 #### `generate`
@@ -89,24 +89,28 @@
 Delete specific tiles.
 
 A list of z/x/y tiles is read from stdin and those tiles are deleted from
 storage. The entire list is read before deletion starts.
 
 ### Serving commands
 These commands start a HTTP server to serve content.
+#### `serve`
+Commands for tile serving.
+
+All tile serving commands serve tiles and a tilejson over HTTP.
 
-#### `dev`
+##### `dev`
 Starts a server to live-render tiles with no caching, intended for development. It presents a tilejson at `/<id>/tilejson.json`, and for convience `/tilejson.json` redirects to it.
 
-#### `live`
+##### `live`
 Like `serve`, but fall back to live generation if a tile is missing from storage.
 
 It presents a tilejson at `/<id>/tilejson.json`.
 
-#### `serve`
+##### `static`
 Serves tiles from tile storage. This is highly scalable and the preferred mode for production.
 
 It presents a tilejson at `/<id>/tilejson.json`. In the future it will allow serving multiple tilesets.
 
 ## Quick-start
 These instructions give you a setup based on osm2pgsql-themepark and their shortbread setup. They assume you have PostgreSQL with PostGIS and Python 3.10+ with venv set up, and a recent version of osm2pgsql.
```

### Comparing `tilekiln-0.4.0/pyproject.toml` & `tilekiln-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,40 +22,41 @@
 ]
 keywords = [
     "mvt",
     "openstreetmap",
     "osm",
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dependencies = [
     "Click",
     "fastapi",
     "fs",
     "Jinja2",
+    "pmtiles",
     "prometheus_client",
     "psycopg",
-    "psycopg[pool]",
     "pyyaml",
+    "tqdm",
     "uvicorn",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
 ]
 
 [project.scripts]
-tilekiln = "tilekiln.scripts:cli"
+tilekiln = "tilekiln.main:cli"
 
 [project.urls]
 "Bug Reports" = "https://github.com/pnorman/tilekiln/issues"
 Homepage = "https://github.com/pnorman/tilekiln"
 Source = "https://github.com/pnorman/tilekiln/"
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `tilekiln-0.4.0/PKG-INFO` & `tilekiln-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.3
 Name: tilekiln
-Version: 0.4.0
+Version: 0.5.0
 Summary: A set of command-line utilities to generate and serve Mapbox Vector Tiles (MVTs)
 Project-URL: Bug Reports, https://github.com/pnorman/tilekiln/issues
 Project-URL: Homepage, https://github.com/pnorman/tilekiln
 Project-URL: Source, https://github.com/pnorman/tilekiln/
 Author-email: Paul Norman <osm@paulnorman.ca>
 License-File: LICENSE
 Keywords: mvt,openstreetmap,osm
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: <4,>=3.10
 Requires-Dist: click
 Requires-Dist: fastapi
 Requires-Dist: fs
 Requires-Dist: jinja2
+Requires-Dist: pmtiles
 Requires-Dist: prometheus-client
 Requires-Dist: psycopg
-Requires-Dist: psycopg[pool]
 Requires-Dist: pyyaml
+Requires-Dist: tqdm
 Requires-Dist: uvicorn
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Tilekiln
 
@@ -66,15 +67,15 @@
 ##### `config test`
 Tests a config for validity.
 
 The process will exit with exit code 0 if tilekiln can load the config.
 
 This is intended for build and CI scripts used by configs.
 
-#### `sql`
+##### `config sql`
 Print the SQL for a tile or layer.
 
 Prints the SQL that would be issued to generate a particular tile layer,
 or if no layer is given, the entire tile. This allows manual debugging of
 a tile query.
 
 #### `generate`
@@ -119,24 +120,28 @@
 Delete specific tiles.
 
 A list of z/x/y tiles is read from stdin and those tiles are deleted from
 storage. The entire list is read before deletion starts.
 
 ### Serving commands
 These commands start a HTTP server to serve content.
+#### `serve`
+Commands for tile serving.
+
+All tile serving commands serve tiles and a tilejson over HTTP.
 
-#### `dev`
+##### `dev`
 Starts a server to live-render tiles with no caching, intended for development. It presents a tilejson at `/<id>/tilejson.json`, and for convience `/tilejson.json` redirects to it.
 
-#### `live`
+##### `live`
 Like `serve`, but fall back to live generation if a tile is missing from storage.
 
 It presents a tilejson at `/<id>/tilejson.json`.
 
-#### `serve`
+##### `static`
 Serves tiles from tile storage. This is highly scalable and the preferred mode for production.
 
 It presents a tilejson at `/<id>/tilejson.json`. In the future it will allow serving multiple tilesets.
 
 ## Quick-start
 These instructions give you a setup based on osm2pgsql-themepark and their shortbread setup. They assume you have PostgreSQL with PostGIS and Python 3.10+ with venv set up, and a recent version of osm2pgsql.
```


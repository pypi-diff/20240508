# Comparing `tmp/anystore-0.1.2.tar.gz` & `tmp/anystore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anystore-0.1.2.tar", max compression
+gzip compressed data, was "anystore-0.1.3.tar", max compression
```

## Comparing `anystore-0.1.2.tar` & `anystore-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2024-01-30 17:13:21.261633 anystore-0.1.2/LICENSE
--rw-r--r--   0        0        0     3908 2024-03-13 14:16:50.778774 anystore-0.1.2/README.md
--rw-r--r--   0        0        0      289 2024-04-03 18:27:33.205097 anystore-0.1.2/anystore/__init__.py
--rw-r--r--   0        0        0     2794 2024-03-18 07:58:57.406424 anystore-0.1.2/anystore/cli.py
--rw-r--r--   0        0        0     1021 2024-04-02 13:08:44.544199 anystore-0.1.2/anystore/decorators.py
--rw-r--r--   0        0        0       48 2024-01-31 04:09:17.694069 anystore-0.1.2/anystore/exceptions.py
--rw-r--r--   0        0        0     2237 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/io.py
--rw-r--r--   0        0        0     1909 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/mixins.py
--rw-r--r--   0        0        0     1321 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/serialize.py
--rw-r--r--   0        0        0      539 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/settings.py
--rw-r--r--   0        0        0     1027 2024-03-13 14:16:50.778774 anystore-0.1.2/anystore/store/__init__.py
--rw-r--r--   0        0        0     3658 2024-03-19 20:18:15.500121 anystore-0.1.2/anystore/store/base.py
--rw-r--r--   0        0        0     1544 2024-03-19 20:18:25.476053 anystore-0.1.2/anystore/store/fs.py
--rw-r--r--   0        0        0     1969 2024-03-13 14:16:50.782774 anystore-0.1.2/anystore/store/redis.py
--rw-r--r--   0        0        0     4307 2024-03-19 20:56:07.690434 anystore-0.1.2/anystore/store/sql.py
--rw-r--r--   0        0        0      150 2024-03-13 14:16:50.782774 anystore-0.1.2/anystore/types.py
--rw-r--r--   0        0        0     1576 2024-03-13 14:16:50.782774 anystore-0.1.2/anystore/util.py
--rw-r--r--   0        0        0     1656 2024-04-03 18:27:33.205097 anystore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5468 1970-01-01 00:00:00.000000 anystore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-30 17:13:21.261633 anystore-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3908 2024-03-13 14:16:50.778774 anystore-0.1.3/README.md
+-rw-r--r--   0        0        0      289 2024-05-08 04:31:30.800774 anystore-0.1.3/anystore/__init__.py
+-rw-r--r--   0        0        0     2794 2024-03-18 07:58:57.406424 anystore-0.1.3/anystore/cli.py
+-rw-r--r--   0        0        0     1021 2024-04-02 13:08:44.544199 anystore-0.1.3/anystore/decorators.py
+-rw-r--r--   0        0        0       48 2024-01-31 04:09:17.694069 anystore-0.1.3/anystore/exceptions.py
+-rw-r--r--   0        0        0     2237 2024-03-13 14:16:50.778774 anystore-0.1.3/anystore/io.py
+-rw-r--r--   0        0        0     1909 2024-03-13 14:16:50.778774 anystore-0.1.3/anystore/mixins.py
+-rw-r--r--   0        0        0     1321 2024-03-13 14:16:50.778774 anystore-0.1.3/anystore/serialize.py
+-rw-r--r--   0        0        0      539 2024-03-13 14:16:50.778774 anystore-0.1.3/anystore/settings.py
+-rw-r--r--   0        0        0     1054 2024-05-07 22:35:49.052329 anystore-0.1.3/anystore/store/__init__.py
+-rw-r--r--   0        0        0     3658 2024-03-19 20:18:15.500121 anystore-0.1.3/anystore/store/base.py
+-rw-r--r--   0        0        0     1544 2024-03-19 20:18:25.476053 anystore-0.1.3/anystore/store/fs.py
+-rw-r--r--   0        0        0     1969 2024-03-13 14:16:50.782774 anystore-0.1.3/anystore/store/redis.py
+-rw-r--r--   0        0        0     4307 2024-03-19 20:56:07.690434 anystore-0.1.3/anystore/store/sql.py
+-rw-r--r--   0        0        0      150 2024-03-13 14:16:50.782774 anystore-0.1.3/anystore/types.py
+-rw-r--r--   0        0        0     1576 2024-03-13 14:16:50.782774 anystore-0.1.3/anystore/util.py
+-rw-r--r--   0        0        0     1661 2024-05-08 04:31:30.800774 anystore-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5464 1970-01-01 00:00:00.000000 anystore-0.1.3/PKG-INFO
```

### Comparing `anystore-0.1.2/LICENSE` & `anystore-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/README.md` & `anystore-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/cli.py` & `anystore-0.1.3/anystore/cli.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/decorators.py` & `anystore-0.1.3/anystore/decorators.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/io.py` & `anystore-0.1.3/anystore/io.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/mixins.py` & `anystore-0.1.3/anystore/mixins.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/serialize.py` & `anystore-0.1.3/anystore/serialize.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/settings.py` & `anystore-0.1.3/anystore/settings.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/store/__init__.py` & `anystore-0.1.3/anystore/store/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     if uri is None:
         if settings.yaml_uri is not None:
             store = BaseStore.from_yaml_uri(settings.yaml_uri, **kwargs)
             return get_store(**store.model_dump())
         if settings.json_uri is not None:
             store = BaseStore.from_json_uri(settings.json_uri, **kwargs)
             return get_store(**store.model_dump())
+        uri = settings.uri
     uri = ensure_uri(uri)
     parsed = urlparse(uri)
     if parsed.scheme == "redis":
         return RedisStore(**kwargs)
     if "sql" in parsed.scheme:
         return SqlStore(**kwargs)
     return Store(**kwargs)
```

### Comparing `anystore-0.1.2/anystore/store/base.py` & `anystore-0.1.3/anystore/store/base.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/store/fs.py` & `anystore-0.1.3/anystore/store/fs.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/store/redis.py` & `anystore-0.1.3/anystore/store/redis.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/store/sql.py` & `anystore-0.1.3/anystore/store/sql.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/anystore/util.py` & `anystore-0.1.3/anystore/util.py`

 * *Files identical despite different names*

### Comparing `anystore-0.1.2/pyproject.toml` & `anystore-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anystore"
-version = "0.1.2"
+version = "0.1.3"
 description = "Store and cache things anywhere"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/anystore"
 repository = "https://github.com/investigativedata/anystore"
 documentation = "https://github.com/investigativedata/anystore"
@@ -32,15 +32,15 @@
 s3fs = ">2023.10,<2025"
 gcsfs = ">2023.10,<2025"
 adlfs = ">2023.10,<2025"
 sqlalchemy = "^2.0.28"
 redis = "^5.0.2"
 fakeredis = "^2.21.1"
 typer = ">=0.9,<0.13"
-pyaml = "^23.12.0"
+pyaml = ">=23.12,<25.0"
 cloudpickle = "^3.0.0"
 pydantic-settings = "^2.2.1"
 rich = "^13.7.0"
 pytest = "^8.0.2"
 cryptography = ">=42.0.4"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `anystore-0.1.2/PKG-INFO` & `anystore-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anystore
-Version: 0.1.2
+Version: 0.1.3
 Summary: Store and cache things anywhere
 Home-page: https://github.com/investigativedata/anystore
 License: GPL-3.0
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.11,<4
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Requires-Dist: banal (>=1.0.6,<2.0.0)
 Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
 Requires-Dist: cryptography (>=42.0.4)
 Requires-Dist: fakeredis (>=2.21.1,<3.0.0)
 Requires-Dist: fsspec (>2023.10,<2025)
 Requires-Dist: gcsfs (>2023.10,<2025)
 Requires-Dist: orjson (>=3.9.15,<4.0.0)
-Requires-Dist: pyaml (>=23.12.0,<24.0.0)
+Requires-Dist: pyaml (>=23.12,<25.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pytest (>=8.0.2,<9.0.0)
 Requires-Dist: redis (>=5.0.2,<6.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: s3fs (>2023.10,<2025)
 Requires-Dist: sqlalchemy (>=2.0.28,<3.0.0)
```


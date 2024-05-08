# Comparing `tmp/squirrel_core-0.20.1.tar.gz` & `tmp/squirrel_core-0.20.1.dev493.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrel_core-0.20.1.tar", max compression
+gzip compressed data, was "squirrel_core-0.20.1.dev493.tar", max compression
```

## Comparing `squirrel_core-0.20.1.tar` & `squirrel_core-0.20.1.dev493.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11348 2024-05-08 14:45:16.353407 squirrel_core-0.20.1/LICENSE
--rw-r--r--   0        0        0     5424 2024-05-08 14:45:16.353407 squirrel_core-0.20.1/README.md
--rw-r--r--   0        0        0     4211 2024-05-08 14:52:08.110163 squirrel_core-0.20.1/pyproject.toml
--rw-r--r--   0        0        0       80 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/__init__.py
--rw-r--r--   0        0        0       49 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/artifact_manager/__init__.py
--rw-r--r--   0        0        0     9406 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/artifact_manager/base.py
--rw-r--r--   0        0        0     1251 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/artifact_manager/drivers.py
--rw-r--r--   0        0        0     9869 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/artifact_manager/filesystem.py
--rw-r--r--   0        0        0     8877 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/artifact_manager/wandb.py
--rw-r--r--   0        0        0     1526 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/benchmark/msgpack_caching.py
--rw-r--r--   0        0        0     3253 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/benchmark/quantify_randomness.py
--rw-r--r--   0        0        0      147 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/catalog/__init__.py
--rw-r--r--   0        0        0    15250 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/catalog/catalog.py
--rw-r--r--   0        0        0      937 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/catalog/source.py
--rw-r--r--   0        0        0     2208 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/catalog/yaml.py
--rw-r--r--   0        0        0      581 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/constants.py
--rw-r--r--   0        0        0      887 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/__init__.py
--rw-r--r--   0        0        0     1182 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/csv.py
--rw-r--r--   0        0        0     4716 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/data_frame.py
--rw-r--r--   0        0        0     8479 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/driver.py
--rw-r--r--   0        0        0      977 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/excel.py
--rw-r--r--   0        0        0     1045 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/feather.py
--rw-r--r--   0        0        0     2330 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/file.py
--rw-r--r--   0        0        0     2396 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/jsonl.py
--rw-r--r--   0        0        0     1303 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/msgpack.py
--rw-r--r--   0        0        0     1203 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/parquet.py
--rw-r--r--   0        0        0     5113 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/source_combiner.py
--rw-r--r--   0        0        0     4030 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/store.py
--rw-r--r--   0        0        0     3230 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/driver/zarr.py
--rw-r--r--   0        0        0        0 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/framework/__init__.py
--rw-r--r--   0        0        0      165 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/framework/exceptions.py
--rw-r--r--   0        0        0     2234 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/framework/io.py
--rw-r--r--   0        0        0       30 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/framework/plugins/__init__.py
--rw-r--r--   0        0        0      788 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/framework/plugins/hookimpl.py
--rw-r--r--   0        0        0      644 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/framework/plugins/hookspec.py
--rw-r--r--   0        0        0     1566 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/framework/plugins/plugin_manager.py
--rw-r--r--   0        0        0      410 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/fsspec/__init__.py
--rw-r--r--   0        0        0     1313 2024-05-08 14:45:16.365408 squirrel_core-0.20.1/squirrel/fsspec/custom_gcsfs.py
--rw-r--r--   0        0        0     2510 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/fsspec/fs.py
--rw-r--r--   0        0        0        0 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/integration_test/__init__.py
--rw-r--r--   0        0        0      466 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/integration_test/conftest.py
--rw-r--r--   0        0        0     1747 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/integration_test/helpers.py
--rw-r--r--   0        0        0     3837 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/integration_test/shared_fixtures.py
--rw-r--r--   0        0        0     5841 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
--rw-r--r--   0        0        0      615 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/iterstream/__init__.py
--rw-r--r--   0        0        0    24732 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/iterstream/base.py
--rw-r--r--   0        0        0     9230 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/iterstream/iterators.py
--rw-r--r--   0        0        0     2289 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/iterstream/metrics.py
--rw-r--r--   0        0        0    10487 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/iterstream/multiplexer.py
--rw-r--r--   0        0        0     6004 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/iterstream/source.py
--rw-r--r--   0        0        0     5829 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/iterstream/torch_composables.py
--rw-r--r--   0        0        0      224 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/py.typed
--rw-r--r--   0        0        0      263 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/serialization/__init__.py
--rw-r--r--   0        0        0     4805 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/serialization/jsonl.py
--rw-r--r--   0        0        0     3471 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/serialization/msgpack.py
--rw-r--r--   0        0        0      750 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/serialization/serializer.py
--rw-r--r--   0        0        0      222 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/store/__init__.py
--rw-r--r--   0        0        0     4588 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/store/filesystem.py
--rw-r--r--   0        0        0     3117 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/store/squirrel_store.py
--rw-r--r--   0        0        0     1880 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/store/store.py
--rw-r--r--   0        0        0      110 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/zarr/__init__.py
--rw-r--r--   0        0        0     6137 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/zarr/group.py
--rw-r--r--   0        0        0     2041 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/zarr/key.py
--rw-r--r--   0        0        0     3794 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/zarr/store.py
--rw-r--r--   0        0        0      832 2024-05-08 14:45:16.369409 squirrel_core-0.20.1/squirrel/zarr/sync.py
--rw-r--r--   0        0        0     8080 1970-01-01 00:00:00.000000 squirrel_core-0.20.1/PKG-INFO
+-rw-r--r--   0        0        0    11348 2024-05-08 14:44:52.870919 squirrel_core-0.20.1.dev493/LICENSE
+-rw-r--r--   0        0        0     5424 2024-05-08 14:44:52.870919 squirrel_core-0.20.1.dev493/README.md
+-rw-r--r--   0        0        0     4218 2024-05-08 14:50:51.312474 squirrel_core-0.20.1.dev493/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/artifact_manager/__init__.py
+-rw-r--r--   0        0        0     9406 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/artifact_manager/base.py
+-rw-r--r--   0        0        0     1251 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/artifact_manager/drivers.py
+-rw-r--r--   0        0        0     9869 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/artifact_manager/filesystem.py
+-rw-r--r--   0        0        0     8877 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/artifact_manager/wandb.py
+-rw-r--r--   0        0        0     1526 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/benchmark/msgpack_caching.py
+-rw-r--r--   0        0        0     3253 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/benchmark/quantify_randomness.py
+-rw-r--r--   0        0        0      147 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/catalog/__init__.py
+-rw-r--r--   0        0        0    15250 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/catalog/catalog.py
+-rw-r--r--   0        0        0      937 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/catalog/source.py
+-rw-r--r--   0        0        0     2208 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/catalog/yaml.py
+-rw-r--r--   0        0        0      581 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/constants.py
+-rw-r--r--   0        0        0      887 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/__init__.py
+-rw-r--r--   0        0        0     1182 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/csv.py
+-rw-r--r--   0        0        0     4716 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/data_frame.py
+-rw-r--r--   0        0        0     8479 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/driver.py
+-rw-r--r--   0        0        0      977 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/excel.py
+-rw-r--r--   0        0        0     1045 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/feather.py
+-rw-r--r--   0        0        0     2330 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/file.py
+-rw-r--r--   0        0        0     2396 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/jsonl.py
+-rw-r--r--   0        0        0     1303 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/msgpack.py
+-rw-r--r--   0        0        0     1203 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/parquet.py
+-rw-r--r--   0        0        0     5113 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/source_combiner.py
+-rw-r--r--   0        0        0     4030 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/store.py
+-rw-r--r--   0        0        0     3230 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/driver/zarr.py
+-rw-r--r--   0        0        0        0 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/framework/__init__.py
+-rw-r--r--   0        0        0      165 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/framework/exceptions.py
+-rw-r--r--   0        0        0     2234 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/framework/io.py
+-rw-r--r--   0        0        0       30 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/framework/plugins/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/framework/plugins/hookimpl.py
+-rw-r--r--   0        0        0      644 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/framework/plugins/hookspec.py
+-rw-r--r--   0        0        0     1566 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/framework/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      410 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/fsspec/__init__.py
+-rw-r--r--   0        0        0     1313 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/fsspec/custom_gcsfs.py
+-rw-r--r--   0        0        0     2510 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/fsspec/fs.py
+-rw-r--r--   0        0        0        0 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/integration_test/__init__.py
+-rw-r--r--   0        0        0      466 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/integration_test/conftest.py
+-rw-r--r--   0        0        0     1747 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/integration_test/helpers.py
+-rw-r--r--   0        0        0     3837 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/integration_test/shared_fixtures.py
+-rw-r--r--   0        0        0     5841 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
+-rw-r--r--   0        0        0      615 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/iterstream/__init__.py
+-rw-r--r--   0        0        0    24732 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/iterstream/base.py
+-rw-r--r--   0        0        0     9230 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/iterstream/iterators.py
+-rw-r--r--   0        0        0     2289 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/iterstream/metrics.py
+-rw-r--r--   0        0        0    10487 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/iterstream/multiplexer.py
+-rw-r--r--   0        0        0     6004 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/iterstream/source.py
+-rw-r--r--   0        0        0     5829 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/iterstream/torch_composables.py
+-rw-r--r--   0        0        0      224 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/py.typed
+-rw-r--r--   0        0        0      263 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/serialization/__init__.py
+-rw-r--r--   0        0        0     4805 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/serialization/jsonl.py
+-rw-r--r--   0        0        0     3471 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/serialization/msgpack.py
+-rw-r--r--   0        0        0      750 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/serialization/serializer.py
+-rw-r--r--   0        0        0      222 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/store/__init__.py
+-rw-r--r--   0        0        0     4588 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/store/filesystem.py
+-rw-r--r--   0        0        0     3117 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/store/squirrel_store.py
+-rw-r--r--   0        0        0     1880 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/store/store.py
+-rw-r--r--   0        0        0      110 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/zarr/__init__.py
+-rw-r--r--   0        0        0     6137 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/zarr/group.py
+-rw-r--r--   0        0        0     2041 2024-05-08 14:44:52.886921 squirrel_core-0.20.1.dev493/squirrel/zarr/key.py
+-rw-r--r--   0        0        0     3794 2024-05-08 14:44:52.890921 squirrel_core-0.20.1.dev493/squirrel/zarr/store.py
+-rw-r--r--   0        0        0      832 2024-05-08 14:44:52.890921 squirrel_core-0.20.1.dev493/squirrel/zarr/sync.py
+-rw-r--r--   0        0        0     8087 1970-01-01 00:00:00.000000 squirrel_core-0.20.1.dev493/PKG-INFO
```

### Comparing `squirrel_core-0.20.1/LICENSE` & `squirrel_core-0.20.1.dev493/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/README.md` & `squirrel_core-0.20.1.dev493/README.md`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/pyproject.toml` & `squirrel_core-0.20.1.dev493/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squirrel-core"
-version = "0.20.1"
+version = "0.20.1-dev493"
 description = "Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way."
 authors = ["Merantix Momentum"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "squirrel"}]
 homepage = "https://merantix-momentum.com/technology/squirrel/"
 repository = "https://github.com/merantix-momentum/squirrel-core"
```

### Comparing `squirrel_core-0.20.1/squirrel/artifact_manager/base.py` & `squirrel_core-0.20.1.dev493/squirrel/artifact_manager/base.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/artifact_manager/drivers.py` & `squirrel_core-0.20.1.dev493/squirrel/artifact_manager/drivers.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/artifact_manager/filesystem.py` & `squirrel_core-0.20.1.dev493/squirrel/artifact_manager/filesystem.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/artifact_manager/wandb.py` & `squirrel_core-0.20.1.dev493/squirrel/artifact_manager/wandb.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/benchmark/msgpack_caching.py` & `squirrel_core-0.20.1.dev493/squirrel/benchmark/msgpack_caching.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/benchmark/quantify_randomness.py` & `squirrel_core-0.20.1.dev493/squirrel/benchmark/quantify_randomness.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/catalog/catalog.py` & `squirrel_core-0.20.1.dev493/squirrel/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/catalog/source.py` & `squirrel_core-0.20.1.dev493/squirrel/catalog/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/catalog/yaml.py` & `squirrel_core-0.20.1.dev493/squirrel/catalog/yaml.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/constants.py` & `squirrel_core-0.20.1.dev493/squirrel/constants.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/__init__.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/csv.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/csv.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/data_frame.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/data_frame.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/driver.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/excel.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/excel.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/feather.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/feather.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/file.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/file.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/jsonl.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/msgpack.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/parquet.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/parquet.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/source_combiner.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/source_combiner.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/store.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/driver/zarr.py` & `squirrel_core-0.20.1.dev493/squirrel/driver/zarr.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/framework/io.py` & `squirrel_core-0.20.1.dev493/squirrel/framework/io.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/framework/plugins/hookimpl.py` & `squirrel_core-0.20.1.dev493/squirrel/framework/plugins/hookimpl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/framework/plugins/hookspec.py` & `squirrel_core-0.20.1.dev493/squirrel/framework/plugins/hookspec.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/framework/plugins/plugin_manager.py` & `squirrel_core-0.20.1.dev493/squirrel/framework/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/fsspec/custom_gcsfs.py` & `squirrel_core-0.20.1.dev493/squirrel/fsspec/custom_gcsfs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/fsspec/fs.py` & `squirrel_core-0.20.1.dev493/squirrel/fsspec/fs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/integration_test/helpers.py` & `squirrel_core-0.20.1.dev493/squirrel/integration_test/helpers.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/integration_test/shared_fixtures.py` & `squirrel_core-0.20.1.dev493/squirrel/integration_test/shared_fixtures.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py` & `squirrel_core-0.20.1.dev493/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/iterstream/__init__.py` & `squirrel_core-0.20.1.dev493/squirrel/iterstream/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/iterstream/base.py` & `squirrel_core-0.20.1.dev493/squirrel/iterstream/base.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/iterstream/iterators.py` & `squirrel_core-0.20.1.dev493/squirrel/iterstream/iterators.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/iterstream/metrics.py` & `squirrel_core-0.20.1.dev493/squirrel/iterstream/metrics.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/iterstream/multiplexer.py` & `squirrel_core-0.20.1.dev493/squirrel/iterstream/multiplexer.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/iterstream/source.py` & `squirrel_core-0.20.1.dev493/squirrel/iterstream/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/iterstream/torch_composables.py` & `squirrel_core-0.20.1.dev493/squirrel/iterstream/torch_composables.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/serialization/jsonl.py` & `squirrel_core-0.20.1.dev493/squirrel/serialization/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/serialization/msgpack.py` & `squirrel_core-0.20.1.dev493/squirrel/serialization/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/serialization/serializer.py` & `squirrel_core-0.20.1.dev493/squirrel/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/store/filesystem.py` & `squirrel_core-0.20.1.dev493/squirrel/store/filesystem.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/store/squirrel_store.py` & `squirrel_core-0.20.1.dev493/squirrel/store/squirrel_store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/store/store.py` & `squirrel_core-0.20.1.dev493/squirrel/store/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/zarr/group.py` & `squirrel_core-0.20.1.dev493/squirrel/zarr/group.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/zarr/key.py` & `squirrel_core-0.20.1.dev493/squirrel/zarr/key.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/zarr/store.py` & `squirrel_core-0.20.1.dev493/squirrel/zarr/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/squirrel/zarr/sync.py` & `squirrel_core-0.20.1.dev493/squirrel/zarr/sync.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.20.1/PKG-INFO` & `squirrel_core-0.20.1.dev493/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squirrel-core
-Version: 0.20.1
+Version: 0.20.1.dev493
 Summary: Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way.
 Home-page: https://merantix-momentum.com/technology/squirrel/
 License: Apache 2.0
 Author: Merantix Momentum
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```


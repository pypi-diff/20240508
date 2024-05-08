# Comparing `tmp/squirrel_core-0.19.8.dev649345.tar.gz` & `tmp/squirrel_core-0.19.8.dev8920.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrel_core-0.19.8.dev649345.tar", max compression
+gzip compressed data, was "squirrel_core-0.19.8.dev8920.tar", max compression
```

## Comparing `squirrel_core-0.19.8.dev649345.tar` & `squirrel_core-0.19.8.dev8920.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11348 2024-05-08 14:24:50.388273 squirrel_core-0.19.8.dev649345/LICENSE
--rw-r--r--   0        0        0     5424 2024-05-08 14:24:50.388273 squirrel_core-0.19.8.dev649345/README.md
--rw-r--r--   0        0        0     4221 2024-05-08 14:30:57.913123 squirrel_core-0.19.8.dev649345/pyproject.toml
--rw-r--r--   0        0        0       80 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/__init__.py
--rw-r--r--   0        0        0       49 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/artifact_manager/__init__.py
--rw-r--r--   0        0        0     9406 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/artifact_manager/base.py
--rw-r--r--   0        0        0     1251 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/artifact_manager/drivers.py
--rw-r--r--   0        0        0     9869 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/artifact_manager/filesystem.py
--rw-r--r--   0        0        0     8877 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/artifact_manager/wandb.py
--rw-r--r--   0        0        0     1526 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/benchmark/msgpack_caching.py
--rw-r--r--   0        0        0     3253 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/benchmark/quantify_randomness.py
--rw-r--r--   0        0        0      147 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/catalog/__init__.py
--rw-r--r--   0        0        0    15250 2024-05-08 14:24:50.400274 squirrel_core-0.19.8.dev649345/squirrel/catalog/catalog.py
--rw-r--r--   0        0        0      937 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/catalog/source.py
--rw-r--r--   0        0        0     2208 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/catalog/yaml.py
--rw-r--r--   0        0        0      581 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/constants.py
--rw-r--r--   0        0        0      887 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/__init__.py
--rw-r--r--   0        0        0     1182 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/csv.py
--rw-r--r--   0        0        0     4716 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/data_frame.py
--rw-r--r--   0        0        0     8479 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/driver.py
--rw-r--r--   0        0        0      977 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/excel.py
--rw-r--r--   0        0        0     1045 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/feather.py
--rw-r--r--   0        0        0     2330 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/file.py
--rw-r--r--   0        0        0     2396 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/jsonl.py
--rw-r--r--   0        0        0     1303 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/msgpack.py
--rw-r--r--   0        0        0     1203 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/parquet.py
--rw-r--r--   0        0        0     5113 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/source_combiner.py
--rw-r--r--   0        0        0     4030 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/store.py
--rw-r--r--   0        0        0     3230 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/driver/zarr.py
--rw-r--r--   0        0        0        0 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/framework/__init__.py
--rw-r--r--   0        0        0      165 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/framework/exceptions.py
--rw-r--r--   0        0        0     2234 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/framework/io.py
--rw-r--r--   0        0        0       30 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/framework/plugins/__init__.py
--rw-r--r--   0        0        0      788 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/framework/plugins/hookimpl.py
--rw-r--r--   0        0        0      644 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/framework/plugins/hookspec.py
--rw-r--r--   0        0        0     1566 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/framework/plugins/plugin_manager.py
--rw-r--r--   0        0        0      410 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/fsspec/__init__.py
--rw-r--r--   0        0        0     1313 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/fsspec/custom_gcsfs.py
--rw-r--r--   0        0        0     2510 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/fsspec/fs.py
--rw-r--r--   0        0        0        0 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/integration_test/__init__.py
--rw-r--r--   0        0        0      466 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/integration_test/conftest.py
--rw-r--r--   0        0        0     1747 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/integration_test/helpers.py
--rw-r--r--   0        0        0     3837 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/integration_test/shared_fixtures.py
--rw-r--r--   0        0        0     5841 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
--rw-r--r--   0        0        0      615 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/iterstream/__init__.py
--rw-r--r--   0        0        0    24732 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/iterstream/base.py
--rw-r--r--   0        0        0     9230 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/iterstream/iterators.py
--rw-r--r--   0        0        0     2289 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/iterstream/metrics.py
--rw-r--r--   0        0        0    10487 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/iterstream/multiplexer.py
--rw-r--r--   0        0        0     6004 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/iterstream/source.py
--rw-r--r--   0        0        0     5829 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/iterstream/torch_composables.py
--rw-r--r--   0        0        0      224 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/py.typed
--rw-r--r--   0        0        0      263 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/serialization/__init__.py
--rw-r--r--   0        0        0     4805 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/serialization/jsonl.py
--rw-r--r--   0        0        0     3471 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/serialization/msgpack.py
--rw-r--r--   0        0        0      750 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/serialization/serializer.py
--rw-r--r--   0        0        0      222 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/store/__init__.py
--rw-r--r--   0        0        0     4588 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/store/filesystem.py
--rw-r--r--   0        0        0     3117 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/store/squirrel_store.py
--rw-r--r--   0        0        0     1880 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/store/store.py
--rw-r--r--   0        0        0      110 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/zarr/__init__.py
--rw-r--r--   0        0        0     6137 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/zarr/group.py
--rw-r--r--   0        0        0     2041 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/zarr/key.py
--rw-r--r--   0        0        0     3794 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/zarr/store.py
--rw-r--r--   0        0        0      832 2024-05-08 14:24:50.404275 squirrel_core-0.19.8.dev649345/squirrel/zarr/sync.py
--rw-r--r--   0        0        0     8090 1970-01-01 00:00:00.000000 squirrel_core-0.19.8.dev649345/PKG-INFO
+-rw-r--r--   0        0        0    11348 2024-01-15 11:49:27.418613 squirrel_core-0.19.8.dev8920/LICENSE
+-rw-r--r--   0        0        0     5424 2024-01-15 11:49:27.418613 squirrel_core-0.19.8.dev8920/README.md
+-rw-r--r--   0        0        0     4318 2024-01-15 11:54:54.064434 squirrel_core-0.19.8.dev8920/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/__init__.py
+-rw-r--r--   0        0        0       49 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/artifact_manager/__init__.py
+-rw-r--r--   0        0        0     9406 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/artifact_manager/base.py
+-rw-r--r--   0        0        0     1251 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/artifact_manager/drivers.py
+-rw-r--r--   0        0        0     9869 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/artifact_manager/filesystem.py
+-rw-r--r--   0        0        0     8877 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/artifact_manager/wandb.py
+-rw-r--r--   0        0        0     1526 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/benchmark/msgpack_caching.py
+-rw-r--r--   0        0        0     3253 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/benchmark/quantify_randomness.py
+-rw-r--r--   0        0        0      147 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/catalog/__init__.py
+-rw-r--r--   0        0        0    15250 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/catalog/catalog.py
+-rw-r--r--   0        0        0      937 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/catalog/source.py
+-rw-r--r--   0        0        0     2208 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/catalog/yaml.py
+-rw-r--r--   0        0        0      581 2024-01-15 11:49:27.426613 squirrel_core-0.19.8.dev8920/squirrel/constants.py
+-rw-r--r--   0        0        0      887 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/__init__.py
+-rw-r--r--   0        0        0     1182 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/csv.py
+-rw-r--r--   0        0        0     4716 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/data_frame.py
+-rw-r--r--   0        0        0     8479 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/driver.py
+-rw-r--r--   0        0        0      977 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/excel.py
+-rw-r--r--   0        0        0     1045 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/feather.py
+-rw-r--r--   0        0        0     2330 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/file.py
+-rw-r--r--   0        0        0     2396 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/jsonl.py
+-rw-r--r--   0        0        0     1303 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/msgpack.py
+-rw-r--r--   0        0        0     1203 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/parquet.py
+-rw-r--r--   0        0        0     5113 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/source_combiner.py
+-rw-r--r--   0        0        0     4030 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/store.py
+-rw-r--r--   0        0        0     3230 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/driver/zarr.py
+-rw-r--r--   0        0        0        0 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/framework/__init__.py
+-rw-r--r--   0        0        0      165 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/framework/exceptions.py
+-rw-r--r--   0        0        0     2234 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/framework/io.py
+-rw-r--r--   0        0        0       30 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/framework/plugins/__init__.py
+-rw-r--r--   0        0        0      788 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/framework/plugins/hookimpl.py
+-rw-r--r--   0        0        0      644 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/framework/plugins/hookspec.py
+-rw-r--r--   0        0        0     1566 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/framework/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      410 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/fsspec/__init__.py
+-rw-r--r--   0        0        0     1313 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/fsspec/custom_gcsfs.py
+-rw-r--r--   0        0        0     2510 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/fsspec/fs.py
+-rw-r--r--   0        0        0        0 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/integration_test/__init__.py
+-rw-r--r--   0        0        0      466 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/integration_test/conftest.py
+-rw-r--r--   0        0        0     1747 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/integration_test/helpers.py
+-rw-r--r--   0        0        0     3837 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/integration_test/shared_fixtures.py
+-rw-r--r--   0        0        0     5841 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py
+-rw-r--r--   0        0        0      615 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/iterstream/__init__.py
+-rw-r--r--   0        0        0    24732 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/iterstream/base.py
+-rw-r--r--   0        0        0     9230 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/iterstream/iterators.py
+-rw-r--r--   0        0        0     2289 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/iterstream/metrics.py
+-rw-r--r--   0        0        0    10487 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/iterstream/multiplexer.py
+-rw-r--r--   0        0        0     6004 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/iterstream/source.py
+-rw-r--r--   0        0        0     5829 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/iterstream/torch_composables.py
+-rw-r--r--   0        0        0      224 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/py.typed
+-rw-r--r--   0        0        0      263 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/serialization/__init__.py
+-rw-r--r--   0        0        0     4805 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/serialization/jsonl.py
+-rw-r--r--   0        0        0     3471 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/serialization/msgpack.py
+-rw-r--r--   0        0        0      750 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/serialization/serializer.py
+-rw-r--r--   0        0        0      222 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/store/__init__.py
+-rw-r--r--   0        0        0     4588 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/store/filesystem.py
+-rw-r--r--   0        0        0     3117 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/store/squirrel_store.py
+-rw-r--r--   0        0        0     1880 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/store/store.py
+-rw-r--r--   0        0        0      110 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/zarr/__init__.py
+-rw-r--r--   0        0        0     6137 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/zarr/group.py
+-rw-r--r--   0        0        0     2041 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/zarr/key.py
+-rw-r--r--   0        0        0     3794 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/zarr/store.py
+-rw-r--r--   0        0        0      832 2024-01-15 11:49:27.430614 squirrel_core-0.19.8.dev8920/squirrel/zarr/sync.py
+-rw-r--r--   0        0        0     8132 1970-01-01 00:00:00.000000 squirrel_core-0.19.8.dev8920/PKG-INFO
```

### Comparing `squirrel_core-0.19.8.dev649345/LICENSE` & `squirrel_core-0.19.8.dev8920/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/README.md` & `squirrel_core-0.19.8.dev8920/README.md`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/pyproject.toml` & `squirrel_core-0.19.8.dev8920/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squirrel-core"
-version = "0.19.8-dev649345"
+version = "0.19.8-dev8920"
 description = "Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way."
 authors = ["Merantix Momentum"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "squirrel"}]
 homepage = "https://merantix-momentum.com/technology/squirrel/"
 repository = "https://github.com/merantix-momentum/squirrel-core"
@@ -16,43 +16,43 @@
     "Typing :: Typed",
 ]
 
 [tool.poetry.plugins."fsspec.specs"]
 "gs" = "squirrel.fsspec.custom_gcsfs.CustomGCSFileSystem"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 aiohttp = ">=3.8.4"    # dependabot: GHSA-q3qx-c6g2-7pw2
 fsspec = ">=2021.7.0"
 mako = ">=1.2.4"    # dependabot: GHSA-v973-fxgf-6xhp
 msgpack = ">=1.0.4"
 msgpack-numpy = ">=0.4.8"
 more-itertools = ">=9.0.0"
 numpy = ">=1.23.5"
 oauthlib = ">=3.2.2"   # dependabot: GHSA-3pgj-pg6c-r5p7
+pandas = "<=1.5.3"    # pin for dask compatibility (afterwards core.strings.Stringmethods is not available anymore)
 pluggy = ">=1.0.0"
 pyjwt = ">=2.6.0"   # dependabot: GHSA-ffqj-6fqr-9h24
 ruamel-yaml = ">=0.17.21"
 tqdm = ">=4.64.1"   # dependabot: GHSA-r7q7-xcjw-qx8q
 urllib3 = ">=1.25.4,<1.27" # workaround for: https://github.com/python-poetry/poetry-plugin-export/issues/183
 
 adlfs = {version = "<2021.10", optional = true}
-dask = {version = ">=2023.2.0", optional = true, extras = ["dataframe", "distributed"]}  # dependabot: GHSA-hwqr-f3v9-hwxr
+dask = {version = ">=2021.10.0", optional = true, extras = ["dataframe", "distributed"]}  # dependabot: GHSA-hwqr-f3v9-hwxr
 gcsfs = {version = ">=2021.7.0", optional = true}
 numba = {version = ">=0.56.4", optional = true}
 odfpy = {version = ">=1.4.1", optional = true}
 openpyxl = {version = ">=3.1.1", optional = true}   # dependabot: GHSA-chqf-hx79-gxc6
 pyarrow = {version = ">=14.0.1", optional = true}  # dependabot: GHSA-5wvp-7f3h-6wmm
 pyxlsb = {version = ">=1.0.10", optional = true}
 s3fs = {version = ">=2021.7.0", optional = true}
 torch = {version = ">=1.13.1", optional = true}     # dependabot: GHSA-47fc-vmwq-366v
 wandb = {version = "*", optional = true}
 xlrd = {version = ">=2.0.1", optional = true}
 zarr = {version = ">=2.10.3", optional = true}
-pandas = "^2.0.3"
 
 [tool.poetry.group.dev.dependencies]
 # dev dependencies pinned for faster resolution
 autopep8 = "2.0.4"
 black = "23.12.0"
 faker = "21.0.0"
 hypothesis = "6.92.1"
```

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/artifact_manager/base.py` & `squirrel_core-0.19.8.dev8920/squirrel/artifact_manager/base.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/artifact_manager/drivers.py` & `squirrel_core-0.19.8.dev8920/squirrel/artifact_manager/drivers.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/artifact_manager/filesystem.py` & `squirrel_core-0.19.8.dev8920/squirrel/artifact_manager/filesystem.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/artifact_manager/wandb.py` & `squirrel_core-0.19.8.dev8920/squirrel/artifact_manager/wandb.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/benchmark/msgpack_caching.py` & `squirrel_core-0.19.8.dev8920/squirrel/benchmark/msgpack_caching.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/benchmark/quantify_randomness.py` & `squirrel_core-0.19.8.dev8920/squirrel/benchmark/quantify_randomness.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/catalog/catalog.py` & `squirrel_core-0.19.8.dev8920/squirrel/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/catalog/source.py` & `squirrel_core-0.19.8.dev8920/squirrel/catalog/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/catalog/yaml.py` & `squirrel_core-0.19.8.dev8920/squirrel/catalog/yaml.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/constants.py` & `squirrel_core-0.19.8.dev8920/squirrel/constants.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/__init__.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/csv.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/csv.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/data_frame.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/data_frame.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/driver.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/driver.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/excel.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/excel.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/feather.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/feather.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/file.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/file.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/jsonl.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/msgpack.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/parquet.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/parquet.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/source_combiner.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/source_combiner.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/store.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/driver/zarr.py` & `squirrel_core-0.19.8.dev8920/squirrel/driver/zarr.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/framework/io.py` & `squirrel_core-0.19.8.dev8920/squirrel/framework/io.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/framework/plugins/hookimpl.py` & `squirrel_core-0.19.8.dev8920/squirrel/framework/plugins/hookimpl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/framework/plugins/hookspec.py` & `squirrel_core-0.19.8.dev8920/squirrel/framework/plugins/hookspec.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/framework/plugins/plugin_manager.py` & `squirrel_core-0.19.8.dev8920/squirrel/framework/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/fsspec/custom_gcsfs.py` & `squirrel_core-0.19.8.dev8920/squirrel/fsspec/custom_gcsfs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/fsspec/fs.py` & `squirrel_core-0.19.8.dev8920/squirrel/fsspec/fs.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/integration_test/helpers.py` & `squirrel_core-0.19.8.dev8920/squirrel/integration_test/helpers.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/integration_test/shared_fixtures.py` & `squirrel_core-0.19.8.dev8920/squirrel/integration_test/shared_fixtures.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py` & `squirrel_core-0.19.8.dev8920/squirrel/integration_test/test_jsonl/test_torch_distibuted_loading.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/iterstream/__init__.py` & `squirrel_core-0.19.8.dev8920/squirrel/iterstream/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/iterstream/base.py` & `squirrel_core-0.19.8.dev8920/squirrel/iterstream/base.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/iterstream/iterators.py` & `squirrel_core-0.19.8.dev8920/squirrel/iterstream/iterators.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/iterstream/metrics.py` & `squirrel_core-0.19.8.dev8920/squirrel/iterstream/metrics.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/iterstream/multiplexer.py` & `squirrel_core-0.19.8.dev8920/squirrel/iterstream/multiplexer.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/iterstream/source.py` & `squirrel_core-0.19.8.dev8920/squirrel/iterstream/source.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/iterstream/torch_composables.py` & `squirrel_core-0.19.8.dev8920/squirrel/iterstream/torch_composables.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/serialization/jsonl.py` & `squirrel_core-0.19.8.dev8920/squirrel/serialization/jsonl.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/serialization/msgpack.py` & `squirrel_core-0.19.8.dev8920/squirrel/serialization/msgpack.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/serialization/serializer.py` & `squirrel_core-0.19.8.dev8920/squirrel/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/store/filesystem.py` & `squirrel_core-0.19.8.dev8920/squirrel/store/filesystem.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/store/squirrel_store.py` & `squirrel_core-0.19.8.dev8920/squirrel/store/squirrel_store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/store/store.py` & `squirrel_core-0.19.8.dev8920/squirrel/store/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/zarr/group.py` & `squirrel_core-0.19.8.dev8920/squirrel/zarr/group.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/zarr/key.py` & `squirrel_core-0.19.8.dev8920/squirrel/zarr/key.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/zarr/store.py` & `squirrel_core-0.19.8.dev8920/squirrel/zarr/store.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/squirrel/zarr/sync.py` & `squirrel_core-0.19.8.dev8920/squirrel/zarr/sync.py`

 * *Files identical despite different names*

### Comparing `squirrel_core-0.19.8.dev649345/PKG-INFO` & `squirrel_core-0.19.8.dev8920/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: squirrel-core
-Version: 0.19.8.dev649345
+Version: 0.19.8.dev8920
 Summary: Squirrel is a Python library that enables ML teams to share, load, and transform data in a collaborative, flexible and efficient way.
 Home-page: https://merantix-momentum.com/technology/squirrel/
 License: Apache 2.0
 Author: Merantix Momentum
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Provides-Extra: all
 Provides-Extra: azure
@@ -25,27 +26,27 @@
 Provides-Extra: parquet
 Provides-Extra: s3
 Provides-Extra: torch
 Provides-Extra: wandb
 Provides-Extra: zarr
 Requires-Dist: adlfs (<2021.10) ; extra == "azure" or extra == "all"
 Requires-Dist: aiohttp (>=3.8.4)
-Requires-Dist: dask[dataframe,distributed] (>=2023.2.0) ; extra == "dask" or extra == "all"
+Requires-Dist: dask[dataframe,distributed] (>=2021.10.0) ; extra == "dask" or extra == "all"
 Requires-Dist: fsspec (>=2021.7.0)
 Requires-Dist: gcsfs (>=2021.7.0) ; extra == "gcp" or extra == "all"
 Requires-Dist: mako (>=1.2.4)
 Requires-Dist: more-itertools (>=9.0.0)
 Requires-Dist: msgpack (>=1.0.4)
 Requires-Dist: msgpack-numpy (>=0.4.8)
 Requires-Dist: numba (>=0.56.4) ; extra == "numba" or extra == "all"
 Requires-Dist: numpy (>=1.23.5)
 Requires-Dist: oauthlib (>=3.2.2)
 Requires-Dist: odfpy (>=1.4.1) ; extra == "excel" or extra == "all"
 Requires-Dist: openpyxl (>=3.1.1) ; extra == "excel" or extra == "all"
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: pandas (<=1.5.3)
 Requires-Dist: pluggy (>=1.0.0)
 Requires-Dist: pyarrow (>=14.0.1) ; extra == "feather" or extra == "parquet" or extra == "all"
 Requires-Dist: pyjwt (>=2.6.0)
 Requires-Dist: pyxlsb (>=1.0.10) ; extra == "excel" or extra == "all"
 Requires-Dist: ruamel-yaml (>=0.17.21)
 Requires-Dist: s3fs (>=2021.7.0) ; extra == "s3" or extra == "all"
 Requires-Dist: torch (>=1.13.1) ; extra == "torch" or extra == "all"
```


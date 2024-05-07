# Comparing `tmp/dvcx-0.76.0.tar.gz` & `tmp/dvcx-0.77.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.76.0.tar", last modified: Tue Apr 23 06:01:41 2024, max compression
+gzip compressed data, was "dvcx-0.77.0.tar", last modified: Tue May  7 22:04:32 2024, max compression
```

## Comparing `dvcx-0.76.0.tar` & `dvcx-0.77.0.tar`

### file list

```diff
@@ -1,232 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.988620 dvcx-0.76.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-23 06:01:32.000000 dvcx-0.76.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 06:01:32.000000 dvcx-0.76.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.940620 dvcx-0.76.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.940620 dvcx-0.76.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.944620 dvcx-0.76.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-23 06:01:32.000000 dvcx-0.76.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-23 06:01:32.000000 dvcx-0.76.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-23 06:01:32.000000 dvcx-0.76.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.944620 dvcx-0.76.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-23 06:01:32.000000 dvcx-0.76.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 06:01:32.000000 dvcx-0.76.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-23 06:01:32.000000 dvcx-0.76.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-23 06:01:32.000000 dvcx-0.76.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-23 06:01:32.000000 dvcx-0.76.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.944620 dvcx-0.76.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-23 06:01:32.000000 dvcx-0.76.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-23 06:01:32.000000 dvcx-0.76.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-04-23 06:01:32.000000 dvcx-0.76.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-23 06:01:41.988620 dvcx-0.76.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-23 06:01:32.000000 dvcx-0.76.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.944620 dvcx-0.76.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-23 06:01:32.000000 dvcx-0.76.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.948620 dvcx-0.76.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.948620 dvcx-0.76.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.948620 dvcx-0.76.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.952620 dvcx-0.76.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 06:01:32.000000 dvcx-0.76.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-23 06:01:32.000000 dvcx-0.76.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-23 06:01:32.000000 dvcx-0.76.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:01:41.988620 dvcx-0.76.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.932620 dvcx-0.76.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.956620 dvcx-0.76.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.956620 dvcx-0.76.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71363 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    30133 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.956620 dvcx-0.76.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.960620 dvcx-0.76.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45015 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30640 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    33101 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15516 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.964620 dvcx-0.76.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/param.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7644 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.964620 dvcx-0.76.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    57821 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.964620 dvcx-0.76.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.964620 dvcx-0.76.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.968620 dvcx-0.76.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.968620 dvcx-0.76.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.968620 dvcx-0.76.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-04-23 06:01:32.000000 dvcx-0.76.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.980620 dvcx-0.76.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 06:01:41.000000 dvcx-0.76.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.968620 dvcx-0.76.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.972620 dvcx-0.76.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.972620 dvcx-0.76.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34442 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   112414 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/func/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/test_cli_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.976620 dvcx-0.76.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.976620 dvcx-0.76.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.980620 dvcx-0.76.0/tests/unit/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:01:41.980620 dvcx-0.76.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-23 06:01:32.000000 dvcx-0.76.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.505053 dvcx-0.77.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 22:04:27.000000 dvcx-0.77.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 22:04:27.000000 dvcx-0.77.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.457053 dvcx-0.77.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.457053 dvcx-0.77.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.461053 dvcx-0.77.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 22:04:27.000000 dvcx-0.77.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-07 22:04:27.000000 dvcx-0.77.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-07 22:04:27.000000 dvcx-0.77.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.461053 dvcx-0.77.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 22:04:27.000000 dvcx-0.77.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 22:04:27.000000 dvcx-0.77.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-07 22:04:27.000000 dvcx-0.77.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-07 22:04:27.000000 dvcx-0.77.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-07 22:04:27.000000 dvcx-0.77.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.461053 dvcx-0.77.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-07 22:04:27.000000 dvcx-0.77.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-07 22:04:27.000000 dvcx-0.77.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-07 22:04:27.000000 dvcx-0.77.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-07 22:04:32.505053 dvcx-0.77.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-07 22:04:27.000000 dvcx-0.77.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.461053 dvcx-0.77.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-07 22:04:27.000000 dvcx-0.77.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.465053 dvcx-0.77.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.465053 dvcx-0.77.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.465053 dvcx-0.77.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.465053 dvcx-0.77.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 22:04:27.000000 dvcx-0.77.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-07 22:04:27.000000 dvcx-0.77.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-07 22:04:27.000000 dvcx-0.77.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 22:04:32.505053 dvcx-0.77.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.453053 dvcx-0.77.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.469053 dvcx-0.77.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.473053 dvcx-0.77.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72292 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30885 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.473053 dvcx-0.77.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.473053 dvcx-0.77.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45366 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30660 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34621 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15901 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.477053 dvcx-0.77.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10309 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/tar_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60425 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.481053 dvcx-0.77.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.485053 dvcx-0.77.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-07 22:04:27.000000 dvcx-0.77.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.497053 dvcx-0.77.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 22:04:32.000000 dvcx-0.77.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.485053 dvcx-0.77.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.485053 dvcx-0.77.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14464 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.489053 dvcx-0.77.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35673 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113295 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26682 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.489053 dvcx-0.77.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.493053 dvcx-0.77.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.497053 dvcx-0.77.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15983 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.497053 dvcx-0.77.0/tests/unit/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 22:04:32.497053 dvcx-0.77.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_catalog_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-07 22:04:27.000000 dvcx-0.77.0/tests/utils.py
```

### Comparing `dvcx-0.76.0/.cruft.json` & `dvcx-0.77.0/.cruft.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'6925fc738cd3d7086ab4a2efdd1a3ad56af54691'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "80e68ce58293580b73e5de011f71b2ce5fbd9dda",
+    "commit": "6925fc738cd3d7086ab4a2efdd1a3ad56af54691",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/iterative/py-template",
             "author": "Dmitry Petrov",
             "copyright_year": "2022",
             "development_status": "Development Status :: 2 - Pre-Alpha",
             "docs": "False",
```

### Comparing `dvcx-0.76.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.77.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.77.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/.github/workflows/benchmarks.yml` & `dvcx-0.77.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/.github/workflows/release.yml` & `dvcx-0.77.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/.github/workflows/tests.yml` & `dvcx-0.77.0/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
       fail-fast: false
       matrix:
         os: [ubuntu-latest-8-cores]
         pyv: ['3.9', '3.10', '3.11', '3.12']
         include:
           - os: macos-latest
             pyv: '3.9'
-          - os: macos-14
+          - os: macos-latest
             pyv: '3.12'
           - os: windows-latest-8-cores
             pyv: '3.9'
           - os: windows-latest-8-cores
             pyv: '3.12'
 
     steps:
```

### Comparing `dvcx-0.76.0/.gitignore` & `dvcx-0.77.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/.pre-commit-config.yaml` & `dvcx-0.77.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 default_language_version:
   python: python3
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
         exclude: '^examples/'
       - id: check-executables-have-shebangs
       - id: check-json
@@ -17,15 +17,15 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
         exclude: '^LICENSES/'
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.3.5'
+    rev: 'v0.4.2'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.5
     hooks:
```

### Comparing `dvcx-0.76.0/CODE_OF_CONDUCT.rst` & `dvcx-0.77.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/CONTRIBUTING.rst` & `dvcx-0.77.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/LICENSE` & `dvcx-0.77.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/LICENSES/Apache-2.0.txt` & `dvcx-0.77.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.77.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/LICENSES/Python-2.0.txt` & `dvcx-0.77.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/PKG-INFO` & `dvcx-0.77.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.76.0
+Version: 0.77.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,14 +15,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: tomlkit
 Requires-Dist: tqdm
 Requires-Dist: pandas
+Requires-Dist: typing-extensions
 Requires-Dist: python-dateutil>=2
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: s3fs>=2024.2.0
 Requires-Dist: gcsfs>=2024.2.0
 Requires-Dist: adlfs>=2024.2.0
 Requires-Dist: dvc-data<4,>=3.10
 Requires-Dist: dvc-objects<6,>=4
@@ -66,15 +67,15 @@
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
 Requires-Dist: open_clip_torch; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: dvcx[tests]; extra == "dev"
-Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 
 |PyPI| |Status| |Python Version| |License|
 
 |Tests| |Codecov| |pre-commit| |Black|
```

### Comparing `dvcx-0.76.0/README.rst` & `dvcx-0.77.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/docs/udfs.md` & `dvcx-0.77.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/blip2_image_desc_lib.py` & `dvcx-0.77.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/clip.py` & `dvcx-0.77.0/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/common_sql_functions.py` & `dvcx-0.77.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/dir_expansion.py` & `dvcx-0.77.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/hf_pipeline.py` & `dvcx-0.77.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/llava2_image_desc_lib.py` & `dvcx-0.77.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/loader.py` & `dvcx-0.77.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/neurips/README` & `dvcx-0.77.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/neurips/distance_to_query.py` & `dvcx-0.77.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/neurips/llm_chat.py` & `dvcx-0.77.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/neurips/single_query.py` & `dvcx-0.77.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/neurips/text_loaders.py` & `dvcx-0.77.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/openai_image_desc_lib.py` & `dvcx-0.77.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/openimage-detect.py` & `dvcx-0.77.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/pose_detection.py` & `dvcx-0.77.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/torch-loader.py` & `dvcx-0.77.0/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/udfs/batching.py` & `dvcx-0.77.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/udfs/image_transformation.py` & `dvcx-0.77.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/udfs/parallel.py` & `dvcx-0.77.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/udfs/simple.py` & `dvcx-0.77.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/udfs/stateful.py` & `dvcx-0.77.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/udfs/stateful_similarity.py` & `dvcx-0.77.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/unstructured-text.py` & `dvcx-0.77.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/wds.py` & `dvcx-0.77.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/wds_filtered.py` & `dvcx-0.77.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/wds_meta.py` & `dvcx-0.77.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/zalando/zalando_clip.py` & `dvcx-0.77.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.77.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/noxfile.py` & `dvcx-0.77.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/pyproject.toml` & `dvcx-0.77.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 requires-python = ">=3.9"
 dynamic = ["version"]
 dependencies = [
   "pyyaml",
   "tomlkit",
   "tqdm",
   "pandas",
+  "typing-extensions",
   "python-dateutil>=2",
   "attrs>=21.3.0",
   "s3fs>=2024.2.0",
   "gcsfs>=2024.2.0",
   "adlfs>=2024.2.0",
   "dvc-data>=3.10,<4",
   "dvc-objects>=4,<6",
@@ -76,15 +77,15 @@
   "numpy",
   "open_clip_torch",
   "aiotools>=1.7.0",
   "requests-mock"
 ]
 dev = [
   "dvcx[tests]",
-  "mypy==1.9.0",
+  "mypy==1.10.0",
   "types-python-dateutil",
   "types-PyYAML",
   "types-requests"
 ]
 
 [project.urls]
 Issues = "https://github.com/iterative/dvcx/issues"
```

### Comparing `dvcx-0.76.0/src/dvcx/asyn.py` & `dvcx-0.77.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/cache.py` & `dvcx-0.77.0/src/dvcx/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
     def contains(self, uid: UniqueId) -> bool:
         return self.odb.exists(uid.get_hash())
 
     def path_from_checksum(self, checksum: str) -> str:
         assert checksum
         return self.odb.oid_to_path(checksum)
 
+    def remove(self, uid: UniqueId) -> None:
+        self.odb.delete(uid.get_hash())
+
     async def download(self, uid: UniqueId, client: "Client", callback=None) -> None:
         from_path = f"{uid.storage}/{uid.path}"
         from dvc_objects.fs.utils import tmp_fname
 
         odb_fs = self.odb.fs
         tmp_info = odb_fs.join(self.odb.tmp_dir, tmp_fname())  # type: ignore[arg-type]
         size = uid.size
```

### Comparing `dvcx-0.76.0/src/dvcx/catalog/catalog.py` & `dvcx-0.77.0/src/dvcx/catalog/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -605,19 +605,15 @@
             result.warehouse = None
         return result
 
     @classmethod
     def generate_query_dataset_name(cls) -> str:
         return f"{QUERY_DATASET_PREFIX}_{uuid4().hex}"
 
-    def compile_query_script(self, script: str, save=False) -> str:
-        wrapper_function = "query_wrapper_print"
-        if save:
-            wrapper_function = "query_wrapper_save"
-
+    def compile_query_script(self, script: str) -> str:
         code_ast = ast.parse(script)
         if code_ast.body:
             last_expr = code_ast.body[-1]
             if isinstance(last_expr, Expr):
                 new_expressions = [
                     Import(names=[alias(name="dvcx.query.dataset", asname=None)]),
                     Expr(
@@ -628,15 +624,15 @@
                                         value=Name(id="dvcx", ctx=Load()),
                                         attr="query",
                                         ctx=Load(),
                                     ),
                                     attr="dataset",
                                     ctx=Load(),
                                 ),
-                                attr=wrapper_function,
+                                attr="query_wrapper",
                                 ctx=Load(),
                             ),
                             args=[last_expr],
                             keywords=[],
                         )
                     ),
                 ]
@@ -1081,16 +1077,35 @@
 
         if create_rows_table:
             table_name = self.warehouse.dataset_table_name(dataset.name, version)
             self.warehouse.create_dataset_rows_table(
                 table_name, custom_columns=custom_columns
             )
 
+            self.update_dataset_version_with_stats(dataset, version)
+
         return dataset
 
+    def update_dataset_version_with_stats(
+        self, dataset: DatasetRecord, version: int, **kwargs
+    ) -> None:
+        dataset_version = dataset.get_version(version)
+
+        num_objects = dataset_version.num_objects
+        size = dataset_version.size
+        if not num_objects:
+            num_objects, size = self.warehouse.dataset_stats(dataset, version)
+
+        self.metastore.update_dataset_version(
+            dataset_version,
+            num_objects=num_objects,
+            size=size,
+            **kwargs,
+        )
+
     def update_dataset(
         self, dataset: DatasetRecord, conn=None, **kwargs
     ) -> DatasetRecord:
         """Updates dataset fields."""
         old_name = None
         new_name = None
         if "name" in kwargs and kwargs["name"] != dataset.name:
@@ -1120,14 +1135,17 @@
         """
         if not dataset.has_version(version):
             return
         dataset = self.metastore.remove_dataset_version(dataset, version)
         if drop_rows:
             self.warehouse.drop_dataset_rows_table(dataset, version)
 
+    def get_temp_table_names(self) -> list[str]:
+        return self.warehouse.get_temp_table_names()
+
     def cleanup_temp_tables(self, names: Iterable[str]) -> None:
         """
         Drop tables created temporarily when processing datasets.
 
         This should be implemented even if temporary tables are used to
         ensure that they are cleaned up as soon as they are no longer
         needed. When running the same `DatasetQuery` multiple times we
@@ -1175,24 +1193,27 @@
             self.metastore.update_dataset_status(
                 ds,
                 DatasetStatus.FAILED,
                 version=ds.latest_version,
                 error_message=DATASET_INTERNAL_ERROR_MESSAGE,
                 error_stack=traceback.format_exc(),
             )
-            self.metastore.update_dataset_version(
-                ds.get_version(ds.latest_version),  # type: ignore[arg-type]
+            self.warehouse.drop_dataset_rows_table(ds, ds.latest_version)
+            self.update_dataset_version_with_stats(
+                ds,
+                ds.latest_version,
                 sources="\n".join(sources),
             )
             raise
 
         ds = self.get_dataset(name)
 
-        self.metastore.update_dataset_version(
-            ds.get_version(ds.latest_version),  # type: ignore[arg-type]
+        self.update_dataset_version_with_stats(
+            ds,
+            ds.latest_version,
             sources="\n".join(sources),
         )
 
         return self.get_dataset(name)
 
     def register_dataset(
         self,
@@ -1229,14 +1250,16 @@
             query_script=dataset_version.query_script,
             error_message=dataset_version.error_message,
             error_stack=dataset_version.error_stack,
             script_output=dataset_version.script_output,
             created_at=dataset_version.created_at,
             finished_at=dataset_version.finished_at,
             custom_column_types=dataset_version.custom_column_types_serialized,
+            num_objects=dataset_version.num_objects,
+            size=dataset_version.size,
         )
         # to avoid re-creating rows table, we are just renaming it for a new version
         # of target dataset
         self.warehouse.rename_dataset_table(
             dataset.name,
             target_dataset.name,
             old_version=version,
@@ -1340,18 +1363,18 @@
         return self.warehouse.dataset_table_export_file_names(dataset, version)
 
     def dataset_stats(self, name: str, version: int) -> DatasetStats:
         """
         Returns tuple with dataset stats: total number of rows and total dataset size.
         """
         dataset = self.get_dataset(name)
-        num_objects, size = self.warehouse.dataset_stats(dataset, version)
+        dataset_version = dataset.get_version(version)
         return DatasetStats(
-            num_objects=num_objects,
-            size=size,
+            num_objects=dataset_version.num_objects,
+            size=dataset_version.size,
         )
 
     def remove_dataset(
         self,
         name: str,
         version: Optional[int] = None,
         force: Optional[bool] = False,
@@ -1430,16 +1453,17 @@
                 dst_version=dst_version,  # type: ignore[arg-type]
             )
             merged_custom_column_types = {
                 **src.custom_column_types_serialized,
                 **dst.custom_column_types_serialized,
             }
             self.update_dataset(dst, custom_column_types=merged_custom_column_types)
-            self.metastore.update_dataset_version(
-                dst.get_version(dst_version),  # type: ignore[arg-type]
+            self.update_dataset_version_with_stats(
+                dst,
+                dst_version,  # type: ignore[arg-type]
                 custom_column_types=merged_custom_column_types,
             )
             for dep in src_dep:
                 if dep and dep not in dst_dep:
                     self.metastore.add_dependency(
                         dep,
                         dst.name,
@@ -1467,14 +1491,15 @@
             )
             self.warehouse.merge_dataset_rows(
                 src,
                 dst,
                 src_version,
                 dst_version,
             )
+            self.update_dataset_version_with_stats(dst, dst_version)
             for dep in set(src_dep + dst_dep):
                 if dep:
                     self.metastore.add_dependency(dep, dst.name, dst_version)
 
         return dst
 
     def open_object(self, row: DatasetRow, use_cache: bool = True, **config: Any):
@@ -1658,14 +1683,15 @@
             dataset,
             DatasetStatus.COMPLETE,
             version=version,
             error_message=remote_dataset.error_message,
             error_stack=remote_dataset.error_stack,
             script_output=remote_dataset.error_stack,
         )
+        self.update_dataset_version_with_stats(dataset, version)
 
         dataset_save_progress_bar.close()
         print(f"Dataset {dataset_uri} saved locally")
 
         _instantiate_dataset()
 
     def clone(
@@ -1745,14 +1771,15 @@
         python_executable: Optional[str] = None,
         save: bool = False,
         preview_limit: Optional[int] = 10,
         preview_offset: int = 0,
         preview_columns: Optional[list[str]] = None,
         capture_output: bool = True,
         output_hook: Callable[[str], None] = noop,
+        params: Optional[dict[str, str]] = None,
     ) -> QueryResult:
         """
         Method to run custom user Python script to run a query and, as result,
         creates new dataset from the results of a query.
         Returns tuple of result dataset and script output.
 
         Constraints on query script:
@@ -1768,16 +1795,18 @@
 
         Example of query script:
             from dvcx.query import DatasetQuery, C
             DatasetQuery('s3://ldb-public/remote/datasets/mnist-tiny/').filter(
                 C.size > 1000
             )
         """
+        from dvcx.query.dataset import ExecutionResult
+
         try:
-            query_script_compiled = self.compile_query_script(query_script, save=save)
+            query_script_compiled = self.compile_query_script(query_script)
         except Exception as exc:
             raise QueryScriptCompileError(
                 f"Query script failed to compile, reason: {exc}"
             ) from exc
 
         r, w = os.pipe()
         if os.name == "nt":
@@ -1792,21 +1821,23 @@
         else:
             handle = w
             kwargs = {"pass_fds": [w]}
 
         envs = dict(envs or os.environ)
         envs.update(
             {
+                "DVCX_QUERY_PARAMS": json.dumps(params or {}),
                 "DVCX_QUERY_PREVIEW_ARGS": json.dumps(
                     {
                         "limit": preview_limit,
                         "offset": preview_offset,
                         "columns": preview_columns,
                     }
                 ),
+                "DVCX_QUERY_SAVE": "1" if save else "",
                 "PYTHONUNBUFFERED": "1",
                 "DVCX_OUTPUT_FD": str(handle),
             },
         )
 
         python_executable = python_executable or sys.executable
         with subprocess.Popen(
@@ -1831,70 +1862,67 @@
                     time.sleep(0.1)
                 response_text += f.readline()
 
         try:
             response = json.loads(response_text)
         except ValueError:
             response = {}
-        records = response.get("preview", None)
-        dataset_name, dataset_version = response.get("dataset", (None, None))
+        exec_result = ExecutionResult(**response)
 
-        script_output = "".join(lines)
+        output = "".join(lines)
 
         if proc.returncode:
             if proc.returncode == QUERY_SCRIPT_CANCELED_EXIT_CODE:
                 raise QueryScriptCancelError(
                     "Query script was canceled by user",
                     return_code=proc.returncode,
-                    output=script_output,
+                    output=output,
                 )
             if proc.returncode == QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE:
                 raise QueryScriptRunError(
                     "Last line in a script was not an instance of DatasetQuery",
                     return_code=proc.returncode,
-                    output=script_output,
+                    output=output,
                 )
             raise QueryScriptRunError(
                 f"Query script exited with error code {proc.returncode}",
                 return_code=proc.returncode,
-                output=script_output,
+                output=output,
             )
 
-        if not save:
-            return QueryResult(
-                dataset=None, version=None, output=script_output, preview=records
-            )
-
-        # finding returning dataset
-        returned_dataset = None
-        returned_dataset_version = None
-        if dataset_name and dataset_version:
+        dataset: Optional["DatasetRecord"] = None
+        version: Optional[int] = None
+        if save:
+            if not exec_result.dataset:
+                raise QueryScriptDatasetNotFound(
+                    "No dataset found after running Query script",
+                    output=output,
+                )
+            name, version = exec_result.dataset
+            # finding returning dataset
             try:
-                returned_dataset = self.get_dataset(dataset_name)
-                returned_dataset_version = returned_dataset.get_version(dataset_version)
-            except DatasetNotFoundError:
-                pass
-
-        if not returned_dataset or not returned_dataset_version:
-            raise QueryScriptDatasetNotFound(
-                "No dataset found after running Query script",
-                output=script_output,
-            )
+                dataset = self.get_dataset(name)
+                dataset.get_version(version)
+            except (DatasetNotFoundError, ValueError) as e:
+                raise QueryScriptDatasetNotFound(
+                    "No dataset found after running Query script",
+                    output=output,
+                ) from e
 
-        returned_dataset = self.update_dataset(
-            returned_dataset,
-            script_output=script_output,
-            query_script=query_script,
-        )
+            dataset = self.update_dataset(
+                dataset,
+                script_output=output,
+                query_script=query_script,
+            )
 
         return QueryResult(
-            dataset=returned_dataset,
-            version=dataset_version,
-            output=script_output,
-            preview=records,
+            dataset=dataset,
+            version=version,
+            output=output,
+            preview=exec_result.preview,
         )
 
     def cp(
         self,
         sources: list[str],
         output: str,
         force: bool = False,
```

### Comparing `dvcx-0.76.0/src/dvcx/catalog/datasource.py` & `dvcx-0.77.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/catalog/formats.py` & `dvcx-0.77.0/src/dvcx/catalog/formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/catalog/loader.py` & `dvcx-0.77.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/cli.py` & `dvcx-0.77.0/src/dvcx/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from itertools import chain
 from multiprocessing import freeze_support
 from typing import TYPE_CHECKING, Optional, Union
 
 import shtab
 
 from dvcx import __version__, utils
-from dvcx.cli_utils import BooleanOptionalAction, CommaSeparatedArgs
+from dvcx.cli_utils import BooleanOptionalAction, CommaSeparatedArgs, KeyValueArgs
 from dvcx.utils import DVCXDir
 
 if TYPE_CHECKING:
     from dvcx.catalog import Catalog
 
 logger = logging.getLogger("dvcx")
 
@@ -497,14 +497,22 @@
     )
     query_parser.add_argument(
         "--no-collapse",
         action="store_true",
         default=False,
         help="Do not collapse the columns",
     )
+    query_parser.add_argument(
+        "-p",
+        "--param",
+        metavar="param=value",
+        nargs=1,
+        action=KeyValueArgs,
+        help="Query parameters",
+    )
 
     apply_udf_parser = subp.add_parser(
         "apply-udf", parents=[parent_parser], help="Apply UDF"
     )
     apply_udf_parser.add_argument("udf", type=str, help="UDF location")
     apply_udf_parser.add_argument("source", type=str, help="Source storage or dataset")
     apply_udf_parser.add_argument("target", type=str, help="Target dataset name")
@@ -522,14 +530,17 @@
     )
     apply_udf_parser.add_argument(
         "--udf-params", type=str, default=None, help="UDF class parameters"
     )
     subp.add_parser(
         "clear-cache", parents=[parent_parser], help="Clear the local file cache"
     )
+    subp.add_parser(
+        "gc", parents=[parent_parser], help="Garbage collect temporary tables"
+    )
 
     add_completion_parser(subp, [parent_parser])
     return parser
 
 
 def add_completion_parser(subparsers, parents):
     parser = subparsers.add_parser(
@@ -796,14 +807,15 @@
     script: str,
     dataset_name: str,
     parallel: Optional[int] = None,
     limit: int = 10,
     offset: int = 0,
     columns: Optional[list[str]] = None,
     no_collapse: bool = False,
+    params: Optional[dict[str, str]] = None,
 ) -> None:
     from dvcx.utils import show_records
 
     with open(script, encoding="utf-8") as f:
         script_content = f.read()
 
     if parallel is not None:
@@ -812,22 +824,32 @@
 
     result = catalog.query(
         script_content,
         preview_limit=limit,
         preview_offset=offset,
         preview_columns=columns,
         capture_output=False,
+        params=params,
     )
     show_records(result.preview, collapse_columns=not no_collapse)
 
 
 def clear_cache(catalog: "Catalog"):
     catalog.cache.clear()
 
 
+def garbage_collect(catalog: "Catalog"):
+    temp_tables = catalog.get_temp_table_names()
+    if not temp_tables:
+        print("Nothing to clean up.")
+    else:
+        print(f"Garbage collecting {len(temp_tables)} tables.")
+        catalog.cleanup_temp_tables(temp_tables)
+
+
 def completion(shell: str) -> str:
     return shtab.complete(
         get_parser(),
         shell=shell,
     )
 
 
@@ -989,21 +1011,24 @@
                 catalog,
                 args.script,
                 args.parallel,
                 limit=args.limit,
                 offset=args.offset,
                 columns=args.columns,
                 no_collapse=args.no_collapse,
+                params=args.param,
             )
         elif args.command == "apply-udf":
             catalog.apply_udf(
                 args.udf, args.source, args.target, args.parallel, args.udf_params
             )
         elif args.command == "clear-cache":
             clear_cache(catalog)
+        elif args.command == "gc":
+            garbage_collect(catalog)
         else:
             print(f"invalid command: {args.command}", file=sys.stderr)
             return 1
         return 0
     except BrokenPipeError:
         # Python flushes standard streams on exit; redirect remaining output
         # to devnull to avoid another BrokenPipeError at shutdown
```

### Comparing `dvcx-0.76.0/src/dvcx/cli_utils.py` & `dvcx-0.77.0/src/dvcx/cli_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from argparse import SUPPRESS, Action, _AppendAction
+from argparse import SUPPRESS, Action, ArgumentError, _AppendAction
 
 
 class BooleanOptionalAction(Action):
     """
     Creates --[no-]option style bool options.
 
     Defined here since it doesn't exist in argparse in Python 3.8.
@@ -54,7 +54,19 @@
 
 
 class CommaSeparatedArgs(_AppendAction):  # pylint: disable=protected-access
     def __call__(self, parser, namespace, values, option_string=None):  # noqa: ARG002
         items = getattr(namespace, self.dest) or []
         items.extend(v for value in values.split(",") if (v := value.strip()))
         setattr(namespace, self.dest, list(dict.fromkeys(items)))
+
+
+class KeyValueArgs(_AppendAction):  # pylint: disable=protected-access
+    def __call__(self, parser, namespace, values, option_string=None):  # noqa: ARG002
+        items = getattr(namespace, self.dest) or {}
+        for raw_value in filter(bool, values):
+            key, sep, value = raw_value.partition("=")
+            if not key or not sep or value == "":
+                raise ArgumentError(self, f"expected 'key=value', got {raw_value!r}")
+            items[key.strip()] = value
+
+        setattr(namespace, self.dest, items)
```

### Comparing `dvcx-0.76.0/src/dvcx/client/azure.py` & `dvcx-0.77.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/client/fileslice.py` & `dvcx-0.77.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/client/fsspec.py` & `dvcx-0.77.0/src/dvcx/client/fsspec.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,21 +251,14 @@
         nodes,
         shared_progress_bar=None,
     ) -> None:
         fetcher = NodesFetcher(self, self.MAX_THREADS, self.cache)
         chunk_gen = NodeChunk(self.cache, self.uri, nodes)
         fetcher.run(chunk_gen, shared_progress_bar)
 
-    def iter_object_chunks(self, bucket, path, version=None):
-        with self.fs.open(f"{bucket}/{path}", version_id=version) as f:
-            chunk = f.read()
-            while chunk:
-                yield chunk
-                chunk = f.read()
-
     def instantiate_object(
         self,
         uid: UniqueId,
         dst: str,
         progress_bar: tqdm,
         force: bool = False,
     ) -> None:
@@ -293,15 +286,17 @@
             return self._open_tar(uid, use_cache=True)
         if use_cache and (cache_path := self.cache.get_path(uid)):
             return open(cache_path, mode="rb")
         return self.fs.open(self.get_full_path(uid.path))
 
     def _open_tar(self, uid: UniqueId, use_cache: bool = True):
         assert uid.location is not None
-        loc_stack = json.loads(uid.location)
+        loc_stack = (
+            json.loads(uid.location) if isinstance(uid.location, str) else uid.location
+        )
         if len(loc_stack) > 1:
             raise NotImplementedError("Nested v-objects are not supported yet.")
         obj_location = loc_stack[0]
         tar_path = posixpath.split(obj_location["parent"])
         parent_etag = obj_location["etag"]
         offset = obj_location["offset"]
         size = obj_location["size"]
@@ -312,17 +307,14 @@
             size=-1,
             vtype="",
             location=None,
         )
         f = self.open_object(parent_uid, use_cache=use_cache)
         return FileSlice(f, offset, size, posixpath.basename(uid.path))
 
-    def open(self, path: str, mode="rb") -> Any:
-        return self.fs.open(self.get_full_path(path), mode=mode)
-
     def download(self, uid: UniqueId, *, callback=None) -> None:
         sync(get_loop(), functools.partial(self._download, uid, callback=callback))
 
     async def _download(self, uid: UniqueId, *, callback=None) -> None:
         if self.cache.contains(uid):
             # Already in cache, so there's nothing to do.
             return
@@ -335,19 +327,20 @@
         if uid.vtype == "tar":
             loop = asyncio.get_running_loop()
             await loop.run_in_executor(
                 None, functools.partial(self._download_from_tar, uid, callback=callback)
             )
             # self._download_from_tar(uid, callback=callback)
             return
-        etag = await self.get_current_etag(uid)
-        if uid.etag != etag:
-            raise FileNotFoundError(
-                f"Invalid etag for {uid.storage}/{uid.path}: "
-                f"expected {uid.etag}, got {etag}"
-            )
+        if uid.etag:
+            etag = await self.get_current_etag(uid)
+            if uid.etag != etag:
+                raise FileNotFoundError(
+                    f"Invalid etag for {uid.storage}/{uid.path}: "
+                    f"expected {uid.etag}, got {etag}"
+                )
         await self.cache.download(uid, self, callback=callback)
 
     def _download_from_tar(self, uid, *, callback=None):
         with self._open_tar(uid, use_cache=False) as f:
             contents = f.read()
         self.cache.store_data(uid, contents, callback=callback)
```

### Comparing `dvcx-0.76.0/src/dvcx/client/gcs.py` & `dvcx-0.77.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/client/local.py` & `dvcx-0.77.0/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/client/s3.py` & `dvcx-0.77.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/config.py` & `dvcx-0.77.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.77.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.77.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.77.0/src/dvcx/data_storage/metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from datetime import datetime, timezone
 from functools import cached_property, reduce
 from itertools import groupby
 from typing import TYPE_CHECKING, Any, Optional
 
 from sqlalchemy import (
     JSON,
+    BigInteger,
     Boolean,
     Column,
     DateTime,
     ForeignKey,
     Integer,
     Table,
     Text,
@@ -211,14 +212,16 @@
         error_message: str = "",
         error_stack: str = "",
         script_output: str = "",
         created_at: Optional[datetime] = None,
         finished_at: Optional[datetime] = None,
         custom_column_types: Optional[dict[str, Any]] = None,
         ignore_if_exists: bool = False,
+        num_objects: Optional[int] = None,
+        size: Optional[int] = None,
     ) -> DatasetRecord:
         """Creates new dataset version."""
 
     @abstractmethod
     def remove_dataset(self, dataset: DatasetRecord) -> None:
         """Removes dataset."""
 
@@ -438,14 +441,16 @@
             # adding default for now until we fully remove shadow datasets
             Column("status", Integer, nullable=False, default=DatasetStatus.COMPLETE),
             Column("created_at", DateTime(timezone=True)),
             Column("finished_at", DateTime(timezone=True)),
             Column("error_message", Text, nullable=False, default=""),
             Column("error_stack", Text, nullable=False, default=""),
             Column("script_output", Text, nullable=False, default=""),
+            Column("num_objects", BigInteger, nullable=True),
+            Column("size", BigInteger, nullable=True),
             Column("job_id", Text, nullable=True),
             Column("sources", Text, nullable=False, default=""),
             Column("query_script", Text, nullable=False, default=""),
             Column("custom_column_types", JSON, nullable=True),
             UniqueConstraint("dataset_id", "version"),
         ]
 
@@ -948,14 +953,16 @@
         error_message: str = "",
         error_stack: str = "",
         script_output: str = "",
         created_at: Optional[datetime] = None,
         finished_at: Optional[datetime] = None,
         custom_column_types: Optional[dict[str, Any]] = None,
         ignore_if_exists: bool = False,
+        num_objects: Optional[int] = None,
+        size: Optional[int] = None,
         conn=None,
     ) -> DatasetRecord:
         """Creates new dataset version."""
         if status in [DatasetStatus.COMPLETE, DatasetStatus.FAILED]:
             finished_at = finished_at or datetime.now(timezone.utc)
         else:
             finished_at = None
@@ -968,14 +975,16 @@
             finished_at=finished_at,
             error_message=error_message,
             error_stack=error_stack,
             script_output=script_output,
             sources=sources,
             query_script=query_script,
             custom_column_types=json.dumps(custom_column_types or {}),
+            num_objects=num_objects,
+            size=size,
         )
         if ignore_if_exists:
             query = query.on_conflict_do_nothing(
                 index_elements=["dataset_id", "version"]
             )
         self.db.execute(query, conn=conn)
```

### Comparing `dvcx-0.76.0/src/dvcx/data_storage/schema.py` & `dvcx-0.77.0/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/data_storage/serializer.py` & `dvcx-0.77.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.77.0/src/dvcx/data_storage/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -795,15 +795,15 @@
         This will result in the original index table being replaced
         with a table that is a join between the signals table and the
         index table (joining on the id column).
         """
 
         with self.db.transaction():
             # Create temporary table.
-            join_tbl_name = "tmp_" + index.name
+            join_tbl_name = self.TMP_TABLE_NAME_PREFIX + index.name
 
             signal_columns = [c for c in signals.table.c if c.name != "id"]
 
             join_tbl = self.schema.node_cls.new_table(
                 join_tbl_name,
                 [self.schema.node_cls.copy_signal_column(c) for c in signal_columns],
                 self.db.metadata,
```

### Comparing `dvcx-0.76.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.77.0/src/dvcx/data_storage/warehouse.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     #
     # Constants, Initialization, and Tables
     #
 
     BUCKET_TABLE_NAME_PREFIX = "src_"
     DATASET_TABLE_PREFIX = "ds_"
     SIGNALS_TABLE_PREFIX = "sg_"
+    UDF_TABLE_NAME_PREFIX = "udf_"
+    TMP_TABLE_NAME_PREFIX = "tmp_"
 
     id_generator: "AbstractIDGenerator"
     schema: "schema.Schema"
     db: "DatabaseEngine"
 
     def __init__(
         self,
@@ -199,42 +201,59 @@
         """
         This is equivalent to `db.execute`, but for selecting rows in batches
         """
         cols = query.selected_columns
         cols_names = [c.name for c in cols]
 
         if not order_by:
-            ordering = [cols.source, cols.parent, cols.name, cols.version, cols.etag]
+            ordering = [
+                cols.source,
+                cols.parent,
+                cols.name,
+                cols.version,
+                cols.etag,
+            ]
         else:
             ordering = order_by  # type: ignore
 
         # reset query order by and apply new order by id
         paginated_query = query.order_by(None).order_by(*ordering).limit(page_size)
 
+        results = None
         offset = 0
         num_yielded = 0
-        while True:
-            if limit is not None:
-                limit -= num_yielded
-                if limit == 0:
-                    break
-                if limit < page_size:
-                    paginated_query = paginated_query.limit(None).limit(limit)
-
-            results = self.db.execute(paginated_query.offset(offset))
-
-            processed = False
-            for row in results:
-                processed = True
-                yield DatasetRow.from_result_row(cols_names, row)
-                num_yielded += 1
-
-            if not processed:
-                break  # no more results
-            offset += page_size
+        try:
+            while True:
+                if limit is not None:
+                    limit -= num_yielded
+                    if limit == 0:
+                        break
+                    if limit < page_size:
+                        paginated_query = paginated_query.limit(None).limit(limit)
+
+                results = self.db.execute(paginated_query.offset(offset))
+
+                processed = False
+                for row in results:
+                    processed = True
+                    yield DatasetRow.from_result_row(cols_names, row)
+                    num_yielded += 1
+
+                if not processed:
+                    break  # no more results
+                offset += page_size
+        finally:
+            # https://www2.sqlite.org/cvstrac/wiki?p=DatabaseIsLocked (SELECT not
+            # finalized or reset) to prevent database table is locked error when an
+            # exception is raised in the middle of processing the results (e.g.
+            # https://github.com/iterative/dvcx/issues/924). Connections close
+            # apparently is not enough in some cases, at least on sqlite
+            # https://www.sqlite.org/c3ref/close.html
+            if results and hasattr(results, "close"):
+                results.close()
 
     #
     # Table Name Internal Functions
     #
 
     @staticmethod
     def uri_to_storage_info(uri: str) -> tuple[str, str]:
@@ -416,22 +435,26 @@
     def dataset_rows_count(self, dataset: DatasetRecord, version=None) -> int:
         """Returns total number of rows in a dataset"""
         dr = self.dataset_rows(dataset, version)
         query = select(sa.func.count()).select_from(dr.get_table())
         (res,) = self.db.execute(query)
         return res[0]
 
-    def dataset_stats(self, dataset: DatasetRecord, version: int) -> tuple[int, int]:
+    def dataset_stats(
+        self, dataset: DatasetRecord, version: int
+    ) -> tuple[Optional[int], Optional[int]]:
         """
         Returns tuple with dataset stats: total number of rows and total dataset size.
         """
+        if not (self.db.has_table(self.dataset_table_name(dataset.name, version))):
+            return None, None
+
         dr = self.dataset_rows(dataset, version)
-        query = select(sa.func.count(), sa.func.sum(dr.c.size)).select_from(
-            dr.get_table()
-        )
+        table = dr.get_table()
+        query = select(sa.func.count(), sa.func.sum(dr.c.size)).select_from(table)
         (res,) = self.db.execute(query)
         return res[0], res[1]
 
     #
     # Nodes
     #
 
@@ -885,14 +908,30 @@
             sa.MetaData(),
             sa.Column("id", Int, primary_key=True),
             *custom_columns,
         )
         self.db.create_table(tbl, if_not_exists=True)
         return tbl
 
+    def is_temp_table_name(self, name: str) -> bool:
+        """Returns if the given table name refers to a temporary
+        or no longer needed table."""
+        if name.startswith(
+            (self.TMP_TABLE_NAME_PREFIX, self.UDF_TABLE_NAME_PREFIX, "ds_shadow_")
+        ) or name.endswith("_shadow"):
+            return True
+        return False
+
+    def get_temp_table_names(self) -> list[str]:
+        return [
+            t
+            for t in sa.inspect(self.db.engine).get_table_names()
+            if self.is_temp_table_name(t)
+        ]
+
     def cleanup_temp_tables(self, names: Iterable[str]) -> None:
         """
         Drop tables created temporarily when processing datasets.
 
         This should be implemented even if temporary tables are used to
         ensure that they are cleaned up as soon as they are no longer
         needed. When running the same `DatasetQuery` multiple times we
```

### Comparing `dvcx-0.76.0/src/dvcx/dataset.py` & `dvcx-0.77.0/src/dvcx/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,16 +139,16 @@
 
     def __hash__(self):
         return hash(f"{self.type}_{self.name}_{self.version}")
 
 
 @dataclass
 class DatasetStats:
-    num_objects: int
-    size: int  # in bytes
+    num_objects: Optional[int]  # None if table is missing
+    size: Optional[int]  # in bytes None if table is missing or empty
 
 
 class Status:
     CREATED = 1
     PENDING = 2
     FAILED = 3
     COMPLETE = 4
@@ -163,14 +163,16 @@
     status: int
     created_at: datetime
     finished_at: Optional[datetime]
     error_message: str
     error_stack: str
     script_output: str
     custom_column_types: dict[str, Union[SQLType, type[SQLType]]]
+    num_objects: Optional[int]
+    size: Optional[int]
     job_id: Optional[str] = None
     sources: str = ""
     query_script: str = ""
 
     @classmethod
     def parse(
         cls: type[V],
@@ -179,14 +181,16 @@
         version: int,
         status: int,
         created_at: datetime,
         finished_at: Optional[datetime],
         error_message: str,
         error_stack: str,
         script_output: str,
+        num_objects: Optional[int],
+        size: Optional[int],
         job_id: Optional[str],
         custom_column_types: dict[str, Union[SQLType, type[SQLType]]],
         sources: str = "",
         query_script: str = "",
     ):
         return cls(
             id,
@@ -195,14 +199,16 @@
             status,
             created_at,
             finished_at,
             error_message,
             error_stack,
             script_output,
             custom_column_types,
+            num_objects,
+            size,
             job_id,
             sources,
             query_script,
         )
 
     def __eq__(self, other):
         if not isinstance(other, DatasetVersion):
@@ -294,14 +300,16 @@
         version: int,
         version_status: int,
         version_created_at: datetime,
         version_finished_at: Optional[datetime],
         version_error_message: str,
         version_error_stack: str,
         version_script_output: str,
+        version_num_objects: Optional[int],
+        version_size: Optional[int],
         version_job_id: Optional[str],
         version_sources: Optional[str],
         version_query_script: Optional[str],
         version_custom_column_types: str,
     ) -> "DatasetRecord":
         labels_lst: list[str] = json.loads(labels) if labels else []
         custom_column_types_dct: dict[str, Any] = (
@@ -319,14 +327,16 @@
             version,
             version_status,
             version_created_at,
             version_finished_at,
             version_error_message,
             version_error_stack,
             version_script_output,
+            version_num_objects,
+            version_size,
             version_job_id,
             cls.parse_custom_column_types(version_custom_column_types_dct),  # type: ignore[arg-type]
             version_sources,  # type: ignore[arg-type]
             version_query_script,  # type: ignore[arg-type]
         )
 
         return cls(
```

### Comparing `dvcx-0.76.0/src/dvcx/error.py` & `dvcx-0.77.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/cached_stream.py` & `dvcx-0.77.0/src/dvcx/lib/cached_stream.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 class AbstractCachedStream(AbstractContextManager, ABC):
     def __init__(self, stream, size, catalog, uid: UniqueId):
         self.stream = stream
         self.size = size
         self.catalog = catalog
         self.uid = uid
+        self.mode = "rb"
+
+    def set_mode(self, mode):
+        self.mode = mode
 
 
 class ProgressiveCacheStream(AbstractCachedStream):
     BUF_SIZE = 4096
 
     def __init__(self, stream, size, catalog, uid: UniqueId):
         super().__init__(stream, size, catalog, uid)
@@ -25,15 +29,15 @@
         self.cached_file = None
 
         self.temp_file = None
         self.temp_file_pos = 0
 
     def __enter__(self):
         if os.path.exists(self.target_path):
-            self.cached_file = open(self.target_path, mode="rb")
+            self.cached_file = open(self.target_path, mode=self.mode)
             return self.cached_file
 
         tmp_dir = self.catalog.cache.tmp_dir
         if not os.path.exists(tmp_dir):
             os.makedirs(tmp_dir)
         self.temp_file = tempfile.NamedTemporaryFile(
             prefix=str(self.uid.get_hash()), dir=tmp_dir, delete=False
@@ -99,18 +103,18 @@
         self.cached_file = None
 
     def get_path_in_cache(self):
         return self.catalog.cache.path_from_checksum(self.uid.get_hash())
 
     def __enter__(self):
         self.client.download(self.uid)
-        self.cached_file = open(self.get_path_in_cache(), "rb")
+        self.cached_file = open(self.get_path_in_cache(), self.mode)
         return self.cached_file
 
     def __exit__(self, *args):
         self.cached_file.close()
 
 
 class PreDownloadStream(PreCachedStream):
     def __exit__(self, *args):
         super().__exit__(*args)
-        os.remove(self.get_path_in_cache())
+        self.catalog.cache.remove(self.uid)
```

### Comparing `dvcx-0.76.0/src/dvcx/lib/dataset.py` & `dvcx-0.77.0/src/dvcx/lib/dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import inspect
-from collections.abc import Sequence
+from collections.abc import Iterator, Sequence
 from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import sqlalchemy
 from sqlalchemy.sql.elements import ColumnElement
 
-from dvcx.lib.feature import Feature, FeatureClass
+from dvcx.lib.feature import Feature
+from dvcx.lib.feature_types import FeatureLike, FeatureTypes
+from dvcx.lib.feature_udf import FeatureConverter
 from dvcx.lib.udf import (
     Aggregator,
     BatchMapper,
     Generator,
     GroupMapper,
     Mapper,
     UDFBase,
 )
-from dvcx.query.dataset import DatasetQuery, JoinPredicateType, PartitionByType, detach
+from dvcx.query.dataset import (
+    DatasetQuery,
+    JoinPredicateType,
+    PartitionByType,
+    detach,
+)
 from dvcx.query.schema import Column
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 C = Column
 
@@ -33,14 +40,23 @@
     These columns typically include labels, embeddings, or auto-generated labels,
     providing a comprehensive view of the file's attributes.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+    def save(
+        self, name: Optional[str] = None, version: Optional[int] = None, **kwargs
+    ) -> "Dataset":
+        """Save and return a Dataset instead of a DatasetQuery."""
+        ds = super().save(name=name, version=version, **kwargs)
+        self.name = ds.name
+        self.version = ds.version
+        return self
+
     def apply(self, func, *args, **kwargs):
         return func(self, *args, **kwargs)
 
     def map(
         self,
         udf: Union[Callable, UDFBase],
         params=None,
@@ -87,14 +103,15 @@
 
         udf_obj = self._udf_to_obj(udf, Mapper, "map()", params, output, cache=cache)
         return self.add_signals(
             udf_obj.to_udf_wrapper(),
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
+            cache=cache,
         )
 
     def generate(  # type: ignore[override]
         self,
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
@@ -126,14 +143,15 @@
         )
         return DatasetQuery.generate(
             self,
             udf_obj.to_udf_wrapper(),
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
+            cache=cache,
         )
 
     def aggregate(
         self,
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
@@ -164,14 +182,15 @@
         return DatasetQuery.generate(
             self,
             udf_obj.to_udf_wrapper(),
             partition_by=partition_by,
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
+            cache=cache,
         )
 
     def batch_map(
         self,
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
@@ -194,14 +213,15 @@
             udf, BatchMapper, "batch_map()", params, output, batch, cache=cache
         )
         return self.add_signals(
             udf_obj.to_udf_wrapper(),
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
+            cache=cache,
         )
 
     def group_map(
         self,
         udf: Union[Callable, UDFBase],
         params=None,
         output=None,
@@ -237,14 +257,15 @@
         )
         return self.add_signals(
             udf_obj.to_udf_wrapper(),
             parallel=parallel,
             workers=workers,
             min_task_size=min_task_size,
             partition_by=partition_by,
+            cache=cache,
         )
 
     def _udf_to_obj(
         self,
         udf,
         target_class: type[UDFBase],
         name: str,
@@ -319,46 +340,82 @@
                 f"'partition_by' argument must be PartitionByType or None"
                 f", {partition_by.__class__.__name__} was given"
             )
 
         if msg:
             raise TypeError(f"Dataset {name} error: {msg}")
 
-    def _args_to_columns(self, *args):
-        return [column for arg in args for column in self._feature_to_columns(arg)]
+    def _args_to_columns(self, *features):
+        uniq_columns = {}
+        for fr in features:
+            uniq_columns = uniq_columns | dict(self._feature_to_column_name_types(fr))
+
+        return [C(name, typ) for name, typ in uniq_columns.items()]
 
     @staticmethod
-    def _feature_to_columns(fr: Union[C, FeatureClass, str]):
+    def _feature_to_column_name_types(fr: FeatureLike) -> list[tuple[str, type]]:
         if isinstance(fr, str):
-            return [C(fr)]
+            return [(fr, str)]
 
         if isinstance(fr, C):
-            return [fr]
+            return [(fr.name, type(fr.type))]
 
         if not issubclass(fr, Feature):
             raise TypeError(f"feature or column '{fr}' has a wrong type '{type(fr)}'")
 
-        spec = fr._to_udf_spec()
-        return [C(name) for (name, typ) in spec]
+        return fr._to_udf_spec()
 
     def _extend_features(self, method_name, *args):
         super_func = getattr(super(), method_name)
 
         columns = self._args_to_columns(*args)
-        res = super_func(self, *columns)
+        res = super_func(*columns)
         return res
 
     @detach
     def select(self, *args, **kwargs) -> "Self":
         return self._extend_features("select", *args)
 
     @detach
     def select_except(self, *args) -> "Self":
         return self._extend_features("select_except", *args)
 
+    def get_values(self, *fr_classes: FeatureLike) -> Iterator[Sequence]:
+        for features in self.iterate(*fr_classes):
+            yield [fr._get_value_with_check() for fr in features]
+
+    def iterate(self, *fr_classes: FeatureLike) -> Iterator[Sequence[Feature]]:
+        fr_classes_only = FeatureTypes._to_features(*fr_classes)
+        ds = self.select(*fr_classes_only)
+
+        with ds.as_iterable() as rows_iter:
+            params = FeatureConverter.get_flattened_params(fr_classes_only)
+            for row in rows_iter:
+                yield from FeatureConverter.deserialize(
+                    [row], params, fr_classes_only, self.catalog, True
+                )
+
+    def to_pytorch(self, *fr_classes: FeatureLike, **kwargs):
+        try:
+            import torch  # noqa: F401
+        except ImportError as exc:
+            raise ImportError(
+                "Missing required dependency 'torch' for Dataset.to_pytorch()"
+            ) from exc
+        from dvcx.lib.pytorch import PytorchDataset
+
+        if self.attached:
+            ds = self
+        else:
+            ds = self.save()
+        assert ds.name is not None  # for mypy
+        return PytorchDataset(
+            fr_classes, ds.name, ds.version, catalog=self.catalog, **kwargs
+        )
+
     @detach
     def merge(
         self,
         right_ds: "Dataset",
         on: Union[JoinPredicateType, Sequence[JoinPredicateType]],
         right_on: Union[JoinPredicateType, Sequence[JoinPredicateType], None] = None,
         inner=False,
```

### Comparing `dvcx-0.76.0/src/dvcx/lib/feature.py` & `dvcx-0.77.0/src/dvcx/lib/feature.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 import inspect
 import re
 import warnings
 from collections.abc import Sequence
 from datetime import datetime
 from types import GenericAlias
-from typing import ClassVar, Union, get_args, get_origin
+from typing import Any, ClassVar, Literal, Union, get_args, get_origin
 
 import attrs
 from pydantic import BaseModel
+from typing_extensions import Literal as LiteralEx
 
 from dvcx.query import C
 from dvcx.query.udf import UDFOutputSpec
-from dvcx.sql.types import JSON, Array, Binary, Boolean, DateTime, Float, Int, String
+from dvcx.sql.types import (
+    JSON,
+    Array,
+    Binary,
+    Boolean,
+    DateTime,
+    Float,
+    Int,
+    NullType,
+    String,
+)
 
 TYPE_TO_DVCX = {
     int: Int,
     str: String,
+    Literal: String,
+    LiteralEx: String,
     float: Float,
     bool: Boolean,
     datetime: DateTime,
     bytes: Binary,
-    list: Array,
+    list: Array(NullType),
     dict: JSON,
+    Any: NullType,
+    None: NullType,
 }
 
-FeatureClass = type["Feature"]
-FeatureClassSeq = Sequence[FeatureClass]
 
 # Disable Pydantic warning, see https://github.com/iterative/dvcx/issues/1285
 warnings.filterwarnings(
     "ignore",
     message="Field name .* shadows an attribute in parent",
     category=UserWarning,
 )
@@ -41,14 +54,32 @@
     `pydantic`'s BaseModel, allowing for data validation and definition.
     """
 
     _expand_name: ClassVar[bool] = True
     _delimiter: ClassVar[str] = "__"
     _is_file: ClassVar[bool] = False
 
+    def get_value(self, *args: Any, **kwargs: Any) -> Any:
+        name = self.__class__.__name__
+        raise NotImplementedError(f"value is not defined for feature class {name}")
+
+    def _get_value_with_check(self, *args: Any, **kwargs: Any) -> Any:
+        signature = inspect.signature(self.get_value)
+        for i, (name, prm) in enumerate(signature.parameters.items()):
+            if prm.default == inspect.Parameter.empty:
+                if i < len(args):
+                    continue
+                if name not in kwargs:
+                    raise ValueError(
+                        f"unable to get value for class {self.__class__.__name__}"
+                        f" due to a missing parameter {name} in get_value()"
+                    )
+
+        return self.get_value(*args, **kwargs)
+
     @classmethod
     def __pydantic_init_subclass__(cls):
         for name, field_info in cls.model_fields.items():
             attr_value = _resolve(cls, name, field_info, cls._prefix())
             setattr(cls, name, RestrictedAttribute(attr_value, cls, name))
 
     @classmethod
@@ -76,14 +107,18 @@
     @staticmethod
     def _convert_type(typ):
         res = TYPE_TO_DVCX.get(typ, None)
         if res:
             return res
 
         orig = get_origin(typ)
+
+        if orig in (Literal, LiteralEx):
+            return String
+
         if orig == list:
             args = get_args(typ)
             if args is None or len(args) != 1:
                 raise TypeError(f"Cannot resolve type '{typ}' for flattening features")
             next_type = Feature._convert_type(args[0])
             return Array(next_type)
 
@@ -113,23 +148,40 @@
             yield name, f_info.annotation, f_info.is_required()
 
     @classmethod
     def _flatten_full_schema(cls, fields, name_path):
         for name, anno, is_required in cls._iter_fields(fields):
             name = cls._normalize(name)
 
+            orig = get_origin(anno)
+            if orig == list:
+                anno = get_args(anno)
+                if isinstance(anno, tuple):
+                    anno = anno[0]
+                is_list = True
+            else:
+                is_list = False
+
+            expanded_name = name
+            if cls._expand_name:
+                lst = [cls._prefix()] + name_path + [name]
+                expanded_name = cls._delimiter.join(lst)
+
             if Feature._is_feature_class(anno):
-                yield from cls._flatten_full_schema(
-                    anno.model_fields, name_path + [name]
-                )
+                if is_list:
+                    yield expanded_name, Array(JSON), is_required
+                else:
+                    yield from cls._flatten_full_schema(
+                        anno.model_fields, name_path + [name]
+                    )
             else:
-                if cls._expand_name:
-                    lst = [cls._prefix()] + name_path + [name]
-                    name = cls._delimiter.join(lst)
-                yield name, Feature._convert_type(anno), is_required
+                typ = Feature._convert_type(anno)
+                if is_list:
+                    typ = Array(typ)
+                yield expanded_name, typ, is_required
 
     @classmethod
     def _is_feature_class(cls, anno):
         return (
             inspect.isclass(anno)
             and not isinstance(anno, GenericAlias)
             and issubclass(anno, Feature)
@@ -137,15 +189,15 @@
 
     @classmethod
     def _to_udf_spec(cls):
         full_schema = cls._flatten_full_schema(cls.model_fields, [])
         return [(name, typ) for name, typ, is_required in full_schema]
 
     @staticmethod
-    def _features_to_udf_spec(fr_classes: FeatureClassSeq) -> UDFOutputSpec:
+    def _features_to_udf_spec(fr_classes: Sequence[type["Feature"]]) -> UDFOutputSpec:
         return dict(
             item
             for b in fr_classes
             for item in b._to_udf_spec()  # type: ignore[attr-defined]
         )
 
     def _flatten_fields_values(self, fields, dump):
@@ -241,17 +293,21 @@
     Users just use `MyClass.sub_attr1.sub_attr2.field` and it will return a DB column
     with a proper name (with default naming - `my_class__sub_attr1__sub_attr2__field`).
     """
     anno = field_info.annotation
     norm_name = cls._normalize(name)
 
     if not cls._is_feature_class(anno):
+        try:
+            anno_sql_class = cls._convert_type(anno)
+        except RuntimeError:
+            anno_sql_class = NullType
         if cls._expand_name:
-            return C(cls._delimiter.join([prefix, norm_name]))
-        return C(norm_name)
+            return C(cls._delimiter.join([prefix, norm_name]), anno_sql_class)
+        return C(norm_name, anno_sql_class)
 
     if not cls._expand_name:
         return FeatureAttributeWrapper(anno, "")
 
     new_prefix_value = cls._delimiter.join([prefix, norm_name])
     return FeatureAttributeWrapper(anno, new_prefix_value)
```

### Comparing `dvcx-0.76.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.77.0/src/dvcx/lib/feature_udf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import inspect
+import io
 import sys
 import traceback
 from collections.abc import Sequence
 from typing import Optional, Union
 
-from dvcx.lib.feature import Feature, FeatureClass, FeatureClassSeq
+from dvcx.catalog import Catalog
+from dvcx.lib.feature import Feature
+from dvcx.lib.feature_types import FeatureLike, FeatureTypes
+from dvcx.lib.file import File
 from dvcx.lib.udf import Aggregator, BatchMapper, Generator, Mapper, UDFBase
 from dvcx.lib.utils import DvcxError
 from dvcx.query import Stream
 
 
 class ValidationError(DvcxError):
     pass
@@ -28,85 +32,130 @@
 
 
 class UserCodeError(DvcxError):
     def __init__(self, class_name: str, message: str):
         super().__init__(f"Error in user code in class '{class_name}': {message}")
 
 
-class FeatureConvertor:
+class FeatureConverter:
     @property
     def udf_params_list(self):
         return self._udf_params_list
 
     @property
     def udf_output_spec(self):
         return self._udf_output_spec
 
     @property
-    def has_stream(self):
-        return self._has_stream
-
-    @property
     def cache(self):
         return self._udf.catalog.cache
 
+    @staticmethod
+    def has_feature_stream(fr_classes: Sequence[type[Feature]]):
+        return any(
+            f._is_file  # type: ignore[attr-defined]
+            for f in fr_classes
+        )
+
+    @staticmethod
+    def has_row_stream(row):
+        if len(row) == 0:
+            return False
+        return isinstance(row[0], (Stream, io.IOBase))
+
     def __init__(
         self,
         udf: UDFBase,
-        inputs: Union[FeatureClass, FeatureClassSeq] = (),
-        outputs: Union[FeatureClass, FeatureClassSeq] = (),
+        inputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
+        outputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
     ):
         self._udf = udf
 
         self._inputs, self._is_single_input = self._convert_to_sequence(inputs)
         self._outputs, self._is_single_output = self._convert_to_sequence(outputs)
 
         self._validate_schema("params", self._inputs)
         self._validate_schema("output", self._outputs)
 
-        self._has_stream = any(
-            f._is_file  # type: ignore[attr-defined]
-            for f in self._inputs
-        )
-
-        udf_params_spec = Feature._features_to_udf_spec(self._inputs)
-        stream_prm = [Stream()] if self._has_stream else []
-        self._udf_params_list = stream_prm + list(udf_params_spec.keys())
-
+        self._udf_params_list = self.get_flattened_params(self._inputs)
         self._udf_output_spec = Feature._features_to_udf_spec(self._outputs)  # type: ignore[attr-defined]
 
     @staticmethod
+    def get_flattened_params(fr_classes: Sequence[type[Feature]]):
+        udf_params_spec = Feature._features_to_udf_spec(fr_classes)
+        stream_prm = (
+            [Stream()] if FeatureConverter.has_feature_stream(fr_classes) else []
+        )
+        param_list = stream_prm + list(udf_params_spec.keys())
+        return param_list
+
+    @staticmethod
     def _convert_to_sequence(
-        arg: Union[FeatureClass, FeatureClassSeq],
-    ) -> tuple[FeatureClassSeq, bool]:
+        arg: Union[FeatureLike, Sequence[FeatureLike]],
+    ) -> tuple[Sequence[type[Feature]], bool]:
         if not isinstance(arg, Sequence):
-            return [arg], True
+            return FeatureTypes._to_features(*[arg]), True
         else:
-            return arg, False
+            return FeatureTypes._to_features(*arg), False
+
+    @staticmethod
+    def deserialize(
+        rows: Sequence[Sequence],
+        params: Sequence[str],
+        fr_classes: Sequence[type[Feature]],
+        catalog: Catalog,
+        caching_enabled: bool,
+    ) -> Sequence[Sequence[Feature]]:
+        clean_rows, streams = FeatureConverter._separate_streams_from_rows(
+            rows, fr_classes
+        )
 
-    def deserialize_objs(self, params, args):
+        feature_rows = [
+            FeatureConverter._row_with_params_to_features(row, fr_classes, params)
+            for row in clean_rows
+        ]
+
+        for features, stream in zip(feature_rows, streams):
+            for feature in features:
+                if isinstance(feature, File):
+                    feature.set_catalog(catalog)  # type: ignore [attr-defined]
+                    feature.set_file(stream, caching_enabled)  # type: ignore [attr-defined]
+
+        return feature_rows
+
+    @staticmethod
+    def _separate_streams_from_rows(
+        rows, fr_classes: Sequence[type[Feature]]
+    ) -> tuple[Sequence, Sequence]:
         streams = []
-        if self._has_stream:
-            streams = [arg[0] for arg in args]
-            args = [arg[1:] for arg in args]
-
-        obj_rows = [self._params_to_objects(params, arg) for arg in args]
-        for row, stream in zip(obj_rows, streams):
-            for feature in row:
-                if feature._is_file:
-                    feature.set_catalog(self._udf.catalog)
-                    feature.set_file(stream, self._udf.caching_enabled)
-
-        return obj_rows
-
-    def _params_to_objects(self, params, args):
-        new_params = params if not self._has_stream else params[1:]
-        return [cls._unflatten(dict(zip(new_params, args))) for cls in self._inputs]
+        res_rows = []
+        if FeatureConverter.has_feature_stream(fr_classes):
+            for row in rows:
+                if FeatureConverter.has_row_stream(row):
+                    streams.append(row[0])
+                    res_rows.append(row[1:])
+                else:
+                    streams.append(None)  # type: ignore [arg-type]
+                    res_rows.append(row)
+        else:
+            res_rows = rows
+        return res_rows, streams
+
+    @staticmethod
+    def _row_with_params_to_features(
+        row: Sequence, fr_classes: Sequence[type[Feature]], params: Sequence[str]
+    ) -> Sequence[Feature]:
+        new_params = (
+            params
+            if not FeatureConverter.has_feature_stream(fr_classes)
+            else params[1:]
+        )
+        return [cls._unflatten(dict(zip(new_params, row))) for cls in fr_classes]
 
-    def _validate_schema(self, context: str, features: FeatureClassSeq):
+    def _validate_schema(self, context: str, features: Sequence[type[Feature]]):
         for type_ in features:
             if not isinstance(type_, type):
                 raise SchemaError(
                     self._udf.name,
                     context,
                     "cannot accept objects, a 'Feature' class must be provided",
                 )
@@ -142,15 +191,22 @@
                         self._udf.name,
                         f"expected type '{type_.__name__}',"
                         f" but found type '{type(o).__name__}'",
                         num=num,
                     )
 
     def process_rows(self, rows, is_input_batched=True, is_output_batched=True):
-        obj_rows = self.deserialize_objs(self._udf.params, rows)
+        obj_rows = FeatureConverter.deserialize(
+            rows,
+            self._udf.params,
+            self._inputs,
+            self._udf.catalog,
+            self._udf.caching_enabled,
+        )
+
         if self._is_single_input:
             obj_rows = [objs[0] for objs in obj_rows]
 
         if not is_input_batched:
             assert (
                 len(obj_rows) == 1
             ), f"{self._udf.name} takes {len(obj_rows)} rows while it's not batched"
@@ -192,58 +248,58 @@
             raise UserCodeError(self._udf.name, str(e)) from None
         return result_objs
 
 
 class FeatureAggregator(Aggregator):
     def __init__(
         self,
-        inputs: Union[FeatureClass, FeatureClassSeq] = (),
-        outputs: Union[FeatureClass, FeatureClassSeq] = (),
+        inputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
+        outputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
         batch=1,
     ):
-        self._fc = FeatureConvertor(self, inputs, outputs)
+        self._fc = FeatureConverter(self, inputs, outputs)
         super().__init__(self._fc.udf_params_list, self._fc.udf_output_spec, batch)
 
     def __call__(self, rows):
         return self._fc.process_rows(rows)
 
 
 class FeatureMapper(Mapper):
     def __init__(
         self,
-        inputs: Union[FeatureClass, FeatureClassSeq] = (),
-        outputs: Union[FeatureClass, FeatureClassSeq] = (),
+        inputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
+        outputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
         batch=1,
     ):
-        self._fc = FeatureConvertor(self, inputs, outputs)
+        self._fc = FeatureConverter(self, inputs, outputs)
         super().__init__(self._fc.udf_params_list, self._fc.udf_output_spec, batch)
 
     def __call__(self, *row):
         return self._fc.process_rows([row], False, False)
 
 
 class FeatureBatchMapper(BatchMapper):
     def __init__(
         self,
-        inputs: Union[FeatureClass, FeatureClassSeq] = (),
-        outputs: Union[FeatureClass, FeatureClassSeq] = (),
+        inputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
+        outputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
         batch=1,
     ):
-        self._fc = FeatureConvertor(self, inputs, outputs)
+        self._fc = FeatureConverter(self, inputs, outputs)
         super().__init__(self._fc.udf_params_list, self._fc.udf_output_spec, batch)
 
     def __call__(self, rows):
         return self._fc.process_rows(rows)
 
 
 class FeatureGenerator(Generator):
     def __init__(
         self,
-        inputs: Union[FeatureClass, FeatureClassSeq] = (),
-        outputs: Union[FeatureClass, FeatureClassSeq] = (),
+        inputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
+        outputs: Union[FeatureLike, Sequence[FeatureLike]] = (),
         batch=1,
     ):
-        self._fc = FeatureConvertor(self, inputs, outputs)
+        self._fc = FeatureConverter(self, inputs, outputs)
         super().__init__(self._fc.udf_params_list, self._fc.udf_output_spec, batch)
 
     def __call__(self, *row):
         return self._fc.process_rows([row], False)
```

### Comparing `dvcx-0.76.0/src/dvcx/lib/file.py` & `dvcx-0.77.0/src/dvcx/lib/file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,79 @@
 import json
+from abc import ABC, abstractmethod
 from datetime import datetime
 from pathlib import Path
 from random import getrandbits
 from typing import Optional, Union
 
 from pydantic import Field, field_validator
 
 from dvcx.cache import UniqueId
 from dvcx.lib.cached_stream import PreCachedStream, PreDownloadStream
 from dvcx.lib.feature import ShallowFeature
 from dvcx.lib.utils import DvcxError
+from dvcx.utils import TIME_ZERO
 
 
 class FileFeature(ShallowFeature):
     _is_file = True
 
     def set_file(self, stream, caching_enabled: bool) -> None:
         raise NotImplementedError()
 
     def open(self):
         raise NotImplementedError()
 
+    def read(self):
+        with self.open() as stream:
+            return stream.read()
+
+    def get_value(self):
+        return self.read()
+
+
+class VFileError(DvcxError):
+    def __init__(self, file: "File", message: str, vtype: str = ""):
+        type_ = f" of vtype '{vtype}'" if vtype else ""
+        super().__init__(f"Error in v-file '{file.get_uid().path}'{type_}: {message}")
+
+
+class VFile(ABC):
+    @classmethod
+    @abstractmethod
+    def get_vtype(cls) -> str:
+        pass
+
+    @classmethod
+    @abstractmethod
+    def open(cls, file: "File", location: list[dict]):
+        pass
+
+
+class VFileRegistry:
+    _vtype_readers: dict[str, type["VFile"]] = {}
+
+    @classmethod
+    def register(cls, reader: type["VFile"]):
+        cls._vtype_readers[reader.get_vtype()] = reader
+
+    @classmethod
+    def resolve(cls, file: "File", location: list[dict]):
+        if len(location) == 0:
+            raise VFileError(file, "'location' must not be list of JSONs")
+
+        if not (vtype := location[0].get("vtype", "")):
+            raise VFileError(file, "vtype is not specified")
+
+        reader = cls._vtype_readers.get(vtype, None)
+        if not reader:
+            raise VFileError(file, "reader not registered", vtype)
+
+        return reader.open(file, location)
+
 
 class File(FileFeature):
     source: str = Field(default="")
     parent: str = Field(default="")
     name: str
     version: str = Field(default="")
     etag: str = Field(default="")
@@ -55,29 +104,34 @@
     def validate_location(cls, v):
         return File.to_dict(v)
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._stream = None
         self._catalog = None
+        self._caching_enabled = False
 
     def open(self):
+        if self.location:
+            return VFileRegistry.resolve(self, self.location)
+
         return self._stream
 
     def set_catalog(self, catalog):
         self._catalog = catalog
 
     def set_file(self, stream, caching_enabled: bool) -> None:
         if self._catalog is None:
             raise DvcxError(f"Cannot set file '{stream}' without catalog")
 
         stream_class = PreCachedStream if caching_enabled else PreDownloadStream
         self._stream = stream_class(stream, self.size, self._catalog, self.get_uid())
+        self._caching_enabled = caching_enabled
 
-    def get_uid(self):
+    def get_uid(self) -> UniqueId:
         dump = self.model_dump()
         return UniqueId(*(dump[k] for k in self._unique_id_keys))
 
     def get_local_path(self) -> Optional[str]:
         """Get path to a file in a local cache.
         Return None if file is not cached. Throws an exception if cache is not setup."""
         if self._catalog is None:
@@ -100,26 +154,36 @@
             return self.name
         return f"{self.parent}/{self.name}"
 
     def get_full_path(self):
         return f"{self.source}/{self.get_full_name()}"
 
 
+class TextFile(File):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self._file = None
+
+    def set_file(self, stream, caching_enabled: bool) -> None:
+        super().set_file(stream, caching_enabled)
+        self._stream.set_mode("r")
+
+
 class FileInfo(FileFeature):
     source: str = Field(default="")
     parent: str = Field(default="")
     name: str
     size: int = Field(default=0)
     location: Optional[Union[dict, list[dict]]] = Field(default=None)
     vtype: str = Field(default="")
     dir_type: int = Field(default=0)
     owner_name: str = Field(default="")
     owner_id: str = Field(default="")
     is_latest: bool = Field(default=True)
-    last_modified: datetime = Field(default=datetime.min)
+    last_modified: datetime = Field(default=TIME_ZERO)
     version: str = Field(default="")
     etag: str = Field(default="")
     checksum: str = Field(default="")
     anno: Optional[Union[dict, list[dict]]] = Field(default=None)
     random: int = Field(default_factory=lambda: getrandbits(63))
 
     @field_validator("location", "anno", mode="before")
```

### Comparing `dvcx-0.76.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.77.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.77.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.77.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/image_transform.py` & `dvcx-0.77.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.77.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/param.py` & `dvcx-0.77.0/src/dvcx/lib/param.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/pytorch.py` & `dvcx-0.77.0/src/dvcx/lib/pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 from collections.abc import Iterator, Sequence
 from typing import TYPE_CHECKING, Any, Optional
 
 from torch import float32
 from torch.distributed import get_rank, get_world_size
 from torch.utils.data import IterableDataset, get_worker_info
 
-from dvcx.asyn import ASYNC_WORKERS
 from dvcx.catalog import Catalog, get_catalog
-from dvcx.query import DatasetQuery
+from dvcx.lib.dataset import Dataset
+from dvcx.lib.feature_types import FeatureLike
 
 if TYPE_CHECKING:
     from torchvision.transforms.v2 import Transform
 
-    from dvcx.query.schema import UDFParamSpec
-
 
 logger = logging.getLogger("dvcx")
 
 
 try:
     from torchvision.transforms import v2
 
@@ -27,43 +25,37 @@
     logger.warning("Missing dependency torchvision for computer vision transforms.")
     DEFAULT_TRANSFORM = None
 
 
 class PytorchDataset(IterableDataset):
     def __init__(
         self,
-        params: Sequence["UDFParamSpec"],
+        fr_classes: Sequence[FeatureLike],
         name: str,
         version: Optional[int] = None,
         catalog: Optional["Catalog"] = None,
         transform: Optional["Transform"] = DEFAULT_TRANSFORM,
-        workers: int = ASYNC_WORKERS,
-        cache: bool = False,
         num_samples: int = 0,
     ):
         """
         Pytorch IterableDataset that streams DVCx datasets.
 
         Args:
-            params (UDFParamSpec): Fields from DVCx dataset to stream.
+            fr_classes: Feature-like classes from DVCx dataset to stream.
             name (str): Name of DVCx dataset to stream.
             version (int): Version of DVCx dataset to stream.
             catalog (Catalog): DVCx catalog to which dataset belongs.
             transform (Transform): Torchvision v2 transforms to apply to the dataset.
-            workers (int): Number of async workers per process.
-            cache (bool): Whether to download and cache objects locally.
             num_samples (int): Number of random samples to draw for each epoch.
                 This argument is ignored if `num_samples=0` (the default).
         """
-        self.params = params
+        self.fr_classes = fr_classes
         self.name = name
         self.version = version
         self.transform = transform
-        self.workers = workers
-        self.cache = cache
         self.num_samples = num_samples
         if catalog is None:
             catalog = get_catalog()
         self._init_catalog(catalog)
 
     def _init_catalog(self, catalog: "Catalog"):
         # For compatibility with multiprocessing,
@@ -84,19 +76,19 @@
         wh = wh_cls(*wh_args, **wh_kwargs)
         return Catalog(idgen, ms, wh, **self._catalog_params)
 
     def __iter__(self) -> Iterator[Any]:
         if self.catalog is None:
             self.catalog = self._get_catalog()
         total_rank, total_workers = self.get_rank_and_workers()
-        q = DatasetQuery(name=self.name, version=self.version, catalog=self.catalog)
+        ds = Dataset(name=self.name, version=self.version, catalog=self.catalog)
         if self.num_samples > 0:
-            q = q.sample(self.num_samples)
-        q = q.chunk(total_rank, total_workers)
-        stream = q.extract(*self.params, workers=self.workers, cache=self.cache)
+            ds = ds.sample(self.num_samples)
+        ds = ds.chunk(total_rank, total_workers)
+        stream = ds.get_values(*self.fr_classes)
         for row in stream:
             # Apply transforms
             if self.transform:
                 try:
                     row = self.transform(row)
                 except ValueError:
                     logger.warning("Skipping transform due to unsupported data types.")
```

### Comparing `dvcx-0.76.0/src/dvcx/lib/udf.py` & `dvcx-0.77.0/src/dvcx/lib/udf.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,19 +56,24 @@
     def catalog(self):
         return self._catalog
 
     def to_udf_wrapper(self) -> "UDFWrapper":
         udf_wrapper = udf(params=self.params, output=self.output, batch=self.batch)
         return udf_wrapper(self)
 
-    def setup(self):  # noqa: B027
+    def bootstrap(self):  # noqa: B027
         """Initialization process executed on each worker before processing begins.
         This is needed for tasks like pre-loading ML models prior to scoring.
         """
 
+    def teardown(self):  # noqa: B027
+        """Teardown process executed on each process/worker after processing ends.
+        This is needed for tasks like closing connections to end-points.
+        """
+
     def process(self, *args, **kwargs):
         """Abstract processing method that needs to be re-defined in child classes."""
         NotImplementedError(f"UDF processing is not implemented in class {self.name}")
 
     def validate_results(self, results, *args, **kwargs):
         return results
```

### Comparing `dvcx-0.76.0/src/dvcx/lib/unstructured.py` & `dvcx-0.77.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/utils.py` & `dvcx-0.77.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/webdataset.py` & `dvcx-0.77.0/src/dvcx/lib/webdataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional, Union, get_args, get_origin
 
 from pydantic import Field
 
 from dvcx.lib.feature import Feature
 from dvcx.lib.feature_udf import FeatureGenerator
 from dvcx.lib.file import File, FileInfo
+from dvcx.lib.tar_file import TarVFile
 from dvcx.lib.utils import DvcxError
 
 
 class WDSError(DvcxError):
     def __init__(self, tar_stream, message: str):
         super().__init__(f"WebDataset error '{tar_stream.get_full_name()}': {message}")
 
@@ -166,21 +167,21 @@
 
         f_info = FileInfo(
             name=core_file.name,
             source=self._tar_stream.source,
             parent=new_parent,
             size=core_file.size,
             etag=etag,
-            vtype="tar",
+            vtype="",
             location=[
                 {
-                    "parent": new_parent,
+                    "vtype": TarVFile.get_vtype(),
+                    "parent": self._tar_stream.model_dump(),
                     "size": core_file.size,
-                    "offset": core_file.offset,
-                    "etag": etag,
+                    "offset": core_file.offset_data,
                 }
             ],
         )
 
         self.state = BuilderState()
 
         return f_info, wds
```

### Comparing `dvcx-0.76.0/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.77.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.77.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/listing.py` & `dvcx-0.77.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/node.py` & `dvcx-0.77.0/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.77.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.77.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/progress.py` & `dvcx-0.77.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/query/batch.py` & `dvcx-0.77.0/src/dvcx/query/batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import math
 from abc import ABC, abstractmethod
 from collections.abc import Generator, Sequence
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import sqlalchemy as sa
@@ -63,22 +64,25 @@
     ) -> Generator[DatasetRowsBatch, None, None]:
         # choose page size that is a multiple of the batch size
         page_size = math.ceil(SELECT_BATCH_SIZE / self.count) * self.count
 
         # select rows in batches
         results: list["DatasetRow"] = []
 
-        for row in execute(query, page_size=page_size, limit=query._limit):
-            results.append(row)
-            if len(results) >= self.count:
-                batch, results = results[: self.count], results[self.count :]
-                yield DatasetRowsBatch(batch)
+        with contextlib.closing(
+            execute(query, page_size=page_size, limit=query._limit)
+        ) as rows:
+            for row in rows:
+                results.append(row)
+                if len(results) >= self.count:
+                    batch, results = results[: self.count], results[self.count :]
+                    yield DatasetRowsBatch(batch)
 
-        if len(results) > 0:
-            yield DatasetRowsBatch(results)
+            if len(results) > 0:
+                yield DatasetRowsBatch(results)
 
 
 class Partition(BatchingStrategy):
     """
     Partition implements UDF call batching, where each execution of a UDF
     is run on a list of dataset rows grouped by the specified column.
     Dataset rows need to be sorted by the grouping column.
@@ -88,20 +92,21 @@
         self,
         execute: Callable,
         query: sa.sql.selectable.Select,
     ) -> Generator[DatasetRowsBatch, None, None]:
         current_partition: Optional[int] = None
         batch: list["DatasetRow"] = []
 
-        for row in execute(
-            query, order_by=(PARTITION_COLUMN_ID, "id"), limit=query._limit
-        ):
-            partition = row[PARTITION_COLUMN_ID]
-            if current_partition != partition:
-                current_partition = partition
-                if len(batch) > 0:
-                    yield DatasetRowsBatch(batch)
-                    batch = []
-            batch.append(row)
+        with contextlib.closing(
+            execute(query, order_by=(PARTITION_COLUMN_ID, "id"), limit=query._limit)
+        ) as rows:
+            for row in rows:
+                partition = row[PARTITION_COLUMN_ID]
+                if current_partition != partition:
+                    current_partition = partition
+                    if len(batch) > 0:
+                        yield DatasetRowsBatch(batch)
+                        batch = []
+                batch.append(row)
 
-        if len(batch) > 0:
-            yield DatasetRowsBatch(batch)
+            if len(batch) > 0:
+                yield DatasetRowsBatch(batch)
```

### Comparing `dvcx-0.76.0/src/dvcx/query/builtins.py` & `dvcx-0.77.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/query/dataset.py` & `dvcx-0.77.0/src/dvcx/query/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import random
 import re
 import string
 import subprocess
 import sys
 from abc import ABC, abstractmethod
-from collections.abc import Iterable, Iterator, Sequence
+from collections.abc import Generator, Iterable, Iterator, Sequence
 from copy import copy
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Optional,
@@ -23,14 +23,15 @@
     Union,
 )
 
 import attrs
 import sqlalchemy
 from attrs import frozen
 from dill import dumps
+from fsspec.callbacks import DEFAULT_CALLBACK, Callback, TqdmCallback
 from sqlalchemy.sql import func as f
 from sqlalchemy.sql.elements import ColumnClause, ColumnElement
 from sqlalchemy.sql.expression import label
 from sqlalchemy.sql.schema import TableClause
 from sqlalchemy.sql.selectable import Select
 
 from dvcx.asyn import ASYNC_WORKERS, AsyncMapper, OrderedMapper
@@ -49,28 +50,28 @@
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetNotFoundError, QueryScriptCancelError
 from dvcx.sql.functions import rand
 from dvcx.sql.types import SQLType
 from dvcx.storage import StorageURI
 from dvcx.utils import chunk, determine_processes
 
+from .batch import DatasetRowsBatch
 from .schema import C, UDFParamSpec, normalize_param
 from .session import Session
 from .udf import UDFBase, UDFClassWrapper, UDFFactory, UDFType
 
 if TYPE_CHECKING:
     from sqlalchemy.sql.elements import ClauseElement
     from sqlalchemy.sql.schema import Table
     from sqlalchemy.sql.selectable import GenerativeSelect
     from typing_extensions import Concatenate, ParamSpec, Self
 
     from dvcx.catalog import Catalog
     from dvcx.data_storage import AbstractWarehouse
     from dvcx.dataset import DatasetRecord
-    from dvcx.lib.pytorch import PytorchDataset
 
     from .udf import UDFResult
 
     P = ParamSpec("P")
 
 
 INSERT_BATCH_SIZE = 10000
@@ -128,27 +129,24 @@
             return self.func(*self.columns)
         return self.func(*(c for c in self.columns if c.name in column_names))
 
 
 @frozen
 class StepResult:
     query_generator: QueryGenerator
-    temp_table_names: tuple[str, ...]
     dependencies: tuple[DatasetDependencyType, ...]
 
 
 def step_result(
     func: QueryGeneratorFunc,
     columns: Iterable[ColumnElement],
-    temp_table_names: Iterable[str] = (),
     dependencies: Iterable[DatasetDependencyType] = (),
 ) -> "StepResult":
     return StepResult(
         query_generator=QueryGenerator(func=func, columns=tuple(columns)),
-        temp_table_names=tuple(temp_table_names),
         dependencies=tuple(dependencies),
     )
 
 
 class StartingStep(ABC):
     """An initial query processing step, referencing a data source."""
 
@@ -157,15 +155,17 @@
 
 
 @frozen
 class Step(ABC):
     """A query processing step (filtering, mutation, etc.)"""
 
     @abstractmethod
-    def apply(self, query_generator: "QueryGenerator") -> "StepResult":
+    def apply(
+        self, query_generator: "QueryGenerator", temp_tables: list[str]
+    ) -> "StepResult":
         """Apply the processing step."""
 
 
 @frozen
 class QueryStep(StartingStep):
     catalog: "Catalog"
     dataset_name: str
@@ -247,21 +247,25 @@
         source_query: Select,
         target_query: Select,
     ) -> Select:
         """
         Should return select query that calculates desired diff between dataset queries
         """
 
-    def apply(self, query_generator):
+    def apply(self, query_generator, temp_tables: list[str]):
         source_query = query_generator.exclude(("id", "parent_id"))
         target_query = self.dq.apply_steps().select()
+        temp_tables.extend(self.dq.temp_table_names)
 
         # creating temp table that will hold subtract results
-        temp_table_name = "tmp_" + _random_string(6)
-        custom_columns = [
+        temp_table_name = self.catalog.warehouse.TMP_TABLE_NAME_PREFIX + _random_string(
+            6
+        )
+        temp_tables.append(temp_table_name)
+        custom_columns: list[sqlalchemy.Column] = [
             sqlalchemy.Column(col.name, col.type)
             for col in source_query.columns
             if col.name not in DATASET_CORE_COLUMN_NAMES
         ]
         temp_table = self.catalog.warehouse.create_dataset_rows_table(
             temp_table_name,
             custom_columns=custom_columns,
@@ -275,15 +279,15 @@
         )
 
         self.catalog.warehouse.db.execute(insert_q)
 
         def q(*columns):
             return sqlalchemy.select(*columns).select_from(temp_table)
 
-        return step_result(q, temp_table.c, temp_table_names=[temp_table.name])
+        return step_result(q, temp_table.c)
 
 
 @frozen
 class Subtract(DatasetDiffOperation):
     """
     Calculates rows that are in a source query but are not in target query (diff)
     This can be used to do delta updates (calculate UDF only on newly added rows)
@@ -359,31 +363,53 @@
 
 def process_udf_outputs(
     warehouse: "AbstractWarehouse",
     udf_table: "Table",
     udf_results: Iterator[Iterable["UDFResult"]],
     udf: UDFBase,
     batch_size=INSERT_BATCH_SIZE,
+    cb: Callback = DEFAULT_CALLBACK,
 ) -> None:
     rows: list["UDFResult"] = []
     for udf_output in udf_results:
         if not udf_output:
             continue
         for row in udf_output:
+            cb.relative_update()
             rows.append(adjust_outputs(warehouse, row, udf))
             if len(rows) >= batch_size:
                 for row_chunk in chunk(rows, batch_size):
                     warehouse.insert_rows(udf_table, row_chunk)
                 rows.clear()
 
     if rows:
         for row_chunk in chunk(rows, batch_size):
             warehouse.insert_rows(udf_table, row_chunk)
 
 
+def get_processed_callback() -> Callback:
+    return TqdmCallback({"desc": "Processed", "unit": " rows"})
+
+
+def get_generated_callback(is_generator: bool = False) -> Callback:
+    if is_generator:
+        return TqdmCallback({"desc": "Generated", "unit": " rows"})
+    return DEFAULT_CALLBACK
+
+
+def run_udf(
+    udf, udf_inputs, catalog, is_generator, cache, cb: Callback = DEFAULT_CALLBACK
+) -> Iterator[Iterable["UDFResult"]]:
+    for batch in udf_inputs:
+        n_rows = len(batch.rows) if isinstance(batch, DatasetRowsBatch) else 1
+        output = udf(catalog, batch, is_generator, cache)
+        cb.relative_update(n_rows)
+        yield output
+
+
 @frozen
 class UDF(Step, ABC):
     udf: UDFType
     catalog: "Catalog"
     partition_by: Optional[PartitionByType] = None
     parallel: Optional[int] = None
     workers: Union[bool, int] = False
@@ -405,15 +431,15 @@
     ) -> tuple[QueryGeneratorFunc, list["sqlalchemy.Column"]]:
         """
         Method that should return query to fetch results from udf and columns
         to select
         """
 
     def udf_table_name(self) -> str:
-        return "udf_" + _random_string(6)
+        return self.catalog.warehouse.UDF_TABLE_NAME_PREFIX + _random_string(6)
 
     @property
     def custom_columns_created(self) -> dict[str, SQLType]:
         return {
             col_name: col_type
             for (col_name, col_type) in self.udf.output.items()
             if col_name not in DATASET_CORE_COLUMN_NAMES
@@ -478,36 +504,56 @@
                 )
                 if result.returncode != 0:
                     raise RuntimeError("UDF Execution Failed!")
             else:
                 # Otherwise process single-threaded (faster for smaller UDFs)
                 # Optionally instantiate the UDF instance if a class is provided.
                 if isinstance(self.udf, UDFFactory):
-                    udf = self.udf()
+                    udf: UDFBase = self.udf()
                 else:
                     udf = self.udf
 
-                udf_inputs = batching(
-                    self.catalog.warehouse.dataset_select_paginated, query
-                )
-                udf_results = (
-                    udf(
-                        self.catalog,
-                        row,
-                        is_generator=self.is_generator,
-                        cache=self.cache,
-                    )
-                    for row in udf_inputs
-                )
-                process_udf_outputs(self.catalog.warehouse, udf_table, udf_results, udf)
-                self.catalog.warehouse.insert_rows_done(udf_table)
+                if hasattr(udf.func, "bootstrap") and callable(udf.func.bootstrap):
+                    udf.func.bootstrap()
+                warehouse = self.catalog.warehouse
+
+                with contextlib.closing(
+                    batching(warehouse.dataset_select_paginated, query)
+                ) as udf_inputs:
+                    processed_cb = get_processed_callback()
+                    generated_cb = get_generated_callback(self.is_generator)
+                    try:
+                        udf_results = run_udf(
+                            udf,
+                            udf_inputs,
+                            self.catalog,
+                            self.is_generator,
+                            self.cache,
+                            processed_cb,
+                        )
+                        process_udf_outputs(
+                            warehouse,
+                            udf_table,
+                            udf_results,
+                            udf,
+                            cb=generated_cb,
+                        )
+                    finally:
+                        processed_cb.close()
+                        generated_cb.close()
+
+                warehouse.insert_rows_done(udf_table)
+
+                if hasattr(udf.func, "teardown") and callable(udf.func.teardown):
+                    udf.func.teardown()
+
         except QueryScriptCancelError:
             self.catalog.warehouse.close()
             sys.exit(QUERY_SCRIPT_CANCELED_EXIT_CODE)
-        except Exception:
+        except (Exception, KeyboardInterrupt):
             # Close any open database connections if an error is encountered
             self.catalog.warehouse.close()
             raise
 
     def create_partitions_table(self, query: Select) -> "Table":
         """
         Create temporary table with group by partitions.
@@ -543,17 +589,18 @@
                 partition_by=partition_by,
                 parallel=self.parallel,
                 workers=self.workers,
                 min_task_size=self.min_task_size,
             )
         return self.__class__(self.udf, self.catalog)
 
-    def apply(self, query_generator: QueryGenerator) -> "StepResult":
+    def apply(
+        self, query_generator: QueryGenerator, temp_tables: list[str]
+    ) -> "StepResult":
         query = query_generator.select()
-        temp_tables = []
 
         # Apply partitioning if needed.
         if self.partition_by is not None:
             partition_tbl = self.create_partitions_table(query)
             temp_tables.append(partition_tbl.name)
 
             subq = query.subquery()
@@ -568,15 +615,15 @@
         for t in tables:
             temp_tables.append(t.name)
         udf_table = self.create_udf_table()
         temp_tables.append(udf_table.name)
         self.populate_udf_table(udf_table, query)
         q, cols = self.create_result_query(udf_table, query)
 
-        return step_result(q, cols, temp_table_names=temp_tables)
+        return step_result(q, cols)
 
 
 @frozen
 class UDFSignal(UDF):
     is_generator = False
 
     def create_udf_table(self) -> "Table":
@@ -712,15 +759,17 @@
             return sqlalchemy.select(*cols).select_from(udf_table_query)
 
         return q, udf_table_query.columns
 
 
 @frozen
 class SQLClause(Step, ABC):
-    def apply(self, query_generator: QueryGenerator) -> StepResult:
+    def apply(
+        self, query_generator: QueryGenerator, temp_tables: list[str]
+    ) -> StepResult:
         query = query_generator.select()
         new_query = self.apply_sql_clause(query)
 
         def q(*columns):
             return new_query.with_only_columns(*columns)
 
         return step_result(q, new_query.selected_columns)
@@ -806,17 +855,21 @@
 
 
 @frozen
 class SQLUnion(Step):
     query1: "DatasetQuery"
     query2: "DatasetQuery"
 
-    def apply(self, query_generator: QueryGenerator) -> StepResult:
+    def apply(
+        self, query_generator: QueryGenerator, temp_tables: list[str]
+    ) -> StepResult:
         q1 = self.query1.apply_steps().select().subquery()
+        temp_tables.extend(self.query1.temp_table_names)
         q2 = self.query2.apply_steps().select().subquery()
+        temp_tables.extend(self.query2.temp_table_names)
         columns1, columns2 = fill_columns(q1.columns, q2.columns)
 
         def q(*columns):
             names = {c.name for c in columns}
             col1 = [c for c in columns1 if c.name in names]
             col2 = [c for c in columns2 if c.name in names]
             res = (
@@ -870,17 +923,21 @@
                         " part of the join"
                     )
                 else:
                     continue
             else:
                 self.validate_expression(c, q1, q2)
 
-    def apply(self, query_generator: QueryGenerator) -> StepResult:
+    def apply(
+        self, query_generator: QueryGenerator, temp_tables: list[str]
+    ) -> StepResult:
         q1 = self.query1.apply_steps().select().subquery(self.query1.table.name)
+        temp_tables.extend(self.query1.temp_table_names)
         q2 = self.query2.apply_steps().select().subquery(self.query2.table.name)
+        temp_tables.extend(self.query2.temp_table_names)
 
         q1_columns = list(q1.c)
         q1_column_names = {c.name for c in q1_columns}
         q2_columns = [
             c
             if c.name not in q1_column_names and c.name != "id"
             else c.label(self.rname.format(name=c.name))
@@ -935,15 +992,17 @@
     """Group rows by a specific column."""
 
     cols: PartitionByType
 
     def clone(self) -> "Self":
         return self.__class__(self.cols)
 
-    def apply(self, query_generator: QueryGenerator) -> StepResult:
+    def apply(
+        self, query_generator: QueryGenerator, temp_tables: list[str]
+    ) -> StepResult:
         query = query_generator.select()
         grouped_query = query.group_by(*self.cols)
 
         def q(*columns):
             return grouped_query.with_only_columns(*columns)
 
         return step_result(q, grouped_query.selected_columns)
@@ -1075,33 +1134,30 @@
 
             # Prepend the chunk filter to the step chain.
             query = query.filter(C.random % total == index)
             query.steps = query.steps[-1:] + query.steps[:-1]
 
         result = query.starting_step.apply()
         group_by = None
-        self.temp_table_names.extend(result.temp_table_names)
         self.dependencies.update(result.dependencies)
 
         for step in query.steps:
             if isinstance(step, GroupBy):
                 if group_by is not None:
                     raise TypeError("only one group_by allowed")
                 group_by = step
                 continue
 
             result = step.apply(
-                result.query_generator
+                result.query_generator, self.temp_table_names
             )  # a chain of steps linked by results
-            self.temp_table_names.extend(result.temp_table_names)
             self.dependencies.update(result.dependencies)
 
         if group_by:
-            result = group_by.apply(result.query_generator)
-            self.temp_table_names.extend(result.temp_table_names)
+            result = group_by.apply(result.query_generator, self.temp_table_names)
             self.dependencies.update(result.dependencies)
 
         return result.query_generator
 
     @staticmethod
     def _chunk_limit(steps: list["Step"], index: int, total: int) -> list["Step"]:
         no_limit_steps = []
@@ -1119,16 +1175,37 @@
             limit = limit // total
             if index < limit_modulo:
                 limit += 1
             return no_limit_steps + [SQLLimit(limit)]
         return steps
 
     def cleanup(self) -> None:
-        self.catalog.warehouse.clone().cleanup_temp_tables(self.temp_table_names)
-        self.catalog.metastore.clone().cleanup_temp_tables(self.temp_table_names)
+        """Cleanup any temporary tables."""
+        if not self.temp_table_names:
+            # Nothing to clean up.
+            return
+        # This is needed to always use a new connection with all metastore and warehouse
+        # implementations, as errors may close or render unusable the existing
+        # connections.
+        (
+            metastore_class,
+            metastore_args,
+            metastore_kwargs,
+        ) = self.catalog.metastore.clone_params()
+        metastore = metastore_class(*metastore_args, **metastore_kwargs)
+        metastore.cleanup_temp_tables(self.temp_table_names)
+        metastore.close()
+        (
+            warehouse_class,
+            warehouse_args,
+            warehouse_kwargs,
+        ) = self.catalog.warehouse.clone_params()
+        warehouse = warehouse_class(*warehouse_args, **warehouse_kwargs)
+        warehouse.cleanup_temp_tables(self.temp_table_names)
+        warehouse.close()
         self.temp_table_names = []
 
     def results(self, row_factory=None, **kwargs):
         with self.as_iterable(**kwargs) as result:
             if row_factory:
                 cols = result.columns
                 return [row_factory(cols, r) for r in result]
@@ -1158,34 +1235,44 @@
         To ensure prompt resource cleanup, it is recommended to wrap this
         with contextlib.closing().
         """
         actual_params = [normalize_param(p) for p in params]
         try:
             query = self.apply_steps().select()
 
-            def row_iter() -> Iterable[DatasetRow]:
+            def row_iter() -> Generator[DatasetRow, None, None]:
                 # warehouse isn't threadsafe, we need to clone() it
                 # in the thread that uses the results
-                db = self.catalog.warehouse.clone()
-                yield from db.dataset_select_paginated(
-                    query, limit=query._limit, order_by=query._order_by_clauses
-                )
+                warehouse = None
+                try:
+                    warehouse = self.catalog.warehouse.clone()
+                    gen = warehouse.dataset_select_paginated(
+                        query, limit=query._limit, order_by=query._order_by_clauses
+                    )
+                    with contextlib.closing(gen) as rows:
+                        yield from rows
+                finally:
+                    # clone doesn't necessarily create a new connection
+                    # we can't do `warehouse.close()` for now. It is a bad design
+                    # in clone / close interface that needs to be fixed.
+                    pass
 
             async def get_params(row: DatasetRow) -> tuple:
                 return tuple(
                     [
                         await p.get_value_async(self.catalog, row, mapper, **kwargs)
                         for p in actual_params
                     ]
                 )
 
             MapperCls = OrderedMapper if query._order_by_clauses else AsyncMapper  # noqa: N806
-            mapper = MapperCls(get_params, row_iter(), workers=workers)
-            for params in mapper.iterate():
-                yield params
+            with contextlib.closing(row_iter()) as rows:
+                mapper = MapperCls(get_params, rows, workers=workers)
+                for params in mapper.iterate():
+                    yield params
         finally:
             self.cleanup()
 
     def to_records(self) -> list[dict]:
         with self.as_iterable() as result:
             cols = result.columns
             return [dict(zip(cols, row)) for row in result]
@@ -1199,46 +1286,19 @@
                 "To install run:\n\n"
                 "  pip install 'dvcx[pandas]'\n"
             ) from exc
 
         records = self.to_records()
         return pd.DataFrame.from_records(records)
 
-    def to_pytorch(
-        self,
-        *params: UDFParamSpec,
-        **kwargs,
-    ) -> "PytorchDataset":
-        try:
-            import torch  # noqa: F401
-        except ImportError as exc:
-            raise ImportError(
-                "Missing required dependency 'torch' for DatasetQuery.to_pytorch()"
-            ) from exc
-        from dvcx.lib.pytorch import PytorchDataset
-
-        if self.attached:
-            ds = self
-        else:
-            ds_name = self.catalog.generate_query_dataset_name()
-            ds = self.save(ds_name)
-        assert ds.name is not None  # for mypy
-        return PytorchDataset(
-            params,
-            ds.name,
-            ds.version,
-            catalog=self.catalog,
-            **kwargs,
-        )
-
     def shuffle(self) -> "DatasetQuery":
         # ToDo: implement shaffle based on seed and/or generating random column
         return self.order_by(C.random)
 
-    def sample(self, n) -> "DatasetQuery":
+    def sample(self, n) -> "Self":
         """
         Return a random sample from the dataset.
 
         Args:
             n (int): Number of samples to draw.
 
         NOTE: Sampled are not deterministic, and streamed/paginated queries or
@@ -1472,17 +1532,17 @@
         For distributed processing with the appropriate distributed module installed,
         workers can optionally be specified as >= 1 for a specific number of workers,
         or set to True for the default of all nodes in the cluster.
         As well, a custom minimum task size (min_task_size) can be provided to send
         at least that minimum number of rows to each distributed worker, mostly useful
         if there are a very large number of small tasks to process.
         """
-        if isinstance(udf, UDFClassWrapper):
+        if isinstance(udf, UDFClassWrapper):  # type: ignore[unreachable]
             # This is a bare decorated class, "instantiate" it now.
-            udf = udf()
+            udf = udf()  # type: ignore[unreachable]
         query = self.clone()
         query.steps.append(
             UDFSignal(
                 udf,
                 self.catalog,
                 partition_by=partition_by,
                 parallel=parallel,
@@ -1511,17 +1571,17 @@
         udf: UDFType,
         parallel: Optional[int] = None,
         workers: Union[bool, int] = False,
         min_task_size: Optional[int] = None,
         partition_by: Optional[PartitionByType] = None,
         cache: bool = False,
     ) -> "Self":
-        if isinstance(udf, UDFClassWrapper):
+        if isinstance(udf, UDFClassWrapper):  # type: ignore[unreachable]
             # This is a bare decorated class, "instantiate" it now.
-            udf = udf()
+            udf = udf()  # type: ignore[unreachable]
         query = self.clone()
         steps = query.steps
         steps.append(
             RowGenerator(
                 udf,
                 self.catalog,
                 partition_by=partition_by,
@@ -1620,14 +1680,15 @@
                 sqlalchemy.insert(dr.get_table()).from_select(cols, q),
                 **kwargs,
             )
 
             self.catalog.metastore.update_dataset_status(
                 dataset, DatasetStatus.COMPLETE, version=version
             )
+            self.catalog.update_dataset_version_with_stats(dataset, version)
 
             self._add_dependencies(dataset, version)  # type: ignore [arg-type]
         finally:
             self.cleanup()
 
         return DatasetQuery(name=name, version=version, catalog=self.catalog)
 
@@ -1641,53 +1702,28 @@
         return int(handle)
 
     import msvcrt
 
     return msvcrt.open_osfhandle(int(handle), os.O_WRONLY)  # type: ignore[attr-defined]
 
 
-def query_wrapper_save(dataset_query: DatasetQuery) -> DatasetQuery:
-    """
-    Wrapper function that wraps the last statement of user query script for creating
-    new dataset
-    Last statement MUST be instance of DatasetQuery, otherwise script exits with
-    error code 10
-    """
-    if not isinstance(dataset_query, DatasetQuery):
-        sys.exit(QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE)
-
-    if dataset_query.attached:
-        name = dataset_query.name
-        version = dataset_query.version
-    else:
-        name = dataset_query.catalog.generate_query_dataset_name()
-        dataset_query.save(name)
-        version = 1
-
-    with open(_get_output_fd_for_write(), mode="w") as out:
-        print(json.dumps({"dataset": (name, version)}), file=out)
-    return dataset_query
-
+@attrs.define
+class ExecutionResult:
+    preview: list[dict] = attrs.field(factory=list)
+    dataset: Optional[tuple[str, int]] = None
 
-def query_wrapper_print(dataset_query: DatasetQuery) -> DatasetQuery:
-    """
-    Wrapper function that wraps the last statement of user query script for printing
-    results in console.
-    Last statement MUST be instance of DatasetQuery, otherwise script exits with
-    error code 10
-    """
 
+def _send_result(
+    dataset_query: DatasetQuery, dataset: Optional[tuple[str, int]] = None
+):
     def _json_serialize(obj):
         if isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
         return obj
 
-    if not isinstance(dataset_query, DatasetQuery):
-        sys.exit(QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE)
-
     try:
         preview_args: dict[str, Any] = json.loads(
             os.getenv("DVCX_QUERY_PREVIEW_ARGS", "")
         )
     except ValueError:
         preview_args = {}
 
@@ -1697,17 +1733,45 @@
 
     preview_query = (
         dataset_query.select(*columns)
         .limit(preview_args.get("limit", 10))
         .offset(preview_args.get("offset", 0))
     )
 
-    with open(_get_output_fd_for_write(), mode="w") as out:
-        d = {"preview": preview_query.to_records()}
-        print(json.dumps(d, default=_json_serialize), file=out)
+    preview = preview_query.to_records()
+    result = ExecutionResult(preview, dataset)
+    data = attrs.asdict(result)
+
+    with open(_get_output_fd_for_write(), mode="w") as f:
+        json.dump(data, f, default=_json_serialize)
+
+
+def query_wrapper(dataset_query: DatasetQuery) -> DatasetQuery:
+    """
+    Wrapper function that wraps the last statement of user query script.
+    Last statement MUST be instance of DatasetQuery, otherwise script exits with
+    error code 10
+    """
+    if not isinstance(dataset_query, DatasetQuery):
+        sys.exit(QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE)
+
+    save = bool(os.getenv("DVCX_QUERY_SAVE"))
+    dataset: Optional[tuple[str, int]] = None
+    if dataset_query.attached:
+        name = dataset_query.name
+        version = dataset_query.version
+        assert name
+        assert version
+        dataset = name, version
+    elif save:
+        name = dataset_query.catalog.generate_query_dataset_name()
+        dataset_query.save(name)
+        version = 1
+        dataset = name, version
+    _send_result(dataset_query, dataset=dataset)
     return dataset_query
 
 
 def _random_string(length: int) -> str:
     return "".join(
         random.choice(string.ascii_letters + string.digits)  # noqa: S311
         for i in range(length)
```

### Comparing `dvcx-0.76.0/src/dvcx/query/dispatch.py` & `dvcx-0.77.0/src/dvcx/query/dispatch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,29 @@
-from collections.abc import Iterable, Iterator
+import contextlib
+from collections.abc import Iterator, Sequence
 from itertools import chain
 from multiprocessing import cpu_count
+from queue import Empty, Full, Queue
 from sys import stdin
+from time import sleep
 from types import GeneratorType
-from typing import Optional
+from typing import Any, Optional
 
 from dill import load
+from fsspec.callbacks import DEFAULT_CALLBACK, Callback
 from multiprocess import get_context
 
 from dvcx.catalog import Catalog
 from dvcx.catalog.loader import get_distributed_class
-from dvcx.query.dataset import process_udf_outputs
+from dvcx.query.batch import DatasetRowsBatch
+from dvcx.query.dataset import (
+    get_generated_callback,
+    get_processed_callback,
+    process_udf_outputs,
+)
 from dvcx.query.udf import UDFFactory, UDFResult
 
 DEFAULT_BATCH_SIZE = 10000
 STOP_SIGNAL = "STOP"
 OK_STATUS = "OK"
 FINISHED_STATUS = "FINISHED"
 FAILED_STATUS = "FAILED"
@@ -28,14 +37,52 @@
     if not n_workers:
         return cpu_count()
     if n_workers < 1:
         raise RuntimeError("Must use at least one worker for parallel UDF execution!")
     return n_workers
 
 
+# For more context on the get_from_queue and put_into_queue functions, see the
+# discussion here:
+# https://github.com/iterative/dvcx/pull/1297#issuecomment-2026308773
+# This problem is not exactly described by, but is also related to these Python issues:
+# https://github.com/python/cpython/issues/66587
+# https://github.com/python/cpython/issues/88628
+# https://github.com/python/cpython/issues/108645
+
+
+def get_from_queue(queue: Queue) -> Any:
+    """
+    Gets an item from a queue.
+    This is required to handle signals, such as KeyboardInterrupt exceptions
+    while waiting for items to be available, although only on certain installations.
+    (See the above comment for more context.)
+    """
+    while True:
+        try:
+            return queue.get_nowait()
+        except Empty:
+            sleep(0.01)
+
+
+def put_into_queue(queue: Queue, item: Any) -> None:
+    """
+    Puts an item into a queue.
+    This is required to handle signals, such as KeyboardInterrupt exceptions
+    while waiting for items to be queued, although only on certain installations.
+    (See the above comment for more context.)
+    """
+    while True:
+        try:
+            queue.put_nowait(item)
+            return
+        except Full:
+            sleep(0.01)
+
+
 def udf_entrypoint() -> int:
     # Load UDF info from stdin
     udf_info = load(stdin.buffer)  # noqa: S301
 
     (
         warehouse_class,
         warehouse_args,
@@ -59,18 +106,28 @@
     table = udf_info["table"]
     n_workers = udf_info["processes"]
     udf = udf_info["udf"]
     if n_workers is True:
         # Use default number of CPUs (cores)
         n_workers = None
 
-    udf_inputs = batching(warehouse.dataset_select_paginated, query)
-    udf_results = dispatch.run_udf_parallel(udf_inputs, n_workers=n_workers)
+    with contextlib.closing(
+        batching(warehouse.dataset_select_paginated, query)
+    ) as udf_inputs:
+        processed_cb = get_processed_callback()
+        generated_cb = get_generated_callback(dispatch.is_generator)
+        try:
+            udf_results = dispatch.run_udf_parallel(
+                udf_inputs, n_workers=n_workers, cb=processed_cb
+            )
+            process_udf_outputs(warehouse, table, udf_results, udf, cb=generated_cb)
+        finally:
+            processed_cb.close()
+            generated_cb.close()
 
-    process_udf_outputs(warehouse, table, udf_results, udf)
     warehouse.insert_rows_done(table)
 
     return 0
 
 
 def udf_worker_entrypoint() -> int:
     return get_distributed_class().run_worker()
@@ -148,64 +205,65 @@
                 *self.warehouse_args, **self.warehouse_kwargs
             )
             self.catalog = Catalog(
                 id_generator, metastore, warehouse, **self.catalog_init_params
             )
         if not self.udf:
             self.udf = self.udf_factory()
+
+        if hasattr(self.udf.func, "bootstrap") and callable(self.udf.func.bootstrap):
+            self.udf.func.bootstrap()
+
         self.initialized = True
 
     def _run_worker(self):
         try:
             self._init_worker()
-            for row in iter(self.task_queue.get, STOP_SIGNAL):
-                udf_output = self._call_udf(row)
-                if isinstance(udf_output, GeneratorType):
-                    udf_output = list(udf_output)  # can not pickle generator
-                self.done_queue.put({"status": OK_STATUS, "result": udf_output})
-            # Finalize UDF, clearing the batch collection and returning
-            # any held results
-            if udf_output := self._finalize_udf():
+            while (batch := get_from_queue(self.task_queue)) != STOP_SIGNAL:
+                n_rows = len(batch.rows) if isinstance(batch, DatasetRowsBatch) else 1
+                udf_output = self._call_udf(batch)
                 if isinstance(udf_output, GeneratorType):
                     udf_output = list(udf_output)  # can not pickle generator
-                self.done_queue.put({"status": OK_STATUS, "result": udf_output})
-            self.done_queue.put({"status": FINISHED_STATUS})
-        except Exception as e:
-            self.done_queue.put({"status": FAILED_STATUS, "exception": e})
+                put_into_queue(
+                    self.done_queue,
+                    {"status": OK_STATUS, "result": udf_output, "processed": n_rows},
+                )
+
+            if hasattr(self.udf.func, "teardown") and callable(self.udf.func.teardown):
+                self.udf.func.teardown()
+
+            put_into_queue(self.done_queue, {"status": FINISHED_STATUS})
+        except (Exception, KeyboardInterrupt) as e:
+            put_into_queue(self.done_queue, {"status": FAILED_STATUS, "exception": e})
             raise e
 
     def _call_udf(self, row):
         if not self.initialized:
             raise RuntimeError("Internal Error: Attempted to call uninitialized UDF!")
         return self.udf(
             self.catalog, row, is_generator=self.is_generator, cache=self.cache
         )
 
-    def _finalize_udf(self):
-        if not self.initialized:
-            raise RuntimeError("Internal Error: Attempted to call uninitialized UDF!")
-        if hasattr(self.udf, "finalize"):
-            return self.udf.finalize()
-        return None
-
-    def send_stop_signal_to_workers(self, task_queue, n_workers: Optional[int] = None):
+    @staticmethod
+    def send_stop_signal_to_workers(task_queue, n_workers: Optional[int] = None):
         n_workers = get_n_workers_from_arg(n_workers)
         for _ in range(n_workers):
-            task_queue.put(STOP_SIGNAL)
+            put_into_queue(task_queue, STOP_SIGNAL)
 
     def create_input_queue(self):
         return self.ctx.Queue()
 
     def run_udf_parallel(  # noqa: C901, PLR0912
         self,
         input_rows,
         n_workers: Optional[int] = None,
         cache: bool = False,
         input_queue=None,
-    ) -> Iterator[Iterable[UDFResult]]:
+        cb: Callback = DEFAULT_CALLBACK,
+    ) -> Iterator[Sequence[UDFResult]]:
         n_workers = get_n_workers_from_arg(n_workers)
 
         if self.buffer_size < n_workers:
             raise RuntimeError(
                 f"Parallel run error: buffer size is smaller than "
                 f"number of workers: {self.buffer_size} < {n_workers}"
             )
@@ -233,60 +291,61 @@
             if not streaming_mode:
                 # Stop all workers after the input rows have finished processing
                 input_data = chain(input_rows, [STOP_SIGNAL] * n_workers)
 
                 # Add initial buffer of tasks
                 for _ in range(self.buffer_size):
                     try:
-                        self.task_queue.put(next(input_data))
+                        put_into_queue(self.task_queue, next(input_data))
                     except StopIteration:
                         input_finished = True
                         break
 
             # Process all tasks
             while n_workers > 0:
-                result = self.done_queue.get()
+                result = get_from_queue(self.done_queue)
                 status = result["status"]
                 if status == FINISHED_STATUS:
                     # Worker finished
                     n_workers -= 1
                 elif status == OK_STATUS:
+                    cb.relative_update(result["processed"])
                     yield result["result"]
                 else:  # Failed / error
                     n_workers -= 1
                     exc = result.get("exception")
                     if exc:
                         raise exc
                     raise RuntimeError("Internal error: Parallel UDF execution failed")
 
                 if not streaming_mode and not input_finished:
                     try:
-                        self.task_queue.put(next(input_data))
+                        put_into_queue(self.task_queue, next(input_data))
                     except StopIteration:
                         input_finished = True
 
             # Finished with all tasks normally
             normal_completion = True
         finally:
             if not normal_completion:
                 # Stop all workers if there is an unexpected exception
                 for _ in pool:
-                    self.task_queue.put(STOP_SIGNAL)
+                    put_into_queue(self.task_queue, STOP_SIGNAL)
                 self.task_queue.close()
 
                 # This allows workers (and this process) to exit without
                 # consuming any remaining data in the queues.
                 # (If they exit due to an exception.)
                 self.task_queue.cancel_join_thread()
                 self.done_queue.cancel_join_thread()
 
                 # Flush all items from the done queue.
                 # This is needed if any workers are still running.
                 while n_workers > 0:
-                    result = self.done_queue.get()
+                    result = get_from_queue(self.done_queue)
                     status = result["status"]
                     if status != OK_STATUS:
                         n_workers -= 1
 
             # Wait for workers to stop
             for p in pool:
                 p.join()
```

### Comparing `dvcx-0.76.0/src/dvcx/query/schema.py` & `dvcx-0.77.0/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/query/session.py` & `dvcx-0.77.0/src/dvcx/query/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,11 +89,19 @@
 
         if cls.GLOBAL_SESSION is None:
             cls.GLOBAL_SESSION_CTX = Session(cls.GLOBAL_SESSION_NAME, catalog)
             cls.GLOBAL_SESSION = cls.GLOBAL_SESSION_CTX.__enter__()
             atexit.register(cls._global_cleanup)
         return cls.GLOBAL_SESSION
 
+    @classmethod
+    def cleanup_for_tests(cls):
+        if cls.GLOBAL_SESSION_CTX is not None:
+            cls.GLOBAL_SESSION_CTX.__exit__(None, None, None)
+            cls.GLOBAL_SESSION = None
+            cls.GLOBAL_SESSION_CTX = None
+            atexit.unregister(cls._global_cleanup)
+
     @staticmethod
     def _global_cleanup():
         if Session.GLOBAL_SESSION_CTX is not None:
             Session.GLOBAL_SESSION_CTX.__exit__(None, None, None)
```

### Comparing `dvcx-0.76.0/src/dvcx/query/udf.py` & `dvcx-0.77.0/src/dvcx/query/udf.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         self.udf_class = udf_class
         self.udf_method = method
         self.args = args
         self.kwargs = kwargs
         self.properties = properties
         self.output = properties.output
 
-    def __call__(self):
+    def __call__(self) -> UDFWrapper:
         udf_func = self.udf_class(*self.args, **self.kwargs)
         if self.udf_method:
             udf_func = getattr(udf_func, self.udf_method)
 
         return UDFWrapper(udf_func, self.properties)
```

### Comparing `dvcx-0.76.0/src/dvcx/remote/studio.py` & `dvcx-0.77.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/sql/default/base.py` & `dvcx-0.77.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/sql/functions/array.py` & `dvcx-0.77.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/sql/functions/path.py` & `dvcx-0.77.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/sql/selectable.py` & `dvcx-0.77.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.77.0/src/dvcx/sql/sqlite/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,20 +243,20 @@
 
 def compile_path_file_ext(element, compiler, **kwargs):
     return compiler.process(path_file_ext(*element.clauses.clauses), **kwargs)
 
 
 def compile_cosine_distance(element, compiler, **kwargs):
     run_compiler_hook("cosine_distance")
-    return "cosine_distance(%s)" % compiler.process(element.clauses, **kwargs)
+    return f"cosine_distance({compiler.process(element.clauses, **kwargs)})"
 
 
 def compile_euclidean_distance(element, compiler, **kwargs):
     run_compiler_hook("euclidean_distance")
-    return "euclidean_distance(%s)" % compiler.process(element.clauses, **kwargs)
+    return f"euclidean_distance({compiler.process(element.clauses, **kwargs)})"
 
 
 def py_json_array_length(arr):
     return len(ujson.loads(arr))
 
 
 def compile_array_length(element, compiler, **kwargs):
```

### Comparing `dvcx-0.76.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.77.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/sql/types.py` & `dvcx-0.77.0/src/dvcx/sql/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 _read_converter_registry: dict[str, "TypeReadConverter"] = {}
 read_converter_registry = MappingProxyType(_read_converter_registry)
 
 _type_defaults_registry: dict[str, "TypeDefaults"] = {}
 type_defaults_registry = MappingProxyType(_type_defaults_registry)
 
+NullType = types.NullType
+
 
 def register_backend_types(dialect_name: str, type_cls):
     _registry[dialect_name] = type_cls
 
 
 def register_type_read_converters(dialect_name: str, trc: "TypeReadConverter"):
     _read_converter_registry[dialect_name] = trc
```

### Comparing `dvcx-0.76.0/src/dvcx/sql/utils.py` & `dvcx-0.77.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/storage.py` & `dvcx-0.77.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx/utils.py` & `dvcx-0.77.0/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.77.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.76.0
+Version: 0.77.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,14 +15,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: tomlkit
 Requires-Dist: tqdm
 Requires-Dist: pandas
+Requires-Dist: typing-extensions
 Requires-Dist: python-dateutil>=2
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: s3fs>=2024.2.0
 Requires-Dist: gcsfs>=2024.2.0
 Requires-Dist: adlfs>=2024.2.0
 Requires-Dist: dvc-data<4,>=3.10
 Requires-Dist: dvc-objects<6,>=4
@@ -66,15 +67,15 @@
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
 Requires-Dist: open_clip_torch; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: dvcx[tests]; extra == "dev"
-Requires-Dist: mypy==1.9.0; extra == "dev"
+Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 
 |PyPI| |Status| |Python Version| |License|
 
 |Tests| |Codecov| |pre-commit| |Black|
```

### Comparing `dvcx-0.76.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.77.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 examples/blip2_image_desc_lib.py
 examples/clip.py
 examples/common_sql_functions.py
 examples/dir_expansion.py
 examples/hf_pipeline.py
 examples/iptc_exif_xmp_lib.py
 examples/llava2_image_desc_lib.py
+examples/llm-claude-aggregate-query.py
+examples/llm-claude-simple-query.py
+examples/llm-claude.py
 examples/loader.py
 examples/openai_image_desc_lib.py
 examples/openimage-detect.py
 examples/pose_detection.py
 examples/torch-loader.py
 examples/unstructured-text.py
 examples/wds.py
@@ -97,36 +100,42 @@
 src/dvcx/data_storage/metastore.py
 src/dvcx/data_storage/schema.py
 src/dvcx/data_storage/serializer.py
 src/dvcx/data_storage/sqlite.py
 src/dvcx/data_storage/warehouse.py
 src/dvcx/lib/__init__.py
 src/dvcx/lib/cached_stream.py
+src/dvcx/lib/claude.py
 src/dvcx/lib/dataset.py
 src/dvcx/lib/feature.py
+src/dvcx/lib/feature_types.py
 src/dvcx/lib/feature_udf.py
 src/dvcx/lib/file.py
 src/dvcx/lib/gpt4_vision.py
 src/dvcx/lib/hf_image_to_text.py
 src/dvcx/lib/hf_pipeline.py
+src/dvcx/lib/image.py
 src/dvcx/lib/image_transform.py
 src/dvcx/lib/iptc_exif_xmp.py
 src/dvcx/lib/param.py
 src/dvcx/lib/pytorch.py
+src/dvcx/lib/tar_file.py
+src/dvcx/lib/text.py
 src/dvcx/lib/udf.py
 src/dvcx/lib/unstructured.py
 src/dvcx/lib/utils.py
 src/dvcx/lib/webdataset.py
 src/dvcx/lib/webdataset_laion.py
 src/dvcx/lib/webdataset_meta.py
 src/dvcx/query/__init__.py
 src/dvcx/query/batch.py
 src/dvcx/query/builtins.py
 src/dvcx/query/dataset.py
 src/dvcx/query/dispatch.py
+src/dvcx/query/params.py
 src/dvcx/query/schema.py
 src/dvcx/query/session.py
 src/dvcx/query/udf.py
 src/dvcx/remote/__init__.py
 src/dvcx/remote/studio.py
 src/dvcx/sql/__init__.py
 src/dvcx/sql/selectable.py
@@ -144,44 +153,49 @@
 src/dvcx/sql/sqlite/base.py
 src/dvcx/sql/sqlite/types.py
 src/dvcx/sql/sqlite/vector.py
 tests/__init__.py
 tests/conftest.py
 tests/data.py
 tests/test_cli_e2e.py
+tests/test_query_e2e.py
 tests/utils.py
 tests/benchmarks/__init__.py
 tests/benchmarks/conftest.py
 tests/benchmarks/test_ls.py
 tests/benchmarks/test_version.py
 tests/func/__init__.py
 tests/func/test_catalog.py
 tests/func/test_client.py
 tests/func/test_dataset_query.py
 tests/func/test_datasets.py
 tests/func/test_ls.py
 tests/func/test_pull.py
 tests/func/test_pytorch.py
 tests/func/test_query.py
+tests/scripts/name_len_normal.py
+tests/scripts/name_len_slow.py
 tests/unit/__init__.py
 tests/unit/test_asyn.py
 tests/unit/test_cache.py
 tests/unit/test_catalog.py
 tests/unit/test_catalog_formats.py
 tests/unit/test_catalog_loader.py
 tests/unit/test_cli_parsing.py
 tests/unit/test_client.py
 tests/unit/test_client_s3.py
 tests/unit/test_data_storage.py
 tests/unit/test_database_engine.py
 tests/unit/test_dataset.py
+tests/unit/test_dispatch.py
 tests/unit/test_fileslice.py
 tests/unit/test_id_generator.py
 tests/unit/test_listing.py
 tests/unit/test_metastore.py
+tests/unit/test_query_params.py
 tests/unit/test_serializer.py
 tests/unit/test_session.py
 tests/unit/test_storage.py
 tests/unit/test_udf.py
 tests/unit/test_utils.py
 tests/unit/test_warehouse.py
 tests/unit/lib/test_cached_stream.py
```

### Comparing `dvcx-0.76.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.77.0/src/dvcx.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 pyyaml
 tomlkit
 tqdm
 pandas
+typing-extensions
 python-dateutil>=2
 attrs>=21.3.0
 s3fs>=2024.2.0
 gcsfs>=2024.2.0
 adlfs>=2024.2.0
 dvc-data<4,>=3.10
 dvc-objects<6,>=4
@@ -22,15 +23,15 @@
 torch>=2.1.0
 torchvision
 numpy
 transformers>=4.36.0
 
 [dev]
 dvcx[tests]
-mypy==1.9.0
+mypy==1.10.0
 types-python-dateutil
 types-PyYAML
 types-requests
 
 [pandas]
 pandas>=1.4.0
```

### Comparing `dvcx-0.76.0/tests/benchmarks/conftest.py` & `dvcx-0.77.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/conftest.py` & `dvcx-0.77.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import uuid
 from collections.abc import Generator
 from pathlib import PosixPath
 
 import attrs
 import pytest
 import pytest_servers.exceptions
+import sqlalchemy
 from pytest import MonkeyPatch, TempPathFactory
 from upath.implementations.cloud import CloudPath
 
 from dvcx.catalog import Catalog
 from dvcx.catalog.loader import get_id_generator, get_metastore, get_warehouse
 from dvcx.data_storage.sqlite import (
     SQLiteDatabaseEngine,
     SQLiteIDGenerator,
     SQLiteMetastore,
     SQLiteWarehouse,
 )
 from dvcx.dataset import DatasetRecord
+from dvcx.query.session import Session
 from dvcx.utils import DVCXDir, get_env_list
 
 from .utils import DEFAULT_TREE, get_simple_ds_query, instantiate_tree
 
 DEFAULT_DVCX_BIN = "dvcx"
 DEFAULT_DVCX_GIT_REPO = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
@@ -79,53 +81,85 @@
     for table in reversed(cleanup_tables):
         db.execute_str(f"DROP TABLE IF EXISTS '{table}'")
 
     for (table,) in tables:
         name = table.replace("'", "''")
         db.execute_str(f"DROP TABLE IF EXISTS '{name}'")
 
+    # Close the connection so that the SQLite file is no longer open, to avoid
+    # pytest throwing: OSError: [Errno 24] Too many open files
+    db.close()
+
 
 @pytest.fixture
 def id_generator():
     if os.environ.get("DVCX_ID_GENERATOR"):
         _id_generator = get_id_generator()
     else:
         db = SQLiteDatabaseEngine.from_db_file(":memory:")
         _id_generator = SQLiteIDGenerator(db)
     yield _id_generator
     _id_generator.cleanup_for_tests()
 
+    if not os.environ.get("DVCX_ID_GENERATOR"):
+        # Close the connection so that the SQLite file is no longer open, to avoid
+        # pytest throwing: OSError: [Errno 24] Too many open files
+        _id_generator.db.close()
+
 
 @pytest.fixture
 def metastore(id_generator):
     if os.environ.get("DVCX_METASTORE"):
         _metastore = get_metastore(id_generator)
         yield _metastore
 
         _metastore.cleanup_for_tests()
     else:
         _metastore = SQLiteMetastore(id_generator, db_file=":memory:")
         yield _metastore
 
         cleanup_sqlite_db(_metastore.db.clone(), _metastore.default_table_names)
+        Session.cleanup_for_tests()
+
+        # Close the connection so that the SQLite file is no longer open, to avoid
+        # pytest throwing: OSError: [Errno 24] Too many open files
+        _metastore.db.close()
+
+
+def check_temp_tables_cleaned_up(original_warehouse):
+    """Ensure that temporary tables are cleaned up."""
+    warehouse = original_warehouse.clone()
+    assert [
+        t
+        for t in sqlalchemy.inspect(warehouse.db.engine).get_table_names()
+        if t.startswith(
+            (warehouse.UDF_TABLE_NAME_PREFIX, warehouse.TMP_TABLE_NAME_PREFIX)
+        )
+    ] == []
 
 
 @pytest.fixture
 def warehouse(id_generator, metastore):
     if os.environ.get("DVCX_WAREHOUSE"):
         _warehouse = get_warehouse(id_generator)
         yield _warehouse
+        check_temp_tables_cleaned_up(_warehouse)
 
         _warehouse.cleanup_for_tests()
     else:
         _warehouse = SQLiteWarehouse(id_generator, db_file=":memory:")
         yield _warehouse
+        check_temp_tables_cleaned_up(_warehouse)
 
         cleanup_sqlite_db(_warehouse.db.clone(), metastore.default_table_names)
 
+        # Close the connection so that the SQLite file is no longer open, to avoid
+        # pytest throwing: OSError: [Errno 24] Too many open files
+        _warehouse.db.close()
+
 
 @pytest.fixture
 def catalog(id_generator, metastore, warehouse):
     return Catalog(id_generator=id_generator, metastore=metastore, warehouse=warehouse)
 
 
 @pytest.fixture
@@ -134,42 +168,58 @@
         _id_generator = get_id_generator()
     else:
         db = SQLiteDatabaseEngine.from_db_file(tmp_path / "test.db")
         _id_generator = SQLiteIDGenerator(db)
     yield _id_generator
     _id_generator.cleanup_for_tests()
 
+    if not os.environ.get("DVCX_ID_GENERATOR"):
+        # Close the connection so that the SQLite file is no longer open, to avoid
+        # pytest throwing: OSError: [Errno 24] Too many open files
+        _id_generator.db.close()
+
 
 @pytest.fixture
 def metastore_tmpfile(tmp_path, id_generator_tmpfile):
     if os.environ.get("DVCX_METASTORE"):
         _metastore = get_metastore(id_generator_tmpfile)
         yield _metastore
 
         _metastore.cleanup_for_tests()
     else:
         _metastore = SQLiteMetastore(id_generator_tmpfile, db_file=tmp_path / "test.db")
         yield _metastore
 
         cleanup_sqlite_db(_metastore.db.clone(), _metastore.default_table_names)
+        Session.cleanup_for_tests()
+
+        # Close the connection so that the SQLite file is no longer open, to avoid
+        # pytest throwing: OSError: [Errno 24] Too many open files
+        _metastore.db.close()
 
 
 @pytest.fixture
 def warehouse_tmpfile(tmp_path, id_generator_tmpfile, metastore_tmpfile):
     if os.environ.get("DVCX_WAREHOUSE"):
         _warehouse = get_warehouse(id_generator_tmpfile)
         yield _warehouse
+        check_temp_tables_cleaned_up(_warehouse)
 
         _warehouse.cleanup_for_tests()
     else:
         _warehouse = SQLiteWarehouse(id_generator_tmpfile, db_file=tmp_path / "test.db")
         yield _warehouse
+        check_temp_tables_cleaned_up(_warehouse)
 
         cleanup_sqlite_db(_warehouse.db.clone(), metastore_tmpfile.default_table_names)
 
+        # Close the connection so that the SQLite file is no longer open, to avoid
+        # pytest throwing: OSError: [Errno 24] Too many open files
+        _warehouse.db.close()
+
 
 @pytest.fixture
 def tmp_dir(tmp_path_factory, monkeypatch):
     dpath = tmp_path_factory.mktemp("dvcx-test")
     monkeypatch.chdir(dpath)
     return dpath
```

### Comparing `dvcx-0.76.0/tests/data.py` & `dvcx-0.77.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/func/test_catalog.py` & `dvcx-0.77.0/tests/func/test_catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from urllib.parse import urlparse
 
 import pytest
 import yaml
 from fsspec.implementations.local import LocalFileSystem
 
 from dvcx.catalog import indexer_formats, parse_edvcx_file
+from dvcx.cli import garbage_collect
 from dvcx.error import (
     QueryScriptCompileError,
     QueryScriptDatasetNotFound,
     QueryScriptRunError,
     StorageNotFoundError,
 )
 
@@ -948,14 +949,30 @@
         "dog3",
         "dog4",
     }
     assert dataset.query_script == query_script
     assert dataset.sources == ""
 
 
+def test_query_save_size(cloud_test_catalog, mock_popen_dataset_created):
+    catalog = cloud_test_catalog.catalog
+    src_uri = cloud_test_catalog.src_uri
+
+    query_script = f"""\
+    from dvcx.query import C, DatasetQuery
+    DatasetQuery({src_uri!r})
+    """
+    query_script = dedent(query_script)
+
+    dataset, version, _, _ = catalog.query(query_script, save=True)
+    dataset_version = dataset.get_version(version)
+    assert dataset_version.num_objects == 4
+    assert dataset_version.size == 15
+
+
 def test_query_fail_to_compile(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
 
     query_script = "syntax error"
 
     with pytest.raises(QueryScriptCompileError):
         catalog.query(query_script)
@@ -1039,7 +1056,24 @@
     assert stats.num_objects == 11
     assert stats.size == 36
 
     catalog.enlist_source(f"{src_uri}/dogs/", ttl=1234, force_update=True)
     stats = catalog.storage_stats(src_uri)
     assert stats.num_objects == 6
     assert stats.size == 15
+
+
+@pytest.mark.parametrize("from_cli", [False, True])
+def test_garbage_collect(cloud_test_catalog, from_cli, capsys):
+    catalog = cloud_test_catalog.catalog
+    assert catalog.get_temp_table_names() == []
+    temp_tables = ["tmp_vc12F", "udf_jh653", "ds_shadow_12345", "old_ds_shadow"]
+    for t in temp_tables:
+        catalog.warehouse.create_udf_table(t)
+    assert set(catalog.get_temp_table_names()) == set(temp_tables)
+    if from_cli:
+        garbage_collect(catalog)
+        captured = capsys.readouterr()
+        assert captured.out == "Garbage collecting 4 tables.\n"
+    else:
+        catalog.cleanup_temp_tables(temp_tables)
+    assert catalog.get_temp_table_names() == []
```

### Comparing `dvcx-0.76.0/tests/func/test_client.py` & `dvcx-0.77.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/func/test_dataset_query.py` & `dvcx-0.77.0/tests/func/test_dataset_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 
 import numpy as np
 import pytest
 import sqlalchemy
 from dateutil.parser import isoparse
 from sqlalchemy import tuple_
 
-from dvcx.catalog import indexer_formats
+from dvcx.catalog import QUERY_SCRIPT_CANCELED_EXIT_CODE, indexer_formats
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.data_storage.warehouse import RANDOM_BITS
 from dvcx.dataset import DatasetDependencyType
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetInvalidVersionError, DatasetNotFoundError
-from dvcx.lib.param import Label, Text
 from dvcx.node import Node
 from dvcx.query import (
     C,
     DatasetQuery,
     DatasetRow,
     LocalFilename,
     Object,
@@ -674,20 +673,14 @@
         .filter(C.parent.glob("cats*") | (C.size < 4))
         .add_signals(name_len)
     )
     result1 = q.select(C.name, C.name_len).results()
     # ensure that we're able to run with same query multiple times
     result2 = q.select(C.name, C.name_len).results()
     count = q.count()
-    # ensure that temporary tables are cleaned up
-    assert [
-        t
-        for t in sqlalchemy.inspect(catalog.warehouse.db.engine).get_table_names()
-        if t.startswith("udf_")
-    ] == []
     assert len(result1) == 3
     assert len(result2) == 3
     assert count == 3
 
     for r1, r2 in zip(result1, result2):
         # Check that the UDF ran successfully
         assert len(r1[0]) == r1[1]
@@ -996,21 +989,51 @@
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
+def test_udf_parallel_interrupt(cloud_test_catalog_tmpfile, capfd):
+    catalog = cloud_test_catalog_tmpfile.catalog
+    sources = [cloud_test_catalog_tmpfile.src_uri]
+    globs = [s.rstrip("/") + "/*" for s in sources]
+    catalog.index(sources)
+    catalog.create_dataset_from_sources("animals", globs, recursive=True)
+
+    @udf(("name",), {"name_len": Int})
+    def name_len_interrupt(_name):
+        # A UDF that emulates cancellation due to a KeyboardInterrupt.
+        raise KeyboardInterrupt
+
+    q = (
+        DatasetQuery(name="animals", version=1, catalog=catalog)
+        .filter(C.size < 13)
+        .filter(C.parent.glob("cats*") | (C.size < 4))
+        .add_signals(name_len_interrupt, parallel=-1)
+    )
+    with pytest.raises(RuntimeError, match="UDF Execution Failed!"):
+        q.results()
+    captured = capfd.readouterr()
+    assert "KeyboardInterrupt" in captured.err
+    assert "semaphore" not in captured.err
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
 @pytest.mark.parametrize("batch", [False, True])
 @pytest.mark.parametrize("workers", (1, 2))
+@pytest.mark.skipif(
+    "not os.environ.get('DVCX_DISTRIBUTED')",
+    reason="Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs",
+)
 def test_udf_distributed(cloud_test_catalog_tmpfile, batch, workers):
-    if not os.environ.get("DVCX_DISTRIBUTED"):
-        pytest.skip(
-            "Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs"
-        )
     catalog = cloud_test_catalog_tmpfile.catalog
     sources = [cloud_test_catalog_tmpfile.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
     catalog.create_dataset_from_sources("animals", globs, recursive=True)
 
     @udf(("name",), {"name_len": Int, "blank": String})
@@ -1048,19 +1071,19 @@
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
 @pytest.mark.parametrize("workers", (1, 2))
+@pytest.mark.skipif(
+    "not os.environ.get('DVCX_DISTRIBUTED')",
+    reason="Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs",
+)
 def test_udf_distributed_exec_error(cloud_test_catalog_tmpfile, workers):
-    if not os.environ.get("DVCX_DISTRIBUTED"):
-        pytest.skip(
-            "Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs"
-        )
     catalog = cloud_test_catalog_tmpfile.catalog
     sources = [cloud_test_catalog_tmpfile.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
     catalog.create_dataset_from_sources("animals", globs, recursive=True)
 
     @udf((C.name,), {"name_len": Int})
@@ -1074,14 +1097,105 @@
         .filter(C.parent.glob("cats*") | (C.size < 4))
         .add_signals(name_len_error, parallel=2, workers=workers)
     )
     with pytest.raises(RuntimeError, match="Test Error!"):
         q.results()
 
 
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+@pytest.mark.skipif(
+    "not os.environ.get('DVCX_DISTRIBUTED')",
+    reason="Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs",
+)
+def test_udf_distributed_interrupt(cloud_test_catalog_tmpfile, capfd):
+    catalog = cloud_test_catalog_tmpfile.catalog
+    sources = [cloud_test_catalog_tmpfile.src_uri]
+    globs = [s.rstrip("/") + "/*" for s in sources]
+    catalog.index(sources)
+    catalog.create_dataset_from_sources("animals", globs, recursive=True)
+
+    @udf(("name",), {"name_len": Int})
+    def name_len_interrupt(_name):
+        # A UDF that emulates cancellation due to a KeyboardInterrupt.
+        raise KeyboardInterrupt
+
+    q = (
+        DatasetQuery(name="animals", version=1, catalog=catalog)
+        .filter(C.size < 13)
+        .filter(C.parent.glob("cats*") | (C.size < 4))
+        .add_signals(name_len_interrupt, parallel=2, workers=2)
+    )
+    with pytest.raises(RuntimeError, match=r"Worker Killed \(KeyboardInterrupt\)"):
+        q.results()
+    captured = capfd.readouterr()
+    assert "KeyboardInterrupt" in captured.err
+    assert "semaphore" not in captured.err
+
+
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True)],
+    indirect=True,
+)
+@pytest.mark.skipif(
+    "not os.environ.get('DVCX_DISTRIBUTED')",
+    reason="Set the DVCX_DISTRIBUTED environment variable to test distributed UDFs",
+)
+def test_udf_distributed_cancel(cloud_test_catalog_tmpfile, capfd, monkeypatch):
+    catalog = cloud_test_catalog_tmpfile.catalog
+    metastore = catalog.metastore
+    sources = [cloud_test_catalog_tmpfile.src_uri]
+    globs = [s.rstrip("/") + "/*" for s in sources]
+    catalog.index(sources)
+    catalog.create_dataset_from_sources("animals", globs, recursive=True)
+
+    job_id = "a53bb062dfdf437baf6003795a62d17d"
+
+    # A job is required for query script cancellation (not using a KeyboardInterrupt)
+    metastore.db.execute(
+        metastore._jobs_insert().values(
+            id=job_id,
+            status=7,  # CANCELING
+            celery_task_id="",
+            name="Test Cancel Job",
+            workers=2,
+            team_id=metastore.team_id,
+            created_at=datetime.now(timezone.utc),
+        ),
+    )
+    monkeypatch.setenv("DVCX_JOB_ID", job_id)
+
+    @udf(("name",), {"name_len": Int})
+    def name_len_slow(name):
+        # A very simple udf, that processes slowly to emulate being stuck.
+        from time import sleep
+
+        sleep(10)
+        return len(name), None
+
+    q = (
+        DatasetQuery(name="animals", version=1, catalog=catalog)
+        .filter(C.size < 13)
+        .filter(C.parent.glob("cats*") | (C.size < 4))
+        .add_signals(name_len_slow, parallel=2, workers=2)
+    )
+
+    with pytest.raises(SystemExit) as excinfo:
+        q.results()
+
+    assert excinfo.value.code == QUERY_SCRIPT_CANCELED_EXIT_CODE
+    captured = capfd.readouterr()
+    assert "canceled" in captured.out
+    assert "semaphore" not in captured.err
+
+
 def test_apply_udf(cloud_test_catalog, tmp_path):
     catalog = cloud_test_catalog.catalog
     sources = [cloud_test_catalog.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
     catalog.create_dataset_from_sources("animals", globs, recursive=True)
 
@@ -1254,61 +1368,14 @@
     q = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
     results = list(q.order_by("random").extract("name"))
     pairs = list(q.extract("random", "name"))
     assert results == [(p[1],) for p in sorted(pairs)]
 
 
 @pytest.mark.parametrize(
-    "cloud_type, version_aware",
-    [("file", False)],
-    indirect=True,
-)
-def test_label_param(cloud_test_catalog, listed_bucket):
-    ctc = cloud_test_catalog
-
-    @udf(params=("name",), output={"label": String})
-    def extract_label(name):
-        return (name[:3],)
-
-    ds = (
-        DatasetQuery(ctc.src_uri, catalog=ctc.catalog)
-        .add_signals(extract_label)
-        .filter(C("label").in_(["cat", "dog"]))
-        .save("cats-dogs")
-    )
-    results = list(ds.order_by("name").extract(Label("label", ["cat", "dog"])))
-    assert results == [(0,)] * 2 + [(1,)] * 4
-
-
-# Test hf and non-hf tokenizers
-@pytest.mark.parametrize("tokenizer_model", ["ViT-B-32", "hf-hub:timm/ViT-B-16-SigLIP"])
-@pytest.mark.parametrize(
-    "cloud_type, version_aware",
-    [("file", False)],
-    indirect=True,
-)
-def test_text_param(cloud_test_catalog, listed_bucket, tokenizer_model):
-    import open_clip
-    import torch
-
-    ctc = cloud_test_catalog
-
-    @udf(params=("name",), output={"text": String})
-    def extract_text(name):
-        return (name,)
-
-    ds = DatasetQuery(ctc.src_uri, catalog=ctc.catalog).add_signals(extract_text)
-
-    tokenizer = open_clip.get_tokenizer(tokenizer_model)
-
-    for row in ds.extract(Text("text", tokenizer)):
-        assert row[0].dtype == torch.int64
-
-
-@pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
 def test_union(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
     sources = [str(cloud_test_catalog.src_uri)]
@@ -2597,15 +2664,14 @@
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
-@pytest.mark.skip(reason="Test fails on other platforms because of db being locked")
 def test_row_generator_with_new_columns_wrong_type(cloud_test_catalog, dogs_dataset):
     catalog = cloud_test_catalog.catalog
 
     @udf(
         params=(C.name, C.parent),
         output={**DatasetRow.schema, "int_col": Int},
         method="generate_subobjects",
@@ -3175,58 +3241,14 @@
     import pandas as pd
 
     df = simple_ds_query.to_pandas()
     expected = pd.DataFrame.from_records(SIMPLE_DS_QUERY_RECORDS)
     assert (df == expected).all(axis=None)
 
 
-@pytest.mark.parametrize("use_cache", [False, True])
-@pytest.mark.parametrize("cloud_type,version_aware", [("file", False)], indirect=True)
-def test_to_pytorch(cloud_test_catalog, dogs_dataset, use_cache):
-    from torch.utils.data import IterableDataset
-
-    catalog = cloud_test_catalog.catalog
-    q = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
-    results = set()
-    pt_dataset = q.to_pytorch("name", Stream(), cache=use_cache)
-    assert isinstance(pt_dataset, IterableDataset)
-    for name, stream in pt_dataset:
-        with stream:
-            value = stream.read().decode("utf-8")
-        results.add((name, value))
-    assert results == {
-        ("dog1", "woof"),
-        ("dog2", "arf"),
-        ("dog3", "bark"),
-        ("dog4", "ruff"),
-    }
-
-
-@pytest.mark.parametrize("use_cache", [False, True])
-@pytest.mark.parametrize("cloud_type,version_aware", [("file", False)], indirect=True)
-def test_to_pytorch_from_path(cloud_test_catalog, use_cache):
-    from torch.utils.data import IterableDataset
-
-    ctc = cloud_test_catalog
-    q = DatasetQuery(path=ctc.src_uri, catalog=ctc.catalog).filter(C.name.glob("dog*"))
-    results = set()
-    pt_dataset = q.to_pytorch("name", Stream(), cache=use_cache)
-    assert isinstance(pt_dataset, IterableDataset)
-    for name, stream in pt_dataset:
-        with stream:
-            value = stream.read().decode("utf-8")
-        results.add((name, value))
-    assert results == {
-        ("dog1", "woof"),
-        ("dog2", "arf"),
-        ("dog3", "bark"),
-        ("dog4", "ruff"),
-    }
-
-
 @pytest.mark.parametrize("method", ["to_records", "extract"])
 @pytest.mark.parametrize("save", [True, False])
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
     [("s3", True)],
     indirect=True,
 )
```

### Comparing `dvcx-0.76.0/tests/func/test_datasets.py` & `dvcx-0.77.0/tests/func/test_datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 from json import dumps
-from unittest.mock import ANY, patch
+from unittest.mock import ANY
 
 import pytest
 import sqlalchemy as sa
 from dateutil.parser import isoparse
 
 from dvcx.catalog.catalog import DATASET_INTERNAL_ERROR_MESSAGE
 from dvcx.dataset import DatasetDependencyType
@@ -69,21 +69,20 @@
     dataset_version = dataset.get_version(1)
 
     assert dataset.name == name
     assert dataset.query_script == "script"
     assert dataset_version.query_script == "script"
     assert dataset.custom_column_types["similarity"] == Float32
     assert dataset_version.custom_column_types["similarity"] == Float32
-    dataset_table_name = catalog.warehouse.dataset_table_name(name, 1)
     assert dataset_version.status == DatasetStatus.PENDING
     assert dataset.status == DatasetStatus.CREATED  # dataset status is deprecated
     if create_rows:
-        assert get_table_row_count(catalog.warehouse.db, dataset_table_name) == 0
+        assert dataset_version.num_objects == 0
     else:
-        assert get_table_row_count(catalog.warehouse.db, dataset_table_name) is None
+        assert dataset_version.num_objects is None
 
 
 @pytest.mark.parametrize("create_rows", [True, False])
 def test_create_dataset_with_explicit_version(cloud_test_catalog, create_rows):
     catalog = cloud_test_catalog.catalog
 
     name = uuid.uuid4().hex
@@ -100,21 +99,20 @@
     dataset_version = dataset.get_version(1)
 
     assert dataset.name == name
     assert dataset.query_script == "script"
     assert dataset_version.query_script == "script"
     assert dataset.custom_column_types["similarity"] == Float32
     assert dataset_version.custom_column_types["similarity"] == Float32
-    dataset_table_name = catalog.warehouse.dataset_table_name(name, 1)
     assert dataset_version.status == DatasetStatus.PENDING
     assert dataset.status == DatasetStatus.CREATED
     if create_rows:
-        assert get_table_row_count(catalog.warehouse.db, dataset_table_name) == 0
+        assert dataset_version.num_objects == 0
     else:
-        assert get_table_row_count(catalog.warehouse.db, dataset_table_name) is None
+        assert dataset_version.num_objects is None
 
 
 @pytest.mark.parametrize("create_rows", [True, False])
 def test_create_dataset_already_exist(cloud_test_catalog, dogs_dataset, create_rows):
     catalog = cloud_test_catalog.catalog
 
     dataset = catalog.create_dataset(
@@ -127,21 +125,20 @@
     assert dataset.versions_values == [1, 2]
 
     dataset_version = dataset.get_version(2)
 
     assert dataset.name == dogs_dataset.name
     assert dataset_version.query_script == "script"
     assert dataset_version.custom_column_types["similarity"] == Float32
-    dataset_table_name = catalog.warehouse.dataset_table_name(dogs_dataset.name, 2)
     assert dataset_version.status == DatasetStatus.PENDING
     assert dataset.status == DatasetStatus.COMPLETE
     if create_rows:
-        assert get_table_row_count(catalog.warehouse.db, dataset_table_name) == 0
+        assert dataset_version.num_objects == 0
     else:
-        assert get_table_row_count(catalog.warehouse.db, dataset_table_name) is None
+        assert dataset_version.num_objects is None
 
 
 @pytest.mark.parametrize("create_rows", [True, False])
 def test_create_dataset_already_exist_wrong_version(
     cloud_test_catalog, dogs_dataset, create_rows
 ):
     catalog = cloud_test_catalog.catalog
@@ -207,42 +204,40 @@
     }
 
     assert dataset.custom_column_types == default_dataset_custom_column_types
     assert dataset.query_script == ""
 
     assert dataset_version.custom_column_types == default_dataset_custom_column_types
     assert dataset_version.query_script == ""
-
-    dataset_table_name = catalog.warehouse.dataset_table_name(dataset.name, 1)
-    assert get_table_row_count(catalog.warehouse.db, dataset_table_name)
+    assert dataset_version.num_objects
 
 
 def test_create_dataset_from_sources_empty_sources(cloud_test_catalog):
     dataset_name = uuid.uuid4().hex
     catalog = cloud_test_catalog.catalog
 
     with pytest.raises(ValueError) as exc_info:
         catalog.create_dataset_from_sources(dataset_name, [], recursive=True)
 
     assert str(exc_info.value) == "Sources needs to be non empty list"
 
 
-def test_create_dataset_from_sources_failed(listed_bucket, cloud_test_catalog):
+def test_create_dataset_from_sources_failed(listed_bucket, cloud_test_catalog, mocker):
     dataset_name = uuid.uuid4().hex
     src_uri = cloud_test_catalog.src_uri
     catalog = cloud_test_catalog.catalog
-    with patch.object(
+    mocker.patch.object(
         catalog.warehouse.__class__,
-        "dataset_rows",
+        "create_dataset_rows_table",
         side_effect=RuntimeError("Error"),
-    ) as _:
-        with pytest.raises(RuntimeError):
-            catalog.create_dataset_from_sources(
-                dataset_name, [f"{src_uri}/dogs/*"], recursive=True
-            )
+    )
+    with pytest.raises(RuntimeError):
+        catalog.create_dataset_from_sources(
+            dataset_name, [f"{src_uri}/dogs/*"], recursive=True
+        )
     dataset = catalog.get_dataset(dataset_name)
     dataset_version = dataset.get_version(dataset.latest_version)
 
     assert dataset.name == dataset_name
     assert dataset.status == DatasetStatus.FAILED
     assert dataset.versions_values == [1]
     assert dataset.created_at
@@ -253,19 +248,16 @@
 
     assert dataset_version.status == DatasetStatus.FAILED
     assert dataset_version.created_at
     assert dataset_version.finished_at
     assert dataset_version.error_message == DATASET_INTERNAL_ERROR_MESSAGE
     assert dataset_version.error_stack
     assert dataset_version.sources == f"{src_uri}/dogs/*"
-
-    dataset_table_name = catalog.warehouse.dataset_table_name(
-        dataset.name, dataset.latest_version
-    )
-    assert get_table_row_count(catalog.warehouse.db, dataset_table_name) == 0
+    assert dataset_version.num_objects is None
+    assert dataset_version.size is None
 
 
 def test_create_dataset_whole_bucket(listed_bucket, cloud_test_catalog):
     dataset_name_1 = uuid.uuid4().hex
     dataset_name_2 = uuid.uuid4().hex
     src_uri = cloud_test_catalog.src_uri
     catalog = cloud_test_catalog.catalog
@@ -337,14 +329,18 @@
     assert version2.query_script == "DatasetQuery()"
     assert version2.error_message == "no error"
     assert version2.error_stack == "no error stack"
     assert version2.script_output == "log"
     assert version2.custom_column_types == dogs_version.custom_column_types
     assert version2.created_at == dogs_version.created_at
     assert version2.finished_at == dogs_version.finished_at
+    assert dogs_version.num_objects
+    assert version2.num_objects == dogs_version.num_objects
+    assert dogs_version.size
+    assert version2.size == dogs_version.size
 
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, 1)} == {
         "cat1",
         "cat2",
     }
 
     assert {r.name for r in catalog.ls_dataset_rows(dataset.name, target_version)} == {
@@ -392,16 +388,16 @@
         "dog3",
         "dog4",
     }
 
     # check if dogs dataset is still present as it has one more version
     dogs_dataset = catalog.get_dataset(dogs_dataset.name)
     assert dogs_dataset.versions_values == [2]
-    dataset_table_name = catalog.warehouse.dataset_table_name(dogs_dataset.name, 2)
-    assert get_table_row_count(catalog.warehouse.db, dataset_table_name) == 0
+    dataset_version = dogs_dataset.get_version(2)
+    assert dataset_version.num_objects == 0
 
 
 @pytest.mark.parametrize("target_version", [None, 3])
 def test_registering_dataset_with_new_version_of_itself(
     cloud_test_catalog, cats_dataset, target_version
 ):
     catalog = cloud_test_catalog.catalog
@@ -479,21 +475,22 @@
         "Cannot register dataset version in non final status"
     )
 
 
 def test_remove_dataset(cloud_test_catalog, dogs_dataset):
     catalog = cloud_test_catalog.catalog
 
-    dataset_table_name = catalog.warehouse.dataset_table_name(dogs_dataset.name, 1)
-    assert get_table_row_count(catalog.warehouse.db, dataset_table_name)
+    dataset_version = dogs_dataset.get_version(1)
+    assert dataset_version.num_objects
 
     catalog.remove_dataset(dogs_dataset.name, force=True)
     with pytest.raises(DatasetNotFoundError):
         catalog.get_dataset(dogs_dataset.name)
 
+    dataset_table_name = catalog.warehouse.dataset_table_name(dogs_dataset.name, 1)
     assert get_table_row_count(catalog.warehouse.db, dataset_table_name) is None
 
     assert catalog.metastore.get_direct_dataset_dependencies(dogs_dataset, 1) == []
 
 
 def test_remove_dataset_dataset_not_found(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
@@ -527,15 +524,19 @@
     assert dataset.description == "new description"
     assert dataset.labels == ["cats", "birds"]
 
     # check if dataset tables are renamed correctly
     old_dataset_table_name = catalog.warehouse.dataset_table_name(dataset_old_name, 1)
     new_dataset_table_name = catalog.warehouse.dataset_table_name(dataset_new_name, 1)
     assert get_table_row_count(catalog.warehouse.db, old_dataset_table_name) is None
-    assert get_table_row_count(catalog.warehouse.db, new_dataset_table_name)
+    expected_table_row_count = get_table_row_count(
+        catalog.warehouse.db, new_dataset_table_name
+    )
+    assert expected_table_row_count
+    assert dataset.get_version(1).num_objects == expected_table_row_count
 
 
 def test_edit_dataset_same_name(cloud_test_catalog, dogs_dataset):
     dataset_old_name = dogs_dataset.name
     dataset_new_name = dogs_dataset.name
     catalog = cloud_test_catalog.catalog
 
@@ -543,16 +544,22 @@
 
     dataset = catalog.get_dataset(dataset_new_name)
     assert dataset.name == dataset_new_name
 
     # check if dataset tables are renamed correctly
     old_dataset_table_name = catalog.warehouse.dataset_table_name(dataset_old_name, 1)
     new_dataset_table_name = catalog.warehouse.dataset_table_name(dataset_new_name, 1)
-    assert get_table_row_count(catalog.warehouse.db, old_dataset_table_name)
-    assert get_table_row_count(catalog.warehouse.db, new_dataset_table_name)
+    expected_table_row_count = get_table_row_count(
+        catalog.warehouse.db, old_dataset_table_name
+    )
+    assert expected_table_row_count
+    assert dataset.get_version(1).num_objects == expected_table_row_count
+    assert expected_table_row_count == get_table_row_count(
+        catalog.warehouse.db, new_dataset_table_name
+    )
 
 
 def test_edit_dataset_remove_labels_and_description(cloud_test_catalog, dogs_dataset):
     dataset_new_name = uuid.uuid4().hex
     catalog = cloud_test_catalog.catalog
 
     catalog.edit_dataset(
@@ -763,14 +770,40 @@
 
     cats_dep = catalog.get_dataset_dependencies(cats_custom_column.name, 1)
     dogs_dep = catalog.get_dataset_dependencies(dogs_dataset.name, 2)
 
     assert set(dogs_dep) == set(cats_dep)
 
 
+def test_merge_datasets_size(cloud_test_catalog, dogs_dataset, cats_dataset):
+    catalog = cloud_test_catalog.catalog
+    catalog.merge_datasets(
+        cats_dataset,
+        dogs_dataset,
+        1,
+        dst_version=2,
+    )
+
+    dogs_dataset = catalog.get_dataset(dogs_dataset.name)
+    assert dogs_dataset.versions_values == [1, 2]
+
+    dogs_version_1 = dogs_dataset.get_version(1)
+    dogs_version_2 = dogs_dataset.get_version(2)
+    cats_version_1 = cats_dataset.get_version(1)
+
+    assert dogs_version_2.size
+    assert dogs_version_2.size == dogs_version_1.size + cats_version_1.size
+
+    assert dogs_version_2.num_objects
+    assert (
+        dogs_version_2.num_objects
+        == dogs_version_1.num_objects + cats_version_1.num_objects
+    )
+
+
 @pytest.mark.parametrize("tree", [{str(i): str(i) for i in range(50)}], indirect=True)
 def test_row_random(cloud_test_catalog):
     # Note: this is technically a probabilistic test, but the probability
     # of accidental failure is < 1e-10
     ctc = cloud_test_catalog
     catalog = ctc.catalog
     catalog.index([ctc.src_uri])
```

### Comparing `dvcx-0.76.0/tests/func/test_ls.py` & `dvcx-0.77.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/func/test_pull.py` & `dvcx-0.77.0/tests/func/test_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,16 @@
         "dataset_id": 1,
         "version": 1,
         "status": 4,
         "created_at": "2024-02-23T10:42:31.842944+00:00",
         "finished_at": "2024-02-23T10:43:31.842944+00:00",
         "error_message": "",
         "error_stack": "",
+        "num_objects": 5,
+        "size": 1073741824,
         "script_output": "",
         "custom_column_types": custom_column_types,
         "sources": "",
         "query_script": (
             'from dvcx.query import DatasetQuery\nDatasetQuery(path="s3://ldb-public)',
         ),
         "created_by_id": 1,
@@ -176,14 +178,16 @@
     assert dataset.finished_at
     assert dataset.custom_column_types
     dataset_version = dataset.get_version(1)
     assert dataset_version.status == DatasetStatus.COMPLETE
     assert dataset_version.created_at
     assert dataset_version.finished_at
     assert dataset_version.custom_column_types
+    assert dataset_version.num_objects == 4
+    assert dataset_version.size == 15
 
     expected_rows = {
         "dog1",
         "dog2",
         "dog3",
         "dog4",
     }
```

### Comparing `dvcx-0.76.0/tests/func/test_pytorch.py` & `dvcx-0.77.0/tests/func/test_pytorch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 from torch import Size, Tensor
 from torchvision.datasets import FakeData
 from torchvision.transforms import v2
 
 from dvcx.catalog import get_catalog
-from dvcx.lib.param import Image
+from dvcx.lib.dataset import Dataset
+from dvcx.lib.image import ImageFile
 from dvcx.lib.pytorch import PytorchDataset
-from dvcx.query import DatasetQuery, udf
 from dvcx.sql.types import Int
 
 
 @pytest.fixture
 def fake_dataset(tmp_path):
     # Create fake images in labeled dirs
     data_path = tmp_path / "data"
@@ -20,41 +20,56 @@
         img.save(data_path / label / f"{i}.jpg")
 
     # Create dataset from images
     uri = data_path.as_uri()
     catalog = get_catalog()
     catalog.add_storage(uri)
 
-    @udf(params=("parent",), output={"label": Int})
     def extract_label(parent):
         return (int(parent),)
 
-    yield DatasetQuery(uri).add_signals(extract_label).save("fake")
+    yield (
+        Dataset(uri)
+        .map(extract_label, params=("parent",), output={"label": Int})
+        .save("fake")
+    )
 
     catalog.remove_dataset("fake", version=1)
     catalog.id_generator.cleanup_for_tests()
 
 
-def test_pytorch_dataset(tmp_path, fake_dataset):
+def test_pytorch_dataset(fake_dataset):
     transform = v2.Compose([v2.ToTensor(), v2.Resize((64, 64))])
     pt_dataset = PytorchDataset(
-        params=[Image(), "label"],
+        fr_classes=[ImageFile, "label"],
         name=fake_dataset.name,
         version=fake_dataset.version,
         transform=transform,
     )
     for img, label in pt_dataset:
         assert isinstance(img, Tensor)
         assert isinstance(label, int)
         assert img.size() == Size([3, 64, 64])
 
 
-def test_pytorch_dataset_sample(tmp_path, fake_dataset):
+def test_pytorch_dataset_sample(fake_dataset):
     transform = v2.Compose([v2.ToTensor(), v2.Resize((64, 64))])
     pt_dataset = PytorchDataset(
-        params=[Image(), "label"],
+        fr_classes=[ImageFile, "label"],
         name=fake_dataset.name,
         version=fake_dataset.version,
         transform=transform,
         num_samples=700,
     )
     assert len(list(pt_dataset)) == 700
+
+
+def test_to_pytorch(fake_dataset):
+    from torch.utils.data import IterableDataset
+
+    transform = v2.Compose([v2.ToTensor(), v2.Resize((64, 64))])
+    pt_dataset = fake_dataset.to_pytorch(ImageFile, "label", transform=transform)
+    assert isinstance(pt_dataset, IterableDataset)
+    for img, label in pt_dataset:
+        assert isinstance(img, Tensor)
+        assert isinstance(label, int)
+        assert img.size() == Size([3, 64, 64])
```

### Comparing `dvcx-0.76.0/tests/func/test_query.py` & `dvcx-0.77.0/tests/func/test_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,14 +108,42 @@
         "dog1",
         "dog2",
         "dog3",
         "dog4",
     }
 
 
+@pytest.mark.parametrize(
+    "params,count",
+    (
+        (None, 7),
+        ({"limit": 1}, 1),
+        ({"limit": 5}, 5),
+    ),
+)
+def test_query_params(
+    params, count, cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath
+):
+    catalog = cloud_test_catalog_tmpfile.catalog
+    src_uri = cloud_test_catalog_tmpfile.src_uri
+
+    query_script = f"""\
+    from dvcx.query import C, DatasetQuery, param
+
+    ds = DatasetQuery({src_uri!r}, catalog=catalog)
+    if param("limit"):
+        ds = ds.limit(int(param("limit")))
+    ds
+    """
+    query_script = setup_catalog(query_script, catalog_info_filepath)
+
+    dataset, version, output, _ = catalog.query(query_script, save=True, params=params)
+    assert len(list(catalog.ls_dataset_rows(dataset.name, version))) == count
+
+
 def test_query_where_last_command_is_call_on_save_which_returns_attached_dataset(
     cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath
 ):
     """
     Testing use case where last command is call on DatasetQuery save which returns
     attached instance to underlying saved dataset
     """
@@ -187,15 +215,15 @@
 
     query_script = f"""\
     from dvcx.query import C, DatasetQuery
 
     ds = DatasetQuery(
         {src_uri!r}, catalog=catalog
     ).filter(C.name.glob("dog*")).save("dogs")
-    DatasetQuery(name="dogs", version=1)
+    DatasetQuery(name="dogs", version=1, catalog=catalog)
     """
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
     dataset, version, output, _ = catalog.query(query_script, save=True)
     assert dataset.name == "dogs"
     assert dataset.query_script == query_script
     assert version == 1
```

### Comparing `dvcx-0.76.0/tests/test_cli_e2e.py` & `dvcx-0.77.0/tests/test_cli_e2e.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,14 +208,18 @@
         "command": ("dvcx", "rm-dataset", "mnt-new", "--version", "1"),
         "expected": "",
     },
     {
         "command": ("dvcx", "ls-datasets"),
         "expected": "",
     },
+    {
+        "command": ("dvcx", "gc"),
+        "expected": "Nothing to clean up.\n",
+    },
 )
 
 
 def verify_files(files, base=""):
     """Recursively validate file and directory structure."""
     for name, value in files.items():
         full_name = os.path.join(base, name)
```

### Comparing `dvcx-0.76.0/tests/unit/lib/test_cached_stream.py` & `dvcx-0.77.0/tests/unit/lib/test_cached_stream.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,16 @@
 import io
 
-import pytest
-
-from dvcx.catalog import Catalog
-from dvcx.catalog.loader import get_id_generator, get_metastore, get_warehouse
 from dvcx.lib.cached_stream import ProgressiveCacheStream
 from dvcx.lib.file import File
 
 DATA = b"qwertyuiop"
 FILE_UID = File(name="name").get_uid()
 
 
-@pytest.fixture
-def catalog(tmp_path):
-    id_generator = get_id_generator()
-    return Catalog(
-        id_generator,
-        get_metastore(id_generator),
-        get_warehouse(id_generator),
-        str(tmp_path / "cache"),
-        str(tmp_path / "tmp"),
-    )
-
-
 def test_close(catalog):
     input = io.BytesIO()
     input.write(DATA)
     input.seek(0)
 
     with ProgressiveCacheStream(input, len(DATA), catalog, FILE_UID) as stream:
         stream.close()
```

### Comparing `dvcx-0.76.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.77.0/tests/unit/lib/test_feature_udf.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pytest
 from pydantic import Field
 
 from dvcx.lib.feature import Feature
 from dvcx.lib.feature_udf import (
     FeatureAggregator,
     FeatureBatchMapper,
+    FeatureConverter,
     FeatureGenerator,
     FeatureMapper,
     OutputError,
     SchemaError,
     UserCodeError,
 )
 from dvcx.lib.file import File
@@ -369,7 +370,27 @@
     path = "dir1/dir2"
     size = 16
     params = (name, path, size)
 
     agg = MyBuggyClass()
     with pytest.raises(UserCodeError):
         list(agg(*params))
+
+
+def test_split():
+    features = [File]
+    f1 = File(name="abc")._flatten()
+    f2 = File(name="zxc")._flatten()
+
+    rows = [f1, f2]
+    clean_rows, streams = FeatureConverter._separate_streams_from_rows(rows, features)
+    assert clean_rows == rows
+    assert streams == [None, None]
+
+    rows_with_streams = [(Stream(),) + f1, (Stream(),) + f2]
+    clean_rows, streams = FeatureConverter._separate_streams_from_rows(
+        rows_with_streams, features
+    )
+    assert clean_rows == rows
+    assert len(streams) == 2
+    assert isinstance(streams[0], Stream)
+    assert isinstance(streams[1], Stream)
```

### Comparing `dvcx-0.76.0/tests/unit/lib/test_webdataset.py` & `dvcx-0.77.0/tests/unit/lib/test_webdataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,38 +35,43 @@
             def read(self):
                 return tar_info._content
 
         return TmpReader()
 
 
 def test_webdataset_basic():
-    stream = File(name="nnn.tar")
+    tar_file = File(name="nnn.tar")
     tar = MockTar(
         [
             MockTarInfo("01.jpg"),
             MockTarInfo("01.json", b'{"uid": "5678"}'),
             MockTarInfo("64.jpg"),
             MockTarInfo("64.json", b"{}"),
         ]
     )
 
-    groups = list(WebDataset().get_tar_groups(stream, tar, ["jpg"], WDSLaion))
+    groups = list(WebDataset().get_tar_groups(tar_file, tar, ["jpg"], WDSLaion))
 
     assert len(groups) == 2
 
     (file01, laion01), (file64, laion64) = groups
 
     assert file01.name == "01.jpg"
-    assert file01.parent == stream.name
+    assert file01.parent == tar_file.name
     assert file01.location is not None
     assert isinstance(file01.location, list)
-    assert file01.location[0]["parent"] == stream.name
+    assert len(file01.location) > 0
+
+    parent = file01.location[0].get("parent", None)
+    assert parent is not None
+    parent_file = File(**parent)
+    assert parent_file == tar_file
 
     assert file64.name == "64.jpg"
-    assert file64.parent == stream.name
+    assert file64.parent == tar_file.name
 
     assert laion01.txt is None
     assert laion01.json.uid == "5678"
 
     assert laion64.json.uid == ""
```

### Comparing `dvcx-0.76.0/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.77.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/sql/test_array.py` & `dvcx-0.77.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/sql/test_conditional.py` & `dvcx-0.77.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/sql/test_path.py` & `dvcx-0.77.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/sql/test_selectable.py` & `dvcx-0.77.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/sql/test_string.py` & `dvcx-0.77.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_asyn.py` & `dvcx-0.77.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_cache.py` & `dvcx-0.77.0/tests/unit/test_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,7 +39,18 @@
         cache.store_data(uid, data)
     total = cache.get_total_size()
     assert total == expected_total
 
     cache.clear()
     empty_total = cache.get_total_size()
     assert empty_total == 0
+
+
+def test_remove(cache):
+    uid = UniqueId(
+        "s3://bkt42", "dir1/dir2", "file84", etag="abc", size=3, vtype="", location=None
+    )
+    cache.store_data(uid, b"some random string 679")
+
+    assert cache.contains(uid)
+    cache.remove(uid)
+    assert not cache.contains(uid)
```

### Comparing `dvcx-0.76.0/tests/unit/test_catalog.py` & `dvcx-0.77.0/tests/unit/test_catalog.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,31 +9,12 @@
         """
     ).strip()
     result = catalog.compile_query_script(script)
     expected = dedent(
         """
         from dvcx.query import C, DatasetQuery, asUDF
         import dvcx.query.dataset
-        dvcx.query.dataset.query_wrapper_print(
-        DatasetQuery('s3://bkt/dir1'))
-        """
-    ).strip()
-    assert result == expected
-
-
-def test_compile_query_script_with_save(cloud_test_catalog):
-    script = dedent(
-        """
-        from dvcx.query import C, DatasetQuery, asUDF
-        DatasetQuery("s3://bkt/dir1")
-        """
-    ).strip()
-    result = cloud_test_catalog.catalog.compile_query_script(script, save=True)
-    expected = dedent(
-        """
-        from dvcx.query import C, DatasetQuery, asUDF
-        import dvcx.query.dataset
-        dvcx.query.dataset.query_wrapper_save(
+        dvcx.query.dataset.query_wrapper(
         DatasetQuery('s3://bkt/dir1'))
         """
     ).strip()
     assert result == expected
```

### Comparing `dvcx-0.76.0/tests/unit/test_catalog_formats.py` & `dvcx-0.77.0/tests/unit/test_catalog_formats.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_catalog_loader.py` & `dvcx-0.77.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_client.py` & `dvcx-0.77.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_client_s3.py` & `dvcx-0.77.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_data_storage.py` & `dvcx-0.77.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_database_engine.py` & `dvcx-0.77.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_dataset.py` & `dvcx-0.77.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_fileslice.py` & `dvcx-0.77.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_id_generator.py` & `dvcx-0.77.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_listing.py` & `dvcx-0.77.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_metastore.py` & `dvcx-0.77.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_serializer.py` & `dvcx-0.77.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_storage.py` & `dvcx-0.77.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_udf.py` & `dvcx-0.77.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/unit/test_utils.py` & `dvcx-0.77.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.76.0/tests/utils.py` & `dvcx-0.77.0/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import dataclasses
 import io
 import math
 import os
 import tarfile
 from string import printable
 from tarfile import DIRTYPE, TarInfo
-from typing import Any, Optional
+from time import sleep, time
+from typing import Any, Callable, Optional
 
 import pytest
 
 from dvcx.dataset import DatasetDependency
 from dvcx.node import Entry
 from dvcx.query import C, DatasetQuery
 from dvcx.storage import Status as StorageStatus
@@ -254,7 +255,22 @@
 
     if dep.dependencies:
         parsed["dependencies"] = [
             dataset_dependency_asdict(d) for d in dep.dependencies
         ]
 
     return parsed
+
+
+def wait_for_condition(
+    callback: Callable,
+    message: str,
+    check_interval: float = 0.01,
+    timeout: float = 1.0,
+) -> Any:
+    start_time = time()
+    while time() - start_time < timeout:
+        result = callback()
+        if result:
+            return result
+        sleep(check_interval)
+    raise TimeoutError(f"Timeout expired while waiting for: {message}")
```


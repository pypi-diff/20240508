# Comparing `tmp/weaviate-client-4.5rc0.tar.gz` & `tmp/weaviate_client-4.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaviate-client-4.5rc0.tar", last modified: Fri Feb 23 14:54:14 2024, max compression
+gzip compressed data, was "weaviate_client-4.6.0b0.tar", last modified: Tue May  7 02:24:12 2024, max compression
```

## Comparing `weaviate-client-4.5rc0.tar` & `weaviate_client-4.6.0b0.tar`

### file list

```diff
@@ -1,405 +1,425 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.341352 weaviate-client-4.5rc0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.341352 weaviate-client-4.5rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.341352 weaviate-client-4.5rc0/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-async.yml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-azure.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-cluster.yml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-generative.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-okta-cc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-okta-users.yml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-rerank.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose-wcs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/start_weaviate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      687 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/ci/stop_weaviate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.349352 weaviate-client-4.5rc0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    52716 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.backup.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.classification.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.client.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.cluster.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.aggregations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.classes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.grpc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.collections.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.connect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.contextionary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.data.references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.data.replication.rst
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.gql.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.proto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.proto.v1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.schema.properties.rst
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/docs/weaviate.util.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.353352 weaviate-client-4.5rc0/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/1234.3gp
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/hobbits.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    18861 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_batch_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    17603 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    75458 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    25941 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_multi_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    20956 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_collection_rerank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_gql_raw_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/test_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration/weaviate-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.357352 weaviate-client-4.5rc0/integration_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/people_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_backup_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    20523 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_grcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/integration_v3/test_timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.357352 weaviate-client-4.5rc0/mock_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_automatic_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_batching_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_resend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/mock_tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/test_import_and_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/test_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/profiling/test_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/publishing.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/run-mypy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/test/batch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/batch/test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/test/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/classification/test_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.361352 weaviate-client-4.5rc0/test/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/cluster/test_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/collection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    32370 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/collection/test_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/connection/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/contextionary/test_text2vec_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/data/references/test_crud_references.py
--rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/data/test_crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/gql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/gql/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.365352 weaviate-client-4.5rc0/test/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/properties/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/schema_company.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/tenants.json
--rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/schema/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_server_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/test/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.369352 weaviate-client-4.5rc0/weaviate/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.369352 weaviate-client-4.5rc0/weaviate/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23819 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/backup/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.369352 weaviate-client-4.5rc0/weaviate/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74355 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/batch/crud_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/batch/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.369352 weaviate-client-4.5rc0/weaviate/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classes/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.373352 weaviate-client-4.5rc0/weaviate/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/classification/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22034 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.373352 weaviate-client-4.5rc0/weaviate/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/cluster/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.373352 weaviate-client-4.5rc0/weaviate/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.377352 weaviate-client-4.5rc0/weaviate/collections/aggregations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14951 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/near_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/near_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/near_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/near_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/aggregations/over_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.377352 weaviate-client-4.5rc0/weaviate/collections/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24333 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/batch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/grpc_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/grpc_batch_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/batch/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    63226 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    30800 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_vector_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    31703 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/config_vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    20454 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19035 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/classes/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15417 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26191 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/grpc/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/grpc/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22611 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/bm25/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.381352 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_image/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_media/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_object/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.385352 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_text/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/collections/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/connect/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    25530 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/connect/v4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/contextionary/crud_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/data/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/references/crud_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.389352 weaviate-client-4.5rc0/weaviate/data/replication/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/data/replication/replication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/error_msgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.393352 weaviate-client-4.5rc0/weaviate/gql/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39101 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/multi_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/gql/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.393352 weaviate-client-4.5rc0/weaviate/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/outputs/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.393352 weaviate-client-4.5rc0/weaviate/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/weaviate/proto/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/properties_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/properties_pb2_grpc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/regen.sh
--rw-r--r--   0 runner    (1001) docker     (127)    17865 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/weaviate/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/schema/crud_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/weaviate/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/schema/properties/crud_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    27997 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-02-23 14:53:46.000000 weaviate-client-4.5rc0/weaviate/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 14:54:14.397352 weaviate-client-4.5rc0/weaviate_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-23 14:54:14.000000 weaviate-client-4.5rc0/weaviate_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.791950 weaviate_client-4.6.0b0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.791950 weaviate_client-4.6.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.795950 weaviate_client-4.6.0b0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/compose.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-async.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-azure.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-generative.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-okta-cc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-okta-users.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-proxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-rerank.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-wcs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.795950 weaviate_client-4.6.0b0/ci/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/proxy/envoy.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      922 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/start_weaviate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/stop_weaviate.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.799950 weaviate_client-4.6.0b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    56116 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.backup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.classification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.aggregations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.classes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.grpc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.connect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.contextionary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.data.references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.data.replication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.gql.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.proto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.proto.v1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.schema.properties.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.util.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.803950 weaviate_client-4.6.0b0/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/1234.3gp
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/hobbits.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_batch_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78466 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31180 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33149 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_multi_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_gql_raw_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/weaviate-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.803950 weaviate_client-4.6.0b0/integration_embedded/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_embedded/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.807950 weaviate_client-4.6.0b0/integration_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/people_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_backup_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_grcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.807950 weaviate_client-4.6.0b0/mock_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_automatic_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_batching_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_resend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/test_import_and_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/test_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/test_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/publishing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/run-mypy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/batch/test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/classification/test_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/cluster/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_byteops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36501 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/connection/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/contextionary/test_text2vec_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/data/references/test_crud_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/data/test_crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/properties/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/schema_company.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/tenants.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_server_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/backup/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/batch/crud_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/batch/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classification/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22119 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/cluster/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.823950 weaviate_client-4.6.0b0/weaviate/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.823950 weaviate_client-4.6.0b0/weaviate/collections/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/over_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.827950 weaviate_client-4.6.0b0/weaviate/collections/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27772 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/batch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/grpc_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/grpc_batch_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.827950 weaviate_client-4.6.0b0/weaviate/collections/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69063 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38971 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_vector_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39194 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19528 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.827950 weaviate_client-4.6.0b0/weaviate/collections/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28802 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/grpc/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/grpc/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/grpc/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/byteops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/v4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/contextionary/crud_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/references/crud_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/data/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/replication/replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/error_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42084 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/multi_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.843950 weaviate_client-4.6.0b0/weaviate/proto/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/properties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/properties_pb2_grpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/regen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/tenants_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/tenants_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/tenants_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.843950 weaviate_client-4.6.0b0/weaviate/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/schema/crud_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/weaviate/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/schema/properties/crud_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/weaviate_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/top_level.txt
```

### Comparing `weaviate-client-4.5rc0/.github/workflows/main.yaml` & `weaviate_client-4.6.0b0/.github/workflows/main.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -10,16 +10,18 @@
       - docs/**
       - README.rst
       - LICENSE.md
       - publishing.md
   pull_request:
 
 env:
-  OLD_WEAVIATE_VERSION: 1.23.10
-  NEW_WEAVIATE_VERSION: 1.24.0-rc.1
+  WEAVIATE_123: 1.23.14
+  WEAVIATE_124: 1.24.10
+  WEAVIATE_125: preview-remove-consistency-from-tenant-get-486f1a6
+
 
 jobs:
   lint-and-format:
     name: Run Linter and Formatter
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
@@ -79,29 +81,58 @@
       - name: Archive code coverage results
         if: matrix.version == '3.10' && (github.ref_name != 'main')
         uses: actions/upload-artifact@v4
         with:
           name: coverage-report-${{ matrix.folder }}
           path: coverage-${{ matrix.folder }}.xml
 
+  integration-tests-embedded:
+    name: Run Integration Tests Embedded
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        optional_dependencies: [false]
+    steps:
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+          fetch-tags: true
+      - uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.version }}
+          cache: 'pip' # caching pip dependencies
+      - run: |
+          pip install -r requirements-devel.txt
+          pip install .
+      - name: Run integration tests
+        if: ${{ !github.event.pull_request.head.repo.fork }}
+        run: pytest -v --cov --cov-report=term-missing --cov=weaviate --cov-report xml:coverage-integration-embedded.xml integration_embedded
+      - name: Archive code coverage results
+        if: matrix.version == '3.10' && (github.ref_name != 'main')
+        uses: actions/upload-artifact@v4
+        with:
+          name: coverage-report-integration-embedded
+          path: coverage-integration-embedded.xml
+
   integration-tests-v3:
     name: Run Integration Tests v3
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         versions: [
-          { py: "3.8", weaviate: $NEW_WEAVIATE_VERSION},
-          { py: "3.9", weaviate: $NEW_WEAVIATE_VERSION},
-          { py: "3.10", weaviate: $NEW_WEAVIATE_VERSION},
-          { py: "3.11", weaviate: $NEW_WEAVIATE_VERSION},
-          { py: "3.11", weaviate: $OLD_WEAVIATE_VERSION},
-          { py: "3.12", weaviate: $NEW_WEAVIATE_VERSION}
+          { py: "3.8", weaviate: $WEAVIATE_125},
+          { py: "3.9", weaviate: $WEAVIATE_125},
+          { py: "3.10", weaviate: $WEAVIATE_125},
+          { py: "3.11", weaviate: $WEAVIATE_123},
+          { py: "3.11", weaviate: $WEAVIATE_124},
+          { py: "3.11", weaviate: $WEAVIATE_125},
+          { py: "3.12", weaviate: $WEAVIATE_125}
         ]
-
         optional_dependencies: [false]
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
           fetch-tags: true
       - uses: actions/setup-python@v5
@@ -137,22 +168,22 @@
   integration-tests:
     name: Run Integration Tests
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         versions: [
-          { py: "3.8", weaviate: $NEW_WEAVIATE_VERSION},
-          { py: "3.9", weaviate: $NEW_WEAVIATE_VERSION},
-          { py: "3.10", weaviate: $NEW_WEAVIATE_VERSION},
-          { py: "3.11", weaviate: $NEW_WEAVIATE_VERSION},
-          { py: "3.11", weaviate: $OLD_WEAVIATE_VERSION},
-          { py: "3.12", weaviate: $NEW_WEAVIATE_VERSION}
+          { py: "3.8", weaviate: $WEAVIATE_125},
+          { py: "3.9", weaviate: $WEAVIATE_125},
+          { py: "3.10", weaviate: $WEAVIATE_125},
+          { py: "3.11", weaviate: $WEAVIATE_123},
+          { py: "3.11", weaviate: $WEAVIATE_124},
+          { py: "3.11", weaviate: $WEAVIATE_125},
+          { py: "3.12", weaviate: $WEAVIATE_125}
         ]
-
         optional_dependencies: [false]
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
           fetch-tags: true
       - uses: actions/setup-python@v5
@@ -203,19 +234,23 @@
         uses: actions/download-artifact@v4
         with:
           name: coverage-report-integration
       - name: Download coverage integration v3
         uses: actions/download-artifact@v4
         with:
           name: coverage-report-integration-v3
+      - name: Download coverage integration embedded
+        uses: actions/download-artifact@v4
+        with:
+          name: coverage-report-integration-embedded
       - name: Codecov
         uses: codecov/codecov-action@v4
         with:
           fail_ci_if_error: true
-          files: ./coverage-integration.xml, ./coverage-integration-v3.xml, ./coverage-test.xml, ./coverage-mock_tests.xml
+          files: ./coverage-integration.xml, ./coverage-integration-v3.xml, ./coverage-integration-embedded.xml, ./coverage-test.xml, ./coverage-mock_tests.xml
           verbose: true
           token: ${{ secrets.CODECOV_TOKEN }}
 
 
   build-package:
     name: Build package
     runs-on: ubuntu-latest
@@ -243,16 +278,17 @@
   test-package:
     needs: [build-package]
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         server: [
-          $OLD_WEAVIATE_VERSION,
-          $NEW_WEAVIATE_VERSION,
+          $WEAVIATE_123,
+          $WEAVIATE_124,
+          $WEAVIATE_125
         ]
     steps:
       - name: Download build artifact to append to release
         uses: actions/download-artifact@v4
         with:
           name: weaviate-python-client-wheel
       - run: |
```

### Comparing `weaviate-client-4.5rc0/.pre-commit-config.yaml` & `weaviate_client-4.6.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/.pylintrc` & `weaviate_client-4.6.0b0/.pylintrc`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/CONTRIBUTING.md` & `weaviate_client-4.6.0b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/LICENSE` & `weaviate_client-4.6.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/PKG-INFO` & `weaviate_client-4.6.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.5rc0
+Version: 4.6.0b0
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
 Project-URL: Tracker, https://github.com/weaviate/weaviate-python-client/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 Requires-Dist: requests<3.0.0,>=2.30.0
-Requires-Dist: httpx==0.27.0
-Requires-Dist: validators==0.22.0
+Requires-Dist: httpx<=0.27.0,>=0.25.0
+Requires-Dist: validators==0.28.1
 Requires-Dist: authlib<2.0.0,>=1.2.1
 Requires-Dist: pydantic<3.0.0,>=2.5.0
 Requires-Dist: grpcio<2.0.0,>=1.57.0
 Requires-Dist: grpcio-tools<2.0.0,>=1.57.0
 Requires-Dist: grpcio-health-checking<2.0.0,>=1.57.0
 
 Weaviate python client
```

### Comparing `weaviate-client-4.5rc0/README.rst` & `weaviate_client-4.6.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/ci/docker-compose-async.yml` & `weaviate_client-4.6.0b0/ci/docker-compose-async.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
       - --port
       - '8090'
       - --scheme
       - http
     image: semitechnologies/weaviate:${WEAVIATE_VERSION}
     ports:
       - "8090:8090"
-      - "50060:50051"
+      - "50061:50051"
     restart: on-failure:0
     environment:
       QUERY_DEFAULTS_LIMIT: 25
       AUTHENTICATION_ANONYMOUS_ACCESS_ENABLED: 'true'
       PERSISTENCE_DATA_PATH: '/var/lib/weaviate'
       CLUSTER_HOSTNAME: 'node1'
       ASYNC_INDEXING: 'true'
```

### Comparing `weaviate-client-4.5rc0/ci/docker-compose-azure.yml` & `weaviate_client-4.6.0b0/ci/docker-compose-azure.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/ci/docker-compose-generative.yml` & `weaviate_client-4.6.0b0/ci/docker-compose-generative.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/ci/docker-compose-okta-cc.yml` & `weaviate_client-4.6.0b0/ci/docker-compose-okta-cc.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/ci/docker-compose-okta-users.yml` & `weaviate_client-4.6.0b0/ci/docker-compose-okta-users.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/ci/docker-compose-rerank.yml` & `weaviate_client-4.6.0b0/ci/docker-compose-rerank.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/ci/docker-compose-wcs.yml` & `weaviate_client-4.6.0b0/ci/docker-compose-wcs.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/ci/docker-compose.yml` & `weaviate_client-4.6.0b0/ci/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/Makefile` & `weaviate_client-4.6.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/README.rst` & `weaviate_client-4.6.0b0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/changelog.rst` & `weaviate_client-4.6.0b0/docs/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,87 @@
 Changelog
 =========
+Version 4.5.7
+--------------
+This patch version includes:
+
+- Deprecation of the ``bit_compression`` field in the ``PQConfig`` class
+- Improvements to closing possibly open objects and connections
+- Enhances the ``WeaviateGRPCUnavailableError`` message with added context relevant to the user's environment
+- Relaxes the ``httpx`` requirements to aid compatability with other packages
+
+
+Version 4.5.6
+--------------
+This patch version includes:
+
+- Support for configuring collections with the new ``reranker-voyageai`` module
+- Providing an ``alpha`` parameter to ``collection.iterator()`` to control the beginning of the iteration
+- Update the default ``Timeout.init`` value from ``1s`` to ``2s``
+
+Version 4.5.5
+--------------
+This patch version includes:
+
+- Bugfix when parsing the result from ``v1/nodes`` API with ``shards: null``
+- Bugfix when parsing the result from ``v1/schema`` API with ``class.properties.moduleConfig: null`` and ``class.vectoriser: !'none'``
+- Dependency bumps
+
+Version 4.5.4
+--------------
+This patch version includes:
+
+- Fix parsing of creation/update time from old weaviate versions that write them in ns instead of ms
+- Support ``video_fields`` in ``multi2vec-palm`` which was added in Weaviate 1.24.4:
+
+Version 4.5.3
+--------------
+This patch version includes:
+
+- Fix bug with hybrid searches without vector.
+- Support for new modules in Weaviate 1.24.2:
+  - ``text2vec-voyageai``
+  - ``generative-mistral``
+  - Support new parameters for interference URLs in ``text2vec-transformers`` and ``multi2vec-clip``
+- Support for new modules in Weaviate 1.24.3:
+  - ``multi2vec-palm``
+
+Version 4.5.2
+--------------
+This patch version includes:
+
+- Fixes endpoint parameter for ``text2vec-palm``
+- Adds support for GSE and TRIGRAM tokenizers
+
+Version 4.5.1
+--------------
+This patch version includes:
+
+- Implements an extension to the filtering syntax allowing to pass lists of filters
+    - ``Filter.all_of([f1, f2]])`` is a shortcut for ``f1 & f2``
+    - ``Filter.any_of([f1, f2]])`` is a shortcut for ``f1 | f2``
+    - Can all be chained and mixed together to create dynamic and complex filters
+- Introduces ``weaviate.classes.init.Timeout`` class allowing to define the timeout used when performing client init checks, in addition to connect and query
+- Fixes a bug when performing ``contains_any/contains_all`` filtering using an empty list
+- Adds the ability to limit the ``top_occurences`` return when performing aggregation queries
+- Allows for defining gRPC proxying of the client and fixes the parsing of ``http`` and ``https`` proxies
+- Allow ``None`` as a query value in BM25 and hybrid queries
+- Fix missing named vectors support in ``data.update`` and ``data.replace``
+- Reimplement support for updating named vector configurations alongside the patched ``1.24.1`` server version
+
+Version 4.5.0
+--------------
+This minor version includes:
+
+- Full support for the new named vectors feature available in the Weaviate ``1.24`` release.
+- Bugfixes to passing of Weaviate schema objects as collection configurations in certain edge cases.
+- Support use of Sagemaker when vectorizing with the ``text2vec-aws`` module.
+- Allow creation of collections that use the ``hnsw`` index with the ``bq`` quantizing strategy.
+- Allow specifying ``dimensions`` when vectorizing with the ``text2vec-openai`` module.
+- Python in-memory performance improvements when making queries .
 
 Version 4.4.4
 --------------
 This patch version includes:
 
 - A fix to the validation logic of the ``apiEndpoint`` field of ``GenerativePaLMConfig`` object.
```

### Comparing `weaviate-client-4.5rc0/docs/conf.py` & `weaviate_client-4.6.0b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/index.rst` & `weaviate_client-4.6.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/make.bat` & `weaviate_client-4.6.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.classification.rst` & `weaviate_client-4.6.0b0/docs/weaviate.classification.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.collections.aggregations.rst` & `weaviate_client-4.6.0b0/docs/weaviate.collections.aggregations.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.collections.batch.rst` & `weaviate_client-4.6.0b0/docs/weaviate.collections.batch.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.collections.classes.rst` & `weaviate_client-4.6.0b0/docs/weaviate.collections.classes.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.collections.grpc.rst` & `weaviate_client-4.6.0b0/docs/weaviate.collections.grpc.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.collections.queries.rst` & `weaviate_client-4.6.0b0/docs/weaviate.collections.queries.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.collections.rst` & `weaviate_client-4.6.0b0/docs/weaviate.collections.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.connect.rst` & `weaviate_client-4.6.0b0/docs/weaviate.connect.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.gql.rst` & `weaviate_client-4.6.0b0/docs/weaviate.gql.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.proto.v1.rst` & `weaviate_client-4.6.0b0/docs/weaviate.proto.v1.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/docs/weaviate.rst` & `weaviate_client-4.6.0b0/docs/weaviate.rst`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/1234.3gp` & `weaviate_client-4.6.0b0/integration/1234.3gp`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/conftest.py` & `weaviate_client-4.6.0b0/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/constants.py` & `weaviate_client-4.6.0b0/integration/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/hobbits.mp4` & `weaviate_client-4.6.0b0/integration/hobbits.mp4`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_auth.py` & `weaviate_client-4.6.0b0/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_batch_v4.py` & `weaviate_client-4.6.0b0/integration/test_batch_v4.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
         assert len(obj.references["test"].objects) == nr_objects - 1
     client.collections.delete(name)
 
 
 def test_add_1000_objects_with_async_indexing_and_wait(
     client_factory: ClientFactory, request: SubRequest
 ) -> None:
-    client, name = client_factory(ports=(8090, 50060))
+    client, name = client_factory(ports=(8090, 50061))
 
     nr_objects = 1000
     with client.batch.dynamic() as batch:
         for i in range(nr_objects):
             batch.add_object(
                 collection=name,
                 properties={"name": "text" + str(i)},
@@ -418,20 +418,20 @@
     assert ret.total_count == nr_objects
 
     old_client = weaviate.Client("http://localhost:8090")
     assert old_client.schema.get_class_shards(name)[0]["status"] == "READY"
     assert old_client.schema.get_class_shards(name)[0]["vectorQueueSize"] == 0
 
 
-@pytest.mark.skip("Difficult to find numbers that work reliable in the CI")
+@pytest.mark.skip("Difficult to find numbers that work reliably in the CI")
 def test_add_10000_objects_with_async_indexing_and_dont_wait(
     client_factory: ClientFactory, request: SubRequest
 ) -> None:
     old_client = weaviate.Client("http://localhost:8090")
-    client, name = client_factory(ports=(8090, 50060))
+    client, name = client_factory(ports=(8090, 50061))
 
     nr_objects = 10000
     vec_length = 1000
     with client.batch.fixed_size(batch_size=1000, concurrent_requests=1) as batch:
         for i in range(nr_objects):
             batch.add_object(
                 collection=name,
@@ -447,15 +447,15 @@
     ret = client.collections.get(name).aggregate.over_all(total_count=True)
     assert ret.total_count == nr_objects
 
 
 def test_add_1000_tenant_objects_with_async_indexing_and_wait_for_all(
     client_factory: ClientFactory, request: SubRequest
 ) -> None:
-    client, name = client_factory(ports=(8090, 50060), multi_tenant=True)
+    client, name = client_factory(ports=(8090, 50061), multi_tenant=True)
     tenants = [Tenant(name="tenant" + str(i)) for i in range(2)]
     collection = client.collections.get(name)
     collection.tenants.create(tenants)
     nr_objects = 2000
 
     with client.batch.dynamic() as batch:
         for i in range(nr_objects):
@@ -472,18 +472,19 @@
         assert ret.total_count == nr_objects / len(tenants)
     old_client = weaviate.Client("http://localhost:8090")
     for shard in old_client.schema.get_class_shards(name):
         assert shard["status"] == "READY"
         assert shard["vectorQueueSize"] == 0
 
 
+@pytest.mark.skip("Difficult to find numbers that work reliably in the CI")
 def test_add_1000_tenant_objects_with_async_indexing_and_wait_for_only_one(
     client_factory: ClientFactory,
 ) -> None:
-    client, name = client_factory(ports=(8090, 50060), multi_tenant=True)
+    client, name = client_factory(ports=(8090, 50061), multi_tenant=True)
     tenants = [Tenant(name="tenant" + str(i)) for i in range(2)]
     collection = client.collections.get(name)
     collection.tenants.create(tenants)
 
     nr_objects = 1001
 
     with client.batch.dynamic() as batch:
```

### Comparing `weaviate-client-4.5rc0/integration/test_client.py` & `weaviate_client-4.6.0b0/integration/test_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generator
+from typing import Generator, Tuple, Union
 
 import pytest
 from _pytest.fixtures import SubRequest
 
 import weaviate
 from weaviate.collections import Collection
 from weaviate.collections.classes.config import (
@@ -10,18 +10,19 @@
     _CollectionConfig,
     DataType,
     GenerativeSearches,
     Property,
     ReferenceProperty,
     Vectorizers,
 )
-from weaviate.connect.base import _Timeout
 from weaviate.exceptions import WeaviateClosedClientError, WeaviateStartUpError
 import weaviate.classes as wvc
 
+from weaviate.config import Timeout
+
 WCS_HOST = "piblpmmdsiknacjnm1ltla.c1.europe-west3.gcp.weaviate.cloud"
 WCS_URL = f"https://{WCS_HOST}"
 WCS_GRPC_HOST = f"grpc-{WCS_HOST}"
 WCS_CREDS = wvc.init.Auth.api_key("cy4ua772mBlMdfw3YnclqAWzFhQt0RLIN0sl")
 
 
 @pytest.fixture(scope="module")
@@ -325,14 +326,34 @@
     client.collections.delete(request.node.name)
     collection = client.collections.create(name=request.node.name)
 
     nodes = client.cluster.nodes(collection.name, output="verbose")
     assert len(nodes) == 1
     assert len(nodes[0].shards) == 1
     assert nodes[0].shards[0].collection == collection.name
+    assert nodes[0].shards[0].object_count == 0
+    assert nodes[0].shards[0].vector_indexing_status == "READY"
+    assert nodes[0].shards[0].vector_queue_length == 0
+    assert nodes[0].shards[0].compressed is False
+    if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
+        assert nodes[0].shards[0].loaded is None
+    else:
+        assert nodes[0].shards[0].loaded is True
+
+
+def test_client_cluster_multitenant(client: weaviate.WeaviateClient, request: SubRequest) -> None:
+    client.collections.delete(request.node.name)
+    collection = client.collections.create(
+        name=request.node.name,
+        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
+    )
+
+    nodes = client.cluster.nodes(collection.name, output="verbose")
+    assert len(nodes) == 1
+    assert len(nodes[0].shards) == 0
 
 
 def test_client_cluster_minimal(client: weaviate.WeaviateClient, request: SubRequest) -> None:
     client.collections.delete(request.node.name)
     collection = client.collections.create(name=request.node.name)
 
     nodes = client.cluster.nodes(collection.name, output="minimal")
@@ -427,16 +448,17 @@
 
     col.data.insert(properties={"name": "Name"})
 
     obj = col.query.fetch_objects().objects[0]
     assert obj.properties["name"] == "Name"
 
 
-def test_client_with_extra_options() -> None:
-    additional_config = wvc.init.AdditionalConfig(timeout=(1, 2), trust_env=True)
+@pytest.mark.parametrize("timeout", [(1, 2), Timeout(query=1, insert=2, init=2)])
+def test_client_with_extra_options(timeout: Union[Tuple[int, int], Timeout]) -> None:
+    additional_config = wvc.init.AdditionalConfig(timeout=timeout, trust_env=True)
 
     for client in [
         weaviate.connect_to_wcs(
             cluster_url=WCS_URL, auth_credentials=WCS_CREDS, additional_config=additional_config
         ),
         weaviate.connect_to_local(additional_config=additional_config),
         weaviate.connect_to_custom(
@@ -445,81 +467,16 @@
             http_port=443,
             grpc_secure=True,
             grpc_host=WCS_GRPC_HOST,
             grpc_port=443,
             auth_credentials=WCS_CREDS,
             additional_config=additional_config,
         ),
-        weaviate.connect_to_embedded(
-            port=8070, grpc_port=50040, additional_config=additional_config
-        ),
     ]:
-        assert client._connection.timeout_config == _Timeout(1, 2)
-
-
-def test_connect_and_close_to_embedded() -> None:
-    # Can't use the default port values as they are already in use by the local instances
-    client = weaviate.connect_to_embedded(port=8078, grpc_port=50151, version="1.23.7")
-
-    client.connect()
-    assert client.is_connected()
-    metadata = client.get_meta()
-    assert "1.23.7" == metadata["version"]
-    assert client.is_ready()
-    assert "8078" == metadata["hostname"].split(":")[2]
-    assert client.is_live()
-
-    client.close()
-    assert not client.is_connected()
-    with pytest.raises(WeaviateClosedClientError):
-        client.get_meta()
-
-
-def test_embedded_as_context_manager() -> None:
-    default_version = "1.23.7"
-    with weaviate.connect_to_embedded(port=8077, grpc_port=50152) as client:
-        assert client.is_connected()
-        metadata = client.get_meta()
-        assert default_version == metadata["version"]
-        assert client.is_ready()
-        assert client.is_live()
-
-    assert not client.is_connected()
-    with pytest.raises(WeaviateClosedClientError):
-        client.get_meta()
-
-
-def test_embedded_with_wrong_version() -> None:
-    with pytest.raises(weaviate.exceptions.WeaviateEmbeddedInvalidVersionError):
-        weaviate.connect_to_embedded(version="this_version_does_not_exist")
-
-
-def test_embedded_already_running() -> None:
-    client = weaviate.connect_to_embedded(port=8096, grpc_port=50155)
-    assert client._connection.embedded_db is not None
-    assert client._connection.embedded_db.process is not None
-
-    with pytest.raises(weaviate.exceptions.WeaviateStartUpError):
-        weaviate.connect_to_embedded(port=8096, grpc_port=50155)
-
-    client.close()
-
-
-def test_embedded_startup_with_blocked_http_port() -> None:
-    client = weaviate.connect_to_embedded(port=8098, grpc_port=50096)
-    with pytest.raises(weaviate.exceptions.WeaviateStartUpError):
-        weaviate.connect_to_embedded(port=8098, grpc_port=50097)
-    client.close()
-
-
-def test_embedded_startup_with_blocked_grpc_port() -> None:
-    client = weaviate.connect_to_embedded(port=8099, grpc_port=50150)
-    with pytest.raises(weaviate.exceptions.WeaviateStartUpError):
-        weaviate.connect_to_embedded(port=8100, grpc_port=50150)
-    client.close()
+        assert client._connection.timeout_config == Timeout(query=1, insert=2, init=2)
 
 
 def test_client_error_for_wcs_without_auth() -> None:
     with pytest.raises(weaviate.exceptions.AuthenticationFailedError) as e:
         weaviate.connect_to_wcs(cluster_url=WCS_URL, auth_credentials=None)
         assert "wvc.init.Auth.api_key" in e.value.message
 
@@ -533,7 +490,25 @@
     ).is_ready()
 
 
 def test_client_is_ready() -> None:
     assert weaviate.connect_to_wcs(
         cluster_url=WCS_URL, auth_credentials=WCS_CREDS, skip_init_checks=True
     ).is_ready()
+
+
+def test_local_proxies() -> None:
+    with weaviate.connect_to_local(
+        additional_config=wvc.init.AdditionalConfig(
+            proxies=wvc.init.Proxies(
+                http="http://localhost:8075",
+                grpc="http://localhost:10000",
+            )
+        )
+    ) as client:
+        client.collections.delete("TestLocalProxies")
+        collection = client.collections.create(
+            "TestLocalProxies",
+            properties=[wvc.config.Property(name="name", data_type=wvc.config.DataType.TEXT)],
+        )
+        collection.data.insert({"name": "Test"})
+        assert collection.query.fetch_objects().objects[0].properties["name"] == "Test"
```

### Comparing `weaviate-client-4.5rc0/integration/test_collection.py` & `weaviate_client-4.6.0b0/integration/test_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,25 +36,27 @@
     NearMediaType,
 )
 from weaviate.collections.classes.internal import (
     _CrossReference,
     Object,
     ReferenceToMulti,
 )
-from weaviate.collections.classes.tenants import Tenant, TenantActivityStatus
 from weaviate.collections.classes.types import PhoneNumber, WeaviateProperties
 from weaviate.exceptions import (
     UnexpectedStatusCodeError,
     WeaviateInvalidInputError,
     WeaviateQueryError,
     WeaviateInsertInvalidPropertyError,
     WeaviateInsertManyAllFailedError,
+    WeaviateUnsupportedFeatureError,
 )
 from weaviate.types import UUID, UUIDS
 
+import weaviate.classes as wvc
+
 UUID1 = uuid.UUID("806827e0-2b31-43ca-9269-24fa95a221f9")
 UUID2 = uuid.UUID("8ad0d33c-8db1-4437-87f3-72161ca2a51a")
 UUID3 = uuid.UUID("83d99755-9deb-4b16-8431-d1dff4ab0a75")
 
 DATE1 = datetime.datetime.strptime("2012-02-09", "%Y-%m-%d").replace(tzinfo=datetime.timezone.utc)
 DATE2 = datetime.datetime.strptime("2013-02-10", "%Y-%m-%d").replace(tzinfo=datetime.timezone.utc)
 DATE3 = datetime.datetime.strptime("2019-06-10", "%Y-%m-%d").replace(tzinfo=datetime.timezone.utc)
@@ -139,29 +141,14 @@
     assert collection.query.fetch_object_by_id(uuid) is not None
     assert collection.data.delete_by_id(uuid)
     assert collection.query.fetch_object_by_id(uuid) is None
     # does not exist anymore
     assert not collection.data.delete_by_id(uuid)
 
 
-def test_delete_by_id_tenant(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        vectorizer_config=Configure.Vectorizer.none(),
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-    collection.tenants.create([Tenant(name="tenant1")])
-    tenant1 = collection.with_tenant("tenant1")
-    uuid = tenant1.data.insert(properties={})
-    assert tenant1.query.fetch_object_by_id(uuid) is not None
-    assert tenant1.data.delete_by_id(uuid)
-    assert tenant1.query.fetch_object_by_id(uuid) is None
-    # does not exist anymore
-    assert not tenant1.data.delete_by_id(uuid)
-
-
 def test_delete_by_id_consistency_level(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(
         vectorizer_config=Configure.Vectorizer.none(),
     ).with_consistency_level(ConsistencyLevel.ALL)
 
     uuid = collection.data.insert(properties={})
     assert collection.query.fetch_object_by_id(uuid) is not None
@@ -413,40 +400,14 @@
 
     assert isinstance(ret.all_responses[0], ErrorObject) and isinstance(
         ret.all_responses[2], ErrorObject
     )
     assert isinstance(ret.all_responses[1], uuid.UUID)
 
 
-def test_insert_many_with_tenant(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        properties=[Property(name="Name", data_type=DataType.TEXT)],
-        vectorizer_config=Configure.Vectorizer.none(),
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-
-    collection.tenants.create([Tenant(name="tenant1"), Tenant(name="tenant2")])
-    tenant1 = collection.with_tenant("tenant1")
-    tenant2 = collection.with_tenant("tenant2")
-
-    ret = tenant1.data.insert_many(
-        [
-            DataObject(properties={"name": "some name"}, vector=[1, 2, 3]),
-            DataObject(properties={"name": "some other name"}, uuid=uuid.uuid4()),
-        ]
-    )
-    assert not ret.has_errors
-    obj1 = tenant1.query.fetch_object_by_id(ret.uuids[0])
-    obj2 = tenant1.query.fetch_object_by_id(ret.uuids[1])
-    assert obj1.properties["name"] == "some name"
-    assert obj2.properties["name"] == "some other name"
-    assert tenant2.query.fetch_object_by_id(ret.uuids[0]) is None
-    assert tenant2.query.fetch_object_by_id(ret.uuids[1]) is None
-
-
 def test_replace(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(
         properties=[Property(name="Name", data_type=DataType.TEXT)],
         vectorizer_config=Configure.Vectorizer.none(),
     )
     uuid = collection.data.insert(properties={"name": "some name"})
     collection.data.replace(properties={"name": "other name"}, uuid=uuid)
@@ -510,60 +471,14 @@
 
     collection.data.replace(properties={"name": "real name"}, uuid=uuid, vector=[2, 3, 4])
     obj = collection.query.fetch_object_by_id(uuid, include_vector=True)
     assert obj.properties["name"] == "real name"
     assert obj.vector["default"] == [2, 3, 4]
 
 
-def test_replace_with_tenant(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        properties=[Property(name="Name", data_type=DataType.TEXT)],
-        vectorizer_config=Configure.Vectorizer.none(),
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-
-    collection.tenants.create([Tenant(name="tenant1"), Tenant(name="tenant2")])
-    tenant1 = collection.with_tenant("tenant1")
-    tenant2 = collection.with_tenant("tenant2")
-
-    uuid = tenant1.data.insert(properties={"name": "some name"})
-    tenant1.data.replace(properties={"name": "other name"}, uuid=uuid)
-    assert tenant1.query.fetch_object_by_id(uuid).properties["name"] == "other name"
-    assert tenant2.query.fetch_object_by_id(uuid) is None
-
-
-def test_update(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        properties=[Property(name="Name", data_type=DataType.TEXT)],
-        vectorizer_config=Configure.Vectorizer.none(),
-    )
-    uuid = collection.data.insert(properties={"name": "some name"})
-    collection.data.update(properties={"name": "other name"}, uuid=uuid, vector=[1, 2, 3])
-    obj = collection.query.fetch_object_by_id(uuid, include_vector=True)
-    assert obj.properties["name"] == "other name"
-    assert obj.vector["default"] == [1, 2, 3]
-
-
-def test_update_with_tenant(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        properties=[Property(name="Name", data_type=DataType.TEXT)],
-        vectorizer_config=Configure.Vectorizer.none(),
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-
-    collection.tenants.create([Tenant(name="tenant1"), Tenant(name="tenant2")])
-    tenant1 = collection.with_tenant("tenant1")
-    tenant2 = collection.with_tenant("tenant2")
-
-    uuid = tenant1.data.insert(properties={"name": "some name"})
-    tenant1.data.update(properties={"name": "other name"}, uuid=uuid)
-    assert tenant1.query.fetch_object_by_id(uuid).properties["name"] == "other name"
-    assert tenant2.query.fetch_object_by_id(uuid) is None
-
-
 @pytest.mark.parametrize("to_uuids", [UUID3, [UUID3]])
 def test_update_with_refs(collection_factory: CollectionFactory, to_uuids: UUIDS) -> None:
     ref_collection = collection_factory(
         name="target", vectorizer_config=Configure.Vectorizer.none()
     )
     ref_collection.data.insert(properties={}, uuid=UUID1)
     ref_collection.data.insert(properties={}, uuid=UUID2)
@@ -648,14 +563,42 @@
 
     objs = collection.query.hybrid(
         alpha=1, query="name", fusion_type=fusion_type, vector=objs[0].vector["default"]
     ).objects
     assert len(objs) == 2
 
 
+def test_search_hybrid_group_by(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory(
+        properties=[Property(name="Name", data_type=DataType.TEXT)],
+        vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
+            vectorize_collection_name=False
+        ),
+    )
+    collection.data.insert({"Name": "some name"}, uuid=uuid.uuid4())
+    collection.data.insert({"Name": "other word"}, uuid=uuid.uuid4())
+    if collection._connection.supports_groupby_in_bm25_and_hybrid():
+        objs = collection.query.hybrid(
+            alpha=0,
+            query="name",
+            include_vector=True,
+            group_by=GroupBy(prop="name", objects_per_group=1, number_of_groups=2),
+        ).objects
+        assert len(objs) == 1
+        assert objs[0].belongs_to_group == "some name"
+    else:
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            collection.query.hybrid(
+                alpha=0,
+                query="name",
+                include_vector=True,
+                group_by=GroupBy(prop="name", objects_per_group=1, number_of_groups=2),
+            )
+
+
 @pytest.mark.parametrize("query", [None, ""])
 def test_search_hybrid_only_vector(
     collection_factory: CollectionFactory, query: Optional[str]
 ) -> None:
     collection = collection_factory(
         properties=[Property(name="Name", data_type=DataType.TEXT)],
         vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
@@ -705,14 +648,90 @@
         ]
     )
     assert res.has_errors is False
 
     assert len(collection.query.hybrid(query="test", alpha=0, offset=offset).objects) == expected
 
 
+def test_hybrid_alpha(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory(
+        properties=[Property(name="name", data_type=DataType.TEXT)],
+        vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
+            vectorize_collection_name=False
+        ),
+    )
+
+    res = collection.data.insert_many(
+        [
+            {"name": "banana"},
+            {"name": "fruit"},
+            {"name": "car"},
+        ]
+    )
+    assert res.has_errors is False
+
+    hybrid_res = collection.query.hybrid(query="fruit", alpha=0)
+    bm25_res = collection.query.bm25(query="fruit")
+    assert all(
+        bm25_res.objects[i].uuid == hybrid_res.objects[i].uuid
+        for i in range(len(hybrid_res.objects))
+    )
+
+    hybrid_res = collection.query.hybrid(query="fruit", alpha=1)
+    text_res = collection.query.near_text(query="fruit")
+    assert all(
+        text_res.objects[i].uuid == hybrid_res.objects[i].uuid
+        for i in range(len(hybrid_res.objects))
+    )
+
+
+def test_bm25(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory(
+        properties=[Property(name="Name", data_type=DataType.TEXT)],
+        vectorizer_config=Configure.Vectorizer.none(),
+    )
+
+    res = collection.data.insert_many(
+        [
+            {"Name": "test"},
+            {"Name": "another"},
+            {"Name": "test"},
+        ]
+    )
+    assert res.has_errors is False
+    assert len(collection.query.bm25(query="test").objects) == 2
+
+
+def test_bm25_group_by(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory(
+        properties=[Property(name="Name", data_type=DataType.TEXT)],
+        vectorizer_config=Configure.Vectorizer.none(),
+    )
+
+    res = collection.data.insert_many(
+        [
+            {"Name": "test"},
+            {"Name": "another"},
+            {"Name": "test"},
+        ]
+    )
+    assert res.has_errors is False
+    if collection._connection.supports_groupby_in_bm25_and_hybrid():
+        objs = collection.query.bm25(
+            query="test", group_by=GroupBy(prop="name", objects_per_group=1, number_of_groups=2)
+        ).objects
+        assert len(objs) == 1
+        assert objs[0].belongs_to_group == "test"
+    else:
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            collection.query.bm25(
+                query="test", group_by=GroupBy(prop="name", objects_per_group=1, number_of_groups=2)
+            )
+
+
 @pytest.mark.parametrize("limit", [1, 2])
 def test_bm25_limit(collection_factory: CollectionFactory, limit: int) -> None:
     collection = collection_factory(
         properties=[Property(name="Name", data_type=DataType.TEXT, tokenization=Tokenization.WORD)],
         vectorizer_config=Configure.Vectorizer.none(),
     )
 
@@ -1044,35 +1063,14 @@
     assert len(ret.objects) == 4
     assert ret.objects[0].belongs_to_group == "Banana"
     assert ret.objects[1].belongs_to_group == "Banana"
     assert ret.objects[2].belongs_to_group == "car"
     assert ret.objects[3].belongs_to_group == "Mountain"
 
 
-def test_tenants(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        vectorizer_config=Configure.Vectorizer.none(),
-        multi_tenancy_config=Configure.multi_tenancy(
-            enabled=True,
-        ),
-    )
-
-    collection.tenants.create([Tenant(name="tenant1")])
-
-    tenants = collection.tenants.get()
-    assert len(tenants) == 1
-    assert type(tenants["tenant1"]) is Tenant
-    assert tenants["tenant1"].name == "tenant1"
-
-    collection.tenants.remove(["tenant1"])
-
-    tenants = collection.tenants.get()
-    assert len(tenants) == 0
-
-
 def test_multi_searches(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(
         properties=[Property(name="name", data_type=DataType.TEXT)],
         vectorizer_config=Configure.Vectorizer.none(),
     )
 
     collection.data.insert(properties={"name": "word"})
@@ -1093,97 +1091,27 @@
 
     objects = collection.query.bm25(query="other", return_properties=[]).objects
     assert "name" not in objects[0].properties
     assert objects[0].uuid is not None
     assert objects[0].metadata._is_empty()
 
 
-def test_search_with_tenant(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        vectorizer_config=Configure.Vectorizer.none(),
-        properties=[Property(name="name", data_type=DataType.TEXT)],
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-
-    collection.tenants.create([Tenant(name="Tenant1"), Tenant(name="Tenant2")])
-    tenant1 = collection.with_tenant("Tenant1")
-    tenant2 = collection.with_tenant("Tenant2")
-    uuid1 = tenant1.data.insert({"name": "some name"})
-    objects1 = tenant1.query.bm25(query="some").objects
-    assert len(objects1) == 1
-    assert objects1[0].uuid == uuid1
-
-    objects2 = tenant2.query.bm25(query="some").objects
-    assert len(objects2) == 0
-
-
-def test_fetch_object_by_id_with_tenant(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        vectorizer_config=Configure.Vectorizer.none(),
-        properties=[Property(name="name", data_type=DataType.TEXT)],
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-
-    collection.tenants.create([Tenant(name="Tenant1"), Tenant(name="Tenant2")])
-    tenant1 = collection.with_tenant("Tenant1")
-    tenant2 = collection.with_tenant("Tenant2")
-
-    uuid1 = tenant1.data.insert({"name": "some name"})
-    obj1 = tenant1.query.fetch_object_by_id(uuid1)
-    assert obj1.properties["name"] == "some name"
-
-    obj2 = tenant2.query.fetch_object_by_id(uuid1)
-    assert obj2 is None
-
-    uuid2 = tenant2.data.insert({"name": "some other name"})
-    obj3 = tenant2.query.fetch_object_by_id(uuid2)
-    assert obj3.properties["name"] == "some other name"
-
-    obj4 = tenant1.query.fetch_object_by_id(uuid2)
-    assert obj4 is None
-
-
 def test_fetch_objects_with_limit(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(
         vectorizer_config=Configure.Vectorizer.none(),
         properties=[Property(name="name", data_type=DataType.TEXT)],
     )
 
     for i in range(10):
         collection.data.insert({"name": str(i)})
 
     objects = collection.query.fetch_objects(limit=5).objects
     assert len(objects) == 5
 
 
-def test_fetch_objects_with_tenant(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        vectorizer_config=Configure.Vectorizer.none(),
-        properties=[Property(name="name", data_type=DataType.TEXT)],
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-
-    collection.tenants.create([Tenant(name="Tenant1"), Tenant(name="Tenant2")])
-    tenant1 = collection.with_tenant("Tenant1")
-    tenant2 = collection.with_tenant("Tenant2")
-
-    tenant1.data.insert({"name": "some name"})
-    objects = tenant1.query.fetch_objects().objects
-    assert len(objects) == 1
-    assert objects[0].properties["name"] == "some name"
-
-    objects = tenant2.query.fetch_objects().objects
-    assert len(objects) == 0
-
-    tenant2.data.insert({"name": "some other name"})
-    objects = tenant2.query.fetch_objects().objects
-    assert len(objects) == 1
-    assert objects[0].properties["name"] == "some other name"
-
-
 def test_add_property(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(
         vectorizer_config=Configure.Vectorizer.none(),
         properties=[Property(name="name", data_type=DataType.TEXT)],
     )
     uuid1 = collection.data.insert({"name": "first"})
     collection.config.add_property(Property(name="number", data_type=DataType.INT))
@@ -1366,66 +1294,14 @@
 
     uuid1 = collection.data.insert({})
 
     assert collection.data.exists(uuid1)
     assert not collection.data.exists(uuid.uuid4())
 
 
-def test_exist_with_tenant(collection_factory: CollectionFactory) -> None:
-    collection = collection_factory(
-        vectorizer_config=Configure.Vectorizer.none(),
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-    collection.tenants.create([Tenant(name="Tenant1"), Tenant(name="Tenant2")])
-
-    uuid1 = collection.with_tenant("Tenant1").data.insert({})
-    uuid2 = collection.with_tenant("Tenant2").data.insert({})
-
-    assert collection.with_tenant("Tenant1").data.exists(uuid1)
-    assert not collection.with_tenant("Tenant2").data.exists(uuid1)
-    assert collection.with_tenant("Tenant2").data.exists(uuid2)
-    assert not collection.with_tenant("Tenant1").data.exists(uuid2)
-
-
-def test_tenant_with_activity(collection_factory: CollectionFactory) -> None:
-    name = "TestTenantActivity"
-    collection = collection_factory(
-        name=name,
-        vectorizer_config=Configure.Vectorizer.none(),
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-    collection.tenants.create(
-        [
-            Tenant(name="1", activity_status=TenantActivityStatus.HOT),
-            Tenant(name="2", activity_status=TenantActivityStatus.COLD),
-            Tenant(name="3"),
-        ]
-    )
-    tenants = collection.tenants.get()
-    assert tenants["1"].activity_status == TenantActivityStatus.HOT
-    assert tenants["2"].activity_status == TenantActivityStatus.COLD
-    assert tenants["3"].activity_status == TenantActivityStatus.HOT
-
-
-def test_update_tenant(collection_factory: CollectionFactory) -> None:
-    name = "TestUpdateTenant"
-    collection = collection_factory(
-        name=name,
-        vectorizer_config=Configure.Vectorizer.none(),
-        multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-    )
-    collection.tenants.create([Tenant(name="1", activity_status=TenantActivityStatus.HOT)])
-    tenants = collection.tenants.get()
-    assert tenants["1"].activity_status == TenantActivityStatus.HOT
-
-    collection.tenants.update([Tenant(name="1", activity_status=TenantActivityStatus.COLD)])
-    tenants = collection.tenants.get()
-    assert tenants["1"].activity_status == TenantActivityStatus.COLD
-
-
 def test_return_list_properties(collection_factory: CollectionFactory) -> None:
     name_small = "TestReturnList"
     collection = collection_factory(
         name=name_small,
         vectorizer_config=Configure.Vectorizer.none(),
         properties=[
             Property(name="ints", data_type=DataType.INT_ARRAY),
@@ -2045,7 +1921,245 @@
 
     collection.data.insert({"a": "a1"})
     objs = collection.query.fetch_objects(return_properties=["a", "b"]).objects
     assert len(objs) == 1
     assert objs[0].properties["a"] == "a1"
     if "b" in objs[0].properties:  # change this when server version bumps to 1.24.0
         assert objs[0].properties["b"] is None
+
+
+def test_none_query_hybrid_bm25(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory(
+        properties=[
+            Property(name="text", data_type=DataType.TEXT),
+        ],
+        vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
+            vectorize_collection_name=False
+        ),
+    )
+
+    collection.data.insert({"text": "banana"})
+    collection.data.insert({"text": "dog"})
+    collection.data.insert({"text": "different concept"})
+
+    hybrid_objs = collection.query.hybrid(
+        query=None, vector=None, return_metadata=MetadataQuery.full()
+    ).objects
+    assert len(hybrid_objs) == 3
+    assert all(obj.metadata.score is not None and obj.metadata.score == 0.0 for obj in hybrid_objs)
+
+    bm25_objs = collection.query.bm25(query=None, return_metadata=MetadataQuery.full()).objects
+    assert len(bm25_objs) == 3
+    assert all(obj.metadata.score is not None and obj.metadata.score == 0.0 for obj in bm25_objs)
+
+
+def test_hybrid_near_vector_search(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory(
+        properties=[
+            Property(name="text", data_type=DataType.TEXT),
+        ],
+        vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
+            vectorize_collection_name=False
+        ),
+    )
+    uuid_banana = collection.data.insert({"text": "banana"})
+    obj = collection.query.fetch_object_by_id(uuid_banana, include_vector=True)
+
+    if collection._connection._weaviate_version.is_lower_than(1, 25, 0):
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            collection.query.hybrid(
+                query=None,
+                vector=wvc.query.HybridNear.vector(vector=obj.vector["default"]),
+            ).objects
+        return
+
+    collection.data.insert({"text": "dog"})
+    collection.data.insert({"text": "different concept"})
+
+    hybrid_objs: List[Object[Any, Any]] = collection.query.hybrid(
+        query=None,
+        vector=wvc.query.HybridNear.vector(vector=obj.vector["default"]),
+    ).objects
+
+    assert hybrid_objs[0].uuid == uuid_banana
+    assert len(hybrid_objs) == 3
+
+    # make a near vector search to get the distance
+    near_vec = collection.query.near_vector(
+        near_vector=obj.vector["default"], return_metadata=["distance"]
+    ).objects
+    assert near_vec[0].metadata.distance is not None
+
+    hybrid_objs2 = collection.query.hybrid(
+        query=None,
+        vector=wvc.query.HybridNear.vector(
+            vector=obj.vector["default"], distance=near_vec[0].metadata.distance + 0.001
+        ),
+        return_metadata=MetadataQuery.full(),
+    ).objects
+
+    assert hybrid_objs2[0].uuid == uuid_banana
+    assert len(hybrid_objs2) == 1
+
+
+def test_hybrid_near_vector_search_named_vectors(collection_factory: CollectionFactory) -> None:
+    dummy = collection_factory("dummy")
+    collection_maker = lambda: collection_factory(
+        properties=[
+            Property(name="text", data_type=DataType.TEXT),
+            Property(name="int", data_type=DataType.INT),
+        ],
+        vectorizer_config=[
+            Configure.NamedVectors.text2vec_contextionary(
+                name="text", vectorize_collection_name=False
+            ),
+            Configure.NamedVectors.text2vec_contextionary(
+                name="int", vectorize_collection_name=False
+            ),
+        ],
+    )
+
+    if dummy._connection._weaviate_version.is_lower_than(1, 24, 0):
+        with pytest.raises(WeaviateInvalidInputError):
+            collection_maker()
+        return
+
+    collection = collection_maker()
+    uuid_banana = collection.data.insert({"text": "banana"})
+    collection.data.insert({"text": "dog"})
+    collection.data.insert({"text": "different concept"})
+
+    obj = collection.query.fetch_object_by_id(uuid_banana, include_vector=True)
+
+    if collection._connection._weaviate_version.is_lower_than(1, 25, 0):
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            hybrid_objs: List[Object[Any, Any]] = collection.query.hybrid(
+                query=None,
+                vector=wvc.query.HybridNear.vector(vector=obj.vector["text"], target_vector="text"),
+            ).objects
+        return
+
+    hybrid_objs = collection.query.hybrid(
+        query=None,
+        vector=wvc.query.HybridNear.vector(vector=obj.vector["text"], target_vector="text"),
+    ).objects
+
+    assert hybrid_objs[0].uuid == uuid_banana
+    assert len(hybrid_objs) == 3
+
+    # make a near vector search to get the distance
+    near_vec = collection.query.near_vector(
+        near_vector=obj.vector["text"], return_metadata=["distance"], target_vector="text"
+    ).objects
+    assert near_vec[0].metadata.distance is not None
+
+    hybrid_objs2 = collection.query.hybrid(
+        query=None,
+        vector=wvc.query.HybridNear.vector(
+            vector=obj.vector["text"],
+            distance=near_vec[0].metadata.distance + 0.001,
+            target_vector="text",
+        ),
+        return_metadata=MetadataQuery.full(),
+    ).objects
+
+    assert hybrid_objs2[0].uuid == uuid_banana
+    assert len(hybrid_objs2) == 1
+
+
+def test_hybrid_near_text_search(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory(
+        properties=[
+            Property(name="text", data_type=DataType.TEXT),
+        ],
+        vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
+            vectorize_collection_name=False
+        ),
+    )
+
+    if collection._connection._weaviate_version.is_lower_than(1, 25, 0):
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            collection.query.hybrid(
+                query=None,
+                vector=wvc.query.HybridNear.text(text="banana pudding"),
+            ).objects
+        return
+
+    uuid_banana_pudding = collection.data.insert({"text": "banana pudding"})
+    collection.data.insert({"text": "banana smoothie"})
+    collection.data.insert({"text": "different concept"})
+
+    hybrid_objs: List[Object[Any, Any]] = collection.query.hybrid(
+        query=None,
+        vector=wvc.query.HybridNear.text(text="banana pudding"),
+    ).objects
+
+    assert hybrid_objs[0].uuid == uuid_banana_pudding
+    assert len(hybrid_objs) == 3
+
+    hybrid_objs2 = collection.query.hybrid(
+        query=None,
+        vector=wvc.query.HybridNear.text(
+            text="banana",
+            move_to=wvc.query.Move(concepts="pudding", force=0.1),
+            move_away=wvc.query.Move(concepts="smoothie", force=0.1),
+        ),
+        return_metadata=MetadataQuery.full(),
+    ).objects
+
+    assert hybrid_objs2[0].uuid == uuid_banana_pudding
+
+
+def test_hybrid_near_text_search_named_vectors(collection_factory: CollectionFactory) -> None:
+    dummy = collection_factory("dummy")
+    collection_maker = lambda: collection_factory(
+        properties=[
+            Property(name="text", data_type=DataType.TEXT),
+            Property(name="int", data_type=DataType.INT),
+        ],
+        vectorizer_config=[
+            Configure.NamedVectors.text2vec_contextionary(
+                name="text", vectorize_collection_name=False
+            ),
+            Configure.NamedVectors.text2vec_contextionary(
+                name="int", vectorize_collection_name=False
+            ),
+        ],
+    )
+    if dummy._connection._weaviate_version.is_lower_than(1, 24, 0):
+        with pytest.raises(WeaviateInvalidInputError):
+            collection_maker()
+        return
+
+    collection = collection_maker()
+    uuid_banana_pudding = collection.data.insert({"text": "banana pudding"})
+    collection.data.insert({"text": "banana smoothie"})
+    collection.data.insert({"text": "different concept"})
+
+    if collection._connection._weaviate_version.is_lower_than(1, 25, 0):
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            hybrid_objs: List[Object[Any, Any]] = collection.query.hybrid(
+                query=None,
+                vector=wvc.query.HybridNear.text(text="banana pudding", target_vector="text"),
+            ).objects
+        return
+
+    hybrid_objs = collection.query.hybrid(
+        query=None,
+        vector=wvc.query.HybridNear.text(text="banana pudding", target_vector="text"),
+    ).objects
+
+    assert hybrid_objs[0].uuid == uuid_banana_pudding
+    assert len(hybrid_objs) == 3
+
+    hybrid_objs2 = collection.query.hybrid(
+        query=None,
+        vector=wvc.query.HybridNear.text(
+            text="banana",
+            move_to=wvc.query.Move(concepts="pudding", force=0.1),
+            move_away=wvc.query.Move(concepts="smoothie", force=0.1),
+            target_vector="text",
+        ),
+        return_metadata=MetadataQuery.full(),
+    ).objects
+
+    assert hybrid_objs2[0].uuid == uuid_banana_pudding
```

### Comparing `weaviate-client-4.5rc0/integration/test_collection_aggregate.py` & `weaviate_client-4.6.0b0/integration/test_collection_aggregate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pathlib
 import uuid
 from datetime import datetime, timezone
+from typing import Union
 
 import pytest
 from _pytest.fixtures import SubRequest
 
 from integration.conftest import CollectionFactory, CollectionFactoryGet
 from weaviate.collections.classes.aggregate import (
     AggregateBoolean,
@@ -14,15 +15,19 @@
     AggregateText,
     AggregateReturn,
     Metrics,
     GroupByAggregate,
 )
 from weaviate.collections.classes.config import DataType, Property, ReferenceProperty, Configure
 from weaviate.collections.classes.filters import Filter, _Filters
-from weaviate.exceptions import WeaviateInvalidInputError, WeaviateQueryError
+from weaviate.exceptions import (
+    WeaviateInvalidInputError,
+    WeaviateQueryError,
+    WeaviateUnsupportedFeatureError,
+)
 from weaviate.util import file_encoder_b64
 
 from weaviate.collections.classes.grpc import Move
 
 from weaviate.collections.classes.tenants import Tenant
 
 UUID1 = uuid.UUID("8ad0d33c-8db1-4437-87f3-72161ca2a51a")
@@ -67,15 +72,28 @@
     collection = collection_factory(properties=[Property(name="text", data_type=DataType.TEXT)])
     collection.data.insert({"text": "some text"})
     res = collection.aggregate.over_all(return_metrics=[Metrics("text").text(count=True)])
     assert isinstance(res.properties["text"], AggregateText)
     assert res.properties["text"].count == 1
 
 
-def test_aggregation_with_limit(collection_factory: CollectionFactory) -> None:
+def test_aggregation_top_occurence_with_limit(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory(properties=[Property(name="text", data_type=DataType.TEXT)])
+    collection.data.insert({"text": "one"})
+    collection.data.insert({"text": "one"})
+    collection.data.insert({"text": "two"})
+    res = collection.aggregate.over_all(
+        return_metrics=[Metrics("text").text(min_occurrences=1)],
+    )
+    assert isinstance(res.properties["text"], AggregateText)
+    assert len(res.properties["text"].top_occurrences) == 1
+    assert res.properties["text"].top_occurrences[0].count == 2
+
+
+def test_aggregation_groupby_with_limit(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(properties=[Property(name="text", data_type=DataType.TEXT)])
     collection.data.insert({"text": "one"})
     collection.data.insert({"text": "two"})
     collection.data.insert({"text": "three"})
     res = collection.aggregate.over_all(
         return_metrics=[Metrics("text").text(count=True)],
         group_by=GroupByAggregate(prop="text", limit=2),
@@ -277,30 +295,158 @@
     )
 
 
 @pytest.mark.parametrize(
     "option,expected_len",
     [
         ({"object_limit": 1}, 1),
+        ({"object_limit": 2}, 2),
+    ],
+)
+def test_hybrid_aggregation(
+    collection_factory: CollectionFactory, option: dict, expected_len: int
+) -> None:
+    collection = collection_factory(
+        properties=[Property(name="text", data_type=DataType.TEXT)],
+        vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
+            vectorize_collection_name=False
+        ),
+    )
+    text_1 = "some text"
+    text_2 = "nothing like the other one at all, not even a little bit"
+    uuid = collection.data.insert({"text": text_1})
+    obj = collection.query.fetch_object_by_id(uuid, include_vector=True)
+    assert "default" in obj.vector
+    collection.data.insert({"text": text_2})
+    res: AggregateReturn = collection.aggregate.hybrid(
+        None,
+        alpha=1,
+        vector=obj.vector["default"],
+        return_metrics=[
+            Metrics("text").text(count=True, top_occurrences_count=True, top_occurrences_value=True)
+        ],
+        **option,
+    )
+    assert isinstance(res.properties["text"], AggregateText)
+    assert res.properties["text"].count == expected_len
+    assert len(res.properties["text"].top_occurrences) == expected_len
+    assert text_1 in [
+        top_occurrence.value for top_occurrence in res.properties["text"].top_occurrences
+    ]
+    if expected_len == 2:
+        assert text_2 in [
+            top_occurrence.value for top_occurrence in res.properties["text"].top_occurrences
+        ]
+    else:
+        assert text_2 not in [
+            top_occurrence.value for top_occurrence in res.properties["text"].top_occurrences
+        ]
+
+
+@pytest.mark.parametrize("group_by", ["text", GroupByAggregate(prop="text", limit=1)])
+def test_hybrid_aggregation_group_by(
+    collection_factory: CollectionFactory, group_by: Union[str, GroupByAggregate]
+) -> None:
+    collection = collection_factory(
+        properties=[Property(name="text", data_type=DataType.TEXT)],
+        vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
+            vectorize_collection_name=False
+        ),
+    )
+
+    text_1 = "some text"
+    text_2 = "nothing like the other one at all, not even a little bit"
+    collection.data.insert({"text": text_1})
+    collection.data.insert({"text": text_2})
+
+    querier = lambda: collection.aggregate.hybrid(
+        "text",
+        alpha=0,
+        query_properties=["text"],
+        group_by=group_by,
+        total_count=True,
+        object_limit=2,  # has no effect due to alpha=0
+    )
+    if collection._connection._weaviate_version.is_lower_than(1, 25, 0):
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            querier()
+        return
+
+    res = querier()
+    assert res.groups[0].grouped_by.prop == "text"
+    assert res.groups[0].grouped_by.value == "some text"
+    assert res.groups[0].total_count == 1
+
+
+@pytest.mark.parametrize("group_by", ["text", GroupByAggregate(prop="text", limit=1)])
+def test_hybrid_aggregation_group_by_with_named_vectors(
+    collection_factory: CollectionFactory, group_by: Union[str, GroupByAggregate]
+) -> None:
+    dummy = collection_factory("dummy")
+    collection_maker = lambda: collection_factory(
+        properties=[Property(name="text", data_type=DataType.TEXT)],
+        vectorizer_config=[
+            Configure.NamedVectors.text2vec_contextionary(
+                name="all", vectorize_collection_name=False
+            )
+        ],
+    )
+    if dummy._connection._weaviate_version.is_lower_than(1, 24, 0):
+        with pytest.raises(WeaviateInvalidInputError):
+            collection_maker()
+        return
+
+    collection = collection_maker()
+    text_1 = "some text"
+    text_2 = "nothing like the other one at all, not even a little bit"
+    collection.data.insert({"text": text_1})
+    collection.data.insert({"text": text_2})
+
+    querier = lambda: collection.aggregate.hybrid(
+        "text",
+        alpha=0,
+        query_properties=["text"],
+        group_by=group_by,
+        total_count=True,
+        object_limit=2,  # has no effect due to alpha=0
+        target_vector="all",
+    )
+    if dummy._connection._weaviate_version.is_lower_than(1, 25, 0):
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            querier()
+        return
+
+    res = querier()
+    assert res.groups[0].grouped_by.prop == "text"
+    assert res.groups[0].grouped_by.value == "some text"
+    assert res.groups[0].total_count == 1
+
+
+@pytest.mark.parametrize(
+    "option,expected_len",
+    [
+        ({"object_limit": 1}, 1),
         ({"certainty": 0.9}, 1),
         ({"distance": 0.1}, 1),
         ({"object_limit": 2}, 2),
         ({"certainty": 0.1}, 2),
         ({"distance": 0.9}, 2),
     ],
 )
 def test_near_vector_aggregation(
     collection_factory: CollectionFactory, option: dict, expected_len: int
 ) -> None:
-    collection = collection_factory(
+    collection_maker = lambda: collection_factory(
         properties=[Property(name="text", data_type=DataType.TEXT)],
         vectorizer_config=Configure.Vectorizer.text2vec_contextionary(
             vectorize_collection_name=False
         ),
     )
+
+    collection = collection_maker()
     text_1 = "some text"
     text_2 = "nothing like the other one at all, not even a little bit"
     uuid = collection.data.insert({"text": text_1})
     obj = collection.query.fetch_object_by_id(uuid, include_vector=True)
     assert "default" in obj.vector
     collection.data.insert({"text": text_2})
     res: AggregateReturn = collection.aggregate.near_vector(
```

### Comparing `weaviate-client-4.5rc0/integration/test_collection_batch.py` & `weaviate_client-4.6.0b0/integration/test_collection_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_collection_batch_delete.py` & `weaviate_client-4.6.0b0/integration/test_collection_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_collection_config.py` & `weaviate_client-4.6.0b0/integration/test_collection_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from integration.conftest import OpenAICollection, CollectionFactory
 from integration.conftest import _sanitize_collection_name
 from weaviate.collections.classes.config import (
     _BQConfig,
     _CollectionConfig,
     _CollectionConfigSimple,
     _PQConfig,
+    _VectorIndexConfigDynamic,
+    _VectorIndexConfigFlat,
     _VectorIndexConfigHNSW,
     Configure,
     Reconfigure,
     Property,
     ReferenceProperty,
     DataType,
     PQEncoderType,
@@ -233,27 +235,26 @@
             index_property_length=True,
             index_null_state=True,
             stopwords_additions=["a"],
             stopwords_preset=StopwordsPreset.EN,
             stopwords_removals=["the"],
         ),
         multi_tenancy_config=Configure.multi_tenancy(enabled=True),
-        replication_config=Configure.replication(factor=2),
+        # replication_config=Configure.replication(factor=2), # currently not updateable in RAFT
         vector_index_config=Configure.VectorIndex.hnsw(
             cleanup_interval_seconds=10,
             distance_metric=VectorDistances.DOT,
             dynamic_ef_factor=6,
             dynamic_ef_max=100,
             dynamic_ef_min=10,
             ef=-2,
             ef_construction=100,
             flat_search_cutoff=41000,
             max_connections=72,
             quantizer=Configure.VectorIndex.Quantizer.pq(
-                bit_compression=True,
                 centroids=128,
                 encoder_distribution=PQEncoderDistribution.NORMAL,
                 encoder_type=PQEncoderType.TILE,
                 segments=4,
                 training_limit=1000001,
             ),
             vector_cache_max_objects=100000,
@@ -304,28 +305,28 @@
     assert config.inverted_index_config.index_null_state is True
     # assert config.inverted_index_config.stopwords.additions == ["a"] # potential weaviate bug, this returns as None
     assert config.inverted_index_config.stopwords.preset == StopwordsPreset.EN
     assert config.inverted_index_config.stopwords.removals == ["the"]
 
     assert config.multi_tenancy_config.enabled is True
 
-    assert config.replication_config.factor == 2
+    # assert config.replication_config.factor == 2
 
     assert isinstance(config.vector_index_config, _VectorIndexConfigHNSW)
     assert isinstance(config.vector_index_config.quantizer, _PQConfig)
     assert config.vector_index_config.cleanup_interval_seconds == 10
     assert config.vector_index_config.distance_metric == VectorDistances.DOT
     assert config.vector_index_config.dynamic_ef_factor == 6
     assert config.vector_index_config.dynamic_ef_max == 100
     assert config.vector_index_config.dynamic_ef_min == 10
     assert config.vector_index_config.ef == -2
     assert config.vector_index_config.ef_construction == 100
     assert config.vector_index_config.flat_search_cutoff == 41000
     assert config.vector_index_config.max_connections == 72
-    assert config.vector_index_config.quantizer.bit_compression is True
+    assert config.vector_index_config.quantizer.bit_compression is False
     assert config.vector_index_config.quantizer.centroids == 128
     assert config.vector_index_config.quantizer.encoder.distribution == PQEncoderDistribution.NORMAL
     # assert config.vector_index_config.pq.encoder.type_ == PQEncoderType.TILE # potential weaviate bug, this returns as PQEncoderType.KMEANS
     assert config.vector_index_config.quantizer.segments == 4
     assert config.vector_index_config.quantizer.training_limit == 1000001
     assert config.vector_index_config.skip is False
     assert config.vector_index_config.vector_cache_max_objects == 100000
@@ -336,15 +337,15 @@
 def test_collection_config_update(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(
         vectorizer_config=Configure.Vectorizer.none(),
         properties=[
             Property(name="name", data_type=DataType.TEXT),
             Property(name="age", data_type=DataType.INT),
         ],
-        ports=(8087, 50051),
+        ports=(8087, 50058),
     )
     config = collection.config.get()
 
     assert config.replication_config.factor == 1
 
     collection.config.update(
         description="Test",
@@ -352,52 +353,51 @@
             bm25_b=0.8,
             bm25_k1=1.25,
             cleanup_interval_seconds=10,
             stopwords_additions=["a"],
             stopwords_preset=StopwordsPreset.EN,
             stopwords_removals=["the"],
         ),
-        replication_config=Reconfigure.replication(factor=2),
+        # replication_config=Reconfigure.replication(factor=2), # currently not updateable in RAFT
         vectorizer_config=Reconfigure.VectorIndex.hnsw(
             vector_cache_max_objects=2000000,
             quantizer=Reconfigure.VectorIndex.Quantizer.pq(
-                bit_compression=True,
                 centroids=128,
                 encoder_type=PQEncoderType.TILE,
                 encoder_distribution=PQEncoderDistribution.NORMAL,
                 segments=4,
                 training_limit=100001,
             ),
         ),
     )
 
     config = collection.config.get()
 
-    assert config.description == "Test"
+    # assert config.description == "Test"
 
     assert config.inverted_index_config.bm25.b == 0.8
     assert config.inverted_index_config.bm25.k1 == 1.25
     assert config.inverted_index_config.cleanup_interval_seconds == 10
     # assert config.inverted_index_config.stopwords.additions is ["a"] # potential weaviate bug, this returns as None
     assert config.inverted_index_config.stopwords.removals == ["the"]
 
-    assert config.replication_config.factor == 2
+    # assert config.replication_config.factor == 2
 
     assert isinstance(config.vector_index_config, _VectorIndexConfigHNSW)
     assert isinstance(config.vector_index_config.quantizer, _PQConfig)
     assert config.vector_index_config.cleanup_interval_seconds == 300
     assert config.vector_index_config.distance_metric == VectorDistances.COSINE
     assert config.vector_index_config.dynamic_ef_factor == 8
     assert config.vector_index_config.dynamic_ef_max == 500
     assert config.vector_index_config.dynamic_ef_min == 100
     assert config.vector_index_config.ef == -1
     assert config.vector_index_config.ef_construction == 128
     assert config.vector_index_config.flat_search_cutoff == 40000
     assert config.vector_index_config.max_connections == 64
-    assert config.vector_index_config.quantizer.bit_compression is True
+    assert config.vector_index_config.quantizer.bit_compression is False
     assert config.vector_index_config.quantizer.centroids == 128
     assert config.vector_index_config.quantizer.encoder.type_ == PQEncoderType.TILE
     assert config.vector_index_config.quantizer.encoder.distribution == PQEncoderDistribution.NORMAL
     assert config.vector_index_config.quantizer.segments == 4
     assert config.vector_index_config.quantizer.training_limit == 100001
     assert config.vector_index_config.skip is False
     assert config.vector_index_config.vector_cache_max_objects == 2000000
@@ -406,23 +406,24 @@
 
     collection.config.update(
         vectorizer_config=Reconfigure.VectorIndex.hnsw(
             quantizer=Reconfigure.VectorIndex.Quantizer.pq(enabled=False),
         )
     )
     config = collection.config.get()
-    assert config.description == "Test"
+
+    # assert config.description == "Test"
 
     assert config.inverted_index_config.bm25.b == 0.8
     assert config.inverted_index_config.bm25.k1 == 1.25
     assert config.inverted_index_config.cleanup_interval_seconds == 10
     # assert config.inverted_index_config.stopwords.additions is ["a"] # potential weaviate bug, this returns as None
     assert config.inverted_index_config.stopwords.removals == ["the"]
 
-    assert config.replication_config.factor == 2
+    # assert config.replication_config.factor == 2
 
     assert isinstance(config.vector_index_config, _VectorIndexConfigHNSW)
     assert config.vector_index_config.cleanup_interval_seconds == 300
     assert config.vector_index_config.distance_metric == VectorDistances.COSINE
     assert config.vector_index_config.dynamic_ef_factor == 8
     assert config.vector_index_config.dynamic_ef_max == 500
     assert config.vector_index_config.dynamic_ef_min == 100
@@ -460,27 +461,29 @@
             quantizer=Configure.VectorIndex.Quantizer.bq(rescore_limit=10),
         ),
     )
 
     config = collection.config.get()
     assert config.vector_index_type == VectorIndexType.FLAT
     assert config.vector_index_config is not None
+    assert isinstance(config.vector_index_config, _VectorIndexConfigFlat)
     assert config.vector_index_config.vector_cache_max_objects == 5
     assert isinstance(config.vector_index_config.quantizer, _BQConfig)
     assert config.vector_index_config.quantizer.rescore_limit == 10
 
     collection.config.update(
         vectorizer_config=Reconfigure.VectorIndex.flat(
             vector_cache_max_objects=10,
             quantizer=Reconfigure.VectorIndex.Quantizer.bq(rescore_limit=20),
         ),
     )
     config = collection.config.get()
     assert config.vector_index_type == VectorIndexType.FLAT
     assert config.vector_index_config is not None
+    assert isinstance(config.vector_index_config, _VectorIndexConfigFlat)
     assert config.vector_index_config.vector_cache_max_objects == 10
     assert isinstance(config.vector_index_config.quantizer, _BQConfig)
     assert config.vector_index_config.quantizer.rescore_limit == 20
 
     # Cannot currently disabled BQ after it has been enabled
     # collection.config.update(
     #     vectorizer_config=Reconfigure.VectorIndex.flat(
@@ -567,14 +570,15 @@
             quantizer=Configure.VectorIndex.Quantizer.bq(rescore_limit=456),
         ),
     )
 
     conf = collection.config.get()
     assert conf.vector_index_type == VectorIndexType.FLAT
     assert conf.vector_index_config is not None
+    assert isinstance(conf.vector_index_config, _VectorIndexConfigFlat)
     assert conf.vector_index_config.vector_cache_max_objects == 234
     assert isinstance(conf.vector_index_config.quantizer, _BQConfig)
     assert conf.vector_index_config.quantizer.rescore_limit == 456
 
 
 def test_config_vector_index_hnsw_and_quantizer_pq(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(
@@ -584,16 +588,16 @@
             quantizer=Configure.VectorIndex.Quantizer.pq(segments=456),
         ),
     )
 
     conf = collection.config.get()
     assert conf.vector_index_type == VectorIndexType.HNSW
     assert conf.vector_index_config is not None
-    assert conf.vector_index_config.vector_cache_max_objects == 234
     assert isinstance(conf.vector_index_config, _VectorIndexConfigHNSW)
+    assert conf.vector_index_config.vector_cache_max_objects == 234
     assert conf.vector_index_config.ef_construction == 789
     assert isinstance(conf.vector_index_config.quantizer, _PQConfig)
     assert conf.vector_index_config.quantizer.segments == 456
 
 
 @pytest.mark.parametrize(
     "reranker_config,expected_reranker,expected_model",
@@ -739,7 +743,33 @@
     assert config.vector_index_config.ef == -1
     assert config.vector_index_config.ef_construction == 128
     assert config.vector_index_config.flat_search_cutoff == 40000
     assert config.vector_index_config.max_connections == 64
     assert config.vector_index_config.quantizer is None
     assert config.vector_index_config.skip is True
     assert config.vector_index_config.vector_cache_max_objects == 1000000000000
+
+
+def test_dynamic_collection(collection_factory: CollectionFactory) -> None:
+    collection_dummy = collection_factory("dummy")
+    if collection_dummy._connection._weaviate_version.is_lower_than(1, 25, 0):
+        pytest.skip("Dynamic index is not supported in Weaviate versions lower than 1.25.0")
+
+    collection = collection_factory(
+        vector_index_config=Configure.VectorIndex.dynamic(
+            distance_metric=VectorDistances.COSINE,
+            threshold=1000,
+            hnsw=Configure.VectorIndex.hnsw(cleanup_interval_seconds=123, flat_search_cutoff=1234),
+            flat=Configure.VectorIndex.flat(vector_cache_max_objects=7643),
+        ),
+        ports=(8090, 50061),
+    )
+
+    config = collection.config.get()
+    assert isinstance(config.vector_index_config, _VectorIndexConfigDynamic)
+    assert config.vector_index_config.distance_metric == VectorDistances.COSINE
+    assert config.vector_index_config.threshold == 1000
+    assert isinstance(config.vector_index_config.hnsw, _VectorIndexConfigHNSW)
+    assert config.vector_index_config.hnsw.cleanup_interval_seconds == 123
+    assert config.vector_index_config.hnsw.flat_search_cutoff == 1234
+    assert isinstance(config.vector_index_config.flat, _VectorIndexConfigFlat)
+    assert config.vector_index_config.flat.vector_cache_max_objects == 7643
```

### Comparing `weaviate-client-4.5rc0/integration/test_collection_filter.py` & `weaviate_client-4.6.0b0/integration/test_collection_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_collection_geo.py` & `weaviate_client-4.6.0b0/integration/test_collection_geo.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_collection_get.py` & `weaviate_client-4.6.0b0/integration/test_collection_get.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_collection_model.py` & `weaviate_client-4.6.0b0/integration/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_collection_multi_node.py` & `weaviate_client-4.6.0b0/integration/test_collection_multi_node.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_collection_nested.py` & `weaviate_client-4.6.0b0/integration/test_collection_nested.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_collection_openai.py` & `weaviate_client-4.6.0b0/integration/test_collection_openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from weaviate.collections.classes.config import (
     Configure,
     DataType,
     Property,
 )
 from weaviate.collections.classes.data import DataObject
 from weaviate.collections.classes.grpc import GroupBy, Rerank
-from weaviate.exceptions import WeaviateQueryError
+from weaviate.exceptions import WeaviateQueryError, WeaviateUnsupportedFeatureError
 from weaviate.util import _ServerVersion
 
 
 @pytest.mark.parametrize("parameter,answer", [("text", "yes"), ("content", "no")])
 def test_generative_search_single(
     openai_collection: OpenAICollection, parameter: str, answer: str
 ) -> None:
@@ -176,14 +176,60 @@
         grouped_task="What is the biggest and what is the smallest? Only write the names separated by a space",
     )
     assert res.generated == "Teddy apples"
     for obj in res.objects:
         assert obj.generated == "Yes"
 
 
+def test_bm25_generate_and_group_by_with_everything(
+    openai_collection: OpenAICollection, request: SubRequest
+) -> None:
+    collection = openai_collection()
+
+    collection.data.insert_many(
+        [
+            DataObject(
+                properties={
+                    "text": "apples are big",
+                    "content": "Teddy is the biggest and bigger than everything else",
+                }
+            ),
+            DataObject(
+                properties={
+                    "text": "bananas are small",
+                    "content": "cats are the smallest and smaller than everything else",
+                }
+            ),
+        ]
+    )
+
+    if collection._connection.supports_groupby_in_bm25_and_hybrid():
+        res = collection.generate.bm25(
+            query="Teddy",
+            query_properties=["content"],
+            single_prompt="Is there something to eat in {text}? Only answer yes if there is something to eat or no if not without punctuation",
+            grouped_task="What is the biggest and what is the smallest? Only write the names separated by a space",
+            group_by=GroupBy(prop="text", number_of_groups=2, objects_per_group=1),
+        )
+        assert res.generated == "Teddy apples"
+        assert len(res.groups) == 1
+        groups = list(res.groups.values())
+        assert groups[0].generated == "Yes"
+        assert res.objects[0].belongs_to_group == "apples are big"
+    else:
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            collection.generate.bm25(
+                query="Teddy",
+                query_properties=["content"],
+                single_prompt="Is there something to eat in {text}? Only answer yes if there is something to eat or no if not without punctuation",
+                grouped_task="What is the biggest and what is the smallest? Only write the names separated by a space",
+                group_by=GroupBy(prop="text", number_of_groups=2, objects_per_group=1),
+            )
+
+
 def test_hybrid_generate_with_everything(
     openai_collection: OpenAICollection, request: SubRequest
 ) -> None:
     collection = openai_collection()
 
     collection.data.insert_many(
         [
@@ -211,14 +257,62 @@
     )
     assert res.generated == "cats bananas"
     for obj in res.objects:
         assert obj.generated is not None
         assert obj.generated.lower() == "yes"
 
 
+def test_hybrid_generate_and_group_by_with_everything(
+    openai_collection: OpenAICollection, request: SubRequest
+) -> None:
+    collection = openai_collection()
+
+    collection.data.insert_many(
+        [
+            DataObject(
+                properties={
+                    "text": "apples are big",
+                    "content": "Teddy is the biggest and bigger than everything else",
+                }
+            ),
+            DataObject(
+                properties={
+                    "text": "bananas are small",
+                    "content": "cats are the smallest and smaller than everything else",
+                }
+            ),
+        ]
+    )
+
+    if collection._connection.supports_groupby_in_bm25_and_hybrid():
+        res = collection.generate.hybrid(
+            query="Teddy",
+            alpha=0,
+            query_properties=["content"],
+            single_prompt="Is there something to eat in {text}? Only answer yes if there is something to eat or no if not without punctuation",
+            grouped_task="What is the biggest and what is the smallest? Only write the names separated by a space",
+            group_by=GroupBy(prop="text", number_of_groups=2, objects_per_group=1),
+        )
+        assert res.generated == "Teddy apples"
+        assert len(res.groups) == 1
+        groups = list(res.groups.values())
+        assert groups[0].generated == "Yes"
+        assert res.objects[0].belongs_to_group == "apples are big"
+    else:
+        with pytest.raises(WeaviateUnsupportedFeatureError):
+            collection.generate.hybrid(
+                query="Teddy",
+                alpha=0,
+                query_properties=["content"],
+                single_prompt="Is there something to eat in {text}? Only answer yes if there is something to eat or no if not without punctuation",
+                grouped_task="What is the biggest and what is the smallest? Only write the names separated by a space",
+                group_by=GroupBy(prop="text", number_of_groups=2, objects_per_group=1),
+            )
+
+
 def test_near_object_generate_with_everything(openai_collection: OpenAICollection) -> None:
     collection = openai_collection(
         vectorizer_config=Configure.Vectorizer.text2vec_openai(vectorize_collection_name=False),
     )
 
     ret = collection.data.insert_many(
         [
```

### Comparing `weaviate-client-4.5rc0/integration/test_collection_references.py` & `weaviate_client-4.6.0b0/integration/test_collection_references.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_collection_rerank.py` & `weaviate_client-4.6.0b0/integration/test_collection_rerank.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_gql_raw_v4.py` & `weaviate_client-4.6.0b0/integration/test_gql_raw_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration/test_iterator.py` & `weaviate_client-4.6.0b0/integration/test_iterator.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,7 +199,24 @@
         ret: list[int] = [obj.properties["data"] for obj in collection.iterator()]
         if first_order is None:
             first_order = ret
         else:
             assert first_order == ret
 
         assert sorted(ret) == expected
+
+
+def test_iterator_with_after(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory(
+        properties=[Property(name="data", data_type=DataType.INT)],
+        vectorizer_config=Configure.Vectorizer.none(),
+        data_model_properties=Dict[str, int],
+    )
+
+    collection.data.insert_many([DataObject(properties={"data": i}) for i in range(10)])
+
+    uuids = [obj.uuid for obj in collection.iterator()]
+    iterator = collection.iterator(after=uuids[5])
+    assert (
+        next(iterator).properties["data"]
+        == collection.query.fetch_object_by_id(uuids[6]).properties["data"]
+    )
```

### Comparing `weaviate-client-4.5rc0/integration/test_named_vectors.py` & `weaviate_client-4.6.0b0/integration/test_named_vectors.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from integration.conftest import CollectionFactory, OpenAICollection
 import pytest
 import weaviate.classes as wvc
 
 from weaviate.collections.classes.data import DataObject
 
 from weaviate.collections.classes.config import (
+    PQConfig,
     _VectorIndexConfigFlat,
     Vectorizers,
 )
 
 from weaviate.collections.classes.aggregate import AggregateInteger
 
 from weaviate.exceptions import WeaviateInvalidInputError
@@ -129,14 +130,85 @@
     obj = collection.query.fetch_object_by_id(
         batch_return.uuids[0], include_vector=["title", "bringYourOwn"]
     )
     assert obj.vector["title"] is not None
     assert obj.vector["bringYourOwn"] == [0.5, 0.25, 0.75]
 
 
+def test_update(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory("dummy")
+    if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
+        pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
+
+    collection = collection_factory(
+        properties=[
+            wvc.config.Property(name="title", data_type=wvc.config.DataType.TEXT),
+            wvc.config.Property(name="content", data_type=wvc.config.DataType.TEXT),
+        ],
+        vectorizer_config=[
+            wvc.config.Configure.NamedVectors.none(name="bringYourOwn"),
+        ],
+    )
+
+    uuid = collection.data.insert(
+        properties={"title": "Hello", "content": "World"},
+        vector={
+            "bringYourOwn": [0.5, 0.25, 0.75],
+        },
+    )
+    assert collection.query.fetch_object_by_id(uuid, include_vector=True).vector[
+        "bringYourOwn"
+    ] == [0.5, 0.25, 0.75]
+    collection.data.update(
+        uuid,
+        vector={
+            "bringYourOwn": [0.375, 0.625, 0.875],
+        },
+    )
+    assert collection.query.fetch_object_by_id(uuid, include_vector=True).vector[
+        "bringYourOwn"
+    ] == [0.375, 0.625, 0.875]
+
+
+def test_replace(collection_factory: CollectionFactory) -> None:
+    collection = collection_factory("dummy")
+    if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
+        pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
+
+    collection = collection_factory(
+        properties=[
+            wvc.config.Property(name="title", data_type=wvc.config.DataType.TEXT),
+            wvc.config.Property(name="content", data_type=wvc.config.DataType.TEXT),
+        ],
+        vectorizer_config=[
+            wvc.config.Configure.NamedVectors.none(name="bringYourOwn"),
+        ],
+    )
+
+    uuid = collection.data.insert(
+        properties={"title": "Hello", "content": "World"},
+        vector={
+            "bringYourOwn": [0.5, 0.25, 0.75],
+        },
+    )
+    assert collection.query.fetch_object_by_id(uuid, include_vector=True).vector[
+        "bringYourOwn"
+    ] == [0.5, 0.25, 0.75]
+    collection.data.replace(
+        uuid,
+        properties={"title": "Hello", "content": "World"},
+        vector={
+            "bringYourOwn": [0.375, 0.625, 0.875],
+        },
+    )
+    assert collection.query.fetch_object_by_id(uuid, include_vector=True).vector[
+        "bringYourOwn"
+    ] == [0.375, 0.625, 0.875]
+
+
 def test_query(collection_factory: CollectionFactory) -> None:
     collection = collection_factory("dummy")
     if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
         pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
     collection = collection_factory(
         properties=[
             wvc.config.Property(name="title", data_type=wvc.config.DataType.TEXT),
@@ -370,61 +442,60 @@
         return_metrics=wvc.aggregate.Metrics("number").integer(),
     )
     assert isinstance(agg.properties["number"], AggregateInteger)
     assert agg.properties["number"].sum_ == 1
     assert agg.properties["number"].minimum == 1
 
 
-# def test_update_to_enable_quantizer_on_specific_named_vector(
-#     collection_factory: CollectionFactory,
-# ) -> None:
-#     collection = collection_factory("dummy")
-#     if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
-#         pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
-#     collection = collection_factory(
-#         properties=[
-#             wvc.config.Property(name="first", data_type=wvc.config.DataType.TEXT),
-#             wvc.config.Property(name="second", data_type=wvc.config.DataType.TEXT),
-#         ],
-#         vectorizer_config=[
-#             wvc.config.Configure.NamedVectors.text2vec_contextionary(
-#                 "first",
-#                 source_properties=["first"],
-#                 vectorize_collection_name=False,
-#             ),
-#             wvc.config.Configure.NamedVectors.text2vec_contextionary(
-#                 "second",
-#                 source_properties=["second"],
-#                 vectorize_collection_name=False,
-#             ),
-#         ],
-#     )
-
-#     config = collection.config.get()
-#     assert config.vector_config is not None
-#     assert config.vector_config["first"].vector_index_config is not None
-#     assert config.vector_config["second"].vector_index_config is not None
-#     assert config.vector_config["second"].vector_index_config.quantizer is None
-
-#     collection.config.update(
-#         vectorizer_config=[
-#             wvc.config.Reconfigure.NamedVectors.update(
-#                 name="second",
-#                 vector_index_config=wvc.config.Reconfigure.VectorIndex.hnsw(
-#                     quantizer=wvc.config.Reconfigure.VectorIndex.Quantizer.pq(bit_compression=True)
-#                 ),
-#             )
-#         ]
-#     )
-#     config = collection.config.get()
-#     assert config.vector_config is not None
-#     assert config.vector_config["first"].vector_index_config is not None
-#     assert config.vector_config["second"].vector_index_config is not None
-#     assert isinstance(config.vector_config["second"].vector_index_config.quantizer, PQConfig)
-#     assert config.vector_config["second"].vector_index_config.quantizer.bit_compression is True
+def test_update_to_enable_quantizer_on_specific_named_vector(
+    collection_factory: CollectionFactory,
+) -> None:
+    collection = collection_factory("dummy")
+    if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
+        pytest.skip("Named vectors are not supported in versions lower than 1.24.0")
+    collection = collection_factory(
+        properties=[
+            wvc.config.Property(name="first", data_type=wvc.config.DataType.TEXT),
+            wvc.config.Property(name="second", data_type=wvc.config.DataType.TEXT),
+        ],
+        vectorizer_config=[
+            wvc.config.Configure.NamedVectors.text2vec_contextionary(
+                "first",
+                source_properties=["first"],
+                vectorize_collection_name=False,
+            ),
+            wvc.config.Configure.NamedVectors.text2vec_contextionary(
+                "second",
+                source_properties=["second"],
+                vectorize_collection_name=False,
+            ),
+        ],
+    )
+    config = collection.config.get()
+    assert config.vector_config is not None
+    assert config.vector_config["first"].vector_index_config is not None
+    assert config.vector_config["second"].vector_index_config is not None
+    assert config.vector_config["second"].vector_index_config.quantizer is None
+
+    collection.config.update(
+        vectorizer_config=[
+            wvc.config.Reconfigure.NamedVectors.update(
+                name="second",
+                vector_index_config=wvc.config.Reconfigure.VectorIndex.hnsw(
+                    quantizer=wvc.config.Reconfigure.VectorIndex.Quantizer.pq()
+                ),
+            )
+        ]
+    )
+    config = collection.config.get()
+    assert config.vector_config is not None
+    assert config.vector_config["first"].vector_index_config is not None
+    assert config.vector_config["second"].vector_index_config is not None
+    assert isinstance(config.vector_config["second"].vector_index_config.quantizer, PQConfig)
+    assert config.vector_config["second"].vector_index_config.quantizer.centroids == 256
 
 
 # def test_update_to_change_quantizer_from_pq_to_bq_on_specific_named_vector(
 #     collection_factory: CollectionFactory,
 # ) -> None:
 #     collection = collection_factory("dummy")
 #     if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
```

### Comparing `weaviate-client-4.5rc0/integration/weaviate-logo.png` & `weaviate_client-4.6.0b0/integration/weaviate-logo.png`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/people_schema.json` & `weaviate_client-4.6.0b0/integration_v3/people_schema.json`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/test_authentication.py` & `weaviate_client-4.6.0b0/integration_v3/test_authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/test_backup.py` & `weaviate_client-4.6.0b0/integration_v3/test_backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,16 +286,16 @@
     with pytest.raises(UnexpectedStatusCodeException) as excinfo:
         client.backup.create(
             backup_id=backup_id,
             include_classes=class_name,
             backend=BACKEND,
             wait_for_completion=True,
         )
-        assert backup_id in str(excinfo.value)
-        assert "422" in str(excinfo.value)
+    assert backup_id in str(excinfo.value)
+    assert "422" in str(excinfo.value)
 
 
 def test_fail_restoring_non_existing_backup(client: weaviate.Client):
     """fail restoring non-existing backup"""
     backup_id = _create_backup_id()
     with pytest.raises(UnexpectedStatusCodeException) as excinfo:
         client.backup.restore(backup_id=backup_id, backend=BACKEND, wait_for_completion=True)
```

### Comparing `weaviate-client-4.5rc0/integration_v3/test_backup_v4.py` & `weaviate_client-4.6.0b0/integration_v3/test_backup_v4.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 import datetime
 import time
 from typing import Generator, List, Union
 
 import pytest
 
 import weaviate
-from weaviate.backup.backup import BackupStatus, BackupStorage
+from weaviate.backup.backup import (
+    BackupCompressionLevel,
+    BackupConfigCreate,
+    BackupConfigRestore,
+    BackupStatus,
+    BackupStorage,
+)
 from weaviate.collections.classes.config import DataType, Property, ReferenceProperty
-from weaviate.exceptions import UnexpectedStatusCodeException, BackupFailedException
+from weaviate.exceptions import (
+    WeaviateUnsupportedFeatureError,
+    UnexpectedStatusCodeException,
+    BackupFailedException,
+)
 
 BACKEND = BackupStorage.FILESYSTEM
 
 PARAGRAPHS_IDS = [
     "fd34ccf4-1a2a-47ad-8446-231839366c3f",
     "2653442b-05d8-4fa3-b46a-d4a152eb63bc",
     "55374edb-17de-487f-86cb-9a9fbc30823f",
@@ -357,7 +367,85 @@
 
     # # check data exists again
     assert len(article) == len(ARTICLES_IDS)
 
     # check restore status
     restore_status = article.backup.get_restore_status(backup_id, BACKEND)
     assert restore_status.status == BackupStatus.SUCCESS
+
+
+def test_backup_and_restore_with_collection_and_config_1_24_x(
+    client: weaviate.WeaviateClient,
+) -> None:
+    if client._connection._weaviate_version.is_lower_than(1, 25, 0):
+        pytest.skip("Backup config is only supported from Weaviate 1.25.0")
+
+    backup_id = _create_backup_id()
+
+    article = client.collections.get("Article")
+
+    # create backup
+    create = article.backup.create(
+        backup_id=backup_id,
+        backend=BACKEND,
+        wait_for_completion=True,
+        config=BackupConfigCreate(
+            cpu_percentage=60, chunk_size=256, compression_level=BackupCompressionLevel.BEST_SPEED
+        ),
+    )
+    assert create.status == BackupStatus.SUCCESS
+
+    assert len(article) == len(ARTICLES_IDS)
+
+    # check create status
+    create_status = article.backup.get_create_status(backup_id, BACKEND)
+    assert create_status.status == BackupStatus.SUCCESS
+
+    # remove existing class
+    client.collections.delete("Article")
+
+    # restore backup
+    restore = article.backup.restore(
+        backup_id=backup_id,
+        backend=BACKEND,
+        wait_for_completion=True,
+        config=BackupConfigRestore(cpu_percentage=70),
+    )
+    assert restore.status == BackupStatus.SUCCESS
+
+    # # check data exists again
+    assert len(article) == len(ARTICLES_IDS)
+
+    # check restore status
+    restore_status = article.backup.get_restore_status(backup_id, BACKEND)
+    assert restore_status.status == BackupStatus.SUCCESS
+
+
+def test_backup_and_restore_with_collection_and_config_1_23_x(
+    client: weaviate.WeaviateClient,
+) -> None:
+    if client._connection._weaviate_version.is_at_least(1, 24, 0):
+        pytest.skip("Backup config is supported from Weaviate 1.24.0")
+
+    backup_id = _create_backup_id()
+
+    article = client.collections.get("Article")
+
+    with pytest.raises(WeaviateUnsupportedFeatureError):
+        article.backup.create(
+            backup_id=backup_id,
+            backend=BACKEND,
+            wait_for_completion=True,
+            config=BackupConfigCreate(
+                cpu_percentage=60,
+                chunk_size=256,
+                compression_level=BackupCompressionLevel.BEST_SPEED,
+            ),
+        )
+
+    with pytest.raises(WeaviateUnsupportedFeatureError):
+        article.backup.restore(
+            backup_id=backup_id,
+            backend=BACKEND,
+            wait_for_completion=True,
+            config=BackupConfigRestore(cpu_percentage=70),
+        )
```

### Comparing `weaviate-client-4.5rc0/integration_v3/test_batch.py` & `weaviate_client-4.6.0b0/integration_v3/test_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,15 +546,15 @@
             batch.add_data_object(
                 class_name="BatchTestAsync",
                 data_object={"text": "text" + str(i)},
                 vector=[float((j + i) % nr_objects) / nr_objects for j in range(nr_objects)],
             )
     shard_status = client.schema.get_class_shards("BatchTestAsync")
     assert shard_status[0]["status"] == "INDEXING"
-    assert shard_status[0]["vectorQueueSize"] > 0
+    assert shard_status[0]["vectorQueueSize"] >= 0
     res = client.query.aggregate("BatchTestAsync").with_meta_count().do()
     assert res["data"]["Aggregate"]["BatchTestAsync"][0]["meta"]["count"] == nr_objects
 
 
 def test_add_2000_tenant_objects_with_async_indexing_and_wait_for_all():
     client = weaviate.Client("http://localhost:8090")
     client.schema.delete_all()
@@ -645,8 +645,8 @@
         )
     for shard in client.schema.get_class_shards("BatchTestAsync"):
         if shard["name"] == tenants[0].name:
             assert shard["status"] == "READY"
             assert shard["vectorQueueSize"] == 0
         else:
             assert shard["status"] == "INDEXING"
-            assert shard["vectorQueueSize"] > 0
+            assert shard["vectorQueueSize"] >= 0
```

### Comparing `weaviate-client-4.5rc0/integration_v3/test_classification.py` & `weaviate_client-4.6.0b0/integration_v3/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/test_cluster.py` & `weaviate_client-4.6.0b0/integration_v3/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/test_crud.py` & `weaviate_client-4.6.0b0/integration_v3/test_crud.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/test_graphql.py` & `weaviate_client-4.6.0b0/integration_v3/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/test_grcp.py` & `weaviate_client-4.6.0b0/integration_v3/test_grcp.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/test_schema.py` & `weaviate_client-4.6.0b0/integration_v3/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/test_stress.py` & `weaviate_client-4.6.0b0/integration_v3/test_stress.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/integration_v3/test_timeout.py` & `weaviate_client-4.6.0b0/integration_v3/test_timeout.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/mock_tests/conftest.py` & `weaviate_client-4.6.0b0/mock_tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     ready_mock.expect_request("/v1/nodes").respond_with_json({"nodes": [{"gitHash": "ABC"}]})
 
     yield ready_mock
 
 
 @pytest.fixture(scope="function")
 def weaviate_no_auth_mock(ready_mock):
-    ready_mock.expect_request("/v1/meta").respond_with_json({"version": "1.16"})
+    ready_mock.expect_request("/v1/meta").respond_with_json({"version": "1.25"})
     ready_mock.expect_request("/v1/.well-known/openid-configuration").respond_with_response(
         Response(json.dumps({}), status=404)
     )
 
     yield ready_mock
```

### Comparing `weaviate-client-4.5rc0/mock_tests/test_auth.py` & `weaviate_client-4.6.0b0/mock_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/mock_tests/test_automatic_retries.py` & `weaviate_client-4.6.0b0/mock_tests/test_automatic_retries.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/mock_tests/test_batching_manual.py` & `weaviate_client-4.6.0b0/mock_tests/test_batching_manual.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/mock_tests/test_collection.py` & `weaviate_client-4.6.0b0/mock_tests/test_collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from datetime import datetime
 import json
 import time
 from typing import Any, Dict
 import grpc
 from werkzeug import Request, Response
 
 import pytest
 from pytest_httpserver import HTTPServer
 
 import weaviate
-from mock_tests.conftest import MOCK_SERVER_URL, MOCK_PORT, MOCK_IP, MOCK_PORT_GRPC, CLIENT_ID
+from mock_tests.conftest import MOCK_PORT, MOCK_IP, MOCK_PORT_GRPC, CLIENT_ID
 from weaviate.collections.classes.config import (
     CollectionConfig,
     VectorIndexConfigFlat,
     VectorDistances,
     InvertedIndexConfig,
     MultiTenancyConfig,
     BM25Config,
@@ -26,37 +25,21 @@
 )
 
 from weaviate.exceptions import UnexpectedStatusCodeError, WeaviateStartUpError
 import weaviate.classes as wvc
 
 from weaviate.connect.base import ConnectionParams, ProtocolParams
 
+from weaviate.connect.integrations import _IntegrationConfig
+
 
 ACCESS_TOKEN = "HELLO!IamAnAccessToken"
 REFRESH_TOKEN = "UseMeToRefreshYourAccessToken"
 
 
-@pytest.mark.skip(reason="Fails with gRPC not enabled error")
-def test_warning_old_weaviate(recwarn: pytest.WarningsRecorder, ready_mock: HTTPServer) -> None:
-    ready_mock.expect_request("/v1/meta").respond_with_json({"version": "1.21.0"})
-    ready_mock.expect_request("/v1/objects").respond_with_json({})
-
-    client = weaviate.WeaviateClient(MOCK_SERVER_URL)
-    client.collections.get("Class").data.insert(
-        {
-            "date": datetime.now(),
-        }
-    )
-
-    assert len(recwarn) == 1
-    w = recwarn.pop()
-    assert issubclass(w.category, UserWarning)
-    assert str(w.message).startswith("Con002")
-
-
 def test_status_code_exception(weaviate_mock: HTTPServer, start_grpc_server: grpc.Server) -> None:
     weaviate_mock.expect_request("/v1/schema/Test").respond_with_json(response_json={}, status=403)
 
     client = weaviate.connect_to_local(
         port=MOCK_PORT, host=MOCK_IP, grpc_port=MOCK_PORT_GRPC, skip_init_checks=True
     )
     collection = client.collections.get("Test")
@@ -182,15 +165,15 @@
             bm25=BM25Config(b=0, k1=0),
             cleanup_interval_seconds=0,
             index_null_state=False,
             index_property_length=False,
             index_timestamps=False,
             stopwords=StopwordsConfig(preset=StopwordsPreset.NONE, additions=[], removals=[]),
         ),
-        multi_tenancy_config=MultiTenancyConfig(enabled=True),
+        multi_tenancy_config=MultiTenancyConfig(enabled=True, auto_tenant_creation=False),
         sharding_config=ShardingConfig(
             virtual_per_physical=0,
             desired_count=0,
             actual_count=0,
             desired_virtual_count=0,
             actual_virtual_count=0,
             key="",
@@ -272,7 +255,89 @@
     )
     collection = client.collections.get("TestBindCollection")
     conf = collection.config.get()
 
     assert conf.properties[0].vectorizer_config is not None
     assert not conf.properties[0].vectorizer_config.skip
     assert not conf.properties[0].vectorizer_config.vectorize_property_name
+
+
+@pytest.mark.parametrize(
+    "integrations,headers",
+    [
+        (wvc.init.Integrations.cohere(api_key="key"), {"X-Cohere-Api-Key": "key"}),
+        (
+            wvc.init.Integrations.cohere(
+                api_key="key", request_per_minute_embeddings=50, base_url="http://some-url.com"
+            ),
+            {
+                "X-Cohere-Api-Key": "key",
+                "X-Cohere-Ratelimit-RequestPM-Embedding": "50",
+                "X-Cohere-Baseurl": "http://some-url.com",
+            },
+        ),
+        ([wvc.init.Integrations.cohere(api_key="key")], {"X-Cohere-Api-Key": "key"}),
+        (
+            [
+                wvc.init.Integrations.cohere(api_key="key"),
+                wvc.init.Integrations.openai(api_key="key2"),
+            ],
+            {"X-Cohere-Api-Key": "key", "X-Openai-Api-Key": "key2"},
+        ),
+        (
+            [
+                wvc.init.Integrations.voyageai(
+                    api_key="key", base_url="http://some-url.com", request_per_minute_embeddings=50
+                )
+            ],
+            {
+                "X-Voyageai-Api-Key": "key",
+                "X-Voyageai-Ratelimit-RequestPM-Embedding": "50",
+                "X-Voyageai-Baseurl": "http://some-url.com",
+            },
+        ),
+        (
+            [
+                wvc.init.Integrations.jinaai(
+                    api_key="key", base_url="http://some-url.com", request_per_minute_embeddings=50
+                )
+            ],
+            {
+                "X-Jinaai-Api-Key": "key",
+                "X-Jinaai-Ratelimit-RequestPM-Embedding": "50",
+                "X-Jinaai-Baseurl": "http://some-url.com",
+            },
+        ),
+        (
+            [
+                wvc.init.Integrations.octoai(
+                    api_key="key", base_url="http://some-url.com", request_per_minute_embeddings=50
+                )
+            ],
+            {
+                "X-Octoai-Api-Key": "key",
+                "X-Octoai-Ratelimit-RequestPM-Embedding": "50",
+                "X-Octoai-Baseurl": "http://some-url.com",
+            },
+        ),
+    ],
+)
+def test_integration_config(
+    weaviate_no_auth_mock: HTTPServer,
+    start_grpc_server: grpc.Server,
+    integrations: _IntegrationConfig,
+    headers: Dict[str, Any],
+) -> None:
+    client = weaviate.connect_to_local(
+        port=MOCK_PORT,
+        host=MOCK_IP,
+        grpc_port=MOCK_PORT_GRPC,
+    )
+
+    client.integrations.configure(integrations)
+
+    weaviate_no_auth_mock.expect_request("/v1/schema", headers=headers).respond_with_json(
+        status=200, response_json={"classes": []}
+    )
+
+    client.collections.list_all()  # return is irrelevant
+    weaviate_no_auth_mock.check_assertions()
```

### Comparing `weaviate-client-4.5rc0/mock_tests/test_connection.py` & `weaviate_client-4.6.0b0/mock_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/mock_tests/test_exception.py` & `weaviate_client-4.6.0b0/mock_tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/mock_tests/test_graphql.py` & `weaviate_client-4.6.0b0/mock_tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/mock_tests/test_resend.py` & `weaviate_client-4.6.0b0/mock_tests/test_resend.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/mock_tests/test_schema.py` & `weaviate_client-4.6.0b0/mock_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/profiling/constants.py` & `weaviate_client-4.6.0b0/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/profiling/test_import_and_query.py` & `weaviate_client-4.6.0b0/profiling/test_import_and_query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/profiling/test_profiling.py` & `weaviate_client-4.6.0b0/profiling/test_profiling.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # run:
 # - profiling: pytest -m profiling profiling/test_profiling.py --profile-svg
 # - benchmark: pytest profiling/test_profiling.py --benchmark-only --benchmark-disable-gc
 
 import math
 from typing import Any, List
+import uuid
 import pytest
 import weaviate
 from weaviate.collections.classes.config import Configure, DataType, Property
 from weaviate.collections.classes.data import DataObject
 from weaviate.collections.classes.grpc import MetadataQuery
 
 from .constants import WEAVIATE_LOGO_OLD_ENCODED
@@ -184,14 +185,54 @@
     col.data.insert_many([{"index": i, "blob": WEAVIATE_LOGO_OLD_ENCODED} for i in range(1000)])
 
     for _i in range(1000):
         objs = col.query.fetch_objects(limit=100, return_properties=["blob"]).objects
         assert len(objs) == 100
 
 
+@pytest.mark.profiling
+def test_list_value_properties(client: weaviate.WeaviateClient) -> None:
+    name = "TestProfileListValueProperties"
+    client.collections.delete(name)
+
+    col = client.collections.create(
+        name=name,
+        properties=[
+            Property(name="bools", data_type=DataType.BOOL_ARRAY),
+            Property(name="dates", data_type=DataType.DATE_ARRAY),
+            Property(name="ints", data_type=DataType.INT_ARRAY),
+            Property(name="numbers", data_type=DataType.NUMBER_ARRAY),
+            Property(name="texts", data_type=DataType.TEXT_ARRAY),
+            Property(name="uuids", data_type=DataType.UUID_ARRAY),
+        ],
+        vectorizer_config=Configure.Vectorizer.none(),
+    )
+
+    col = client.collections.get(name)
+
+    with col.batch.dynamic() as batch:
+        for i in range(100):
+            batch.add_object(
+                properties={
+                    "bools": [True] * 10000,
+                    "dates": ["2021-01-01T00:00:00Z"] * 10000,
+                    "ints": [i] * 10000,
+                    "numbers": [3.3] * 10000,
+                    "texts": ["Test"] * 10000,
+                    "uuids": [uuid.uuid4()] * 10000,
+                }
+            )
+
+    for _ in range(100):
+        objs = col.query.fetch_objects(
+            limit=100, return_properties=["bools", "ints", "numbers", "texts"]
+        ).objects
+        assert len(objs) == 100
+
+
 def test_benchmark_get_vector(benchmark: Any, client: weaviate.WeaviateClient) -> None:
     benchmark(test_get_vector, client)
 
 
 def test_benchmark_get_float_properties(benchmark: Any, client: weaviate.WeaviateClient) -> None:
     benchmark(test_get_float_properties, client)
 
@@ -202,7 +243,11 @@
 
 def test_benchmark_vector_search(benchmark: Any, client: weaviate.WeaviateClient) -> None:
     benchmark(test_vector_search, client)
 
 
 def test_benchmark_blob_properties(benchmark: Any, client: weaviate.WeaviateClient) -> None:
     benchmark(test_blob_properties, client)
+
+
+def test_benchmark_list_value_properties(benchmark: Any, client: weaviate.WeaviateClient) -> None:
+    benchmark(test_list_value_properties, client)
```

### Comparing `weaviate-client-4.5rc0/profiling/test_refs.py` & `weaviate_client-4.6.0b0/profiling/test_refs.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/profiling/test_sphere.py` & `weaviate_client-4.6.0b0/profiling/test_sphere.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         #     "X-Cohere-Api-Key": "YOUR_KEY",
         #     "X-OpenAI-Api-Key": "YOUR_KEY",
         # },
     )
     start = time.time()
 
     import_objects = 50000
-    with collection.batch.rate_limit(requests_per_minute=1234) as batch:
+    with collection.batch.dynamic() as batch:
         with open(sphere_file) as jsonl_file:
             for i, jsonl in enumerate(jsonl_file):
                 if i == import_objects or batch.number_errors > 10:
                     break
 
                 json_parsed = json.loads(jsonl)
                 batch.add_object(
```

### Comparing `weaviate-client-4.5rc0/publishing.md` & `weaviate_client-4.6.0b0/publishing.md`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/pyproject.toml` & `weaviate_client-4.6.0b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -26,13 +26,12 @@
 
 [tool.mypy]
 python_version = "3.11"
 disallow_untyped_defs = true
 show_error_codes = true
 no_implicit_optional = true
 warn_return_any = true
-warn_unused_ignores = true
 exclude = ["weaviate/proto", "docs", "integration_v3"]
 
 [[tool.mypy.overrides]]
 module = "weaviate.proto.v1.*"
 ignore_errors = true
```

### Comparing `weaviate-client-4.5rc0/requirements-devel.txt` & `weaviate_client-4.6.0b0/requirements-devel.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 requests>=2.30.0,<3.0.0
-httpx==0.27.0
-validators==0.22.0
+httpx>=0.25.2,<=0.27.0
+validators==0.28.1
 authlib>=1.2.1,<2.0.0
 grpcio>=1.57.0,<2.0.0
 grpcio-tools>=1.57.0,<2.0.0
 grpcio-health-checking>=1.57.0,<2.0.0
 pydantic>=2.5.0,<3.0.0
 
 build
 twine
 wheel
 setuptools_scm
 Sphinx>=7.0.0
 sphinx-rtd-theme==2.0.0
-autodoc-pydantic==2.0.1
+autodoc-pydantic==2.2.0
 
 grpcio-tools
 
-pytest==8.0.1
-pytest-cov==4.1.0
+pytest==8.2.0
+pytest-cov==5.0.0
 pytest-benchmark==4.0.0
 pytest-profiling==1.7.0
-coverage==7.4.2
-pytest-xdist==3.5.0
+coverage==7.5.1
+pytest-xdist==3.6.1
 werkzeug>=2.3.7
 pytest-httpserver>=1.0.8
 
-mypy>=1.5.1<2.0.0
+mypy>=1.9.0<2.0.0
 mypy-extensions==1.0.0
 tomli>=2.0.1<3.0.0
 types-Deprecated>=1.2.9.3<2.0.0
 types-protobuf>=4.24.0.1<5.0.0
 types-requests>=2.31.0.2<3.0.0
 types-urllib3>=1.26.25.14<2.0.0
 typing_extensions>=4.7.1<5.0.0
 
 pre-commit
 
 flake8
-flake8-bugbear==24.2.6
+flake8-bugbear==24.4.26
 flake8-comprehensions==3.14.0
-flake8-builtins==2.2.0
+flake8-builtins==2.5.0
```

### Comparing `weaviate-client-4.5rc0/setup.cfg` & `weaviate_client-4.6.0b0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 	weaviate.cluster
 	weaviate.proto
 	weaviate.proto.v1
 platforms = any
 include_package_data = True
 install_requires = 
 	requests>=2.30.0,<3.0.0
-	httpx==0.27.0
-	validators==0.22.0
+	httpx>=0.25.0,<=0.27.0
+	validators==0.28.1
 	authlib>=1.2.1,<2.0.0
 	pydantic>=2.5.0,<3.0.0
 	grpcio>=1.57.0,<2.0.0
 	grpcio-tools>=1.57.0,<2.0.0
 	grpcio-health-checking>=1.57.0,<2.0.0
 python_requires = >=3.8
```

### Comparing `weaviate-client-4.5rc0/test/README.md` & `weaviate_client-4.6.0b0/test/README.md`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/batch/test_requests.py` & `weaviate_client-4.6.0b0/test/batch/test_requests.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/classification/test_classification.py` & `weaviate_client-4.6.0b0/test/classification/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/cluster/test_cluster.py` & `weaviate_client-4.6.0b0/test/cluster/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/collection/test_aggregates.py` & `weaviate_client-4.6.0b0/test/collection/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/collection/test_classes.py` & `weaviate_client-4.6.0b0/test/collection/test_classes.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/collection/test_client.py` & `weaviate_client-4.6.0b0/test/collection/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/collection/test_collection_model.py` & `weaviate_client-4.6.0b0/test/collection/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/collection/test_config.py` & `weaviate_client-4.6.0b0/test/collection/test_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -191,14 +191,28 @@
                 "endpoint": "something",
                 "region": "us-east-1",
                 "service": "sagemaker",
             }
         },
     ),
     (
+        Configure.Vectorizer.text2vec_octoai(
+            vectorize_collection_name=False,
+            model="thenlper/gte-large",
+            base_url="https://text.octoai.com",
+        ),
+        {
+            "text2vec-octoai": {
+                "vectorizeClassName": False,
+                "model": "thenlper/gte-large",
+                "baseURL": "https://text.octoai.com",
+            }
+        },
+    ),
+    (
         Configure.Vectorizer.text2vec_openai(),
         {
             "text2vec-openai": {
                 "vectorizeClassName": True,
             }
         },
     ),
@@ -232,22 +246,22 @@
                 "vectorizeClassName": True,
             }
         },
     ),
     (
         Configure.Vectorizer.text2vec_palm(
             project_id="project",
-            api_endpoint="https://api.google.com",
+            api_endpoint="api.google.com",
             model_id="model",
             vectorize_collection_name=False,
         ),
         {
             "text2vec-palm": {
                 "projectId": "project",
-                "apiEndpoint": "https://api.google.com/",
+                "apiEndpoint": "api.google.com",
                 "modelId": "model",
                 "vectorizeClassName": False,
             }
         },
     ),
     (
         Configure.Vectorizer.text2vec_transformers(),
@@ -258,19 +272,37 @@
             }
         },
     ),
     (
         Configure.Vectorizer.text2vec_transformers(
             pooling_strategy="cls",
             vectorize_collection_name=False,
+            inference_url="https://api.transformers.com",
         ),
         {
             "text2vec-transformers": {
                 "vectorizeClassName": False,
                 "poolingStrategy": "cls",
+                "inferenceUrl": "https://api.transformers.com",
+            }
+        },
+    ),
+    (
+        Configure.Vectorizer.text2vec_voyageai(
+            vectorize_collection_name=False,
+            model="voyage-large-2",
+            truncate=False,
+            base_url="https://voyage.made-up.com",
+        ),
+        {
+            "text2vec-voyageai": {
+                "vectorizeClassName": False,
+                "model": "voyage-large-2",
+                "baseURL": "https://voyage.made-up.com",
+                "truncate": False,
             }
         },
     ),
     (
         Configure.Vectorizer.img2vec_neural(
             image_fields=["test"],
         ),
@@ -290,14 +322,35 @@
                 "imageFields": ["image"],
                 "textFields": ["text"],
                 "vectorizeClassName": True,
             }
         },
     ),
     (
+        Configure.Vectorizer.multi2vec_palm(
+            image_fields=["image"],
+            text_fields=["text"],
+            video_fields=["video"],
+            project_id="project",
+            video_interval_seconds=1,
+            location="us-central1",
+        ),
+        {
+            "multi2vec-palm": {
+                "imageFields": ["image"],
+                "textFields": ["text"],
+                "videoFields": ["video"],
+                "projectId": "project",
+                "location": "us-central1",
+                "videoIntervalSeconds": 1,
+                "vectorizeClassName": True,
+            }
+        },
+    ),
+    (
         Configure.Vectorizer.multi2vec_clip(
             image_fields=[Multi2VecField(name="image")],
             text_fields=[Multi2VecField(name="text")],
         ),
         {
             "multi2vec-clip": {
                 "imageFields": ["image"],
@@ -532,14 +585,34 @@
         {"generative-openai": {}},
     ),
     (
         Configure.Generative.anyscale(),
         {"generative-anyscale": {}},
     ),
     (
+        Configure.Generative.mistral(temperature=0.5, max_tokens=100, model="model"),
+        {"generative-mistral": {"temperature": 0.5, "maxTokens": 100, "model": "model"}},
+    ),
+    (
+        Configure.Generative.octoai(
+            model="mistral-7b-instruct",
+            temperature=0.5,
+            base_url="https://text.octoai.run",
+            max_tokens=123,
+        ),
+        {
+            "generative-octoai": {
+                "model": "mistral-7b-instruct",
+                "maxTokens": 123,
+                "temperature": 0.5,
+                "baseURL": "https://text.octoai.run",
+            }
+        },
+    ),
+    (
         Configure.Generative.openai(
             model="gpt-4",
             frequency_penalty=0.5,
             max_tokens=100,
             presence_penalty=0.5,
             temperature=0.5,
             top_p=0.5,
@@ -696,25 +769,25 @@
 ]
 
 
 @pytest.mark.parametrize("reranker_config,expected_mc", TEST_CONFIG_WITH_RERANKER)
 def test_config_with_reranker(
     reranker_config: _RerankerConfigCreate,
     expected_mc: dict,
-):
+) -> None:
     config = _CollectionConfigCreate(name="test", reranker_config=reranker_config)
     assert config._to_dict() == {
         **DEFAULTS,
         "vectorizer": "none",
         "class": "Test",
         "moduleConfig": expected_mc,
     }
 
 
-def test_config_with_properties():
+def test_config_with_properties() -> None:
     config = _CollectionConfigCreate(
         name="test",
         description="test",
         vectorizer_config=Configure.Vectorizer.none(),
         properties=[
             Property(
                 name="text",
@@ -876,22 +949,22 @@
     assert vi_dict["bq"]["rescoreLimit"] == 123
 
 
 def test_vector_config_flat_pq() -> None:
     vector_index = Configure.VectorIndex.flat(
         distance_metric=VectorDistances.DOT,
         vector_cache_max_objects=456,
-        quantizer=Configure.VectorIndex.Quantizer.pq(bit_compression=True, segments=789),
+        quantizer=Configure.VectorIndex.Quantizer.pq(segments=789),
     )
 
     vi_dict = vector_index._to_dict()
 
     assert vi_dict["distance"] == "dot"
     assert vi_dict["vectorCacheMaxObjects"] == 456
-    assert vi_dict["pq"]["bitCompression"]
+    assert "bitCompression" not in vi_dict["pq"]
     assert vi_dict["pq"]["segments"] == 789
 
 
 TEST_CONFIG_WITH_NAMED_VECTORIZER_PARAMETERS = [
     (
         [Configure.NamedVectors.text2vec_contextionary(name="test", source_properties=["prop"])],
         {
@@ -989,14 +1062,33 @@
                 },
                 "vectorIndexType": "hnsw",
             }
         },
     ),
     (
         [
+            Configure.NamedVectors.text2vec_octoai(
+                name="test", source_properties=["prop"], base_url="https://text.octoai.com"
+            )
+        ],
+        {
+            "test": {
+                "vectorizer": {
+                    "text2vec-octoai": {
+                        "properties": ["prop"],
+                        "vectorizeClassName": True,
+                        "baseURL": "https://text.octoai.com",
+                    }
+                },
+                "vectorIndexType": "hnsw",
+            }
+        },
+    ),
+    (
+        [
             Configure.NamedVectors.text2vec_openai(
                 name="test", source_properties=["prop"], base_url="https://api.openai.com/"
             )
         ],
         {
             "test": {
                 "vectorizer": {
@@ -1044,14 +1136,33 @@
                 },
                 "vectorIndexType": "hnsw",
             }
         },
     ),
     (
         [
+            Configure.NamedVectors.text2vec_voyageai(
+                name="test", source_properties=["prop"], truncate=True
+            )
+        ],
+        {
+            "test": {
+                "vectorizer": {
+                    "text2vec-voyageai": {
+                        "properties": ["prop"],
+                        "vectorizeClassName": True,
+                        "truncate": True,
+                    }
+                },
+                "vectorIndexType": "hnsw",
+            }
+        },
+    ),
+    (
+        [
             Configure.NamedVectors.img2vec_neural(
                 name="test",
                 image_fields=["test"],
             )
         ],
         {
             "test": {
@@ -1081,14 +1192,39 @@
                         "vectorizeClassName": True,
                     }
                 },
                 "vectorIndexType": "hnsw",
             }
         },
     ),
+    (
+        [
+            Configure.NamedVectors.multi2vec_palm(
+                name="test",
+                image_fields=["image"],
+                text_fields=["text"],
+                project_id="project",
+                location="us-central1",
+            )
+        ],
+        {
+            "test": {
+                "vectorizer": {
+                    "multi2vec-palm": {
+                        "imageFields": ["image"],
+                        "textFields": ["text"],
+                        "projectId": "project",
+                        "location": "us-central1",
+                        "vectorizeClassName": True,
+                    }
+                },
+                "vectorIndexType": "hnsw",
+            }
+        },
+    ),
     (
         [
             Configure.NamedVectors.multi2vec_bind(
                 name="test",
                 audio_fields=["audio"],
                 depth_fields=["depth"],
                 image_fields=["image"],
```

### Comparing `weaviate-client-4.5rc0/test/collection/test_queries.py` & `weaviate_client-4.6.0b0/test/collection/test_queries.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/connection/test_connection.py` & `weaviate_client-4.6.0b0/test/connection/test_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     @patch("weaviate.connect.base.os")
     def test_get_proxies(self, os_mock):
         """
         Test the `_get_proxies` function.
         """
 
         error_msg = lambda dt: (
-            "If 'proxies' is not None, it must be of type dict or str. " f"Given type: {dt}."
+            "If 'proxies' is not None, it must be of type dict, str, or wvc.init.Proxies. "
+            f"Given type: {dt}."
         )
         with self.assertRaises(TypeError) as error:
             proxies = _get_proxies([], False)
         check_error_message(self, error, error_msg(list))
 
         proxies = _get_proxies({}, False)
         self.assertEqual(proxies, {})
@@ -75,23 +76,23 @@
         proxies = _get_proxies({"test": True}, False)
         self.assertEqual(proxies, {"test": True})
 
         proxies = _get_proxies({"test": True}, True)
         self.assertEqual(proxies, {"test": True})
 
         proxies = _get_proxies("test", True)
-        self.assertEqual(proxies, {"http": "test", "https": "test"})
+        self.assertEqual(proxies, {"http": "test", "https": "test", "grpc": "test"})
 
         os_mock.environ.get.return_value = None
         proxies = _get_proxies(None, True)
         self.assertEqual(proxies, {})
 
         os_mock.environ.get.return_value = "test"
         proxies = _get_proxies(None, True)
-        self.assertEqual(proxies, {"http": "test", "https": "test"})
+        self.assertEqual(proxies, {"http": "test", "https": "test", "grpc": "test"})
 
     def test__get_valid_timeout_config(self):
         """
         Test the `_get_valid_timeout_config` function.
         """
 
         # incalid calls
```

### Comparing `weaviate-client-4.5rc0/test/contextionary/test_text2vec_contextionary.py` & `weaviate_client-4.6.0b0/test/contextionary/test_text2vec_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/data/references/test_crud_references.py` & `weaviate_client-4.6.0b0/test/data/references/test_crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/data/test_crud_data.py` & `weaviate_client-4.6.0b0/test/data/test_crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/gql/test_aggregate.py` & `weaviate_client-4.6.0b0/test/gql/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/gql/test_filter.py` & `weaviate_client-4.6.0b0/test/gql/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/gql/test_get.py` & `weaviate_client-4.6.0b0/test/gql/test_get.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/gql/test_query.py` & `weaviate_client-4.6.0b0/test/gql/test_query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/schema/properties/test_properties.py` & `weaviate_client-4.6.0b0/test/schema/properties/test_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/schema/schema_company.json` & `weaviate_client-4.6.0b0/test/schema/schema_company.json`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/schema/test_schema.py` & `weaviate_client-4.6.0b0/test/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/test_auth.py` & `weaviate_client-4.6.0b0/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/test_client.py` & `weaviate_client-4.6.0b0/test/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/test_embedded.py` & `weaviate_client-4.6.0b0/test/test_embedded.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/test_exceptions.py` & `weaviate_client-4.6.0b0/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/test_server_version.py` & `weaviate_client-4.6.0b0/test/test_server_version.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/test_util.py` & `weaviate_client-4.6.0b0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/test/util.py` & `weaviate_client-4.6.0b0/test/util.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/__init__.py` & `weaviate_client-4.6.0b0/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/auth.py` & `weaviate_client-4.6.0b0/weaviate/auth.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/backup/backup.py` & `weaviate_client-4.6.0b0/weaviate/backup/backup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,37 @@
 from typing import Optional, Union, List, Tuple, Any, Dict
 from pydantic import BaseModel, Field
 
 from requests.exceptions import ConnectionError as RequestsConnectionError
 
 from weaviate.connect import Connection, ConnectionV4
 from weaviate.exceptions import (
+    WeaviateInvalidInputError,
+    WeaviateUnsupportedFeatureError,
     BackupFailedException,
     EmptyResponseException,
 )
 from weaviate.util import _capitalize_first_letter, _decode_json_response_dict
 
 STORAGE_NAMES = {
     "filesystem",
     "s3",
     "gcs",
     "azure",
 }
 
 
+class BackupCompressionLevel(str, Enum):
+    """Which compression level should be used to compress the backup."""
+
+    DEFAULT = "DefaultCompression"
+    BEST_SPEED = "BestSpeed"
+    BEST_COMPRESSION = "BestCompression"
+
+
 class BackupStorage(str, Enum):
     """Which backend should be used to write the backup to."""
 
     FILESYSTEM = "filesystem"
     S3 = "s3"
     GCS = "gcs"
     AZURE = "azure"
@@ -39,17 +49,35 @@
     STARTED = "STARTED"
     TRANSFERRING = "TRANSFERRING"
     TRANSFERRED = "TRANSFERRED"
     SUCCESS = "SUCCESS"
     FAILED = "FAILED"
 
 
+class _BackupConfigBase(BaseModel):
+    CPUPercentage: Optional[int] = Field(default=None, alias="cpu_percentage")
+
+
+class BackupConfigCreate(_BackupConfigBase):
+    """Options to configure the backup when creating a backup."""
+
+    ChunkSize: Optional[int] = Field(default=None, alias="chunk_size")
+    CompressionLevel: Optional[BackupCompressionLevel] = Field(
+        default=None, alias="compression_level"
+    )
+
+
+class BackupConfigRestore(_BackupConfigBase):
+    """Options to configure the backup when restoring a backup."""
+
+
 class BackupStatusReturn(BaseModel):
     """Return type of the backup status methods."""
 
+    error: Optional[str] = Field(default=None)
     status: BackupStatus
     path: str
 
 
 class BackupReturn(BackupStatusReturn):
     """Return type of the backup creation and restore methods."""
 
@@ -65,14 +93,15 @@
     def create(
         self,
         backup_id: str,
         backend: BackupStorage,
         include_collections: Optional[Union[List[str], str]] = None,
         exclude_collections: Optional[Union[List[str], str]] = None,
         wait_for_completion: bool = False,
+        config: Optional[BackupConfigCreate] = None,
     ) -> BackupReturn:
         """Create a backup of all/per collection Weaviate objects.
 
         Parameters
         ----------
         backup_id : str
             The identifier name of the backup.
@@ -83,14 +112,16 @@
             The collection/list of collections to be included in the backup. If not specified all
             collections will be included. Either `include_collections` or `exclude_collections` can be set. By default None.
         exclude_collections : Union[List[str], str], optional
             The collection/list of collections to be excluded in the backup.
             Either `include_collections` or `exclude_collections` can be set. By default None.
         wait_for_completion : bool, optional
             Whether to wait until the backup is done. By default False.
+        config: BackupConfigCreate, optional
+            The configuration of the backup creation. By default None.
 
         Returns
         -------
          A `_BackupReturn` object that contains the backup creation response.
 
         Raises
         ------
@@ -110,19 +141,31 @@
             backup_id=backup_id,
             backend=backend,  # can be removed when we remove the old backup class
             include_classes=include_collections,
             exclude_classes=exclude_collections,
             wait_for_completion=wait_for_completion,
         )
 
-        payload = {
+        payload: dict = {
             "id": backup_id,
             "include": include_collections,
             "exclude": exclude_collections,
         }
+
+        if config is not None:
+            if self._connection._weaviate_version.is_lower_than(1, 25, 0):
+                raise WeaviateUnsupportedFeatureError(
+                    "BackupConfigCreate", str(self._connection._weaviate_version), "1.25.0"
+                )
+            if not isinstance(config, BackupConfigCreate):
+                raise WeaviateInvalidInputError(
+                    f"Expected 'config' to be of type 'BackupConfigCreate', but got {type(config)}."
+                )
+            payload["config"] = config.model_dump()
+
         path = f"/backups/{backend.value}"
 
         response = self._connection.post(
             path=path,
             weaviate_object=payload,
             error_msg="Backup creation failed due to connection error.",
         )
@@ -135,15 +178,17 @@
                     backup_id=backup_id,
                     backend=backend,
                 )
                 create_status["status"] = status.status
                 if status.status == BackupStatus.SUCCESS:
                     break
                 if status.status == BackupStatus.FAILED:
-                    raise BackupFailedException(f"Backup failed: {create_status}")
+                    raise BackupFailedException(
+                        f"Backup failed: {create_status} with error: {status.error}"
+                    )
                 sleep(1)
         return BackupReturn(**create_status)
 
     def get_create_status(self, backup_id: str, backend: BackupStorage) -> BackupStatusReturn:
         """
         Checks if a started backup job has completed.
 
@@ -178,14 +223,15 @@
     def restore(
         self,
         backup_id: str,
         backend: BackupStorage,
         include_collections: Union[List[str], str, None] = None,
         exclude_collections: Union[List[str], str, None] = None,
         wait_for_completion: bool = False,
+        config: Optional[BackupConfigRestore] = None,
     ) -> BackupReturn:
         """
         Restore a backup of all/per collection Weaviate objects.
 
         Parameters
         ----------
         backup_id : str
@@ -198,14 +244,16 @@
             collections will be included (that were backup-ed). Either `include_collections` or
             `exclude_collections` can be set. By default None.
         exclude_collections : Union[List[str], str], optional
             The collection/list of collections to be excluded in the backup restore.
             Either `include_collections` or `exclude_collections` can be set. By default None.
         wait_for_completion : bool, optional
             Whether to wait until the backup restore is done.
+        config: BackupConfigRestore, optional
+            The configuration of the backup restoration. By default None.
 
         Returns
         -------
          A `BackupReturn` object that contains the backup restore response.
 
         Raises
         ------
@@ -223,18 +271,30 @@
             backup_id=backup_id,
             backend=backend,
             include_classes=include_collections,
             exclude_classes=exclude_collections,
             wait_for_completion=wait_for_completion,
         )
 
-        payload = {
+        payload: dict = {
             "include": include_collections,
             "exclude": exclude_collections,
         }
+
+        if config is not None:
+            if self._connection._weaviate_version.is_lower_than(1, 25, 0):
+                raise WeaviateUnsupportedFeatureError(
+                    "BackupConfigRestore", str(self._connection._weaviate_version), "1.25.0"
+                )
+            if not isinstance(config, BackupConfigRestore):
+                raise WeaviateInvalidInputError(
+                    f"Expected 'config' to be of type 'BackupConfigRestore', but got {type(config)}."
+                )
+            payload["config"] = config.model_dump()
+
         path = f"/backups/{backend.value}/{backup_id}/restore"
         response = self._connection.post(
             path=path,
             weaviate_object=payload,
             error_msg="Backup restore failed due to connection error.",
         )
         restore_status = _decode_json_response_dict(response, "Backup restore")
@@ -245,15 +305,17 @@
                     backup_id=backup_id,
                     backend=backend,
                 )
                 restore_status["status"] = status.status
                 if status.status == BackupStatus.SUCCESS:
                     break
                 if status.status == BackupStatus.FAILED:
-                    raise BackupFailedException(f"Backup restore failed: {restore_status}")
+                    raise BackupFailedException(
+                        f"Backup restore failed: {restore_status} with error: {status.error}"
+                    )
                 sleep(1)
         return BackupReturn(**restore_status)
 
     def get_restore_status(self, backup_id: str, backend: BackupStorage) -> BackupStatusReturn:
         """
         Checks if a started classification job has completed.
```

### Comparing `weaviate-client-4.5rc0/weaviate/batch/crud_batch.py` & `weaviate_client-4.6.0b0/weaviate/batch/crud_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -964,15 +964,17 @@
             self._objects_throughput_frame.append(
                 len(self._objects_batch) / response.elapsed.total_seconds()
             )
             obj_per_second = sum(self._objects_throughput_frame) / len(
                 self._objects_throughput_frame
             )
 
-            self._recommended_num_objects = max(round(obj_per_second * self._creation_time), 1)
+            self._recommended_num_objects = max(
+                round(obj_per_second * float(self._creation_time)), 1
+            )
 
             res = _decode_json_response_list(response, "batch add objects")
             assert res is not None
             return res
         return []
 
     def create_references(self) -> list:
@@ -1061,15 +1063,15 @@
             self._references_throughput_frame.append(
                 len(self._reference_batch) / response.elapsed.total_seconds()
             )
             ref_per_sec = sum(self._references_throughput_frame) / len(
                 self._references_throughput_frame
             )
 
-            self._recommended_num_references = round(ref_per_sec * self._creation_time)
+            self._recommended_num_references = round(ref_per_sec * float(self._creation_time))
 
             res = _decode_json_response_list(response, "Create references")
             assert res is not None
             return res
         return []
 
     def _flush_in_thread(
@@ -1168,15 +1170,15 @@
             and not self._new_dynamic_batching
         ):
             obj_per_second = (
                 sum(self._objects_throughput_frame) / len(self._objects_throughput_frame) * 0.75
             )
             self._recommended_num_objects = max(
                 min(
-                    round(obj_per_second * self._creation_time),
+                    round(obj_per_second * float(self._creation_time)),
                     self._recommended_num_objects + 250,
                 ),
                 1,
             )
 
         # Create references after all the objects have been created
         reference_future_pool = []
@@ -1206,15 +1208,15 @@
             len(self._references_throughput_frame) != 0
             and self._recommended_num_references is not None
         ):
             ref_per_sec = sum(self._references_throughput_frame) / len(
                 self._references_throughput_frame
             )
             self._recommended_num_references = min(
-                round(ref_per_sec * self._creation_time),
+                round(ref_per_sec * float(self._creation_time)),
                 self._recommended_num_references * 2,
             )
 
         self._future_pool = []
         self._reference_batch_queue = []
         return
 
@@ -1738,19 +1740,19 @@
         return self._creation_time
 
     @creation_time.setter
     def creation_time(self, value: Real) -> None:
         _check_positive_num(value, "creation_time", Real)
         if self._recommended_num_references is not None:
             self._recommended_num_references = round(
-                self._recommended_num_references * value / self._creation_time
+                self._recommended_num_references * float(value) / float(self._creation_time)
             )
         if self._recommended_num_objects is not None:
             self._recommended_num_objects = round(
-                self._recommended_num_objects * value / self._creation_time
+                self._recommended_num_objects * float(value) / float(self._creation_time)
             )
         self._creation_time = value
         if self._batching_type:
             self._auto_create()
 
     @property
     def timeout_retries(self) -> int:
```

### Comparing `weaviate-client-4.5rc0/weaviate/batch/requests.py` & `weaviate_client-4.6.0b0/weaviate/batch/requests.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/classes/config.py` & `weaviate_client-4.6.0b0/weaviate/classes/config.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/classes/query.py` & `weaviate_client-4.6.0b0/weaviate/classes/query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from weaviate.collections.classes.filters import Filter
 from weaviate.collections.classes.aggregate import Metrics
 from weaviate.collections.classes.grpc import (
     HybridFusion,
     GroupBy,
+    HybridNear,
     MetadataQuery,
     Move,
     NearMediaType,
     QueryNested,
     QueryReference,
     Rerank,
     Sort,
@@ -15,14 +16,15 @@
 
 
 __all__ = [
     "Filter",
     "GeoCoordinate",
     "GroupBy",
     "HybridFusion",
+    "HybridNear",
     "MetadataQuery",
     "Metrics",
     "Move",
     "NearMediaType",
     "QueryNested",
     "QueryReference",
     "Rerank",
```

### Comparing `weaviate-client-4.5rc0/weaviate/classification/classification.py` & `weaviate_client-4.6.0b0/weaviate/classification/classification.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/classification/config_builder.py` & `weaviate_client-4.6.0b0/weaviate/classification/config_builder.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/client.py` & `weaviate_client-4.6.0b0/weaviate/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from httpx import HTTPError as HttpxError
 from requests.exceptions import ConnectionError as RequestsConnectionError
 
 from weaviate.backup.backup import _Backup
 from weaviate.collections.classes.internal import _GQLEntryReturnType, _RawGQLReturn
 
+from weaviate.integrations import _Integrations
+
 from .auth import AuthCredentials
 from .backup import Backup
 from .batch import Batch
 from .classification import Classification
 from .cluster import Cluster
 from .collections.collections import _Collections
 from .collections.batch.client import _BatchClientWrapper
@@ -183,38 +185,41 @@
             - `skip_init_checks`: `bool`, optional
                 - If set to `True` then the client will not perform any checks including ensuring that weaviate has started. This is useful for air-gapped environments and high-performance setups.
         """
         connection_params, embedded_db = self.__parse_connection_params_and_embedded_db(
             connection_params, embedded_options
         )
         config = additional_config or AdditionalConfig()
+
         self.__skip_init_checks = skip_init_checks
 
         self._connection = ConnectionV4(  # pyright: ignore reportIncompatibleVariableOverride
             connection_params=connection_params,
             auth_client_secret=auth_client_secret,
-            timeout_config=_get_valid_timeout_config(config.timeout),
+            timeout_config=config.timeout,
             additional_headers=additional_headers,
             embedded_db=embedded_db,
             connection_config=config.connection,
             proxies=config.proxies,
             trust_env=config.trust_env,
         )
 
-        self.batch = _BatchClientWrapper(self._connection, consistency_level=None)
-        """This namespace contains all the functionality to upload data in batches to Weaviate for all collections and tenants."""
         self.backup = _Backup(self._connection)
         """This namespace contains all functionality to backup data."""
         self.cluster = _Cluster(self._connection)
         """This namespace contains all functionality to inspect the connected Weaviate cluster."""
         self.collections = _Collections(self._connection)
         """This namespace contains all the functionality to manage Weaviate data collections. It is your main entry point for all collection-related functionality.
 
         Use it to retrieve collection objects using `client.collections.get("MyCollection")` or to create new collections using `client.collections.create("MyCollection", ...)`.
         """
+        self.batch = _BatchClientWrapper(self._connection, config=self.collections)
+        """This namespace contains all the functionality to upload data in batches to Weaviate for all collections and tenants."""
+
+        self.integrations = _Integrations(self._connection)
 
     def __parse_connection_params_and_embedded_db(
         self,
         connection_params: Optional[ConnectionParams],
         embedded_options: Optional[EmbeddedOptions],
     ) -> Tuple[ConnectionParams, Optional[EmbeddedV4]]:
         if connection_params is None and embedded_options is None:
```

### Comparing `weaviate-client-4.5rc0/weaviate/cluster/cluster.py` & `weaviate_client-4.6.0b0/weaviate/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/aggregations/base.py` & `weaviate_client-4.6.0b0/weaviate/collections/aggregations/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,21 +48,21 @@
     def __init__(
         self,
         connection: ConnectionV4,
         name: str,
         consistency_level: Optional[ConsistencyLevel],
         tenant: Optional[str],
     ):
-        self.__connection = connection
+        self._connection = connection
         self.__name = name
         self._tenant = tenant
         self._consistency_level = consistency_level
 
     def _query(self) -> AggregateBuilder:
-        return AggregateBuilder(self.__name, self.__connection)
+        return AggregateBuilder(self.__name, self._connection)
 
     def _to_aggregate_result(
         self, response: dict, metrics: Optional[List[_Metrics]]
     ) -> AggregateReturn:
         try:
             result: dict = response["data"]["Aggregate"][self.__name][0]
             return AggregateReturn(
@@ -231,15 +231,41 @@
                 _ValidateArgument([int, float, None], "certainty", certainty),
                 _ValidateArgument([int, float, None], "distance", distance),
                 _ValidateArgument([int, None], "object_limit", object_limit),
             ]
         )
 
     @staticmethod
-    def _add_near_image(
+    def _add_hybrid_to_builder(
+        builder: AggregateBuilder,
+        query: Optional[str],
+        alpha: Optional[NUMBER],
+        vector: Optional[List[float]],
+        query_properties: Optional[List[str]],
+        object_limit: Optional[int],
+        target_vector: Optional[str],
+    ) -> AggregateBuilder:
+        payload: dict = {}
+        if query is not None:
+            payload["query"] = query
+        if alpha is not None:
+            payload["alpha"] = alpha
+        if vector is not None:
+            payload["vector"] = vector
+        if query_properties is not None:
+            payload["properties"] = query_properties
+        if target_vector is not None:
+            payload["targetVectors"] = [target_vector]
+        builder = builder.with_hybrid(payload)
+        if object_limit is not None:
+            builder = builder.with_object_limit(object_limit)
+        return builder
+
+    @staticmethod
+    def _add_near_image_to_builder(
         builder: AggregateBuilder,
         near_image: Union[str, pathlib.Path, io.BufferedReader],
         certainty: Optional[NUMBER],
         distance: Optional[NUMBER],
         object_limit: Optional[int],
         target_vector: Optional[str],
     ) -> AggregateBuilder:
@@ -261,15 +287,15 @@
             payload["targetVector"] = target_vector
         builder = builder.with_near_image(payload, encode=False)
         if object_limit is not None:
             builder = builder.with_object_limit(object_limit)
         return builder
 
     @staticmethod
-    def _add_near_object(
+    def _add_near_object_to_builder(
         builder: AggregateBuilder,
         near_object: UUID,
         certainty: Optional[NUMBER],
         distance: Optional[NUMBER],
         object_limit: Optional[int],
         target_vector: Optional[str],
     ) -> AggregateBuilder:
@@ -289,15 +315,15 @@
             payload["targetVector"] = target_vector
         builder = builder.with_near_object(payload)
         if object_limit is not None:
             builder = builder.with_object_limit(object_limit)
         return builder
 
     @staticmethod
-    def _add_near_text(
+    def _add_near_text_to_builder(
         builder: AggregateBuilder,
         query: Union[List[str], str],
         certainty: Optional[NUMBER],
         distance: Optional[NUMBER],
         move_to: Optional[Move],
         move_away: Optional[Move],
         object_limit: Optional[int],
@@ -330,15 +356,15 @@
             payload["targetVector"] = target_vector
         builder = builder.with_near_text(payload)
         if object_limit is not None:
             builder = builder.with_object_limit(object_limit)
         return builder
 
     @staticmethod
-    def _add_near_vector(
+    def _add_near_vector_to_builder(
         builder: AggregateBuilder,
         near_vector: List[float],
         certainty: Optional[NUMBER],
         distance: Optional[NUMBER],
         object_limit: Optional[int],
         target_vector: Optional[str],
     ) -> AggregateBuilder:
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/aggregations/near_image.py` & `weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return_metrics = (
             return_metrics
             if (return_metrics is None or isinstance(return_metrics, list))
             else [return_metrics]
         )
         builder = self._base(return_metrics, filters, total_count)
         builder = self._add_groupby_to_builder(builder, group_by)
-        builder = self._add_near_image(
+        builder = self._add_near_image_to_builder(
             builder, near_image, certainty, distance, object_limit, target_vector
         )
         res = self._do(builder)
         return (
             self._to_aggregate_result(res, return_metrics)
             if group_by is None
             else self._to_group_by_result(res, return_metrics)
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/aggregations/near_object.py` & `weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         return_metrics = (
             return_metrics
             if (return_metrics is None or isinstance(return_metrics, list))
             else [return_metrics]
         )
         builder = self._base(return_metrics, filters, total_count)
         builder = self._add_groupby_to_builder(builder, group_by)
-        builder = self._add_near_object(
+        builder = self._add_near_object_to_builder(
             builder, near_object, certainty, distance, object_limit, target_vector
         )
         res = self._do(builder)
         return (
             self._to_aggregate_result(res, return_metrics)
             if group_by is None
             else self._to_group_by_result(res, return_metrics)
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/aggregations/near_text.py` & `weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         return_metrics = (
             return_metrics
             if (return_metrics is None or isinstance(return_metrics, list))
             else [return_metrics]
         )
         builder = self._base(return_metrics, filters, total_count)
         builder = self._add_groupby_to_builder(builder, group_by)
-        builder = self._add_near_text(
+        builder = self._add_near_text_to_builder(
             builder=builder,
             query=query,
             certainty=certainty,
             distance=distance,
             move_to=move_to,
             move_away=move_away,
             object_limit=object_limit,
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/aggregations/near_vector.py` & `weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         return_metrics = (
             return_metrics
             if (return_metrics is None or isinstance(return_metrics, list))
             else [return_metrics]
         )
         builder = self._base(return_metrics, filters, total_count)
         builder = self._add_groupby_to_builder(builder, group_by)
-        builder = self._add_near_vector(
+        builder = self._add_near_vector_to_builder(
             builder, near_vector, certainty, distance, object_limit, target_vector
         )
         res = self._do(builder)
         return (
             self._to_aggregate_result(res, return_metrics)
             if group_by is None
             else self._to_group_by_result(res, return_metrics)
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/aggregations/over_all.py` & `weaviate_client-4.6.0b0/weaviate/collections/aggregations/over_all.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/backups.py` & `weaviate_client-4.6.0b0/weaviate/collections/backups.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from typing import Optional
 from weaviate.backup.backup import (
     _Backup,
+    BackupConfigCreate,
+    BackupConfigRestore,
     BackupStatusReturn,
     BackupStorage,
 )
 from weaviate.connect import ConnectionV4
 
 
 class _CollectionBackup:
@@ -11,70 +14,87 @@
 
     def __init__(self, connection: ConnectionV4, name: str):
         self._connection = connection
         self._name = name
         self._backup = _Backup(connection)
 
     def create(
-        self, backup_id: str, backend: BackupStorage, wait_for_completion: bool = False
+        self,
+        backup_id: str,
+        backend: BackupStorage,
+        wait_for_completion: bool = False,
+        config: Optional[BackupConfigCreate] = None,
     ) -> BackupStatusReturn:
         """Create a backup of this collection.
 
         Arguments:
             `backup_id`
                 The identifier name of the backup. NOTE: Case insensitive.
             `backend`
                 The backend storage where to create the backup.
             `wait_for_completion`
                 Whether to wait until the backup is done. By default False.
+            `config`
+                The configuration for the backup creation. By default None.
 
         Returns:
             A `BackupStatusReturn` object that contains the backup creation response.
 
         Raises:
             `weaviate.WeaviateConnectionError`
                 If the network connection to weaviate fails.
             `weaviate.UnexpectedStatusCodeError`
                 If weaviate reports a none OK status.
             `weaviate.BackupFailedError`
                 If the backup failed.
             `TypeError`
                 One of the arguments have a wrong type.
         """
-        create = self._backup.create(backup_id, backend, [self._name], None, wait_for_completion)
-        return BackupStatusReturn(status=create.status, path=create.path)
+        create = self._backup.create(
+            backup_id, backend, [self._name], None, wait_for_completion, config
+        )
+        return BackupStatusReturn(error=create.error, status=create.status, path=create.path)
 
     def restore(
-        self, backup_id: str, backend: BackupStorage, wait_for_completion: bool = False
+        self,
+        backup_id: str,
+        backend: BackupStorage,
+        wait_for_completion: bool = False,
+        config: Optional[BackupConfigRestore] = None,
     ) -> BackupStatusReturn:
         """
         Restore a backup of all/per class Weaviate objects.
 
         Arguments:
             `backup_id`
                 The identifier name of the backup.
                 NOTE: Case insensitive.
             `backend`
                 The backend storage from where to restore the backup.
             `wait_for_completion`
-                Whether to wait until the backup restore is done.
+                Whether to wait until the backup restore is done. By default False.
+            `config`
+                The configuration for the backup restoration. By default None.
+
 
         Returns:
             A `BackupStatusReturn` object that contains the backup restore response.
 
         Raises:
             `weaviate.WeaviateConnectionError`
                 If the network connection to weaviate fails.
             `weaviate.UnexpectedStatusCodeError`
                 If weaviate reports a none OK status.
             `weaviate.BackupFailedError`
                 If the backup failed.
         """
-        restore = self._backup.restore(backup_id, backend, [self._name], None, wait_for_completion)
-        return BackupStatusReturn(status=restore.status, path=restore.path)
+        restore = self._backup.restore(
+            backup_id, backend, [self._name], None, wait_for_completion, config
+        )
+        return BackupStatusReturn(error=restore.error, status=restore.status, path=restore.path)
 
     def get_create_status(self, backup_id: str, backend: BackupStorage) -> BackupStatusReturn:
         """Check if a started backup job has completed.
 
         Arguments:
             `backup_id`
                 The identifier name of the backup.
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/base.py` & `weaviate_client-4.6.0b0/weaviate/collections/base.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/batch/base.py` & `weaviate_client-4.6.0b0/weaviate/collections/batch/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from collections import deque
 import math
 import threading
 import time
 import uuid as uuid_package
 from abc import ABC
 from copy import copy
 from dataclasses import dataclass, field
@@ -49,15 +50,18 @@
 
 BatchResponse = List[Dict[str, Any]]
 
 
 TBatchInput = TypeVar("TBatchInput")
 TBatchReturn = TypeVar("TBatchReturn")
 MAX_CONCURRENT_REQUESTS = 10
-DEFAULT_REQUEST_TIMEOUT = 120
+DEFAULT_REQUEST_TIMEOUT = 180
+CONCURRENT_REQUESTS_DYNAMIC_VECTORIZER = 2
+BATCH_TIME_TARGET = 10
+VECTORIZER_BATCHING_STEP_SIZE = 48  # cohere max batch size is 96
 
 
 class BatchRequest(ABC, Generic[TBatchInput, TBatchReturn]):
     """`BatchRequest` abstract class used as a interface for batch requests."""
 
     def __init__(self) -> None:
         self._items: List[TBatchInput] = []
@@ -154,21 +158,23 @@
 class _BatchBase:
     def __init__(
         self,
         connection: ConnectionV4,
         consistency_level: Optional[ConsistencyLevel],
         results: _BatchDataWrapper,
         batch_mode: _BatchMode,
+        vectorizer_batching: bool,
         objects_: Optional[ObjectsBatchRequest] = None,
         references: Optional[ReferencesBatchRequest] = None,
     ) -> None:
         self.__batch_objects = objects_ or ObjectsBatchRequest()
         self.__batch_references = references or ReferencesBatchRequest()
         self.__connection = connection
         self.__consistency_level: Optional[ConsistencyLevel] = consistency_level
+        self.__vectorizer_batching = vectorizer_batching
 
         self.__batch_grpc = _BatchGRPC(connection, self.__consistency_level)
         self.__batch_rest = _BatchRESTAsync(connection, self.__consistency_level)
 
         # lookup table for objects that are currently being processed - is used to not send references from objects that have not been added yet
         self.__uuid_lookup_lock = threading.Lock()
         self.__uuid_lookup: Set[str] = set()
@@ -195,27 +201,33 @@
             #  3000 objects, 1000/min -> 3 batches of 1000 objects, send every 20 seconds
             self.__concurrent_requests = (
                 self.__batching_mode.requests_per_minute + self.__max_batch_size
             ) // self.__max_batch_size
             self.__recommended_num_objects = (
                 self.__batching_mode.requests_per_minute // self.__concurrent_requests
             )
-        else:
-            assert isinstance(self.__batching_mode, _DynamicBatching)
+        elif isinstance(self.__batching_mode, _DynamicBatching) and not self.__vectorizer_batching:
             self.__recommended_num_objects = 10
             self.__concurrent_requests = 2
+        else:
+            assert isinstance(self.__batching_mode, _DynamicBatching) and self.__vectorizer_batching
+            self.__recommended_num_objects = VECTORIZER_BATCHING_STEP_SIZE
+            self.__concurrent_requests = 2
+            self.__dynamic_batching_sleep_time: int = 0
+            self._batch_send: bool = False
 
         self.__recommended_num_refs: int = 50
 
         self.__active_requests = 0
         self.__active_requests_lock = threading.Lock()
 
         # dynamic batching
         self.__time_last_scale_up: float = 0
-        self.__max_observed_rate: int = 0
+        self.__rate_queue: deque = deque(maxlen=50)  # 5s with 0.1s refresh rate
+        self.__took_queue: deque = deque(maxlen=CONCURRENT_REQUESTS_DYNAMIC_VECTORIZER)
 
         # fixed rate batching
         self.__time_stamp_last_request: float = 0
         # do 62 secs to give us some buffer to the "per-minute" calculation
         self.__fix_rate_batching_base_time = 62
 
         self.__bg_thread = self.__start_bg_threads()
@@ -272,59 +284,76 @@
         )
 
     def __batch_send(self) -> None:
         loop = self.__start_new_event_loop()
         future = asyncio.run_coroutine_threadsafe(self.__connection.aopen(), loop)
         future.result()  # Wait for self._connection.aopen() to finish
         refresh_time: float = 0.01
-        while (
-            self.__shut_background_thread_down is not None
-            and not self.__shut_background_thread_down.is_set()
-        ):
-            if isinstance(self.__batching_mode, _RateLimitedBatching):
-                if (
-                    time.time() - self.__time_stamp_last_request
-                    < self.__fix_rate_batching_base_time // self.__concurrent_requests
-                ):
-                    time.sleep(1)
-                    continue
-                self.__time_stamp_last_request = time.time()
-                refresh_time = 0
 
-            if self.__active_requests < self.__concurrent_requests and (
-                len(self.__batch_objects) > 0 or len(self.__batch_references) > 0
+        try:
+            while (
+                self.__shut_background_thread_down is not None
+                and not self.__shut_background_thread_down.is_set()
             ):
-                self.__active_requests_lock.acquire()
-                self.__active_requests += 1
-                self.__active_requests_lock.release()
-
-                objs = self.__batch_objects.pop_items(self.__recommended_num_objects)
-                self.__uuid_lookup_lock.acquire()
-                refs = self.__batch_references.pop_items(
-                    self.__recommended_num_refs, uuid_lookup=self.__uuid_lookup
-                )
-                self.__uuid_lookup_lock.release()
-                # do not block the thread - the results are written to a central (locked) list and we want to have multiple concurrent batch-requests
-                asyncio.run_coroutine_threadsafe(
-                    self.__send_batch_async(
-                        objs,
-                        refs,
-                        readd_rate_limit=isinstance(self.__batching_mode, _RateLimitedBatching),
-                    ),
-                    loop,
-                )
+                if isinstance(self.__batching_mode, _RateLimitedBatching):
+                    if (
+                        time.time() - self.__time_stamp_last_request
+                        < self.__fix_rate_batching_base_time // self.__concurrent_requests
+                    ):
+                        time.sleep(1)
+                        continue
+                    self.__time_stamp_last_request = time.time()
+                    refresh_time = 0
+                elif (
+                    isinstance(self.__batching_mode, _DynamicBatching)
+                    and self.__vectorizer_batching
+                ):
+                    if self.__dynamic_batching_sleep_time > 0:
+                        if (
+                            time.time() - self.__time_stamp_last_request
+                            < self.__dynamic_batching_sleep_time
+                        ):
+                            time.sleep(1)
+                            continue
 
-            time.sleep(refresh_time)
+                    self.__time_stamp_last_request = time.time()
+
+                if self.__active_requests < self.__concurrent_requests and (
+                    len(self.__batch_objects) > 0 or len(self.__batch_references) > 0
+                ):
+                    self._batch_send = True
+                    self.__active_requests_lock.acquire()
+                    self.__active_requests += 1
+                    self.__active_requests_lock.release()
+
+                    objs = self.__batch_objects.pop_items(self.__recommended_num_objects)
+                    self.__uuid_lookup_lock.acquire()
+                    refs = self.__batch_references.pop_items(
+                        self.__recommended_num_refs, uuid_lookup=self.__uuid_lookup
+                    )
+                    self.__uuid_lookup_lock.release()
+                    # do not block the thread - the results are written to a central (locked) list and we want to have multiple concurrent batch-requests
+                    asyncio.run_coroutine_threadsafe(
+                        self.__send_batch_async(
+                            objs,
+                            refs,
+                            readd_rate_limit=isinstance(self.__batching_mode, _RateLimitedBatching),
+                        ),
+                        loop,
+                    )
 
-        future = asyncio.run_coroutine_threadsafe(self.__connection.aclose(), loop)
-        future.result()  # Wait for self._connection.aclose() to finish
-        loop.call_soon_threadsafe(loop.stop)
+                time.sleep(refresh_time)
+
+        finally:
+            future = asyncio.run_coroutine_threadsafe(self.__connection.aclose(), loop)
+            future.result()  # Wait for self._connection.aclose() to finish
+            loop.call_soon_threadsafe(loop.stop)
 
     def dynamic_batch_rate_loop(self) -> None:
-        refresh_time = 0.1
+        refresh_time = 1
         while (
             self.__shut_background_thread_down is not None
             and not self.__shut_background_thread_down.is_set()
         ):
             if not isinstance(self.__batching_mode, _DynamicBatching):
                 return
 
@@ -371,61 +400,96 @@
         if "batchStats" not in status[0] or "queueLength" not in status[0]["batchStats"]:
             # async indexing - just send a lot
             self.__batching_mode = _FixedSizeBatching(1000, 10)
             self.__recommended_num_objects = 1000
             self.__concurrent_requests = 10
             return
 
-        rate = status[0]["batchStats"]["ratePerSecond"]
+        rate: int = status[0]["batchStats"]["ratePerSecond"]
         rate_per_worker = rate / self.__concurrent_requests
 
         batch_length = status[0]["batchStats"]["queueLength"]
 
-        if rate > self.__max_observed_rate:
-            self.__max_observed_rate = rate
-
-        if batch_length == 0:  # scale up if queue is empty
-            self.__recommended_num_objects = min(
-                self.__recommended_num_objects + 50,
-                self.__max_batch_size,
-            )
+        self.__rate_queue.append(rate)
 
-            if (
-                self.__max_batch_size == self.__recommended_num_objects
-                and len(self.__batch_objects) > self.__recommended_num_objects
-                and time.time() - self.__time_last_scale_up > 1
-                and self.__concurrent_requests < MAX_CONCURRENT_REQUESTS
-            ):
-                self.__concurrent_requests += 1
-                self.__time_last_scale_up = time.time()
+        if self.__vectorizer_batching:
+            # slow vectorizer, we want to send larger batches that can take a bit longer, but fewer of them. We might need to sleep
+            if len(self.__took_queue) > 0 and self._batch_send:
+                max_took = max(self.__took_queue)
+                self.__dynamic_batching_sleep_time = 0
+                if max_took > 2 * BATCH_TIME_TARGET:
+                    self.__concurrent_requests = 1
+                    self.__recommended_num_objects = VECTORIZER_BATCHING_STEP_SIZE
+                elif max_took > BATCH_TIME_TARGET:
+                    current_step = self.__recommended_num_objects // VECTORIZER_BATCHING_STEP_SIZE
+
+                    if self.__concurrent_requests > 1:
+                        self.__concurrent_requests -= 1
+                    elif current_step > 1:
+                        self.__recommended_num_objects = VECTORIZER_BATCHING_STEP_SIZE * (
+                            current_step - 1
+                        )
+                    else:
+                        # cannot scale down, sleep a bit
+                        self.__dynamic_batching_sleep_time = max_took - BATCH_TIME_TARGET
+
+                elif max_took < 3 * BATCH_TIME_TARGET // 4:
+                    if self.__dynamic_batching_sleep_time > 0:
+                        self.__dynamic_batching_sleep_time = 0
+                    elif self.__concurrent_requests < 3:
+                        self.__concurrent_requests += 1
+                    else:
+                        current_step = (
+                            self.__recommended_num_objects // VECTORIZER_BATCHING_STEP_SIZE
+                        )
+                        self.__recommended_num_objects = VECTORIZER_BATCHING_STEP_SIZE * (
+                            current_step + 1
+                        )
+                self._batch_send = False
 
         else:
-            ratio = batch_length / rate
-            if 2.1 > ratio > 1.9:  # ideal, send exactly as many objects as weaviate can process
-                self.__recommended_num_objects = math.floor(rate_per_worker)
-            elif ratio <= 1.9:  # we can send more
-                self.__recommended_num_objects = math.floor(
-                    min(
-                        self.__recommended_num_objects * 1.5,
-                        rate_per_worker * 2 / ratio,
-                    )
+            if batch_length == 0:  # scale up if queue is empty
+                self.__recommended_num_objects = min(
+                    self.__recommended_num_objects + 50,
+                    self.__max_batch_size,
                 )
 
-                if self.__max_batch_size == self.__recommended_num_objects:
+                if (
+                    self.__max_batch_size == self.__recommended_num_objects
+                    and len(self.__batch_objects) > self.__recommended_num_objects
+                    and time.time() - self.__time_last_scale_up > 1
+                    and self.__concurrent_requests < MAX_CONCURRENT_REQUESTS
+                ):
                     self.__concurrent_requests += 1
+                    self.__time_last_scale_up = time.time()
+
+            else:
+                ratio = batch_length / rate
+                if 2.1 > ratio > 1.9:  # ideal, send exactly as many objects as weaviate can process
+                    self.__recommended_num_objects = math.floor(rate_per_worker)
+                elif ratio <= 1.9:  # we can send more
+                    self.__recommended_num_objects = math.floor(
+                        min(
+                            self.__recommended_num_objects * 1.5,
+                            rate_per_worker * 2 / ratio,
+                        )
+                    )
 
-            elif ratio < 10:  # too high, scale down
-                self.__recommended_num_objects = math.floor(rate_per_worker * 2 / ratio)
+                    if self.__max_batch_size == self.__recommended_num_objects:
+                        self.__concurrent_requests += 1
 
-                if self.__recommended_num_objects < 100 and self.__concurrent_requests > 2:
-                    self.__concurrent_requests -= 1
+                elif ratio < 10:  # too high, scale down
+                    self.__recommended_num_objects = math.floor(rate_per_worker * 2 / ratio)
 
-            else:  # way too high, stop sending new batches
-                self.__recommended_num_objects = 0
-                self.__concurrent_requests = 2
+                    if self.__recommended_num_objects < 100 and self.__concurrent_requests > 2:
+                        self.__concurrent_requests -= 1
+
+                else:  # way too high, stop sending new batches
+                    self.__recommended_num_objects = 0
+                    self.__concurrent_requests = 2
 
     async def __send_batch_async(
         self, objs: List[_BatchObject], refs: List[_BatchReference], readd_rate_limit: bool
     ) -> None:
         if len(objs) > 0:
             start = time.time()
             try:
@@ -441,69 +505,71 @@
                     elapsed_seconds=time.time() - start,
                     errors=errors_obj,
                     has_errors=True,
                     uuids={},
                 )
 
             readded_uuids = set()
-            if readd_rate_limit:
-                readded_objects = []
-                highest_retry_count = 0
-                for i, err in response_obj.errors.items():
-                    if ("support@cohere.com" in err.message and "rate limit" in err.message) or (
-                        "OpenAI" in err.message
-                        and (
-                            "Rate limit reached" in err.message
-                            or "on tokens per min (TPM)" in err.message
-                            or "503 error: Service Unavailable." in err.message
-                            or "500 error: The server had an error while processing your request."
-                            in err.message
-                        )
-                    ):
-                        if err.object_.retry_count > highest_retry_count:
-                            highest_retry_count = err.object_.retry_count
-
-                        if err.object_.retry_count > 5:
-                            continue  # too many retries, give up
-                        err.object_.retry_count += 1
-                        readded_objects.append(i)
-
-                if len(readded_objects) > 0:
-                    _Warnings.batch_rate_limit_reached(
-                        response_obj.errors[readded_objects[0]].message,
-                        self.__fix_rate_batching_base_time * (highest_retry_count + 1),
+            readded_objects = []
+            highest_retry_count = 0
+            for i, err in response_obj.errors.items():
+                if (
+                    "support@cohere.com" in err.message
+                    and (
+                        "rate limit" in err.message
+                        or "500 error: internal server error" in err.message
                     )
-
-                    readd_objects = [
-                        err.object_
-                        for i, err in response_obj.errors.items()
-                        if i in readded_objects
-                    ]
-                    readded_uuids = {obj.uuid for obj in readd_objects}
-
-                    self.__batch_objects.prepend(readd_objects)
-
-                    new_errors = {
-                        i: err for i, err in response_obj.errors.items() if i not in readded_objects
-                    }
-                    response_obj = BatchObjectReturn(
-                        uuids={
-                            i: uid
-                            for i, uid in response_obj.uuids.items()
-                            if i not in readded_objects
-                        },
-                        errors=new_errors,
-                        has_errors=len(new_errors) > 0,
-                        all_responses=[
-                            err
-                            for i, err in enumerate(response_obj.all_responses)
-                            if i not in readded_objects
-                        ],
-                        elapsed_seconds=response_obj.elapsed_seconds,
+                ) or (
+                    "OpenAI" in err.message
+                    and (
+                        "Rate limit reached" in err.message
+                        or "on tokens per min (TPM)" in err.message
+                        or "503 error: Service Unavailable." in err.message
+                        or "500 error: The server had an error while processing your request."
+                        in err.message
                     )
+                ):
+                    if err.object_.retry_count > highest_retry_count:
+                        highest_retry_count = err.object_.retry_count
+
+                    if err.object_.retry_count > 5:
+                        continue  # too many retries, give up
+                    err.object_.retry_count += 1
+                    readded_objects.append(i)
+
+            if len(readded_objects) > 0:
+                _Warnings.batch_rate_limit_reached(
+                    response_obj.errors[readded_objects[0]].message,
+                    self.__fix_rate_batching_base_time * (highest_retry_count + 1),
+                )
+
+                readd_objects = [
+                    err.object_ for i, err in response_obj.errors.items() if i in readded_objects
+                ]
+                readded_uuids = {obj.uuid for obj in readd_objects}
+
+                self.__batch_objects.prepend(readd_objects)
+
+                new_errors = {
+                    i: err for i, err in response_obj.errors.items() if i not in readded_objects
+                }
+                response_obj = BatchObjectReturn(
+                    uuids={
+                        i: uid for i, uid in response_obj.uuids.items() if i not in readded_objects
+                    },
+                    errors=new_errors,
+                    has_errors=len(new_errors) > 0,
+                    all_responses=[
+                        err
+                        for i, err in enumerate(response_obj.all_responses)
+                        if i not in readded_objects
+                    ],
+                    elapsed_seconds=response_obj.elapsed_seconds,
+                )
+                if readd_rate_limit:
                     self.__time_stamp_last_request = (
                         time.time() + self.__fix_rate_batching_base_time * (highest_retry_count + 1)
                     )  # skip a full minute to recover from the rate limit
                     self.__fix_rate_batching_base_time += (
                         1  # increase the base time as the current one is too low
                     )
             self.__uuid_lookup_lock.acquire()
@@ -512,14 +578,15 @@
             )
             self.__uuid_lookup_lock.release()
 
             self.__results_lock.acquire()
             self.__results_for_wrapper.results.objs += response_obj
             self.__results_for_wrapper.failed_objects.extend(response_obj.errors.values())
             self.__results_lock.release()
+            self.__took_queue.append(time.time() - start)
 
         if len(refs) > 0:
             start = time.time()
             try:
                 response_ref = await self.__batch_rest.references(references=refs)
 
             except Exception as e:
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/batch/batch_wrapper.py` & `weaviate_client-4.6.0b0/weaviate/collections/batch/batch_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 from weaviate.collections.classes.batch import BatchResult, ErrorObject, ErrorReference, Shard
 from weaviate.collections.classes.config import ConsistencyLevel
 from weaviate.connect import ConnectionV4
 from weaviate.util import _capitalize_first_letter, _decode_json_response_list
 
 
 class _BatchWrapper:
-    def __init__(
-        self, connection: ConnectionV4, consistency_level: Optional[ConsistencyLevel] = None
-    ):
+    def __init__(self, connection: ConnectionV4, consistency_level: Optional[ConsistencyLevel]):
         self._connection = connection
         self._consistency_level = consistency_level
         self._current_batch: Optional[_BatchBase] = None
         # config options
         self._batch_mode: _BatchMode = _DynamicBatching()
 
         self._batch_data = _BatchDataWrapper()
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/batch/client.py` & `weaviate_client-4.6.0b0/weaviate/collections/batch/collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,191 @@
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Generic, List, Optional, Union
 
 from weaviate.collections.batch.base import (
     _BatchBase,
     _BatchDataWrapper,
+    _BatchMode,
     _DynamicBatching,
     _FixedSizeBatching,
     _RateLimitedBatching,
 )
-from weaviate.collections.batch.batch_wrapper import (
-    _BatchWrapper,
-    _BatchMode,
-    _ContextManagerWrapper,
-)
-from weaviate.collections.classes.config import ConsistencyLevel
-from weaviate.collections.classes.internal import ReferenceInput, ReferenceInputs
-from weaviate.collections.classes.tenants import Tenant
-from weaviate.collections.classes.types import WeaviateProperties
+from weaviate.collections.batch.batch_wrapper import _BatchWrapper, _ContextManagerWrapper
+from weaviate.collections.classes.config import ConsistencyLevel, Vectorizers
+from weaviate.collections.classes.internal import ReferenceInputs, ReferenceInput
+from weaviate.collections.classes.types import Properties
+from weaviate.connect import ConnectionV4
 from weaviate.types import UUID, VECTORS
 
+if TYPE_CHECKING:
+    from weaviate.collections.config import _ConfigCollection
+
+
+class _BatchCollection(Generic[Properties], _BatchBase):
+    def __init__(
+        self,
+        connection: ConnectionV4,
+        consistency_level: Optional[ConsistencyLevel],
+        results: _BatchDataWrapper,
+        batch_mode: _BatchMode,
+        name: str,
+        tenant: Optional[str],
+        vectorizer_batching: bool,
+    ) -> None:
+        super().__init__(
+            connection=connection,
+            consistency_level=consistency_level,
+            results=results,
+            batch_mode=batch_mode,
+            vectorizer_batching=vectorizer_batching,
+        )
+        self.__name = name
+        self.__tenant = tenant
 
-class _BatchClient(_BatchBase):
     def add_object(
         self,
-        collection: str,
-        properties: Optional[WeaviateProperties] = None,
+        properties: Optional[Properties] = None,
         references: Optional[ReferenceInputs] = None,
         uuid: Optional[UUID] = None,
         vector: Optional[VECTORS] = None,
-        tenant: Optional[Union[str, Tenant]] = None,
     ) -> UUID:
-        """
-        Add one object to this batch.
+        """Add one object to this batch.
 
-        NOTE: If the UUID of one of the objects already exists then the existing object will be
-        replaced by the new object.
+        NOTE: If the UUID of one of the objects already exists then the existing object will be replaced by the new object.
 
         Arguments:
-            `collection`
-                The name of the collection this object belongs to.
             `properties`
                 The data properties of the object to be added as a dictionary.
             `references`
                 The references of the object to be added as a dictionary.
             `uuid`:
-                The UUID of the object as an uuid.UUID object or str. It can be a Weaviate beacon or Weaviate href.
-                If it is None an UUIDv4 will generated, by default None
+                The UUID of the object as an uuid.UUID object or str. If it is None an UUIDv4 will generated, by default None
             `vector`:
                 The embedding of the object. Can be used when a collection does not have a vectorization module or the given
                 vector was generated using the _identical_ vectorization module that is configured for the class. In this
                 case this vector takes precedence.
                 Supported types are
                 - for single vectors: `list`, 'numpy.ndarray`, `torch.Tensor` and `tf.Tensor`, by default None.
                 - for named vectors: Dict[str, *list above*], where the string is the name of the vector.
-            `tenant`
-                The tenant name or Tenant object to be used for this request.
 
         Returns:
             `str`
                 The UUID of the added object. If one was not provided a UUIDv4 will be auto-generated for you and returned here.
 
         Raises:
             `WeaviateBatchValidationError`
                 If the provided options are in the format required by Weaviate.
         """
-        return super()._add_object(
-            collection=collection,
+        return self._add_object(
+            collection=self.__name,
             properties=properties,
             references=references,
             uuid=uuid,
             vector=vector,
-            tenant=tenant.name if isinstance(tenant, Tenant) else tenant,
+            tenant=self.__tenant,
         )
 
     def add_reference(
-        self,
-        from_uuid: UUID,
-        from_collection: str,
-        from_property: str,
-        to: ReferenceInput,
-        tenant: Optional[Union[str, Tenant]] = None,
+        self, from_uuid: UUID, from_property: str, to: Union[ReferenceInput, List[UUID]]
     ) -> None:
-        """Add one reference to this batch.
+        """Add a reference to this batch.
 
         Arguments:
             `from_uuid`
                 The UUID of the object, as an uuid.UUID object or str, that should reference another object.
-            `from_collection`
-                The name of the collection that should reference another object.
             `from_property`
                 The name of the property that contains the reference.
             `to`
                 The UUID of the referenced object, as an uuid.UUID object or str, that is actually referenced.
                 For multi-target references use wvc.Reference.to_multi_target().
-            `tenant`
-                The tenant name or Tenant object to be used for this request.
 
         Raises:
             `WeaviateBatchValidationError`
                 If the provided options are in the format required by Weaviate.
         """
-        super()._add_reference(
-            from_object_uuid=from_uuid,
-            from_object_collection=from_collection,
-            from_property_name=from_property,
-            to=to,
-            tenant=tenant.name if isinstance(tenant, Tenant) else tenant,
+        self._add_reference(
+            from_uuid,
+            self.__name,
+            from_property,
+            to,
+            self.__tenant,
         )
 
 
-class _BatchClientWrapper(_BatchWrapper):
-    def __create_batch_and_reset(self) -> _ContextManagerWrapper[_BatchClient]:
+class _BatchCollectionWrapper(Generic[Properties], _BatchWrapper):
+    def __init__(
+        self,
+        connection: ConnectionV4,
+        consistency_level: Optional[ConsistencyLevel],
+        name: str,
+        tenant: Optional[str],
+        config: "_ConfigCollection",
+    ) -> None:
+        super().__init__(connection, consistency_level)
+        self.__name = name
+        self.__tenant = tenant
+        self.__config = config
+        self._vectorizer_batching: Optional[bool] = None
+
+    def __create_batch_and_reset(self) -> _ContextManagerWrapper[_BatchCollection[Properties]]:
+        if self._vectorizer_batching is None:
+            config = self.__config.get(simple=True)
+            if config.vector_config is not None:
+                vectorizer_batching = False
+                for vec_config in config.vector_config.values():
+                    if vec_config.vectorizer.vectorizer is not Vectorizers.NONE:
+                        vectorizer_batching = True
+                        break
+                self._vectorizer_batching = vectorizer_batching
+            else:
+                self._vectorizer_batching = config.vectorizer is not Vectorizers.NONE
+
         self._batch_data = _BatchDataWrapper()  # clear old data
         return _ContextManagerWrapper(
-            _BatchClient(
+            _BatchCollection[Properties](
                 connection=self._connection,
                 consistency_level=self._consistency_level,
                 results=self._batch_data,
                 batch_mode=self._batch_mode,
+                name=self.__name,
+                tenant=self.__tenant,
+                vectorizer_batching=self._vectorizer_batching,
             )
         )
 
-    def dynamic(
-        self, consistency_level: Optional[ConsistencyLevel] = None
-    ) -> _ContextManagerWrapper[_BatchClient]:
+    def dynamic(self) -> _ContextManagerWrapper[_BatchCollection[Properties]]:
         """Configure dynamic batching.
 
         When you exit the context manager, the final batch will be sent automatically.
-
-        Arguments:
-            `consistency_level`
-                The consistency level to be used to send batches. If not provided, the default value is `None`.
         """
         self._batch_mode: _BatchMode = _DynamicBatching()
-        self._consistency_level = consistency_level
         return self.__create_batch_and_reset()
 
     def fixed_size(
-        self,
-        batch_size: int = 100,
-        concurrent_requests: int = 2,
-        consistency_level: Optional[ConsistencyLevel] = None,
-    ) -> _ContextManagerWrapper[_BatchClient]:
+        self, batch_size: int = 100, concurrent_requests: int = 2
+    ) -> _ContextManagerWrapper[_BatchCollection[Properties]]:
         """Configure fixed size batches. Note that the default is dynamic batching.
 
         When you exit the context manager, the final batch will be sent automatically.
 
         Arguments:
             `batch_size`
                 The number of objects/references to be sent in one batch. If not provided, the default value is 100.
             `concurrent_requests`
                 The number of concurrent requests when sending batches. This controls the number of concurrent requests
                 made to Weaviate and not the speed of batch creation within Python.
-            `consistency_level`
-                The consistency level to be used to send batches. If not provided, the default value is `None`.
-
         """
         self._batch_mode = _FixedSizeBatching(batch_size, concurrent_requests)
-        self._consistency_level = consistency_level
         return self.__create_batch_and_reset()
 
     def rate_limit(
-        self, requests_per_minute: int, consistency_level: Optional[ConsistencyLevel] = None
-    ) -> _ContextManagerWrapper[_BatchClient]:
+        self, requests_per_minute: int
+    ) -> _ContextManagerWrapper[_BatchCollection[Properties]]:
         """Configure batches with a rate limited vectorizer.
 
         When you exit the context manager, the final batch will be sent automatically.
 
         Arguments:
             `requests_per_minute`
                 The number of requests that the vectorizer can process per minute.
-            `consistency_level`
-                The consistency level to be used to send batches. If not provided, the default value is `None`.
         """
         self._batch_mode = _RateLimitedBatching(requests_per_minute)
-        self._consistency_level = consistency_level
         return self.__create_batch_and_reset()
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/batch/grpc_batch_delete.py` & `weaviate_client-4.6.0b0/weaviate/collections/batch/grpc_batch_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                     consistency_level=self._consistency_level,
                     verbose=verbose,
                     dry_run=dry_run,
                     tenant=tenant,
                     filters=_FilterToGRPC.convert(filters),
                 ),
                 metadata=metadata,
-                timeout=self._connection.timeout_config.connect,
+                timeout=self._connection.timeout_config.insert,
             )
 
             if verbose:
                 objects: List[DeleteManyObject] = [
                     DeleteManyObject(
                         uuid=_WeaviateUUIDInt(int.from_bytes(obj.uuid, byteorder="big")),
                         successful=obj.successful,
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/batch/grpc_batch_objects.py` & `weaviate_client-4.6.0b0/weaviate/collections/batch/grpc_batch_objects.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/batch/rest.py` & `weaviate_client-4.6.0b0/weaviate/collections/batch/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     ) -> None:
         self.__consistency_level = consistency_level
         self.__connection = connection
 
     async def references(self, references: List[_BatchReference]) -> BatchReferenceReturn:
         params: Dict[str, str] = {}
         if self.__consistency_level is not None:
-            params["consistency_level"] = self.__consistency_level
+            params["consistency_level"] = self.__consistency_level.value
 
         refs = [
             (
                 {"from": ref.from_, "to": ref.to}
                 if ref.tenant is None
                 else {"from": ref.from_, "to": ref.to, "tenant": ref.tenant}
             )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/aggregate.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/aggregate.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,21 +134,23 @@
     property_name: str
     count: bool
 
 
 class _MetricsText(_MetricsBase):
     top_occurrences_count: bool
     top_occurrences_value: bool
+    min_occurrences: Optional[int]
 
     def to_gql(self) -> str:
+        limit = f"(limit: {self.min_occurrences})" if self.min_occurrences is not None else ""
         body = " ".join(
             [
                 "count" if self.count else "",
                 (
-                    "topOccurrences {"
+                    "topOccurrences" + limit + " {"
                     if self.top_occurrences_count or self.top_occurrences_value
                     else ""
                 ),
                 "occurs" if self.top_occurrences_count else "",
                 "value" if self.top_occurrences_value else "",
                 "}" if self.top_occurrences_count or self.top_occurrences_value else "",
             ]
@@ -271,39 +273,43 @@
         self.__property = property_
 
     def text(
         self,
         count: bool = False,
         top_occurrences_count: bool = False,
         top_occurrences_value: bool = False,
+        min_occurrences: Optional[int] = None,
     ) -> _MetricsText:
         """Define the metrics to be returned for a TEXT or TEXT_ARRAY property when aggregating over a collection.
 
         If none of the arguments are provided then all metrics will be returned.
 
         Arguments:
             `count`
                 Whether to include the number of objects that contain this property.
             `top_occurrences_count`
                 Whether to include the number of the top occurrences of a property's value.
             `top_occurrences_value`
                 Whether to include the value of the top occurrences of a property's value.
+            `min_occurrences`
+                Only include entries with more occurrences than the given limit.
 
         Returns:
             A `_MetricsStr` object that includes the metrics to be returned.
         """
         if not any([count, top_occurrences_count, top_occurrences_value]):
             count = True
             top_occurrences_count = True
             top_occurrences_value = True
         return _MetricsText(
             property_name=self.__property,
             count=count,
             top_occurrences_count=top_occurrences_count,
             top_occurrences_value=top_occurrences_value,
+            min_occurrences=min_occurrences,
         )
 
     def integer(
         self,
         count: bool = False,
         maximum: bool = False,
         mean: bool = False,
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/batch.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/batch.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/cluster.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/cluster.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from dataclasses import dataclass
-from typing import Generic, List, TypeVar, cast
+from typing import Generic, List, Literal, Optional, TypeVar, cast
 
 from weaviate.cluster.types import Node as NodeREST, Shard as ShardREST
 
 
 @dataclass
 class Shard:
     """The properties of a single shard of a collection."""
 
     collection: str
     name: str
     node: str
     object_count: int
+    vector_indexing_status: Literal["READONLY", "INDEXING", "READY"]
+    vector_queue_length: int
+    compressed: bool
+    loaded: Optional[bool]  # not present in <1.24.x
 
 
 @dataclass
 class Stats:
     """The statistics of a collection."""
 
     object_count: int
@@ -49,18 +53,22 @@
                 shards=(
                     [
                         Shard(
                             collection=shard["class"],
                             name=shard["name"],
                             node=node["name"],
                             object_count=shard["objectCount"],
+                            vector_indexing_status=shard["vectorIndexingStatus"],
+                            vector_queue_length=shard["vectorQueueLength"],
+                            compressed=shard["compressed"],
+                            loaded=shard.get("loaded"),
                         )
                         for shard in cast(List[ShardREST], node["shards"])
                     ]
-                    if "shards" in node
+                    if "shards" in node and node["shards"] is not None
                     else []
                 ),
                 stats=(
                     Stats(
                         object_count=node["stats"]["objectCount"],
                         shard_count=node["stats"]["shardCount"],
                     )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/config.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,26 +37,28 @@
 from weaviate.collections.classes.config_vector_index import (
     _QuantizerConfigCreate,
     _VectorIndexConfigCreate,
     _VectorIndexConfigHNSWCreate,
     _VectorIndexConfigFlatCreate,
     _VectorIndexConfigHNSWUpdate,
     _VectorIndexConfigFlatUpdate,
+    _VectorIndexConfigDynamicCreate,
     _VectorIndexConfigSkipCreate,
     _VectorIndexConfigUpdate,
     VectorIndexType as VectorIndexTypeAlias,
 )
 
 from weaviate.collections.classes.config_named_vectors import (
     _NamedVectorConfigCreate,
     _NamedVectorConfigUpdate,
     _NamedVectors,
     _NamedVectorsUpdate,
 )
 from weaviate.exceptions import WeaviateInvalidInputError
+from weaviate.warnings import _Warnings
 
 # BC for direct imports
 Vectorizers: TypeAlias = VectorizersAlias
 VectorIndexType: TypeAlias = VectorIndexTypeAlias
 VectorDistances: TypeAlias = VectorDistancesAlias
 
 
@@ -124,20 +126,26 @@
             Tokenize by word.
         `WHITESPACE`
             Tokenize by whitespace.
         `LOWERCASE`
             Tokenize by lowercase.
         `FIELD`
             Tokenize by field.
+        `GSE`
+            Tokenize using GSE (for Chinese and Japanese).
+        `TRIGRAM`
+            Tokenize into trigrams.
     """
 
     WORD = "word"
     WHITESPACE = "whitespace"
     LOWERCASE = "lowercase"
     FIELD = "field"
+    GSE = "gse"
+    TRIGRAM = "trigram"
 
 
 class GenerativeSearches(str, Enum):
     """The available generative search modules in Weaviate.
 
     These modules generate text from text-based inputs.
     See the [docs](https://weaviate.io/developers/weaviate/modules/reader-generator-modules) for more details.
@@ -149,19 +157,21 @@
             Weaviate module backed by Cohere generative models.
         `PALM`
             Weaviate module backed by PaLM generative models.
         `AWS`
             Weaviate module backed by AWS Bedrock generative models.
     """
 
-    OPENAI = "generative-openai"
-    COHERE = "generative-cohere"
-    PALM = "generative-palm"
     AWS = "generative-aws"
     ANYSCALE = "generative-anyscale"
+    COHERE = "generative-cohere"
+    MISTRAL = "generative-mistral"
+    OCTOAI = "generative-octoai"
+    OPENAI = "generative-openai"
+    PALM = "generative-palm"
 
 
 class Rerankers(str, Enum):
     """The available reranker modules in Weaviate.
 
     These modules rerank the results of a search query.
     See the [docs](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules#re-ranking) for more details.
@@ -174,14 +184,15 @@
         `TRANSFORMERS`
             Weaviate module backed by Transformers reranking models.
     """
 
     NONE = "none"
     COHERE = "reranker-cohere"
     TRANSFORMERS = "reranker-transformers"
+    VOYAGEAI = "reranker-voyageai"
 
 
 class StopwordsPreset(str, Enum):
     """Preset stopwords to use in the `Stopwords` class.
 
     Attributes:
         `EN`
@@ -240,15 +251,15 @@
             schema["type"] = str(self.type_.value)
         if self.distribution is not None:
             schema["distribution"] = str(self.distribution.value)
         return schema
 
 
 class _PQConfigCreate(_QuantizerConfigCreate):
-    bitCompression: Optional[bool]
+    bitCompression: Optional[bool] = Field(default=None)
     centroids: Optional[int]
     encoder: _PQEncoderConfigCreate
     segments: Optional[int]
     trainingLimit: Optional[int]
 
     @staticmethod
     def quantizer_name() -> str:
@@ -261,15 +272,15 @@
 
     @staticmethod
     def quantizer_name() -> str:
         return "bq"
 
 
 class _PQConfigUpdate(_QuantizerConfigUpdate):
-    bitCompression: Optional[bool]
+    bitCompression: Optional[bool] = Field(default=None)
     centroids: Optional[int]
     enabled: Optional[bool]
     segments: Optional[int]
     trainingLimit: Optional[int]
     encoder: Optional[_PQEncoderConfigUpdate]
 
     @staticmethod
@@ -284,17 +295,15 @@
     def quantizer_name() -> str:
         return "bq"
 
 
 class _ShardingConfigCreate(_ConfigCreateModel):
     virtualPerPhysical: Optional[int]
     desiredCount: Optional[int]
-    actualCount: Optional[int]
     desiredVirtualCount: Optional[int]
-    actualVirtualCount: Optional[int]
     key: str = "_id"
     strategy: str = "hash"
     function: str = "murmur3"
 
 
 class _ReplicationConfigCreate(_ConfigCreateModel):
     factor: Optional[int]
@@ -339,32 +348,52 @@
     bm25: Optional[_BM25ConfigUpdate]
     cleanupIntervalSeconds: Optional[int]
     stopwords: Optional[_StopwordsUpdate]
 
 
 class _MultiTenancyConfigCreate(_ConfigCreateModel):
     enabled: bool
+    autoTenantCreation: Optional[bool]
 
 
 class _MultiTenancyConfigUpdate(_ConfigUpdateModel):
-    enabled: Optional[bool] = None
+    autoTenantCreation: Optional[bool] = None
 
 
 class _GenerativeConfigCreate(_ConfigCreateModel):
     generative: GenerativeSearches
 
 
 class _GenerativeAnyscale(_GenerativeConfigCreate):
     generative: GenerativeSearches = Field(
         default=GenerativeSearches.ANYSCALE, frozen=True, exclude=True
     )
     temperature: Optional[float]
     model: Optional[str]
 
 
+class _GenerativeOctoai(_GenerativeConfigCreate):
+    generative: GenerativeSearches = Field(
+        default=GenerativeSearches.OCTOAI, frozen=True, exclude=True
+    )
+    baseURL: Optional[str]
+    temperature: Optional[float]
+    maxTokens: Optional[int]
+    model: Optional[str]
+
+
+class _GenerativeMistral(_GenerativeConfigCreate):
+    generative: GenerativeSearches = Field(
+        default=GenerativeSearches.MISTRAL, frozen=True, exclude=True
+    )
+    temperature: Optional[float]
+    model: Optional[str]
+    maxTokens: Optional[int]
+
+
 class _GenerativeOpenAIConfigBase(_GenerativeConfigCreate):
     generative: GenerativeSearches = Field(
         default=GenerativeSearches.OPENAI, frozen=True, exclude=True
     )
     baseURL: Optional[AnyHttpUrl]
     frequencyPenaltyProperty: Optional[float]
     presencePenaltyProperty: Optional[float]
@@ -440,14 +469,22 @@
     model: Optional[Union[RerankerCohereModel, str]] = Field(default=None)
 
 
 class _RerankerTransformersConfig(_RerankerConfigCreate):
     reranker: Rerankers = Field(default=Rerankers.TRANSFORMERS, frozen=True, exclude=True)
 
 
+RerankerVoyageAIModel = Literal["rerank-lite-1"]
+
+
+class _RerankerVoyageAIConfig(_RerankerConfigCreate):
+    reranker: Rerankers = Field(default=Rerankers.VOYAGEAI, frozen=True, exclude=True)
+    model: Optional[Union[RerankerVoyageAIModel, str]] = Field(default=None)
+
+
 class _Generative:
     """Use this factory class to create the correct object for the `generative_config` argument in the `collections.create()` method.
 
     Each staticmethod provides options specific to the named generative search module in the function's name. Under-the-hood data validation steps
     will ensure that any mis-specifications will be caught before the request is sent to Weaviate.
     """
 
@@ -455,14 +492,34 @@
     def anyscale(
         model: Optional[str] = None,
         temperature: Optional[float] = None,
     ) -> _GenerativeConfigCreate:
         return _GenerativeAnyscale(model=model, temperature=temperature)
 
     @staticmethod
+    def mistral(
+        model: Optional[str] = None,
+        temperature: Optional[float] = None,
+        max_tokens: Optional[int] = None,
+    ) -> _GenerativeConfigCreate:
+        return _GenerativeMistral(model=model, temperature=temperature, maxTokens=max_tokens)
+
+    @staticmethod
+    def octoai(
+        *,
+        base_url: Optional[str] = None,
+        max_tokens: Optional[int] = None,
+        model: Optional[str] = None,
+        temperature: Optional[float] = None,
+    ) -> _GenerativeConfigCreate:
+        return _GenerativeOctoai(
+            baseURL=base_url, maxTokens=max_tokens, model=model, temperature=temperature
+        )
+
+    @staticmethod
     def openai(
         model: Optional[str] = None,
         frequency_penalty: Optional[float] = None,
         max_tokens: Optional[int] = None,
         presence_penalty: Optional[float] = None,
         temperature: Optional[float] = None,
         top_p: Optional[float] = None,
@@ -675,14 +732,29 @@
 
         Arguments:
             `model`
                 The model to use. Defaults to `None`, which uses the server-defined default
         """
         return _RerankerCohereConfig(model=model)
 
+    @staticmethod
+    def voyageai(
+        model: Optional[Union[RerankerVoyageAIModel, str]] = None,
+    ) -> _RerankerConfigCreate:
+        """Create a `_RerankerVoyageAIConfig` object for use when reranking using the `reranker-voyageai` module.
+
+        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/reranker-voyageai)
+        for detailed usage.
+
+        Arguments:
+            `model`
+                The model to use. Defaults to `None`, which uses the server-defined default
+        """
+        return _RerankerVoyageAIConfig(model=model)
+
 
 class _CollectionConfigCreateBase(_ConfigCreateModel):
     description: Optional[str] = Field(default=None)
     invertedIndexConfig: Optional[_InvertedIndexConfigCreate] = Field(
         default=None, alias="inverted_index_config"
     )
     multiTenancyConfig: Optional[_MultiTenancyConfigCreate] = Field(
@@ -750,26 +822,33 @@
     )
     vectorIndexConfig: Optional[_VectorIndexConfigUpdate] = Field(
         default=None, alias="vector_index_config"
     )
     vectorizerConfig: Optional[
         Union[_VectorIndexConfigUpdate, List[_NamedVectorConfigUpdate]]
     ] = Field(default=None, alias="vectorizer_config")
+    multiTenancyConfig: Optional[_MultiTenancyConfigUpdate] = Field(
+        default=None, alias="multi_tenancy_config"
+    )
 
     def merge_with_existing(self, schema: Dict[str, Any]) -> Dict[str, Any]:
         if self.description is not None:
             schema["description"] = self.description
         if self.invertedIndexConfig is not None:
             schema["invertedIndexConfig"] = self.invertedIndexConfig.merge_with_existing(
                 schema["invertedIndexConfig"]
             )
         if self.replicationConfig is not None:
             schema["replicationConfig"] = self.replicationConfig.merge_with_existing(
                 schema["replicationConfig"]
             )
+        if self.multiTenancyConfig is not None:
+            schema["multiTenancyConfig"] = self.multiTenancyConfig.merge_with_existing(
+                schema["multiTenancyConfig"]
+            )
         if self.vectorIndexConfig is not None:
             schema["vectorIndexConfig"] = self.vectorIndexConfig.merge_with_existing(
                 schema["vectorIndexConfig"]
             )
         if self.vectorizerConfig is not None:
             if isinstance(self.vectorizerConfig, _VectorIndexConfigUpdate):
                 schema["vectorIndexConfig"] = self.vectorizerConfig.merge_with_existing(
@@ -835,14 +914,15 @@
 
 InvertedIndexConfig = _InvertedIndexConfig
 
 
 @dataclass
 class _MultiTenancyConfig(_ConfigBase):
     enabled: bool
+    auto_tenant_creation: bool
 
 
 MultiTenancyConfig = _MultiTenancyConfig
 
 
 @dataclass
 class _PropertyVectorizerConfig:
@@ -964,20 +1044,25 @@
 
 
 PQEncoderConfig = _PQEncoderConfig
 
 
 @dataclass
 class _PQConfig(_ConfigBase):
-    bit_compression: bool
+    internal_bit_compression: bool
     segments: int
     centroids: int
     training_limit: int
     encoder: PQEncoderConfig
 
+    @property
+    def bit_compression(self) -> bool:
+        _Warnings.bit_compression_in_pq_config()
+        return self.internal_bit_compression
+
 
 PQConfig = _PQConfig
 
 
 @dataclass
 class _BQConfig(_ConfigBase):
     cache: Optional[bool]
@@ -1032,14 +1117,29 @@
         return VectorIndexType.FLAT.value
 
 
 VectorIndexConfigFlat = _VectorIndexConfigFlat
 
 
 @dataclass
+class _VectorIndexConfigDynamic(_VectorIndexConfig):
+    distance_metric: VectorDistances
+    hnsw: Optional[VectorIndexConfigHNSW]
+    flat: Optional[VectorIndexConfigFlat]
+    threshold: Optional[int]
+
+    @staticmethod
+    def vector_index_type() -> str:
+        return VectorIndexType.DYNAMIC.value
+
+
+VectorIndexConfigDynamic = _VectorIndexConfigDynamic
+
+
+@dataclass
 class _GenerativeConfig(_ConfigBase):
     generative: GenerativeSearches
     model: Dict[str, Any]
 
 
 GenerativeConfig = _GenerativeConfig
 
@@ -1074,15 +1174,17 @@
         ret_dict["properties"] = ret_dict.pop("sourceProperties", None)
         return ret_dict
 
 
 @dataclass
 class _NamedVectorConfig(_ConfigBase):
     vectorizer: _NamedVectorizerConfig
-    vector_index_config: Union[VectorIndexConfigHNSW, VectorIndexConfigFlat]
+    vector_index_config: Union[
+        VectorIndexConfigHNSW, VectorIndexConfigFlat, VectorIndexConfigDynamic
+    ]
 
     def to_dict(self) -> Dict:
         ret_dict = super().to_dict()
         ret_dict["vectorIndexType"] = self.vector_index_config.vector_index_type()
         return ret_dict
 
 
@@ -1097,15 +1199,17 @@
     inverted_index_config: InvertedIndexConfig
     multi_tenancy_config: MultiTenancyConfig
     properties: List[PropertyConfig]
     references: List[ReferencePropertyConfig]
     replication_config: ReplicationConfig
     reranker_config: Optional[RerankerConfig]
     sharding_config: Optional[ShardingConfig]
-    vector_index_config: Union[VectorIndexConfigHNSW, VectorIndexConfigFlat, None]
+    vector_index_config: Union[
+        VectorIndexConfigHNSW, VectorIndexConfigFlat, VectorIndexConfigDynamic, None
+    ]
     vector_index_type: Optional[VectorIndexType]
     vectorizer_config: Optional[VectorizerConfig]
     vectorizer: Optional[Vectorizers]
     vector_config: Optional[Dict[str, _NamedVectorConfig]]
 
     def to_dict(self) -> dict:
         out = super().to_dict()
@@ -1438,16 +1542,17 @@
         """Create a `_PQConfigCreate` object to be used when defining the product quantization (PQ) configuration of Weaviate.
 
         Use this method when defining the `quantizer` argument in the `vector_index` configuration.
 
         Arguments:
             See [the docs](https://weaviate.io/developers/weaviate/concepts/vector-index#hnsw-with-compression) for a more detailed view!
         """  # noqa: D417 (missing argument descriptions in the docstring)
+        if bit_compression is not None:
+            _Warnings.bit_compression_in_pq_config()
         return _PQConfigCreate(
-            bitCompression=bit_compression,
             centroids=centroids,
             segments=segments,
             trainingLimit=training_limit,
             encoder=_PQEncoderConfigCreate(type_=encoder_type, distribution=encoder_distribution),
         )
 
     @staticmethod
@@ -1533,14 +1638,39 @@
         """  # noqa: D417 (missing argument descriptions in the docstring)
         return _VectorIndexConfigFlatCreate(
             distance=distance_metric,
             vectorCacheMaxObjects=vector_cache_max_objects,
             quantizer=quantizer,
         )
 
+    @staticmethod
+    def dynamic(
+        distance_metric: Optional[VectorDistances] = None,
+        threshold: Optional[int] = None,
+        hnsw: Optional[_VectorIndexConfigHNSWCreate] = None,
+        flat: Optional[_VectorIndexConfigFlatCreate] = None,
+        vector_cache_max_objects: Optional[int] = None,
+        quantizer: Optional[_BQConfigCreate] = None,
+    ) -> _VectorIndexConfigDynamicCreate:
+        """Create a `_VectorIndexConfigDynamicCreate` object to be used when defining the DYNAMIC vector index configuration of Weaviate.
+
+        Use this method when defining the `vector_index_config` argument in `collections.create()`.
+
+        Arguments:
+            See [the docs](https://weaviate.io/developers/weaviate/configuration/indexes#how-to-configure-hnsw) for a more detailed view!
+        """  # noqa: D417 (missing argument descriptions in the docstring)
+        return _VectorIndexConfigDynamicCreate(
+            distance=distance_metric,
+            threshold=threshold,
+            hnsw=hnsw,
+            flat=flat,
+            vectorCacheMaxObjects=vector_cache_max_objects,
+            quantizer=quantizer,
+        )
+
 
 class Configure:
     """Use this factory class to generate the correct object for use when using the `collections.create()` method. E.g., `.multi_tenancy()` will return a `MultiTenancyConfigCreate` object to be used in the `multi_tenancy_config` argument.
 
     Each class method provides options specific to the named configuration type in the function's name. Under-the-hood data validation steps
     will ensure that any mis-specifications are caught before the request is sent to Weaviate.
     """
@@ -1585,22 +1715,26 @@
                 preset=stopwords_preset,
                 additions=stopwords_additions,
                 removals=stopwords_removals,
             ),
         )
 
     @staticmethod
-    def multi_tenancy(enabled: bool = True) -> _MultiTenancyConfigCreate:
+    def multi_tenancy(
+        enabled: bool = True, auto_tenant_creation: bool = False
+    ) -> _MultiTenancyConfigCreate:
         """Create a `MultiTenancyConfigCreate` object to be used when defining the multi-tenancy configuration of Weaviate.
 
         Arguments:
             `enabled`
                 Whether multi-tenancy is enabled. Defaults to `True`.
+            `auto_tenant_creation`
+                Automatically create nonexistent tenants during batch import. Defaults to `False`
         """
-        return _MultiTenancyConfigCreate(enabled=enabled)
+        return _MultiTenancyConfigCreate(enabled=enabled, autoTenantCreation=auto_tenant_creation)
 
     @staticmethod
     def replication(factor: Optional[int] = None) -> _ReplicationConfigCreate:
         """Create a `ReplicationConfigCreate` object to be used when defining the replication configuration of Weaviate.
 
         Arguments:
             `factor`
@@ -1623,27 +1757,31 @@
         See [the docs](https://weaviate.io/developers/weaviate/concepts/replication-architecture#replication-vs-sharding) for more details.
 
         Arguments:
             `virtual_per_physical`
                 The number of virtual shards per physical shard.
             `desired_count`
                 The desired number of physical shards.
-            `actual_count`
-                The actual number of physical shards.
+            `actual_count` DEPRECATED
+                The actual number of physical shards. This is a read-only field so has no effect.
+                It is kept for backwards compatibility but will be removed in a future release.
             `desired_virtual_count`
                 The desired number of virtual shards.
-            `actual_virtual_count`
-                The actual number of virtual shards.
+            `actual_virtual_count` DEPRECATED
+                The actual number of virtual shards. This is a read-only field so has no effect.
+                It is kept for backwards compatibility but will be removed in a future release.
         """
+        if actual_count is not None:
+            _Warnings.sharding_actual_count_is_deprecated("actual_count")
+        if actual_virtual_count is not None:
+            _Warnings.sharding_actual_count_is_deprecated("actual_virtual_count")
         return _ShardingConfigCreate(
             virtualPerPhysical=virtual_per_physical,
             desiredCount=desired_count,
-            actualCount=actual_count,
             desiredVirtualCount=desired_virtual_count,
-            actualVirtualCount=actual_virtual_count,
         )
 
 
 class _VectorIndexQuantizerUpdate:
     @staticmethod
     def pq(
         bit_compression: Optional[bool] = None,
@@ -1657,17 +1795,19 @@
         """Create a `_PQConfigUpdate` object to be used when updating the product quantization (PQ) configuration of Weaviate.
 
         Use this method when defining the `quantizer` argument in the `vector_index` configuration in `collection.update()`.
 
         Arguments:
             See [the docs](https://weaviate.io/developers/weaviate/concepts/vector-index#hnsw-with-compression) for a more detailed view!
         """  # noqa: D417 (missing argument descriptions in the docstring)
+        if bit_compression is not None:
+            _Warnings.bit_compression_in_pq_config()
+
         return _PQConfigUpdate(
             enabled=enabled,
-            bitCompression=bit_compression,
             centroids=centroids,
             segments=segments,
             trainingLimit=training_limit,
             encoder=(
                 _PQEncoderConfigUpdate(type_=encoder_type, distribution=encoder_distribution)
                 if encoder_type is not None or encoder_distribution is not None
                 else None
@@ -1779,7 +1919,19 @@
         Use this method when defining the `replication_config` argument in `collection.update()`.
 
         Arguments:
             `factor`
                 The replication factor.
         """
         return _ReplicationConfigUpdate(factor=factor)
+
+    @staticmethod
+    def multi_tenancy(auto_tenant_creation: Optional[bool] = None) -> _MultiTenancyConfigUpdate:
+        """Create a `MultiTenancyConfigUpdate` object.
+
+        Use this method when defining the `multi_tenancy` argument in `collection.update()`.
+
+        Arguments:
+            `auto_tenant_creation`
+                When set, implicitly creates nonexisting tenants during batch imports
+        """
+        return _MultiTenancyConfigUpdate(autoTenantCreation=auto_tenant_creation)
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/config_base.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/config_base.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/config_methods.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/config_methods.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     _BQConfig,
     _CollectionConfig,
     _CollectionConfigSimple,
     _NamedVectorConfig,
     _NamedVectorizerConfig,
     _PQConfig,
     _VectorIndexConfigFlat,
+    _VectorIndexConfigDynamic,
     _InvertedIndexConfig,
     _BM25Config,
     _StopwordsConfig,
     _MultiTenancyConfig,
     _Property,
     _ReferenceProperty,
     _ReplicationConfig,
@@ -94,62 +95,84 @@
 def __get_vector_index_type(schema: Dict[str, Any]) -> Optional[VectorIndexType]:
     if "vectorIndexType" in schema:
         return VectorIndexType(schema["vectorIndexType"])
     else:
         return None
 
 
-def __get_vector_index_config(
-    schema: Dict[str, Any]
-) -> Union[_VectorIndexConfigHNSW, _VectorIndexConfigFlat, None]:
-    if "vectorIndexConfig" not in schema:
-        return None
+def __get_quantizer_config(config: Dict[str, Any]) -> Optional[Union[_PQConfig, _BQConfig]]:
     quantizer: Optional[Union[_PQConfig, _BQConfig]] = None
-    if "bq" in schema["vectorIndexConfig"] and schema["vectorIndexConfig"]["bq"]["enabled"]:
+    if "bq" in config and config["bq"]["enabled"]:
         # values are not present for bq+hnsw
         quantizer = _BQConfig(
-            cache=schema["vectorIndexConfig"]["bq"].get("cache"),
-            rescore_limit=schema["vectorIndexConfig"]["bq"].get("rescoreLimit"),
+            cache=config["bq"].get("cache"),
+            rescore_limit=config["bq"].get("rescoreLimit"),
         )
-    elif "pq" in schema["vectorIndexConfig"] and schema["vectorIndexConfig"]["pq"]["enabled"]:
+    elif "pq" in config and config["pq"].get("enabled"):
         quantizer = _PQConfig(
-            bit_compression=schema["vectorIndexConfig"]["pq"]["bitCompression"],
-            segments=schema["vectorIndexConfig"]["pq"]["segments"],
-            centroids=schema["vectorIndexConfig"]["pq"]["centroids"],
-            training_limit=schema["vectorIndexConfig"]["pq"]["trainingLimit"],
+            internal_bit_compression=config["pq"].get("bitCompression"),
+            segments=config["pq"].get("segments"),
+            centroids=config["pq"].get("centroids"),
+            training_limit=config["pq"].get("trainingLimit"),
             encoder=_PQEncoderConfig(
-                type_=PQEncoderType(schema["vectorIndexConfig"]["pq"]["encoder"]["type"]),
+                type_=PQEncoderType(config["pq"].get("encoder", {}).get("type")),
                 distribution=PQEncoderDistribution(
-                    schema["vectorIndexConfig"]["pq"]["encoder"]["distribution"]
+                    config["pq"].get("encoder", {}).get("distribution")
                 ),
             ),
         )
+    return quantizer
+
+
+def __get_hnsw_config(config: Dict[str, Any]) -> _VectorIndexConfigHNSW:
+    quantizer = __get_quantizer_config(config)
+    return _VectorIndexConfigHNSW(
+        cleanup_interval_seconds=config["cleanupIntervalSeconds"],
+        distance_metric=VectorDistances(config.get("distance")),
+        dynamic_ef_min=config["dynamicEfMin"],
+        dynamic_ef_max=config["dynamicEfMax"],
+        dynamic_ef_factor=config["dynamicEfFactor"],
+        ef=config["ef"],
+        ef_construction=config["efConstruction"],
+        flat_search_cutoff=config["flatSearchCutoff"],
+        max_connections=config["maxConnections"],
+        quantizer=quantizer,
+        skip=config["skip"],
+        vector_cache_max_objects=config["vectorCacheMaxObjects"],
+    )
+
+
+def __get_flat_config(config: Dict[str, Any]) -> _VectorIndexConfigFlat:
+    quantizer = __get_quantizer_config(config)
+    return _VectorIndexConfigFlat(
+        distance_metric=VectorDistances(config["distance"]),
+        quantizer=quantizer,
+        vector_cache_max_objects=config["vectorCacheMaxObjects"],
+    )
 
+
+def __get_vector_index_config(
+    schema: Dict[str, Any]
+) -> Union[_VectorIndexConfigHNSW, _VectorIndexConfigFlat, _VectorIndexConfigDynamic, None]:
+    if "vectorIndexConfig" not in schema:
+        return None
     if schema["vectorIndexType"] == "hnsw":
-        return _VectorIndexConfigHNSW(
-            cleanup_interval_seconds=schema["vectorIndexConfig"]["cleanupIntervalSeconds"],
+        return __get_hnsw_config(schema["vectorIndexConfig"])
+    elif schema["vectorIndexType"] == "flat":
+        return __get_flat_config(schema["vectorIndexConfig"])
+    elif schema["vectorIndexType"] == "dynamic":
+        return _VectorIndexConfigDynamic(
             distance_metric=VectorDistances(schema["vectorIndexConfig"]["distance"]),
-            dynamic_ef_min=schema["vectorIndexConfig"]["dynamicEfMin"],
-            dynamic_ef_max=schema["vectorIndexConfig"]["dynamicEfMax"],
-            dynamic_ef_factor=schema["vectorIndexConfig"]["dynamicEfFactor"],
-            ef=schema["vectorIndexConfig"]["ef"],
-            ef_construction=schema["vectorIndexConfig"]["efConstruction"],
-            flat_search_cutoff=schema["vectorIndexConfig"]["flatSearchCutoff"],
-            max_connections=schema["vectorIndexConfig"]["maxConnections"],
-            quantizer=quantizer,
-            skip=schema["vectorIndexConfig"]["skip"],
-            vector_cache_max_objects=schema["vectorIndexConfig"]["vectorCacheMaxObjects"],
+            threshold=schema["vectorIndexConfig"].get("threshold"),
+            quantizer=None,
+            hnsw=__get_hnsw_config(schema["vectorIndexConfig"]["hnsw"]),
+            flat=__get_flat_config(schema["vectorIndexConfig"]["flat"]),
         )
     else:
-        assert schema["vectorIndexType"] == "flat"
-        return _VectorIndexConfigFlat(
-            distance_metric=VectorDistances(schema["vectorIndexConfig"]["distance"]),
-            quantizer=quantizer,
-            vector_cache_max_objects=schema["vectorIndexConfig"]["vectorCacheMaxObjects"],
-        )
+        return None
 
 
 def __get_vector_config(
     schema: Dict[str, Any], simple: bool
 ) -> Optional[Dict[str, _NamedVectorConfig]]:
     if "vectorConfig" in schema:
         named_vectors: Dict[str, _NamedVectorConfig] = {}
@@ -215,31 +238,36 @@
             stopwords=_StopwordsConfig(
                 preset=StopwordsPreset(schema["invertedIndexConfig"]["stopwords"]["preset"]),
                 additions=schema["invertedIndexConfig"]["stopwords"]["additions"],
                 removals=schema["invertedIndexConfig"]["stopwords"]["removals"],
             ),
         ),
         multi_tenancy_config=_MultiTenancyConfig(
-            enabled=schema.get("multiTenancyConfig", {}).get("enabled", False)
+            enabled=schema.get("multiTenancyConfig", {}).get("enabled", False),
+            auto_tenant_creation=schema.get("multiTenancyConfig", {}).get(
+                "autoTenantCreation", False
+            ),
         ),
         properties=_properties_from_config(schema) if schema.get("properties") is not None else [],
         references=_references_from_config(schema) if schema.get("properties") is not None else [],
         replication_config=_ReplicationConfig(factor=schema["replicationConfig"]["factor"]),
         reranker_config=__get_rerank_config(schema),
-        sharding_config=None
-        if schema.get("multiTenancyConfig", {}).get("enabled", False)
-        else _ShardingConfig(
-            virtual_per_physical=schema["shardingConfig"]["virtualPerPhysical"],
-            desired_count=schema["shardingConfig"]["desiredCount"],
-            actual_count=schema["shardingConfig"]["actualCount"],
-            desired_virtual_count=schema["shardingConfig"]["desiredVirtualCount"],
-            actual_virtual_count=schema["shardingConfig"]["actualVirtualCount"],
-            key=schema["shardingConfig"]["key"],
-            strategy=schema["shardingConfig"]["strategy"],
-            function=schema["shardingConfig"]["function"],
+        sharding_config=(
+            None
+            if schema.get("multiTenancyConfig", {}).get("enabled", False)
+            else _ShardingConfig(
+                virtual_per_physical=schema["shardingConfig"]["virtualPerPhysical"],
+                desired_count=schema["shardingConfig"]["desiredCount"],
+                actual_count=schema["shardingConfig"]["actualCount"],
+                desired_virtual_count=schema["shardingConfig"]["desiredVirtualCount"],
+                actual_virtual_count=schema["shardingConfig"]["actualVirtualCount"],
+                key=schema["shardingConfig"]["key"],
+                strategy=schema["shardingConfig"]["strategy"],
+                function=schema["shardingConfig"]["function"],
+            )
         ),
         vector_index_config=__get_vector_index_config(schema),
         vector_index_type=__get_vector_index_type(schema),
         vectorizer_config=__get_vectorizer_config(schema),
         vectorizer=__get_vectorizer(schema),
         vector_config=__get_vector_config(schema, simple=False),
     )
@@ -298,14 +326,15 @@
                 _PropertyVectorizerConfig(
                     skip=prop["moduleConfig"][schema["vectorizer"]].get("skip", False),
                     vectorize_property_name=prop["moduleConfig"][schema["vectorizer"]].get(
                         "vectorizePropertyName", False
                     ),
                 )
                 if schema.get("vectorizer", "none") != "none"
+                and prop.get("moduleConfig", None) is not None
                 else None
             ),
             vectorizer=schema.get("vectorizer", "none"),
         )
         for prop in schema["properties"]
         if _is_primitive(prop["dataType"])
     ]
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/config_named_vectors.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/config_named_vectors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from typing import Any, Dict, List, Literal, Optional, Union
+
 from pydantic import AnyHttpUrl, Field
+
 from weaviate.collections.classes.config_base import (
     _ConfigCreateModel,
     _ConfigUpdateModel,
 )
+from weaviate.collections.classes.config_vector_index import (
+    _VectorIndexConfigCreate,
+    _VectorIndexConfigHNSWUpdate,
+    _VectorIndexConfigFlatUpdate,
+    _VectorIndexConfigDynamicUpdate,
+    _VectorIndexConfigUpdate,
+    VectorIndexType,
+)
 from weaviate.collections.classes.config_vectorizers import (
     _Img2VecNeuralConfigCreate,
     _Multi2VecBindConfigCreate,
     _Multi2VecClipConfigCreate,
+    _Multi2VecPalmConfig,
     _Ref2VecCentroidConfigCreate,
     _Text2VecAWSConfigCreate,
     _Text2VecAzureOpenAIConfigCreate,
     _Text2VecCohereConfigCreate,
     _Text2VecContextionaryConfigCreate,
     _Text2VecGPT4AllConfigCreate,
     _Text2VecHuggingFaceConfigCreate,
     _Text2VecJinaConfigCreate,
+    _Text2VecOctoConfig,
     _Text2VecOpenAIConfigCreate,
     _Text2VecPalmConfigCreate,
     _Text2VecTransformersConfigCreate,
+    _Text2VecVoyageConfigCreate,
     _VectorizerConfigCreate,
     AWSModel,
     AWSService,
     CohereModel,
     CohereTruncation,
     JinaModel,
     Multi2VecField,
     OpenAIModel,
     OpenAIType,
     Vectorizers,
+    VoyageModel,
     _map_multi2vec_fields,
 )
-from weaviate.collections.classes.config_vector_index import (
-    _VectorIndexConfigCreate,
-    _VectorIndexConfigHNSWUpdate,
-    _VectorIndexConfigFlatUpdate,
-    _VectorIndexConfigUpdate,
-    VectorIndexType,
-)
 
 
 class _NamedVectorizerConfigCreate(_ConfigCreateModel):
     vectorizer: Vectorizers
     properties: Optional[List[str]] = Field(default=None, min_length=1, alias="source_properties")
 
     def _to_dict(self) -> Dict[str, Any]:
@@ -179,14 +186,57 @@
             vectorizer=_Text2VecContextionaryConfigCreate(
                 vectorizeClassName=vectorize_collection_name,
             ),
             vector_index_config=vector_index_config,
         )
 
     @staticmethod
+    def text2vec_octoai(
+        name: str,
+        *,
+        source_properties: Optional[List[str]] = None,
+        vector_index_config: Optional[_VectorIndexConfigCreate] = None,
+        vectorize_collection_name: bool = True,
+        model: Optional[Union[OpenAIModel, str]] = None,
+        base_url: Optional[str] = None,
+    ) -> _NamedVectorConfigCreate:
+        """Create a named vector using the `text2vec_octoai` model.
+
+        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-octoai)
+        for detailed usage.
+
+        Arguments:
+            `name`
+                The name of the named vector.
+            `source_properties`
+                Which properties should be included when vectorizing. By default all text properties are included.
+            `vector_index_config`
+                The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+            `model`
+                The model to use. Defaults to `None`, which uses the server-defined default.
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+            `base_url`
+                The base URL to use where API requests should go. Defaults to `None`, which uses the server-defined default.
+
+        """
+        return _NamedVectorConfigCreate(
+            name=name,
+            source_properties=source_properties,
+            vectorizer=_Text2VecOctoConfig(
+                baseURL=base_url,
+                model=model,
+                vectorizeClassName=vectorize_collection_name,
+            ),
+            vector_index_config=vector_index_config,
+        )
+
+    @staticmethod
     def text2vec_openai(
         name: str,
         *,
         source_properties: Optional[List[str]] = None,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
         model: Optional[Union[OpenAIModel, str]] = None,
@@ -313,39 +363,105 @@
             vector_index_config=vector_index_config,
         )
 
     @staticmethod
     def multi2vec_clip(
         name: str,
         *,
+        vector_index_config: Optional[_VectorIndexConfigCreate] = None,
+        vectorize_collection_name: bool = True,
         image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
         text_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
+        interference_url: Optional[str] = None,
+    ) -> _NamedVectorConfigCreate:
+        """Create a named vector using the `multi2vec_clip` model.
+
+        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-gpt4all)
+        for detailed usage.
+
+        Arguments:
+            `name`
+                The name of the named vector.
+            `vector_index_config`
+                The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+            `image_fields`
+                The image fields to use in vectorization.
+            `text_fields`
+                The text fields to use in vectorization.
+            `inference_url`
+                The inference url to use where API requests should go. Defaults to `None`, which uses the server-defined default.
+        """
+        return _NamedVectorConfigCreate(
+            name=name,
+            vectorizer=_Multi2VecClipConfigCreate(
+                imageFields=_map_multi2vec_fields(image_fields),
+                textFields=_map_multi2vec_fields(text_fields),
+                vectorizeClassName=vectorize_collection_name,
+                inferenceUrl=interference_url,
+            ),
+            vector_index_config=vector_index_config,
+        )
+
+    @staticmethod
+    def multi2vec_palm(
+        name: str,
+        *,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
+        location: str,
+        project_id: str,
+        image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
+        text_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
+        video_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
+        dimensions: Optional[int] = None,
+        video_interval_seconds: Optional[int] = None,
+        model_id: Optional[str] = None,
     ) -> _NamedVectorConfigCreate:
         """Create a named vector using the `multi2vec_clip` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-gpt4all)
         for detailed usage.
 
         Arguments:
             `name`
                 The name of the named vector.
-            `source_properties`
-                Which properties should be included when vectorizing. By default all text properties are included.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
+            `location`
+                Where the model runs. REQUIRED.
+            `project_id`
+                The project ID to use, REQUIRED.
+            `image_fields`
+                The image fields to use in vectorization.
+            `text_fields`
+                The text fields to use in vectorization.
+            `video_fields`
+                The video fields to use in vectorization.
+            `dimensions`
+                The number of dimensions to use. Defaults to `None`, which uses the server-defined default.
+            `video_interval_seconds`
+                Length of a video interval. Defaults to `None`, which uses the server-defined default.
+            `model_id`
+                The model ID to use. Defaults to `None`, which uses the server-defined default.
         """
         return _NamedVectorConfigCreate(
             name=name,
-            vectorizer=_Multi2VecClipConfigCreate(
+            vectorizer=_Multi2VecPalmConfig(
+                projectId=project_id,
+                location=location,
                 imageFields=_map_multi2vec_fields(image_fields),
                 textFields=_map_multi2vec_fields(text_fields),
+                videoFields=_map_multi2vec_fields(video_fields),
+                dimensions=dimensions,
+                modelId=model_id,
+                videoIntervalSeconds=video_interval_seconds,
                 vectorizeClassName=vectorize_collection_name,
             ),
             vector_index_config=vector_index_config,
         )
 
     @staticmethod
     def multi2vec_bind(
@@ -365,16 +481,14 @@
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-gpt4all)
         for detailed usage.
 
         Arguments:
             `name`
                 The name of the named vector.
-            `source_properties`
-                Which properties should be included when vectorizing. By default all text properties are included.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
         """
         return _NamedVectorConfigCreate(
             name=name,
@@ -403,16 +517,16 @@
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-gpt4all)
         for detailed usage.
 
         Arguments:
             `name`
                 The name of the named vector.
-            `source_properties`
-                Which properties should be included when vectorizing. By default all text properties are included.
+            `reference_properties`
+                The reference properties to use in vectorization, REQUIRED.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
         """
         return _NamedVectorConfigCreate(
             name=name,
@@ -562,15 +676,15 @@
     def text2vec_palm(
         name: str,
         project_id: str,
         *,
         source_properties: Optional[List[str]] = None,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
-        api_endpoint: Optional[AnyHttpUrl] = None,
+        api_endpoint: Optional[str] = None,
         model_id: Optional[str] = None,
     ) -> _NamedVectorConfigCreate:
         """Create a named vector using the `text2vec_palm` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-palm)
         for detailed usage.
 
@@ -584,15 +698,15 @@
             `source_properties`
                 Which properties should be included when vectorizing. By default all text properties are included.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
             `api_endpoint`
-                The API endpoint to use. Defaults to `None`, which uses the server-defined default.
+                The API endpoint to use without a leading scheme such as `http://`. Defaults to `None`, which uses the server-defined default
             `model_id`
                 The model ID to use. Defaults to `None`, which uses the server-defined default.
 
         Raises:
             `pydantic.ValidationError` if `api_endpoint` is not a valid URL.
         """
         return _NamedVectorConfigCreate(
@@ -611,14 +725,17 @@
     def text2vec_transformers(
         name: str,
         *,
         source_properties: Optional[List[str]] = None,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
         pooling_strategy: Literal["masked_mean", "cls"] = "masked_mean",
+        inference_url: Optional[str] = None,
+        passage_inference_url: Optional[str] = None,
+        query_inference_url: Optional[str] = None,
     ) -> _NamedVectorConfigCreate:
         """Create a named vector using the `text2vec_transformers` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-transformers)
         for detailed usage.
 
         Arguments:
@@ -628,21 +745,30 @@
                 Which properties should be included when vectorizing. By default all text properties are included.
             `vector_index_config`
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
             `pooling_strategy`
                 The pooling strategy to use. Defaults to `masked_mean`.
+            `inference_url`
+                The inferenceUrl to use where API requests should go. You can use either this OR passage/query_inference_url. Defaults to `None`, which uses the server-defined default.
+            `passage_inference_url`
+                The inferenceUrl to use where passage API requests should go. You can use either this and query_inference_url OR inference_url. Defaults to `None`, which uses the server-defined default.
+            `query_inference_url`
+                The inferenceUrl to use where query API requests should go. You can use either this and passage_inference_url OR inference_url. Defaults to `None`, which uses the server-defined default.
         """
         return _NamedVectorConfigCreate(
             name=name,
             source_properties=source_properties,
             vectorizer=_Text2VecTransformersConfigCreate(
                 poolingStrategy=pooling_strategy,
                 vectorizeClassName=vectorize_collection_name,
+                inferenceUrl=inference_url,
+                passageInferenceUrl=passage_inference_url,
+                queryInferenceUrl=query_inference_url,
             ),
             vector_index_config=vector_index_config,
         )
 
     @staticmethod
     def text2vec_jinaai(
         name: str,
@@ -677,21 +803,71 @@
             vectorizer=_Text2VecJinaConfigCreate(
                 model=model,
                 vectorizeClassName=vectorize_collection_name,
             ),
             vector_index_config=vector_index_config,
         )
 
+    @staticmethod
+    def text2vec_voyageai(
+        name: str,
+        *,
+        source_properties: Optional[List[str]] = None,
+        vector_index_config: Optional[_VectorIndexConfigCreate] = None,
+        vectorize_collection_name: bool = True,
+        model: Optional[Union[VoyageModel, str]] = None,
+        base_url: Optional[str] = None,
+        truncate: Optional[bool] = None,
+    ) -> _NamedVectorConfigCreate:
+        """Create a named vector using the `text2vec-jinaai` model.
+
+        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-jinaai)
+        for detailed usage.
+
+        Arguments:
+            `name`
+                The name of the named vector.
+            `source_properties`
+                Which properties should be included when vectorizing. By default all text properties are included.
+            `vector_index_config`
+                The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+            `model`
+                The model to use. Defaults to `None`, which uses the server-defined default.
+                See the
+                [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-voyageai#available-models) for more details.
+            `base_url`
+                The base URL to use where API requests should go. Defaults to `None`, which uses the server-defined default.
+            `truncate`
+                Whether to truncate the input texts to fit within the context length. Defaults to `None`, which uses the server-defined default.
+        """
+        return _NamedVectorConfigCreate(
+            name=name,
+            source_properties=source_properties,
+            vectorizer=_Text2VecVoyageConfigCreate(
+                model=model,
+                vectorizeClassName=vectorize_collection_name,
+                baseURL=base_url,
+                truncate=truncate,
+            ),
+            vector_index_config=vector_index_config,
+        )
+
 
 class _NamedVectorsUpdate:
     @staticmethod
     def update(
         name: str,
         *,
-        vector_index_config: Union[_VectorIndexConfigHNSWUpdate, _VectorIndexConfigFlatUpdate],
+        vector_index_config: Union[
+            _VectorIndexConfigHNSWUpdate,
+            _VectorIndexConfigFlatUpdate,
+            _VectorIndexConfigDynamicUpdate,
+        ],
     ) -> _NamedVectorConfigUpdate:
         """Update the vector index configuration of a named vector.
 
         This is the only update operation allowed currently. If you wish to change the vectorization configuration itself, you will have to
         recreate the collection with the new configuration.
 
         Arguments:
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/config_vector_index.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/config_vector_index.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Attributes:
         HNSW: Hierarchical Navigable Small World (HNSW) index.
         FLAT: Flat index.
     """
 
     HNSW = "hnsw"
     FLAT = "flat"
+    DYNAMIC = "dynamic"
 
 
 class _VectorIndexConfigCreate(_ConfigCreateModel):
     distance: Optional[VectorDistances]
     vectorCacheMaxObjects: Optional[int]
     quantizer: Optional[_QuantizerConfigCreate] = Field(exclude=True)
 
@@ -97,7 +98,23 @@
         return VectorIndexType.HNSW
 
 
 class _VectorIndexConfigFlatUpdate(_VectorIndexConfigUpdate):
     @staticmethod
     def vector_index_type() -> VectorIndexType:
         return VectorIndexType.FLAT
+
+
+class _VectorIndexConfigDynamicCreate(_VectorIndexConfigCreate):
+    threshold: Optional[int]
+    hnsw: Optional[_VectorIndexConfigHNSWCreate]
+    flat: Optional[_VectorIndexConfigFlatCreate]
+
+    @staticmethod
+    def vector_index_type() -> VectorIndexType:
+        return VectorIndexType.DYNAMIC
+
+
+class _VectorIndexConfigDynamicUpdate(_VectorIndexConfigUpdate):
+    @staticmethod
+    def vector_index_type() -> VectorIndexType:
+        return VectorIndexType.DYNAMIC
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/config_vectorizers.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/config_vectorizers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from enum import Enum
 from typing import Any, Dict, List, Literal, Optional, Union, cast
-from typing_extensions import TypeAlias
 
 from pydantic import AnyHttpUrl, BaseModel, Field, field_validator
+from typing_extensions import TypeAlias
 
 from weaviate.collections.classes.config_base import _ConfigCreateModel
 
-
 CohereModel: TypeAlias = Literal[
     "embed-multilingual-v2.0",
     "embed-multilingual-v3.0",
     "embed-multilingual-light-v3.0",
     "small",
     "medium",
     "large",
@@ -21,14 +20,15 @@
     "embed-english-light-v3.0",
 ]
 CohereTruncation: TypeAlias = Literal["NONE", "START", "END", "LEFT", "RIGHT"]
 OpenAIModel: TypeAlias = Literal[
     "text-embedding-3-small", "text-embedding-3-large", "text-embedding-ada-002"
 ]
 JinaModel: TypeAlias = Literal["jina-embeddings-v2-base-en", "jina-embeddings-v2-small-en"]
+VoyageModel: TypeAlias = Literal["voyage-large-2, voyage-code-2, voyage-2"]
 AWSModel: TypeAlias = Literal[
     "amazon.titan-embed-text-v1",
     "cohere.embed-english-v3",
     "cohere.embed-multilingual-v3",
 ]
 AWSService: TypeAlias = Literal[
     "bedrock",
@@ -59,37 +59,44 @@
             Weaviate module backed by OpenAI and Azure-OpenAI text-based embedding models.
         `TEXT2VEC_PALM`
             Weaviate module backed by PaLM text-based embedding models.
         `TEXT2VEC_TRANSFORMERS`
             Weaviate module backed by Transformers text-based embedding models.
         `TEXT2VEC_JINAAI`
             Weaviate module backed by Jina AI text-based embedding models.
+        `TEXT2VEC_VOYAGEAI`
+            Weaviate module backed by Voyage AI text-based embedding models.
         `IMG2VEC_NEURAL`
             Weaviate module backed by a ResNet-50 neural network for images.
         `MULTI2VEC_CLIP`
             Weaviate module backed by a Sentence-BERT CLIP model for images and text.
+        `MULTI2VEC_PALM`
+            Weaviate module backed by a palm model for images and text.
         `MULTI2VEC_BIND`
             Weaviate module backed by the ImageBind model for images, text, audio, depth, IMU, thermal, and video.
         `REF2VEC_CENTROID`
             Weaviate module backed by a centroid-based model that calculates an object's vectors from its referenced vectors.
     """
 
     NONE = "none"
     TEXT2VEC_AWS = "text2vec-aws"
     TEXT2VEC_COHERE = "text2vec-cohere"
     TEXT2VEC_CONTEXTIONARY = "text2vec-contextionary"
     TEXT2VEC_GPT4ALL = "text2vec-gpt4all"
     TEXT2VEC_HUGGINGFACE = "text2vec-huggingface"
+    TEXT2VEC_OCTOAI = "text2vec-octoai"
     TEXT2VEC_OPENAI = "text2vec-openai"
     TEXT2VEC_PALM = "text2vec-palm"
     TEXT2VEC_TRANSFORMERS = "text2vec-transformers"
     TEXT2VEC_JINAAI = "text2vec-jinaai"
+    TEXT2VEC_VOYAGEAI = "text2vec-voyageai"
     IMG2VEC_NEURAL = "img2vec-neural"
     MULTI2VEC_CLIP = "multi2vec-clip"
     MULTI2VEC_BIND = "multi2vec-bind"
+    MULTI2VEC_PALM = "multi2vec-palm"
     REF2VEC_CENTROID = "ref2vec-centroid"
 
 
 class VectorDistances(str, Enum):
     """Vector similarity distance metric to be used in the `VectorIndexConfig` class.
 
     To ensure optimal search results, we recommend reviewing whether your model provider advises a
@@ -242,35 +249,32 @@
 class _Text2VecCohereConfigCreate(_Text2VecCohereConfig, _VectorizerConfigCreate):
     pass
 
 
 class _Text2VecPalmConfig(_ConfigCreateModel):
     vectorizer: Vectorizers = Field(default=Vectorizers.TEXT2VEC_PALM, frozen=True, exclude=True)
     projectId: str
-    apiEndpoint: Optional[AnyHttpUrl]
+    apiEndpoint: Optional[str]
     modelId: Optional[str]
     vectorizeClassName: bool
 
-    def _to_dict(self) -> Dict[str, Any]:
-        ret_dict = super()._to_dict()
-        if self.apiEndpoint is not None:
-            ret_dict["apiEndpoint"] = self.apiEndpoint.unicode_string()
-        return ret_dict
-
 
 class _Text2VecPalmConfigCreate(_Text2VecPalmConfig, _VectorizerConfigCreate):
     pass
 
 
 class _Text2VecTransformersConfig(_ConfigCreateModel):
     vectorizer: Vectorizers = Field(
         default=Vectorizers.TEXT2VEC_TRANSFORMERS, frozen=True, exclude=True
     )
     poolingStrategy: Literal["masked_mean", "cls"]
     vectorizeClassName: bool
+    inferenceUrl: Optional[str]
+    passageInferenceUrl: Optional[str]
+    queryInferenceUrl: Optional[str]
 
 
 class _Text2VecTransformersConfigCreate(_Text2VecTransformersConfig, _VectorizerConfigCreate):
     pass
 
 
 class _Text2VecGPT4AllConfig(_ConfigCreateModel):
@@ -288,14 +292,35 @@
     vectorizeClassName: bool
 
 
 class _Text2VecJinaConfigCreate(_Text2VecJinaConfig, _VectorizerConfigCreate):
     pass
 
 
+class _Text2VecVoyageConfig(_ConfigCreateModel):
+    vectorizer: Vectorizers = Field(
+        default=Vectorizers.TEXT2VEC_VOYAGEAI, frozen=True, exclude=True
+    )
+    model: Optional[str]
+    baseURL: Optional[str]
+    truncate: Optional[bool]
+    vectorizeClassName: bool
+
+
+class _Text2VecVoyageConfigCreate(_Text2VecVoyageConfig, _VectorizerConfigCreate):
+    pass
+
+
+class _Text2VecOctoConfig(_VectorizerConfigCreate):
+    vectorizer: Vectorizers = Field(default=Vectorizers.TEXT2VEC_OCTOAI, frozen=True, exclude=True)
+    model: Optional[str]
+    baseURL: Optional[str]
+    vectorizeClassName: bool
+
+
 class _Img2VecNeuralConfig(_ConfigCreateModel):
     vectorizer: Vectorizers = Field(default=Vectorizers.IMG2VEC_NEURAL, frozen=True, exclude=True)
     imageFields: List[str]
 
 
 class _Img2VecNeuralConfigCreate(_Img2VecNeuralConfig, _VectorizerConfigCreate):
     pass
@@ -327,20 +352,32 @@
         if len(ret_dict["weights"]) == 0:
             del ret_dict["weights"]
         return ret_dict
 
 
 class _Multi2VecClipConfig(_Multi2VecBase):
     vectorizer: Vectorizers = Field(default=Vectorizers.MULTI2VEC_CLIP, frozen=True, exclude=True)
+    inferenceUrl: Optional[str]
 
 
 class _Multi2VecClipConfigCreate(_Multi2VecClipConfig, _VectorizerConfigCreate):
     pass
 
 
+class _Multi2VecPalmConfig(_Multi2VecBase, _VectorizerConfigCreate):
+    vectorizer: Vectorizers = Field(default=Vectorizers.MULTI2VEC_PALM, frozen=True, exclude=True)
+    videoFields: Optional[List[Multi2VecField]]
+    projectId: str
+    location: Optional[str]
+    modelId: Optional[str]
+    dimensions: Optional[int]
+    videoIntervalSeconds: Optional[int]
+    vectorizeClassName: bool
+
+
 class _Multi2VecBindConfig(_Multi2VecBase):
     vectorizer: Vectorizers = Field(default=Vectorizers.MULTI2VEC_BIND, frozen=True, exclude=True)
     audioFields: Optional[List[Multi2VecField]]
     depthFields: Optional[List[Multi2VecField]]
     IMUFields: Optional[List[Multi2VecField]]
     thermalFields: Optional[List[Multi2VecField]]
     videoFields: Optional[List[Multi2VecField]]
@@ -399,36 +436,40 @@
         """
         return _Img2VecNeuralConfigCreate(imageFields=image_fields)
 
     @staticmethod
     def multi2vec_clip(
         image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
         text_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
+        interference_url: Optional[str] = None,
         vectorize_collection_name: bool = True,
     ) -> _VectorizerConfigCreate:
         """Create a `_Multi2VecClipConfigCreate` object for use when vectorizing using the `multi2vec-clip` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/multi2vec-clip)
         for detailed usage.
 
         Arguments:
             `image_fields`
                 The image fields to use in vectorization.
             `text_fields`
                 The text fields to use in vectorization.
+            `inference_url`
+                The inference url to use where API requests should go. Defaults to `None`, which uses the server-defined default.
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
 
         Raises:
             `pydantic.ValidationError` if `image_fields` or `text_fields` are not `None` or a `list`.
         """
         return _Multi2VecClipConfigCreate(
             imageFields=_map_multi2vec_fields(image_fields),
             textFields=_map_multi2vec_fields(text_fields),
             vectorizeClassName=vectorize_collection_name,
+            inferenceUrl=interference_url,
         )
 
     @staticmethod
     def multi2vec_bind(
         audio_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
         depth_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
         image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
@@ -677,14 +718,40 @@
             waitForModel=wait_for_model,
             useGPU=use_gpu,
             useCache=use_cache,
             vectorizeClassName=vectorize_collection_name,
         )
 
     @staticmethod
+    def text2vec_octoai(
+        *,
+        base_url: Optional[str] = None,
+        model: Optional[Union[OpenAIModel, str]] = None,
+        vectorize_collection_name: bool = True,
+    ) -> _VectorizerConfigCreate:
+        """Create a `_Text2VecOctoConfig` object for use when vectorizing using the `text2vec-openai` model.
+
+        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-octoai)
+        for detailed usage.
+
+        Arguments:
+            `base_url`
+                The base URL to use where API requests should go. Defaults to `None`, which uses the server-defined default.
+            `model`
+                The model to use. Defaults to `None`, which uses the server-defined default.
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+        """
+        return _Text2VecOctoConfig(
+            baseURL=base_url,
+            model=model,
+            vectorizeClassName=vectorize_collection_name,
+        )
+
+    @staticmethod
     def text2vec_openai(
         model: Optional[Union[OpenAIModel, str]] = None,
         model_version: Optional[str] = None,
         type_: Optional[OpenAIType] = None,
         vectorize_collection_name: bool = True,
         base_url: Optional[AnyHttpUrl] = None,
         dimensions: Optional[int] = None,
@@ -719,28 +786,28 @@
             vectorizeClassName=vectorize_collection_name,
             dimensions=dimensions,
         )
 
     @staticmethod
     def text2vec_palm(
         project_id: str,
-        api_endpoint: Optional[AnyHttpUrl] = None,
+        api_endpoint: Optional[str] = None,
         model_id: Optional[str] = None,
         vectorize_collection_name: bool = True,
     ) -> _VectorizerConfigCreate:
         """Create a `_Text2VecPalmConfigCreate` object for use when vectorizing using the `text2vec-palm` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-palm)
         for detailed usage.
 
         Arguments:
             `project_id`
                 The project ID to use, REQUIRED.
             `api_endpoint`
-                The API endpoint to use. Defaults to `None`, which uses the server-defined default.
+                The API endpoint to use without a leading scheme such as `http://`. Defaults to `None`, which uses the server-defined default
             `model_id`
                 The model ID to use. Defaults to `None`, which uses the server-defined default.
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
 
         Raises:
             `pydantic.ValidationError` if `api_endpoint` is not a valid URL.
@@ -749,35 +816,100 @@
             projectId=project_id,
             apiEndpoint=api_endpoint,
             modelId=model_id,
             vectorizeClassName=vectorize_collection_name,
         )
 
     @staticmethod
+    def multi2vec_palm(
+        *,
+        location: str,
+        project_id: str,
+        image_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
+        text_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
+        video_fields: Optional[Union[List[str], List[Multi2VecField]]] = None,
+        dimensions: Optional[int] = None,
+        model_id: Optional[str] = None,
+        video_interval_seconds: Optional[int] = None,
+        vectorize_collection_name: bool = True,
+    ) -> _VectorizerConfigCreate:
+        """Create a `_Multi2VecPalmConfig` object for use when vectorizing using the `text2vec-palm` model.
+
+        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-palm)
+        for detailed usage.
+
+        Arguments:
+            `location`
+                Where the model runs. REQUIRED.
+            `project_id`
+                The project ID to use, REQUIRED.
+            `image_fields`
+                The image fields to use in vectorization.
+            `text_fields`
+                The text fields to use in vectorization.
+            `video_fields`
+                The video fields to use in vectorization.
+            `dimensions`
+                The number of dimensions to use. Defaults to `None`, which uses the server-defined default.
+            `model_id`
+                The model ID to use. Defaults to `None`, which uses the server-defined default.
+            `video_interval_seconds`
+                Length of a video interval. Defaults to `None`, which uses the server-defined default.
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+
+        Raises:
+            `pydantic.ValidationError` if `api_endpoint` is not a valid URL.
+        """
+        return _Multi2VecPalmConfig(
+            projectId=project_id,
+            location=location,
+            imageFields=_map_multi2vec_fields(image_fields),
+            textFields=_map_multi2vec_fields(text_fields),
+            videoFields=_map_multi2vec_fields(video_fields),
+            dimensions=dimensions,
+            modelId=model_id,
+            videoIntervalSeconds=video_interval_seconds,
+            vectorizeClassName=vectorize_collection_name,
+        )
+
+    @staticmethod
     def text2vec_transformers(
         pooling_strategy: Literal["masked_mean", "cls"] = "masked_mean",
         vectorize_collection_name: bool = True,
+        inference_url: Optional[str] = None,
+        passage_inference_url: Optional[str] = None,
+        query_inference_url: Optional[str] = None,
     ) -> _VectorizerConfigCreate:
         """Create a `_Text2VecTransformersConfigCreate` object for use when vectorizing using the `text2vec-transformers` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-transformers)
         for detailed usage.
 
         Arguments:
             `pooling_strategy`
                 The pooling strategy to use. Defaults to `masked_mean`.
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
+            `inference_url`
+                The inference url to use where API requests should go. You can use either this OR passage/query_inference_url. Defaults to `None`, which uses the server-defined default.
+            `passage_inference_url`
+                The inference url to use where passage API requests should go. You can use either this and query_inference_url OR inference_url. Defaults to `None`, which uses the server-defined default.
+            `query_inference_url`
+                The inference url to use where query API requests should go. You can use either this and passage_inference_url OR inference_url. Defaults to `None`, which uses the server-defined default.
 
         Raises:
             `pydantic.ValidationError` if `pooling_strategy` is not a valid value from the `PoolingStrategy` type.
         """
         return _Text2VecTransformersConfigCreate(
             poolingStrategy=pooling_strategy,
             vectorizeClassName=vectorize_collection_name,
+            inferenceUrl=inference_url,
+            passageInferenceUrl=passage_inference_url,
+            queryInferenceUrl=query_inference_url,
         )
 
     @staticmethod
     def text2vec_jinaai(
         model: Optional[Union[JinaModel, str]] = None,
         vectorize_collection_name: bool = True,
     ) -> _VectorizerConfigCreate:
@@ -791,7 +923,39 @@
                 The model to use. Defaults to `None`, which uses the server-defined default.
                 See the
                 [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-jinaai#available-models) for more details.
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
         """
         return _Text2VecJinaConfigCreate(model=model, vectorizeClassName=vectorize_collection_name)
+
+    @staticmethod
+    def text2vec_voyageai(
+        *,
+        model: Optional[Union[VoyageModel, str]] = None,
+        base_url: Optional[str] = None,
+        truncate: Optional[bool] = None,
+        vectorize_collection_name: bool = True,
+    ) -> _VectorizerConfigCreate:
+        """Create a `_Text2VecVoyageConfigCreate` object for use when vectorizing using the `text2vec-voyageai` model.
+
+        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-voyageai)
+        for detailed usage.
+
+        Arguments:
+            `model`
+                The model to use. Defaults to `None`, which uses the server-defined default.
+                See the
+                [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-voyageai#available-models) for more details.
+            `base_url`
+                The base URL to use where API requests should go. Defaults to `None`, which uses the server-defined default.
+            `truncate`
+                Whether to truncate the input texts to fit within the context length. Defaults to `None`, which uses the server-defined default.
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+        """
+        return _Text2VecVoyageConfigCreate(
+            model=model,
+            baseURL=base_url,
+            truncate=truncate,
+            vectorizeClassName=vectorize_collection_name,
+        )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/data.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/data.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/filters.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 
 from weaviate.collections.classes.types import _WeaviateInput
 from weaviate.types import UUID
 from weaviate.proto.v1 import base_pb2
 from weaviate.util import get_valid_uuid
 
+from weaviate.exceptions import WeaviateInvalidInputError
+
 
 class _Operator(str, Enum):
     EQUAL = "Equal"
     NOT_EQUAL = "NotEqual"
     LESS_THAN = "LessThan"
     LESS_THAN_EQUAL = "LessThanEqual"
     GREATER_THAN = "GreaterThan"
@@ -56,35 +58,35 @@
             return base_pb2.Filters.OPERATOR_AND
         else:
             assert self == _Operator.OR
             return base_pb2.Filters.OPERATOR_OR
 
 
 class _Filters:
-    def __and__(self, other: "_Filters") -> "_FilterAnd":
-        return _FilterAnd(self, other)
+    def __and__(self, other: "_Filters") -> "_Filters":
+        return _FilterAnd([self, other])
 
-    def __or__(self, other: "_Filters") -> "_FilterOr":
-        return _FilterOr(self, other)
+    def __or__(self, other: "_Filters") -> "_Filters":
+        return _FilterOr([self, other])
 
 
 class _FilterAnd(_Filters):
-    def __init__(self, *args: _Filters):
-        self.filters: List[_Filters] = list(args)
+    def __init__(self, filters: List[_Filters]):
+        self.filters: List[_Filters] = filters
 
     # replace with the following once 3.11 is the minimum version
     #     Operator: weaviate_pb2.Filters.OperatorType = weaviate_pb2.Filters.OperatorAnd
     @property
     def operator(self) -> _Operator:
         return _Operator.AND
 
 
 class _FilterOr(_Filters):
-    def __init__(self, *args: _Filters):
-        self.filters: List[_Filters] = list(args)
+    def __init__(self, filters: List[_Filters]):
+        self.filters: List[_Filters] = filters
 
     # replace with the following once 3.11 is the minimum version
     #     Operator: weaviate_pb2.Filters.OperatorType = weaviate_pb2.Filters.OperatorOr
     @property
     def operator(self) -> _Operator:
         return _Operator.OR
 
@@ -150,187 +152,192 @@
     def __init__(self, prop: str, length: bool, target: Optional[_TargetRefs] = None) -> None:
         self._target = target
         if length:
             prop = "len(" + prop + ")"
 
         self._property = prop
 
-    def is_none(self, val: bool) -> _FilterValue:
+    def is_none(self, val: bool) -> _Filters:
         """Filter on whether the property is `None`."""
         return _FilterValue(
             target=self._target_path(),
             value=val,
             operator=_Operator.IS_NULL,
         )
 
-    def contains_any(self, val: FilterValuesList) -> _FilterValue:
+    def contains_any(self, val: FilterValuesList) -> _Filters:
         """Filter on whether the property contains any of the given values."""
+        if len(val) == 0:
+            raise WeaviateInvalidInputError("Filter contains_any must have at least one value")
         return _FilterValue(
             target=self._target_path(),
             value=val,
             operator=_Operator.CONTAINS_ANY,
         )
 
-    def contains_all(self, val: FilterValuesList) -> _FilterValue:
+    def contains_all(self, val: FilterValuesList) -> _Filters:
         """Filter on whether the property contains all of the given values."""
+        if len(val) == 0:
+            raise WeaviateInvalidInputError("Filter contains_all must have at least one value")
+
         return _FilterValue(
             target=self._target_path(),
             value=val,
             operator=_Operator.CONTAINS_ALL,
         )
 
-    def equal(self, val: FilterValues) -> _FilterValue:
+    def equal(self, val: FilterValues) -> _Filters:
         """Filter on whether the property is equal to the given value."""
         return _FilterValue(target=self._target_path(), value=val, operator=_Operator.EQUAL)
 
-    def not_equal(self, val: FilterValues) -> _FilterValue:
+    def not_equal(self, val: FilterValues) -> _Filters:
         """Filter on whether the property is not equal to the given value."""
         return _FilterValue(target=self._target_path(), value=val, operator=_Operator.NOT_EQUAL)
 
-    def less_than(self, val: FilterValues) -> _FilterValue:
+    def less_than(self, val: FilterValues) -> _Filters:
         """Filter on whether the property is less than the given value."""
         return _FilterValue(target=self._target_path(), value=val, operator=_Operator.LESS_THAN)
 
-    def less_or_equal(self, val: FilterValues) -> _FilterValue:
+    def less_or_equal(self, val: FilterValues) -> _Filters:
         """Filter on whether the property is less than or equal to the given value."""
         return _FilterValue(
             target=self._target_path(),
             value=val,
             operator=_Operator.LESS_THAN_EQUAL,
         )
 
-    def greater_than(self, val: FilterValues) -> _FilterValue:
+    def greater_than(self, val: FilterValues) -> _Filters:
         """Filter on whether the property is greater than the given value."""
         return _FilterValue(
             target=self._target_path(),
             value=val,
             operator=_Operator.GREATER_THAN,
         )
 
-    def greater_or_equal(self, val: FilterValues) -> _FilterValue:
+    def greater_or_equal(self, val: FilterValues) -> _Filters:
         """Filter on whether the property is greater than or equal to the given value."""
         return _FilterValue(
             target=self._target_path(),
             value=val,
             operator=_Operator.GREATER_THAN_EQUAL,
         )
 
-    def like(self, val: str) -> _FilterValue:
+    def like(self, val: str) -> _Filters:
         """Filter on whether the property is like the given value.
 
         This filter can make use of `*` and `?` as wildcards. See [the docs](https://weaviate.io/developers/weaviate/search/filters#by-partial-matches-text) for more details.
         """
         return _FilterValue(target=self._target_path(), value=val, operator=_Operator.LIKE)
 
-    def within_geo_range(self, coordinate: GeoCoordinate, distance: float) -> _FilterValue:
+    def within_geo_range(self, coordinate: GeoCoordinate, distance: float) -> _Filters:
         """Filter on whether the property is within a given range of a geo-coordinate.
 
         See [the docs](https://weaviate.io/developers/weaviate/search/filters##by-geo-coordinates) for more details.
         """
         return _FilterValue(
             target=self._target_path(),
             value=_GeoCoordinateFilter(
                 latitude=coordinate.latitude, longitude=coordinate.longitude, distance=distance
             ),
             operator=_Operator.WITHIN_GEO_RANGE,
         )
 
 
 class _FilterByTime(_FilterBase):
-    def contains_any(self, dates: List[datetime]) -> _FilterValue:
+    def contains_any(self, dates: List[datetime]) -> _Filters:
         """Filter for objects with the given time.
 
         Arguments:
             `dates`
                 List of dates to filter on.
             `on_reference_path`
                 If the filter is on a cross-ref property, the path to the property to be filtered on, example: on_reference_path=["ref_property", "target_collection"].
         """
         return _FilterValue(
             target=self._target_path(),
             value=dates,
             operator=_Operator.CONTAINS_ANY,
         )
 
-    def equal(self, date: datetime) -> _FilterValue:
+    def equal(self, date: datetime) -> _Filters:
         """Filter on whether the creation time is equal to the given time.
 
         Arguments:
             `date`
                 date to filter on.
             `on_reference_path`
                 If the filter is on a cross-ref property, the path to the property to be filtered on, example: on_reference_path=["ref_property", "target_collection"].
         """
         return _FilterValue(
             target=self._target_path(),
             value=date,
             operator=_Operator.EQUAL,
         )
 
-    def not_equal(self, date: datetime) -> _FilterValue:
+    def not_equal(self, date: datetime) -> _Filters:
         """Filter on whether the creation time is not equal to the given time.
 
         Arguments:
             `date`
                 date to filter on.
             `on_reference_path`
                 If the filter is on a cross-ref property, the path to the property to be filtered on, example: on_reference_path=["ref_property", "target_collection"].
         """
         return _FilterValue(
             target=self._target_path(),
             value=date,
             operator=_Operator.NOT_EQUAL,
         )
 
-    def less_than(self, date: datetime) -> _FilterValue:
+    def less_than(self, date: datetime) -> _Filters:
         """Filter on whether the creation time is less than the given time.
 
         Arguments:
             `date`
                 date to filter on.
             `on_reference_path`
                 If the filter is on a cross-ref property, the path to the property to be filtered on, example: on_reference_path=["ref_property", "target_collection"].
         """
         return _FilterValue(
             target=self._target_path(),
             value=date,
             operator=_Operator.LESS_THAN,
         )
 
-    def less_or_equal(self, date: datetime) -> _FilterValue:
+    def less_or_equal(self, date: datetime) -> _Filters:
         """Filter on whether the creation time is less than or equal to the given time.
 
         Arguments:
             `date`
                 date to filter on.
             `on_reference_path`
                 If the filter is on a cross-ref property, the path to the property to be filtered on, example: on_reference_path=["ref_property", "target_collection"].
         """
         return _FilterValue(
             target=self._target_path(),
             value=date,
             operator=_Operator.LESS_THAN_EQUAL,
         )
 
-    def greater_than(self, date: datetime) -> _FilterValue:
+    def greater_than(self, date: datetime) -> _Filters:
         """Filter on whether the creation time is greater than the given time.
 
         Arguments:
             `date`
                 date to filter on.
             `on_reference_path`
                 If the filter is on a cross-ref property, the path to the property to be filtered on, example: on_reference_path=["ref_property", "target_collection"].
         """
         return _FilterValue(
             target=self._target_path(),
             value=date,
             operator=_Operator.GREATER_THAN,
         )
 
-    def greater_or_equal(self, date: datetime) -> _FilterValue:
+    def greater_or_equal(self, date: datetime) -> _Filters:
         """Filter on whether the creation time is greater than or equal to the given time.
 
         Arguments:
             `date`
                 date to filter on.
             `on_reference_path`
                 If the filter is on a cross-ref property, the path to the property to be filtered on, example: on_reference_path=["ref_property", "target_collection"].
@@ -353,110 +360,112 @@
 
 
 class _FilterById(_FilterBase):
     def __init__(self, target: Optional[_TargetRefs] = None) -> None:
         self._target = target
         self._property = "_id"
 
-    def contains_any(self, uuids: List[UUID]) -> _FilterValue:
+    def contains_any(self, uuids: List[UUID]) -> _Filters:
         """Filter for objects that has one of the given ID."""
+        if len(uuids) == 0:
+            raise WeaviateInvalidInputError("Filter contains_any must have at least one value")
         return _FilterValue(
             target=self._target_path(),
             value=[get_valid_uuid(val) for val in uuids],
             operator=_Operator.CONTAINS_ANY,
         )
 
-    def equal(self, uuid: UUID) -> _FilterValue:
+    def equal(self, uuid: UUID) -> _Filters:
         """Filter for object that has the given ID."""
         return _FilterValue(
             target=self._target_path(),
             value=get_valid_uuid(uuid),
             operator=_Operator.EQUAL,
         )
 
-    def not_equal(self, uuid: UUID) -> _FilterValue:
+    def not_equal(self, uuid: UUID) -> _Filters:
         """Filter our object that has the given ID."""
         return _FilterValue(
             target=self._target_path(),
             value=get_valid_uuid(uuid),
             operator=_Operator.NOT_EQUAL,
         )
 
 
 class _FilterByCount(_FilterBase):
     def __init__(self, link_on: str, target: Optional[_TargetRefs] = None) -> None:
         self._target = target
         self._property = _CountRef(link_on=link_on)
 
-    def equal(self, count: int) -> _FilterValue:
+    def equal(self, count: int) -> _Filters:
         """Filter on whether the number of references is equal to the given integer.
 
         Arguments:
             `count`
                 count to filter on.
         """
         return _FilterValue(
             target=self._target_path(),
             value=count,
             operator=_Operator.EQUAL,
         )
 
-    def not_equal(self, count: int) -> _FilterValue:
+    def not_equal(self, count: int) -> _Filters:
         """Filter on whether the number of references is equal to the given integer.
 
         Arguments:
             `count`
                 count to filter on.
         """
         return _FilterValue(
             target=self._target_path(),
             value=count,
             operator=_Operator.NOT_EQUAL,
         )
 
-    def less_than(self, count: int) -> _FilterValue:
+    def less_than(self, count: int) -> _Filters:
         """Filter on whether the number of references is equal to the given integer.
 
         Arguments:
             `count`
                 count to filter on.
         """
         return _FilterValue(
             target=self._target_path(),
             value=count,
             operator=_Operator.LESS_THAN,
         )
 
-    def less_or_equal(self, count: int) -> _FilterValue:
+    def less_or_equal(self, count: int) -> _Filters:
         """Filter on whether the number of references is equal to the given integer.
 
         Arguments:
             `count`
                 count to filter on.
         """
         return _FilterValue(
             target=self._target_path(),
             value=count,
             operator=_Operator.LESS_THAN_EQUAL,
         )
 
-    def greater_than(self, count: int) -> _FilterValue:
+    def greater_than(self, count: int) -> _Filters:
         """Filter on whether the number of references is equal to the given integer.
 
         Arguments:
             `count`
                 count to filter on.
         """
         return _FilterValue(
             target=self._target_path(),
             value=count,
             operator=_Operator.GREATER_THAN,
         )
 
-    def greater_or_equal(self, count: int) -> _FilterValue:
+    def greater_or_equal(self, count: int) -> _Filters:
         """Filter on whether the number of references is equal to the given integer.
 
         Arguments:
             `count`
                 count to filter on.
         """
         return _FilterValue(
@@ -548,14 +557,32 @@
         return _FilterByUpdateTime(target=None)
 
     @staticmethod
     def by_property(name: str, length: bool = False) -> _FilterByProperty:
         """Define a filter based on a property to be used when querying and deleting from a collection."""
         return _FilterByProperty(prop=name, length=length, target=None)
 
+    @staticmethod
+    def all_of(filters: List[_Filters]) -> _Filters:
+        """Combine all filters in the input list with an AND operator."""
+        if len(filters) == 1:
+            return filters[0]
+        elif len(filters) == 0:
+            raise WeaviateInvalidInputError("Filter.all_of must have at least one filter")
+        return _FilterAnd(filters)
+
+    @staticmethod
+    def any_of(filters: List[_Filters]) -> _Filters:
+        """Combine all filters in the input list with an OR operator."""
+        if len(filters) == 1:
+            return filters[0]
+        elif len(filters) == 0:
+            raise WeaviateInvalidInputError("Filter.any_of must have at least one filter")
+        return _FilterOr(filters)
+
 
 # type aliases for return classes
 FilterByProperty: TypeAlias = _FilterByProperty
 FilterById: TypeAlias = _FilterById
 FilterByCreationTime: TypeAlias = _FilterByCreationTime
 FilterByUpdateTime: TypeAlias = _FilterByUpdateTime
 FilterByRef: TypeAlias = _FilterByRef
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/internal.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/internal.py`

 * *Files 3% similar despite different names*

```diff
@@ -555,14 +555,20 @@
 # are listed first and in the order of their appearance in the typealias.
 # GenerativeNearMediaReturn[Properties, References, TProperties, TReferences] is the intended use and so
 # these four generics appear first. All others resolve afterwards correctly
 GenerativeNearMediaReturnType = Union[
     GenerativeReturnType[Properties, References, TProperties, TReferences],
     GenerativeGroupByReturnType[Properties, References, TProperties, TReferences],
 ]
+"""@Deprecated: Use `GenerativeSearchReturnType` instead."""
+
+GenerativeSearchReturnType = Union[
+    GenerativeReturnType[Properties, References, TProperties, TReferences],
+    GenerativeGroupByReturnType[Properties, References, TProperties, TReferences],
+]
 
 QueryReturnType = Union[
     QueryReturn[Properties, References],
     QueryReturn[TProperties, TReferences],
     QueryReturn[Properties, CrossReferences],
     QueryReturn[Properties, TReferences],
     QueryReturn[TProperties, References],
@@ -574,11 +580,17 @@
     GroupByReturn[TProperties, TReferences],
     GroupByReturn[Properties, CrossReferences],
     GroupByReturn[Properties, TReferences],
     GroupByReturn[TProperties, References],
     GroupByReturn[TProperties, CrossReferences],
 ]
 
+QuerySearchReturnType = Union[
+    QueryReturnType[Properties, References, TProperties, TReferences],
+    GroupByReturnType[Properties, References, TProperties, TReferences],
+]
+
 QueryNearMediaReturnType = Union[
     QueryReturnType[Properties, References, TProperties, TReferences],
     GroupByReturnType[Properties, References, TProperties, TReferences],
 ]
+"""@Deprecated: Use `QuerySearchReturnType` instead."""
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/orm.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/classes/types.py` & `weaviate_client-4.6.0b0/weaviate/collections/classes/types.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/cluster.py` & `weaviate_client-4.6.0b0/weaviate/collections/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/collection.py` & `weaviate_client-4.6.0b0/weaviate/collections/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import uuid as uuid_package
 from dataclasses import asdict
 from typing import Generic, Literal, Optional, Type, Union, overload
 
 from weaviate.collections.aggregate import _AggregateCollection
 from weaviate.collections.backups import _CollectionBackup
 from weaviate.collections.base import _CollectionBase
 from weaviate.collections.batch.collection import _BatchCollectionWrapper
@@ -21,14 +22,15 @@
 from weaviate.collections.classes.types import Properties, TProperties
 from weaviate.collections.config import _ConfigCollection
 from weaviate.collections.data import _DataCollection
 from weaviate.collections.iterator import _ObjectIterator
 from weaviate.collections.query import _GenerateCollection, _QueryCollection
 from weaviate.collections.tenants import _Tenants
 from weaviate.connect import ConnectionV4
+from weaviate.types import UUID
 from weaviate.validator import _validate_input, _ValidateArgument
 
 
 class Collection(_CollectionBase, Generic[Properties, References]):
     """The collection class is the main entry point for interacting with a collection in Weaviate.
 
     This class is returned by the `client.collections.create` and `client.collections.get` methods. It provides
@@ -68,20 +70,20 @@
     ) -> None:
         super().__init__(connection, name, validate_arguments)
 
         self.aggregate = _AggregateCollection(
             self._connection, self.name, consistency_level, tenant
         )
         """This namespace includes all the querying methods available to you when using Weaviate's standard aggregation capabilities."""
+        self.config = _ConfigCollection(self._connection, self.name, tenant)
+        """This namespace includes all the CRUD methods available to you when modifying the configuration of the collection in Weaviate."""
         self.batch = _BatchCollectionWrapper[Properties](
-            connection, consistency_level, self.name, tenant
+            connection, consistency_level, self.name, tenant, self.config
         )
         """This namespace contains all the functionality to upload data in batches to Weaviate for this specific collection."""
-        self.config = _ConfigCollection(self._connection, self.name, tenant)
-        """This namespace includes all the CRUD methods available to you when modifying the configuration of the collection in Weaviate."""
         self.data = _DataCollection[Properties](
             connection, self.name, consistency_level, tenant, validate_arguments, properties
         )
         """This namespace includes all the CUD methods available to you when modifying the data of the collection in Weaviate."""
         self.generate = _GenerateCollection(
             connection,
             self.name,
@@ -98,15 +100,15 @@
             consistency_level,
             tenant,
             properties,
             references,
             validate_arguments,
         )
         """This namespace includes all the querying methods available to you when using Weaviate's standard query capabilities."""
-        self.tenants = _Tenants(connection, self.name)
+        self.tenants = _Tenants(connection, self.name, consistency_level, validate_arguments)
         """This namespace includes all the CRUD methods available to you when modifying the tenants of a multi-tenancy-enabled collection in Weaviate."""
 
         self.backup = _CollectionBackup(connection, self.name)
         """This namespace includes all the backup methods available to you when backing up a collection in Weaviate."""
 
         self.__tenant = tenant
         self.__consistency_level = consistency_level
@@ -188,78 +190,87 @@
     def iterator(
         self,
         include_vector: bool = False,
         return_metadata: Optional[METADATA] = None,
         *,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
+        after: Optional[UUID] = None,
     ) -> _ObjectIterator[Properties, References]:
         ...
 
     @overload
     def iterator(
         self,
         include_vector: bool = False,
         return_metadata: Optional[METADATA] = None,
         *,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
+        after: Optional[UUID] = None,
     ) -> _ObjectIterator[Properties, CrossReferences]:
         ...
 
     @overload
     def iterator(
         self,
         include_vector: bool = False,
         return_metadata: Optional[METADATA] = None,
         *,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
+        after: Optional[UUID] = None,
     ) -> _ObjectIterator[Properties, TReferences]:
         ...
 
     @overload
     def iterator(
         self,
         include_vector: bool = False,
         return_metadata: Optional[METADATA] = None,
         *,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
+        after: Optional[UUID] = None,
     ) -> _ObjectIterator[TProperties, References]:
         ...
 
     @overload
     def iterator(
         self,
         include_vector: bool = False,
         return_metadata: Optional[METADATA] = None,
         *,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
+        after: Optional[UUID] = None,
     ) -> _ObjectIterator[TProperties, CrossReferences]:
         ...
 
     @overload
     def iterator(
         self,
         include_vector: bool = False,
         return_metadata: Optional[METADATA] = None,
         *,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
+        after: Optional[UUID] = None,
     ) -> _ObjectIterator[TProperties, TReferences]:
         ...
 
-    def iterator(
+    # weaviate/collections/collection.py:263: error: Overloaded function implementation does not accept all possible arguments of signature 3  [misc]
+    # weaviate/collections/collection.py:263: error: Overloaded function implementation cannot produce return type of signature 3  [misc]
+    def iterator(  # type: ignore
         self,
         include_vector: bool = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
+        after: Optional[UUID] = None,
     ) -> Union[
         _ObjectIterator[Properties, References],
         _ObjectIterator[Properties, CrossReferences],
         _ObjectIterator[Properties, TReferences],
         _ObjectIterator[TProperties, References],
         _ObjectIterator[TProperties, CrossReferences],
         _ObjectIterator[TProperties, TReferences],
@@ -279,22 +290,27 @@
                 Whether to include the vector in the metadata of the returned objects.
             `return_metadata`
                 The metadata to return with each object.
             `return_properties`
                 The properties to return with each object.
             `return_references`
                 The references to return with each object.
+            `after`
+                The cursor to use to mark the initial starting point of the iterator in the collection.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
                 If the request to the Weaviate server fails.
         """
         return _ObjectIterator(  # type: ignore
             lambda limit, after: self.query.fetch_objects(  # pyright: ignore # problems with invariance of list
                 limit=limit,
                 after=after,
                 include_vector=include_vector,
                 return_metadata=return_metadata,
                 return_properties=return_properties,
                 return_references=return_references,
-            ).objects
+            ).objects,
+            after
+            if after is None or isinstance(after, uuid_package.UUID)
+            else uuid_package.UUID(after),
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/collections.py` & `weaviate_client-4.6.0b0/weaviate/collections/collections.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from weaviate.collections.classes.internal import References
 from weaviate.collections.classes.types import (
     Properties,
     _check_properties_generic,
     _check_references_generic,
 )
 from weaviate.collections.collection import Collection
-from weaviate.exceptions import WeaviateInvalidInputError
+from weaviate.exceptions import WeaviateInvalidInputError, WeaviateUnsupportedFeatureError
 from weaviate.validator import _validate_input, _ValidateArgument
 from weaviate.util import _capitalize_first_letter
 
 
 class _Collections(_CollectionsBase):
     def create(
         self,
@@ -95,14 +95,16 @@
                 The generic class that you want to use to represent the references of objects in this collection. See the `get` method for more information.
             `skip_argument_validation`
                 If arguments to functions such as near_vector should be validated. Disable this if you need to squeeze out some extra performance.
 
         Raises:
             `weaviate.WeaviateInvalidInputError`
                 If the input parameters are invalid.
+            `weaviate.exceptions.WeaviateUnsupportedFeatureError`
+                If the Weaviate version is lower than 1.24.0 and named vectorizers are provided.
             `weaviate.WeaviateConnectionError`
                 If the network connection to Weaviate fails.
             `weaviate.UnexpectedStatusCodeError`
                 If Weaviate reports a non-OK status.
         """
         if isinstance(vectorizer_config, list) and self._connection._weaviate_version.is_lower_than(
             1, 24, 0
@@ -121,16 +123,18 @@
                 references=references,
                 replication_config=replication_config,
                 reranker_config=reranker_config,
                 sharding_config=sharding_config,
                 vectorizer_config=vectorizer_config or _Vectorizer.none(),
                 vector_index_config=vector_index_config,
             )
-        except ValidationError as e:
-            raise WeaviateInvalidInputError("Invalid collection config create parameters.") from e
+        except ValidationError:
+            raise WeaviateUnsupportedFeatureError(
+                "Named vectorizers", self._connection.server_version, "1.24.0"
+            )
         name = super()._create(config._to_dict())
         assert (
             config.name == name
         ), f"Name of created collection ({name}) does not match given name ({config.name})"
         return self.get(
             name,
             data_model_properties,
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/config.py` & `weaviate_client-4.6.0b0/weaviate/collections/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,33 @@
     CollectionConfig,
     CollectionConfigSimple,
     _Property,
     _ReferenceProperty,
     ShardStatus,
     _ShardStatus,
     ShardTypes,
+    _NamedVectorConfigUpdate,
+    _MultiTenancyConfigUpdate,
 )
 from weaviate.collections.classes.config_methods import (
     _collection_config_from_json,
     _collection_config_simple_from_json,
 )
 from weaviate.validator import _validate_input, _ValidateArgument
 from weaviate.connect import ConnectionV4
 from weaviate.exceptions import (
     WeaviateInvalidInputError,
 )
 from weaviate.util import _decode_json_response_dict, _decode_json_response_list
+from weaviate.warnings import _Warnings
 
 from weaviate.connect.v4 import _ExpectedStatusCodes
 
+from weaviate.collections.classes.config_vector_index import _VectorIndexConfigDynamicUpdate
+
 
 class _ConfigBase:
     def __init__(self, connection: ConnectionV4, name: str, tenant: Optional[str]) -> None:
         self.__connection = connection
         self._name = name
         self.__tenant = tenant
 
@@ -81,22 +86,29 @@
     def update(
         self,
         *,
         description: Optional[str] = None,
         inverted_index_config: Optional[_InvertedIndexConfigUpdate] = None,
         replication_config: Optional[_ReplicationConfigUpdate] = None,
         vector_index_config: Optional[
-            Union[_VectorIndexConfigHNSWUpdate, _VectorIndexConfigFlatUpdate]
+            Union[
+                _VectorIndexConfigHNSWUpdate,
+                _VectorIndexConfigFlatUpdate,
+                _VectorIndexConfigDynamicUpdate,
+            ]
         ] = None,
         vectorizer_config: Optional[
             Union[
                 _VectorIndexConfigHNSWUpdate,
                 _VectorIndexConfigFlatUpdate,
+                _VectorIndexConfigDynamicUpdate,
+                List[_NamedVectorConfigUpdate],
             ]
         ] = None,
+        multi_tenancy_config: Optional[_MultiTenancyConfigUpdate] = None,
     ) -> None:
         """Update the configuration for this collection in Weaviate.
 
         Use the `weaviate.classes.Reconfigure` class to generate the necessary configuration objects for this method.
 
         Arguments:
             `description`
@@ -104,36 +116,43 @@
             `inverted_index_config`
                 Configuration for the inverted index. Use `Reconfigure.inverted_index` to generate one.
             `replication_config`
                 Configuration for the replication. Use `Reconfigure.replication` to generate one.
             `vector_index_config` DEPRECATED USE `vectorizer_config` INSTEAD
                 Configuration for the vector index of the default single vector. Use `Reconfigure.vector_index` to generate one.
             `vectorizer_config`
-                Configuration for the vector index of the default single vector. Use `Reconfigure.vector_index` to generate one.
+                Configurations for the vector index (or indices) of your collection.
+                Use `Reconfigure.vector_index` if there is only one vectorizer and `Reconfigure.NamedVectors` if you have many named vectors to generate them.
+            `multi_tenancy_config`
+                Configuration for multi-tenancy settings. Use `Reconfigure.multi_tenancy` to generate one.
+                Only `auto_tenant_creation` is supported.
 
         Raises:
             `weaviate.WeaviateInvalidInputError`:
                 If the input parameters are invalid.
             `weaviate.WeaviateConnectionError`:
                 If the network connection to Weaviate fails.
             `weaviate.UnexpectedStatusCodeError`:
                 If Weaviate reports a non-OK status.
 
         NOTE:
             - If you wish to update a specific option within the configuration and cannot find it in `CollectionConfigUpdate` then it is an immutable option.
             - To change it, you will have to delete the collection and recreate it with the desired options.
             - This is not the case of adding properties, which can be done with `collection.config.add_property()`.
         """
+        if vector_index_config is not None:
+            _Warnings.vector_index_config_in_config_update()
         try:
             config = _CollectionConfigUpdate(
                 description=description,
                 inverted_index_config=inverted_index_config,
                 replication_config=replication_config,
                 vector_index_config=vector_index_config,
                 vectorizer_config=vectorizer_config,
+                multi_tenancy_config=multi_tenancy_config,
             )
         except ValidationError as e:
             raise WeaviateInvalidInputError("Invalid collection config update parameters.") from e
         schema = self.__get()
         schema = config.merge_with_existing(schema)
         self.__connection.put(
             path=f"/schema/{self._name}",
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/data.py` & `weaviate_client-4.6.0b0/weaviate/collections/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,14 +325,21 @@
             self.name,
             self._consistency_level,
             self._tenant,
             self._validate_arguments,
             data_model,
         )
 
+    def __parse_vector(self, obj: Dict[str, Any], vector: VECTORS) -> Dict[str, Any]:
+        if isinstance(vector, dict):
+            obj["vectors"] = {key: _get_vector_v4(val) for key, val in vector.items()}
+        else:
+            obj["vector"] = _get_vector_v4(vector)
+        return obj
+
     def insert(
         self,
         properties: Properties,
         references: Optional[ReferenceInputs] = None,
         uuid: Optional[UUID] = None,
         vector: Optional[VECTORS] = None,
     ) -> uuid_package.UUID:
@@ -342,17 +349,17 @@
             `properties`
                 The properties of the object, REQUIRED.
             `references`
                 Any references to other objects in Weaviate.
             `uuid`
                 The UUID of the object. If not provided, a random UUID will be generated.
             `vector`
-                The vector of the object.
+                The vector(s) of the object.
                 Supported types are
-                - for single vectors: `list`, 'numpy.ndarray`, `torch.Tensor` and `tf.Tensor`, by default None.
+                - for single vectors: `list`, 'numpy.ndarray`, `torch.Tensor`, `tf.Tensor`, `pd.Series` and `pl.Series`, by default None.
                 - for named vectors: Dict[str, *list above*], where the string is the name of the vector.
 
         Returns:
             `uuid.UUID`, the UUID of the inserted object.
 
         Raises:
             `weaviate.exceptions.UnexpectedStatusCodeError`:
@@ -374,22 +381,16 @@
         props = self._serialize_props(properties) if properties is not None else {}
         refs = self._serialize_refs(references) if references is not None else {}
         weaviate_obj: Dict[str, Any] = {
             "class": self.name,
             "properties": {**props, **refs},
             "id": str(uuid if uuid is not None else uuid_package.uuid4()),
         }
-
         if vector is not None:
-            if isinstance(vector, dict):
-                for key, val in vector.items():
-                    vector[key] = _get_vector_v4(val)
-                weaviate_obj["vectors"] = vector
-            else:
-                weaviate_obj["vector"] = _get_vector_v4(vector)
+            weaviate_obj = self.__parse_vector(weaviate_obj, vector)
 
         return self._insert(weaviate_obj)
 
     def insert_many(
         self,
         objects: Sequence[Union[Properties, DataObject[Properties, Optional[ReferenceInputs]]]],
     ) -> BatchObjectReturn:
@@ -428,37 +429,40 @@
                         properties=cast(dict, obj),
                         tenant=self._tenant,
                         references=None,
                     )
                 )
                 for obj in objects
             ],
-            timeout=self._connection.timeout_config.connect,
+            timeout=self._connection.timeout_config.insert,
         )
 
     def replace(
         self,
         uuid: UUID,
         properties: Properties,
         references: Optional[ReferenceInputs] = None,
-        vector: Optional[Sequence[float]] = None,
+        vector: Optional[VECTORS] = None,
     ) -> None:
         """Replace an object in the collection.
 
         This is equivalent to a PUT operation.
 
         Arguments:
             `uuid`
                 The UUID of the object, REQUIRED.
             `properties`
                 The properties of the object, REQUIRED.
             `references`
                 Any references to other objects in Weaviate, REQUIRED.
             `vector`
-                The vector of the object.
+                The vector(s) of the object.
+                Supported types are
+                - for single vectors: `list`, 'numpy.ndarray`, `torch.Tensor`, `tf.Tensor`, `pd.Series` and `pl.Series`, by default None.
+                - for named vectors: Dict[str, *list above*], where the string is the name of the vector.
 
         Raises:
             `weaviate.WeaviateConnectionError`:
                 If the network connection to Weaviate fails.
             `weaviate.exceptions.WeaviateInvalidInputError`:
                 If any of the arguments are invalid.
             `weaviate.UnexpectedStatusCodeError`:
@@ -470,34 +474,36 @@
             _validate_input(
                 [
                     _ValidateArgument(expected=[UUID], name="uuid", value=uuid),
                     _ValidateArgument(expected=[Mapping], name="properties", value=properties),
                     _ValidateArgument(
                         expected=[Mapping, None], name="references", value=references
                     ),
-                    _ValidateArgument(expected=[Sequence, None], name="vector", value=vector),
+                    _ValidateArgument(
+                        expected=[Sequence, None, Mapping], name="vector", value=vector
+                    ),
                 ]
             )
         props = self._serialize_props(properties) if properties is not None else {}
         refs = self._serialize_refs(references) if references is not None else {}
         weaviate_obj: Dict[str, Any] = {
             "class": self.name,
             "properties": {**props, **refs},
         }
         if vector is not None:
-            weaviate_obj["vector"] = _get_vector_v4(vector)
+            weaviate_obj = self.__parse_vector(weaviate_obj, vector)
 
         self._replace(weaviate_obj, uuid=uuid)
 
     def update(
         self,
         uuid: UUID,
         properties: Optional[Properties] = None,
         references: Optional[ReferenceInputs] = None,
-        vector: Optional[List[float]] = None,
+        vector: Optional[VECTORS] = None,
     ) -> None:
         """Update an object in the collection.
 
         This is equivalent to a PATCH operation.
 
         If the object does not exist yet, it will be created.
 
@@ -505,34 +511,39 @@
             `uuid`
                 The UUID of the object, REQUIRED.
             `properties`
                 The properties of the object.
             `references`
                 Any references to other objects in Weaviate.
             `vector`
-                The vector of the object.
+                The vector(s) of the object.
+                Supported types are
+                - for single vectors: `list`, 'numpy.ndarray`, `torch.Tensor`, `tf.Tensor`, `pd.Series` and `pl.Series`, by default None.
+                - for named vectors: Dict[str, *list above*], where the string is the name of the vector.
         """
         if self._validate_arguments:
             _validate_input(
                 [
                     _ValidateArgument(expected=[UUID], name="uuid", value=uuid),
                     _ValidateArgument(
                         expected=[Mapping, None], name="properties", value=properties
                     ),
                     _ValidateArgument(
                         expected=[Mapping, None], name="references", value=references
                     ),
-                    _ValidateArgument(expected=[Sequence, None], name="vector", value=vector),
+                    _ValidateArgument(
+                        expected=[Sequence, None, Mapping], name="vector", value=vector
+                    ),
                 ],
             )
         props = self._serialize_props(properties) if properties is not None else {}
         refs = self._serialize_refs(references) if references is not None else {}
         weaviate_obj: Dict[str, Any] = {"class": self.name, "properties": {**props, **refs}}
         if vector is not None:
-            weaviate_obj["vector"] = _get_vector_v4(vector)
+            weaviate_obj = self.__parse_vector(weaviate_obj, vector)
 
         self._update(weaviate_obj, uuid=uuid)
 
     def reference_add(self, from_uuid: UUID, from_property: str, to: SingleReferenceInput) -> None:
         """Create a reference between an object in this collection and any other object in Weaviate.
 
         Arguments:
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/filters.py` & `weaviate_client-4.6.0b0/weaviate/collections/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/grpc/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/grpc/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from weaviate.collections.classes.config import ConsistencyLevel
 
 from weaviate.collections.classes.filters import _Filters
 from weaviate.collections.classes.grpc import (
     HybridFusion,
     _QueryReferenceMultiTarget,
     _MetadataQuery,
+    _HybridNearText,
+    _HybridNearVector,
+    HybridVectorType,
     Move,
     QueryNested,
     _QueryReference,
     PROPERTIES,
     PROPERTY,
     REFERENCE,
     REFERENCES,
@@ -26,15 +29,15 @@
 )
 from weaviate.collections.classes.internal import _Generative, _GroupBy
 from weaviate.collections.filters import _FilterToGRPC
 
 from weaviate.collections.grpc.shared import _BaseGRPC
 
 from weaviate.connect import ConnectionV4
-from weaviate.exceptions import WeaviateQueryError
+from weaviate.exceptions import WeaviateQueryError, WeaviateUnsupportedFeatureError
 from weaviate.types import NUMBER, UUID
 from weaviate.util import _get_vector_v4
 
 from weaviate.proto.v1 import search_get_pb2
 
 from weaviate.validator import _ValidateArgument, _validate_input
 
@@ -69,19 +72,21 @@
     def __init__(
         self,
         connection: ConnectionV4,
         name: str,
         tenant: Optional[str],
         consistency_level: Optional[ConsistencyLevel],
         validate_arguments: bool,
+        uses_125_api: bool,
     ):
         super().__init__(connection, consistency_level)
         self._name: str = name
         self._tenant = tenant
         self._validate_arguments = validate_arguments
+        self.__uses_125_api = uses_125_api
 
     def __parse_near_options(
         self,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
     ) -> Tuple[Optional[float], Optional[float]]:
         if self._validate_arguments:
@@ -133,109 +138,163 @@
             sort_by=sort_by,
         )
 
         return self.__call(request)
 
     def hybrid(
         self,
-        query: str,
+        query: Optional[str],
         alpha: Optional[float] = None,
-        vector: Optional[List[float]] = None,
+        vector: Optional[HybridVectorType] = None,
         properties: Optional[List[str]] = None,
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         autocut: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Optional[_GroupBy] = None,
         return_metadata: Optional[_MetadataQuery] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Optional[REFERENCES] = None,
         generative: Optional[_Generative] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
     ) -> search_get_pb2.SearchReply:
+        if self._connection._weaviate_version.is_lower_than(1, 25, 0) and (
+            isinstance(vector, _HybridNearText) or isinstance(vector, _HybridNearVector)
+        ):
+            raise WeaviateUnsupportedFeatureError(
+                "Hybrid search with NearText or NearVector",
+                str(self._connection._weaviate_version),
+                "1.25.0",
+            )
         if self._validate_arguments:
             _validate_input(
                 [
-                    _ValidateArgument([str], "query", query),
+                    _ValidateArgument([None, str], "query", query),
                     _ValidateArgument([float, int, None], "alpha", alpha),
-                    _ValidateArgument([List, None], "vector", vector),
+                    _ValidateArgument(
+                        [list, _HybridNearText, _HybridNearVector, None], "vector", vector
+                    ),
                     _ValidateArgument([List, None], "properties", properties),
                     _ValidateArgument([HybridFusion, None], "fusion_type", fusion_type),
                     _ValidateArgument([str, None], "target_vector", target_vector),
                 ]
             )
 
-        hybrid_search = search_get_pb2.Hybrid(
-            properties=properties,
-            query=query,
-            alpha=float(alpha) if alpha is not None else None,
-            vector_bytes=(
-                struct.pack("{}f".format(len(vector)), *vector) if vector is not None else None
-            ),
-            fusion_type=(
-                cast(
-                    search_get_pb2.Hybrid.FusionType,
-                    search_get_pb2.Hybrid.FusionType.Value(fusion_type.value),
-                )
-                if fusion_type is not None
-                else None
-            ),
-            target_vectors=[target_vector] if target_vector is not None else None,
+        # Set hybrid search to only query the other search-type if one of the two is not set
+        if query is None:
+            alpha = 1
+
+        hybrid_search = (
+            search_get_pb2.Hybrid(
+                properties=properties,
+                query=query,
+                alpha=float(alpha) if alpha is not None else None,
+                fusion_type=(
+                    cast(
+                        search_get_pb2.Hybrid.FusionType,
+                        search_get_pb2.Hybrid.FusionType.Value(fusion_type.value),
+                    )
+                    if fusion_type is not None
+                    else None
+                ),
+                target_vectors=[target_vector] if target_vector is not None else None,
+                vector_bytes=(
+                    struct.pack("{}f".format(len(vector)), *vector)
+                    if vector is not None and isinstance(vector, list)
+                    else None
+                ),
+                near_text=(
+                    search_get_pb2.NearTextSearch(
+                        query=[vector.text] if isinstance(vector.text, str) else vector.text,
+                        certainty=vector.certainty,
+                        distance=vector.distance,
+                        move_away=self.__parse_move(vector.move_away),
+                        move_to=self.__parse_move(vector.move_to),
+                        target_vectors=[vector.target_vector]
+                        if vector.target_vector is not None
+                        else None,
+                    )
+                    if vector is not None and isinstance(vector, _HybridNearText)
+                    else None
+                ),
+                near_vector=(
+                    search_get_pb2.NearVector(
+                        vector_bytes=struct.pack("{}f".format(len(vector.vector)), *vector.vector),
+                        certainty=vector.certainty,
+                        distance=vector.distance,
+                        target_vectors=[vector.target_vector]
+                        if vector.target_vector is not None
+                        else None,
+                    )
+                    if vector is not None and isinstance(vector, _HybridNearVector)
+                    else None
+                ),
+            )
+            if query is not None or vector is not None
+            else None
         )
 
         request = self.__create_request(
             limit=limit,
             offset=offset,
             filters=filters,
+            group_by=group_by,
             metadata=return_metadata,
             return_properties=return_properties,
             return_references=return_references,
             generative=generative,
             rerank=rerank,
             autocut=autocut,
             hybrid_search=hybrid_search,
         )
 
         return self.__call(request)
 
     def bm25(
         self,
-        query: str,
+        query: Optional[str],
         properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         autocut: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Optional[_GroupBy] = None,
         return_metadata: Optional[_MetadataQuery] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Optional[REFERENCES] = None,
         generative: Optional[_Generative] = None,
         rerank: Optional[Rerank] = None,
     ) -> search_get_pb2.SearchReply:
         if self._validate_arguments:
             _validate_input(
                 [
-                    _ValidateArgument([str], "query", query),
+                    _ValidateArgument([None, str], "query", query),
                     _ValidateArgument([List, None], "properties", properties),
                 ]
             )
 
         request = self.__create_request(
             limit=limit,
             offset=offset,
             filters=filters,
+            group_by=group_by,
             metadata=return_metadata,
             return_properties=return_properties,
             return_references=return_references,
             generative=generative,
             rerank=rerank,
             autocut=autocut,
-            bm25=search_get_pb2.BM25(
-                query=query, properties=properties if properties is not None else []
+            bm25=(
+                search_get_pb2.BM25(
+                    query=query, properties=properties if properties is not None else []
+                )
+                if query is not None
+                else None
             ),
         )
         return self.__call(request)
 
     def near_vector(
         self,
         near_vector: List[float],
@@ -367,28 +426,16 @@
         certainty, distance = self.__parse_near_options(certainty, distance)
 
         near_text_req = search_get_pb2.NearTextSearch(
             query=near_text,
             certainty=certainty,
             distance=distance,
             target_vectors=[target_vector] if target_vector is not None else None,
-            move_away=search_get_pb2.NearTextSearch.Move(
-                force=move_away.force,
-                concepts=move_away._concepts_list,
-                uuids=move_away._objects_list,
-            )
-            if move_away is not None
-            else None,
-            move_to=search_get_pb2.NearTextSearch.Move(
-                force=move_to.force,
-                concepts=move_to._concepts_list,
-                uuids=move_to._objects_list,
-            )
-            if move_to is not None
-            else None,
+            move_away=self.__parse_move(move_away),
+            move_to=self.__parse_move(move_to),
         )
 
         request = self.__create_request(
             limit=limit,
             offset=offset,
             filters=filters,
             metadata=return_metadata,
@@ -473,14 +520,26 @@
             rerank=rerank,
             autocut=autocut,
             group_by=group_by,
             **kwargs,
         )
         return self.__call(request)
 
+    @staticmethod
+    def __parse_move(move: Optional[Move]) -> Optional[search_get_pb2.NearTextSearch.Move]:
+        return (
+            search_get_pb2.NearTextSearch.Move(
+                force=move.force,
+                concepts=move._concepts_list,
+                uuids=move._objects_list,
+            )
+            if move is not None
+            else None
+        )
+
     def __create_request(
         self,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
         metadata: Optional[_MetadataQuery] = None,
@@ -551,14 +610,15 @@
                 return_properties
             )
         else:
             return_properties_parsed = None
 
         return search_get_pb2.SearchRequest(
             uses_123_api=True,
+            uses_125_api=self.__uses_125_api,
             collection=self._name,
             limit=limit,
             offset=offset,
             after=str(after) if after is not None else "",
             autocut=autocut,
             properties=self._translate_properties_from_python_to_grpc(
                 return_properties_parsed, return_references_parsed
@@ -591,15 +651,15 @@
     def __call(self, request: search_get_pb2.SearchRequest) -> search_get_pb2.SearchReply:
         try:
             assert self._connection.grpc_stub is not None
             res: search_get_pb2.SearchReply  # According to PEP-0526
             res, _ = self._connection.grpc_stub.Search.with_call(
                 request,
                 metadata=self._connection.grpc_headers(),
-                timeout=self._connection.timeout_config.connect,
+                timeout=self._connection.timeout_config.query,
             )
 
             return res
 
         except grpc.RpcError as e:
             raise WeaviateQueryError(e.details(), "GRPC search")  # pyright: ignore
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/grpc/shared.py` & `weaviate_client-4.6.0b0/weaviate/collections/grpc/shared.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/iterator.py` & `weaviate_client-4.6.0b0/weaviate/collections/iterator.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 
 
 ITERATOR_CACHE_SIZE = 100
 
 
 class _ObjectIterator(Generic[P, R], Iterable[Object[P, R]]):
     def __init__(
-        self, fetch_objects_query: Callable[[int, Optional[UUID]], List[Object[P, R]]]
+        self,
+        fetch_objects_query: Callable[[int, Optional[UUID]], List[Object[P, R]]],
+        init_after: Optional[UUID],
     ) -> None:
         self.__query = fetch_objects_query
+        self.__init_after = init_after
 
         self.__iter_object_cache: List[Object[P, R]] = []
-        self.__iter_object_last_uuid: Optional[UUID] = None
+        self.__iter_object_last_uuid: Optional[UUID] = init_after
 
     def __iter__(self) -> Iterator[Object[P, R]]:
         self.__iter_object_cache = []
-        self.__iter_object_last_uuid = None
+        self.__iter_object_last_uuid = self.__init_after
         return self
 
     def __next__(self) -> Object[P, R]:
         if len(self.__iter_object_cache) == 0:
             objects = self.__query(
                 ITERATOR_CACHE_SIZE,
                 self.__iter_object_last_uuid,
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/orm.py` & `weaviate_client-4.6.0b0/weaviate/collections/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/base.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import datetime
 import io
 import os
 import pathlib
-import struct
 import uuid as uuid_lib
 from typing import Any, Dict, Generic, List, Optional, Sequence, Type, Union, cast
 
 from typing_extensions import is_typeddict
 
 from weaviate.collections.classes.config import ConsistencyLevel
 from weaviate.collections.classes.grpc import (
@@ -22,37 +21,38 @@
     GroupByObject,
     MetadataReturn,
     GroupByMetadataReturn,
     GenerativeObject,
     Object,
     _extract_properties_from_data_model,
     _extract_references_from_data_model,
-    GenerativeNearMediaReturnType,
+    GenerativeSearchReturnType,
     GenerativeReturn,
     GenerativeGroupByReturn,
     GroupByReturn,
     GroupByReturnType,
     Group,
     GenerativeGroup,
     QueryReturn,
-    QueryNearMediaReturnType,
+    QuerySearchReturnType,
     _QueryOptions,
     ReturnProperties,
     ReturnReferences,
     CrossReferences,
     _CrossReference,
 )
 from weaviate.collections.classes.types import (
     GeoCoordinate,
     _PhoneNumber,
     Properties,
     TProperties,
     References,
     TReferences,
 )
+from weaviate.collections.queries.byteops import _ByteOps
 from weaviate.collections.grpc.query import _QueryGRPC
 from weaviate.connect import ConnectionV4
 from weaviate.exceptions import WeaviateInvalidInputError
 from weaviate.proto.v1 import search_get_pb2, properties_pb2
 from weaviate.util import (
     file_encoder_b64,
     _datetime_from_weaviate_str,
@@ -75,47 +75,56 @@
         name: str,
         consistency_level: Optional[ConsistencyLevel],
         tenant: Optional[str],
         properties: Optional[Type[Properties]],
         references: Optional[Type[References]],
         validate_arguments: bool,
     ):
-        self.__connection = connection
+        self._connection = connection
         self._name = name
         self.__tenant = tenant
         self.__consistency_level = consistency_level
         self._properties = properties
         self._references = references
         self._validate_arguments = validate_arguments
+
+        self.__uses_125_api = self._connection._weaviate_version.is_at_least(1, 25, 0)
         self._query = _QueryGRPC(
-            self.__connection,
+            self._connection,
             self._name,
             self.__tenant,
             self.__consistency_level,
             validate_arguments=self._validate_arguments,
+            uses_125_api=self.__uses_125_api,
         )
 
+    def __retrieve_timestamp(
+        self,
+        timestamp: int,
+    ) -> datetime.datetime:
+        # Handle the case in which last_update_time_unix is in nanoseconds or milliseconds, issue #958
+        if len(str(timestamp)) <= 13:
+            return datetime.datetime.fromtimestamp(timestamp / 1000, tz=datetime.timezone.utc)
+        else:
+            return datetime.datetime.fromtimestamp(timestamp / 1e9, tz=datetime.timezone.utc)
+
     def __extract_metadata_for_object(
         self,
         add_props: "search_get_pb2.MetadataResult",
     ) -> MetadataReturn:
         meta = MetadataReturn(
             distance=add_props.distance if add_props.distance_present else None,
             certainty=add_props.certainty if add_props.certainty_present else None,
             creation_time=(
-                datetime.datetime.fromtimestamp(
-                    add_props.creation_time_unix / 1000, tz=datetime.timezone.utc
-                )
+                self.__retrieve_timestamp(add_props.creation_time_unix)
                 if add_props.creation_time_unix_present
                 else None
             ),
             last_update_time=(
-                datetime.datetime.fromtimestamp(
-                    add_props.last_update_time_unix / 1000, tz=datetime.timezone.utc
-                )
+                self.__retrieve_timestamp(add_props.last_update_time_unix)
                 if add_props.last_update_time_unix_present
                 else None
             ),
             score=add_props.score if add_props.score_present else None,
             explain_score=add_props.explain_score if add_props.explain_score_present else None,
             is_consistent=add_props.is_consistent if add_props.is_consistent_present else None,
             rerank_score=add_props.rerank_score if add_props.rerank_score_present else None,
@@ -145,46 +154,73 @@
             len(add_props.vector_bytes) == 0
             and len(add_props.vector) == 0
             and len(add_props.vectors) == 0
         ):
             return {}
 
         if len(add_props.vector_bytes) > 0:
-            vector_bytes = struct.unpack(
-                f"{len(add_props.vector_bytes)//4}f", add_props.vector_bytes
-            )
-            return {"default": list(vector_bytes)}
+            return {"default": _ByteOps.decode_float32s(add_props.vector_bytes)}
 
         vecs = {}
         for vec in add_props.vectors:
-            vector_bytes = struct.unpack(f"{len(vec.vector_bytes)//4}f", vec.vector_bytes)
-            vecs[vec.name] = list(vector_bytes)
+            vecs[vec.name] = _ByteOps.decode_float32s(vec.vector_bytes)
         return vecs
 
     def __extract_generated_for_object(
         self,
         add_props: "search_get_pb2.MetadataResult",
     ) -> Optional[str]:
         return add_props.generative if add_props.generative_present else None
 
+    def __deserialize_list_value_prop_125(
+        self, value: properties_pb2.ListValue
+    ) -> Optional[List[Any]]:
+        if value.HasField("bool_values"):
+            return list(value.bool_values.values)
+        if value.HasField("date_values"):
+            return [_datetime_from_weaviate_str(val) for val in value.date_values.values]
+        if value.HasField("int_values"):
+            return _ByteOps.decode_int64s(value.int_values.values)
+        if value.HasField("number_values"):
+            return _ByteOps.decode_float64s(value.number_values.values)
+        if value.HasField("text_values"):
+            return list(value.text_values.values)
+        if value.HasField("uuid_values"):
+            return [uuid_lib.UUID(val) for val in value.uuid_values.values]
+        if value.HasField("object_values"):
+            return [
+                self.__parse_nonref_properties_result(val) for val in value.object_values.values
+            ]
+        _Warnings.unknown_type_encountered(value.WhichOneof("Value"))
+        return None
+
+    def __deserialize_list_value_prop_123(self, value: properties_pb2.ListValue) -> List[Any]:
+        return [self.__deserialize_non_ref_prop(val) for val in value.values]
+
     def __deserialize_non_ref_prop(self, value: properties_pb2.Value) -> Any:
         if value.HasField("uuid_value"):
             return uuid_lib.UUID(value.uuid_value)
         if value.HasField("date_value"):
             return _datetime_from_weaviate_str(value.date_value)
         if value.HasField("string_value"):
             return str(value.string_value)
+        if value.HasField("text_value"):
+            return str(value.text_value)
         if value.HasField("int_value"):
             return int(value.int_value)
         if value.HasField("number_value"):
             return float(value.number_value)
         if value.HasField("bool_value"):
             return bool(value.bool_value)
         if value.HasField("list_value"):
-            return [self.__deserialize_non_ref_prop(val) for val in value.list_value.values]
+            return (
+                self.__deserialize_list_value_prop_125(value.list_value)
+                if self.__uses_125_api
+                else self.__deserialize_list_value_prop_123(value.list_value)
+            )
         if value.HasField("object_value"):
             return self.__parse_nonref_properties_result(value.object_value)
         if value.HasField("geo_value"):
             return GeoCoordinate(
                 latitude=value.geo_value.latitude, longitude=value.geo_value.longitude
             )
         if value.HasField("blob_value"):
@@ -405,15 +441,15 @@
         options: _QueryOptions,
         properties: Optional[
             ReturnProperties[TProperties]
         ],  # required until 3.12 is minimum supported version to use new generics syntax
         references: Optional[
             ReturnReferences[TReferences]
         ],  # required until 3.12 is minimum supported version to use new generics syntax
-    ) -> GenerativeNearMediaReturnType[Properties, References, TProperties, TReferences]:
+    ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
         return (
             self._result_to_generative_query_return(res, options, properties, references)
             if options.is_group_by is False
             else self._result_to_generative_groupby_return(res, options, properties, references)
         )
 
     def _result_to_groupby_return(
@@ -484,15 +520,15 @@
         options: _QueryOptions,
         properties: Optional[
             ReturnProperties[TProperties]
         ],  # required until 3.12 is minimum supported version to use new generics syntax
         references: Optional[
             ReturnReferences[TReferences]
         ],  # required until 3.12 is minimum supported version to use new generics syntax
-    ) -> QueryNearMediaReturnType[Properties, References, TProperties, TReferences]:
+    ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
         return (
             self._result_to_query_return(res, options, properties, references)
             if not options.is_group_by
             else self._result_to_groupby_return(res, options, properties, references)
         )
 
     def _parse_return_properties(
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/bm25/generate.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,88 @@
 from typing import Generic, List, Optional
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import Rerank, METADATA
+from weaviate.collections.classes.grpc import METADATA, _Sorting
 from weaviate.collections.classes.internal import (
     GenerativeReturnType,
     _Generative,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
+from weaviate.types import UUID, INCLUDE_VECTOR
 
-from weaviate.types import INCLUDE_VECTOR
 
-
-class _BM25Generate(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def bm25(
+class _FetchObjectsGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def fetch_objects(
         self,
-        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[_Sorting] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
-        return_references: Optional[ReturnReferences[TReferences]] = None,
+        return_references: Optional[ReturnReferences[TReferences]] = None
     ) -> GenerativeReturnType[Properties, References, TProperties, TReferences]:
-        """Perform retrieval-augmented generation (RaG) on the results of a keyword-based BM25 search of objects in this collection.
-
-        See the [docs](https://weaviate.io/developers/weaviate/search/bm25) for a more detailed explanation.
+        """Perform retrieval-augmented generation (RaG) on the results of a simple get query of objects in this collection.
 
         Arguments:
-            `query`
-                The keyword-based query to search for, REQUIRED.
             `single_prompt`
                 The prompt to use for RaG on each object individually.
             `grouped_task`
                 The prompt to use for RaG on the entire result set.
             `grouped_properties`
                 The properties to use in the RaG on the entire result set.
-            `query_properties`
-                The properties to search in. If not specified, all properties are searched.
             `limit`
-                The maximum number of results to return. If not specified, the default limit specified by the server is returned.
+                The maximum number of results to return. If not specified, the default limit specified by Weaviate is returned.
             `offset`
-                The offset to start from. If not specified, the retrieval begins from the first object in the server.
-            `auto_limit`
-                The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
+                The offset to start from. If not specified, the retrieval begins from the first object in Weaviate.
+            `after`
+                The UUID of the object to start from. If not specified, the retrieval begins from the first object in Weaviate.
             `filters`
-                The filters to apply to the search.
-            `rerank`
-                How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+                The filters to apply to the retrieval.
+            `sort`
+                The sorting to apply to the retrieval.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
                 The references to return for each object.
 
         NOTE:
-            If `return_properties` is not provided then all non-reference properties are returned including nested properties.
-            If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
-            If `return_references` is not provided then no references are provided.
+            - If `return_properties` is not provided then all properties are returned except for blob properties.
+            - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
+            - If `return_references` is not provided then no references are provided.
 
         Returns:
             A `_GenerativeNearMediaReturn` object that includes the searched objects with per-object generated results and group generated results.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
                 If the network connection to Weaviate fails.
         """
-        res = self._query.bm25(
-            query=query,
-            properties=query_properties,
+        res = self._query.get(
             limit=limit,
             offset=offset,
-            autocut=auto_limit,
+            after=after,
             filters=filters,
-            rerank=rerank,
+            sort=sort,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
             generative=_Generative(
                 single=single_prompt,
                 grouped=grouped_task,
                 grouped_properties=grouped_properties,
@@ -103,12 +92,11 @@
             res,
             _QueryOptions.from_input(
                 return_metadata,
                 return_properties,
                 include_vector,
                 self._references,
                 return_references,
-                rerank,
             ),
             return_properties,
             return_references,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/bm25/generate.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/generate.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,135 +1,128 @@
-from typing import Generic, List, Literal, Optional, Type, overload
+from typing import Generic, List, Literal, Optional, Union, Type, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import Rerank, METADATA, PROPERTIES, REFERENCES
+from weaviate.collections.classes.grpc import (
+    METADATA,
+    PROPERTIES,
+    REFERENCES,
+    Sort,
+)
 from weaviate.collections.classes.internal import (
     GenerativeReturn,
     CrossReferences,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import INCLUDE_VECTOR
+from weaviate.types import UUID, INCLUDE_VECTOR
 
-class _BM25Generate(Generic[Properties, References], _BaseQuery[Properties, References]):
+class _FetchObjectsGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[Union[Sort, List[Sort]]] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
-        return_references: Literal[None] = None,
+        return_references: Literal[None] = None
     ) -> GenerativeReturn[Properties, References]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
-        *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[Union[Sort, List[Sort]]] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
+        *,
         return_properties: Optional[PROPERTIES] = None,
-        return_references: REFERENCES,
+        return_references: REFERENCES
     ) -> GenerativeReturn[Properties, CrossReferences]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[Union[Sort, List[Sort]]] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
-        return_references: Type[TReferences],
+        return_references: Type[TReferences]
     ) -> GenerativeReturn[Properties, TReferences]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[Union[Sort, List[Sort]]] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
-        return_references: Literal[None] = None,
+        return_references: Literal[None] = None
     ) -> GenerativeReturn[TProperties, References]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[Union[Sort, List[Sort]]] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
-        return_references: REFERENCES,
+        return_references: REFERENCES
     ) -> GenerativeReturn[TProperties, CrossReferences]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[Union[Sort, List[Sort]]] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
-        return_references: Type[TReferences],
+        return_references: Type[TReferences]
     ) -> GenerativeReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/bm25/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/query.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,96 +1,87 @@
-from typing import Generic, List, Optional
+from typing import Generic, Optional
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import Rerank, METADATA
+from weaviate.collections.classes.grpc import METADATA, _Sorting
 from weaviate.collections.classes.internal import (
     QueryReturnType,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import INCLUDE_VECTOR
+from weaviate.types import UUID, INCLUDE_VECTOR
 
 
-class _BM25Query(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def bm25(
+class _FetchObjectsQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def fetch_objects(
         self,
-        query: str,
         *,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[_Sorting] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
-        return_references: Optional[ReturnReferences[TReferences]] = None,
+        return_references: Optional[ReturnReferences[TReferences]] = None
     ) -> QueryReturnType[Properties, References, TProperties, TReferences]:
-        """Search for objects in this collection using the keyword-based BM25 algorithm.
-
-        See the [docs](https://weaviate.io/developers/weaviate/search/bm25) for a more detailed explanation.
+        """Retrieve the objects in this collection without any search.
 
         Arguments:
-            `query`
-                The keyword-based query to search for, REQUIRED.
-            `query_properties`
-                The properties to search in. If not specified, all properties are searched.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
-            `auto_limit`
-                The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
+            `after`
+                The UUID of the object to start from. If not specified, the retrieval begins from the first object in the server.
             `filters`
-                The filters to apply to the search.
-            `rerank`
-                How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+                The filters to apply to the retrieval.
+            `sort`
+                The sorting to apply to the retrieval.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
+            `return_references`
+                The references to return for each object.
 
         NOTE:
-            If `return_properties` is not provided then all non-reference properties are returned including nested properties.
-            If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
-            If `return_references` is not provided then no references are provided.
+            - If `return_properties` is not provided then all properties are returned except for blob properties.
+            - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
+            - If `return_references` is not provided then no references are provided.
 
         Returns:
             A `QueryReturn` object that includes the searched objects.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
                 If the network connection to Weaviate fails.
         """
-        res = self._query.bm25(
-            query=query,
-            properties=query_properties,
+        res = self._query.get(
             limit=limit,
             offset=offset,
-            autocut=auto_limit,
+            after=after,
             filters=filters,
+            sort=sort,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
-            rerank=rerank,
         )
         return self._result_to_query_return(
             res,
             _QueryOptions.from_input(
-                return_metadata=return_metadata,
-                return_properties=return_properties,
-                include_vector=include_vector,
-                collection_references=self._references,
-                query_references=return_references,
-                rerank=rerank,
+                return_metadata,
+                return_properties,
+                include_vector,
+                self._references,
+                return_references,
             ),
             return_properties,
             return_references,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/bm25/query.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/query.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,117 +1,123 @@
-from typing import Generic, List, Literal, Optional, Type, overload
+from typing import Generic, List, Literal, Optional, Union, Type, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import Rerank, METADATA, PROPERTIES, REFERENCES
+from weaviate.collections.classes.grpc import METADATA, PROPERTIES, REFERENCES, _Sort, _Sorting
 from weaviate.collections.classes.internal import (
     QueryReturn,
     CrossReferences,
+    ReturnProperties,
+    ReturnReferences,
+    QueryReturnType,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import INCLUDE_VECTOR
+from weaviate.types import UUID, INCLUDE_VECTOR
 
-class _BM25Query(Generic[Properties, References], _BaseQuery[Properties, References]):
+class _FetchObjectsQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[_Sorting] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
-        return_references: Literal[None] = None,
+        return_references: Literal[None] = None
     ) -> QueryReturn[Properties, References]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[_Sorting] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
-        return_references: REFERENCES,
+        return_references: REFERENCES
     ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[_Sorting] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
-        return_references: Type[TReferences],
+        return_references: Type[TReferences]
     ) -> QueryReturn[Properties, TReferences]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[_Sorting] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
-        return_references: Literal[None] = None,
+        return_references: Literal[None] = None
     ) -> QueryReturn[TProperties, References]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[_Sorting] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
-        return_references: REFERENCES,
+        return_references: REFERENCES
     ) -> QueryReturn[TProperties, CrossReferences]: ...
     @overload
-    def bm25(
+    def fetch_objects(
         self,
-        query: str,
         *,
-        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        auto_limit: Optional[int] = None,
+        after: Optional[UUID] = None,
         filters: Optional[_Filters] = None,
-        rerank: Optional[Rerank] = None,
+        sort: Optional[_Sorting] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
-        return_references: Type[TReferences],
+        return_references: Type[TReferences]
     ) -> QueryReturn[TProperties, TReferences]: ...
+    @overload
+    def fetch_objects(
+        self,
+        *,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        after: Optional[UUID] = None,
+        filters: Optional[_Filters] = None,
+        sort: Optional[_Sorting] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Optional[ReturnProperties[TProperties]] = None,
+        return_references: Optional[ReturnReferences[TReferences]] = None
+    ) -> QueryReturnType[Properties, References, TProperties, TReferences]: ...
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_object_by_id/query.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/generate.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 from typing import Generic, List, Optional
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, _Sorting
+from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
-    GenerativeReturnType,
-    _Generative,
+    _GroupBy,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
+    QuerySearchReturnType,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import UUID, INCLUDE_VECTOR
+from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 
-class _FetchObjectsGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def fetch_objects(
+class _NearVectorQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def near_vector(
         self,
+        near_vector: List[float],
         *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
+        certainty: Optional[NUMBER] = None,
+        distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        after: Optional[UUID] = None,
+        auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
-        sort: Optional[_Sorting] = None,
+        group_by: Optional[GroupBy] = None,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
-        return_references: Optional[ReturnReferences[TReferences]] = None
-    ) -> GenerativeReturnType[Properties, References, TProperties, TReferences]:
-        """Perform retrieval-augmented generation (RaG) on the results of a simple get query of objects in this collection.
+        return_references: Optional[ReturnReferences[TReferences]] = None,
+    ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
+        """Search for objects by vector in this collection using and vector-based similarity search.
+
+        See the [docs](https://weaviate.io/developers/weaviate/search/similarity) for a more detailed explanation.
 
         Arguments:
-            `single_prompt`
-                The prompt to use for RaG on each object individually.
-            `grouped_task`
-                The prompt to use for RaG on the entire result set.
-            `grouped_properties`
-                The properties to use in the RaG on the entire result set.
+            `near_vector`
+                The vector to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
+            `certainty`
+                The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
+            `distance`
+                The maximum distance to search. If not specified, the default distance specified by the server is used.
             `limit`
-                The maximum number of results to return. If not specified, the default limit specified by Weaviate is returned.
+                The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
-                The offset to start from. If not specified, the retrieval begins from the first object in Weaviate.
-            `after`
-                The UUID of the object to start from. If not specified, the retrieval begins from the first object in Weaviate.
+                The offset to start from. If not specified, the retrieval begins from the first object in the server.
+            `auto_limit`
+                The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
-                The filters to apply to the retrieval.
-            `sort`
-                The sorting to apply to the retrieval.
+                The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
+            `rerank`
+                How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -63,40 +71,43 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `_GenerativeNearMediaReturn` object that includes the searched objects with per-object generated results and group generated results.
+            A `QueryReturn` or `GroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GroupByReturn` object is returned, otherwise a `QueryReturn` object is returned.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
-                If the network connection to Weaviate fails.
+                If the request to the Weaviate server fails.
         """
-        res = self._query.get(
+        res = self._query.near_vector(
+            near_vector=near_vector,
+            certainty=certainty,
+            distance=distance,
             limit=limit,
             offset=offset,
-            after=after,
+            autocut=auto_limit,
             filters=filters,
-            sort=sort,
+            group_by=_GroupBy.from_input(group_by),
+            rerank=rerank,
+            target_vector=target_vector,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
-            generative=_Generative(
-                single=single_prompt,
-                grouped=grouped_task,
-                grouped_properties=grouped_properties,
-            ),
         )
-        return self._result_to_generative_query_return(
+        return self._result_to_query_or_groupby_return(
             res,
             _QueryOptions.from_input(
                 return_metadata,
                 return_properties,
                 include_vector,
                 self._references,
                 return_references,
+                rerank,
+                group_by,
             ),
             return_properties,
             return_references,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/fetch_objects/generate.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/query.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,128 +1,125 @@
-from typing import Generic, List, Literal, Optional, Union, Type, overload
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import (
     METADATA,
-    PROPERTIES,
-    REFERENCES,
-    Sort,
+    GroupBy,
+    Move,
+    Rerank,
 )
 from weaviate.collections.classes.internal import (
-    GenerativeReturn,
-    CrossReferences,
+    _GroupBy,
+    ReturnProperties,
+    ReturnReferences,
+    _QueryOptions,
+    QuerySearchReturnType,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import UUID, INCLUDE_VECTOR
+from weaviate.types import NUMBER, INCLUDE_VECTOR
 
-class _FetchObjectsGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
-    @overload
-    def fetch_objects(
-        self,
-        *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        after: Optional[UUID] = None,
-        filters: Optional[_Filters] = None,
-        sort: Optional[Union[Sort, List[Sort]]] = None,
-        target_vector: Optional[str] = None,
-        include_vector: INCLUDE_VECTOR = False,
-        return_metadata: Optional[METADATA] = None,
-        return_properties: Optional[PROPERTIES] = None,
-        return_references: Literal[None] = None
-    ) -> GenerativeReturn[Properties, References]: ...
-    @overload
-    def fetch_objects(
-        self,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        after: Optional[UUID] = None,
-        filters: Optional[_Filters] = None,
-        sort: Optional[Union[Sort, List[Sort]]] = None,
-        target_vector: Optional[str] = None,
-        include_vector: INCLUDE_VECTOR = False,
-        return_metadata: Optional[METADATA] = None,
-        *,
-        return_properties: Optional[PROPERTIES] = None,
-        return_references: REFERENCES
-    ) -> GenerativeReturn[Properties, CrossReferences]: ...
-    @overload
-    def fetch_objects(
-        self,
-        *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        after: Optional[UUID] = None,
-        filters: Optional[_Filters] = None,
-        sort: Optional[Union[Sort, List[Sort]]] = None,
-        target_vector: Optional[str] = None,
-        include_vector: INCLUDE_VECTOR = False,
-        return_metadata: Optional[METADATA] = None,
-        return_properties: Optional[PROPERTIES] = None,
-        return_references: Type[TReferences]
-    ) -> GenerativeReturn[Properties, TReferences]: ...
-    @overload
-    def fetch_objects(
-        self,
-        *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        after: Optional[UUID] = None,
-        filters: Optional[_Filters] = None,
-        sort: Optional[Union[Sort, List[Sort]]] = None,
-        target_vector: Optional[str] = None,
-        include_vector: INCLUDE_VECTOR = False,
-        return_metadata: Optional[METADATA] = None,
-        return_properties: Type[TProperties],
-        return_references: Literal[None] = None
-    ) -> GenerativeReturn[TProperties, References]: ...
-    @overload
-    def fetch_objects(
-        self,
-        *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        after: Optional[UUID] = None,
-        filters: Optional[_Filters] = None,
-        sort: Optional[Union[Sort, List[Sort]]] = None,
-        target_vector: Optional[str] = None,
-        include_vector: INCLUDE_VECTOR = False,
-        return_metadata: Optional[METADATA] = None,
-        return_properties: Type[TProperties],
-        return_references: REFERENCES
-    ) -> GenerativeReturn[TProperties, CrossReferences]: ...
-    @overload
-    def fetch_objects(
+
+class _NearTextQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def near_text(
         self,
+        query: Union[List[str], str],
         *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
+        certainty: Optional[NUMBER] = None,
+        distance: Optional[NUMBER] = None,
+        move_to: Optional[Move] = None,
+        move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
-        after: Optional[UUID] = None,
+        auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
-        sort: Optional[Union[Sort, List[Sort]]] = None,
+        group_by: Optional[GroupBy] = None,
+        rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
-        return_properties: Type[TProperties],
-        return_references: Type[TReferences]
-    ) -> GenerativeReturn[TProperties, TReferences]: ...
+        return_properties: Optional[ReturnProperties[TProperties]] = None,
+        return_references: Optional[ReturnReferences[TReferences]] = None,
+    ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
+        """Search for objects in this collection by text using text-capable vectorization module and vector-based similarity search.
+
+        See the [docs](https://weaviate.io/developers/weaviate/api/graphql/search-operators#neartext) for a more detailed explanation.
+
+        NOTE:
+            You must have a text-capable vectorization module installed in order to use this method, e.g. any of the `text2vec-` and `multi2vec-` modules.
+
+        Arguments:
+            `query`
+                The text or texts to search on, REQUIRED.
+            `certainty`
+                The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
+            `distance`
+                The maximum distance to search. If not specified, the default distance specified by the server is used.
+            `limit`
+                The maximum number of results to return. If not specified, the default limit specified by the server is returned.
+            `offset`
+                The offset to start from. If not specified, the retrieval begins from the first object in the server.
+            `auto_limit`
+                The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
+            `filters`
+                The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
+            `rerank`
+                How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
+            `include_vector`
+                Whether to include the vector in the results. If not specified, this is set to False.
+            `return_metadata`
+                The metadata to return for each object, defaults to `None`.
+            `return_properties`
+                The properties to return for each object.
+            `return_references`
+                The references to return for each object.
+
+        NOTE:
+            If `return_properties` is not provided then all properties are returned except for any cross reference properties.
+            If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
+            If `return_references` is not provided then no references are provided.
+
+        Returns:
+            A `QueryReturn` or `GroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GroupByReturn` object is returned, otherwise a `QueryReturn` object is returned.
+
+        Raises:
+            `weaviate.exceptions.WeaviateGRPCQueryError`:
+                If the request to the Weaviate server fails.
+        """
+        res = self._query.near_text(
+            near_text=query,
+            certainty=certainty,
+            distance=distance,
+            move_to=move_to,
+            move_away=move_away,
+            limit=limit,
+            offset=offset,
+            autocut=auto_limit,
+            filters=filters,
+            target_vector=target_vector,
+            group_by=_GroupBy.from_input(group_by),
+            rerank=rerank,
+            return_metadata=self._parse_return_metadata(return_metadata, include_vector),
+            return_properties=self._parse_return_properties(return_properties),
+            return_references=self._parse_return_references(return_references),
+        )
+        return self._result_to_query_or_groupby_return(
+            res,
+            _QueryOptions.from_input(
+                return_metadata,
+                return_properties,
+                include_vector,
+                self._references,
+                return_references,
+                rerank,
+                group_by,
+            ),
+            return_properties,
+            return_references,
+        )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/generate.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,127 +1,110 @@
 from typing import Generic, List, Optional
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, HybridFusion, Rerank
+from weaviate.collections.classes.grpc import GroupBy, Rerank, METADATA
 from weaviate.collections.classes.internal import (
-    GenerativeReturnType,
-    _Generative,
+    QuerySearchReturnType,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
+    _GroupBy,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import NUMBER, INCLUDE_VECTOR
+from weaviate.exceptions import WeaviateUnsupportedFeatureError
+from weaviate.types import INCLUDE_VECTOR
 
 
-class _HybridGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def hybrid(
+class _BM25Query(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def bm25(
         self,
         query: Optional[str],
         *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        alpha: NUMBER = 0.5,
-        vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
-        fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> GenerativeReturnType[Properties, References, TProperties, TReferences]:
-        """Perform retrieval-augmented generation (RaG) on the results of an object search in this collection using the hybrid algorithm blending keyword-based BM25 and vector-based similarity.
+    ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
+        """Search for objects in this collection using the keyword-based BM25 algorithm.
 
-        See the [docs](https://weaviate.io/developers/weaviate/search/hybrid) for a more detailed explanation.
+        See the [docs](https://weaviate.io/developers/weaviate/search/bm25) for a more detailed explanation.
 
         Arguments:
             `query`
-                The keyword-based query to search for, REQUIRED.
-            `single_prompt`
-                The prompt to use for RaG on each object individually.
-            `grouped_task`
-                The prompt to use for RaG on the entire result set.
-            `grouped_properties`
-                The properties to use in the RaG on the entire result set.
-            `alpha`
-                The weight of the BM25 score. If not specified, the default weight specified by the server is used.
-            `vector`
-                The specific vector to search for. If not specified, the query is vectorized and used in the similarity search.
+                The keyword-based query to search for, REQUIRED. If None, a normal search will be performed.
             `query_properties`
                 The properties to search in. If not specified, all properties are searched.
-            `fusion_type`
-                The type of fusion to apply. If not specified, the default fusion type specified by the server is used.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
-            `return_references`
-                The references to return for each object.
 
         NOTE:
-            - If `return_properties` is not provided then all properties are returned except for blob properties.
-            - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
-            - If `return_references` is not provided then no references are provided.
+            If `return_properties` is not provided then all non-reference properties are returned including nested properties.
+            If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
+            If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `_GenerativeNearMediaReturn` object that includes the searched objects with per-object generated results and group generated results.
+            A `QueryReturn` or `GroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GroupByReturn` object is returned, otherwise a `QueryReturn` object is returned.
 
         Raises:
-            `weaviate.exceptions.WeaviateGRPCQueryError`:
+            `weaviate.exceptions.WeaviateQueryError`:
                 If the network connection to Weaviate fails.
+            `weaviate.exceptions.WeaviateNotImplementedError`:
+                If a group by is provided and the Weaviate server version is lower than 1.25.0.
         """
-        res = self._query.hybrid(
-            query=query or "",
-            alpha=alpha,
-            vector=vector,
+        if group_by is not None and not self._connection.supports_groupby_in_bm25_and_hybrid():
+            raise WeaviateUnsupportedFeatureError(
+                "BM25 group by", self._connection.server_version, "1.25.0"
+            )
+        res = self._query.bm25(
+            query=query,
             properties=query_properties,
-            fusion_type=fusion_type,
             limit=limit,
             offset=offset,
             autocut=auto_limit,
             filters=filters,
-            rerank=rerank,
-            target_vector=target_vector,
+            group_by=_GroupBy.from_input(group_by),
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
-            generative=_Generative(
-                single=single_prompt,
-                grouped=grouped_task,
-                grouped_properties=grouped_properties,
-            ),
+            rerank=rerank,
         )
-        return self._result_to_generative_query_return(
+        return self._result_to_query_or_groupby_return(
             res,
             _QueryOptions.from_input(
-                return_metadata,
-                return_properties,
-                include_vector,
-                self._references,
-                return_references,
-                rerank,
+                return_metadata=return_metadata,
+                return_properties=return_properties,
+                include_vector=include_vector,
+                collection_references=self._references,
+                query_references=return_references,
+                rerank=rerank,
+                group_by=group_by,
             ),
             return_properties,
             return_references,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/generate.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/query.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,153 +1,235 @@
 from typing import Generic, List, Literal, Optional, Type, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, PROPERTIES, REFERENCES, HybridFusion, Rerank
+from weaviate.collections.classes.grpc import GroupBy, Rerank, METADATA, PROPERTIES, REFERENCES
 from weaviate.collections.classes.internal import (
-    GenerativeReturn,
+    GroupByReturn,
+    QueryReturn,
     CrossReferences,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import NUMBER, INCLUDE_VECTOR
+from weaviate.types import INCLUDE_VECTOR
 
-class _HybridGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
+class _BM25Query(Generic[Properties, References], _BaseQuery[Properties, References]):
     @overload
-    def hybrid(
+    def bm25(
         self,
         query: Optional[str],
         *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        alpha: NUMBER = 0.5,
-        vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
-        fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
-    ) -> GenerativeReturn[Properties, References]: ...
+    ) -> QueryReturn[Properties, References]: ...
     @overload
-    def hybrid(
+    def bm25(
         self,
         query: Optional[str],
         *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        alpha: NUMBER = 0.5,
-        vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
-        fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
-    ) -> GenerativeReturn[Properties, CrossReferences]: ...
+    ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
-    def hybrid(
+    def bm25(
         self,
         query: Optional[str],
         *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        alpha: NUMBER = 0.5,
-        vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
-        fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
-    ) -> GenerativeReturn[Properties, TReferences]: ...
+    ) -> QueryReturn[Properties, TReferences]: ...
     @overload
-    def hybrid(
+    def bm25(
         self,
         query: Optional[str],
         *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        alpha: NUMBER = 0.5,
-        vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
-        fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
-    ) -> GenerativeReturn[TProperties, References]: ...
+    ) -> QueryReturn[TProperties, References]: ...
     @overload
-    def hybrid(
+    def bm25(
         self,
         query: Optional[str],
         *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        alpha: NUMBER = 0.5,
-        vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
-        fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
-    ) -> GenerativeReturn[TProperties, CrossReferences]: ...
+    ) -> QueryReturn[TProperties, CrossReferences]: ...
     @overload
-    def hybrid(
+    def bm25(
         self,
         query: Optional[str],
         *,
-        single_prompt: Optional[str] = None,
-        grouped_task: Optional[str] = None,
-        grouped_properties: Optional[List[str]] = None,
-        alpha: NUMBER = 0.5,
-        vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
-        fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
-    ) -> GenerativeReturn[TProperties, TReferences]: ...
+    ) -> QueryReturn[TProperties, TReferences]: ...
+
+    ###### GROUP BY ######
+
+    @overload
+    def bm25(
+        self,
+        query: Optional[str],
+        *,
+        query_properties: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: GroupBy,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Optional[PROPERTIES] = None,
+        return_references: Literal[None] = None,
+    ) -> GroupByReturn[Properties, References]: ...
+    @overload
+    def bm25(
+        self,
+        query: Optional[str],
+        *,
+        query_properties: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: GroupBy,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Optional[PROPERTIES] = None,
+        return_references: REFERENCES,
+    ) -> GroupByReturn[Properties, CrossReferences]: ...
+    @overload
+    def bm25(
+        self,
+        query: Optional[str],
+        *,
+        query_properties: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: GroupBy,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Optional[PROPERTIES] = None,
+        return_references: Type[TReferences],
+    ) -> GroupByReturn[Properties, TReferences]: ...
+    @overload
+    def bm25(
+        self,
+        query: Optional[str],
+        *,
+        query_properties: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: GroupBy,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Type[TProperties],
+        return_references: Literal[None] = None,
+    ) -> GroupByReturn[TProperties, References]: ...
+    @overload
+    def bm25(
+        self,
+        query: Optional[str],
+        *,
+        query_properties: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: GroupBy,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Type[TProperties],
+        return_references: REFERENCES,
+    ) -> GroupByReturn[TProperties, CrossReferences]: ...
+    @overload
+    def bm25(
+        self,
+        query: Optional[str],
+        *,
+        query_properties: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: GroupBy,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Type[TProperties],
+        return_references: Type[TReferences],
+    ) -> GroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from typing import Generic, List, Optional
+from typing import Generic, Optional
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, HybridFusion, Rerank
+from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
-    QueryReturnType,
+    _GroupBy,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
+    QuerySearchReturnType,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import NUMBER, INCLUDE_VECTOR
+from weaviate.types import NUMBER, INCLUDE_VECTOR, UUID
 
 
-class _HybridQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def hybrid(
+class _NearObjectQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def near_object(
         self,
-        query: Optional[str],
+        near_object: UUID,
         *,
-        alpha: NUMBER = 0.5,
-        vector: Optional[List[float]] = None,
-        query_properties: Optional[List[str]] = None,
-        fusion_type: Optional[HybridFusion] = None,
+        certainty: Optional[NUMBER] = None,
+        distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> QueryReturnType[Properties, References, TProperties, TReferences]:
-        """Search for objects in this collection using the hybrid algorithm blending keyword-based BM25 and vector-based similarity.
+    ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
+        """Search for objects in this collection by another object using a vector-based similarity search.
 
-        See the [docs](https://weaviate.io/developers/weaviate/search/hybrid) for a more detailed explanation.
+        See the [docs](https://weaviate.io/developers/weaviate/api/graphql/search-operators#nearobject) for a more detailed explanation.
 
         Arguments:
-            `query`
-                The keyword-based query to search for, REQUIRED.
-            `alpha`
-                The weight of the BM25 score. If not specified, the default weight specified by the server is used.
-            `vector`
-                The specific vector to search for. If not specified, the query is vectorized and used in the similarity search.
-            `query_properties`
-                The properties to search in. If not specified, all properties are searched.
-            `fusion_type`
-                The type of fusion to apply. If not specified, the default fusion type specified by the server is used.
+            `near_object`
+                The UUID of the object to search on, REQUIRED.
+            `certainty`
+                The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
+            `distance`
+                The maximum distance to search. If not specified, the default distance specified by the server is used.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -71,42 +71,43 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `QueryReturn` object that includes the searched objects.
+            A `QueryReturn` or `GroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GroupByReturn` object is returned, otherwise a `QueryReturn` object is returned.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
-                If the network connection to Weaviate fails.
+                If the request to the Weaviate server fails.
         """
-        res = self._query.hybrid(
-            query=query or "",
-            alpha=alpha,
-            vector=vector,
-            properties=query_properties,
-            fusion_type=fusion_type,
+        res = self._query.near_object(
+            near_object=near_object,
+            certainty=certainty,
+            distance=distance,
             limit=limit,
             offset=offset,
             autocut=auto_limit,
             filters=filters,
+            group_by=_GroupBy.from_input(group_by),
             rerank=rerank,
             target_vector=target_vector,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
         )
-        return self._result_to_query_return(
+        return self._result_to_query_or_groupby_return(
             res,
             _QueryOptions.from_input(
                 return_metadata,
                 return_properties,
                 include_vector,
                 self._references,
                 return_references,
                 rerank,
+                group_by,
             ),
             return_properties,
             return_references,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/hybrid/query.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/query.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,279 @@
 from typing import Generic, List, Literal, Optional, Type, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, PROPERTIES, REFERENCES, HybridFusion, Rerank
+from weaviate.collections.classes.grpc import (
+    METADATA,
+    PROPERTIES,
+    REFERENCES,
+    HybridFusion,
+    HybridVectorType,
+    GroupBy,
+    Rerank,
+)
 from weaviate.collections.classes.internal import (
+    GroupByReturn,
     QueryReturn,
     CrossReferences,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 class _HybridQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
     @overload
     def hybrid(
         self,
         query: Optional[str],
         *,
+        alpha: NUMBER = 0.7,
+        vector: Optional[HybridVectorType] = None,
+        query_properties: Optional[List[str]] = None,
+        fusion_type: Optional[HybridFusion] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Optional[PROPERTIES] = None,
+        return_references: Literal[None] = None,
+    ) -> QueryReturn[Properties, References]: ...
+    @overload
+    def hybrid(
+        self,
+        query: Optional[str],
+        *,
+        alpha: NUMBER = 0.7,
+        vector: Optional[HybridVectorType] = None,
+        query_properties: Optional[List[str]] = None,
+        fusion_type: Optional[HybridFusion] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Optional[PROPERTIES] = None,
+        return_references: REFERENCES,
+    ) -> QueryReturn[Properties, CrossReferences]: ...
+    @overload
+    def hybrid(
+        self,
+        query: Optional[str],
+        *,
+        alpha: NUMBER = 0.7,
+        vector: Optional[HybridVectorType] = None,
+        query_properties: Optional[List[str]] = None,
+        fusion_type: Optional[HybridFusion] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Optional[PROPERTIES] = None,
+        return_references: Type[TReferences],
+    ) -> QueryReturn[Properties, TReferences]: ...
+    @overload
+    def hybrid(
+        self,
+        query: Optional[str],
+        *,
+        alpha: NUMBER = 0.7,
+        vector: Optional[HybridVectorType] = None,
+        query_properties: Optional[List[str]] = None,
+        fusion_type: Optional[HybridFusion] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Type[TProperties],
+        return_references: Literal[None] = None,
+    ) -> QueryReturn[TProperties, References]: ...
+    @overload
+    def hybrid(
+        self,
+        query: Optional[str],
+        *,
+        alpha: NUMBER = 0.7,
+        vector: Optional[HybridVectorType] = None,
+        query_properties: Optional[List[str]] = None,
+        fusion_type: Optional[HybridFusion] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Type[TProperties],
+        return_references: REFERENCES,
+    ) -> QueryReturn[TProperties, CrossReferences]: ...
+    @overload
+    def hybrid(
+        self,
+        query: Optional[str],
+        *,
+        alpha: NUMBER = 0.7,
+        vector: Optional[HybridVectorType] = None,
+        query_properties: Optional[List[str]] = None,
+        fusion_type: Optional[HybridFusion] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        auto_limit: Optional[int] = None,
+        filters: Optional[_Filters] = None,
+        group_by: Literal[None] = None,
+        rerank: Optional[Rerank] = None,
+        target_vector: Optional[str] = None,
+        include_vector: INCLUDE_VECTOR = False,
+        return_metadata: Optional[METADATA] = None,
+        return_properties: Type[TProperties],
+        return_references: Type[TReferences],
+    ) -> QueryReturn[TProperties, TReferences]: ...
+
+    ##### GROUP BY #####
+
+    @overload
+    def hybrid(
+        self,
+        query: Optional[str],
+        *,
         alpha: NUMBER = 0.5,
         vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: GroupBy,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
-    ) -> QueryReturn[Properties, References]: ...
+    ) -> GroupByReturn[Properties, References]: ...
     @overload
     def hybrid(
         self,
         query: Optional[str],
         *,
         alpha: NUMBER = 0.5,
         vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: GroupBy,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
-    ) -> QueryReturn[Properties, CrossReferences]: ...
+    ) -> GroupByReturn[Properties, CrossReferences]: ...
     @overload
     def hybrid(
         self,
         query: Optional[str],
         *,
         alpha: NUMBER = 0.5,
         vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: GroupBy,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
-    ) -> QueryReturn[Properties, TReferences]: ...
+    ) -> GroupByReturn[Properties, TReferences]: ...
     @overload
     def hybrid(
         self,
         query: Optional[str],
         *,
         alpha: NUMBER = 0.5,
         vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: GroupBy,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
-    ) -> QueryReturn[TProperties, References]: ...
+    ) -> GroupByReturn[TProperties, References]: ...
     @overload
     def hybrid(
         self,
         query: Optional[str],
         *,
         alpha: NUMBER = 0.5,
         vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: GroupBy,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
-    ) -> QueryReturn[TProperties, CrossReferences]: ...
+    ) -> GroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def hybrid(
         self,
         query: Optional[str],
         *,
         alpha: NUMBER = 0.5,
         vector: Optional[List[float]] = None,
         query_properties: Optional[List[str]] = None,
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
+        group_by: GroupBy,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
-    ) -> QueryReturn[TProperties, TReferences]: ...
+    ) -> GroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_image/generate.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,83 @@
-from io import BufferedReader
-from pathlib import Path
 from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
+from weaviate.collections.classes.grpc import (
+    METADATA,
+    GroupBy,
+    Move,
+    Rerank,
+)
 from weaviate.collections.classes.internal import (
     _Generative,
     _GroupBy,
-    GenerativeNearMediaReturnType,
+    GenerativeSearchReturnType,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 
-class _NearImageGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def near_image(
+class _NearTextGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def near_text(
         self,
-        near_image: Union[str, Path, BufferedReader],
+        query: Union[List[str], str],
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
+        move_to: Optional[Move] = None,
+        move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> GenerativeNearMediaReturnType[Properties, References, TProperties, TReferences]:
-        """Perform retrieval-augmented generation (RaG) on the results of a by-image object search in this collection using an image-capable vectorization module and vector-based similarity search.
+    ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
+        """Perform retrieval-augmented generation (RaG) on the results of a by-image object search in this collection using the image-capable vectorization module and vector-based similarity search.
 
-        See the [docs](https://weaviate.io/developers/weaviate/search/image) for a more detailed explanation.
+        See the [docs](https://weaviate.io/developers/weaviate/api/graphql/search-operators#neartext) for a more detailed explanation.
 
         NOTE:
-            You must have an image-capable vectorization module installed in order to use this method, e.g. `img2vec-neural`, `multi2vec-clip`, or `multi2vec-bind.
+            You must have a text-capable vectorization module installed in order to use this method, e.g. any of the `text2vec-` and `multi2vec-` modules.
 
         Arguments:
-            `near_image`
-                The image file to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
+            `query`
+                The text or texts to search on, REQUIRED.
             `certainty`
                 The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
             `distance`
                 The maximum distance to search. If not specified, the default distance specified by the server is used.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -76,37 +85,39 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `_GenerativeNearMediaReturn` object that includes the searched objects with per-object generated results and group generated results.
+            A `GenerativeReturn` or `GenerativeGroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GenerativeGroupByReturn` object is returned, otherwise a `GenerativeReturn` object is returned.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
                 If the request to the Weaviate server fails.
         """
-        res = self._query.near_media(
-            media=self._parse_media(near_image),
-            type_="image",
+        res = self._query.near_text(
+            near_text=query,
             certainty=certainty,
             distance=distance,
+            move_to=move_to,
+            move_away=move_away,
+            limit=limit,
+            offset=offset,
+            autocut=auto_limit,
             filters=filters,
             group_by=_GroupBy.from_input(group_by),
             rerank=rerank,
             target_vector=target_vector,
             generative=_Generative(
                 single=single_prompt,
                 grouped=grouped_task,
                 grouped_properties=grouped_properties,
             ),
-            limit=limit,
-            offset=offset,
-            autocut=auto_limit,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
         )
         return self._result_to_generative_return(
             res,
             _QueryOptions.from_input(
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_image/generate.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_image/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     _GroupBy,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
-    QueryNearMediaReturnType,
+    QuerySearchReturnType,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 
 class _NearImageQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
@@ -32,15 +32,15 @@
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> QueryNearMediaReturnType[Properties, References, TProperties, TReferences]:
+    ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
         """Search for objects by image in this collection using an image-capable vectorization module and vector-based similarity search.
 
         See the [docs](https://weaviate.io/developers/weaviate/search/image) for a more detailed explanation.
 
         NOTE:
             You must have an image-capable vectorization module installed in order to use this method, e.g. `img2vec-neural`, `multi2vec-clip`, or `multi2vec-bind.
 
@@ -55,16 +55,20 @@
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -72,18 +76,19 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `QueryReturn` object that includes the searched objects.
+            A `QueryReturn` or `GroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GroupByReturn` object is returned, otherwise a `QueryReturn` object is returned.
 
         Raises:
-            `weaviate.exceptions.WeaviateGRPCQueryError`:
+            `weaviate.exceptions.WeaviateQueryError`:
                 If the request to the Weaviate server fails.
         """
         res = self._query.near_media(
             media=self._parse_media(near_image),
             type_="image",
             certainty=certainty,
             distance=distance,
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_image/query.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_media/generate.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from io import BufferedReader
-from pathlib import Path
-from typing import Generic, List, Optional, Union
+from typing import Generic, List, Optional
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank, NearMediaType
+from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     _Generative,
+    GenerativeSearchReturnType,
     _GroupBy,
-    GenerativeNearMediaReturnType,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 
-class _NearMediaGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def near_media(
+class _NearVectorGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
@@ -37,41 +34,40 @@
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> GenerativeNearMediaReturnType[Properties, References, TProperties, TReferences]:
-        """Perform retrieval-augmented generation (RaG) on the results of a by-audio object search in this collection using an audio-capable vectorization module and vector-based similarity search.
+    ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
+        """Perform retrieval-augmented generation (RaG) on the results of a by-vector object search in this collection using vector-based similarity search.
 
-        See the [docs](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/multi2vec-bind) for a more detailed explanation.
-
-        NOTE:
-            You must have a multi-media-capable vectorization module installed in order to use this method, e.g. `multi2vec-bind`.
+        See the [docs](https://weaviate.io/developers/weaviate/search/similarity) for a more detailed explanation.
 
         Arguments:
-            `near_media`
-                The media file to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
-            `media_type`
-                The type of the provided media file, REQUIRED.
+            `near_vector`
+                The vector to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
             `certainty`
                 The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
             `distance`
                 The maximum distance to search. If not specified, the default distance specified by the server is used.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -79,37 +75,37 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `_GenerativeNearMediaReturn` object that includes the searched objects with per-object generated results and group generated results.
+            A `GenerativeReturn` or `GenerativeGroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GenerativeGroupByReturn` object is returned, otherwise a `GenerativeReturn` object is returned.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
                 If the request to the Weaviate server fails.
         """
-        res = self._query.near_media(
-            media=self._parse_media(media),
-            type_=media_type.value,
+        res = self._query.near_vector(
+            near_vector=near_vector,
             certainty=certainty,
             distance=distance,
             filters=filters,
             group_by=_GroupBy.from_input(group_by),
-            rerank=rerank,
-            target_vector=target_vector,
             generative=_Generative(
                 single=single_prompt,
                 grouped=grouped_task,
                 grouped_properties=grouped_properties,
             ),
             limit=limit,
             offset=offset,
             autocut=auto_limit,
+            rerank=rerank,
+            target_vector=target_vector,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
         )
         return self._result_to_generative_return(
             res,
             _QueryOptions.from_input(
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_media/generate.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_media/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/generate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,117 +1,128 @@
-from io import BufferedReader
-from pathlib import Path
-from typing import Generic, Optional, Union
+from typing import Generic, List, Optional
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import GroupBy, METADATA, NearMediaType, Rerank
+from weaviate.collections.classes.grpc import GroupBy, Rerank, METADATA
 from weaviate.collections.classes.internal import (
-    _GroupBy,
+    GenerativeSearchReturnType,
+    _Generative,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
-    QueryNearMediaReturnType,
+    _GroupBy,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import NUMBER, INCLUDE_VECTOR
+from weaviate.exceptions import WeaviateUnsupportedFeatureError
+
+from weaviate.types import INCLUDE_VECTOR
 
 
-class _NearMediaQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def near_media(
+class _BM25Generate(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def bm25(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        query: Optional[str],
         *,
-        certainty: Optional[NUMBER] = None,
-        distance: Optional[NUMBER] = None,
+        single_prompt: Optional[str] = None,
+        grouped_task: Optional[str] = None,
+        grouped_properties: Optional[List[str]] = None,
+        query_properties: Optional[List[str]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> QueryNearMediaReturnType[Properties, References, TProperties, TReferences]:
-        """Search for objects by audio in this collection using an audio-capable vectorization module and vector-based similarity search.
+    ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
+        """Perform retrieval-augmented generation (RaG) on the results of a keyword-based BM25 search of objects in this collection.
 
-        See the [docs](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/multi2vec-bind) for a more detailed explanation.
-
-        NOTE:
-            You must have a multi-media-capable vectorization module installed in order to use this method, e.g. `multi2vec-bind`.
+        See the [docs](https://weaviate.io/developers/weaviate/search/bm25) for a more detailed explanation.
 
         Arguments:
-            `media`
-                The media file to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
-            `media_type`
-                The type of the provided media file, REQUIRED.
-            `certainty`
-                The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
-            `distance`
-                The maximum distance to search. If not specified, the default distance specified by the server is used.
+            `query`
+                The keyword-based query to search for, REQUIRED. If None, a normal search will be performed.
+            `single_prompt`
+                The prompt to use for RaG on each object individually.
+            `grouped_task`
+                The prompt to use for RaG on the entire result set.
+            `grouped_properties`
+                The properties to use in the RaG on the entire result set.
+            `query_properties`
+                The properties to search in. If not specified, all properties are searched.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
                 The references to return for each object.
 
         NOTE:
-            - If `return_properties` is not provided then all properties are returned except for blob properties.
-            - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
-            - If `return_references` is not provided then no references are provided.
+            If `return_properties` is not provided then all non-reference properties are returned including nested properties.
+            If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
+            If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `QueryReturn` or `_GroupByReturn` object that includes the searched objects.
-            If `group_by` is provided then a `_GroupByReturn` object is returned, otherwise a `QueryReturn` object is returned.
+            A `GenerativeReturn` or `GenerativeGroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GenerativeGroupByReturn` object is returned, otherwise a `GenerativeReturn` object is returned.
 
         Raises:
-            `weaviate.exceptions.WeaviateGRPCQueryError`:
-                If the request to the Weaviate server fails.
+            `weaviate.exceptions.WeaviateQueryError`:
+                If the network connection to Weaviate fails.
+            `weaviate.exceptions.WeaviateUnsupportedFeatureError`:
+                If a group by is provided and the Weaviate server version is lower than 1.25.0.
         """
-        res = self._query.near_media(
-            media=self._parse_media(media),
-            type_=media_type.value,
-            certainty=certainty,
-            distance=distance,
+        if group_by is not None and not self._connection.supports_groupby_in_bm25_and_hybrid():
+            raise WeaviateUnsupportedFeatureError(
+                "BM25 group by", self._connection.server_version, "1.25.0"
+            )
+        res = self._query.bm25(
+            query=query,
+            properties=query_properties,
             limit=limit,
             offset=offset,
             autocut=auto_limit,
             filters=filters,
             group_by=_GroupBy.from_input(group_by),
             rerank=rerank,
-            target_vector=target_vector,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
+            generative=_Generative(
+                single=single_prompt,
+                grouped=grouped_task,
+                grouped_properties=grouped_properties,
+            ),
         )
-        return self._result_to_query_or_groupby_return(
+        return self._result_to_generative_return(
             res,
             _QueryOptions.from_input(
-                return_metadata,
-                return_properties,
-                include_vector,
-                self._references,
-                return_references,
-                rerank,
+                return_metadata=return_metadata,
+                return_properties=return_properties,
+                include_vector=include_vector,
+                collection_references=self._references,
+                query_references=return_references,
+                rerank=rerank,
+                group_by=group_by,
             ),
             return_properties,
             return_references,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_media/query.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_object/generate.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     _Generative,
     _GroupBy,
-    GenerativeNearMediaReturnType,
+    GenerativeSearchReturnType,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR, UUID
@@ -34,15 +34,15 @@
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> GenerativeNearMediaReturnType[Properties, References, TProperties, TReferences]:
+    ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
         """Perform retrieval-augmented generation (RaG) on the results of a by-object object search in this collection using a vector-based similarity search.
 
         See the [docs](https://weaviate.io/developers/weaviate/api/graphql/search-operators#nearobject) for a more detailed explanation.
 
         Arguments:
             `near_object`
                 The UUID of the object to search on, REQUIRED.
@@ -54,16 +54,20 @@
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -71,15 +75,16 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `_GenerativeNearMediaReturn` object that includes the searched objects with per-object generated results and group generated results.
+            A `GenerativeReturn` or `GenerativeGroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GenerativeGroupByReturn` object is returned, otherwise a `GenerativeReturn` object is returned.
 
         Raises:
             `weaviate.exceptions.WeaviateGRPCQueryError`:
                 If the request to the Weaviate server fails.
         """
         res = self._query.near_object(
             near_object=near_object,
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_object/generate.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_object/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,83 @@
-from typing import Generic, Optional
+from typing import Generic, List, Optional
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
+
+from weaviate.collections.classes.grpc import (
+    METADATA,
+    GroupBy,
+    HybridFusion,
+    Rerank,
+    HybridVectorType,
+)
 from weaviate.collections.classes.internal import (
-    _GroupBy,
+    QuerySearchReturnType,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
-    QueryNearMediaReturnType,
+    _GroupBy,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
-from weaviate.types import NUMBER, INCLUDE_VECTOR, UUID
+from weaviate.exceptions import WeaviateUnsupportedFeatureError
+from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 
-class _NearObjectQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def near_object(
+class _HybridQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def hybrid(
         self,
-        near_object: UUID,
+        query: Optional[str],
         *,
-        certainty: Optional[NUMBER] = None,
-        distance: Optional[NUMBER] = None,
+        alpha: NUMBER = 0.7,
+        vector: Optional[HybridVectorType] = None,
+        query_properties: Optional[List[str]] = None,
+        fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> QueryNearMediaReturnType[Properties, References, TProperties, TReferences]:
-        """Search for objects in this collection by another object using a vector-based similarity search.
+    ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
+        """Search for objects in this collection using the hybrid algorithm blending keyword-based BM25 and vector-based similarity.
 
-        See the [docs](https://weaviate.io/developers/weaviate/api/graphql/search-operators#nearobject) for a more detailed explanation.
+        See the [docs](https://weaviate.io/developers/weaviate/search/hybrid) for a more detailed explanation.
 
         Arguments:
-            `near_object`
-                The UUID of the object to search on, REQUIRED.
-            `certainty`
-                The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
-            `distance`
-                The maximum distance to search. If not specified, the default distance specified by the server is used.
+            `query`
+                The keyword-based query to search for, REQUIRED. If query and vector are both None, a normal search will be performed.
+            `alpha`
+                The weight of the BM25 score. If not specified, the default weight specified by the server is used.
+            `vector`
+                The specific vector to search for. If not specified, the query is vectorized and used in the similarity search.
+            `query_properties`
+                The properties to search in. If not specified, all properties are searched.
+            `fusion_type`
+                The type of fusion to apply. If not specified, the default fusion type specified by the server is used.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -67,42 +85,51 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `QueryReturn` object that includes the searched objects.
+            A `QueryReturn` or `GroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GroupByReturn` object is returned, otherwise a `QueryReturn` object is returned.
 
         Raises:
-            `weaviate.exceptions.WeaviateGRPCQueryError`:
-                If the request to the Weaviate server fails.
+            `weaviate.exceptions.WeaviateQueryError`:
+                If the network connection to Weaviate fails.
+            `weaviate.exceptions.WeaviateNotImplementedError`:
+                If a group by is provided and the Weaviate server version is lower than 1.25.0.
         """
-        res = self._query.near_object(
-            near_object=near_object,
-            certainty=certainty,
-            distance=distance,
+        if group_by is not None and not self._connection.supports_groupby_in_bm25_and_hybrid():
+            raise WeaviateUnsupportedFeatureError(
+                "Hybrid group by", self._connection.server_version, "1.25.0"
+            )
+        res = self._query.hybrid(
+            query=query,
+            alpha=alpha,
+            vector=vector,
+            properties=query_properties,
+            fusion_type=fusion_type,
             limit=limit,
             offset=offset,
             autocut=auto_limit,
             filters=filters,
             group_by=_GroupBy.from_input(group_by),
             rerank=rerank,
             target_vector=target_vector,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
         )
         return self._result_to_query_or_groupby_return(
             res,
             _QueryOptions.from_input(
-                return_metadata,
-                return_properties,
-                include_vector,
-                self._references,
-                return_references,
-                rerank,
-                group_by,
+                return_metadata=return_metadata,
+                return_properties=return_properties,
+                include_vector=include_vector,
+                collection_references=self._references,
+                query_references=return_references,
+                rerank=rerank,
+                group_by=group_by,
             ),
             return_properties,
             return_references,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_object/query.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_text/generate.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,81 @@
+from io import BufferedReader
+from pathlib import Path
 from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import (
-    METADATA,
-    GroupBy,
-    Move,
-    Rerank,
-)
+from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank, NearMediaType
 from weaviate.collections.classes.internal import (
     _Generative,
     _GroupBy,
-    GenerativeNearMediaReturnType,
+    GenerativeSearchReturnType,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 
-class _NearTextGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def near_text(
+class _NearMediaGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def near_media(
         self,
-        query: Union[List[str], str],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
-        move_to: Optional[Move] = None,
-        move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> GenerativeNearMediaReturnType[Properties, References, TProperties, TReferences]:
-        """Perform retrieval-augmented generation (RaG) on the results of a by-image object search in this collection using the image-capable vectorization module and vector-based similarity search.
+    ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
+        """Perform retrieval-augmented generation (RaG) on the results of a by-audio object search in this collection using an audio-capable vectorization module and vector-based similarity search.
 
-        See the [docs](https://weaviate.io/developers/weaviate/api/graphql/search-operators#neartext) for a more detailed explanation.
+        See the [docs](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/multi2vec-bind) for a more detailed explanation.
 
         NOTE:
-            You must have a text-capable vectorization module installed in order to use this method, e.g. any of the `text2vec-` and `multi2vec-` modules.
+            You must have a multi-media-capable vectorization module installed in order to use this method, e.g. `multi2vec-bind`.
 
         Arguments:
-            `query`
-                The text or texts to search on, REQUIRED.
+            `near_media`
+                The media file to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
+            `media_type`
+                The type of the provided media file, REQUIRED.
             `certainty`
                 The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
             `distance`
                 The maximum distance to search. If not specified, the default distance specified by the server is used.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -81,38 +83,38 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `_GenerativeNearMediaReturn` object that includes the searched objects with per-object generated results and group generated results.
+            A `GenerativeReturn` or `GenerativeGroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GenerativeGroupByReturn` object is returned, otherwise a `GenerativeReturn` object is returned.
 
         Raises:
-            `weaviate.exceptions.WeaviateGRPCQueryError`:
+            `weaviate.exceptions.WeaviateQueryError`:
                 If the request to the Weaviate server fails.
         """
-        res = self._query.near_text(
-            near_text=query,
+        res = self._query.near_media(
+            media=self._parse_media(media),
+            type_=media_type.value,
             certainty=certainty,
             distance=distance,
-            move_to=move_to,
-            move_away=move_away,
-            limit=limit,
-            offset=offset,
-            autocut=auto_limit,
             filters=filters,
             group_by=_GroupBy.from_input(group_by),
             rerank=rerank,
             target_vector=target_vector,
             generative=_Generative(
                 single=single_prompt,
                 grouped=grouped_task,
                 grouped_properties=grouped_properties,
             ),
+            limit=limit,
+            offset=offset,
+            autocut=auto_limit,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
         )
         return self._result_to_generative_return(
             res,
             _QueryOptions.from_input(
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_text/generate.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_text/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,120 +1,121 @@
-from typing import Generic, List, Optional, Union
+from io import BufferedReader
+from pathlib import Path
+from typing import Generic, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import (
-    METADATA,
-    GroupBy,
-    Move,
-    Rerank,
-)
+from weaviate.collections.classes.grpc import GroupBy, METADATA, NearMediaType, Rerank
 from weaviate.collections.classes.internal import (
     _GroupBy,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
-    QueryNearMediaReturnType,
+    QuerySearchReturnType,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 
-class _NearTextQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def near_text(
+class _NearMediaQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def near_media(
         self,
-        query: Union[List[str], str],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
-        move_to: Optional[Move] = None,
-        move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> QueryNearMediaReturnType[Properties, References, TProperties, TReferences]:
-        """Search for objects in this collection by text using text-capable vectorization module and vector-based similarity search.
+    ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
+        """Search for objects by audio in this collection using an audio-capable vectorization module and vector-based similarity search.
 
-        See the [docs](https://weaviate.io/developers/weaviate/api/graphql/search-operators#neartext) for a more detailed explanation.
+        See the [docs](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/multi2vec-bind) for a more detailed explanation.
 
         NOTE:
-            You must have a text-capable vectorization module installed in order to use this method, e.g. any of the `text2vec-` and `multi2vec-` modules.
+            You must have a multi-media-capable vectorization module installed in order to use this method, e.g. `multi2vec-bind`.
 
         Arguments:
-            `query`
-                The text or texts to search on, REQUIRED.
+            `media`
+                The media file to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
+            `media_type`
+                The type of the provided media file, REQUIRED.
             `certainty`
                 The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
             `distance`
                 The maximum distance to search. If not specified, the default distance specified by the server is used.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
                 The references to return for each object.
 
         NOTE:
-            If `return_properties` is not provided then all properties are returned except for any cross reference properties.
-            If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
-            If `return_references` is not provided then no references are provided.
+            - If `return_properties` is not provided then all properties are returned except for blob properties.
+            - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
+            - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `QueryReturn` object that includes the searched objects.
+            A `QueryReturn` or `GroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GroupByReturn` object is returned, otherwise a `QueryReturn` object is returned.
 
         Raises:
-            `weaviate.exceptions.WeaviateGRPCQueryError`:
+            `weaviate.exceptions.WeaviateQueryError`:
                 If the request to the Weaviate server fails.
         """
-        res = self._query.near_text(
-            near_text=query,
+        res = self._query.near_media(
+            media=self._parse_media(media),
+            type_=media_type.value,
             certainty=certainty,
             distance=distance,
-            move_to=move_to,
-            move_away=move_away,
             limit=limit,
             offset=offset,
             autocut=auto_limit,
             filters=filters,
-            target_vector=target_vector,
             group_by=_GroupBy.from_input(group_by),
             rerank=rerank,
+            target_vector=target_vector,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
         )
         return self._result_to_query_or_groupby_return(
             res,
             _QueryOptions.from_input(
                 return_metadata,
                 return_properties,
                 include_vector,
                 self._references,
                 return_references,
                 rerank,
-                group_by,
             ),
             return_properties,
             return_references,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_text/query.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/generate.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/generate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from typing import Generic, List, Optional
+from io import BufferedReader
+from pathlib import Path
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     _Generative,
-    GenerativeNearMediaReturnType,
     _GroupBy,
+    GenerativeSearchReturnType,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 
-class _NearVectorGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def near_vector(
+class _NearImageGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def near_image(
         self,
-        near_vector: List[float],
+        near_image: Union[str, Path, BufferedReader],
         *,
         single_prompt: Optional[str] = None,
         grouped_task: Optional[str] = None,
         grouped_properties: Optional[List[str]] = None,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
@@ -34,36 +36,43 @@
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> GenerativeNearMediaReturnType[Properties, References, TProperties, TReferences]:
-        """Perform retrieval-augmented generation (RaG) on the results of a by-vector object search in this collection using vector-based similarity search.
+    ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
+        """Perform retrieval-augmented generation (RaG) on the results of a by-image object search in this collection using an image-capable vectorization module and vector-based similarity search.
 
-        See the [docs](https://weaviate.io/developers/weaviate/search/similarity) for a more detailed explanation.
+        See the [docs](https://weaviate.io/developers/weaviate/search/image) for a more detailed explanation.
+
+        NOTE:
+            You must have an image-capable vectorization module installed in order to use this method, e.g. `img2vec-neural`, `multi2vec-clip`, or `multi2vec-bind.
 
         Arguments:
-            `near_vector`
-                The vector to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
+            `near_image`
+                The image file to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
             `certainty`
                 The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
             `distance`
                 The maximum distance to search. If not specified, the default distance specified by the server is used.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -71,36 +80,38 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `_GenerativeNearMediaReturn` object that includes the searched objects with per-object generated results and group generated results.
+            A `GenerativeReturn` or `GenerativeGroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GenerativeGroupByReturn` object is returned, otherwise a `GenerativeReturn` object is returned.
 
         Raises:
-            `weaviate.exceptions.WeaviateGRPCQueryError`:
+            `weaviate.exceptions.WeaviateQueryError`:
                 If the request to the Weaviate server fails.
         """
-        res = self._query.near_vector(
-            near_vector=near_vector,
+        res = self._query.near_media(
+            media=self._parse_media(near_image),
+            type_="image",
             certainty=certainty,
             distance=distance,
             filters=filters,
             group_by=_GroupBy.from_input(group_by),
+            rerank=rerank,
+            target_vector=target_vector,
             generative=_Generative(
                 single=single_prompt,
                 grouped=grouped_task,
                 grouped_properties=grouped_properties,
             ),
             limit=limit,
             offset=offset,
             autocut=auto_limit,
-            rerank=rerank,
-            target_vector=target_vector,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
         )
         return self._result_to_generative_return(
             res,
             _QueryOptions.from_input(
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/generate.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/generate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,92 @@
 from typing import Generic, List, Optional
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
+from weaviate.collections.classes.grpc import (
+    METADATA,
+    GroupBy,
+    HybridFusion,
+    Rerank,
+    HybridVectorType,
+)
 from weaviate.collections.classes.internal import (
-    _GroupBy,
+    GenerativeSearchReturnType,
+    _Generative,
     ReturnProperties,
     ReturnReferences,
     _QueryOptions,
-    QueryNearMediaReturnType,
+    _GroupBy,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
+from weaviate.exceptions import WeaviateUnsupportedFeatureError
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
 
-class _NearVectorQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
-    def near_vector(
+class _HybridGenerate(Generic[Properties, References], _BaseQuery[Properties, References]):
+    def hybrid(
         self,
-        near_vector: List[float],
+        query: Optional[str],
         *,
-        certainty: Optional[NUMBER] = None,
-        distance: Optional[NUMBER] = None,
+        single_prompt: Optional[str] = None,
+        grouped_task: Optional[str] = None,
+        grouped_properties: Optional[List[str]] = None,
+        alpha: NUMBER = 0.7,
+        vector: Optional[HybridVectorType] = None,
+        query_properties: Optional[List[str]] = None,
+        fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
         target_vector: Optional[str] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
-    ) -> QueryNearMediaReturnType[Properties, References, TProperties, TReferences]:
-        """Search for objects by vector in this collection using and vector-based similarity search.
+    ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
+        """Perform retrieval-augmented generation (RaG) on the results of an object search in this collection using the hybrid algorithm blending keyword-based BM25 and vector-based similarity.
 
-        See the [docs](https://weaviate.io/developers/weaviate/search/similarity) for a more detailed explanation.
+        See the [docs](https://weaviate.io/developers/weaviate/search/hybrid) for a more detailed explanation.
 
         Arguments:
-            `near_vector`
-                The vector to search on, REQUIRED. This can be a base64 encoded string of the binary, a path to the file, or a file-like object.
-            `certainty`
-                The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
-            `distance`
-                The maximum distance to search. If not specified, the default distance specified by the server is used.
+            `query`
+                The keyword-based query to search for, REQUIRED. If query and vector are both None, a normal search will be performed.
+            `single_prompt`
+                The prompt to use for RaG on each object individually.
+            `grouped_task`
+                The prompt to use for RaG on the entire result set.
+            `grouped_properties`
+                The properties to use in the RaG on the entire result set.
+            `alpha`
+                The weight of the BM25 score. If not specified, the default weight specified by the server is used.
+            `vector`
+                The specific vector to search for. If not specified, the query is vectorized and used in the similarity search.
+            `query_properties`
+                The properties to search in. If not specified, all properties are searched.
+            `fusion_type`
+                The type of fusion to apply. If not specified, the default fusion type specified by the server is used.
             `limit`
                 The maximum number of results to return. If not specified, the default limit specified by the server is returned.
             `offset`
                 The offset to start from. If not specified, the retrieval begins from the first object in the server.
             `auto_limit`
                 The maximum number of [autocut](https://weaviate.io/developers/weaviate/api/graphql/additional-operators#autocut) results to return. If not specified, no limit is applied.
             `filters`
                 The filters to apply to the search.
+            `group_by`
+                How the results should be grouped by a specific property.
             `rerank`
                 How the results should be reranked. NOTE: A `rerank-*` module must be enabled for this functionality to work.
+            `target_vector`
+                The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
             `include_vector`
                 Whether to include the vector in the results. If not specified, this is set to False.
             `return_metadata`
                 The metadata to return for each object, defaults to `None`.
             `return_properties`
                 The properties to return for each object.
             `return_references`
@@ -67,42 +94,56 @@
 
         NOTE:
             - If `return_properties` is not provided then all properties are returned except for blob properties.
             - If `return_metadata` is not provided then no metadata is provided. Use MetadataQuery.full() to retrieve all metadata.
             - If `return_references` is not provided then no references are provided.
 
         Returns:
-            A `QueryReturn` object that includes the searched objects.
+            A `GenerativeReturn` or `GenerativeGroupByReturn` object that includes the searched objects.
+            If `group_by` is provided then a `GenerativeGroupByReturn` object is returned, otherwise a `GenerativeReturn` object is returned.
 
         Raises:
-            `weaviate.exceptions.WeaviateGRPCQueryError`:
-                If the request to the Weaviate server fails.
+            `weaviate.exceptions.WeaviateQueryError`:
+                If the network connection to Weaviate fails.
+            `weaviate.exceptions.WeaviateNotImplementedError`:
+                If a group by is provided and the Weaviate server version is lower than 1.25.0.
         """
-        res = self._query.near_vector(
-            near_vector=near_vector,
-            certainty=certainty,
-            distance=distance,
+        if group_by is not None and not self._connection.supports_groupby_in_bm25_and_hybrid():
+            raise WeaviateUnsupportedFeatureError(
+                "Hybrid group by", self._connection.server_version, "1.25.0"
+            )
+        res = self._query.hybrid(
+            query=query,
+            alpha=alpha,
+            vector=vector,
+            properties=query_properties,
+            fusion_type=fusion_type,
             limit=limit,
             offset=offset,
             autocut=auto_limit,
             filters=filters,
             group_by=_GroupBy.from_input(group_by),
             rerank=rerank,
             target_vector=target_vector,
             return_metadata=self._parse_return_metadata(return_metadata, include_vector),
             return_properties=self._parse_return_properties(return_properties),
             return_references=self._parse_return_references(return_references),
+            generative=_Generative(
+                single=single_prompt,
+                grouped=grouped_task,
+                grouped_properties=grouped_properties,
+            ),
         )
-        return self._result_to_query_or_groupby_return(
+        return self._result_to_generative_return(
             res,
             _QueryOptions.from_input(
-                return_metadata,
-                return_properties,
-                include_vector,
-                self._references,
-                return_references,
-                rerank,
-                group_by,
+                return_metadata=return_metadata,
+                return_properties=return_properties,
+                include_vector=include_vector,
+                collection_references=self._references,
+                query_references=return_references,
+                rerank=rerank,
+                group_by=group_by,
             ),
             return_properties,
             return_references,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/collections/queries/near_vector/query.pyi` & `weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/collections/query.py` & `weaviate_client-4.6.0b0/weaviate/collections/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/connect/authentication.py` & `weaviate_client-4.6.0b0/weaviate/connect/authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/connect/base.py` & `weaviate_client-4.6.0b0/weaviate/connect/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,33 @@
 import datetime
 import os
 import time
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from typing import Literal, Tuple, TypeVar, Union, cast, overload
+from typing import Dict, Literal, Tuple, TypeVar, Union, cast, overload
 from urllib.parse import urlparse
 
 import grpc  # type: ignore
 from grpc import Channel, ssl_channel_credentials
 from grpc.aio import Channel as AsyncChannel  # type: ignore
 
 from pydantic import BaseModel, field_validator, model_validator
 
+from weaviate.config import Proxies
 from weaviate.types import NUMBER
 
 
 JSONPayload = Union[dict, list]
 TIMEOUT_TYPE_RETURN = Tuple[NUMBER, NUMBER]
-PYPI_TIMEOUT = 0.1
 MAX_GRPC_MESSAGE_LENGTH = 104858000  # 10mb, needs to be synchronized with GRPC server
-GRPC_OPTIONS = [
+GRPC_DEFAULT_OPTIONS = [
     ("grpc.max_send_message_length", MAX_GRPC_MESSAGE_LENGTH),
     ("grpc.max_receive_message_length", MAX_GRPC_MESSAGE_LENGTH),
 ]
 
 
-@dataclass
-class _Timeout:
-    connect: int
-    read: int
-
-    @classmethod
-    def from_timeout_config(cls, timeout: TIMEOUT_TYPE_RETURN) -> "_Timeout":
-        return cls(
-            connect=int(timeout[0]),
-            read=int(timeout[1]),
-        )
-
-
 class ProtocolParams(BaseModel):
     host: str
     port: int
     secure: bool
 
     @field_validator("host")
     def _check_host(cls, v: str) -> str:
@@ -120,37 +106,43 @@
         return (self.grpc.host, self.grpc.port)
 
     @property
     def _grpc_target(self) -> str:
         return f"{self.grpc.host}:{self.grpc.port}"
 
     @overload
-    def _grpc_channel(self, async_channel: Literal[False]) -> Channel:
+    def _grpc_channel(self, async_channel: Literal[False], proxies: Dict[str, str]) -> Channel:
         ...
 
     @overload
-    def _grpc_channel(self, async_channel: Literal[True]) -> AsyncChannel:
+    def _grpc_channel(self, async_channel: Literal[True], proxies: Dict[str, str]) -> AsyncChannel:
         ...
 
-    def _grpc_channel(self, async_channel: bool) -> Union[Channel, AsyncChannel]:
+    def _grpc_channel(
+        self, async_channel: bool, proxies: Dict[str, str]
+    ) -> Union[Channel, AsyncChannel]:
         if async_channel:
             import_path = grpc.aio
         else:
             import_path = grpc
 
+        if (p := proxies.get("grpc")) is not None:
+            options: list = [*GRPC_DEFAULT_OPTIONS, ("grpc.http_proxy", p)]
+        else:
+            options = GRPC_DEFAULT_OPTIONS
         if self.grpc.secure:
             return import_path.secure_channel(
                 target=self._grpc_target,
                 credentials=ssl_channel_credentials(),
-                options=GRPC_OPTIONS,
+                options=options,
             )
         else:
             return import_path.insecure_channel(
                 target=self._grpc_target,
-                options=GRPC_OPTIONS,
+                options=options,
             )
 
     @property
     def _http_scheme(self) -> str:
         return "https" if self.http.secure else "http"
 
     @property
@@ -164,15 +156,15 @@
         raise NotImplementedError
 
     @abstractmethod
     def get_proxies(self) -> dict:
         raise NotImplementedError
 
 
-def _get_proxies(proxies: Union[dict, str, None], trust_env: bool) -> dict:
+def _get_proxies(proxies: Union[dict, str, Proxies, None], trust_env: bool) -> dict:
     """
     Get proxies as dict, compatible with 'requests' library.
     NOTE: 'proxies' has priority over 'trust_env', i.e. if 'proxies' is NOT None, 'trust_env'
     is ignored.
 
     Parameters
     ----------
@@ -193,36 +185,42 @@
     """
 
     if proxies is not None:
         if isinstance(proxies, str):
             return {
                 "http": proxies,
                 "https": proxies,
+                "grpc": proxies,
             }
         if isinstance(proxies, dict):
             return proxies
+        if isinstance(proxies, Proxies):
+            return proxies.model_dump(exclude_none=True)
         raise TypeError(
-            "If 'proxies' is not None, it must be of type dict or str. "
+            "If 'proxies' is not None, it must be of type dict, str, or wvc.init.Proxies. "
             f"Given type: {type(proxies)}."
         )
 
     if not trust_env:
         return {}
 
     http_proxy = (os.environ.get("HTTP_PROXY"), os.environ.get("http_proxy"))
     https_proxy = (os.environ.get("HTTPS_PROXY"), os.environ.get("https_proxy"))
+    grpc_proxy = (os.environ.get("GRPC_PROXY"), os.environ.get("grpc_proxy"))
 
-    if not any(http_proxy + https_proxy):
+    if not any(http_proxy + https_proxy + grpc_proxy):
         return {}
 
     proxies = {}
     if any(http_proxy):
         proxies["http"] = http_proxy[0] if http_proxy[0] else http_proxy[1]
     if any(https_proxy):
         proxies["https"] = https_proxy[0] if https_proxy[0] else https_proxy[1]
+    if any(grpc_proxy):
+        proxies["grpc"] = grpc_proxy[0] if grpc_proxy[0] else grpc_proxy[1]
 
     return proxies
 
 
 def _get_epoch_time() -> int:
     """
     Get the current epoch time as an integer.
```

### Comparing `weaviate-client-4.5rc0/weaviate/connect/helpers.py` & `weaviate_client-4.6.0b0/weaviate/connect/helpers.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/connect/v3.py` & `weaviate_client-4.6.0b0/weaviate/connect/v3.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/connect/v4.py` & `weaviate_client-4.6.0b0/weaviate/connect/v4.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,35 +17,32 @@
     ConnectError,
     HTTPError,
     Limits,
     ReadError,
     RemoteProtocolError,
     RequestError,
     Response,
-    Timeout,
     HTTPTransport,
     get,
+    Timeout,
 )
 
 from weaviate import __version__ as client_version
 from weaviate.auth import (
     AuthCredentials,
     AuthApiKey,
     AuthClientCredentials,
 )
-from weaviate.config import ConnectionConfig
+from weaviate.config import ConnectionConfig, Proxies, Timeout as TimeoutConfig
 from weaviate.connect.authentication import _Auth
 from weaviate.connect.base import (
     _ConnectionBase,
     ConnectionParams,
-    _Timeout,
     JSONPayload,
     _get_proxies,
-    PYPI_TIMEOUT,
-    TIMEOUT_TYPE_RETURN,
 )
 from weaviate.embedded import EmbeddedV4
 from weaviate.exceptions import (
     AuthenticationFailedError,
     UnexpectedStatusCodeError,
     WeaviateGRPCUnavailableError,
     WeaviateStartUpError,
@@ -59,14 +56,16 @@
     PYPI_PACKAGE_URL,
     _decode_json_response_dict,
     _ServerVersion,
 )
 from weaviate.validator import _ValidateArgument, _validate_input
 from weaviate.warnings import _Warnings
 
+from weaviate.connect.integrations import _IntegrationConfig
+
 Session = Union[Client, OAuth2Client]
 AsyncSession = Union[AsyncClient, AsyncOAuth2Client]
 
 
 @dataclass
 class _ExpectedStatusCodes:
     ok_in: Union[List[int], int]
@@ -85,16 +84,16 @@
     Connection class used to communicate to a weaviate instance.
     """
 
     def __init__(
         self,
         connection_params: ConnectionParams,
         auth_client_secret: Optional[AuthCredentials],
-        timeout_config: Tuple[float, float],
-        proxies: Union[dict, str, None],
+        timeout_config: TimeoutConfig,
+        proxies: Union[str, Proxies, None],
         trust_env: bool,
         additional_headers: Optional[Dict[str, Any]],
         connection_config: ConnectionConfig,
         embedded_db: Optional[EmbeddedV4] = None,
     ):
         self.url = connection_params._http_url
         self.embedded_db = embedded_db
@@ -104,28 +103,28 @@
         self.__additional_headers = {}
         self._auth = auth_client_secret
         self._connection_params = connection_params
         self._grpc_stub: Optional[weaviate_pb2_grpc.WeaviateStub] = None
         self._grpc_stub_async: Optional[weaviate_pb2_grpc.WeaviateStub] = None
         self._grpc_channel: Optional[Channel] = None
         self._grpc_channel_async: Optional[AsyncChannel] = None
-        self.timeout_config = _Timeout.from_timeout_config(timeout_config)
+        self.timeout_config = timeout_config
         self.__connection_config = connection_config
         self.__trust_env = trust_env
         self._weaviate_version = _ServerVersion.from_string("")
         self.__connected = False
 
         self._headers = {"content-type": "application/json"}
         if additional_headers is not None:
             _validate_input(_ValidateArgument([dict], "additional_headers", additional_headers))
             self.__additional_headers = additional_headers
             for key, value in additional_headers.items():
                 self._headers[key.lower()] = value
 
-        self._proxies = _get_proxies(proxies, trust_env)
+        self._proxies: Dict[str, str] = _get_proxies(proxies, trust_env)
 
         # auth secrets can contain more information than a header (refresh tokens and lifetime) and therefore take
         # precedent over headers
         if "authorization" in self._headers and auth_client_secret is not None:
             _Warnings.auth_header_and_auth_secret()
             self._headers.pop("authorization")
 
@@ -143,81 +142,90 @@
         try:
             self._weaviate_version = _ServerVersion.from_string(self.get_meta()["version"])
         except (WeaviateConnectionError, ReadError, RemoteProtocolError) as e:
             raise WeaviateStartUpError(f"Could not connect to Weaviate:{e}.") from e
 
         if not skip_init_checks:
             try:
-                pkg_info = get(PYPI_PACKAGE_URL, timeout=PYPI_TIMEOUT).json()
+                pkg_info = get(PYPI_PACKAGE_URL, timeout=self.timeout_config.init).json()
                 pkg_info = pkg_info.get("info", {})
                 latest_version = pkg_info.get("version", "unknown version")
                 if is_weaviate_client_too_old(client_version, latest_version):
                     _Warnings.weaviate_client_too_old_vs_latest(client_version, latest_version)
             except RequestError:
                 pass  # ignore any errors related to requests, it is a best-effort warning
 
     def is_connected(self) -> bool:
         return self.__connected
 
+    def set_integrations(self, integrations_config: List[_IntegrationConfig]) -> None:
+        for integration in integrations_config:
+            self._headers.update(integration._to_header())
+            self.__additional_headers.update(integration._to_header())
+
     @overload
     def __make_mounts(self, type_: Literal["sync"]) -> Dict[str, HTTPTransport]:
         ...
 
     @overload
     def __make_mounts(self, type_: Literal["async"]) -> Dict[str, AsyncHTTPTransport]:
         ...
 
     def __make_mounts(
         self, type_: Literal["sync", "async"]
     ) -> Union[Dict[str, HTTPTransport], Dict[str, AsyncHTTPTransport]]:
         if type_ == "async":
-            atransport = AsyncHTTPTransport(
-                limits=Limits(
-                    max_connections=self.__connection_config.session_pool_maxsize,
-                    max_keepalive_connections=self.__connection_config.session_pool_connections,
-                ),
-                retries=self.__connection_config.session_pool_max_retries,
-                trust_env=self.__trust_env,
-            )
             return {
-                "http://": atransport,
-                "https://": atransport,
+                f"{key}://"
+                if key == "http" or key == "https"
+                else key: AsyncHTTPTransport(
+                    limits=Limits(
+                        max_connections=self.__connection_config.session_pool_maxsize,
+                        max_keepalive_connections=self.__connection_config.session_pool_connections,
+                    ),
+                    proxy=proxy,
+                    retries=self.__connection_config.session_pool_max_retries,
+                    trust_env=self.__trust_env,
+                )
+                for key, proxy in self._proxies.items()
+                if key != "grpc"
             }
         else:
             assert type_ == "sync"
-            transport = HTTPTransport(
-                limits=Limits(
-                    max_connections=self.__connection_config.session_pool_maxsize,
-                    max_keepalive_connections=self.__connection_config.session_pool_connections,
-                ),
-                retries=self.__connection_config.session_pool_max_retries,
-                trust_env=self.__trust_env,
-            )
             return {
-                "http://": transport,
-                "https://": transport,
+                f"{key}://"
+                if key == "http" or key == "https"
+                else key: HTTPTransport(
+                    limits=Limits(
+                        max_connections=self.__connection_config.session_pool_maxsize,
+                        max_keepalive_connections=self.__connection_config.session_pool_connections,
+                    ),
+                    proxy=proxy,
+                    retries=self.__connection_config.session_pool_max_retries,
+                    trust_env=self.__trust_env,
+                )
+                for key, proxy in self._proxies.items()
+                if key != "grpc"
             }
 
     def __make_sync_client(self) -> Client:
         return Client(
             headers=self._headers,
             timeout=Timeout(
-                None, connect=self.timeout_config.connect, read=self.timeout_config.read
+                None, connect=self.timeout_config.query, read=self.timeout_config.insert
             ),
-            proxies=self._proxies,
             mounts=self.__make_mounts("sync"),
         )
 
     def __make_async_client(self) -> AsyncClient:
         return AsyncClient(
             headers=self._headers,
             timeout=Timeout(
-                None, connect=self.timeout_config.connect, read=self.timeout_config.read
+                None, connect=self.timeout_config.query, read=self.timeout_config.insert
             ),
-            proxies=self._proxies,
             mounts=self.__make_mounts("async"),
         )
 
     def __make_clients(self) -> None:
         self._client = self.__make_sync_client()
 
     def _create_clients(
@@ -235,15 +243,21 @@
         # no need to check OIDC if no auth is provided and users dont want any checks at initialization time
         if skip_init_checks and auth_client_secret is None:
             self.__make_clients()
             return
 
         oidc_url = self.url + self._api_version_path + "/.well-known/openid-configuration"
         with self.__make_sync_client() as client:
-            response = client.get(oidc_url)
+            try:
+                response = client.get(oidc_url)
+            except Exception as e:
+                raise WeaviateConnectionError(
+                    f"Error: {e}. \nIs Weaviate running and reachable at {self.url}?"
+                )
+
         if response.status_code == 200:
             # Some setups are behind proxies that return some default page - for example a login - for all requests.
             # If the response is not json, we assume that this is the case and try unauthenticated access. Any auth
             # header provided by the user is unaffected.
             try:
                 resp = response.json()
             except Exception:
@@ -353,23 +367,25 @@
             daemon=True,
             name="TokenRefresh",
         )
         demon.start()
 
     async def aopen(self) -> None:
         if self._aclient is None:
-            self._aclient = self.__make_async_client()
+            self._aclient = await self.__make_async_client().__aenter__()
         if self._grpc_stub_async is None:
-            self._grpc_channel_async = self._connection_params._grpc_channel(async_channel=True)
+            self._grpc_channel_async = self._connection_params._grpc_channel(
+                async_channel=True, proxies=self._proxies
+            )
             assert self._grpc_channel_async is not None
             self._grpc_stub_async = weaviate_pb2_grpc.WeaviateStub(self._grpc_channel_async)
 
     async def aclose(self) -> None:
         if self._aclient is not None:
-            await self._aclient.aclose()
+            await self._aclient.__aexit__()
             self._aclient = None
         if self._grpc_stub_async is not None:
             assert self._grpc_channel_async is not None
             await self._grpc_channel_async.close()
             self._grpc_stub_async = None
 
     def close(self) -> None:
@@ -573,22 +589,25 @@
         Returns the meta endpoint.
         """
         response = self.get(path="/meta")
         res = _decode_json_response_dict(response, "Meta endpoint")
         assert res is not None
         return res
 
+    def supports_groupby_in_bm25_and_hybrid(self) -> bool:
+        return self._weaviate_version.is_at_least(1, 25, 0)
+
 
 class ConnectionV4(_Connection):
     def __init__(
         self,
         connection_params: ConnectionParams,
         auth_client_secret: Optional[AuthCredentials],
-        timeout_config: TIMEOUT_TYPE_RETURN,
-        proxies: Union[dict, str, None],
+        timeout_config: TimeoutConfig,
+        proxies: Union[str, Proxies, None],
         trust_env: bool,
         additional_headers: Optional[Dict[str, Any]],
         connection_config: ConnectionConfig,
         embedded_db: Optional[EmbeddedV4] = None,
     ):
         super().__init__(
             connection_params,
@@ -638,24 +657,30 @@
             raise WeaviateClosedClientError()
         assert self._grpc_channel is not None
         try:
             res: health_pb2.HealthCheckResponse = self._grpc_channel.unary_unary(
                 "/grpc.health.v1.Health/Check",
                 request_serializer=health_pb2.HealthCheckRequest.SerializeToString,
                 response_deserializer=health_pb2.HealthCheckResponse.FromString,
-            )(health_pb2.HealthCheckRequest(), timeout=1)
+            )(health_pb2.HealthCheckRequest(), timeout=self.timeout_config.init)
             if res.status != health_pb2.HealthCheckResponse.SERVING:
-                raise WeaviateGRPCUnavailableError(f"v{self.server_version}")
+                raise WeaviateGRPCUnavailableError(
+                    f"v{self.server_version}", self._connection_params._grpc_address
+                )
         except _channel._InactiveRpcError as e:
-            raise WeaviateGRPCUnavailableError(f"v{self.server_version}") from e
+            raise WeaviateGRPCUnavailableError(
+                f"v{self.server_version}", self._connection_params._grpc_address
+            ) from e
 
     def connect(self, skip_init_checks: bool) -> None:
         super().connect(skip_init_checks)
         # create GRPC channel. If Weaviate does not support GRPC then error now.
-        self._grpc_channel = self._connection_params._grpc_channel(async_channel=False)
+        self._grpc_channel = self._connection_params._grpc_channel(
+            async_channel=False, proxies=self._proxies
+        )
         assert self._grpc_channel is not None
         self._grpc_stub = weaviate_pb2_grpc.WeaviateStub(self._grpc_channel)
         if not skip_init_checks:
             self._ping_grpc()
 
         # do it after all other init checks so as not to break all the tests
         if self._weaviate_version.is_lower_than(1, 23, 7):
```

### Comparing `weaviate-client-4.5rc0/weaviate/contextionary/crud_contextionary.py` & `weaviate_client-4.6.0b0/weaviate/contextionary/crud_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/data/crud_data.py` & `weaviate_client-4.6.0b0/weaviate/data/crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/data/references/crud_references.py` & `weaviate_client-4.6.0b0/weaviate/data/references/crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/embedded.py` & `weaviate_client-4.6.0b0/weaviate/embedded.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import zipfile
 from abc import abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, Optional, Tuple
 
 import requests
-import validators  # type: ignore
+import validators
 
 from weaviate import exceptions
 from weaviate.exceptions import WeaviateStartUpError
 from weaviate.util import _decode_json_response_dict
 
 DEFAULT_BINARY_PATH = str(Path.home() / ".cache/weaviate-embedded/")
 DEFAULT_PERSISTENCE_DATA_PATH = str(Path.home() / ".local/share/weaviate")
@@ -138,16 +138,16 @@
         if not self._weaviate_binary_path.exists():
             print(
                 f"Binary {self.options.binary_path} did not exist. Downloading binary from {self._download_url}"
             )
             if self._download_url.endswith(".tar.gz"):
                 tar_filename = Path(self.options.binary_path, "tmp_weaviate.tgz")
                 urllib.request.urlretrieve(self._download_url, tar_filename)
-                binary_tar = tarfile.open(tar_filename)
-                binary_tar.extract("weaviate", path=Path(self.options.binary_path))
+                with tarfile.open(tar_filename) as binary_tar:
+                    binary_tar.extract("weaviate", path=Path(self.options.binary_path))
                 tar_filename.unlink()
             else:
                 assert self._download_url.endswith(".zip")
                 zip_filename = Path(self.options.binary_path, "tmp_weaviate.zip")
                 urllib.request.urlretrieve(self._download_url, zip_filename)
                 with zipfile.ZipFile(zip_filename, "r") as zip_ref:
                     zip_ref.extract("weaviate", path=Path(self.options.binary_path))
@@ -247,19 +247,19 @@
 
 
 class EmbeddedV3(_EmbeddedBase):
     def is_listening(self) -> bool:
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
             s.connect((self.options.hostname, self.options.port))
-            s.close()
             return True
         except (socket.error, ConnectionRefusedError):
-            s.close()
             return False
+        finally:
+            s.close()
 
     def start(self) -> None:
         if self.is_listening():
             print(f"embedded weaviate is already listening on port {self.options.port}")
             return
         super().start()
```

### Comparing `weaviate-client-4.5rc0/weaviate/error_msgs.py` & `weaviate_client-4.6.0b0/weaviate/error_msgs.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/exceptions.py` & `weaviate_client-4.6.0b0/weaviate/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Weaviate Exceptions.
 """
 
 from json.decoder import JSONDecodeError
-from typing import Union
+from typing import Union, Tuple
 import httpx
 import requests
 
 ERROR_CODE_EXPLANATION = {
     413: """Payload Too Large. Try to decrease the batch size or increase the maximum request size on your weaviate
          server."""
 }
@@ -268,19 +268,33 @@
         msg = f"""It is forbidden to insert `id` or `vector` inside properties: {data}. Only properties defined in your collection's config can be inserted as properties of the object, `id` is totally forbidden as it is reserved and `vector` is forbidden at this level. You should use the `DataObject` class if you wish to insert an object with a custom `vector` whilst inserting its properties."""
         super().__init__(msg)
 
 
 class WeaviateGRPCUnavailableError(WeaviateBaseError):
     """Is raised when a gRPC-backed query is made with no gRPC connection present."""
 
-    def __init__(self, weaviate_version: str = "") -> None:
-        msg = f"""gRPC health check could not be completed. This could have several reasons:
-        - gRPC is not enabled or incorrectly configured on the server with version {weaviate_version} or the client
-        - your connection is unstable or has a high latency. In this case you can disable startup checks by connecting using `skip_init_checks=True`
-        """
+    def __init__(
+        self, weaviate_version: str = "", grpc_address: Tuple[str, int] = ("not provided", 0)
+    ) -> None:
+        if grpc_address[0] == "not provided":
+            grpc_msg = "Please check the server address and port."
+        else:
+            grpc_msg = f"Please check that the server address and port ({grpc_address[0]}:{grpc_address[1]}) are correct."
+        msg = f"""
+Weaviate {weaviate_version} makes use of a high-speed gRPC API as well as a REST API.
+Unfortunately, the gRPC health check against Weaviate could not be completed.
+
+This error could be due to one of several reasons:
+- The gRPC traffic at the specified port is blocked by a firewall.
+- gRPC is not enabled or incorrectly configured on the server or the client.
+    - {grpc_msg}
+- your connection is unstable or has a high latency. In this case you can:
+    - increase init-timeout in `weaviate.connect_to_local(additional_config=wvc.init.AdditionalConfig(timeout=wvc.init.Timeout(init=X)))`
+    - disable startup checks by connecting using `skip_init_checks=True`
+"""
         super().__init__(msg)
 
 
 WeaviateGrpcUnavailable = WeaviateGRPCUnavailableError
 
 
 class WeaviateInsertManyAllFailedError(WeaviateBaseError):
@@ -301,7 +315,15 @@
 
 class WeaviateConnectionError(WeaviateBaseError):
     """Is raised when the connection to Weaviate fails."""
 
     def __init__(self, message: str = "") -> None:
         msg = f"""Connection to Weaviate failed. {message}"""
         super().__init__(msg)
+
+
+class WeaviateUnsupportedFeatureError(WeaviateBaseError):
+    """Is raised when a client method tries to use a new feature with an old Weaviate version."""
+
+    def __init__(self, feature: str, current: str, minimum: str) -> None:
+        msg = f"""{feature} is not supported by your connected server's Weaviate version. The current version is {current}, but the feature requires at least version {minimum}."""
+        super().__init__(msg)
```

### Comparing `weaviate-client-4.5rc0/weaviate/gql/aggregate.py` & `weaviate_client-4.6.0b0/weaviate/gql/aggregate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
 GraphQL `Aggregate` command.
 """
 
 import json
+from dataclasses import dataclass
 from typing import List, Optional, Union
 
 from weaviate.connect import Connection, ConnectionV4
-from weaviate.util import (
-    _capitalize_first_letter,
-    file_encoder_b64,
-)
+from weaviate.util import _capitalize_first_letter, file_encoder_b64, _sanitize_str
 from .filter import (
     Where,
     GraphQL,
     Filter,
     NearAudio,
     NearDepth,
     NearImage,
@@ -23,14 +21,46 @@
     NearThermal,
     NearVector,
     NearVideo,
     MediaType,
 )
 
 
+@dataclass
+class Hybrid:
+    query: Optional[str]
+    alpha: Optional[float]
+    vector: Optional[List[float]]
+    properties: Optional[List[str]]
+    target_vectors: Optional[List[str]]
+
+    def __init__(self, content: dict) -> None:
+        self.query = content.get("query")
+        self.alpha = content.get("alpha")
+        self.vector = content.get("vector")
+        self.properties = content.get("properties")
+        self.target_vectors = content.get("targetVectors")
+
+    def __str__(self) -> str:
+        ret = ""
+        if self.query is not None:
+            ret += f"query: {_sanitize_str(self.query)}"
+        if self.vector is not None:
+            ret += f", vector: {self.vector}"
+        if self.alpha is not None:
+            ret += f", alpha: {self.alpha}"
+        if self.properties is not None and len(self.properties) > 0:
+            props = '","'.join(self.properties)
+            ret += f', properties: ["{props}"]'
+        if self.target_vectors is not None:
+            target_vectors = '","'.join(self.target_vectors)
+            ret += f', targetVectors: ["{target_vectors}"]'
+        return "hybrid:{" + ret + "}"
+
+
 class AggregateBuilder(GraphQL):
     """
     AggregateBuilder class used to aggregate Weaviate objects.
     """
 
     def __init__(self, class_name: str, connection: Union[Connection, ConnectionV4]):
         """
@@ -51,14 +81,15 @@
         self._fields: List[str] = []
         self._where: Optional[Where] = None
         self._group_by_properties: Optional[List[str]] = None
         self._uses_filter: bool = False
         self._near: Optional[Filter] = None
         self._tenant: Optional[str] = None
         self._limit: Optional[int] = None
+        self._hybrid: Optional[Hybrid] = None
 
     def with_tenant(self, tenant: str) -> "AggregateBuilder":
         """Sets a tenant for the query."""
         if not isinstance(tenant, str):
             raise TypeError("tenant must be of type str")
 
         self._tenant = tenant
@@ -205,14 +236,28 @@
             Updated AggregateBuilder.
         """
 
         self._where = Where(content)
         self._uses_filter = True
         return self
 
+    def with_hybrid(self, content: dict) -> "AggregateBuilder":
+        """Get objects using bm25 and vector, then combine the results using a reciprocal ranking algorithm.
+
+        Parameters
+        ----------
+        content : dict
+            The content of the `hybrid` filter to set.
+        """
+        if self._near is not None:
+            raise AttributeError("Cannot use 'hybrid' and 'near' filters simultaneously.")
+        self._hybrid = Hybrid(content)
+        self._uses_filter = True
+        return self
+
     def with_group_by_filter(self, properties: List[str]) -> "AggregateBuilder":
         """
         Add a group by filter to the query. Might requires the user to set
         an additional group by clause using `with_fields(..)`.
 
         Parameters
         ----------
@@ -304,14 +349,16 @@
         ------
         AttributeError
             If another 'near' filter was already set.
         """
 
         if self._near is not None:
             raise AttributeError("Cannot use multiple 'near' filters.")
+        if self._hybrid is not None:
+            raise AttributeError("Cannot use 'near' and 'hybrid' filters simultaneously.")
         self._near = NearText(content)
         self._uses_filter = True
         return self
 
     def with_near_vector(self, content: dict) -> "AggregateBuilder":
         """
         Set `nearVector` filter.
@@ -369,14 +416,16 @@
         ------
         AttributeError
             If another 'near' filter was already set.
         """
 
         if self._near is not None:
             raise AttributeError("Cannot use multiple 'near' filters.")
+        if self._hybrid is not None:
+            raise AttributeError("Cannot use 'near' and 'hybrid' filters simultaneously.")
         self._near = NearVector(content)
         self._uses_filter = True
         return self
 
     def with_near_object(self, content: dict) -> "AggregateBuilder":
         """
         Set `nearObject` filter.
@@ -419,14 +468,16 @@
             If another 'near' filter was already set.
         """
 
         is_server_version_14 = self._connection.server_version >= "1.14"
 
         if self._near is not None:
             raise AttributeError("Cannot use multiple 'near' filters.")
+        if self._hybrid is not None:
+            raise AttributeError("Cannot use 'near' and 'hybrid' filters simultaneously.")
         self._near = NearObject(content, is_server_version_14)
         self._uses_filter = True
         return self
 
     def with_near_image(self, content: dict, encode: bool = True) -> "AggregateBuilder":
         """
         Set `nearImage` filter.
@@ -530,14 +581,16 @@
         """
         self._media_type = MediaType.IMAGE
         if self._near is not None:
             raise AttributeError(
                 "Cannot use multiple 'near' filters, or a 'near' filter along"
                 " with a 'ask' filter!"
             )
+        if self._hybrid is not None:
+            raise AttributeError("Cannot use 'near' and 'hybrid' filters simultaneously.")
         if encode:
             content["image"] = file_encoder_b64(content["image"])
         self._near = NearImage(content)
         self._uses_filter = True
         return self
 
     def with_near_audio(self, content: dict, encode: bool = True) -> "AggregateBuilder":
@@ -644,14 +697,16 @@
 
         self._media_type = MediaType.AUDIO
         if self._near is not None:
             raise AttributeError(
                 "Cannot use multiple 'near' filters, or a 'near' filter along"
                 " with a 'ask' filter!"
             )
+        if self._hybrid is not None:
+            raise AttributeError("Cannot use 'near' and 'hybrid' filters simultaneously.")
         if encode:
             content[self._media_type.value] = file_encoder_b64(content[self._media_type.value])
         self._near = NearAudio(content)
         self._uses_filter = True
         return self
 
     def with_near_video(self, content: dict, encode: bool = True) -> "AggregateBuilder":
@@ -758,14 +813,16 @@
 
         self._media_type = MediaType.VIDEO
         if self._near is not None:
             raise AttributeError(
                 "Cannot use multiple 'near' filters, or a 'near' filter along"
                 " with a 'ask' filter!"
             )
+        if self._hybrid is not None:
+            raise AttributeError("Cannot use 'near' and 'hybrid' filters simultaneously.")
         if encode:
             content[self._media_type.value] = file_encoder_b64(content[self._media_type.value])
         self._near = NearVideo(content)
         self._uses_filter = True
         return self
 
     def with_near_depth(self, content: dict, encode: bool = True) -> "AggregateBuilder":
@@ -872,14 +929,16 @@
 
         self._media_type = MediaType.DEPTH
         if self._near is not None:
             raise AttributeError(
                 "Cannot use multiple 'near' filters, or a 'near' filter along"
                 " with a 'ask' filter!"
             )
+        if self._hybrid is not None:
+            raise AttributeError("Cannot use 'near' and 'hybrid' filters simultaneously.")
         if encode:
             content[self._media_type.value] = file_encoder_b64(content[self._media_type.value])
         self._near = NearDepth(content)
         self._uses_filter = True
         return self
 
     def with_near_thermal(self, content: dict, encode: bool = True) -> "AggregateBuilder":
@@ -985,14 +1044,16 @@
 
         self._media_type = MediaType.THERMAL
         if self._near is not None:
             raise AttributeError(
                 "Cannot use multiple 'near' filters, or a 'near' filter along"
                 " with a 'ask' filter!"
             )
+        if self._hybrid is not None:
+            raise AttributeError("Cannot use 'near' and 'hybrid' filters simultaneously.")
         if encode:
             content[self._media_type.value] = file_encoder_b64(content[self._media_type.value])
         self._near = NearThermal(content)
         self._uses_filter = True
         return self
 
     def with_near_imu(self, content: dict, encode: bool = True) -> "AggregateBuilder":
@@ -1099,14 +1160,16 @@
 
         self._media_type = MediaType.IMU
         if self._near is not None:
             raise AttributeError(
                 "Cannot use multiple 'near' filters, or a 'near' filter along"
                 " with a 'ask' filter!"
             )
+        if self._hybrid is not None:
+            raise AttributeError("Cannot use 'near' and 'hybrid' filters simultaneously.")
         if encode:
             content[self._media_type.value] = file_encoder_b64(content[self._media_type.value])
         self._near = NearIMU(content)
         self._uses_filter = True
         return self
 
     def build(self) -> str:
@@ -1133,15 +1196,16 @@
                 query += str(self._near)
             if self._object_limit:
                 query += f"objectLimit: {self._object_limit}"
             if self._tenant is not None:
                 query += f'tenant: "{self._tenant}"'
             if self._limit is not None:
                 query += f"limit: {self._limit}"
-
+            if self._hybrid is not None:
+                query += str(self._hybrid)
             query += ")"
 
         # Body
         query += "{"
         if self._with_meta_count:
             query += "meta{count}"
         for field in self._fields:
```

### Comparing `weaviate-client-4.5rc0/weaviate/gql/filter.py` & `weaviate_client-4.6.0b0/weaviate/gql/filter.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/gql/get.py` & `weaviate_client-4.6.0b0/weaviate/gql/get.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/gql/multi_get.py` & `weaviate_client-4.6.0b0/weaviate/gql/multi_get.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/gql/query.py` & `weaviate_client-4.6.0b0/weaviate/gql/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/outputs/aggregate.py` & `weaviate_client-4.6.0b0/weaviate/outputs/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/outputs/config.py` & `weaviate_client-4.6.0b0/weaviate/outputs/config.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/outputs/query.py` & `weaviate_client-4.6.0b0/weaviate/outputs/query.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2.py` & `weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/base_pb2.pyi` & `weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2.py` & `weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/batch_delete_pb2.pyi` & `weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2.py` & `weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/batch_pb2.pyi` & `weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/properties_pb2.pyi` & `weaviate_client-4.6.0b0/weaviate/proto/v1/properties_pb2.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -38,60 +38,141 @@
         "date_value",
         "uuid_value",
         "int_value",
         "geo_value",
         "blob_value",
         "phone_value",
         "null_value",
+        "text_value",
     )
     NUMBER_VALUE_FIELD_NUMBER: _ClassVar[int]
     STRING_VALUE_FIELD_NUMBER: _ClassVar[int]
     BOOL_VALUE_FIELD_NUMBER: _ClassVar[int]
     OBJECT_VALUE_FIELD_NUMBER: _ClassVar[int]
     LIST_VALUE_FIELD_NUMBER: _ClassVar[int]
     DATE_VALUE_FIELD_NUMBER: _ClassVar[int]
     UUID_VALUE_FIELD_NUMBER: _ClassVar[int]
     INT_VALUE_FIELD_NUMBER: _ClassVar[int]
     GEO_VALUE_FIELD_NUMBER: _ClassVar[int]
     BLOB_VALUE_FIELD_NUMBER: _ClassVar[int]
     PHONE_VALUE_FIELD_NUMBER: _ClassVar[int]
     NULL_VALUE_FIELD_NUMBER: _ClassVar[int]
+    TEXT_VALUE_FIELD_NUMBER: _ClassVar[int]
     number_value: float
     string_value: str
     bool_value: bool
     object_value: Properties
     list_value: ListValue
     date_value: str
     uuid_value: str
     int_value: int
     geo_value: GeoCoordinate
     blob_value: str
     phone_value: PhoneNumber
     null_value: _struct_pb2.NullValue
+    text_value: str
     def __init__(
         self,
         number_value: _Optional[float] = ...,
         string_value: _Optional[str] = ...,
         bool_value: bool = ...,
         object_value: _Optional[_Union[Properties, _Mapping]] = ...,
         list_value: _Optional[_Union[ListValue, _Mapping]] = ...,
         date_value: _Optional[str] = ...,
         uuid_value: _Optional[str] = ...,
         int_value: _Optional[int] = ...,
         geo_value: _Optional[_Union[GeoCoordinate, _Mapping]] = ...,
         blob_value: _Optional[str] = ...,
         phone_value: _Optional[_Union[PhoneNumber, _Mapping]] = ...,
         null_value: _Optional[_Union[_struct_pb2.NullValue, str]] = ...,
+        text_value: _Optional[str] = ...,
     ) -> None: ...
 
 class ListValue(_message.Message):
-    __slots__ = ("values",)
+    __slots__ = (
+        "values",
+        "number_values",
+        "bool_values",
+        "object_values",
+        "date_values",
+        "uuid_values",
+        "int_values",
+        "text_values",
+    )
     VALUES_FIELD_NUMBER: _ClassVar[int]
+    NUMBER_VALUES_FIELD_NUMBER: _ClassVar[int]
+    BOOL_VALUES_FIELD_NUMBER: _ClassVar[int]
+    OBJECT_VALUES_FIELD_NUMBER: _ClassVar[int]
+    DATE_VALUES_FIELD_NUMBER: _ClassVar[int]
+    UUID_VALUES_FIELD_NUMBER: _ClassVar[int]
+    INT_VALUES_FIELD_NUMBER: _ClassVar[int]
+    TEXT_VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedCompositeFieldContainer[Value]
-    def __init__(self, values: _Optional[_Iterable[_Union[Value, _Mapping]]] = ...) -> None: ...
+    number_values: NumberValues
+    bool_values: BoolValues
+    object_values: ObjectValues
+    date_values: DateValues
+    uuid_values: UuidValues
+    int_values: IntValues
+    text_values: TextValues
+    def __init__(
+        self,
+        values: _Optional[_Iterable[_Union[Value, _Mapping]]] = ...,
+        number_values: _Optional[_Union[NumberValues, _Mapping]] = ...,
+        bool_values: _Optional[_Union[BoolValues, _Mapping]] = ...,
+        object_values: _Optional[_Union[ObjectValues, _Mapping]] = ...,
+        date_values: _Optional[_Union[DateValues, _Mapping]] = ...,
+        uuid_values: _Optional[_Union[UuidValues, _Mapping]] = ...,
+        int_values: _Optional[_Union[IntValues, _Mapping]] = ...,
+        text_values: _Optional[_Union[TextValues, _Mapping]] = ...,
+    ) -> None: ...
+
+class NumberValues(_message.Message):
+    __slots__ = ("values",)
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: bytes
+    def __init__(self, values: _Optional[bytes] = ...) -> None: ...
+
+class TextValues(_message.Message):
+    __slots__ = ("values",)
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class BoolValues(_message.Message):
+    __slots__ = ("values",)
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.RepeatedScalarFieldContainer[bool]
+    def __init__(self, values: _Optional[_Iterable[bool]] = ...) -> None: ...
+
+class ObjectValues(_message.Message):
+    __slots__ = ("values",)
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.RepeatedCompositeFieldContainer[Properties]
+    def __init__(
+        self, values: _Optional[_Iterable[_Union[Properties, _Mapping]]] = ...
+    ) -> None: ...
+
+class DateValues(_message.Message):
+    __slots__ = ("values",)
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class UuidValues(_message.Message):
+    __slots__ = ("values",)
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
+
+class IntValues(_message.Message):
+    __slots__ = ("values",)
+    VALUES_FIELD_NUMBER: _ClassVar[int]
+    values: bytes
+    def __init__(self, values: _Optional[bytes] = ...) -> None: ...
 
 class GeoCoordinate(_message.Message):
     __slots__ = ("longitude", "latitude")
     LONGITUDE_FIELD_NUMBER: _ClassVar[int]
     LATITUDE_FIELD_NUMBER: _ClassVar[int]
     longitude: float
     latitude: float
```

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2.py` & `weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from weaviate.proto.v1 import base_pb2 as v1_dot_base__pb2
 from weaviate.proto.v1 import properties_pb2 as v1_dot_properties__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x13v1/search_get.proto\x12\x0bweaviate.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\rv1/base.proto\x1a\x13v1/properties.proto"\xec\n\n\rSearchRequest\x12\x12\n\ncollection\x18\x01 \x01(\t\x12\x0e\n\x06tenant\x18\n \x01(\t\x12=\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32\x1d.weaviate.v1.ConsistencyLevelH\x00\x88\x01\x01\x12\x37\n\nproperties\x18\x14 \x01(\x0b\x32\x1e.weaviate.v1.PropertiesRequestH\x01\x88\x01\x01\x12\x33\n\x08metadata\x18\x15 \x01(\x0b\x32\x1c.weaviate.v1.MetadataRequestH\x02\x88\x01\x01\x12+\n\x08group_by\x18\x16 \x01(\x0b\x32\x14.weaviate.v1.GroupByH\x03\x88\x01\x01\x12\r\n\x05limit\x18\x1e \x01(\r\x12\x0e\n\x06offset\x18\x1f \x01(\r\x12\x0f\n\x07\x61utocut\x18  \x01(\r\x12\r\n\x05\x61\x66ter\x18! \x01(\t\x12$\n\x07sort_by\x18" \x03(\x0b\x32\x13.weaviate.v1.SortBy\x12*\n\x07\x66ilters\x18( \x01(\x0b\x32\x14.weaviate.v1.FiltersH\x04\x88\x01\x01\x12/\n\rhybrid_search\x18) \x01(\x0b\x32\x13.weaviate.v1.HybridH\x05\x88\x01\x01\x12+\n\x0b\x62m25_search\x18* \x01(\x0b\x32\x11.weaviate.v1.BM25H\x06\x88\x01\x01\x12\x31\n\x0bnear_vector\x18+ \x01(\x0b\x32\x17.weaviate.v1.NearVectorH\x07\x88\x01\x01\x12\x31\n\x0bnear_object\x18, \x01(\x0b\x32\x17.weaviate.v1.NearObjectH\x08\x88\x01\x01\x12\x33\n\tnear_text\x18- \x01(\x0b\x32\x1b.weaviate.v1.NearTextSearchH\t\x88\x01\x01\x12\x35\n\nnear_image\x18. \x01(\x0b\x32\x1c.weaviate.v1.NearImageSearchH\n\x88\x01\x01\x12\x35\n\nnear_audio\x18/ \x01(\x0b\x32\x1c.weaviate.v1.NearAudioSearchH\x0b\x88\x01\x01\x12\x35\n\nnear_video\x18\x30 \x01(\x0b\x32\x1c.weaviate.v1.NearVideoSearchH\x0c\x88\x01\x01\x12\x35\n\nnear_depth\x18\x31 \x01(\x0b\x32\x1c.weaviate.v1.NearDepthSearchH\r\x88\x01\x01\x12\x39\n\x0cnear_thermal\x18\x32 \x01(\x0b\x32\x1e.weaviate.v1.NearThermalSearchH\x0e\x88\x01\x01\x12\x31\n\x08near_imu\x18\x33 \x01(\x0b\x32\x1a.weaviate.v1.NearIMUSearchH\x0f\x88\x01\x01\x12\x36\n\ngenerative\x18< \x01(\x0b\x32\x1d.weaviate.v1.GenerativeSearchH\x10\x88\x01\x01\x12(\n\x06rerank\x18= \x01(\x0b\x32\x13.weaviate.v1.RerankH\x11\x88\x01\x01\x12\x18\n\x0cuses_123_api\x18\x64 \x01(\x08\x42\x02\x18\x01\x42\x14\n\x12_consistency_levelB\r\n\x0b_propertiesB\x0b\n\t_metadataB\x0b\n\t_group_byB\n\n\x08_filtersB\x10\n\x0e_hybrid_searchB\x0e\n\x0c_bm25_searchB\x0e\n\x0c_near_vectorB\x0e\n\x0c_near_objectB\x0c\n\n_near_textB\r\n\x0b_near_imageB\r\n\x0b_near_audioB\r\n\x0b_near_videoB\r\n\x0b_near_depthB\x0f\n\r_near_thermalB\x0b\n\t_near_imuB\r\n\x0b_generativeB\t\n\x07_rerank"L\n\x07GroupBy\x12\x0c\n\x04path\x18\x01 \x03(\t\x12\x18\n\x10number_of_groups\x18\x02 \x01(\x05\x12\x19\n\x11objects_per_group\x18\x03 \x01(\x05")\n\x06SortBy\x12\x11\n\tascending\x18\x01 \x01(\x08\x12\x0c\n\x04path\x18\x02 \x03(\t"m\n\x10GenerativeSearch\x12\x1e\n\x16single_response_prompt\x18\x01 \x01(\t\x12\x1d\n\x15grouped_response_task\x18\x02 \x01(\t\x12\x1a\n\x12grouped_properties\x18\x03 \x03(\t"\xdd\x01\n\x0fMetadataRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\x08\x12\x0e\n\x06vector\x18\x02 \x01(\x08\x12\x1a\n\x12\x63reation_time_unix\x18\x03 \x01(\x08\x12\x1d\n\x15last_update_time_unix\x18\x04 \x01(\x08\x12\x10\n\x08\x64istance\x18\x05 \x01(\x08\x12\x11\n\tcertainty\x18\x06 \x01(\x08\x12\r\n\x05score\x18\x07 \x01(\x08\x12\x15\n\rexplain_score\x18\x08 \x01(\x08\x12\x15\n\ris_consistent\x18\t \x01(\x08\x12\x0f\n\x07vectors\x18\n \x03(\t"\xd1\x01\n\x11PropertiesRequest\x12\x1a\n\x12non_ref_properties\x18\x01 \x03(\t\x12\x39\n\x0eref_properties\x18\x02 \x03(\x0b\x32!.weaviate.v1.RefPropertiesRequest\x12?\n\x11object_properties\x18\x03 \x03(\x0b\x32$.weaviate.v1.ObjectPropertiesRequest\x12$\n\x1creturn_all_nonref_properties\x18\x0b \x01(\x08"\x8b\x01\n\x17ObjectPropertiesRequest\x12\x11\n\tprop_name\x18\x01 \x01(\t\x12\x1c\n\x14primitive_properties\x18\x02 \x03(\t\x12?\n\x11object_properties\x18\x03 \x03(\x0b\x32$.weaviate.v1.ObjectPropertiesRequest"\x94\x02\n\x06Hybrid\x12\r\n\x05query\x18\x01 \x01(\t\x12\x12\n\nproperties\x18\x02 \x03(\t\x12\x12\n\x06vector\x18\x03 \x03(\x02\x42\x02\x18\x01\x12\r\n\x05\x61lpha\x18\x04 \x01(\x02\x12\x33\n\x0b\x66usion_type\x18\x05 \x01(\x0e\x32\x1e.weaviate.v1.Hybrid.FusionType\x12\x14\n\x0cvector_bytes\x18\x06 \x01(\x0c\x12\x16\n\x0etarget_vectors\x18\x07 \x03(\t"a\n\nFusionType\x12\x1b\n\x17\x46USION_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x46USION_TYPE_RANKED\x10\x01\x12\x1e\n\x1a\x46USION_TYPE_RELATIVE_SCORE\x10\x02"\xc5\x02\n\x0eNearTextSearch\x12\r\n\x05query\x18\x01 \x03(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x36\n\x07move_to\x18\x04 \x01(\x0b\x32 .weaviate.v1.NearTextSearch.MoveH\x02\x88\x01\x01\x12\x38\n\tmove_away\x18\x05 \x01(\x0b\x32 .weaviate.v1.NearTextSearch.MoveH\x03\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x06 \x03(\t\x1a\x36\n\x04Move\x12\r\n\x05\x66orce\x18\x01 \x01(\x02\x12\x10\n\x08\x63oncepts\x18\x02 \x03(\t\x12\r\n\x05uuids\x18\x03 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distanceB\n\n\x08_move_toB\x0c\n\n_move_away"\x82\x01\n\x0fNearImageSearch\x12\r\n\x05image\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"\x82\x01\n\x0fNearAudioSearch\x12\r\n\x05\x61udio\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"\x82\x01\n\x0fNearVideoSearch\x12\r\n\x05video\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"\x82\x01\n\x0fNearDepthSearch\x12\r\n\x05\x64\x65pth\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"\x86\x01\n\x11NearThermalSearch\x12\x0f\n\x07thermal\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"~\n\rNearIMUSearch\x12\x0b\n\x03imu\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance")\n\x04\x42M25\x12\r\n\x05query\x18\x01 \x01(\t\x12\x12\n\nproperties\x18\x02 \x03(\t"\xb1\x01\n\x14RefPropertiesRequest\x12\x1a\n\x12reference_property\x18\x01 \x01(\t\x12\x32\n\nproperties\x18\x02 \x01(\x0b\x32\x1e.weaviate.v1.PropertiesRequest\x12.\n\x08metadata\x18\x03 \x01(\x0b\x32\x1c.weaviate.v1.MetadataRequest\x12\x19\n\x11target_collection\x18\x04 \x01(\t"\x98\x01\n\nNearVector\x12\x12\n\x06vector\x18\x01 \x03(\x02\x42\x02\x18\x01\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x14\n\x0cvector_bytes\x18\x04 \x01(\x0c\x12\x16\n\x0etarget_vectors\x18\x05 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"z\n\nNearObject\x12\n\n\x02id\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"8\n\x06Rerank\x12\x10\n\x08property\x18\x01 \x01(\t\x12\x12\n\x05query\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_query"\xc3\x01\n\x0bSearchReply\x12\x0c\n\x04took\x18\x01 \x01(\x02\x12*\n\x07results\x18\x02 \x03(\x0b\x32\x19.weaviate.v1.SearchResult\x12&\n\x19generative_grouped_result\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x34\n\x10group_by_results\x18\x04 \x03(\x0b\x32\x1a.weaviate.v1.GroupByResultB\x1c\n\x1a_generative_grouped_result"\x1c\n\x0bRerankReply\x12\r\n\x05score\x18\x01 \x01(\x01"!\n\x0fGenerativeReply\x12\x0e\n\x06result\x18\x01 \x01(\t"\x90\x02\n\rGroupByResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0cmin_distance\x18\x02 \x01(\x02\x12\x14\n\x0cmax_distance\x18\x03 \x01(\x02\x12\x19\n\x11number_of_objects\x18\x04 \x01(\x03\x12*\n\x07objects\x18\x05 \x03(\x0b\x32\x19.weaviate.v1.SearchResult\x12-\n\x06rerank\x18\x06 \x01(\x0b\x32\x18.weaviate.v1.RerankReplyH\x00\x88\x01\x01\x12\x35\n\ngenerative\x18\x07 \x01(\x0b\x32\x1c.weaviate.v1.GenerativeReplyH\x01\x88\x01\x01\x42\t\n\x07_rerankB\r\n\x0b_generative"p\n\x0cSearchResult\x12\x31\n\nproperties\x18\x01 \x01(\x0b\x32\x1d.weaviate.v1.PropertiesResult\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.weaviate.v1.MetadataResult"\xef\x04\n\x0eMetadataResult\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\x06vector\x18\x02 \x03(\x02\x42\x02\x18\x01\x12\x1a\n\x12\x63reation_time_unix\x18\x03 \x01(\x03\x12"\n\x1a\x63reation_time_unix_present\x18\x04 \x01(\x08\x12\x1d\n\x15last_update_time_unix\x18\x05 \x01(\x03\x12%\n\x1dlast_update_time_unix_present\x18\x06 \x01(\x08\x12\x10\n\x08\x64istance\x18\x07 \x01(\x02\x12\x18\n\x10\x64istance_present\x18\x08 \x01(\x08\x12\x11\n\tcertainty\x18\t \x01(\x02\x12\x19\n\x11\x63\x65rtainty_present\x18\n \x01(\x08\x12\r\n\x05score\x18\x0b \x01(\x02\x12\x15\n\rscore_present\x18\x0c \x01(\x08\x12\x15\n\rexplain_score\x18\r \x01(\t\x12\x1d\n\x15\x65xplain_score_present\x18\x0e \x01(\x08\x12\x1a\n\ris_consistent\x18\x0f \x01(\x08H\x00\x88\x01\x01\x12\x12\n\ngenerative\x18\x10 \x01(\t\x12\x1a\n\x12generative_present\x18\x11 \x01(\x08\x12\x1d\n\x15is_consistent_present\x18\x12 \x01(\x08\x12\x14\n\x0cvector_bytes\x18\x13 \x01(\x0c\x12\x13\n\x0bid_as_bytes\x18\x14 \x01(\x0c\x12\x14\n\x0crerank_score\x18\x15 \x01(\x01\x12\x1c\n\x14rerank_score_present\x18\x16 \x01(\x08\x12%\n\x07vectors\x18\x17 \x03(\x0b\x32\x14.weaviate.v1.VectorsB\x10\n\x0e_is_consistent"\xba\x05\n\x10PropertiesResult\x12\x37\n\x12non_ref_properties\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01\x12\x33\n\tref_props\x18\x02 \x03(\x0b\x32 .weaviate.v1.RefPropertiesResult\x12\x19\n\x11target_collection\x18\x03 \x01(\t\x12-\n\x08metadata\x18\x04 \x01(\x0b\x32\x1b.weaviate.v1.MetadataResult\x12G\n\x17number_array_properties\x18\x05 \x03(\x0b\x32".weaviate.v1.NumberArrayPropertiesB\x02\x18\x01\x12\x41\n\x14int_array_properties\x18\x06 \x03(\x0b\x32\x1f.weaviate.v1.IntArrayPropertiesB\x02\x18\x01\x12\x43\n\x15text_array_properties\x18\x07 \x03(\x0b\x32 .weaviate.v1.TextArrayPropertiesB\x02\x18\x01\x12I\n\x18\x62oolean_array_properties\x18\x08 \x03(\x0b\x32#.weaviate.v1.BooleanArrayPropertiesB\x02\x18\x01\x12<\n\x11object_properties\x18\t \x03(\x0b\x32\x1d.weaviate.v1.ObjectPropertiesB\x02\x18\x01\x12G\n\x17object_array_properties\x18\n \x03(\x0b\x32".weaviate.v1.ObjectArrayPropertiesB\x02\x18\x01\x12.\n\rnon_ref_props\x18\x0b \x01(\x0b\x32\x17.weaviate.v1.Properties\x12\x1b\n\x13ref_props_requested\x18\x0c \x01(\x08"[\n\x13RefPropertiesResult\x12\x31\n\nproperties\x18\x01 \x03(\x0b\x32\x1d.weaviate.v1.PropertiesResult\x12\x11\n\tprop_name\x18\x02 \x01(\tBs\n#io.weaviate.client.grpc.protocol.v1B\x16WeaviateProtoSearchGetZ4github.com/weaviate/weaviate/grpc/generated;protocolb\x06proto3'
+    b'\n\x13v1/search_get.proto\x12\x0bweaviate.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\rv1/base.proto\x1a\x13v1/properties.proto"\x82\x0b\n\rSearchRequest\x12\x12\n\ncollection\x18\x01 \x01(\t\x12\x0e\n\x06tenant\x18\n \x01(\t\x12=\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32\x1d.weaviate.v1.ConsistencyLevelH\x00\x88\x01\x01\x12\x37\n\nproperties\x18\x14 \x01(\x0b\x32\x1e.weaviate.v1.PropertiesRequestH\x01\x88\x01\x01\x12\x33\n\x08metadata\x18\x15 \x01(\x0b\x32\x1c.weaviate.v1.MetadataRequestH\x02\x88\x01\x01\x12+\n\x08group_by\x18\x16 \x01(\x0b\x32\x14.weaviate.v1.GroupByH\x03\x88\x01\x01\x12\r\n\x05limit\x18\x1e \x01(\r\x12\x0e\n\x06offset\x18\x1f \x01(\r\x12\x0f\n\x07\x61utocut\x18  \x01(\r\x12\r\n\x05\x61\x66ter\x18! \x01(\t\x12$\n\x07sort_by\x18" \x03(\x0b\x32\x13.weaviate.v1.SortBy\x12*\n\x07\x66ilters\x18( \x01(\x0b\x32\x14.weaviate.v1.FiltersH\x04\x88\x01\x01\x12/\n\rhybrid_search\x18) \x01(\x0b\x32\x13.weaviate.v1.HybridH\x05\x88\x01\x01\x12+\n\x0b\x62m25_search\x18* \x01(\x0b\x32\x11.weaviate.v1.BM25H\x06\x88\x01\x01\x12\x31\n\x0bnear_vector\x18+ \x01(\x0b\x32\x17.weaviate.v1.NearVectorH\x07\x88\x01\x01\x12\x31\n\x0bnear_object\x18, \x01(\x0b\x32\x17.weaviate.v1.NearObjectH\x08\x88\x01\x01\x12\x33\n\tnear_text\x18- \x01(\x0b\x32\x1b.weaviate.v1.NearTextSearchH\t\x88\x01\x01\x12\x35\n\nnear_image\x18. \x01(\x0b\x32\x1c.weaviate.v1.NearImageSearchH\n\x88\x01\x01\x12\x35\n\nnear_audio\x18/ \x01(\x0b\x32\x1c.weaviate.v1.NearAudioSearchH\x0b\x88\x01\x01\x12\x35\n\nnear_video\x18\x30 \x01(\x0b\x32\x1c.weaviate.v1.NearVideoSearchH\x0c\x88\x01\x01\x12\x35\n\nnear_depth\x18\x31 \x01(\x0b\x32\x1c.weaviate.v1.NearDepthSearchH\r\x88\x01\x01\x12\x39\n\x0cnear_thermal\x18\x32 \x01(\x0b\x32\x1e.weaviate.v1.NearThermalSearchH\x0e\x88\x01\x01\x12\x31\n\x08near_imu\x18\x33 \x01(\x0b\x32\x1a.weaviate.v1.NearIMUSearchH\x0f\x88\x01\x01\x12\x36\n\ngenerative\x18< \x01(\x0b\x32\x1d.weaviate.v1.GenerativeSearchH\x10\x88\x01\x01\x12(\n\x06rerank\x18= \x01(\x0b\x32\x13.weaviate.v1.RerankH\x11\x88\x01\x01\x12\x18\n\x0cuses_123_api\x18\x64 \x01(\x08\x42\x02\x18\x01\x12\x14\n\x0cuses_125_api\x18\x65 \x01(\x08\x42\x14\n\x12_consistency_levelB\r\n\x0b_propertiesB\x0b\n\t_metadataB\x0b\n\t_group_byB\n\n\x08_filtersB\x10\n\x0e_hybrid_searchB\x0e\n\x0c_bm25_searchB\x0e\n\x0c_near_vectorB\x0e\n\x0c_near_objectB\x0c\n\n_near_textB\r\n\x0b_near_imageB\r\n\x0b_near_audioB\r\n\x0b_near_videoB\r\n\x0b_near_depthB\x0f\n\r_near_thermalB\x0b\n\t_near_imuB\r\n\x0b_generativeB\t\n\x07_rerank"L\n\x07GroupBy\x12\x0c\n\x04path\x18\x01 \x03(\t\x12\x18\n\x10number_of_groups\x18\x02 \x01(\x05\x12\x19\n\x11objects_per_group\x18\x03 \x01(\x05")\n\x06SortBy\x12\x11\n\tascending\x18\x01 \x01(\x08\x12\x0c\n\x04path\x18\x02 \x03(\t"m\n\x10GenerativeSearch\x12\x1e\n\x16single_response_prompt\x18\x01 \x01(\t\x12\x1d\n\x15grouped_response_task\x18\x02 \x01(\t\x12\x1a\n\x12grouped_properties\x18\x03 \x03(\t"\xdd\x01\n\x0fMetadataRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\x08\x12\x0e\n\x06vector\x18\x02 \x01(\x08\x12\x1a\n\x12\x63reation_time_unix\x18\x03 \x01(\x08\x12\x1d\n\x15last_update_time_unix\x18\x04 \x01(\x08\x12\x10\n\x08\x64istance\x18\x05 \x01(\x08\x12\x11\n\tcertainty\x18\x06 \x01(\x08\x12\r\n\x05score\x18\x07 \x01(\x08\x12\x15\n\rexplain_score\x18\x08 \x01(\x08\x12\x15\n\ris_consistent\x18\t \x01(\x08\x12\x0f\n\x07vectors\x18\n \x03(\t"\xd1\x01\n\x11PropertiesRequest\x12\x1a\n\x12non_ref_properties\x18\x01 \x03(\t\x12\x39\n\x0eref_properties\x18\x02 \x03(\x0b\x32!.weaviate.v1.RefPropertiesRequest\x12?\n\x11object_properties\x18\x03 \x03(\x0b\x32$.weaviate.v1.ObjectPropertiesRequest\x12$\n\x1creturn_all_nonref_properties\x18\x0b \x01(\x08"\x8b\x01\n\x17ObjectPropertiesRequest\x12\x11\n\tprop_name\x18\x01 \x01(\t\x12\x1c\n\x14primitive_properties\x18\x02 \x03(\t\x12?\n\x11object_properties\x18\x03 \x03(\x0b\x32$.weaviate.v1.ObjectPropertiesRequest"\xf2\x02\n\x06Hybrid\x12\r\n\x05query\x18\x01 \x01(\t\x12\x12\n\nproperties\x18\x02 \x03(\t\x12\x12\n\x06vector\x18\x03 \x03(\x02\x42\x02\x18\x01\x12\r\n\x05\x61lpha\x18\x04 \x01(\x02\x12\x33\n\x0b\x66usion_type\x18\x05 \x01(\x0e\x32\x1e.weaviate.v1.Hybrid.FusionType\x12\x14\n\x0cvector_bytes\x18\x06 \x01(\x0c\x12\x16\n\x0etarget_vectors\x18\x07 \x03(\t\x12.\n\tnear_text\x18\x08 \x01(\x0b\x32\x1b.weaviate.v1.NearTextSearch\x12,\n\x0bnear_vector\x18\t \x01(\x0b\x32\x17.weaviate.v1.NearVector"a\n\nFusionType\x12\x1b\n\x17\x46USION_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x46USION_TYPE_RANKED\x10\x01\x12\x1e\n\x1a\x46USION_TYPE_RELATIVE_SCORE\x10\x02"\xc5\x02\n\x0eNearTextSearch\x12\r\n\x05query\x18\x01 \x03(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x36\n\x07move_to\x18\x04 \x01(\x0b\x32 .weaviate.v1.NearTextSearch.MoveH\x02\x88\x01\x01\x12\x38\n\tmove_away\x18\x05 \x01(\x0b\x32 .weaviate.v1.NearTextSearch.MoveH\x03\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x06 \x03(\t\x1a\x36\n\x04Move\x12\r\n\x05\x66orce\x18\x01 \x01(\x02\x12\x10\n\x08\x63oncepts\x18\x02 \x03(\t\x12\r\n\x05uuids\x18\x03 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distanceB\n\n\x08_move_toB\x0c\n\n_move_away"\x82\x01\n\x0fNearImageSearch\x12\r\n\x05image\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"\x82\x01\n\x0fNearAudioSearch\x12\r\n\x05\x61udio\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"\x82\x01\n\x0fNearVideoSearch\x12\r\n\x05video\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"\x82\x01\n\x0fNearDepthSearch\x12\r\n\x05\x64\x65pth\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"\x86\x01\n\x11NearThermalSearch\x12\x0f\n\x07thermal\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"~\n\rNearIMUSearch\x12\x0b\n\x03imu\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance")\n\x04\x42M25\x12\r\n\x05query\x18\x01 \x01(\t\x12\x12\n\nproperties\x18\x02 \x03(\t"\xb1\x01\n\x14RefPropertiesRequest\x12\x1a\n\x12reference_property\x18\x01 \x01(\t\x12\x32\n\nproperties\x18\x02 \x01(\x0b\x32\x1e.weaviate.v1.PropertiesRequest\x12.\n\x08metadata\x18\x03 \x01(\x0b\x32\x1c.weaviate.v1.MetadataRequest\x12\x19\n\x11target_collection\x18\x04 \x01(\t"\x98\x01\n\nNearVector\x12\x12\n\x06vector\x18\x01 \x03(\x02\x42\x02\x18\x01\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x14\n\x0cvector_bytes\x18\x04 \x01(\x0c\x12\x16\n\x0etarget_vectors\x18\x05 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"z\n\nNearObject\x12\n\n\x02id\x18\x01 \x01(\t\x12\x16\n\tcertainty\x18\x02 \x01(\x01H\x00\x88\x01\x01\x12\x15\n\x08\x64istance\x18\x03 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0etarget_vectors\x18\x04 \x03(\tB\x0c\n\n_certaintyB\x0b\n\t_distance"8\n\x06Rerank\x12\x10\n\x08property\x18\x01 \x01(\t\x12\x12\n\x05query\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_query"\xc3\x01\n\x0bSearchReply\x12\x0c\n\x04took\x18\x01 \x01(\x02\x12*\n\x07results\x18\x02 \x03(\x0b\x32\x19.weaviate.v1.SearchResult\x12&\n\x19generative_grouped_result\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x34\n\x10group_by_results\x18\x04 \x03(\x0b\x32\x1a.weaviate.v1.GroupByResultB\x1c\n\x1a_generative_grouped_result"\x1c\n\x0bRerankReply\x12\r\n\x05score\x18\x01 \x01(\x01"!\n\x0fGenerativeReply\x12\x0e\n\x06result\x18\x01 \x01(\t"\x90\x02\n\rGroupByResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0cmin_distance\x18\x02 \x01(\x02\x12\x14\n\x0cmax_distance\x18\x03 \x01(\x02\x12\x19\n\x11number_of_objects\x18\x04 \x01(\x03\x12*\n\x07objects\x18\x05 \x03(\x0b\x32\x19.weaviate.v1.SearchResult\x12-\n\x06rerank\x18\x06 \x01(\x0b\x32\x18.weaviate.v1.RerankReplyH\x00\x88\x01\x01\x12\x35\n\ngenerative\x18\x07 \x01(\x0b\x32\x1c.weaviate.v1.GenerativeReplyH\x01\x88\x01\x01\x42\t\n\x07_rerankB\r\n\x0b_generative"p\n\x0cSearchResult\x12\x31\n\nproperties\x18\x01 \x01(\x0b\x32\x1d.weaviate.v1.PropertiesResult\x12-\n\x08metadata\x18\x02 \x01(\x0b\x32\x1b.weaviate.v1.MetadataResult"\xef\x04\n\x0eMetadataResult\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\x06vector\x18\x02 \x03(\x02\x42\x02\x18\x01\x12\x1a\n\x12\x63reation_time_unix\x18\x03 \x01(\x03\x12"\n\x1a\x63reation_time_unix_present\x18\x04 \x01(\x08\x12\x1d\n\x15last_update_time_unix\x18\x05 \x01(\x03\x12%\n\x1dlast_update_time_unix_present\x18\x06 \x01(\x08\x12\x10\n\x08\x64istance\x18\x07 \x01(\x02\x12\x18\n\x10\x64istance_present\x18\x08 \x01(\x08\x12\x11\n\tcertainty\x18\t \x01(\x02\x12\x19\n\x11\x63\x65rtainty_present\x18\n \x01(\x08\x12\r\n\x05score\x18\x0b \x01(\x02\x12\x15\n\rscore_present\x18\x0c \x01(\x08\x12\x15\n\rexplain_score\x18\r \x01(\t\x12\x1d\n\x15\x65xplain_score_present\x18\x0e \x01(\x08\x12\x1a\n\ris_consistent\x18\x0f \x01(\x08H\x00\x88\x01\x01\x12\x12\n\ngenerative\x18\x10 \x01(\t\x12\x1a\n\x12generative_present\x18\x11 \x01(\x08\x12\x1d\n\x15is_consistent_present\x18\x12 \x01(\x08\x12\x14\n\x0cvector_bytes\x18\x13 \x01(\x0c\x12\x13\n\x0bid_as_bytes\x18\x14 \x01(\x0c\x12\x14\n\x0crerank_score\x18\x15 \x01(\x01\x12\x1c\n\x14rerank_score_present\x18\x16 \x01(\x08\x12%\n\x07vectors\x18\x17 \x03(\x0b\x32\x14.weaviate.v1.VectorsB\x10\n\x0e_is_consistent"\xba\x05\n\x10PropertiesResult\x12\x37\n\x12non_ref_properties\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructB\x02\x18\x01\x12\x33\n\tref_props\x18\x02 \x03(\x0b\x32 .weaviate.v1.RefPropertiesResult\x12\x19\n\x11target_collection\x18\x03 \x01(\t\x12-\n\x08metadata\x18\x04 \x01(\x0b\x32\x1b.weaviate.v1.MetadataResult\x12G\n\x17number_array_properties\x18\x05 \x03(\x0b\x32".weaviate.v1.NumberArrayPropertiesB\x02\x18\x01\x12\x41\n\x14int_array_properties\x18\x06 \x03(\x0b\x32\x1f.weaviate.v1.IntArrayPropertiesB\x02\x18\x01\x12\x43\n\x15text_array_properties\x18\x07 \x03(\x0b\x32 .weaviate.v1.TextArrayPropertiesB\x02\x18\x01\x12I\n\x18\x62oolean_array_properties\x18\x08 \x03(\x0b\x32#.weaviate.v1.BooleanArrayPropertiesB\x02\x18\x01\x12<\n\x11object_properties\x18\t \x03(\x0b\x32\x1d.weaviate.v1.ObjectPropertiesB\x02\x18\x01\x12G\n\x17object_array_properties\x18\n \x03(\x0b\x32".weaviate.v1.ObjectArrayPropertiesB\x02\x18\x01\x12.\n\rnon_ref_props\x18\x0b \x01(\x0b\x32\x17.weaviate.v1.Properties\x12\x1b\n\x13ref_props_requested\x18\x0c \x01(\x08"[\n\x13RefPropertiesResult\x12\x31\n\nproperties\x18\x01 \x03(\x0b\x32\x1d.weaviate.v1.PropertiesResult\x12\x11\n\tprop_name\x18\x02 \x01(\tBs\n#io.weaviate.client.grpc.protocol.v1B\x16WeaviateProtoSearchGetZ4github.com/weaviate/weaviate/grpc/generated;protocolb\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.search_get_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     _globals["DESCRIPTOR"]._options = None
@@ -63,67 +63,67 @@
         "object_properties"
     ]._serialized_options = b"\030\001"
     _globals["_PROPERTIESRESULT"].fields_by_name["object_array_properties"]._options = None
     _globals["_PROPERTIESRESULT"].fields_by_name[
         "object_array_properties"
     ]._serialized_options = b"\030\001"
     _globals["_SEARCHREQUEST"]._serialized_start = 103
-    _globals["_SEARCHREQUEST"]._serialized_end = 1491
-    _globals["_GROUPBY"]._serialized_start = 1493
-    _globals["_GROUPBY"]._serialized_end = 1569
-    _globals["_SORTBY"]._serialized_start = 1571
-    _globals["_SORTBY"]._serialized_end = 1612
-    _globals["_GENERATIVESEARCH"]._serialized_start = 1614
-    _globals["_GENERATIVESEARCH"]._serialized_end = 1723
-    _globals["_METADATAREQUEST"]._serialized_start = 1726
-    _globals["_METADATAREQUEST"]._serialized_end = 1947
-    _globals["_PROPERTIESREQUEST"]._serialized_start = 1950
-    _globals["_PROPERTIESREQUEST"]._serialized_end = 2159
-    _globals["_OBJECTPROPERTIESREQUEST"]._serialized_start = 2162
-    _globals["_OBJECTPROPERTIESREQUEST"]._serialized_end = 2301
-    _globals["_HYBRID"]._serialized_start = 2304
-    _globals["_HYBRID"]._serialized_end = 2580
-    _globals["_HYBRID_FUSIONTYPE"]._serialized_start = 2483
-    _globals["_HYBRID_FUSIONTYPE"]._serialized_end = 2580
-    _globals["_NEARTEXTSEARCH"]._serialized_start = 2583
-    _globals["_NEARTEXTSEARCH"]._serialized_end = 2908
-    _globals["_NEARTEXTSEARCH_MOVE"]._serialized_start = 2801
-    _globals["_NEARTEXTSEARCH_MOVE"]._serialized_end = 2855
-    _globals["_NEARIMAGESEARCH"]._serialized_start = 2911
-    _globals["_NEARIMAGESEARCH"]._serialized_end = 3041
-    _globals["_NEARAUDIOSEARCH"]._serialized_start = 3044
-    _globals["_NEARAUDIOSEARCH"]._serialized_end = 3174
-    _globals["_NEARVIDEOSEARCH"]._serialized_start = 3177
-    _globals["_NEARVIDEOSEARCH"]._serialized_end = 3307
-    _globals["_NEARDEPTHSEARCH"]._serialized_start = 3310
-    _globals["_NEARDEPTHSEARCH"]._serialized_end = 3440
-    _globals["_NEARTHERMALSEARCH"]._serialized_start = 3443
-    _globals["_NEARTHERMALSEARCH"]._serialized_end = 3577
-    _globals["_NEARIMUSEARCH"]._serialized_start = 3579
-    _globals["_NEARIMUSEARCH"]._serialized_end = 3705
-    _globals["_BM25"]._serialized_start = 3707
-    _globals["_BM25"]._serialized_end = 3748
-    _globals["_REFPROPERTIESREQUEST"]._serialized_start = 3751
-    _globals["_REFPROPERTIESREQUEST"]._serialized_end = 3928
-    _globals["_NEARVECTOR"]._serialized_start = 3931
-    _globals["_NEARVECTOR"]._serialized_end = 4083
-    _globals["_NEAROBJECT"]._serialized_start = 4085
-    _globals["_NEAROBJECT"]._serialized_end = 4207
-    _globals["_RERANK"]._serialized_start = 4209
-    _globals["_RERANK"]._serialized_end = 4265
-    _globals["_SEARCHREPLY"]._serialized_start = 4268
-    _globals["_SEARCHREPLY"]._serialized_end = 4463
-    _globals["_RERANKREPLY"]._serialized_start = 4465
-    _globals["_RERANKREPLY"]._serialized_end = 4493
-    _globals["_GENERATIVEREPLY"]._serialized_start = 4495
-    _globals["_GENERATIVEREPLY"]._serialized_end = 4528
-    _globals["_GROUPBYRESULT"]._serialized_start = 4531
-    _globals["_GROUPBYRESULT"]._serialized_end = 4803
-    _globals["_SEARCHRESULT"]._serialized_start = 4805
-    _globals["_SEARCHRESULT"]._serialized_end = 4917
-    _globals["_METADATARESULT"]._serialized_start = 4920
-    _globals["_METADATARESULT"]._serialized_end = 5543
-    _globals["_PROPERTIESRESULT"]._serialized_start = 5546
-    _globals["_PROPERTIESRESULT"]._serialized_end = 6244
-    _globals["_REFPROPERTIESRESULT"]._serialized_start = 6246
-    _globals["_REFPROPERTIESRESULT"]._serialized_end = 6337
+    _globals["_SEARCHREQUEST"]._serialized_end = 1513
+    _globals["_GROUPBY"]._serialized_start = 1515
+    _globals["_GROUPBY"]._serialized_end = 1591
+    _globals["_SORTBY"]._serialized_start = 1593
+    _globals["_SORTBY"]._serialized_end = 1634
+    _globals["_GENERATIVESEARCH"]._serialized_start = 1636
+    _globals["_GENERATIVESEARCH"]._serialized_end = 1745
+    _globals["_METADATAREQUEST"]._serialized_start = 1748
+    _globals["_METADATAREQUEST"]._serialized_end = 1969
+    _globals["_PROPERTIESREQUEST"]._serialized_start = 1972
+    _globals["_PROPERTIESREQUEST"]._serialized_end = 2181
+    _globals["_OBJECTPROPERTIESREQUEST"]._serialized_start = 2184
+    _globals["_OBJECTPROPERTIESREQUEST"]._serialized_end = 2323
+    _globals["_HYBRID"]._serialized_start = 2326
+    _globals["_HYBRID"]._serialized_end = 2696
+    _globals["_HYBRID_FUSIONTYPE"]._serialized_start = 2599
+    _globals["_HYBRID_FUSIONTYPE"]._serialized_end = 2696
+    _globals["_NEARTEXTSEARCH"]._serialized_start = 2699
+    _globals["_NEARTEXTSEARCH"]._serialized_end = 3024
+    _globals["_NEARTEXTSEARCH_MOVE"]._serialized_start = 2917
+    _globals["_NEARTEXTSEARCH_MOVE"]._serialized_end = 2971
+    _globals["_NEARIMAGESEARCH"]._serialized_start = 3027
+    _globals["_NEARIMAGESEARCH"]._serialized_end = 3157
+    _globals["_NEARAUDIOSEARCH"]._serialized_start = 3160
+    _globals["_NEARAUDIOSEARCH"]._serialized_end = 3290
+    _globals["_NEARVIDEOSEARCH"]._serialized_start = 3293
+    _globals["_NEARVIDEOSEARCH"]._serialized_end = 3423
+    _globals["_NEARDEPTHSEARCH"]._serialized_start = 3426
+    _globals["_NEARDEPTHSEARCH"]._serialized_end = 3556
+    _globals["_NEARTHERMALSEARCH"]._serialized_start = 3559
+    _globals["_NEARTHERMALSEARCH"]._serialized_end = 3693
+    _globals["_NEARIMUSEARCH"]._serialized_start = 3695
+    _globals["_NEARIMUSEARCH"]._serialized_end = 3821
+    _globals["_BM25"]._serialized_start = 3823
+    _globals["_BM25"]._serialized_end = 3864
+    _globals["_REFPROPERTIESREQUEST"]._serialized_start = 3867
+    _globals["_REFPROPERTIESREQUEST"]._serialized_end = 4044
+    _globals["_NEARVECTOR"]._serialized_start = 4047
+    _globals["_NEARVECTOR"]._serialized_end = 4199
+    _globals["_NEAROBJECT"]._serialized_start = 4201
+    _globals["_NEAROBJECT"]._serialized_end = 4323
+    _globals["_RERANK"]._serialized_start = 4325
+    _globals["_RERANK"]._serialized_end = 4381
+    _globals["_SEARCHREPLY"]._serialized_start = 4384
+    _globals["_SEARCHREPLY"]._serialized_end = 4579
+    _globals["_RERANKREPLY"]._serialized_start = 4581
+    _globals["_RERANKREPLY"]._serialized_end = 4609
+    _globals["_GENERATIVEREPLY"]._serialized_start = 4611
+    _globals["_GENERATIVEREPLY"]._serialized_end = 4644
+    _globals["_GROUPBYRESULT"]._serialized_start = 4647
+    _globals["_GROUPBYRESULT"]._serialized_end = 4919
+    _globals["_SEARCHRESULT"]._serialized_start = 4921
+    _globals["_SEARCHRESULT"]._serialized_end = 5033
+    _globals["_METADATARESULT"]._serialized_start = 5036
+    _globals["_METADATARESULT"]._serialized_end = 5659
+    _globals["_PROPERTIESRESULT"]._serialized_start = 5662
+    _globals["_PROPERTIESRESULT"]._serialized_end = 6360
+    _globals["_REFPROPERTIESRESULT"]._serialized_start = 6362
+    _globals["_REFPROPERTIESRESULT"]._serialized_end = 6453
 # @@protoc_insertion_point(module_scope)
```

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/search_get_pb2.pyi` & `weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         "near_video",
         "near_depth",
         "near_thermal",
         "near_imu",
         "generative",
         "rerank",
         "uses_123_api",
+        "uses_125_api",
     )
     COLLECTION_FIELD_NUMBER: _ClassVar[int]
     TENANT_FIELD_NUMBER: _ClassVar[int]
     CONSISTENCY_LEVEL_FIELD_NUMBER: _ClassVar[int]
     PROPERTIES_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     GROUP_BY_FIELD_NUMBER: _ClassVar[int]
@@ -66,14 +67,15 @@
     NEAR_VIDEO_FIELD_NUMBER: _ClassVar[int]
     NEAR_DEPTH_FIELD_NUMBER: _ClassVar[int]
     NEAR_THERMAL_FIELD_NUMBER: _ClassVar[int]
     NEAR_IMU_FIELD_NUMBER: _ClassVar[int]
     GENERATIVE_FIELD_NUMBER: _ClassVar[int]
     RERANK_FIELD_NUMBER: _ClassVar[int]
     USES_123_API_FIELD_NUMBER: _ClassVar[int]
+    USES_125_API_FIELD_NUMBER: _ClassVar[int]
     collection: str
     tenant: str
     consistency_level: _base_pb2.ConsistencyLevel
     properties: PropertiesRequest
     metadata: MetadataRequest
     group_by: GroupBy
     limit: int
@@ -92,14 +94,15 @@
     near_video: NearVideoSearch
     near_depth: NearDepthSearch
     near_thermal: NearThermalSearch
     near_imu: NearIMUSearch
     generative: GenerativeSearch
     rerank: Rerank
     uses_123_api: bool
+    uses_125_api: bool
     def __init__(
         self,
         collection: _Optional[str] = ...,
         tenant: _Optional[str] = ...,
         consistency_level: _Optional[_Union[_base_pb2.ConsistencyLevel, str]] = ...,
         properties: _Optional[_Union[PropertiesRequest, _Mapping]] = ...,
         metadata: _Optional[_Union[MetadataRequest, _Mapping]] = ...,
@@ -120,14 +123,15 @@
         near_video: _Optional[_Union[NearVideoSearch, _Mapping]] = ...,
         near_depth: _Optional[_Union[NearDepthSearch, _Mapping]] = ...,
         near_thermal: _Optional[_Union[NearThermalSearch, _Mapping]] = ...,
         near_imu: _Optional[_Union[NearIMUSearch, _Mapping]] = ...,
         generative: _Optional[_Union[GenerativeSearch, _Mapping]] = ...,
         rerank: _Optional[_Union[Rerank, _Mapping]] = ...,
         uses_123_api: bool = ...,
+        uses_125_api: bool = ...,
     ) -> None: ...
 
 class GroupBy(_message.Message):
     __slots__ = ("path", "number_of_groups", "objects_per_group")
     PATH_FIELD_NUMBER: _ClassVar[int]
     NUMBER_OF_GROUPS_FIELD_NUMBER: _ClassVar[int]
     OBJECTS_PER_GROUP_FIELD_NUMBER: _ClassVar[int]
@@ -254,14 +258,16 @@
         "query",
         "properties",
         "vector",
         "alpha",
         "fusion_type",
         "vector_bytes",
         "target_vectors",
+        "near_text",
+        "near_vector",
     )
 
     class FusionType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         FUSION_TYPE_UNSPECIFIED: _ClassVar[Hybrid.FusionType]
         FUSION_TYPE_RANKED: _ClassVar[Hybrid.FusionType]
         FUSION_TYPE_RELATIVE_SCORE: _ClassVar[Hybrid.FusionType]
@@ -271,30 +277,36 @@
     QUERY_FIELD_NUMBER: _ClassVar[int]
     PROPERTIES_FIELD_NUMBER: _ClassVar[int]
     VECTOR_FIELD_NUMBER: _ClassVar[int]
     ALPHA_FIELD_NUMBER: _ClassVar[int]
     FUSION_TYPE_FIELD_NUMBER: _ClassVar[int]
     VECTOR_BYTES_FIELD_NUMBER: _ClassVar[int]
     TARGET_VECTORS_FIELD_NUMBER: _ClassVar[int]
+    NEAR_TEXT_FIELD_NUMBER: _ClassVar[int]
+    NEAR_VECTOR_FIELD_NUMBER: _ClassVar[int]
     query: str
     properties: _containers.RepeatedScalarFieldContainer[str]
     vector: _containers.RepeatedScalarFieldContainer[float]
     alpha: float
     fusion_type: Hybrid.FusionType
     vector_bytes: bytes
     target_vectors: _containers.RepeatedScalarFieldContainer[str]
+    near_text: NearTextSearch
+    near_vector: NearVector
     def __init__(
         self,
         query: _Optional[str] = ...,
         properties: _Optional[_Iterable[str]] = ...,
         vector: _Optional[_Iterable[float]] = ...,
         alpha: _Optional[float] = ...,
         fusion_type: _Optional[_Union[Hybrid.FusionType, str]] = ...,
         vector_bytes: _Optional[bytes] = ...,
         target_vectors: _Optional[_Iterable[str]] = ...,
+        near_text: _Optional[_Union[NearTextSearch, _Mapping]] = ...,
+        near_vector: _Optional[_Union[NearVector, _Mapping]] = ...,
     ) -> None: ...
 
 class NearTextSearch(_message.Message):
     __slots__ = ("query", "certainty", "distance", "move_to", "move_away", "target_vectors")
 
     class Move(_message.Message):
         __slots__ = ("force", "concepts", "uuids")
```

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2.py` & `weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from weaviate.proto.v1 import batch_pb2 as v1_dot_batch__pb2
 from weaviate.proto.v1 import batch_delete_pb2 as v1_dot_batch__delete__pb2
 from weaviate.proto.v1 import search_get_pb2 as v1_dot_search__get__pb2
+from weaviate.proto.v1 import tenants_pb2 as v1_dot_tenants__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x11v1/weaviate.proto\x12\x0bweaviate.v1\x1a\x0ev1/batch.proto\x1a\x15v1/batch_delete.proto\x1a\x13v1/search_get.proto2\xf1\x01\n\x08Weaviate\x12@\n\x06Search\x12\x1a.weaviate.v1.SearchRequest\x1a\x18.weaviate.v1.SearchReply"\x00\x12R\n\x0c\x42\x61tchObjects\x12 .weaviate.v1.BatchObjectsRequest\x1a\x1e.weaviate.v1.BatchObjectsReply"\x00\x12O\n\x0b\x42\x61tchDelete\x12\x1f.weaviate.v1.BatchDeleteRequest\x1a\x1d.weaviate.v1.BatchDeleteReply"\x00\x42j\n#io.weaviate.client.grpc.protocol.v1B\rWeaviateProtoZ4github.com/weaviate/weaviate/grpc/generated;protocolb\x06proto3'
+    b'\n\x11v1/weaviate.proto\x12\x0bweaviate.v1\x1a\x0ev1/batch.proto\x1a\x15v1/batch_delete.proto\x1a\x13v1/search_get.proto\x1a\x10v1/tenants.proto2\xbf\x02\n\x08Weaviate\x12@\n\x06Search\x12\x1a.weaviate.v1.SearchRequest\x1a\x18.weaviate.v1.SearchReply"\x00\x12R\n\x0c\x42\x61tchObjects\x12 .weaviate.v1.BatchObjectsRequest\x1a\x1e.weaviate.v1.BatchObjectsReply"\x00\x12O\n\x0b\x42\x61tchDelete\x12\x1f.weaviate.v1.BatchDeleteRequest\x1a\x1d.weaviate.v1.BatchDeleteReply"\x00\x12L\n\nTenantsGet\x12\x1e.weaviate.v1.TenantsGetRequest\x1a\x1c.weaviate.v1.TenantsGetReply"\x00\x42j\n#io.weaviate.client.grpc.protocol.v1B\rWeaviateProtoZ4github.com/weaviate/weaviate/grpc/generated;protocolb\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.weaviate_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     _globals["DESCRIPTOR"]._options = None
     _globals[
         "DESCRIPTOR"
     ]._serialized_options = b"\n#io.weaviate.client.grpc.protocol.v1B\rWeaviateProtoZ4github.com/weaviate/weaviate/grpc/generated;protocol"
-    _globals["_WEAVIATE"]._serialized_start = 95
-    _globals["_WEAVIATE"]._serialized_end = 336
+    _globals["_WEAVIATE"]._serialized_start = 113
+    _globals["_WEAVIATE"]._serialized_end = 432
 # @@protoc_insertion_point(module_scope)
```

### Comparing `weaviate-client-4.5rc0/weaviate/proto/v1/weaviate_pb2_grpc.py` & `weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2_grpc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from weaviate.proto.v1 import batch_delete_pb2 as v1_dot_batch__delete__pb2
 from weaviate.proto.v1 import batch_pb2 as v1_dot_batch__pb2
 from weaviate.proto.v1 import search_get_pb2 as v1_dot_search__get__pb2
+from weaviate.proto.v1 import tenants_pb2 as v1_dot_tenants__pb2
 
 
 class WeaviateStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
@@ -27,14 +28,19 @@
             response_deserializer=v1_dot_batch__pb2.BatchObjectsReply.FromString,
         )
         self.BatchDelete = channel.unary_unary(
             "/weaviate.v1.Weaviate/BatchDelete",
             request_serializer=v1_dot_batch__delete__pb2.BatchDeleteRequest.SerializeToString,
             response_deserializer=v1_dot_batch__delete__pb2.BatchDeleteReply.FromString,
         )
+        self.TenantsGet = channel.unary_unary(
+            "/weaviate.v1.Weaviate/TenantsGet",
+            request_serializer=v1_dot_tenants__pb2.TenantsGetRequest.SerializeToString,
+            response_deserializer=v1_dot_tenants__pb2.TenantsGetReply.FromString,
+        )
 
 
 class WeaviateServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Search(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -50,14 +56,20 @@
 
     def BatchDelete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def TenantsGet(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
 
 def add_WeaviateServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "Search": grpc.unary_unary_rpc_method_handler(
             servicer.Search,
             request_deserializer=v1_dot_search__get__pb2.SearchRequest.FromString,
             response_serializer=v1_dot_search__get__pb2.SearchReply.SerializeToString,
@@ -68,14 +80,19 @@
             response_serializer=v1_dot_batch__pb2.BatchObjectsReply.SerializeToString,
         ),
         "BatchDelete": grpc.unary_unary_rpc_method_handler(
             servicer.BatchDelete,
             request_deserializer=v1_dot_batch__delete__pb2.BatchDeleteRequest.FromString,
             response_serializer=v1_dot_batch__delete__pb2.BatchDeleteReply.SerializeToString,
         ),
+        "TenantsGet": grpc.unary_unary_rpc_method_handler(
+            servicer.TenantsGet,
+            request_deserializer=v1_dot_tenants__pb2.TenantsGetRequest.FromString,
+            response_serializer=v1_dot_tenants__pb2.TenantsGetReply.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         "weaviate.v1.Weaviate", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -163,9 +180,38 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def TenantsGet(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/weaviate.v1.Weaviate/TenantsGet",
+            v1_dot_tenants__pb2.TenantsGetRequest.SerializeToString,
+            v1_dot_tenants__pb2.TenantsGetReply.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
```

### Comparing `weaviate-client-4.5rc0/weaviate/schema/crud_schema.py` & `weaviate_client-4.6.0b0/weaviate/schema/crud_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/schema/properties/crud_properties.py` & `weaviate_client-4.6.0b0/weaviate/schema/properties/crud_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/types.py` & `weaviate_client-4.6.0b0/weaviate/types.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/util.py` & `weaviate_client-4.6.0b0/weaviate/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 from enum import Enum, EnumMeta
 from pathlib import Path
 from typing import Union, Sequence, Any, Optional, List, Dict, Generator, Tuple, cast
 
 import requests
 import httpx
 import uuid as uuid_lib
-import validators  # type: ignore
+import validators
 from requests.exceptions import JSONDecodeError
 
 from weaviate.exceptions import (
     SchemaValidationError,
     UnexpectedStatusCodeError,
     ResponseCannotBeDecodedError,
     WeaviateInvalidInputError,
+    WeaviateUnsupportedFeatureError,
 )
 from weaviate.warnings import _Warnings
 from weaviate.types import NUMBER, UUIDS, TIME
 
 PYPI_PACKAGE_URL = "https://pypi.org/pypi/weaviate-client/json"
 MAXIMUM_MINOR_VERSION_DELTA = 3  # The maximum delta between minor versions of Weaviate Client that will not trigger an upgrade warning.
 MINIMUM_NO_WARNING_VERSION = (
@@ -121,43 +122,48 @@
             data = buffer.read(chunk_size)
             if not data:
                 break
             yield data
 
     should_close_file = False
     use_buffering = True
+    file = None
 
-    if isinstance(file_or_file_path, str):
-        if not os.path.isfile(file_or_file_path):
-            raise ValueError("No file found at location " + file_or_file_path)
-        file = open(file_or_file_path, "br")
-        should_close_file = True
-        use_buffering = os.path.getsize(file_or_file_path) > BYTES_PER_CHUNK
-    elif isinstance(file_or_file_path, Path):
-        if not file_or_file_path.is_file():
-            raise ValueError("No file found at location " + str(file_or_file_path))
-        file = file_or_file_path.open("br")
-        should_close_file = True
-        use_buffering = file_or_file_path.stat().st_size > BYTES_PER_CHUNK
-    elif isinstance(file_or_file_path, io.BufferedReader):
-        file = file_or_file_path
-    else:
-        raise TypeError(
-            '"file_or_file_path" should be a file path or a binary read file' " (io.BufferedReader)"
-        )
+    try:
+        if isinstance(file_or_file_path, str):
+            if not os.path.isfile(file_or_file_path):
+                raise ValueError("No file found at location " + file_or_file_path)
+            file = open(file_or_file_path, "br")
+            should_close_file = True
+            use_buffering = os.path.getsize(file_or_file_path) > BYTES_PER_CHUNK
+        elif isinstance(file_or_file_path, Path):
+            if not file_or_file_path.is_file():
+                raise ValueError("No file found at location " + str(file_or_file_path))
+            file = file_or_file_path.open("br")
+            should_close_file = True
+            use_buffering = file_or_file_path.stat().st_size > BYTES_PER_CHUNK
+        elif isinstance(file_or_file_path, io.BufferedReader):
+            file = file_or_file_path
+        else:
+            raise TypeError(
+                '"file_or_file_path" should be a file path or a binary read file'
+                " (io.BufferedReader)"
+            )
 
-    if use_buffering:
-        encoded: str = ""
-        for chunk in _chunks(file, BYTES_PER_CHUNK):
-            encoded += base64.b64encode(chunk).decode("utf-8")
-    else:
-        encoded = base64.b64encode(file.read()).decode("utf-8")
+        if use_buffering:
+            encoded: str = ""
+            for chunk in _chunks(file, BYTES_PER_CHUNK):
+                encoded += base64.b64encode(chunk).decode("utf-8")
+        else:
+            encoded = base64.b64encode(file.read()).decode("utf-8")
+
+    finally:
+        if should_close_file and file is not None:
+            file.close()
 
-    if should_close_file:
-        file.close()
     return encoded
 
 
 def image_decoder_b64(encoded_image: str) -> bytes:
     """
     Decode image from a Weaviate format image.
 
@@ -453,15 +459,17 @@
     ) from None
 
 
 def _get_vector_v4(vector: Sequence) -> List[float]:
     try:
         return get_vector(vector)
     except TypeError as e:
-        raise WeaviateInvalidInputError("") from e
+        raise WeaviateInvalidInputError(
+            f"The vector you supplied was malformatted! Vector:  {vector}"
+        ) from e
 
 
 def get_domain_from_weaviate_url(url: str) -> str:
     """
     Get the domain from a weaviate URL.
 
     Parameters
@@ -789,14 +797,22 @@
             ver_tup = tuple(map(int, match.groups()))
             return cls(major=ver_tup[0], minor=ver_tup[1], patch=ver_tup[2])
         else:
             raise ValueError(
                 f"Unable to parse a version from the input string: {initial}. Is it in the format '(v)x.y.z' (e.g. 'v1.18.2' or '1.18.0')?"
             )
 
+    def check_is_at_least_1_25_0(self, feature: str) -> None:
+        if not self >= _ServerVersion(1, 25, 0):
+            raise WeaviateUnsupportedFeatureError(feature, str(self), "1.25.0")
+
+    @property
+    def supports_tenants_get_grpc(self) -> bool:
+        return self >= _ServerVersion(1, 25, 0)
+
 
 def is_weaviate_too_old(current_version_str: str) -> bool:
     """
     Check if the user should be gently nudged to upgrade their Weaviate server version.
 
     Parameters
     ----------
```

### Comparing `weaviate-client-4.5rc0/weaviate/validator.py` & `weaviate_client-4.6.0b0/weaviate/validator.py`

 * *Files identical despite different names*

### Comparing `weaviate-client-4.5rc0/weaviate/warnings.py` & `weaviate_client-4.6.0b0/weaviate/warnings.py`

 * *Files 9% similar despite different names*

```diff
@@ -171,14 +171,31 @@
             Please instead use the `vectorizer_config` argument instead.
             """,
             category=DeprecationWarning,
             stacklevel=1,
         )
 
     @staticmethod
+    def sharding_actual_count_is_deprecated(argument: str) -> None:
+        warnings.warn(
+            message=f"""Dep018: You are using the {argument} argument in the `Configure.sharding` method, which is deprecated.
+            This field is read-only so has no effect and as such is deprecated. It will be removed in a future release.""",
+            category=DeprecationWarning,
+            stacklevel=1,
+        )
+
+    @staticmethod
+    def bit_compression_in_pq_config() -> None:
+        warnings.warn(
+            message="""Dep018: The `bit_compression` argument in `PQConfig` is deprecated and will be removed by Q4 2024.""",
+            category=DeprecationWarning,
+            stacklevel=1,
+        )
+
+    @staticmethod
     def datetime_insertion_with_no_specified_timezone(date: datetime) -> None:
         warnings.warn(
             message=f"""Con002: You are inserting the datetime object {date} without a timezone. The timezone will be set to UTC.
             If you want to use a different timezone, please specify it in the datetime object. For example:
             datetime.datetime(2021, 1, 1, 0, 0, 0, tzinfo=datetime.timezone(-datetime.timedelta(hours=2))).isoformat() = 2021-01-01T00:00:00-02:00
             """,
             category=UserWarning,
```

### Comparing `weaviate-client-4.5rc0/weaviate_client.egg-info/PKG-INFO` & `weaviate_client-4.6.0b0/weaviate_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.5rc0
+Version: 4.6.0b0
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
 Project-URL: Tracker, https://github.com/weaviate/weaviate-python-client/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 Requires-Dist: requests<3.0.0,>=2.30.0
-Requires-Dist: httpx==0.27.0
-Requires-Dist: validators==0.22.0
+Requires-Dist: httpx<=0.27.0,>=0.25.0
+Requires-Dist: validators==0.28.1
 Requires-Dist: authlib<2.0.0,>=1.2.1
 Requires-Dist: pydantic<3.0.0,>=2.5.0
 Requires-Dist: grpcio<2.0.0,>=1.57.0
 Requires-Dist: grpcio-tools<2.0.0,>=1.57.0
 Requires-Dist: grpcio-health-checking<2.0.0,>=1.57.0
 
 Weaviate python client
```

### Comparing `weaviate-client-4.5rc0/weaviate_client.egg-info/SOURCES.txt` & `weaviate_client-4.6.0b0/weaviate_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,28 @@
 requirements-devel.txt
 run-mypy.sh
 setup.cfg
 setup.py
 .github/CODEOWNERS
 .github/dependabot.yml
 .github/workflows/main.yaml
+ci/compose.sh
 ci/docker-compose-async.yml
 ci/docker-compose-azure.yml
 ci/docker-compose-cluster.yml
 ci/docker-compose-generative.yml
 ci/docker-compose-okta-cc.yml
 ci/docker-compose-okta-users.yml
+ci/docker-compose-proxy.yml
 ci/docker-compose-rerank.yml
 ci/docker-compose-wcs.yml
 ci/docker-compose.yml
 ci/start_weaviate.sh
 ci/stop_weaviate.sh
+ci/proxy/envoy.yaml
 docs/Makefile
 docs/README.rst
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/modules.rst
@@ -83,15 +86,18 @@
 integration/test_collection_nested.py
 integration/test_collection_openai.py
 integration/test_collection_references.py
 integration/test_collection_rerank.py
 integration/test_gql_raw_v4.py
 integration/test_iterator.py
 integration/test_named_vectors.py
+integration/test_tenants.py
 integration/weaviate-logo.png
+integration_embedded/__init__.py
+integration_embedded/test_client.py
 integration_v3/__init__.py
 integration_v3/people_schema.json
 integration_v3/test_authentication.py
 integration_v3/test_backup.py
 integration_v3/test_backup_v4.py
 integration_v3/test_batch.py
 integration_v3/test_classification.py
@@ -110,14 +116,15 @@
 mock_tests/test_collection.py
 mock_tests/test_connection.py
 mock_tests/test_exception.py
 mock_tests/test_graphql.py
 mock_tests/test_resend.py
 mock_tests/test_schema.py
 profiling/__init__.py
+profiling/conftest.py
 profiling/constants.py
 profiling/test_import_and_query.py
 profiling/test_profiling.py
 profiling/test_refs.py
 profiling/test_sphere.py
 test/README.md
 test/__init__.py
@@ -133,18 +140,20 @@
 test/classification/__init__.py
 test/classification/test_classification.py
 test/cluster/__init__.py
 test/cluster/test_cluster.py
 test/collection/__init__.py
 test/collection/conftest.py
 test/collection/test_aggregates.py
+test/collection/test_byteops.py
 test/collection/test_classes.py
 test/collection/test_client.py
 test/collection/test_collection_model.py
 test/collection/test_config.py
+test/collection/test_filter.py
 test/collection/test_queries.py
 test/connection/__init__.py
 test/connection/test_connection.py
 test/contextionary/__init__.py
 test/contextionary/test_text2vec_contextionary.py
 test/data/__init__.py
 test/data/test_crud_data.py
@@ -166,25 +175,27 @@
 weaviate/auth.py
 weaviate/client.py
 weaviate/config.py
 weaviate/conftest.py
 weaviate/embedded.py
 weaviate/error_msgs.py
 weaviate/exceptions.py
+weaviate/integrations.py
 weaviate/types.py
 weaviate/util.py
 weaviate/validator.py
 weaviate/warnings.py
 weaviate/backup/__init__.py
 weaviate/backup/backup.py
 weaviate/batch/__init__.py
 weaviate/batch/crud_batch.py
 weaviate/batch/requests.py
 weaviate/classes/__init__.py
 weaviate/classes/aggregate.py
+weaviate/classes/backup.py
 weaviate/classes/batch.py
 weaviate/classes/config.py
 weaviate/classes/data.py
 weaviate/classes/generics.py
 weaviate/classes/init.py
 weaviate/classes/query.py
 weaviate/classes/tenants.py
@@ -206,14 +217,15 @@
 weaviate/collections/filters.py
 weaviate/collections/iterator.py
 weaviate/collections/orm.py
 weaviate/collections/query.py
 weaviate/collections/tenants.py
 weaviate/collections/aggregations/__init__.py
 weaviate/collections/aggregations/base.py
+weaviate/collections/aggregations/hybrid.py
 weaviate/collections/aggregations/near_image.py
 weaviate/collections/aggregations/near_object.py
 weaviate/collections/aggregations/near_text.py
 weaviate/collections/aggregations/near_vector.py
 weaviate/collections/aggregations/over_all.py
 weaviate/collections/batch/__init__.py
 weaviate/collections/batch/base.py
@@ -239,16 +251,18 @@
 weaviate/collections/classes/internal.py
 weaviate/collections/classes/orm.py
 weaviate/collections/classes/tenants.py
 weaviate/collections/classes/types.py
 weaviate/collections/grpc/__init__.py
 weaviate/collections/grpc/query.py
 weaviate/collections/grpc/shared.py
+weaviate/collections/grpc/tenants.py
 weaviate/collections/queries/__init__.py
 weaviate/collections/queries/base.py
+weaviate/collections/queries/byteops.py
 weaviate/collections/queries/bm25/__init__.py
 weaviate/collections/queries/bm25/generate.py
 weaviate/collections/queries/bm25/generate.pyi
 weaviate/collections/queries/bm25/query.py
 weaviate/collections/queries/bm25/query.pyi
 weaviate/collections/queries/fetch_object_by_id/__init__.py
 weaviate/collections/queries/fetch_object_by_id/query.py
@@ -288,14 +302,15 @@
 weaviate/collections/queries/near_vector/generate.pyi
 weaviate/collections/queries/near_vector/query.py
 weaviate/collections/queries/near_vector/query.pyi
 weaviate/connect/__init__.py
 weaviate/connect/authentication.py
 weaviate/connect/base.py
 weaviate/connect/helpers.py
+weaviate/connect/integrations.py
 weaviate/connect/v3.py
 weaviate/connect/v4.py
 weaviate/contextionary/__init__.py
 weaviate/contextionary/crud_contextionary.py
 weaviate/data/__init__.py
 weaviate/data/crud_data.py
 weaviate/data/references/__init__.py
@@ -331,14 +346,17 @@
 weaviate/proto/v1/properties_pb2.py
 weaviate/proto/v1/properties_pb2.pyi
 weaviate/proto/v1/properties_pb2_grpc.py
 weaviate/proto/v1/regen.sh
 weaviate/proto/v1/search_get_pb2.py
 weaviate/proto/v1/search_get_pb2.pyi
 weaviate/proto/v1/search_get_pb2_grpc.py
+weaviate/proto/v1/tenants_pb2.py
+weaviate/proto/v1/tenants_pb2.pyi
+weaviate/proto/v1/tenants_pb2_grpc.py
 weaviate/proto/v1/weaviate_pb2.py
 weaviate/proto/v1/weaviate_pb2.pyi
 weaviate/proto/v1/weaviate_pb2_grpc.py
 weaviate/schema/__init__.py
 weaviate/schema/crud_schema.py
 weaviate/schema/properties/__init__.py
 weaviate/schema/properties/crud_properties.py
```


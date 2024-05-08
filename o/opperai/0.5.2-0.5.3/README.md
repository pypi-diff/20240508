# Comparing `tmp/opperai-0.5.2.tar.gz` & `tmp/opperai-0.5.3.tar.gz`

## Comparing `opperai-0.5.2.tar` & `opperai-0.5.3.tar`

### file list

```diff
@@ -1,83 +1,88 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.5.2/pytest.ini
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.5.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/__init__.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/_client.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/functions.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/indexes.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/spans.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/_http_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/__init__.py
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/_async_functions.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/decorator/__init__.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/decorator/_decorator.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/functions/decorator/_schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/indexes/__init__.py
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/indexes/_async_indexes.py
--rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/indexes/_indexes.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/spans/__init__.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/spans/_async_spans.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/spans/_decorator.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/spans/_spans.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/core/utils/__init__.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/exceptions.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/indexes.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/spans.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.5.2/src/opperai/types/validators.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/conftest.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_async_functions.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_async_indexes.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_async_spans.py
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_decorator.py
--rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_functions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_indexes.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_spans.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_trace_decorator.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/test_types.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
--rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.2/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.5.2/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.5.2/LICENSE
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 opperai-0.5.2/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 opperai-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 opperai-0.5.3/pytest.ini
+-rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 opperai-0.5.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/__init__.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/_client.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/_http_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/functions/__init__.py
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/functions/_async_functions.py
+-rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/functions/_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/indexes/__init__.py
+-rw-r--r--   0        0        0    12400 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/indexes/_async_indexes.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/indexes/_indexes.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/spans/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/spans/_async_spans.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/spans/_decorator.py
+-rw-r--r--   0        0        0     8749 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/spans/_spans.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/core/utils/__init__.py
+-rw-r--r--   0        0        0     6561 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/async_functions.py
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/decorator/__init__.py
+-rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/decorator/_decorator.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/functions/decorator/_schemas.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/indexes/async_indexes.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/indexes/indexes.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/spans/async_spans.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/spans/spans.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/exceptions.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/indexes.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/spans.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 opperai-0.5.3/src/opperai/types/validators.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/conftest.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_async_functions.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_async_indexes.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_async_spans.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_fn_decorator.py
+-rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_functions.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_indexes.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_spans.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_trace_decorator.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/test_types.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator.yaml
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_fn_decorator/test_fn_decorator_async.yaml
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 opperai-0.5.3/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 opperai-0.5.3/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 opperai-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 opperai-0.5.3/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 opperai-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 opperai-0.5.3/PKG-INFO
```

### Comparing `opperai-0.5.2/.github/workflows/publish.yml` & `opperai-0.5.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/src/opperai/_client.py` & `opperai-0.5.3/src/opperai/_client.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/src/opperai/functions.py` & `opperai-0.5.3/src/opperai/functions/functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import itertools
 from dataclasses import dataclass
-from typing import Any, List, Optional
-
-from pydantic import PrivateAttr
+from typing import Any, Dict, Iterator, List, Optional, Union
 
 from opperai._client import Client
-from opperai.core.functions.decorator._schemas import type_to_json_schema
-from opperai.types import ChatPayload, Message
+from opperai.functions.decorator._schemas import type_to_json_schema
+from opperai.types import ChatPayload, Message, StreamingChunk
 from opperai.types import Function as FunctionModel
 from opperai.types import FunctionResponse as FunctionResponseModel
+from pydantic import PrivateAttr
 
-from .spans import Span
+from ..spans.spans import Span
 
 
 class FunctionResponse(FunctionResponseModel):
     _client: Client = PrivateAttr()
 
     def __init__(self, client: Client = None, **kwargs):
         super().__init__(**kwargs)
@@ -22,26 +22,75 @@
         self._client = client
 
     @property
     def span(self):
         return Span(self._client, self.span_id)
 
 
+class StreamingResponse:
+    _client: Client = None
+    _head: StreamingChunk = None
+    _stream: Iterator[StreamingChunk] = None
+    context: List[Dict[str, Any]] = []
+    span: Span = None
+
+    def __init__(
+        self,
+        client: Client = None,
+        stream: Iterator[StreamingChunk] = None,
+    ):
+        if not client:
+            client = Client()
+        self._client = client
+
+        _stream, _head = itertools.tee(stream)
+        self._stream = _stream
+
+        head = next(_head)
+        self.span = Span(self._client, head.span_id)
+        self.context = head.context if head.context else []
+
+    @property
+    def deltas(self) -> Iterator[str]:
+        for chunk in self._stream:
+            if chunk.delta is not None:
+                yield chunk.delta
+
+
 @dataclass
 class Function:
     _client: Client
     _function: FunctionModel
 
     def chat(
-        self, messages: List[Message], parent_span_id: Optional[str] = None
-    ) -> FunctionResponse:
-        response = self._client.functions.chat(
+        self,
+        messages: List[Message],
+        parent_span_id: Optional[str] = None,
+        stream: Optional[bool] = False,
+    ) -> Union[FunctionResponse, StreamingResponse]:
+        if stream:
+            if self._function.out_schema is not None:
+                raise ValueError(
+                    "Cannot stream output for functions structured response"
+                )
+
+            response: Iterator[StreamingChunk] = self._client.functions.chat(
+                function_path=self._function.path,
+                data=ChatPayload(messages=messages, parent_span_uuid=parent_span_id),
+                stream=stream,
+            )
+
+            return StreamingResponse(client=self._client, stream=response)
+
+        response: FunctionResponseModel = self._client.functions.chat(
             function_path=self._function.path,
             data=ChatPayload(messages=messages, parent_span_uuid=parent_span_id),
+            stream=stream,
         )
+
         return FunctionResponse(client=self._client, **response.model_dump())
 
     def delete(self) -> bool:
         return self._client.functions.delete(id=self._function.id)
 
     def flush_cache(self) -> bool:
         return self._client.functions.flush_cache(id=self._function.id)
```

### Comparing `opperai-0.5.2/src/opperai/indexes.py` & `opperai-0.5.3/src/opperai/indexes/indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def upload_file(self, file_path: str, **kwargs):
         """Upload a file to the index."""
         return self._client.indexes.upload_file(
             id=self._index.id, file_path=file_path, **kwargs
         )
 
-    def index(self, doc: Document) -> Document:
+    def add(self, doc: Document) -> Document:
         """Index a document."""
         return self._client.indexes.index(id=self._index.id, doc=doc)
 
     def query(
         self, query: str, k: int = 10, filters: List[Filter] = None
     ) -> List[RetrievalResponse]:
         """Retrieve documents from the index."""
@@ -42,14 +42,15 @@
         if client is None:
             client = Client()
 
         self._client = client
 
     def create(self, name: str) -> Index:
         """Create an index with the given name.
+
         If an index with the given name already exists, return it.
         """
         try:
             index = self.get(name=name)
             if index:
                 return index
         except Exception:
```

### Comparing `opperai-0.5.2/src/opperai/spans.py` & `opperai-0.5.3/src/opperai/spans/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/src/opperai/core/_http_clients.py` & `opperai-0.5.3/src/opperai/core/_http_clients.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/src/opperai/core/functions/decorator/_schemas.py` & `opperai-0.5.3/src/opperai/functions/decorator/_schemas.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/src/opperai/core/spans/_decorator.py` & `opperai-0.5.3/src/opperai/core/spans/_decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,31 @@
 @contextmanager
 def start_span(
     name: str,
     input: Optional[str] = None,
     metadata: Optional[dict] = None,
     client: Optional[Client] = None,
 ):
+    """Context manager to start a new span for operation tracing.
+
+    Args:
+        name (str): The name of the span.
+        input (Optional[str]): The input data for the span, defaults to None.
+        metadata (Optional[dict]): Additional metadata for the span, defaults to None.
+        client (Optional[Client]): Custom client instance, defaults to None.
+
+    Yields:
+        SpanContext: The context of the current span.
+
+    Examples:
+
+        >>> with start_span(name="process_data", metadata={"user": "123"}) as span:
+        >>>     # your calls
+    """
+
     c = client if client is not None else Client()
     project = os.environ.get("OPPER_PROJECT", "missing_project")
     parent_span_id = _current_span_id.get()
     span_id = str(uuid4())
     span = Span(
         uuid=span_id,
         meta=metadata,
```

### Comparing `opperai-0.5.2/src/opperai/core/utils/__init__.py` & `opperai-0.5.3/src/opperai/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/src/opperai/types/__init__.py` & `opperai-0.5.3/src/opperai/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,23 +30,21 @@
     content: str
     metadata: Union[Optional[dict], FileMetadata] = Field(default=None)
 
 
 class StreamingChunk(BaseModel):
     span_id: Optional[str] = None
     delta: Optional[str] = None
-    error: Optional[str] = None
     context: Optional[List[ContextData]] = None
 
 
 class FunctionResponse(BaseModel):
     span_id: Optional[str] = None
     message: Optional[str] = None
     json_payload: Optional[Union[dict, List, Any]] = None
-    error: Optional[str] = None
     context: Optional[List[ContextData]] = None
     cached: Optional[bool] = None
 
 
 class CacheConfiguration(BaseModel):
     exact_match_cache_ttl: Optional[int] = None
     semantic_cache_threshold: Optional[float] = None
```

### Comparing `opperai-0.5.2/src/opperai/types/indexes.py` & `opperai-0.5.3/src/opperai/types/indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/src/opperai/types/spans.py` & `opperai-0.5.3/src/opperai/types/spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/src/opperai/types/validators.py` & `opperai-0.5.3/src/opperai/types/validators.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/conftest.py` & `opperai-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/test_async_functions.py` & `opperai-0.5.3/tests/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/test_async_indexes.py` & `opperai-0.5.3/tests/test_async_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/test_async_spans.py` & `opperai-0.5.3/tests/test_async_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/test_decorator.py` & `opperai-0.5.3/tests/test_fn_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,47 @@
 from typing import Dict, List, Optional, Union
 from unittest.mock import MagicMock, patch
 
 import pytest
 from jsonschema import validate
-from opperai import fn
-from opperai.core.functions.decorator._schemas import type_to_json_schema
+from opperai import AsyncClient, Client, fn
 from opperai.core.utils import convert_function_call_to_json
+from opperai.functions.decorator._schemas import type_to_json_schema
 from pydantic import BaseModel
 
 
+def test_fn_decorator(client: Client, vcr_cassette):
+    @fn(client=client)
+    def translate(text: str, target_language: str) -> str:
+        """Translate text to a target language."""
+
+    translation = translate("Hello", "es")
+    assert translation == "Hola"
+
+    translation, response = translate.call("Hello", "es")
+    assert translation == "Hola"
+
+    response.span.save_metric("metric", 1)
+
+
+@pytest.mark.asyncio(scope="module")
+async def test_fn_decorator_async(aclient: AsyncClient, vcr_cassette):
+    @fn(client=aclient)
+    async def translate(text: str, target_language: str) -> str:
+        """Translate text to a target language."""
+
+    translation = await translate("Hello", "es")
+    assert translation == "Hola"
+
+    translation, response = await translate.call("Hello", "es")
+    assert translation == "Hola"
+
+    await response.span.save_metric("metric", 1)
+
+
 @patch("opperai.core._http_clients._http_client.do_request")
 def test_decorator(mock_do_request):
     mock_do_request.side_effect = [
         MagicMock(status_code=404),
         MagicMock(
             status_code=200,
             json=lambda: {
@@ -156,14 +185,15 @@
 @pytest.mark.parametrize(
     "type_input,  example_input",
     [
         (int, 1),
         (str, "string"),
         (float, 1.0),
         (bool, True),
+        # (Dict[str, int], {"key": 1}),
         (List[int], [1, 2, 3]),
         (
             ParentModel,
             {
                 "child": {
                     "toy": {"name": "name"},
                     "toys": [{"name": "name"}],
```

### Comparing `opperai-0.5.2/tests/test_functions.py` & `opperai-0.5.3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/test_indexes.py` & `opperai-0.5.3/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/test_spans.py` & `opperai-0.5.3/tests/test_spans.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/test_trace_decorator.py` & `opperai-0.5.3/tests/test_trace_decorator.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/test_types.py` & `opperai-0.5.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_async_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_delete_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_spans/test_async_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_async_spans/test_save_metric.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_chat.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_chat_stream.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_create_function_with_cache_flush.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_delete_function_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_failed_structured_generation.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_get_by_path.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_functions/test_update_function.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_create_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_delete_index.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_id.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_get_by_name.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_index_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_list_indexes.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_document.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_indexes/test_retrieve_filters.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml` & `opperai-0.5.3/tests/fixtures/vcr_cassettes/test_spans/test_crud.yaml`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/LICENSE` & `opperai-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opperai-0.5.2/pyproject.toml` & `opperai-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "opperai"
-version = "0.5.2"
+version = "0.5.3"
 description = "Opper Python client"
 authors = [
   {name = "Opper", email = "opper@opper.ai"},
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `opperai-0.5.2/PKG-INFO` & `opperai-0.5.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: opperai
-Version: 0.5.2
+Version: 0.5.3
 Summary: Opper Python client
 Project-URL: Homepage, https://opper.ai
 Project-URL: Documentation, https://docs.opper.ai
 Project-URL: Platform, https://platform.opper.ai
 Author-email: Opper <opper@opper.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -58,95 +58,128 @@
 
 ## Calling functions
 
 To call a function you created at [https://platform.opper.ai](https://platform.opper.ai) you can use the following code:
 
 
 ```python
-from opperai import Client
-from opperai.types import ChatPayload, Message
+from opperai import Opper
+from opperai.types import Message
 
-client = Client(api_key="your-api-key") 
-response = client.functions.chat("your-function-path", 
-  ChatPayload(messages=[Message(role="user", content="hello")])
+opper = Opper()
+
+function = opper.functions.create(
+    "jokes/tell", 
+    instructions="given a topic tell a joke",
+)
+
+response = function.chat(
+    messages=[Message(role="user", content="topic: python")]
 )
 
 print(response)
 ```
 
 ## Async function calling
 
 ```python
 import asyncio
-from opperai import AsyncClient
-from opperai.types import ChatPayload, Message
-
-opper = AsyncClient(api_key="your-api-key")
+from opperai import AsyncOpper
+from opperai.types import Message
 
 async def main():
-    message = ""
-    async for response in await opper.functions.chat(
-        "your-function-path",
-        ChatPayload(messages=[Message(role="user", content="Hello, world!")]),
-        stream=True,
-    ):
-        if response.delta is not None:
-            message += response.delta
+    opper = AsyncOpper()
 
-    print(message)
+    function = await opper.functions.create(
+        "jokes/tell", 
+        instructions="given a topic tell a joke",
+    )
+    
+    response = await function.chat(
+        messages=[Message(role="user", content="topic: python")],
+    )
+
+    print(response)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ## Streaming responses
 
 ```python
-from opperai import Client
-from opperai.types import ChatPayload, Message
+from opperai import Opper
+from opperai.types import Message
+
+opper = Opper()
 
-client = Client(api_key="op-xxxx")
-response = client.functions.chat(
-    "joch/test",
-    ChatPayload(
-        messages=[Message(role="user", content="tell me a story.")],
-    ),
-    stream=True,
+function = opper.functions.create(
+    "jokes/tell", 
+    instructions="given a topic tell a joke",
+    description="tell a joke",
 )
-for data in response:
-    print(data.delta, end="", flush=True)
+
+response = function.chat(
+    messages=[Message(role="user", content="topic: python")],
+    stream=True
+)
+
+for delta in response.deltas:
+    print(delta, end="", flush=True)
 ```
 
 ## Async streaming responses
 
 ```python
 import asyncio
-from opperai import AsyncClient
-from opperai.types import ChatPayload, Message
+from opperai import AsyncOpper
+from opperai.types import Message
 
-client = AsyncClient(api_key="your-api-key")
 
 async def main():
-    async for response in await client.functions.chat(
-        "your-function-path",
-        ChatPayload(
-            messages=[Message(role="user", content="tell me a story.")],
-        ),
+    opper = AsyncOpper()
+    
+    function = await opper.functions.create(
+        "jokes/tell", 
+        instructions="given a topic tell a joke",
+        description="tell a joke",
+    )
+
+    response = await function.chat(
+        messages=[Message(role="user", content="topic: python")],
         stream=True,
-    ):
-        print(response.delta, end="", flush=True)
+    )
+
+    async for delta in response.deltas:
+        print(delta, end="", flush=True)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
-## Retrieval
+## Indexes
 
 ```python
-client.indexes.retrieve(index_id=42, "Who is the president of the USA?", 3)
+from opperai import Opper
+from opperai.types import Document, Filter
+
+opper = Opper()
+
+index = opper.indexes.create("my-index")
+
+index.upload_file("file.txt")
 
+index.add(Document(key="key1", content="Hello world 1", metadata={"score": 0}))
+index.add(Document(key="key1", content="Hello world 1", metadata={"score": 1}))
+index.add(Document(key="key2", content="Hello world 3", metadata={"score": 0}))
+
+response = index.query("Hello")
+print(response)
+
+response = index.query("Hello", filters=[Filter(key="score", operation="=", value="1")])
+print(response)
 ```
 
 # Examples
 
 See examples in our [documentation](https://docs.opper.ai)
```


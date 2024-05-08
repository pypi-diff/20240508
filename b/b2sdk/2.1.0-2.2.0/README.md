# Comparing `tmp/b2sdk-2.1.0.tar.gz` & `tmp/b2sdk-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sdk-2.1.0.tar", last modified: Mon Apr 15 13:35:21 2024, max compression
+gzip compressed data, was "b2sdk-2.2.0.tar", last modified: Wed May  8 18:33:46 2024, max compression
```

## Comparing `b2sdk-2.1.0.tar` & `b2sdk-2.2.0.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0    11963 2024-04-15 13:35:12.516558 b2sdk-2.1.0/LICENSE
--rw-r--r--   0        0        0     2219 2024-04-15 13:35:12.516558 b2sdk-2.1.0/README.md
-lrwxr-xr-x   0        0        0        0 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0      422 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/__init__.py
--rw-r--r--   0        0        0      319 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/__main__.py
--rw-r--r--   0        0        0      443 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/__init__.py
--rw-r--r--   0        0        0      414 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/__init__.py
--rw-r--r--   0        0        0    12688 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/abstract.py
--rw-r--r--   0        0        0     1381 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/exception.py
--rw-r--r--   0        0        0     4400 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/in_memory.py
--rw-r--r--   0        0        0    24095 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/sqlite_account_info.py
--rw-r--r--   0        0        0     4349 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/stub.py
--rw-r--r--   0        0        0     3534 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/account_info/upload_url_pool.py
--rw-r--r--   0        0        0    26244 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/api.py
--rw-r--r--   0        0        0     1748 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/api_config.py
--rw-r--r--   0        0        0     5835 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/application_key.py
--rw-r--r--   0        0        0    21710 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/b2http.py
--rw-r--r--   0        0        0     2316 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/bounded_queue_executor.py
--rw-r--r--   0        0        0    80634 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/bucket.py
--rw-r--r--   0        0        0     3746 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/cache.py
--rw-r--r--   0        0        0      340 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/encryption/__init__.py
--rw-r--r--   0        0        0    12661 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/encryption/setting.py
--rw-r--r--   0        0        0     1433 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/encryption/types.py
--rw-r--r--   0        0        0    20991 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/exception.py
--rw-r--r--   0        0        0    13765 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/file_lock.py
--rw-r--r--   0        0        0    23877 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/file_version.py
--rw-r--r--   0        0        0     1997 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/filter.py
--rw-r--r--   0        0        0     1555 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/http_constants.py
--rw-r--r--   0        0        0      863 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/included_sources.py
--rw-r--r--   0        0        0      340 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/large_file/__init__.py
--rw-r--r--   0        0        0     1496 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/large_file/part.py
--rw-r--r--   0        0        0     4777 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/large_file/services.py
--rw-r--r--   0        0        0     2923 2024-04-15 13:35:12.516558 b2sdk-2.1.0/b2sdk/_internal/large_file/unfinished_large_file.py
--rw-r--r--   0        0        0     7131 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/progress.py
--rw-r--r--   0        0        0    39876 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/raw_api.py
--rw-r--r--   0        0        0    80006 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/raw_simulator.py
--rw-r--r--   0        0        0      341 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/__init__.py
--rw-r--r--   0        0        0     8707 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/monitoring.py
--rw-r--r--   0        0        0     7331 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/setting.py
--rw-r--r--   0        0        0    13198 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/setup.py
--rw-r--r--   0        0        0      710 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/replication/types.py
--rw-r--r--   0        0        0    10141 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/LICENSE
--rw-r--r--   0        0        0      289 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/NOTICE
--rw-r--r--   0        0        0      232 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/README.md
--rw-r--r--   0        0        0     3275 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/__init__.py
--rw-r--r--   0        0        0      868 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/requests/included_source_meta.py
--rw-r--r--   0        0        0      334 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/__init__.py
--rw-r--r--   0        0        0     2880 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/exception.py
--rw-r--r--   0        0        0    15863 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/folder.py
--rw-r--r--   0        0        0     2021 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/folder_parser.py
--rw-r--r--   0        0        0     2724 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/path.py
--rw-r--r--   0        0        0     9060 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/policies.py
--rw-r--r--   0        0        0     6071 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/report.py
--rw-r--r--   0        0        0     3935 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/scan/scan.py
--rw-r--r--   0        0        0    21244 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/session.py
--rw-r--r--   0        0        0      615 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/__init__.py
--rw-r--r--   0        0        0      531 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/base.py
--rw-r--r--   0        0        0     5273 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/chained.py
--rw-r--r--   0        0        0     2389 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/hashing.py
--rw-r--r--   0        0        0     3100 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/progress.py
--rw-r--r--   0        0        0     2597 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/range.py
--rw-r--r--   0        0        0     2278 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/stream/wrapper.py
--rw-r--r--   0        0        0      334 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/__init__.py
--rw-r--r--   0        0        0    18071 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/action.py
--rw-r--r--   0        0        0     3901 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/encryption_provider.py
--rw-r--r--   0        0        0      422 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/exception.py
--rw-r--r--   0        0        0    18364 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/policy.py
--rw-r--r--   0        0        0     4378 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/policy_manager.py
--rw-r--r--   0        0        0     6351 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/report.py
--rw-r--r--   0        0        0    14535 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/sync/sync.py
--rw-r--r--   0        0        0      620 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/__init__.py
--rw-r--r--   0        0        0      345 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/__init__.py
--rw-r--r--   0        0        0    14793 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/emerger.py
--rw-r--r--   0        0        0      556 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/exception.py
--rw-r--r--   0        0        0    29077 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/executor.py
--rw-r--r--   0        0        0      353 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/__init__.py
--rw-r--r--   0        0        0     5456 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py
--rw-r--r--   0        0        0    32575 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/planner.py
--rw-r--r--   0        0        0     3582 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py
--rw-r--r--   0        0        0     8394 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py
--rw-r--r--   0        0        0     3229 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/write_intent.py
--rw-r--r--   0        0        0      346 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/__init__.py
--rw-r--r--   0        0        0     4399 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/download_manager.py
--rw-r--r--   0        0        0    10032 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloaded_file.py
--rw-r--r--   0        0        0      357 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/__init__.py
--rw-r--r--   0        0        0     5098 2024-04-15 13:35:12.520558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py
--rw-r--r--   0        0        0    18422 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py
--rw-r--r--   0        0        0     3702 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/simple.py
--rw-r--r--   0        0        0     3114 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py
--rw-r--r--   0        0        0      347 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/__init__.py
--rw-r--r--   0        0        0    10338 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/copy_manager.py
--rw-r--r--   0        0        0     3118 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/copy_source.py
--rw-r--r--   0        0        0     2114 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py
--rw-r--r--   0        0        0     1804 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/outbound_source.py
--rw-r--r--   0        0        0     1625 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/progress_reporter.py
--rw-r--r--   0        0        0     9583 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/upload_manager.py
--rw-r--r--   0        0        0    13100 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/upload_source.py
--rw-r--r--   0        0        0      560 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/transfer/transfer_manager.py
--rw-r--r--   0        0        0    14788 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1561 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/docs.py
--rw-r--r--   0        0        0     1643 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/escape.py
--rw-r--r--   0        0        0      948 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/filesystem.py
--rw-r--r--   0        0        0     1186 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/http_date.py
--rw-r--r--   0        0        0     1660 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/range_.py
--rw-r--r--   0        0        0     3546 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/thread_pool.py
--rw-r--r--   0        0        0      561 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/utils/typing.py
--rw-r--r--   0        0        0     7160 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_internal/version_utils.py
--rw-r--r--   0        0        0      551 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_pyinstaller/__init__.py
--rw-r--r--   0        0        0      417 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_pyinstaller/hook-b2sdk.py
--rw-r--r--   0        0        0    12542 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_v3/__init__.py
--rw-r--r--   0        0        0     7083 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/_v3/exception.py
--rw-r--r--   0        0        0      705 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/__init__.py
--rw-r--r--   0        0        0     2035 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/account_info.py
--rw-r--r--   0        0        0      999 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/api.py
--rw-r--r--   0        0        0     1078 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/bucket.py
--rw-r--r--   0        0        0      969 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/exception.py
--rw-r--r--   0        0        0     7245 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v0/sync.py
--rw-r--r--   0        0        0     1351 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/__init__.py
--rw-r--r--   0        0        0     5908 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/account_info.py
--rw-r--r--   0        0        0     8348 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/api.py
--rw-r--r--   0        0        0     1927 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/b2http.py
--rw-r--r--   0        0        0    13668 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/bucket.py
--rw-r--r--   0        0        0      530 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/cache.py
--rw-r--r--   0        0        0     6787 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/download_dest.py
--rw-r--r--   0        0        0     1580 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/exception.py
--rw-r--r--   0        0        0     2218 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/file_metadata.py
--rw-r--r--   0        0        0     7019 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/file_version.py
--rw-r--r--   0        0        0      334 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/replication/__init__.py
--rw-r--r--   0        0        0     1148 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/replication/monitoring.py
--rw-r--r--   0        0        0     2596 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/session.py
--rw-r--r--   0        0        0      505 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/__init__.py
--rw-r--r--   0        0        0     3869 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/encryption_provider.py
--rw-r--r--   0        0        0     3849 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/file.py
--rw-r--r--   0        0        0     2816 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/file_to_path_translator.py
--rw-r--r--   0        0        0     2318 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/folder.py
--rw-r--r--   0        0        0      738 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/folder_parser.py
--rw-r--r--   0        0        0      846 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/report.py
--rw-r--r--   0        0        0     6929 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/scan_policies.py
--rw-r--r--   0        0        0     5387 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v1/sync/sync.py
--rw-r--r--   0        0        0     1356 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v2/__init__.py
--rw-r--r--   0        0        0      454 2024-04-15 13:35:12.524558 b2sdk-2.1.0/b2sdk/v2/_compat.py
--rw-r--r--   0        0        0      494 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/account_info.py
--rw-r--r--   0        0        0     2235 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/api.py
--rw-r--r--   0        0        0      803 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/b2http.py
--rw-r--r--   0        0        0     3086 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/bucket.py
--rw-r--r--   0        0        0      812 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/exception.py
--rw-r--r--   0        0        0     2902 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/file_version.py
--rw-r--r--   0        0        0     1339 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/large_file.py
--rw-r--r--   0        0        0     2751 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/raw_api.py
--rw-r--r--   0        0        0     3704 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/raw_simulator.py
--rw-r--r--   0        0        0     1523 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/session.py
--rw-r--r--   0        0        0      369 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/sync.py
--rw-r--r--   0        0        0      584 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/transfer.py
--rw-r--r--   0        0        0     1033 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/utils.py
--rw-r--r--   0        0        0     1612 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/v2/version_utils.py
--rw-r--r--   0        0        0      767 2024-04-15 13:35:12.528558 b2sdk-2.1.0/b2sdk/version.py
--rw-r--r--   0        0        0     4436 2024-04-15 13:35:21.780540 b2sdk-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 b2sdk-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11963 2024-05-08 18:33:34.831703 b2sdk-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2219 2024-05-08 18:33:34.831703 b2sdk-2.2.0/README.md
+lrwxr-xr-x   0        0        0        0 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0      422 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/__init__.py
+-rw-r--r--   0        0        0      319 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/__main__.py
+-rw-r--r--   0        0        0      443 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/__init__.py
+-rw-r--r--   0        0        0      414 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/account_info/__init__.py
+-rw-r--r--   0        0        0    12688 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/account_info/abstract.py
+-rw-r--r--   0        0        0     1381 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/account_info/exception.py
+-rw-r--r--   0        0        0     4400 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/account_info/in_memory.py
+-rw-r--r--   0        0        0    24095 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/account_info/sqlite_account_info.py
+-rw-r--r--   0        0        0     4349 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/account_info/stub.py
+-rw-r--r--   0        0        0     3534 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/account_info/upload_url_pool.py
+-rw-r--r--   0        0        0    26244 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/api.py
+-rw-r--r--   0        0        0     1748 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/api_config.py
+-rw-r--r--   0        0        0     5835 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/application_key.py
+-rw-r--r--   0        0        0    21710 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/b2http.py
+-rw-r--r--   0        0        0     2316 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/bounded_queue_executor.py
+-rw-r--r--   0        0        0    80634 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/bucket.py
+-rw-r--r--   0        0        0     3746 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/cache.py
+-rw-r--r--   0        0        0      340 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/encryption/__init__.py
+-rw-r--r--   0        0        0    12661 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/encryption/setting.py
+-rw-r--r--   0        0        0     1433 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/encryption/types.py
+-rw-r--r--   0        0        0    20991 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/exception.py
+-rw-r--r--   0        0        0    13765 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/file_lock.py
+-rw-r--r--   0        0        0    23877 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/file_version.py
+-rw-r--r--   0        0        0     1997 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/filter.py
+-rw-r--r--   0        0        0     1555 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/http_constants.py
+-rw-r--r--   0        0        0      863 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/included_sources.py
+-rw-r--r--   0        0        0      340 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/large_file/__init__.py
+-rw-r--r--   0        0        0     1496 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/large_file/part.py
+-rw-r--r--   0        0        0     4777 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/large_file/services.py
+-rw-r--r--   0        0        0     2923 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/large_file/unfinished_large_file.py
+-rw-r--r--   0        0        0     7131 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/progress.py
+-rw-r--r--   0        0        0    39883 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/raw_api.py
+-rw-r--r--   0        0        0    80006 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/raw_simulator.py
+-rw-r--r--   0        0        0      341 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/replication/__init__.py
+-rw-r--r--   0        0        0     8707 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/replication/monitoring.py
+-rw-r--r--   0        0        0     7331 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/replication/setting.py
+-rw-r--r--   0        0        0    13198 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/replication/setup.py
+-rw-r--r--   0        0        0      710 2024-05-08 18:33:34.831703 b2sdk-2.2.0/b2sdk/_internal/replication/types.py
+-rw-r--r--   0        0        0    10141 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/requests/LICENSE
+-rw-r--r--   0        0        0      289 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/requests/NOTICE
+-rw-r--r--   0        0        0      232 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/requests/README.md
+-rw-r--r--   0        0        0     3275 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/requests/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/requests/included_source_meta.py
+-rw-r--r--   0        0        0      334 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/scan/__init__.py
+-rw-r--r--   0        0        0     2880 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/scan/exception.py
+-rw-r--r--   0        0        0    15885 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/scan/folder.py
+-rw-r--r--   0        0        0     2021 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/scan/folder_parser.py
+-rw-r--r--   0        0        0     2724 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/scan/path.py
+-rw-r--r--   0        0        0     9060 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/scan/policies.py
+-rw-r--r--   0        0        0     6879 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/scan/report.py
+-rw-r--r--   0        0        0     3935 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/scan/scan.py
+-rw-r--r--   0        0        0    21244 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/session.py
+-rw-r--r--   0        0        0      615 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/stream/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/stream/base.py
+-rw-r--r--   0        0        0     5273 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/stream/chained.py
+-rw-r--r--   0        0        0     2389 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/stream/hashing.py
+-rw-r--r--   0        0        0     3100 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/stream/progress.py
+-rw-r--r--   0        0        0     2597 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/stream/range.py
+-rw-r--r--   0        0        0     2278 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/stream/wrapper.py
+-rw-r--r--   0        0        0      334 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/sync/__init__.py
+-rw-r--r--   0        0        0    18071 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/sync/action.py
+-rw-r--r--   0        0        0     3901 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/sync/encryption_provider.py
+-rw-r--r--   0        0        0      422 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/sync/exception.py
+-rw-r--r--   0        0        0    18364 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/sync/policy.py
+-rw-r--r--   0        0        0     4378 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/sync/policy_manager.py
+-rw-r--r--   0        0        0     6351 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/sync/report.py
+-rw-r--r--   0        0        0    14535 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/sync/sync.py
+-rw-r--r--   0        0        0      620 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/__init__.py
+-rw-r--r--   0        0        0      345 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/__init__.py
+-rw-r--r--   0        0        0    14793 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/emerger.py
+-rw-r--r--   0        0        0      556 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/exception.py
+-rw-r--r--   0        0        0    29077 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/executor.py
+-rw-r--r--   0        0        0      353 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/planner/__init__.py
+-rw-r--r--   0        0        0     5456 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py
+-rw-r--r--   0        0        0    32575 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/planner/planner.py
+-rw-r--r--   0        0        0     3582 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py
+-rw-r--r--   0        0        0     8394 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py
+-rw-r--r--   0        0        0     3229 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/write_intent.py
+-rw-r--r--   0        0        0      346 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/__init__.py
+-rw-r--r--   0        0        0     4399 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/download_manager.py
+-rw-r--r--   0        0        0    10032 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloaded_file.py
+-rw-r--r--   0        0        0      357 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloader/__init__.py
+-rw-r--r--   0        0        0     5098 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py
+-rw-r--r--   0        0        0    18422 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py
+-rw-r--r--   0        0        0     3702 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloader/simple.py
+-rw-r--r--   0        0        0     3114 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py
+-rw-r--r--   0        0        0      347 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/__init__.py
+-rw-r--r--   0        0        0    10338 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/copy_manager.py
+-rw-r--r--   0        0        0     3118 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/copy_source.py
+-rw-r--r--   0        0        0     2114 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py
+-rw-r--r--   0        0        0     1804 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/outbound_source.py
+-rw-r--r--   0        0        0     1625 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/progress_reporter.py
+-rw-r--r--   0        0        0     9583 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/upload_manager.py
+-rw-r--r--   0        0        0    13100 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/upload_source.py
+-rw-r--r--   0        0        0      560 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/transfer/transfer_manager.py
+-rw-r--r--   0        0        0    14906 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1561 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/utils/docs.py
+-rw-r--r--   0        0        0     1659 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/utils/escape.py
+-rw-r--r--   0        0        0      948 2024-05-08 18:33:34.835703 b2sdk-2.2.0/b2sdk/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0     1186 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/_internal/utils/http_date.py
+-rw-r--r--   0        0        0     1660 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/_internal/utils/range_.py
+-rw-r--r--   0        0        0     3546 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/_internal/utils/thread_pool.py
+-rw-r--r--   0        0        0      561 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/_internal/utils/typing.py
+-rw-r--r--   0        0        0     7160 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/_internal/version_utils.py
+-rw-r--r--   0        0        0      551 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/_pyinstaller/__init__.py
+-rw-r--r--   0        0        0      417 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/_pyinstaller/hook-b2sdk.py
+-rw-r--r--   0        0        0    12542 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/_v3/__init__.py
+-rw-r--r--   0        0        0     7083 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/_v3/exception.py
+-rw-r--r--   0        0        0      705 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v0/__init__.py
+-rw-r--r--   0        0        0     2035 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v0/account_info.py
+-rw-r--r--   0        0        0      999 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v0/api.py
+-rw-r--r--   0        0        0     1078 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v0/bucket.py
+-rw-r--r--   0        0        0      969 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v0/exception.py
+-rw-r--r--   0        0        0     7245 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v0/sync.py
+-rw-r--r--   0        0        0     1351 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/__init__.py
+-rw-r--r--   0        0        0     5908 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/account_info.py
+-rw-r--r--   0        0        0     8348 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/api.py
+-rw-r--r--   0        0        0     1927 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/b2http.py
+-rw-r--r--   0        0        0    13668 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/bucket.py
+-rw-r--r--   0        0        0      530 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/cache.py
+-rw-r--r--   0        0        0     6787 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/download_dest.py
+-rw-r--r--   0        0        0     1580 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/exception.py
+-rw-r--r--   0        0        0     2218 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/file_metadata.py
+-rw-r--r--   0        0        0     7019 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/file_version.py
+-rw-r--r--   0        0        0      334 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/replication/__init__.py
+-rw-r--r--   0        0        0     1148 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/replication/monitoring.py
+-rw-r--r--   0        0        0     2596 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/session.py
+-rw-r--r--   0        0        0      505 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/sync/__init__.py
+-rw-r--r--   0        0        0     3869 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/sync/encryption_provider.py
+-rw-r--r--   0        0        0     3849 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/sync/file.py
+-rw-r--r--   0        0        0     2816 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/sync/file_to_path_translator.py
+-rw-r--r--   0        0        0     2318 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/sync/folder.py
+-rw-r--r--   0        0        0      738 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/sync/folder_parser.py
+-rw-r--r--   0        0        0      846 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/sync/report.py
+-rw-r--r--   0        0        0     6929 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/sync/scan_policies.py
+-rw-r--r--   0        0        0     5387 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v1/sync/sync.py
+-rw-r--r--   0        0        0     1356 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/__init__.py
+-rw-r--r--   0        0        0      454 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/_compat.py
+-rw-r--r--   0        0        0      494 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/account_info.py
+-rw-r--r--   0        0        0     2235 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/api.py
+-rw-r--r--   0        0        0      804 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/b2http.py
+-rw-r--r--   0        0        0     3086 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/bucket.py
+-rw-r--r--   0        0        0      812 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/exception.py
+-rw-r--r--   0        0        0     2902 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/file_version.py
+-rw-r--r--   0        0        0     1339 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/large_file.py
+-rw-r--r--   0        0        0     2751 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/raw_api.py
+-rw-r--r--   0        0        0     3704 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/raw_simulator.py
+-rw-r--r--   0        0        0     1523 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/session.py
+-rw-r--r--   0        0        0      369 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/sync.py
+-rw-r--r--   0        0        0      584 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/transfer.py
+-rw-r--r--   0        0        0     1033 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/utils.py
+-rw-r--r--   0        0        0     1612 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/v2/version_utils.py
+-rw-r--r--   0        0        0      767 2024-05-08 18:33:34.839703 b2sdk-2.2.0/b2sdk/version.py
+-rw-r--r--   0        0        0     4436 2024-05-08 18:33:46.175703 b2sdk-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 b2sdk-2.2.0/PKG-INFO
```

### Comparing `b2sdk-2.1.0/LICENSE` & `b2sdk-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/README.md` & `b2sdk-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/account_info/abstract.py` & `b2sdk-2.2.0/b2sdk/_internal/account_info/abstract.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/account_info/exception.py` & `b2sdk-2.2.0/b2sdk/_internal/account_info/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/account_info/in_memory.py` & `b2sdk-2.2.0/b2sdk/_internal/account_info/in_memory.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/account_info/sqlite_account_info.py` & `b2sdk-2.2.0/b2sdk/_internal/account_info/sqlite_account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/account_info/stub.py` & `b2sdk-2.2.0/b2sdk/_internal/account_info/stub.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/account_info/upload_url_pool.py` & `b2sdk-2.2.0/b2sdk/_internal/account_info/upload_url_pool.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/api.py` & `b2sdk-2.2.0/b2sdk/_internal/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/api_config.py` & `b2sdk-2.2.0/b2sdk/_internal/api_config.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/application_key.py` & `b2sdk-2.2.0/b2sdk/_internal/application_key.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/b2http.py` & `b2sdk-2.2.0/b2sdk/_internal/b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/bounded_queue_executor.py` & `b2sdk-2.2.0/b2sdk/_internal/bounded_queue_executor.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/bucket.py` & `b2sdk-2.2.0/b2sdk/_internal/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/cache.py` & `b2sdk-2.2.0/b2sdk/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/encryption/setting.py` & `b2sdk-2.2.0/b2sdk/_internal/encryption/setting.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/encryption/types.py` & `b2sdk-2.2.0/b2sdk/_internal/encryption/types.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/exception.py` & `b2sdk-2.2.0/b2sdk/_internal/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/file_lock.py` & `b2sdk-2.2.0/b2sdk/_internal/file_lock.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/file_version.py` & `b2sdk-2.2.0/b2sdk/_internal/file_version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/filter.py` & `b2sdk-2.2.0/b2sdk/_internal/filter.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/http_constants.py` & `b2sdk-2.2.0/b2sdk/_internal/http_constants.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/included_sources.py` & `b2sdk-2.2.0/b2sdk/_internal/included_sources.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/large_file/part.py` & `b2sdk-2.2.0/b2sdk/_internal/large_file/part.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/large_file/services.py` & `b2sdk-2.2.0/b2sdk/_internal/large_file/services.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/large_file/unfinished_large_file.py` & `b2sdk-2.2.0/b2sdk/_internal/large_file/unfinished_large_file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/progress.py` & `b2sdk-2.2.0/b2sdk/_internal/progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/raw_api.py` & `b2sdk-2.2.0/b2sdk/_internal/raw_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     `hmacSha256SigningSecret`, if present, has to be a string of 32 alphanumeric characters.
     """
     # TODO: add URL to the documentation
 
     targetType: Literal['webhook']
     url: str
     customHeaders: NotRequired[list[NameValueDict] | None]
-    hmacSha256SigningSecret: NotRequired[str]
+    hmacSha256SigningSecret: NotRequired[str | None]
 
 
 EVENT_TYPE = Literal[
     'b2:ObjectCreated:*', 'b2:ObjectCreated:Upload', 'b2:ObjectCreated:MultipartUpload',
     'b2:ObjectCreated:Copy', 'b2:ObjectCreated:Replica', 'b2:ObjectCreated:MultipartReplica',
     'b2:ObjectDeleted:*', 'b2:ObjectDeleted:Delete', 'b2:ObjectDeleted:LifecycleRule',
     'b2:HideMarkerCreated:*', 'b2:HideMarkerCreated:Hide', 'b2:HideMarkerCreated:LifecycleRule',]
```

### Comparing `b2sdk-2.1.0/b2sdk/_internal/raw_simulator.py` & `b2sdk-2.2.0/b2sdk/_internal/raw_simulator.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/replication/monitoring.py` & `b2sdk-2.2.0/b2sdk/_internal/replication/monitoring.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/replication/setting.py` & `b2sdk-2.2.0/b2sdk/_internal/replication/setting.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/replication/setup.py` & `b2sdk-2.2.0/b2sdk/_internal/replication/setup.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/replication/types.py` & `b2sdk-2.2.0/b2sdk/_internal/replication/types.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/requests/LICENSE` & `b2sdk-2.2.0/b2sdk/_internal/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/requests/__init__.py` & `b2sdk-2.2.0/b2sdk/_internal/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/requests/included_source_meta.py` & `b2sdk-2.2.0/b2sdk/_internal/requests/included_source_meta.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/scan/exception.py` & `b2sdk-2.2.0/b2sdk/_internal/scan/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/scan/folder.py` & `b2sdk-2.2.0/b2sdk/_internal/scan/folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import platform
 import re
 import sys
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
 from typing import Iterator
 
-from ..utils import fix_windows_path_limit, get_file_mtime, is_file_readable
+from ..utils import fix_windows_path_limit, get_file_mtime, is_file_readable, validate_b2_file_name
 from .exception import (
     EmptyDirectory,
     EnvironmentEncodingError,
     NotADirectory,
     UnableToCreateDirectory,
     UnsupportedFilename,
 )
@@ -237,25 +237,25 @@
                 # Infinite symlink loop detected, report warning and skip symlink
                 if reporter is not None:
                     reporter.circular_symlink_skipped(str(local_dir))
                 return
 
             visited_symlinks.add(inode_number)
 
-        for name in (x.name for x in local_dir.iterdir()):
-
-            if '/' in name:
-                raise UnsupportedFilename(
-                    "scan does not support file names that include '/'",
-                    f"{name} in dir {local_dir}"
-                )
-
-            local_path = local_dir / name
+        for local_path in local_dir.iterdir():
+            name = local_path.name
             relative_file_path = join_b2_path(relative_dir_path, name)
 
+            try:
+                validate_b2_file_name(name)
+            except ValueError as e:
+                if reporter is not None:
+                    reporter.invalid_name(str(local_path), str(e))
+                continue
+
             # Skip broken symlinks or other inaccessible files
             if not is_file_readable(str(local_path), reporter):
                 continue
 
             if policies_manager.exclude_all_symlinks and local_path.is_symlink():
                 if reporter is not None:
                     reporter.symlink_skipped(str(local_path))
```

### Comparing `b2sdk-2.1.0/b2sdk/_internal/scan/folder_parser.py` & `b2sdk-2.2.0/b2sdk/_internal/scan/folder_parser.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/scan/path.py` & `b2sdk-2.2.0/b2sdk/_internal/scan/path.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/scan/policies.py` & `b2sdk-2.2.0/b2sdk/_internal/scan/policies.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/scan/report.py` & `b2sdk-2.2.0/b2sdk/_internal/scan/report.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import logging
 import threading
 import time
 from dataclasses import dataclass
 from io import TextIOWrapper
 
 from ..utils import format_and_scale_number
+from ..utils.escape import escape_control_chars
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ProgressReport:
     """
@@ -44,14 +45,15 @@
         self.closed = False
         self.lock = threading.Lock()
         self.current_line = ''
         self.encoding_warning_was_already_printed = False
         self._last_update_time = 0
         self._update_progress()
         self.warnings = []
+        self.errors_encountered = False
 
     def close(self):
         """
         Perform a clean-up.
         """
         with self.lock:
             if not self.no_progress:
@@ -62,21 +64,30 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
+    def has_errors_or_warnings(self) -> bool:
+        """
+        Check if there are any errors or warnings.
+
+        :return: True if there are any errors or warnings
+        """
+        return self.errors_encountered or bool(self.warnings)
+
     def error(self, message: str) -> None:
         """
         Print an error, gracefully interleaving it with a progress bar.
 
         :param message: an error message
         """
         self.print_completion(message)
+        self.errors_encountered = True
 
     def print_completion(self, message: str) -> None:
         """
         Remove the progress bar, prints a message, and puts the progress
         bar back.
 
         :param message: an error message
@@ -164,35 +175,49 @@
 
     def local_access_error(self, path: str) -> None:
         """
         Add a file access error message to the list of warnings.
 
         :param path: file path
         """
-        self.warnings.append(f'WARNING: {path} could not be accessed (broken symlink?)')
+        self.warnings.append(
+            f'WARNING: {escape_control_chars(path)} could not be accessed (broken symlink?)'
+        )
 
     def local_permission_error(self, path: str) -> None:
         """
         Add a permission error message to the list of warnings.
 
         :param path: file path
         """
-        self.warnings.append(f'WARNING: {path} could not be accessed (no permissions to read?)')
+        self.warnings.append(
+            f'WARNING: {escape_control_chars(path)} could not be accessed (no permissions to read?)'
+        )
 
     def symlink_skipped(self, path: str) -> None:
         pass
 
     def circular_symlink_skipped(self, path: str) -> None:
         """
         Add a circular symlink error message to the list of warnings.
 
         :param path: file path
         """
         self.warnings.append(
-            f'WARNING: {path} is a circular symlink, which was already visited. Skipping.'
+            f'WARNING: {escape_control_chars(path)} is a circular symlink, which was already visited. Skipping.'
+        )
+
+    def invalid_name(self, path: str, error: str) -> None:
+        """
+        Add an invalid filename error message to the list of warnings.
+
+        :param path: file path
+        """
+        self.warnings.append(
+            f'WARNING: {escape_control_chars(path)} path contains invalid name ({error}). Skipping.'
         )
 
 
 def sample_report_run():
     """
     Generate a sample report.
     """
```

### Comparing `b2sdk-2.1.0/b2sdk/_internal/scan/scan.py` & `b2sdk-2.2.0/b2sdk/_internal/scan/scan.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/session.py` & `b2sdk-2.2.0/b2sdk/_internal/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/stream/__init__.py` & `b2sdk-2.2.0/b2sdk/_internal/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/stream/base.py` & `b2sdk-2.2.0/b2sdk/_internal/stream/base.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/stream/chained.py` & `b2sdk-2.2.0/b2sdk/_internal/stream/chained.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/stream/hashing.py` & `b2sdk-2.2.0/b2sdk/_internal/stream/hashing.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/stream/progress.py` & `b2sdk-2.2.0/b2sdk/_internal/stream/progress.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/stream/range.py` & `b2sdk-2.2.0/b2sdk/_internal/stream/range.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/stream/wrapper.py` & `b2sdk-2.2.0/b2sdk/_internal/stream/wrapper.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/sync/action.py` & `b2sdk-2.2.0/b2sdk/_internal/sync/action.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/sync/encryption_provider.py` & `b2sdk-2.2.0/b2sdk/_internal/sync/encryption_provider.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/sync/policy.py` & `b2sdk-2.2.0/b2sdk/_internal/sync/policy.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/sync/policy_manager.py` & `b2sdk-2.2.0/b2sdk/_internal/sync/policy_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/sync/report.py` & `b2sdk-2.2.0/b2sdk/_internal/sync/report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/sync/sync.py` & `b2sdk-2.2.0/b2sdk/_internal/sync/sync.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/__init__.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/emerger.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/emerger.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/exception.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/executor.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/executor.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/planner.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/planner/planner.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/emerge/write_intent.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/emerge/write_intent.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/download_manager.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/download_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloaded_file.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloaded_file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/simple.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloader/simple.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/copy_manager.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/copy_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/copy_source.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/copy_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/outbound_source.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/outbound_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/progress_reporter.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/progress_reporter.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/upload_manager.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/upload_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/outbound/upload_source.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/outbound/upload_source.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/transfer/transfer_manager.py` & `b2sdk-2.2.0/b2sdk/_internal/transfer/transfer_manager.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/utils/__init__.py` & `b2sdk-2.2.0/b2sdk/_internal/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,18 @@
     Raise a ValueError if the name is not a valid B2 file name.
 
     :param name: a string to check
     :type name: str
     """
     if not isinstance(name, str):
         raise ValueError('file name must be a string, not bytes')
-    name_utf8 = name.encode('utf-8')
+    try:
+        name_utf8 = name.encode('utf-8')
+    except UnicodeEncodeError:
+        raise ValueError('file name must be valid Unicode, check locale')
     if len(name_utf8) < 1:
         raise ValueError('file name too short (0 utf-8 bytes)')
     if 1000 < len(name_utf8):
         raise ValueError('file name too long (more than 1000 utf-8 bytes)')
     if name[0] == '/':
         raise ValueError("file names must not start with '/'")
     if name[-1] == '/':
```

### Comparing `b2sdk-2.1.0/b2sdk/_internal/utils/docs.py` & `b2sdk-2.2.0/b2sdk/_internal/utils/docs.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/utils/escape.py` & `b2sdk-2.2.0/b2sdk/_internal/utils/escape.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,55 +4,53 @@
 #
 # Copyright 2023 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
+from __future__ import annotations
+
 import re
 import shlex
 
 # skip newline, tab
 UNPRINTABLE_PATTERN = re.compile(r'[\x00-\x08\x0e-\x1f\x7f-\x9f]')
 
 
-def unprintable_to_hex(s):
+def unprintable_to_hex(s: str) -> str:
     """
     Replace unprintable chars in string with a hex representation.
 
-    :param string: an arbitrary string, possibly with unprintable characters.
+    :param s: an arbitrary string, possibly with unprintable characters.
     :return: the string, with unprintable characters changed to hex (e.g., "\x07")
-
     """
 
     def hexify(match):
-        return fr'\x{ord(match.group()):02x}'
+        return rf"\x{ord(match.group()):02x}"
 
     if s:
         return UNPRINTABLE_PATTERN.sub(hexify, s)
-    return None
+    return s
 
 
-def escape_control_chars(s):
+def escape_control_chars(s: str) -> str:
     """
     Replace unprintable chars in string with a hex representation AND shell quotes the string.
 
-    :param string: an arbitrary string, possibly with unprintable characters.
+    :param s: an arbitrary string, possibly with unprintable characters.
     :return: the string, with unprintable characters changed to hex (e.g., "\x07")
-
     """
     if s:
         return shlex.quote(unprintable_to_hex(s))
-    return None
+    return s
 
 
-def substitute_control_chars(s):
+def substitute_control_chars(s: str) -> tuple[str, bool]:
     """
     Replace unprintable chars in string with � unicode char
 
-    :param string: an arbitrary string, possibly with unprintable characters.
+    :param s: an arbitrary string, possibly with unprintable characters.
     :return: tuple of the string with � replacements made and boolean indicated if chars were replaced
-
     """
-    match_result = UNPRINTABLE_PATTERN.search(s)
-    s = UNPRINTABLE_PATTERN.sub('�', s)
-    return (s, match_result is not None)
+    new_value = UNPRINTABLE_PATTERN.sub("�", s)
+    return new_value, new_value != s
```

### Comparing `b2sdk-2.1.0/b2sdk/_internal/utils/filesystem.py` & `b2sdk-2.2.0/b2sdk/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/utils/http_date.py` & `b2sdk-2.2.0/b2sdk/_internal/utils/http_date.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/utils/range_.py` & `b2sdk-2.2.0/b2sdk/_internal/utils/range_.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/utils/thread_pool.py` & `b2sdk-2.2.0/b2sdk/_internal/utils/thread_pool.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/utils/typing.py` & `b2sdk-2.2.0/b2sdk/_internal/utils/typing.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_internal/version_utils.py` & `b2sdk-2.2.0/b2sdk/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_pyinstaller/__init__.py` & `b2sdk-2.2.0/b2sdk/_pyinstaller/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_v3/__init__.py` & `b2sdk-2.2.0/b2sdk/_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/_v3/exception.py` & `b2sdk-2.2.0/b2sdk/_v3/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v0/__init__.py` & `b2sdk-2.2.0/b2sdk/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v0/account_info.py` & `b2sdk-2.2.0/b2sdk/v0/account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v0/api.py` & `b2sdk-2.2.0/b2sdk/v0/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v0/bucket.py` & `b2sdk-2.2.0/b2sdk/v0/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v0/exception.py` & `b2sdk-2.2.0/b2sdk/v0/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v0/sync.py` & `b2sdk-2.2.0/b2sdk/v0/sync.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/__init__.py` & `b2sdk-2.2.0/b2sdk/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/account_info.py` & `b2sdk-2.2.0/b2sdk/v1/account_info.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/api.py` & `b2sdk-2.2.0/b2sdk/v1/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/b2http.py` & `b2sdk-2.2.0/b2sdk/v1/b2http.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/bucket.py` & `b2sdk-2.2.0/b2sdk/v1/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/cache.py` & `b2sdk-2.2.0/b2sdk/v1/cache.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/download_dest.py` & `b2sdk-2.2.0/b2sdk/v1/download_dest.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/exception.py` & `b2sdk-2.2.0/b2sdk/v1/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/file_metadata.py` & `b2sdk-2.2.0/b2sdk/v1/file_metadata.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/file_version.py` & `b2sdk-2.2.0/b2sdk/v1/file_version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/replication/monitoring.py` & `b2sdk-2.2.0/b2sdk/v1/replication/monitoring.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/session.py` & `b2sdk-2.2.0/b2sdk/v1/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/sync/encryption_provider.py` & `b2sdk-2.2.0/b2sdk/v1/sync/encryption_provider.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/sync/file.py` & `b2sdk-2.2.0/b2sdk/v1/sync/file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/sync/file_to_path_translator.py` & `b2sdk-2.2.0/b2sdk/v1/sync/file_to_path_translator.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/sync/folder.py` & `b2sdk-2.2.0/b2sdk/v1/sync/folder.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/sync/folder_parser.py` & `b2sdk-2.2.0/b2sdk/v1/sync/folder_parser.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/sync/report.py` & `b2sdk-2.2.0/b2sdk/v1/sync/report.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/sync/scan_policies.py` & `b2sdk-2.2.0/b2sdk/v1/sync/scan_policies.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v1/sync/sync.py` & `b2sdk-2.2.0/b2sdk/v1/sync/sync.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/__init__.py` & `b2sdk-2.2.0/b2sdk/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/api.py` & `b2sdk-2.2.0/b2sdk/v2/api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/b2http.py` & `b2sdk-2.2.0/b2sdk/v2/b2http.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 from b2sdk._v3.exception import BucketIdNotFound as v3BucketIdNotFound
 from .exception import BucketIdNotFound
 
 
 # Overridden to retain old-style BadRequest exception in case of a bad bucket id
 class B2Http(v3.B2Http):
     @classmethod
-    def _translate_error(cls, fcn, post_params=None):
+    def _translate_errors(cls, fcn, post_params=None):
         try:
             return super()._translate_errors(fcn, post_params)
         except v3BucketIdNotFound as e:
             raise BucketIdNotFound(e.bucket_id)
```

### Comparing `b2sdk-2.1.0/b2sdk/v2/bucket.py` & `b2sdk-2.2.0/b2sdk/v2/bucket.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/exception.py` & `b2sdk-2.2.0/b2sdk/v2/exception.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/file_version.py` & `b2sdk-2.2.0/b2sdk/v2/file_version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/large_file.py` & `b2sdk-2.2.0/b2sdk/v2/large_file.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/raw_api.py` & `b2sdk-2.2.0/b2sdk/v2/raw_api.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/raw_simulator.py` & `b2sdk-2.2.0/b2sdk/v2/raw_simulator.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/session.py` & `b2sdk-2.2.0/b2sdk/v2/session.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/transfer.py` & `b2sdk-2.2.0/b2sdk/v2/transfer.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/utils.py` & `b2sdk-2.2.0/b2sdk/v2/utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/v2/version_utils.py` & `b2sdk-2.2.0/b2sdk/v2/version_utils.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/b2sdk/version.py` & `b2sdk-2.2.0/b2sdk/version.py`

 * *Files identical despite different names*

### Comparing `b2sdk-2.1.0/pyproject.toml` & `b2sdk-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "2.1.0"
+version = "2.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Backblaze/b2-sdk-python"
```

### Comparing `b2sdk-2.1.0/PKG-INFO` & `b2sdk-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2sdk
-Version: 2.1.0
+Version: 2.2.0
 Summary: Backblaze B2 SDK
 Keywords: backblaze,b2,cloud,storage
 Author-Email: Backblaze Inc <support@backblaze.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```


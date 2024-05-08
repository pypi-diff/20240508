# Comparing `tmp/whylogs-1.3.9.dev0.tar.gz` & `tmp/whylogs-1.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.3.9.dev0.tar", max compression
+gzip compressed data, was "whylogs-1.4.0rc0.tar", max compression
```

## Comparing `whylogs-1.3.9.dev0.tar` & `whylogs-1.4.0rc0.tar`

### file list

```diff
@@ -1,242 +1,252 @@
--rw-r--r--   0        0        0     3166 2023-06-27 17:33:07.264805 whylogs-1.3.9.dev0/DESCRIPTION.md
--rw-r--r--   0        0        0     6425 2023-10-04 20:19:08.594477 whylogs-1.3.9.dev0/pyproject.toml
--rw-r--r--   0        0        0     1801 2023-10-04 20:07:03.827570 whylogs-1.3.9.dev0/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2023-06-08 01:23:07.097906 whylogs-1.3.9.dev0/whylogs/api/annotations.py
--rw-r--r--   0        0        0      120 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2023-06-16 15:50:21.999413 whylogs-1.3.9.dev0/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0    10067 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0      101 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/events/__init__.py
--rw-r--r--   0        0        0     5599 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/events/event.py
--rw-r--r--   0        0        0      750 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/events/file_name.py
--rw-r--r--   0        0        0        0 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/__init__.py
--rw-r--r--   0        0        0     7857 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/actor.py
--rw-r--r--   0        0        0     2102 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/data_logger.py
--rw-r--r--   0        0        0     1539 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
--rw-r--r--   0        0        0      530 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/future_util.py
--rw-r--r--   0        0        0      650 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/list_util.py
--rw-r--r--   0        0        0     1628 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
--rw-r--r--   0        0        0      282 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
--rw-r--r--   0        0        0     2756 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_actor.py
--rw-r--r--   0        0        0    20221 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
--rw-r--r--   0        0        0     8364 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
--rw-r--r--   0        0        0      358 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/signal_util.py
--rw-r--r--   0        0        0      579 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/string_util.py
--rw-r--r--   0        0        0     2971 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/thread_actor.py
--rw-r--r--   0        0        0    17715 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
--rw-r--r--   0        0        0     4008 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/time_util.py
--rw-r--r--   0        0        0     5458 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    20448 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9549 2023-10-02 21:55:43.763605 whylogs-1.3.9.dev0/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2023-09-14 13:45:35.715676 whylogs-1.3.9.dev0/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     6462 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2023-05-31 17:44:36.663303 whylogs-1.3.9.dev0/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     6168 2023-08-16 17:11:22.596804 whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7663 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2023-03-03 16:21:20.616995 whylogs-1.3.9.dev0/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0    17933 2023-10-02 22:34:26.613605 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      354 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/lazy.py
--rw-r--r--   0        0        0      442 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3893 2023-10-02 22:34:26.613605 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0     2823 2023-10-02 22:34:26.613605 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/prompts.py
--rw-r--r--   0        0        0    13188 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session.py
--rw-r--r--   0        0        0     7029 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0     5095 2023-09-22 16:11:43.930291 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      278 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/why_init.py
--rw-r--r--   0        0        0     6586 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/whylabs_client_cache.py
--rw-r--r--   0        0        0      947 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     2726 2023-06-16 15:50:22.009413 whylogs-1.3.9.dev0/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     1169 2023-06-16 15:50:22.009413 whylogs-1.3.9.dev0/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2084 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     3408 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    42227 2023-10-04 20:17:38.537768 whylogs-1.3.9.dev0/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0     1211 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0        0 2023-10-04 20:06:57.677570 whylogs-1.3.9.dev0/whylogs/context/__init__.py
--rw-r--r--   0        0        0      302 2023-10-04 20:17:37.837768 whylogs-1.3.9.dev0/whylogs/context/environ.py
--rw-r--r--   0        0        0      502 2023-10-04 20:07:00.617570 whylogs-1.3.9.dev0/whylogs/context/version.py
--rw-r--r--   0        0        0     1090 2023-08-31 15:56:24.908582 whylogs-1.3.9.dev0/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3575 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/common.py
--rw-r--r--   0        0        0     1589 2023-07-19 19:51:34.012366 whylogs-1.3.9.dev0/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2023-05-25 19:20:19.422537 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2023-06-27 17:33:07.364805 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2023-05-25 19:20:19.422537 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2023-05-25 19:20:19.422537 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2023-06-27 17:33:07.364805 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2023-06-27 17:33:07.364805 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30661 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11337 2023-09-22 19:58:53.969842 whylogs-1.3.9.dev0/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4230 2023-07-19 19:51:34.012366 whylogs-1.3.9.dev0/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/errors.py
--rw-r--r--   0        0        0     2560 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     2045 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/core/metadata.py
--rw-r--r--   0        0        0     1740 2023-02-24 20:07:49.042231 whylogs-1.3.9.dev0/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2023-04-11 19:13:37.824666 whylogs-1.3.9.dev0/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2023-04-20 13:28:02.613992 whylogs-1.3.9.dev0/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0     7615 2023-06-27 17:33:07.364805 whylogs-1.3.9.dev0/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2023-04-11 19:13:37.824666 whylogs-1.3.9.dev0/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2023-07-04 17:04:07.025540 whylogs-1.3.9.dev0/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2023-06-06 15:22:27.487907 whylogs-1.3.9.dev0/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2023-04-11 19:13:37.824666 whylogs-1.3.9.dev0/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0    10663 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2023-02-24 20:07:49.042231 whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2023-02-24 20:07:49.042231 whylogs-1.3.9.dev0/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14608 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0    12534 2023-10-04 20:35:56.255776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2023-10-04 20:35:55.705776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    21343 2023-10-04 20:35:55.705776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2023-10-04 20:35:55.705776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0    18521 2023-10-04 20:35:56.365776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2023-10-04 20:35:55.705776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0    18571 2023-10-04 20:35:55.575776 whylogs-1.3.9.dev0/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2023-10-04 20:35:55.575776 whylogs-1.3.9.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2023-02-24 20:07:49.042231 whylogs-1.3.9.dev0/whylogs/core/relations.py
--rw-r--r--   0        0        0    11357 2023-07-19 19:51:34.012366 whylogs-1.3.9.dev0/whylogs/core/resolvers.py
--rw-r--r--   0        0        0    10061 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2023-03-22 21:08:17.851744 whylogs-1.3.9.dev0/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2023-04-20 13:28:02.623992 whylogs-1.3.9.dev0/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2118 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2023-06-27 17:33:07.374805 whylogs-1.3.9.dev0/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2023-06-23 19:18:55.967672 whylogs-1.3.9.dev0/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2023-06-27 17:33:07.374805 whylogs-1.3.9.dev0/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     2004 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      281 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4823 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1329 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2023-06-27 17:33:07.374805 whylogs-1.3.9.dev0/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    17867 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     9457 2023-10-04 14:11:26.367936 whylogs-1.3.9.dev0/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2023-03-24 22:58:37.321744 whylogs-1.3.9.dev0/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2023-03-24 22:58:37.321744 whylogs-1.3.9.dev0/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2023-03-24 22:58:37.321744 whylogs-1.3.9.dev0/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2023-03-03 16:19:17.576995 whylogs-1.3.9.dev0/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-19 19:51:34.012366 whylogs-1.3.9.dev0/whylogs/experimental/api/logger/__init__.py
--rw-r--r--   0        0        0     3770 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2023-03-28 21:40:50.417571 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    14428 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0      299 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/experimental/core/validators/__init__.py
--rw-r--r--   0        0        0     1218 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/experimental/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1262 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/experimental/core/validators/validator.py
--rw-r--r--   0        0        0     8861 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2023-02-14 19:22:29.792231 whylogs-1.3.9.dev0/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2023-03-03 16:19:17.576995 whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1554 2023-04-11 19:13:37.834666 whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2023-03-03 16:19:17.576995 whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2023-06-27 17:33:07.394805 whylogs-1.3.9.dev0/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    11126 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2023-02-27 17:39:54.122231 whylogs-1.3.9.dev0/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15564 2023-09-12 18:45:06.905676 whylogs-1.3.9.dev0/whylogs/migration/converters.py
--rw-r--r--   0        0        0     6992 2023-08-28 14:42:47.838581 whylogs-1.3.9.dev0/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    21751 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2023-03-24 22:58:37.321744 whylogs-1.3.9.dev0/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2502 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2023-05-25 19:20:19.432537 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2023-04-20 13:28:02.623992 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    22429 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2023-04-20 13:28:02.623992 whylogs-1.3.9.dev0/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1060 2023-04-20 13:28:02.623992 whylogs-1.3.9.dev0/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 whylogs-1.3.9.dev0/PKG-INFO
+-rw-r--r--   0        0        0     3166 2024-04-26 21:02:29.946175 whylogs-1.4.0rc0/DESCRIPTION.md
+-rw-r--r--   0        0        0     6650 2024-04-27 00:02:55.944051 whylogs-1.4.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1801 2024-04-26 21:02:30.063493 whylogs-1.4.0rc0/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-26 21:02:30.063708 whylogs-1.4.0rc0/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2024-04-26 21:02:30.063845 whylogs-1.4.0rc0/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      168 2024-04-26 21:02:30.064133 whylogs-1.4.0rc0/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2024-04-26 21:02:30.064351 whylogs-1.4.0rc0/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2024-04-26 21:02:30.064518 whylogs-1.4.0rc0/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0    12819 2024-04-26 21:02:57.083873 whylogs-1.4.0rc0/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0      101 2024-04-26 21:02:30.066009 whylogs-1.4.0rc0/whylogs/api/logger/events/__init__.py
+-rw-r--r--   0        0        0     5621 2024-04-26 21:02:30.066189 whylogs-1.4.0rc0/whylogs/api/logger/events/event.py
+-rw-r--r--   0        0        0      750 2024-04-26 21:02:30.066765 whylogs-1.4.0rc0/whylogs/api/logger/events/file_name.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.067049 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/__init__.py
+-rw-r--r--   0        0        0     7953 2024-04-26 21:02:30.068170 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/actor.py
+-rw-r--r--   0        0        0     2614 2024-04-26 21:02:30.068350 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/data_logger.py
+-rw-r--r--   0        0        0     1607 2024-04-26 21:02:30.068507 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
+-rw-r--r--   0        0        0     1557 2024-04-26 21:02:30.068753 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/future_util.py
+-rw-r--r--   0        0        0     1282 2024-04-26 21:02:30.068996 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/list_util.py
+-rw-r--r--   0        0        0     1638 2024-04-26 21:02:30.069153 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
+-rw-r--r--   0        0        0     5181 2024-04-26 21:02:30.069309 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/pipe_signaler.py
+-rw-r--r--   0        0        0      281 2024-04-26 21:02:30.069434 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
+-rw-r--r--   0        0        0     5476 2024-04-26 21:02:30.069598 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_actor.py
+-rw-r--r--   0        0        0    18881 2024-04-26 21:02:57.084243 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
+-rw-r--r--   0        0        0     9034 2024-04-26 21:02:30.074524 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
+-rw-r--r--   0        0        0      486 2024-04-26 21:02:30.074679 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/signal_util.py
+-rw-r--r--   0        0        0      641 2024-04-26 21:02:30.075590 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/string_util.py
+-rw-r--r--   0        0        0     3010 2024-04-26 21:02:30.076218 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py
+-rw-r--r--   0        0        0    18936 2024-04-26 21:02:30.076557 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
+-rw-r--r--   0        0        0     4225 2024-04-26 21:02:30.076782 whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/time_util.py
+-rw-r--r--   0        0        0     5777 2024-04-26 21:02:30.077041 whylogs-1.4.0rc0/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    22351 2024-04-26 21:02:57.084889 whylogs-1.4.0rc0/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9549 2024-04-26 21:02:30.077787 whylogs-1.4.0rc0/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2024-04-26 21:02:30.078010 whylogs-1.4.0rc0/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     7090 2024-04-26 21:02:30.079019 whylogs-1.4.0rc0/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2024-04-26 21:02:30.079308 whylogs-1.4.0rc0/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      406 2024-04-26 21:02:30.079668 whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     6178 2024-04-26 21:02:30.079867 whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7673 2024-04-26 21:02:30.080008 whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2024-04-26 21:02:30.080255 whylogs-1.4.0rc0/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2024-04-26 21:02:30.080389 whylogs-1.4.0rc0/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2024-04-26 21:02:30.080528 whylogs-1.4.0rc0/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2024-04-26 21:02:30.081205 whylogs-1.4.0rc0/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2024-04-26 21:02:30.081559 whylogs-1.4.0rc0/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2024-04-26 21:02:30.081764 whylogs-1.4.0rc0/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2024-04-26 21:02:30.082376 whylogs-1.4.0rc0/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2024-04-26 21:02:30.082644 whylogs-1.4.0rc0/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2024-04-26 21:02:30.083354 whylogs-1.4.0rc0/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2024-04-26 21:02:30.083784 whylogs-1.4.0rc0/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-26 21:02:30.084259 whylogs-1.4.0rc0/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0    18270 2024-04-26 21:02:30.084747 whylogs-1.4.0rc0/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      354 2024-04-26 21:02:30.084948 whylogs-1.4.0rc0/whylogs/api/whylabs/session/lazy.py
+-rw-r--r--   0        0        0      442 2024-04-26 21:02:30.085192 whylogs-1.4.0rc0/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3893 2024-04-26 21:02:30.085442 whylogs-1.4.0rc0/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0     2823 2024-04-26 21:02:30.085705 whylogs-1.4.0rc0/whylogs/api/whylabs/session/prompts.py
+-rw-r--r--   0        0        0    13613 2024-04-26 21:02:30.086301 whylogs-1.4.0rc0/whylogs/api/whylabs/session/session.py
+-rw-r--r--   0        0        0     6940 2024-04-26 21:02:30.086995 whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0     5142 2024-04-26 21:02:30.087545 whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      278 2024-04-26 21:02:30.087706 whylogs-1.4.0rc0/whylogs/api/whylabs/session/why_init.py
+-rw-r--r--   0        0        0     6581 2024-04-26 21:02:30.087863 whylogs-1.4.0rc0/whylogs/api/whylabs/session/whylabs_client_cache.py
+-rw-r--r--   0        0        0     6622 2024-04-26 21:18:13.863456 whylogs-1.4.0rc0/whylogs/api/writer/#whylabs_batch_writer.py#
+-rw-r--r--   0        0        0      152 2024-04-26 21:02:57.085198 whylogs-1.4.0rc0/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     3498 2024-04-26 21:02:57.085563 whylogs-1.4.0rc0/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     2300 2024-04-26 21:02:57.085930 whylogs-1.4.0rc0/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2421 2024-04-26 21:02:57.086194 whylogs-1.4.0rc0/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0        0 2024-04-27 00:05:16.106073 whylogs-1.4.0rc0/whylogs/api/writer/richard@richards-MacBook-Pro.26122
+-rw-r--r--   0        0        0     4021 2024-04-26 21:02:57.086609 whylogs-1.4.0rc0/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    11074 2024-04-26 22:54:01.723581 whylogs-1.4.0rc0/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0    10110 2024-04-26 21:02:57.087536 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_base.py
+-rw-r--r--   0        0        0     6633 2024-04-26 21:16:43.382854 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_batch_writer.py
+-rw-r--r--   0        0        0    38861 2024-04-26 21:02:57.088060 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_client.py
+-rw-r--r--   0        0        0     4167 2024-04-26 21:02:57.088290 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_estimation_result_writer.py
+-rw-r--r--   0        0        0     6678 2024-04-26 21:18:33.755656 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_reference_writer.py
+-rw-r--r--   0        0        0     6755 2024-04-26 22:35:16.271359 whylogs-1.4.0rc0/whylogs/api/writer/whylabs_transaction_writer.py
+-rw-r--r--   0        0        0     5433 2024-04-26 21:02:57.089133 whylogs-1.4.0rc0/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.089202 whylogs-1.4.0rc0/whylogs/context/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-26 21:02:30.089357 whylogs-1.4.0rc0/whylogs/context/environ.py
+-rw-r--r--   0        0        0      516 2024-04-26 21:02:30.090077 whylogs-1.4.0rc0/whylogs/context/version.py
+-rw-r--r--   0        0        0     1090 2024-04-26 21:02:30.090383 whylogs-1.4.0rc0/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3575 2024-04-26 21:02:30.090535 whylogs-1.4.0rc0/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2024-04-26 21:02:30.090670 whylogs-1.4.0rc0/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2024-04-26 21:02:30.090879 whylogs-1.4.0rc0/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2024-04-26 21:02:30.091165 whylogs-1.4.0rc0/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-26 21:02:30.091993 whylogs-1.4.0rc0/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2024-04-26 21:02:30.092239 whylogs-1.4.0rc0/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2024-04-26 21:02:30.092453 whylogs-1.4.0rc0/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2024-04-26 21:02:30.092612 whylogs-1.4.0rc0/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2024-04-26 21:02:30.092764 whylogs-1.4.0rc0/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2024-04-26 21:02:30.092928 whylogs-1.4.0rc0/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2024-04-26 21:02:30.093167 whylogs-1.4.0rc0/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2024-04-26 21:02:30.093863 whylogs-1.4.0rc0/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30661 2024-04-26 21:02:30.094241 whylogs-1.4.0rc0/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11321 2024-04-26 21:02:57.089842 whylogs-1.4.0rc0/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4230 2024-04-26 21:02:30.095454 whylogs-1.4.0rc0/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2024-04-26 21:02:30.096077 whylogs-1.4.0rc0/whylogs/core/errors.py
+-rw-r--r--   0        0        0     1400 2024-04-26 21:02:57.090158 whylogs-1.4.0rc0/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2024-04-26 21:02:30.096562 whylogs-1.4.0rc0/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     2987 2024-04-26 21:02:30.096782 whylogs-1.4.0rc0/whylogs/core/metadata.py
+-rw-r--r--   0        0        0     1740 2024-04-26 21:02:30.096939 whylogs-1.4.0rc0/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2024-04-26 21:02:30.097220 whylogs-1.4.0rc0/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2024-04-26 21:02:30.097456 whylogs-1.4.0rc0/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2024-04-26 21:02:30.097696 whylogs-1.4.0rc0/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2024-04-26 21:02:30.098380 whylogs-1.4.0rc0/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0    10678 2024-04-26 21:02:30.098841 whylogs-1.4.0rc0/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2024-04-26 21:02:30.099685 whylogs-1.4.0rc0/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2024-04-26 21:02:30.099997 whylogs-1.4.0rc0/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2024-04-26 21:02:30.100234 whylogs-1.4.0rc0/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2024-04-26 21:02:30.101104 whylogs-1.4.0rc0/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2024-04-26 21:02:30.101553 whylogs-1.4.0rc0/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2024-04-26 21:02:30.101832 whylogs-1.4.0rc0/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2024-04-26 21:02:30.102576 whylogs-1.4.0rc0/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2024-04-26 21:02:30.102850 whylogs-1.4.0rc0/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2024-04-26 21:02:30.103687 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0    10663 2024-04-26 21:02:30.104196 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2024-04-26 21:02:30.104467 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2024-04-26 21:02:30.104746 whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2024-04-26 21:02:30.105006 whylogs-1.4.0rc0/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14608 2024-04-26 21:02:30.105755 whylogs-1.4.0rc0/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2024-04-26 21:02:30.105951 whylogs-1.4.0rc0/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2024-04-26 21:02:30.106363 whylogs-1.4.0rc0/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2024-04-26 21:02:30.106838 whylogs-1.4.0rc0/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2024-04-26 23:53:13.202845 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2024-04-26 23:53:12.021184 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2024-04-26 23:53:12.023238 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2024-04-26 23:53:12.027712 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2024-04-26 23:53:13.448691 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2024-04-26 23:53:12.032451 whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2024-04-26 23:53:11.785488 whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2024-04-26 23:53:11.788864 whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2024-04-26 21:02:30.107160 whylogs-1.4.0rc0/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11357 2024-04-26 21:02:30.107626 whylogs-1.4.0rc0/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10754 2024-04-26 21:02:30.107983 whylogs-1.4.0rc0/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2024-04-26 21:02:30.108593 whylogs-1.4.0rc0/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2024-04-26 21:02:30.108833 whylogs-1.4.0rc0/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2024-04-26 21:02:30.109060 whylogs-1.4.0rc0/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2118 2024-04-26 21:02:30.109644 whylogs-1.4.0rc0/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2024-04-26 21:02:30.110010 whylogs-1.4.0rc0/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2024-04-26 21:02:30.110216 whylogs-1.4.0rc0/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2024-04-26 21:02:30.110377 whylogs-1.4.0rc0/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2024-04-26 21:02:30.110574 whylogs-1.4.0rc0/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     2004 2024-04-26 21:02:30.110740 whylogs-1.4.0rc0/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      281 2024-04-26 21:02:30.110948 whylogs-1.4.0rc0/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4823 2024-04-26 21:02:30.111113 whylogs-1.4.0rc0/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1329 2024-04-26 21:02:30.111610 whylogs-1.4.0rc0/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2024-04-26 21:02:30.111979 whylogs-1.4.0rc0/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2024-04-26 21:02:30.112333 whylogs-1.4.0rc0/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    18600 2024-04-26 21:02:57.090538 whylogs-1.4.0rc0/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     9474 2024-04-26 21:02:57.091117 whylogs-1.4.0rc0/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2024-04-26 21:02:30.113593 whylogs-1.4.0rc0/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2024-04-26 21:02:30.113832 whylogs-1.4.0rc0/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2024-04-26 21:02:30.114504 whylogs-1.4.0rc0/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.114862 whylogs-1.4.0rc0/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2024-04-26 21:02:30.115167 whylogs-1.4.0rc0/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2024-04-26 21:02:30.116132 whylogs-1.4.0rc0/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2024-04-26 21:02:30.116732 whylogs-1.4.0rc0/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2024-04-26 21:02:30.117401 whylogs-1.4.0rc0/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2024-04-26 21:02:30.117969 whylogs-1.4.0rc0/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2024-04-26 21:02:30.118208 whylogs-1.4.0rc0/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2024-04-26 21:02:30.118700 whylogs-1.4.0rc0/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.118942 whylogs-1.4.0rc0/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.119221 whylogs-1.4.0rc0/whylogs/experimental/api/__init__.py
+-rw-r--r--   0        0        0    15177 2024-04-26 21:02:30.119905 whylogs-1.4.0rc0/whylogs/experimental/api/logger/__init__.py
+-rw-r--r--   0        0        0     3770 2024-04-26 21:02:30.120168 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2024-04-26 21:02:30.120422 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2024-04-26 21:02:30.120686 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2024-04-26 21:02:30.120930 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2024-04-26 21:02:30.121140 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2024-04-26 21:02:30.121327 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2024-04-26 21:02:30.121539 whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2024-04-26 21:02:30.122243 whylogs-1.4.0rc0/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    19154 2024-04-26 21:02:30.122535 whylogs-1.4.0rc0/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0      299 2024-04-26 21:02:30.122823 whylogs-1.4.0rc0/whylogs/experimental/core/validators/__init__.py
+-rw-r--r--   0        0        0     1218 2024-04-26 21:02:30.122974 whylogs-1.4.0rc0/whylogs/experimental/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1698 2024-04-26 21:02:30.123128 whylogs-1.4.0rc0/whylogs/experimental/core/validators/validator.py
+-rw-r--r--   0        0        0     8861 2024-04-26 21:02:30.123654 whylogs-1.4.0rc0/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2024-04-26 21:02:30.123862 whylogs-1.4.0rc0/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2024-04-26 21:02:30.124080 whylogs-1.4.0rc0/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.124365 whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-26 21:02:57.091490 whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2024-04-26 21:02:30.126148 whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2024-04-26 21:02:30.128009 whylogs-1.4.0rc0/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    11126 2024-04-26 21:02:30.128727 whylogs-1.4.0rc0/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2024-04-26 21:02:30.129427 whylogs-1.4.0rc0/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15564 2024-04-26 21:02:30.130625 whylogs-1.4.0rc0/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     7662 2024-04-26 21:02:30.130849 whylogs-1.4.0rc0/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2024-04-26 21:02:30.131116 whylogs-1.4.0rc0/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-26 21:02:30.131338 whylogs-1.4.0rc0/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.131523 whylogs-1.4.0rc0/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    22069 2024-04-26 21:02:30.132305 whylogs-1.4.0rc0/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2024-04-26 21:02:30.132487 whylogs-1.4.0rc0/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.132653 whylogs-1.4.0rc0/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-26 21:02:30.132892 whylogs-1.4.0rc0/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2024-04-26 21:02:30.133697 whylogs-1.4.0rc0/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-26 21:02:30.133973 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2024-04-26 21:02:30.134163 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2171 2024-04-26 21:02:57.091852 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2024-04-26 21:02:30.135017 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2024-04-26 21:02:30.135259 whylogs-1.4.0rc0/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2024-04-26 21:02:30.135605 whylogs-1.4.0rc0/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2024-04-26 21:02:30.135825 whylogs-1.4.0rc0/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2024-04-26 21:02:30.136368 whylogs-1.4.0rc0/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2024-04-26 21:02:30.136699 whylogs-1.4.0rc0/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2024-04-26 21:02:30.137324 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2024-04-26 21:02:30.137795 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2024-04-26 21:02:30.163153 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2024-04-26 21:02:30.163664 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2024-04-26 21:02:30.164714 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2024-04-26 21:02:30.165330 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2024-04-26 21:02:30.165793 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2024-04-26 21:02:30.166103 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2024-04-26 21:02:30.166288 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2024-04-26 21:02:30.166714 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2024-04-26 21:02:30.167040 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2024-04-26 21:02:30.167237 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2024-04-26 21:02:30.167700 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2024-04-26 21:02:30.168007 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2024-04-26 21:02:30.168227 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2024-04-26 21:02:30.168656 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2024-04-26 21:02:30.169371 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2024-04-26 21:02:30.169558 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2024-04-26 21:02:30.170475 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2024-04-26 21:02:30.170829 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2024-04-26 21:02:30.171479 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2024-04-26 21:02:30.171957 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2024-04-26 21:02:30.172659 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2024-04-26 21:02:30.173258 whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2024-04-26 21:02:30.173506 whylogs-1.4.0rc0/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2024-04-26 21:02:30.173841 whylogs-1.4.0rc0/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2024-04-26 21:02:30.174623 whylogs-1.4.0rc0/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2024-04-26 21:02:30.175451 whylogs-1.4.0rc0/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2024-04-26 21:02:30.175796 whylogs-1.4.0rc0/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2024-04-26 21:02:30.176016 whylogs-1.4.0rc0/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2024-04-26 21:02:30.176733 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2024-04-26 21:02:30.177157 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2024-04-26 21:02:30.177379 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2024-04-26 21:02:30.177724 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2024-04-26 21:02:30.178049 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2024-04-26 21:02:30.178223 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2024-04-26 21:02:30.178408 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2024-04-26 21:02:30.179832 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2024-04-26 21:02:30.180443 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2024-04-26 21:02:30.180710 whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2024-04-26 21:02:30.180899 whylogs-1.4.0rc0/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    22429 2024-04-26 21:02:30.181067 whylogs-1.4.0rc0/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2024-04-26 21:02:30.181325 whylogs-1.4.0rc0/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2024-04-26 21:02:30.181455 whylogs-1.4.0rc0/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2024-04-26 21:02:30.182816 whylogs-1.4.0rc0/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2024-04-26 21:02:30.182997 whylogs-1.4.0rc0/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2024-04-26 21:02:30.186179 whylogs-1.4.0rc0/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1128 2024-04-26 21:02:30.186828 whylogs-1.4.0rc0/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2024-04-26 21:02:30.193627 whylogs-1.4.0rc0/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2024-04-26 21:02:30.193953 whylogs-1.4.0rc0/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     7007 1970-01-01 00:00:00.000000 whylogs-1.4.0rc0/PKG-INFO
```

### Comparing `whylogs-1.3.9.dev0/DESCRIPTION.md` & `whylogs-1.4.0rc0/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/pyproject.toml` & `whylogs-1.4.0rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.3.9-dev0"
+version = "1.4.0-rc0"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
 
@@ -12,15 +12,15 @@
 [tool.poetry.dependencies]
 # core dependencies. Be REALLY mindful when touching this list
 python = ">=3.7.1, <4"
 whylogs-sketching = ">=3.4.1.dev3"
 protobuf = ">=3.19.4"
 importlib-metadata = { version = "<4.3", python = "<3.8" }
 typing-extensions = {version = ">=3.10", markers = "python_version < \"4\""}
-whylabs-client = "^0.5.6"
+whylabs-client = "^0.6.2"
 requests = "^2.27"
 types-requests = "^2.30.0.0"
 
 # viz module. Everything after this should be optional
 pybars3 = { version = "^0.9", optional = true }
 ipython = { version = "*", optional = true }
 scipy = [
@@ -174,14 +174,15 @@
 pandas-stubs = "*"
 ipykernel = ">=6.11" # for developing in Jupyter notebook
 types-python-dateutil = "^2.8.12"
 moto = "^4.1.6"
 twine = "^4.0.1"
 gcp-storage-emulator = "^2022.6.11"
 types-urllib3 = "^1.26.25.5"
+pyright = "^1.1.338"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
@@ -262,7 +263,15 @@
     | whylogs/core/proto
     | docs
   )/
   | foo.py           # also separately exclude a file named foo.py in
                      # the root of the project
 )
 '''
+
+[tool.pyright]
+include = ["whylogs/api/logger/experimental/logger/**/*.py"]
+typeCheckingMode = "strict"
+
+reportMissingTypeStubs = false
+reportMissingParameterType = false
+reportMissingTypeArgumet = false
```

### Comparing `whylogs-1.3.9.dev0/whylogs/__init__.py` & `whylogs-1.4.0rc0/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/annotations.py` & `whylogs-1.4.0rc0/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/fugue/profiler.py` & `whylogs-1.4.0rc0/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/fugue/registry.py` & `whylogs-1.4.0rc0/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/__init__.py` & `whylogs-1.4.0rc0/whylogs/api/logger/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from whylogs.api.logger.transient import TransientLogger
 from whylogs.api.usage_stats import emit_usage
 from whylogs.api.whylabs.session.notebook_logger import (
     notebook_session_log,
     notebook_session_log_comparison,
 )
 from whylogs.core import DatasetProfile, DatasetSchema
+from whylogs.core.metadata import WHYLABS_TRACE_ID_KEY
 from whylogs.core.model_performance_metrics.model_performance_metrics import (
     ModelPerformanceMetrics,
 )
 from whylogs.core.stubs import pd
 
 diagnostic_logger = logging.getLogger(__name__)
 
@@ -68,14 +69,16 @@
             obj, pandas=pandas, row=row, name=name, trace_id=trace_id, tags=tags, segment_key_values=segment_key_values
         )
         if dataset_timestamp is not None:
             result_set.set_dataset_timestamp(dataset_timestamp)
         notebook_session_log(result_set, obj, pandas=pandas, row=row, name=name)
 
         if debug_event is not None:
+            if trace_id is None and WHYLABS_TRACE_ID_KEY in result_set.metadata:
+                trace_id = result_set.metadata.get(WHYLABS_TRACE_ID_KEY)
             debug_event_status = log_debug_event(
                 debug_event=debug_event,
                 trace_id=trace_id,
                 tags=tags,
                 segment_key_values=segment_key_values,
                 dataset_timestamp=dataset_timestamp,
             )
@@ -163,23 +166,57 @@
     log_full_data: bool = False,
     dataset_timestamp: Optional[datetime] = None,
 ) -> ResultSet:
     """
     Function to track metrics based on validation data.
     user may also pass the associated attribute names associated with
     target, prediction, and/or score.
+
     Parameters
     ----------
-    targets : List[Union[str, bool, float, int]]
-        actual validated values
-    predictions : List[Union[str, bool, float, int]]
-        inferred/predicted values
-    scores : List[float], optional
-        assocaited scores for each inferred, all values set to 1 if not
-        passed
+    data : pd.DataFrame
+        Dataframe with the data to log.
+    target_column : str
+        Column name for the actual validated values.
+    prediction_column : str
+        Column name for the predicted values.
+    score_column : Optional[str], optional
+        Associated scores for each inferred, all values set to 1 if None, by default None
+    schema : Optional[DatasetSchema], optional
+        Defines the schema for tracking metrics in whylogs, by default None
+    log_full_data : bool, optional
+        Whether to log the complete dataframe or not.
+        If True, the complete DF will be logged in addition to the regression metrics.
+        If False, only the calculated regression metrics will be logged.
+        In a typical production use case, the ground truth might not be available
+        at the time the remaining data is generated. In order to prevent double profiling the
+        input features, consider leaving this as False. by default False.
+    dataset_timestamp : Optional[datetime], optional
+        dataset's timestamp, by default None
+
+    Examples
+    --------
+    ::
+
+        data = {
+            "product": ["milk", "carrot", "cheese", "broccoli"],
+            "category": ["dairies", "vegetables", "dairies", "vegetables"],
+            "output_discount": [0, 0, 1, 1],
+            "output_prediction": [0, 0, 0, 1],
+        }
+        df = pd.DataFrame(data)
+
+        results = why.log_classification_metrics(
+                df,
+                target_column="output_discount",
+                prediction_column="output_prediction",
+                log_full_data=True,
+            )
+
+
     """
 
     perf_column_mapping = {"predictions": prediction_column, "targets": target_column, "scores": score_column}
 
     if schema and schema.segments:
         return _segmented_performance_metrics(
             log_full_data,
@@ -207,27 +244,52 @@
     data: pd.DataFrame,
     target_column: str,
     prediction_column: str,
     schema: Optional[DatasetSchema] = None,
     log_full_data: bool = False,
     dataset_timestamp: Optional[datetime] = None,
 ) -> ResultSet:
-    """
-    Function to track regression metrics based on validation data.
-    user may also pass the associated attribute names associated with
-    target, prediction, and/or score.
+    """Function to track regression metrics based on validation data.
+    User may also pass the associated attribute names associated with target, prediction, and/or score.
+
     Parameters
     ----------
-    targets : List[Union[str, bool, float, int]]
-        actual validated values
-    predictions : List[Union[str, bool, float, int]]
-        inferred/predicted values
-    scores : List[float], optional
-        assocaited scores for each inferred, all values set to 1 if not
-        passed
+    data : pd.DataFrame
+        Dataframe with the data to log.
+    target_column : str
+        Column name for the target values.
+    prediction_column : str
+        Column name for the predicted values.
+    schema : Optional[DatasetSchema], optional
+        Defines the schema for tracking metrics in whylogs, by default None
+    log_full_data : bool, optional
+        Whether to log the complete dataframe or not.
+        If True, the complete DF will be logged in addition to the regression metrics.
+        If False, only the calculated regression metrics will be logged.
+        In a typical production use case, the ground truth might not be available
+        at the time the remaining data is generated. In order to prevent double profiling the
+        input features, consider leaving this as False. by default False.
+    dataset_timestamp : Optional[datetime], optional
+        dataset's timestamp, by default None
+
+    Returns
+    -------
+    ResultSet
+
+    Examples
+    --------
+    ::
+
+        import pandas as pd
+        import whylogs as why
+
+        df = pd.DataFrame({"target_temperature": [[10.5, 24.3, 15.6]], "predicted_temperature": [[9.12,26.42,13.12]]})
+        results = why.log_regression_metrics(df, target_column = "temperature", prediction_column = "prediction_temperature")
+
+
     """
     perf_column_mapping: Dict[str, Optional[str]] = {"predictions": prediction_column, "targets": target_column}
 
     if schema and schema.segments:
         return _segmented_performance_metrics(
             log_full_data,
             schema=schema,
@@ -254,16 +316,19 @@
     return ResultSet.read(path)
 
 
 def reader(name: str) -> ResultSetReader:
     return ResultSet.reader(name=name)
 
 
-def write(profile: DatasetProfile, base_dir: str) -> None:
-    return profile.write(base_dir)
+def write(profile: DatasetProfile, base_dir: Optional[str] = None, filename: Optional[str] = None) -> None:
+    if base_dir and filename:
+        return profile.write(base_dir, filename)
+    else:
+        return profile.write("", base_dir)  # backward compatibility: use base_dir as full filename
 
 
 def logger(
     schema: Optional[DatasetSchema] = None,
     *,
     mode: Literal["transient", "rolling"] = "transient",
     **kwargs: Any,
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/events/event.py` & `whylogs-1.4.0rc0/whylogs/api/logger/events/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from datetime import datetime, timezone
 from typing import Any, Dict, List, Optional
 
 from whylabs_client import ApiClient
 from whylabs_client.api.debug_events_api import DebugEventsApi
 
-from whylogs.api.whylabs.session.session_manager import _default_init
+from whylogs.api.whylabs.session.session_manager import default_init
 from whylogs.api.whylabs.session.whylabs_client_cache import (
     ClientCacheConfig,
     WhylabsClientCache,
 )
 from whylogs.core.metadata import _populate_common_profile_metadata
 from whylogs.core.utils import ensure_timezone
 from whylogs.core.utils.timestamp_calculations import to_utc_milliseconds
@@ -25,23 +25,23 @@
         self,
         api_client: Optional[ApiClient] = None,
         org_id: Optional[str] = None,
         dataset_id: Optional[str] = None,
         ssl_ca_cert: Optional[str] = None,
     ):
         if api_client is None:
-            session = _default_init()
+            session = default_init()
             config = session.config
             self._cache_config = ClientCacheConfig(
                 ssl_ca_cert=ssl_ca_cert,
                 api_key=config.require_api_key(),
             )
             cache = WhylabsClientCache.instance()
             self._api_client, _ = cache.get_client(self._cache_config)
-            self._org_id = config.require_api_key().split(":")[-1]
+            self._org_id = config.require_org_id()
             self._dataset_id = config.require_default_dataset_id()
         else:
             self._api_client = api_client
             self._org_id = org_id
             self._dataset_id = dataset_id
         self._debug_events_api = DebugEventsApi(self._api_client)
 
@@ -73,21 +73,21 @@
                         f"{segment_key}: {segment_value}, converting to str"
                     )
                     segment_value = str(segment_value)
                 segment_tags.append(SegmentTag(key=segment_key, value=segment_value))
         debug_segment = Segment(tags=segment_tags)
         if dataset_timestamp is not None:
             ensure_timezone(dataset_timestamp)
-        checked_dataset_timestamp = dataset_timestamp or now_ms
+        dataset_timestamp_in_ms = to_utc_milliseconds(dataset_timestamp) if dataset_timestamp else now_ms
         whylabs_debug_event = DebugEvent(
             content=json.dumps(debug_event),
             trace_id=trace_id,
             tags=tags,
             segment=debug_segment,
-            dataset_timestamp=checked_dataset_timestamp,
+            dataset_timestamp=dataset_timestamp_in_ms,
             creation_timestamp=now_ms,
         )
         # TODO: retry
         try:
             status = self._debug_events_api.log_debug_event(
                 org_id=self._org_id, dataset_id=self._dataset_id, debug_event=whylabs_debug_event
             )
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/events/file_name.py` & `whylogs-1.4.0rc0/whylogs/api/logger/events/file_name.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/actor.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/actor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import logging
 import queue
-import signal
 import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Generic, List, Optional, Type, TypeVar, Union
 
 from whylogs.api.logger.experimental.logger.actor.list_util import type_batched_items
-from whylogs.api.logger.experimental.logger.actor.signal_util import suspended_signals
 
 QueueMessageType = TypeVar("QueueMessageType")
-_DEFAULT_TIMEOUT = 0.1
+DEFAULT_TIMEOUT = 0.1
 
 
-class QueueWrapper(Generic[QueueMessageType]):
+class QueueWrapper(ABC, Generic[QueueMessageType]):
     @abstractmethod
-    def send(self, message: QueueMessageType, timeout: float = _DEFAULT_TIMEOUT) -> None:
+    def send(self, message: QueueMessageType, timeout: float = DEFAULT_TIMEOUT) -> None:
         raise NotImplementedError()
 
     @abstractmethod
-    def send_many(self, message: QueueMessageType, timeout: float = _DEFAULT_TIMEOUT) -> None:
+    def send_many(self, messages: List[QueueMessageType], timeout: float = DEFAULT_TIMEOUT) -> None:
         raise NotImplementedError()
 
     @abstractmethod
-    def get(self, timeout: float = _DEFAULT_TIMEOUT) -> Optional[QueueMessageType]:
+    def get(self, timeout: float = DEFAULT_TIMEOUT) -> Optional[QueueMessageType]:
         raise NotImplementedError()
 
     @abstractmethod
-    def get_many(self, timeout: float = _DEFAULT_TIMEOUT, max: Optional[int] = None) -> List[QueueMessageType]:
+    def get_many(self, timeout: float = DEFAULT_TIMEOUT, max: Optional[int] = None) -> List[QueueMessageType]:
         raise NotImplementedError()
 
     @abstractmethod
     def size(self) -> int:
         raise NotImplementedError()
 
     @abstractmethod
@@ -39,15 +37,15 @@
         raise NotImplementedError()
 
 
 class CloseMessage:
     pass
 
 
-@dataclass
+@dataclass(frozen=True)
 class QueueConfig:
     """
     Configuration for the queue used by the actor.
 
     Parameters
     ----------
     max_batch_size : int
@@ -57,35 +55,34 @@
     message_poll_wait : float
         How long to block when polling for messages in a loop.
     """
 
     max_batch_size: int = 50_000
     message_accumualtion_duration: float = 1.0  # seconds
     message_poll_wait: float = 0.1  # seconds
+    max_buffer_bytes: int = 100_000_000  # 100 MB
 
 
 MessageType = TypeVar("MessageType")
-Messages = Union[MessageType, CloseMessage]
 
 
 class Actor(ABC, Generic[MessageType]):
     """
     Simple actor inspired interface designed for batch processing messages.
     This was created with thread and process based whylogs logging in mind and it has
     all of the common message passing logic needed.
     """
 
     def __init__(
         self,
-        queue_wrapper: QueueWrapper[Messages],
+        queue_wrapper: QueueWrapper[Union[MessageType, CloseMessage]],
         queue_config: QueueConfig = QueueConfig(),
     ) -> None:
-        self._queue: QueueWrapper[Messages] = queue_wrapper
+        self._queue: QueueWrapper[Union[MessageType, CloseMessage]] = queue_wrapper
         self._logger = logging.getLogger(f"ai.whylabs.actor.{type(self).__name__}")
-        self._logger.setLevel(logging.DEBUG)
         self._queue_config = queue_config
         super().__init__()
 
     @abstractmethod
     def close_message_handled(self) -> bool:
         raise NotImplementedError()
 
@@ -120,18 +117,20 @@
     def set_closed(self) -> None:
         """
         Sets this actor as closed, meaning it should no longer accept messages.
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def process_batch(self, batch: List[Messages], batch_type: Type) -> None:
+    def process_batch(
+        self, batch: List[Union[MessageType, CloseMessage]], batch_type: Type[Union[MessageType, CloseMessage]]
+    ) -> None:
         raise NotImplementedError()
 
-    def send(self, message: Messages) -> None:
+    def send(self, message: Union[MessageType, CloseMessage]) -> None:
         if self.is_closed():
             raise Exception("Actor is closed, can't send message.")
 
         if isinstance(message, CloseMessage):
             self.set_closed()
 
         done = False
@@ -149,16 +148,17 @@
                     )
                     done = True
                 else:
                     self._logger.warning(f"Message queue full, trying again. Current size :{self._queue.size()}")
             except Exception as e:
                 self._logger.exception(e)
 
-    def send_many(self, messages: List[Messages]) -> None:
-        self._queue.send_many(messages)
+    def send_many(self, messages: List[Union[MessageType, CloseMessage]]) -> None:
+        for message in messages:
+            self._queue.send(message)
 
     def close(self) -> None:
         self._logger.info("Sending Close message.")
         self.send(CloseMessage())
         self._logger.info(f"Shutdown after all pending {self._queue.size()} messages have been processed.")
         self.done_wait()
 
@@ -172,40 +172,43 @@
             return False
 
         if time.perf_counter() - last_message_time > self._queue_config.message_accumualtion_duration:
             return False
 
         return True
 
-    def _load_messages(self) -> Optional[List[Messages]]:
+    def _load_messages(self) -> Optional[List[Union[MessageType, CloseMessage]]]:
         max = self._queue_config.max_batch_size
-        batch: List[Messages] = []
+        batch: List[Union[MessageType, CloseMessage]] = []
         last_message_time = time.perf_counter()
 
         while self._polling_condition(len(batch), max, last_message_time, self._queue.size()):
             try:
-                batch += self._queue.get_many(timeout=self._queue_config.message_poll_wait, max=max)
-                self._logger.info(f"Got {len(batch)} messages. {self._queue.size()} remaining")
+                next_batch = self._queue.get_many(timeout=self._queue_config.message_poll_wait, max=max)
+                batch += next_batch
+                self._logger.debug(
+                    f"Adding {len(next_batch)} to poll batch of length {len(batch)}. {self._queue.size()} remaining"
+                )
             except queue.Empty:
                 if self.is_closed() and self.close_message_handled():
                     self._logger.info("Queue closed and no more messages to process.")
                     return None if batch == [] else batch
 
         return batch
 
     def process_messages(self) -> None:
-        messages: Optional[List[Messages]] = []
+        messages: Optional[List[Union[MessageType, CloseMessage]]] = []
         while messages is not None:
             messages = self._load_messages()
 
-            if messages is None:
+            if not messages:
                 continue
 
             for batch, batch_type in type_batched_items(messages):
-                if batch == []:
+                if batch is None or batch_type is None:
                     continue
 
                 self._logger.info(
                     f"Processing batch of {len(batch)} {batch_type.__name__}. {self._queue.size()} remaining"
                 )
 
                 try:
@@ -219,17 +222,13 @@
                     self._logger.exception(e)
 
         # Can only get here if we're done processing messages
         self.set_done()
 
     def run(self) -> None:
         try:
-            with suspended_signals(signal.SIGINT, signal.SIGTERM):
-                self.process_messages()
-        except KeyboardInterrupt:
-            # Swallow this to prevent annoying stack traces in dev.
-            pass
+            self.process_messages()
         except Exception as e:
             self._logger.error("Error while in main processing loop")
             self._logger.exception(e)
         finally:
             self._logger.info("Shutting down.")
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-from typing import Generic, List, Optional, TypeVar
+from typing import Any, Generic, List, Optional, TypeVar
 
 from whylogs.api.logger.experimental.logger.actor.actor import (
-    _DEFAULT_TIMEOUT,
+    DEFAULT_TIMEOUT,
+    QueueConfig,
     QueueWrapper,
 )
 
 try:
     from faster_fifo import Queue as FasterQueue  # type: ignore
 except ImportError:
     from whylogs.api.logger.experimental.logger.actor.proc_error_message import (
-        _proc_error_message,
+        proc_error_message,
     )
 
-    raise ImportError(_proc_error_message)
+    raise ImportError(proc_error_message)
 
-_DEFAULT_QUEUE_SiZE = 1000 * 1000 * 1000
 
 FasterQueueMessageType = TypeVar("FasterQueueMessageType")
 
 
-class FasterQueueWrapper(QueueWrapper, Generic[FasterQueueMessageType]):
+class FasterQueueWrapper(QueueWrapper[FasterQueueMessageType], Generic[FasterQueueMessageType]):
     """
     Implementation of QueueWrapper sufficient for use in the threaded actor.
     """
 
-    def __init__(self) -> None:
-        self._queue = FasterQueue(_DEFAULT_QUEUE_SiZE)
+    def __init__(self, config: QueueConfig) -> None:
+        # fasterfifo doesn't have types
+        self._queue: Any = FasterQueue(config.max_buffer_bytes)
 
-    def send(self, message: FasterQueueMessageType, timeout: float = _DEFAULT_TIMEOUT) -> None:
+    def send(self, message: FasterQueueMessageType, timeout: float = DEFAULT_TIMEOUT) -> None:
         self._queue.put(message, timeout=timeout)
 
-    def send_many(self, messages: List[FasterQueueMessageType], timeout: float = _DEFAULT_TIMEOUT) -> None:
+    def send_many(self, messages: List[FasterQueueMessageType], timeout: float = DEFAULT_TIMEOUT) -> None:
         self._queue.put_many(messages, timeout=timeout)
 
-    def get(self, timeout: float = _DEFAULT_TIMEOUT) -> Optional[FasterQueueMessageType]:
+    def get(self, timeout: float = DEFAULT_TIMEOUT) -> Optional[FasterQueueMessageType]:
         return self._queue.get(timeout=timeout)
 
-    def get_many(self, timeout: float = _DEFAULT_TIMEOUT, max: Optional[int] = None) -> List[FasterQueueMessageType]:
+    def get_many(self, timeout: float = DEFAULT_TIMEOUT, max: Optional[int] = None) -> List[FasterQueueMessageType]:
         return self._queue.get_many(timeout=timeout, max_messages_to_get=max)
 
     def size(self) -> int:
         return self._queue.qsize()
 
     def close(self) -> None:
         self._queue.close()
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from multiprocessing import Queue
 from queue import Empty
 from typing import Generic, List, Optional, TypeVar
 
 from whylogs.api.logger.experimental.logger.actor.actor import (
-    _DEFAULT_TIMEOUT,
+    DEFAULT_TIMEOUT,
     QueueWrapper,
 )
 
 MPWrapperType = TypeVar("MPWrapperType")
 
 
-class MPQueueWrapper(QueueWrapper, Generic[MPWrapperType]):
+class MPQueueWrapper(QueueWrapper[MPWrapperType], Generic[MPWrapperType]):
     """
     Implementation of QueueWrapper sufficient for use in the threaded actor.
     """
 
     def __init__(self) -> None:
         self._queue: Queue[MPWrapperType] = Queue(100_000)
 
-    def send(self, message: MPWrapperType, timeout: float = _DEFAULT_TIMEOUT) -> None:
+    def send(self, message: MPWrapperType, timeout: float = DEFAULT_TIMEOUT) -> None:
         self._queue.put(message, timeout=timeout)
 
-    def send_many(self, messages: List[MPWrapperType], timeout: float = _DEFAULT_TIMEOUT) -> None:
+    def send_many(self, messages: List[MPWrapperType], timeout: float = DEFAULT_TIMEOUT) -> None:
         for message in messages:
             self._queue.put(message, timeout=timeout)
 
-    def get(self, timeout: float = _DEFAULT_TIMEOUT) -> Optional[MPWrapperType]:
+    def get(self, timeout: float = DEFAULT_TIMEOUT) -> Optional[MPWrapperType]:
         return self._queue.get(timeout=timeout)
 
-    def get_many(self, timeout: float = _DEFAULT_TIMEOUT, max: Optional[int] = None) -> List[MPWrapperType]:
+    def get_many(self, timeout: float = DEFAULT_TIMEOUT, max: Optional[int] = None) -> List[MPWrapperType]:
         if max is None or max < 1:
             return []
 
         messages: List[MPWrapperType] = []
 
         while True:
             if len(messages) >= max:
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_actor.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_actor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,105 @@
-import multiprocessing as mp
-import sys
-from enum import Enum
-from typing import Generic, TypeVar
+import queue
+import threading as th
+from typing import Generic, List, Optional, TypeVar
 
 from whylogs.api.logger.experimental.logger.actor.actor import (
+    DEFAULT_TIMEOUT,
     Actor,
     QueueConfig,
     QueueWrapper,
 )
 
+DefaultQueueWrapperType = TypeVar("DefaultQueueWrapperType")
 
-class QueueType(Enum):
-    MP = "MP"
-    FASTER_FIFO = "FASTER_FIFO"
 
+class ThreadQueueWrapper(QueueWrapper[DefaultQueueWrapperType], Generic[DefaultQueueWrapperType]):
+    """
+    Implementation of QueueWrapper sufficient for use in the threaded actor.
+    """
+
+    def __init__(self) -> None:
+        self._queue: queue.Queue[DefaultQueueWrapperType] = queue.Queue(100_000)
+
+    def send(self, message: DefaultQueueWrapperType, timeout: float = DEFAULT_TIMEOUT) -> None:
+        self._queue.put(message, timeout=timeout)
+
+    def send_many(self, messages: List[DefaultQueueWrapperType], timeout: float = DEFAULT_TIMEOUT) -> None:
+        for message in messages:
+            self._queue.put(message, timeout=timeout)
+
+    def get(self, timeout: float = DEFAULT_TIMEOUT) -> Optional[DefaultQueueWrapperType]:
+        return self._queue.get(timeout=timeout)
+
+    def get_many(self, timeout: float = DEFAULT_TIMEOUT, max: Optional[int] = None) -> List[DefaultQueueWrapperType]:
+        if max is None or max < 1:
+            return []
+
+        messages: List[DefaultQueueWrapperType] = []
 
-ProcessMessageType = TypeVar("ProcessMessageType")
+        while True:
+            if len(messages) >= max:
+                break
 
+            try:
+                messages.append(self._queue.get(timeout=timeout))
+            except queue.Empty:
+                if len(messages) == 0:
+                    raise queue.Empty
+                else:
+                    break
 
-class ProcessActor(Actor, mp.Process, Generic[ProcessMessageType]):
+        return messages
+
+    def size(self) -> int:
+        return self._queue.qsize()
+
+    def close(self) -> None:
+        pass
+
+
+ThreadMessageType = TypeVar("ThreadMessageType")
+
+
+class ThreadActor(Actor[ThreadMessageType], th.Thread, Generic[ThreadMessageType]):
     """
-    Subclass of Actor that uses a process to process messages.
+    Subclass of Actor that uses a thread to process messages.
     """
 
-    def __init__(
-        self, queue_config: QueueConfig = QueueConfig(), queue_type: QueueType = QueueType.FASTER_FIFO
-    ) -> None:
-        self._wrapper: QueueWrapper[ProcessMessageType]
-        if queue_type == QueueType.MP:
-            from whylogs.api.logger.experimental.logger.actor.mp_queue_wrapper import (
-                MPQueueWrapper,
-            )
-
-            self._wrapper = MPQueueWrapper()
-        elif queue_type == QueueType.FASTER_FIFO:
-            from whylogs.api.logger.experimental.logger.actor.faster_fifo_queue_wrapper import (
-                FasterQueueWrapper,
-            )
-
-            self._wrapper = FasterQueueWrapper()
-        else:
-            raise ValueError(f"Unknown queue type: {queue_type}")
-
-        self._event = mp.Event()
-        self._is_closed = mp.Event()
-        self._close_handled = mp.Event()
-        # our mypy version has a false positive on this super call
-        super().__init__(self._wrapper, queue_config)  # type: ignore
+    def __init__(self, queue_config: QueueConfig = QueueConfig()) -> None:
+        # mypy can't infer but pyright can
+        super().__init__(ThreadQueueWrapper(), queue_config)  # type: ignore
+        self._event = th.Event()
+        self._is_closed = th.Event()
+        self._close_handled = th.Event()
+        self.daemon = True
+        self.start()
+
+    def run(self) -> None:
+        super().run()
 
     def close_message_handled(self) -> bool:
         return self._close_handled.is_set()
 
     def set_close_message_handled(self) -> None:
         self._close_handled.set()
 
     def close_message_wait(self) -> None:
         self._close_handled.wait()
 
     def is_done(self) -> bool:
         return self._event.is_set()
 
-    def done_wait(self) -> None:
-        self._event.wait()
-
     def set_done(self) -> None:
         self._event.set()
 
+    def done_wait(self) -> None:
+        self._event.wait()
+
     def set_closed(self) -> None:
         self._is_closed.set()
 
     def is_closed(self) -> bool:
         return self._is_closed.is_set()
 
     def close(self) -> None:
-        if self.pid is None:
-            raise Exception("Process hasn't been started yet.")
-
         super().close()
-        self._wrapper.close()
-
-    def run(self) -> None:
-        super().run()
-        sys.exit(0)
-
-    def start(self) -> None:
-        """
-        The process version of the actor apparently has to be manually started after
-        it's created, unlike the thread version which can just be automatically started
-        from within its init. There must be some post-init setup that needs to be done.
-        """
-        self.daemon = True
-        super().start()
-        self.join(0.1)  # This does apparently need to happen after several manual tests.
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,61 @@
-import logging
-import multiprocessing as mp
 import os
-import threading as th
 import time
 from abc import abstractmethod
 from concurrent.futures import Future
+from dataclasses import dataclass, field
 from functools import reduce
 from itertools import groupby
 from typing import (
-    Any,
     Callable,
     Dict,
+    Generic,
     List,
+    NoReturn,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
-from whylogs.api.whylabs.session.config import _INIT_DOCS
+from whylogs.api.whylabs.session.config import INIT_DOCS
+from whylogs.api.whylabs.session.session_manager import default_init
 
 try:
-    import orjson
+    import orjson  # type: ignore
 except ImportError:
     from whylogs.api.logger.experimental.logger.actor.proc_error_message import (
-        _proc_error_message,
+        proc_error_message,
     )
 
-    raise ImportError(_proc_error_message)
+    raise ImportError(proc_error_message)
+
+# Pandas/numpy required in the proc extra that this class requires
+import pandas as pd
 
 from whylogs.api.logger.experimental.logger.actor.actor import CloseMessage, QueueConfig
 from whylogs.api.logger.experimental.logger.actor.data_logger import (
     DataLogger,
     TrackData,
 )
-from whylogs.api.logger.experimental.logger.actor.future_util import wait_result
+from whylogs.api.logger.experimental.logger.actor.future_util import wait_result_while
 from whylogs.api.logger.experimental.logger.actor.process_actor import (
     ProcessActor,
     QueueType,
 )
 from whylogs.api.logger.experimental.logger.actor.process_rolling_logger_messages import (
     DataDict,
     FlushMessage,
     LogEmbeddingRequestDict,
     LogMessage,
     LogRequestDict,
     ProcessLoggerStatus,
-    ProcessLoggerStatusMessage,
+    ProcessStatusMessage,
     RawLogEmbeddingsMessage,
     RawLogMessage,
     RawPubSubEmbeddingMessage,
     RawPubSubMessage,
     data_dict_from_pandas,
     determine_dataset_timestamp,
     get_columns,
@@ -68,211 +71,270 @@
     ThreadRollingLogger,
 )
 from whylogs.api.logger.experimental.logger.actor.time_util import (
     Schedule,
     TimeGranularity,
     current_time_ms,
 )
-from whylogs.api.whylabs.session.session_manager import get_current_session
 from whylogs.api.writer import Writer, Writers
 from whylogs.core.schema import DatasetSchema
-from whylogs.core.stubs import pd
-
-MessageType = Union[
-    FlushMessage,
-    RawLogMessage,
-    RawLogEmbeddingsMessage,
-    RawPubSubMessage,
-    RawPubSubEmbeddingMessage,
-    LogMessage,
-    CloseMessage,
-    ProcessLoggerStatusMessage,
-]
 
 DataTypes = Union[str, int, float, bool, List[float], List[int], List[str]]
 
-DictType = TypeVar("DictType", bound="Union[LogRequestDict, LogEmbeddingRequestDict]")
-Loggable = Union[pd.DataFrame, Dict[str, Any]]
+DictType = TypeVar("DictType", LogRequestDict, LogEmbeddingRequestDict)
+# Loggable = Union[pd.DataFrame, Dict[str, Any], "np.ndarray[Any, Any]"]
 
 
 class WriterFactory:
     @abstractmethod
     def create_writers(self, dataset_id: str) -> List[Writer]:
         raise NotImplementedError()
 
 
 class WhyLabsWriterFactory(WriterFactory):
     def create_writers(self, dataset_id: str) -> List[Writer]:
         return [
-            Writers.get(
+            Writers.get(  # type: ignore
                 "whylabs",
                 dataset_id=dataset_id,
             )
         ]
 
 
-class ProcessRollingLogger(ProcessActor[MessageType], DataLogger[Dict[str, ProcessLoggerStatus]]):
+@dataclass
+class LoggerOptions:
+    aggregate_by: TimeGranularity = TimeGranularity.Hour
+    write_schedule: Optional[Schedule] = field(
+        default_factory=lambda: Schedule(cadence=TimeGranularity.Minute, interval=5)
+    )
+    schema: Optional[DatasetSchema] = None
+    sync_enabled: bool = False
+    current_time_fn: Optional[Callable[[], int]] = None
+    queue_config: QueueConfig = QueueConfig()
+    thread_queue_config: QueueConfig = QueueConfig()
+    writer_factory: WriterFactory = field(default_factory=WhyLabsWriterFactory)
+    queue_type: QueueType = QueueType.FASTER_FIFO
+
+
+class LoggerFactory:
+    @abstractmethod
+    def create_logger(self, dataset_id: str, options: LoggerOptions) -> ThreadRollingLogger:
+        raise NotImplementedError()
+
+
+class ThreadLoggerFactory(LoggerFactory):
+    def create_logger(self, dataset_id: str, options: LoggerOptions) -> ThreadRollingLogger:
+        logger = ThreadRollingLogger(
+            aggregate_by=options.aggregate_by,
+            writers=options.writer_factory.create_writers(dataset_id),
+            schema=options.schema,
+            write_schedule=options.write_schedule,
+            current_time_fn=options.current_time_fn,
+            queue_config=options.thread_queue_config,
+        )
+
+        return logger
+
+
+BuiltinMessageTypes = Union[
+    FlushMessage,
+    RawLogMessage,
+    RawLogEmbeddingsMessage,
+    RawPubSubMessage,
+    RawPubSubEmbeddingMessage,
+    LogMessage,
+    CloseMessage,
+    ProcessStatusMessage,
+    ProcessLoggerStatus,
+]
+
+AdditionalMessages = TypeVar("AdditionalMessages")
+
+
+class BaseProcessRollingLogger(
+    ProcessActor[Union[AdditionalMessages, BuiltinMessageTypes], ProcessLoggerStatus],
+    DataLogger[ProcessLoggerStatus],
+    Generic[AdditionalMessages],
+):
+    """
+    Log data asynchronously using a separate process.
+
+    The ProcessRollingLogger is a rolling logger that manages a separate process to do the actual logging. This means
+    it logs data over time and periodically uploads it in the background, using a separate process so that it doesn't
+    block the main one.
+
+    ```python
+    logger = ProcessRollingLogger(
+        aggregate_by=TimeGranularity.Day,
+        write_schedule=Schedule(cadence=TimeGranularity.Minute, interval=5),
+    )
+
+    logger.start()
+
+    logger.log(data_frame)
+    ```
+
+    This class mostly wraps and manages several ThreadRollingLoggers that do the real logging with whylogs.
+
+    MAC USERS: You'll run into issues running this on Python>=3.8 because Python will use spawn instead of fork.
+    You should be able to get around it by setting the environment variable OBJC_DISABLE_INITIALIZE_FORK_SAFETY=YES
+    in the environment that the process logger runs in, but you can't set it in Python (no using os.environ).
+
+    Most of the arguments that are passed to the underlying loggers are considered the default options for those
+    loggers. If you supply a logger_factory then you can override the options for each dataset id's logger.
+
+    Args:
+        aggregate_by: The time granularity to aggregate data by. This determines how the time bucketing is done. For
+            the Hour type, the logger will end up pooling data into profiles by the hour.
+        write_schedule: The schedule to use for writing data. This is used to determine when to upload data.
+        schema: The DatasetSchema to use for whylogs under the hood.
+        sync_enabled: Whether to enable synchronous logging. If this is enabled then you can pass log(sync=True) to the
+            log call. Without this you can't use the sync flag.
+        queue_config: Let's you change various polling and timeout parameters.
+        thread_queue_config: Same as queue_config, but for the wrapped ThreadRollingLoggers.
+        writer_factory: The writer factory to use for creating writers.
+        queue_type: The type of queue to to manage multiprocessing. By default, faster_fifo is used because it's
+            a lot faster than the default multiprocessing queue, but you can use the built in mp.Queue by setting
+            this to QueueType.MP.
+    """
+
     def __init__(
         self,
-        aggregate_by: TimeGranularity = TimeGranularity.Hour,
-        write_schedule: Optional[Schedule] = Schedule(cadence=TimeGranularity.Minute, interval=10),
+        aggregate_by: TimeGranularity = TimeGranularity.Day,
+        write_schedule: Optional[Schedule] = Schedule(cadence=TimeGranularity.Minute, interval=5),
         schema: Optional[DatasetSchema] = None,
         sync_enabled: bool = False,
         current_time_fn: Optional[Callable[[], int]] = None,
         queue_config: QueueConfig = QueueConfig(),
         thread_queue_config: QueueConfig = QueueConfig(),
         writer_factory: WriterFactory = WhyLabsWriterFactory(),
         queue_type: QueueType = QueueType.FASTER_FIFO,
+        logger_factory: LoggerFactory = ThreadLoggerFactory(),
     ) -> None:
-        super().__init__(queue_config=queue_config, queue_type=queue_type)
-        self._sync_enabled = sync_enabled
+        super().__init__(queue_config=queue_config, queue_type=queue_type, sync_enabled=sync_enabled)
+        self._logger_options = LoggerOptions(
+            aggregate_by=aggregate_by,
+            write_schedule=write_schedule,
+            schema=schema,
+            sync_enabled=sync_enabled,
+            current_time_fn=current_time_fn,
+            queue_config=queue_config,
+            thread_queue_config=thread_queue_config,
+            writer_factory=writer_factory,
+        )
+        self._logger_factory = logger_factory
         self._thread_queue_config = thread_queue_config
         self._writer_factory = writer_factory
         self.current_time_ms = current_time_fn or current_time_ms
         self.loggers: Dict[str, ThreadRollingLogger] = {}
-        self.write_schedule = write_schedule
         self.schema = schema
-        self.aggregate_by = aggregate_by
-        self._pipe_signaler: Optional[PipeSignaler] = PipeSignaler() if sync_enabled else None
-        self._session = get_current_session()
+        self._session = default_init()
 
     def _create_logger(self, dataset_id: str) -> ThreadRollingLogger:
-        logger = ThreadRollingLogger(
-            aggregate_by=self.aggregate_by,
-            writers=self._writer_factory.create_writers(dataset_id),
-            schema=self.schema,
-            write_schedule=self.write_schedule,
-            current_time_fn=self.current_time_ms,
-            queue_config=self._thread_queue_config,
-        )
-
-        self._logger.info(f"Created logger for {dataset_id}")
-        return logger
+        return self._logger_factory.create_logger(dataset_id, self._logger_options)
 
     def _get_logger(self, dataset_id: str) -> ThreadRollingLogger:
         if dataset_id not in self.loggers:
             self.loggers[dataset_id] = self._create_logger(dataset_id)
         return self.loggers[dataset_id]
 
-    def process_batch(self, batch: List[MessageType], batch_type: Type) -> None:
+    def process_batch(
+        self,
+        batch: List[Union[AdditionalMessages, BuiltinMessageTypes]],
+        batch_type: Type[Union[AdditionalMessages, BuiltinMessageTypes]],
+    ) -> None:
         if batch_type == FlushMessage:
             self.process_flush_message(cast(List[FlushMessage], batch))
         elif batch_type == LogMessage:
             self.process_log_messages(cast(List[LogMessage], batch))
         elif batch_type == RawLogMessage:
             self.process_raw_log_dicts(cast(List[RawLogMessage], batch))
         elif batch_type == RawLogEmbeddingsMessage:
             self.process_log_embeddings_messages(cast(List[RawLogEmbeddingsMessage], batch))
         elif batch_type == RawPubSubMessage:
             self.process_pubsub(cast(List[RawPubSubMessage], batch))
         elif batch_type == RawPubSubEmbeddingMessage:
             self.process_pubsub_embedding(cast(List[RawPubSubEmbeddingMessage], batch))
         elif batch_type == CloseMessage:
             self.process_close_message(cast(List[CloseMessage], batch))
-        elif batch_type == ProcessLoggerStatusMessage:
-            self._process_logger_status_message(cast(List[ProcessLoggerStatusMessage], batch))
+        elif batch_type == ProcessStatusMessage:
+            self._process_logger_status_message(cast(List[ProcessStatusMessage], batch))
         else:
             raise Exception(f"Unknown message type {batch_type}")
 
     def process_close_message(self, messages: List[CloseMessage]) -> None:
         self._logger.info("Running pre shutdown operations")
         self._logger.info(f"Closing down {len(self.loggers)} loggers")
         for datasetId, logger in self.loggers.items():
             self._logger.info(f"Closing whylogs logger for {datasetId}")
             logger.close()
 
-        if self._pipe_signaler is not None:
-            self._pipe_signaler.close_child()
-
     def process_pubsub(self, messages: List[RawPubSubMessage]) -> None:
         self._logger.info("Processing pubsub message")
         msgs = [msg["log_request"] for msg in [it.to_pubsub_message() for it in messages] if msg is not None]
         self.process_log_dicts(msgs)
 
-    def _process_logger_status_message(self, messages: List[ProcessLoggerStatusMessage]) -> None:
+    def _process_logger_status_message(self, messages: List[ProcessStatusMessage]) -> None:
         if self._pipe_signaler is None:
             raise Exception(
                 "Can't log synchronously without a pipe signaler. Initialize the process logger with sync_enabled=True."
             )
 
         futures: List[Tuple[str, "Future[LoggerStatus]"]] = []
 
         for dataset_id, logger in self.loggers.items():
             future: "Future[LoggerStatus]" = Future()
             logger.send(StatusMessage(result=future))
             futures.append((dataset_id, future))
 
-        statuses: List[ProcessLoggerStatus] = []
+        statuses: Dict[str, LoggerStatus] = {}
         for dataset_id, future in futures:
             try:
-                status = ProcessLoggerStatus(dataset_id=dataset_id, status=wait_result(future))
-                statuses.append(status)
+                statuses[dataset_id] = wait_result_while(future, self.is_alive)
             except Exception as e:
                 for message in messages:
                     self._pipe_signaler.signal((message.id, e, None))
 
         # Signal all of the status. In practice, there will really only be a single message in messages
         # but we do handle messages in batches so its technically possible to have multiple if the caller
         # is just spamming status requests for some reason.
-        status_dict = {status.dataset_id: status for status in statuses}
+        # status_dict = {status.dataset_id: status for status in statuses}
+        process_logger_status = ProcessLoggerStatus(statuses=statuses)
         for message in messages:
-            self._pipe_signaler.signal((message.id, None, status_dict))
-
-    def status(self, timeout: Optional[float] = 1.0) -> Dict[str, ProcessLoggerStatus]:
-        """
-        Get the internal status of the logger. Used for diangostics and debugging.
-        """
-        if self._pipe_signaler is None:
-            raise Exception(
-                "Can't log synchronously without a pipe signaler. Initialize the process logger with sync_enabled=True."
-            )
-
-        message = ProcessLoggerStatusMessage()
-        future: "Future[Dict[str, ProcessLoggerStatus]]" = Future()
-        self._pipe_signaler.register(future, message.id)
-        self.send(message)
-        return wait_result(future, timeout=timeout)
+            self._pipe_signaler.signal((message.id, None, process_logger_status))
 
     def process_pubsub_embedding(self, messages: List[RawPubSubEmbeddingMessage]) -> None:
         self._logger.info("Processing pubsub embedding message")
         pubsub = [
             msg["log_embedding_request"]
             for msg in [it.to_pubsub_embedding_message() for it in messages]
             if msg is not None
         ]
         self.process_log_embeddings_dicts(pubsub)
 
     def process_log_messages(self, messages: List[LogMessage]) -> None:
         try:
             self._logger.info("Processing log message")
-            log_dicts = [msg for msg in [m.log for m in messages] if msg is not None]
+            log_dicts = [m.log for m in messages]
             self.process_log_dicts(log_dicts)
 
-            for message in messages:
-                self._signal(message.id, None)
+            self._signal(messages, None)
         except Exception as e:
             self._logger.exception("Error processing log message")
-            for message in messages:
-                self._signal(message.id, e)
-
-    def _signal(self, message_id: str, error: Optional[Exception] = None) -> None:
-        if self._pipe_signaler is not None:
-            self._pipe_signaler.signal((message_id, error, None))
+            self._signal(messages, e)
 
     def process_raw_log_dicts(self, messages: List[RawLogMessage]) -> None:
         try:
             self._logger.info("Processing raw log request message")
             log_dicts = [msg for msg in [m.to_log_request_dict() for m in messages] if msg is not None]
             self.process_log_dicts(log_dicts)
-            for message in messages:
-                self._signal(message.id, None)
+            self._signal(messages, None)
         except Exception as e:
             self._logger.exception("Error processing log message")
-            for message in messages:
-                self._signal(message.id, e)
+            self._signal(messages, e)
 
     def process_log_embeddings_messages(self, messages: List[RawLogEmbeddingsMessage]) -> None:
         self._logger.info("Processing log embeddings messages")
         log_dicts = [msg for msg in [m.to_log_embeddings_request_dict() for m in messages] if msg is not None]
         self.process_log_embeddings_dicts(log_dicts)
 
     def process_log_embeddings_dicts(self, messages: List[LogEmbeddingRequestDict]) -> None:
@@ -282,28 +344,31 @@
     def process_log_dicts(self, messages: List[LogRequestDict]) -> None:
         self._process_dicts(messages, reduce_log_requests, log_dict_to_data_frame)
 
     def _process_dicts(
         self,
         dicts: List[DictType],
         reducer: Callable[[DictType, DictType], DictType],
-        pre_processor: Callable[[DictType], Tuple[Loggable, int]],
+        pre_processor: Callable[[DictType], Tuple[TrackData, int]],
     ) -> None:
         for dataset_id, group in groupby(dicts, lambda it: it["datasetId"]):
             for dataset_timestamp, ts_grouped in groupby(
-                group, lambda it: determine_dataset_timestamp(self.aggregate_by, it)
+                group,
+                lambda it: determine_dataset_timestamp(self._logger_options.aggregate_by, it),
             ):
                 for n, sub_group in groupby(ts_grouped, lambda it: encode_strings(get_columns(it))):
                     self._logger.info(
                         f"Logging data for ts {dataset_timestamp} in dataset {dataset_id} for column set {n}"
                     )
                     giga_message = reduce(reducer, sub_group)
                     loggable, row_count = pre_processor(giga_message)
                     start = time.perf_counter()
                     logger = self._get_logger(dataset_id)
+                    # TODO this error looks real. I think the thread logger can't handle numpy arrays currently
+                    # TODO unify the Loggable and TrackData types?
                     logger.log(loggable, timestamp_ms=dataset_timestamp, sync=True)
                     self._logger.debug(f"Took {time.perf_counter() - start}s to log {row_count} rows")
 
     def process_flush_message(self, messages: Optional[List[FlushMessage]] = None) -> None:
         if not self.loggers:
             self._logger.debug("No profiles to publish")
             return
@@ -333,155 +398,66 @@
         timestamp_ms: Optional[int] = None,  # The timestamp that the data happened at
         sync: bool = False,
         dataset_id: Optional[str] = None,
     ) -> None:
         if self.pid is None:
             raise Exception("Logger hasn't been started yet. Call start() first.")
 
+        if not self.is_alive():
+            raise Exception("Logger process is no longer alive. It may have been killed.")
+
         if dataset_id is None:
             dataset_id = self._session.config.get_default_dataset_id()
             if dataset_id is None:
                 raise Exception(
-                    f"Need to specify a dataset_id when calling log, or set it through why.init(). See {_INIT_DOCS}"
+                    f"Need to specify a dataset_id when calling log, or set it through why.init(). See {INIT_DOCS}"
                 )
 
         log_request = LogRequestDict(
             datasetId=dataset_id,
             timestamp=timestamp_ms,
             multiple=self._create_multiple(data),
         )
 
-        message = RawLogMessage(request=orjson.dumps(log_request), request_time=self.current_time_ms())
-        result: Optional["Future[None]"] = Future() if sync else None
+        message = RawLogMessage(
+            request=orjson.dumps(log_request),
+            request_time=self.current_time_ms(),
+            sync=sync,
+        )
+
+        result: Optional["Future[ProcessLoggerStatus]"] = (
+            cast("Future[ProcessLoggerStatus]", Future()) if sync else None
+        )
         if result is not None:
             self._logger.debug(f"Registering result id {message.id} for synchronous logging")
             if self._pipe_signaler is None:
                 raise Exception(
                     "Can't log synchronously without a pipe signaler. Initialize the process logger with sync_enabled=True."
                 )
             self._pipe_signaler.register(result, message.id)
 
         self.send(message)
 
         if result is not None:
             self._logger.debug(f"Waiting on id {message.id}")
-            it = wait_result(result)
-            self._logger.debug(f"Result id {message.id} done {it}")
+            try:
+                it = wait_result_while(result, self.is_alive)
+                self._logger.debug(f"Result id {message.id} done {it}")
+            except TimeoutError as e:
+                raise Exception("Logger killed while waiting for result") from e
 
     def flush(self) -> None:
         """
         Flush the internal state, causing everything to be written using the configured writers.
         """
         self.send(FlushMessage())
 
     def run(self) -> None:
         self._logger.debug(f"Started process logger with pid {os.getpid()}")
         super().run()
 
-    def start(self) -> None:
-        self._logger.debug(f"Starting process logger from pid {os.getpid()}")
-        # This is started in the parent process, not in the child process. It must be started
-        # before the process itself start right below.
-        if self._pipe_signaler is not None:
-            self._pipe_signaler.start()
-        super().start()
-
     def close(self) -> None:
         super().close()
-        if self._pipe_signaler is not None:
-            self._pipe_signaler.close()
-
 
-class PipeSignaler(th.Thread):
-    """
-    A thread that listens on a pipe for messages and signals the corresponding futures.
-
-    This class is used in the process logger to enable synchronous logging requests across processes.
-    It's essentially a dictionary of futures that are registered by the main process and signaled by the
-    child process. A lot of the behavior is implicit because it involves properties of processes, so it's
-    worth documenting here.
-
-    - This thread has to be started from the main process, which means it has to be started right before the
-        process logger is started (before the os.fork under the hood). It has to be started from the main process
-        because the main process will be registering futures on it, and those can't cross the process boundary.
-    - The parent and child process each have references to the pipes and they each need to close their references,
-        which means close_child has to be called from the child process and close has to be called from the parent.
-        Calling close_child in the main processing code will have right effect.
-    - The process actor does message batching so multiple ids mmay be signaled even though a single batch was processed
-        because that batch could have contained multiple messages.
-    - The signaler uses Events under the hood to know when to stop working. They can be th.Events even though this
-        is being used in a multiprocessing environment because nothing the child does can affect them. Keep in mind
-        that introducing any behavior on the child side that depends on knowing whether those events are set won't work
-        though, they would have to be switched to mp.Events for that.
-
-    This class should really never be used by anyone in most cases. It will just slow down the main process by making
-    it wait for logging to complete, but it enables a lot of testing and debugging.
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.daemon = True
-        self._logger = logging.getLogger(__name__)
-        self._parent_conn, self._conn = mp.Pipe()
-        self.futures: Dict[str, Future] = {}
-        self._end_polling = th.Event()
-        self._done = th.Event()
-
-    def signal(self, result: Tuple[str, Optional[Exception], Any]) -> None:
-        """
-        Signal that a message was handled by sending a tuple of (message id, exception, data).
-        data and exception can be None.
-        This should be called from the child process.
-        """
-        self._parent_conn.send(result)
-
-    def register(self, future: Future, message_id: str) -> None:
-        """
-        Register a future to be signaled when the message id is received.
-        This should be called from the parent process.
-        """
-        self._logger.debug(f"Received register request for id {message_id}")
-        self.futures[message_id] = future
-
-    def _start_poll_conn(self) -> None:
-        while not self._end_polling.is_set():
-            try:
-                if self._conn.poll(timeout=0.1):
-                    message_id, exception, data = self._conn.recv()
-                    self._logger.debug(f"Received message id {message_id}")
-                    future: Optional[Future] = self.futures.pop(message_id)
-                    if future is not None:
-                        self._logger.debug(f"Setting result for message id {message_id} {exception}")
-                        if exception is None:
-                            future.set_result(data)
-                        else:
-                            future.set_exception(exception)
-
-            except EOFError:
-                self._logger.exception("Broken pipe")
-                break
-            except Exception:
-                self._logger.exception("Error in ipc pipe")
-
-        self._done.set()
-
-    def run(self) -> None:
-        self._start_poll_conn()
-
-    def close_child(self) -> None:
-        """
-        Closes the file descriptors from the child process side.
-        """
-        self._conn.close()
-        self._parent_conn.close()
-
-    def close(self) -> None:
-        """
-        Closes the thread and all resources. This should be
-        called from the parent side.
-        """
-        self._conn.close()
-        self._parent_conn.close()
 
-        self._end_polling.set()
-        self._done.wait()
-        self.join()
+class ProcessRollingLogger(BaseProcessRollingLogger[NoReturn]):
+    pass
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 important to not raise exceptions in those data classes because the actor does a lot of large batch processing
 and exceptions would result in losing the entire batch. Instead, they return None and log errors if there is
 some issue deserializing or validating.
 """
 import sys
 
 if sys.version_info >= (3, 8):
-    from typing import TypedDict  # pylint: disable=no-name-in-module
+    from typing import Protocol, TypedDict  # pylint: disable=no-name-in-module
 else:
-    from typing_extensions import TypedDict
+    from typing_extensions import TypedDict, Protocol
 
 import base64
 from dataclasses import dataclass, field
-from typing import Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 from whylogs.api.logger.experimental.logger.actor.thread_rolling_logger import (
     LoggerStatus,
 )
 
 try:
-    import orjson
+    import orjson  # type: ignore
 except ImportError:
     raise ImportError("Install whylogs with extra [proc] for process based logging: pip install whylogs[proc]")
 import logging
 import uuid
 
 import numpy as np
 import pandas as pd
@@ -91,67 +91,81 @@
 
 class FlushMessage:
     pass
 
 
 @dataclass
 class ProcessLoggerStatus:
-    dataset_id: str
-    status: LoggerStatus
+    statuses: Dict[str, LoggerStatus] = field(default_factory=dict)
 
 
 @dataclass
-class ProcessLoggerStatusMessage:
+class ProcessStatusMessage:
     id: str = field(default_factory=lambda: str(uuid.uuid4()))
+    timeout: float = 1.0
+    sync: bool = True
 
 
 @dataclass
 class LogMessage:
     request_time: int
     log: LogRequestDict
     id: str = field(default_factory=lambda: str(uuid.uuid4()))
+    sync: bool = False
+
+
+class SyncMessage(Protocol):
+    """
+    A message can be sent synchronously if it has an id and it has a sync flag set to True.
+    It doesnt magically make the message synchronous, but allows us to create a synchronous
+    convenience method for that message type. See log and status on the ProcessRollingLogger.
+    """
+
+    id: str
+    sync: bool
 
 
 @dataclass
 class RawLogMessage:
     request: bytes
     """
     Bytes that represent json stringified LogRequestDict
     """
     request_time: int
     id: str = field(default_factory=lambda: str(uuid.uuid4()))
+    sync: bool = False
 
     def __post_init__(self) -> None:
         if self.id == "None":
             self.id = str(uuid.uuid4())
 
     def to_log_request_dict(self) -> Optional[LogRequestDict]:
         d: LogRequestDict = orjson.loads(self.request)
         if "timestamp" not in d or d["timestamp"] is None:
             d["timestamp"] = self.request_time
 
-        if "datasetId" not in d or d["datasetId"] is None:
+        if "datasetId" not in d or d["datasetId"] is None:  # type: ignore
             _logger.error(f"Request missing dataset id {d}")
             return None
 
-        if "multiple" not in d or d["multiple"] is None:
+        if "multiple" not in d or d["multiple"] is None:  # type: ignore
             _logger.error(f"Request has no 'multiple' field {d}")
             return None
 
         return d
 
 
 def get_columns(request: Union[LogRequestDict, LogEmbeddingRequestDict]) -> List[str]:
     maybe_request = cast(LogRequestDict, request)
-    if "multiple" in maybe_request and maybe_request["multiple"] is not None:
+    if "multiple" in maybe_request and maybe_request["multiple"] is not None:  # type: ignore
         return maybe_request["multiple"]["columns"]
 
     maybe_embedding = cast(LogEmbeddingRequestDict, request)
     embeddings = maybe_embedding["embeddings"]
-    if embeddings is not None:
+    if embeddings is not None:  # type: ignore
         return list(embeddings.keys())
 
     raise Exception(f"Don't know how to get column names for request {request}.")
 
 
 @dataclass
 class RawPubSubMessage:
@@ -177,15 +191,15 @@
 class PubSubEmbeddingDict(TypedDict):
     subscription: str
     message: PubSubMessage
     log_embedding_request: LogEmbeddingRequestDict
 
 
 def _decode_pubsub_data(data: Union[PubSubEmbeddingDict, PubSubDict]) -> Optional[bytes]:
-    if "message" not in data or data["message"] is None:
+    if "message" not in data or data["message"] is None:  # type: ignore
         _logger.error(f"Request missing message field {data}")
         return None
 
     message = data["message"]
     encoded_data = message["data"]
     return base64.b64decode(encoded_data)
 
@@ -216,42 +230,42 @@
     request_time: int
 
     def to_log_embeddings_request_dict(self) -> Optional[LogEmbeddingRequestDict]:
         d: LogEmbeddingRequestDict = orjson.loads(self.request)
         if "timestamp" not in d or d["timestamp"] is None:
             d["timestamp"] = self.request_time
 
-        if "datasetId" not in d or d["datasetId"] is None:
+        if "datasetId" not in d or d["datasetId"] is None:  # type: ignore
             _logger.error(f"Request missing dataset id {d}")
             return None
 
-        if "embeddings" not in d or d["embeddings"] is None:
+        if "embeddings" not in d or d["embeddings"] is None:  # type: ignore
             _logger.error(f"Request has no embeddings field {d}")
             return None
 
-        if not isinstance(d["embeddings"], dict):
+        if not isinstance(d["embeddings"], dict):  # type: ignore
             # TODO test recovering from errors like this. It seems to brick the container
             _logger.error(
                 f'Expected a dictionary format for embeddings of the form {{"column_name": "embedding_2d_list"}}. Got {self.request}'
             )
             return None
 
         return d
 
 
 def log_dict_to_data_frame(request: LogRequestDict) -> Tuple[pd.DataFrame, int]:
     df = pd.DataFrame(request["multiple"]["data"], columns=request["multiple"]["columns"])
     return df, len(df)
 
 
-def log_dict_to_embedding_matrix(request: LogEmbeddingRequestDict) -> Tuple[Dict[str, np.ndarray], int]:
-    row: Dict[str, np.ndarray] = {}
+def log_dict_to_embedding_matrix(request: LogEmbeddingRequestDict) -> Tuple[Dict[str, "np.ndarray[Any, Any]"], int]:
+    row: Dict[str, np.ndarray[Any, Any]] = {}
     row_count = 0
     for col, embeddings in request["embeddings"].items():
-        row[col] = np.array(embeddings)
+        row[col] = np.array(embeddings)  # type: ignore
         row_count += len(embeddings)
 
     return row, row_count
 
 
 def reduce_log_requests(acc: LogRequestDict, cur: LogRequestDict) -> LogRequestDict:
     """
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,20 +18,26 @@
     Schedule,
     TimeGranularity,
     current_time_ms,
     truncate_time_ms,
 )
 from whylogs.api.logger.result_set import ProfileResultSet, ResultSet
 from whylogs.api.logger.segment_cache import SegmentCache
-from whylogs.api.logger.segment_processing import segment_processing
+from whylogs.api.logger.segment_processing import segment_processing  # type: ignore
 from whylogs.api.store import ProfileStore
 from whylogs.api.writer import Writer
 from whylogs.api.writer.writer import Writable
 from whylogs.core import DatasetProfile, DatasetProfileView, DatasetSchema
-from whylogs.core.stubs import pd
+from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
+
+try:
+    import pandas as pd  # type: ignore
+except ImportError:
+    pd: Any = None  # type: ignore
+
 
 Row = Dict[str, Any]
 
 
 class DatasetProfileContainer:
     """
     A container that abstracts over different types of profiles.
@@ -43,20 +49,20 @@
 
     _target: Union[DatasetProfile, SegmentCache]
 
     def __init__(self, dataset_timestamp: int, schema: Optional[DatasetSchema]) -> None:
         self._schema: Optional[DatasetSchema] = schema
         self._active = True
         self._dataset_timestamp = datetime.fromtimestamp(dataset_timestamp / 1000.0, tz=tz.tzutc())
-        if self._has_segments() and schema is not None:  # Need the duplicate None check for type safety
+        if self.has_segments() and schema is not None:  # Need the duplicate None check for type safety
             self._target = SegmentCache(schema=schema)
         else:
             self._target = DatasetProfile(dataset_timestamp=self._dataset_timestamp, schema=schema)
 
-    def _has_segments(self) -> bool:
+    def has_segments(self) -> bool:
         return self._schema is not None and bool(self._schema.segments)
 
     def _track_segments(self, data: TrackData) -> None:
         if self._schema is None:
             raise Exception("Schema missing in logger while using segments")
 
         if not isinstance(self._target, SegmentCache):
@@ -70,55 +76,59 @@
 
     def _track_profile(self, data: TrackData) -> None:
         if not isinstance(self._target, DatasetProfile):
             raise Exception("Dataset profile missing in logger")
 
         if isinstance(data, List):
             for row in data:
-                self._target.track(row=row)
+                self._target.track(row=row)  # type: ignore
         else:
-            self._target.track(data)
+            self._target.track(data)  # type: ignore
 
     def track(self, data: TrackData) -> None:
         """
         Track data against the contained profile or segment.
         """
         if not self._active:
             # Should never happen
             raise Exception("Profile container no longer active.")
 
-        if self._has_segments():
+        if self.has_segments():
             self._track_segments(data)
         else:
             self._track_profile(data)
 
     def to_result_set(self) -> ResultSet:
         """
         Get the ResultSet of the contained profile/segment.
 
         This doesn't have any side effects. It generates a ResultSet of whatever
         is inside when this is called.
         """
         try:
             if isinstance(self._target, SegmentCache):
                 return self._target.flush(dataset_timestamp=self._dataset_timestamp)
-            elif isinstance(self._target, DatasetProfile):
+            else:
                 return ProfileResultSet(self._target)
         finally:
             self._active = False
 
     def to_views(self) -> List[DatasetProfileView]:
         if isinstance(self._target, SegmentCache):
             result_set = self._target.get_result_set(dataset_timestamp=self._dataset_timestamp)
             segments = result_set.segments() or []
             return [it for it in [result_set.view(segment) for segment in segments] if it is not None]
-        elif isinstance(self._target, DatasetProfile):
+        else:
             return [self._target.view()]
 
-        raise Exception("Unknown profile type")
+    def to_serialized_views(self) -> List[bytes]:
+        views: List[bytes] = []
+        for view in self.to_views():
+            views.append(view.serialize())
+        return views
 
 
 @dataclass
 class TrackMessage:
     """
     Send some data to be tracked.
 
@@ -165,14 +175,16 @@
     """
 
     dataset_timestamps: int
     dataset_profiles: int
     segment_caches: int
     writers: int
     pending_writables: int
+    pending_views: List[bytes]
+    views: List[bytes]
 
 
 @dataclass
 class StatusMessage:
     """
     Get various status metrics.
     """
@@ -182,14 +194,25 @@
 
 @dataclass
 class PendingWritable:
     attempts: int
     writable: Writable
 
 
+def _extract_profile_view_bytes(pending: PendingWritable) -> Optional[bytes]:
+    if isinstance(pending.writable, DatasetProfile):
+        return pending.writable.view().serialize()
+    elif isinstance(pending.writable, DatasetProfileView):
+        return pending.writable.serialize()
+    elif isinstance(pending.writable, SegmentedDatasetProfileView):
+        return pending.writable.profile_view.serialize()
+    else:
+        return None
+
+
 LoggerMessage = Union[TrackMessage, FlushMessage, StatusMessage, GetResultsMessage, CloseMessage]
 
 
 class ThreadRollingLogger(ThreadActor[LoggerMessage], DataLogger[LoggerStatus]):
     """
     A logger that manages profiles and segments for various dataset timestamps.
 
@@ -240,15 +263,15 @@
         else:
             self._logger.warning(
                 "No write schedule defined for logger. Profiles will only be written after calls to flush()."
             )
 
         self._logger.debug(f"Created thread logger, pid {os.getpid()}")
 
-    def process_batch(self, batch: List[LoggerMessage], batch_type: Type) -> None:
+    def process_batch(self, batch: List[LoggerMessage], batch_type: Type[LoggerMessage]) -> None:
         if batch_type == TrackMessage:
             self._process_track_messages(cast(List[TrackMessage], batch))
         elif batch_type == FlushMessage:
             self._process_flush_messages(cast(List[FlushMessage], batch))
         elif batch_type == CloseMessage:
             self._process_close_messages(cast(List[CloseMessage], batch))
         elif batch_type == StatusMessage:
@@ -274,32 +297,42 @@
     def _process_status_messages(self, messages: List[StatusMessage]) -> None:
         for message in messages:
             self._process_status_message(message)
 
     def _process_status_message(self, message: StatusMessage) -> None:
         profiles = 0
         segment_caches = 0
-        for ts, container in self._cache.items():
-            if container._has_segments():
+        views: List[bytes] = []
+        for container in self._cache.values():
+            if container.has_segments():
                 segment_caches += 1
             else:
                 profiles += 1
 
+            views.extend(container.to_serialized_views())
+
         writers = 0
         writables = 0
-        for writer, stuff in self._writers.items():
+        pending_views: List[bytes] = []
+        for stuff in self._writers.values():
             writers += 1
             writables += len(stuff)
+            for pending in stuff:
+                view = _extract_profile_view_bytes(pending)
+                if view is not None:
+                    pending_views.append(view)
 
         status = LoggerStatus(
             dataset_timestamps=len(self._cache),
             dataset_profiles=profiles,
             segment_caches=segment_caches,
             writers=writers,
             pending_writables=writables,
+            pending_views=pending_views,
+            views=views,
         )
         message.result.set_result(status)
 
     def _process_close_messages(self, messages: List[CloseMessage]) -> None:
         for message in messages:
             self._process_close_message(message)
 
@@ -307,15 +340,15 @@
         # Force wait for all writers to handle their pending items
         self._process_flush_message(FlushMessage())
         while self._has_pending():
             self._process_flush_message(FlushMessage())
 
     def _has_pending(self) -> bool:
         has_pending = False
-        for writer, pending in self._writers.items():
+        for pending in self._writers.values():
             has_pending = len(pending) > 0
         return has_pending
 
     def _process_track_messages(self, messages: List[TrackMessage]) -> None:
         for message in messages:
             self._process_track_message(message)
 
@@ -382,14 +415,18 @@
             if message.result is not None:
                 message.result.set_result(None)
         except Exception as e:
             if message.result is not None:
                 message.result.set_exception(e)
 
     def status(self, timeout: Optional[float] = None) -> LoggerStatus:
+        """
+        Get the status of the logger.
+        This is always synchronous.
+        """
         result: "Future[LoggerStatus]" = Future()
         self.send(StatusMessage(result))
         return wait_result(result, timeout=timeout)
 
     def _validate_data(self, data: TrackData) -> None:
         if not isinstance(data, pd.DataFrame) and not isinstance(data, list) and not isinstance(data, dict):
             raise Exception(f"Unsupported data type {type(data)}")
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/time_util.py` & `whylogs-1.4.0rc0/whylogs/api/logger/experimental/logger/actor/time_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import time
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from enum import Enum
 from threading import Timer
-from typing import Callable, Type
+from typing import Any, Callable, Type
 
 from dateutil import tz
 
 
 def current_time_ms() -> int:
     return time.time_ns() // 1_000_000
 
@@ -51,15 +51,15 @@
     """
     A timer that executes a function repeatedly given a Schedule. It will execute at the bottom of
     that time period. For example, a schedule of Schedule(TimeGranularity.Hour, 1) will execute at
     the start of each hour. If you start the timer 5 minutes before the next hour then it will first
     execute in five minutes, and then each hour after that.
     """
 
-    def __init__(self, schedule: Schedule, fn: Callable, timer_class: Type = Timer) -> None:
+    def __init__(self, schedule: Schedule, fn: Callable[[], Any], timer_class: Type[Any] = Timer) -> None:
         self._logger = logging.getLogger(f"{type(self).__name__}_{id(self)}")
         self._fn = fn
         self._schedule = schedule
         self._running = True
         self._timer_class = timer_class
         now = datetime.now(tz=tz.tzutc())
 
@@ -80,14 +80,18 @@
             self.repeat_interval = schedule.interval * 60 * 60 * 24
             next_day = (now + timedelta(days=self._schedule.interval)).replace(
                 microsecond=0, second=0, minute=0, hour=0
             )
             initial_interval = (next_day - now).seconds
         elif schedule.cadence == TimeGranularity.Month:
             raise Exception("Can't use Monthly schedule.")
+        elif schedule.cadence == TimeGranularity.Year:
+            raise Exception("Can't use Yearly schedule.")
+        else:
+            raise Exception(f"Unsupported cadence {schedule.cadence}")
 
         self._logger.debug(f"scheduled for {initial_interval} seconds from now")
         self._timer = timer_class(initial_interval, self._run)
         self._timer.start()
 
     def _run(self) -> None:
         self._logger.debug(f"scheduled for {self.repeat_interval} seconds from now")
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/logger.py` & `whylogs-1.4.0rc0/whylogs/api/logger/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import atexit
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional
 
-from whylogs.api.logger.result_set import ProfileResultSet, ResultSet
+from whylogs.api.logger.result_set import (
+    ProfileResultSet,
+    ResultSet,
+    SegmentedResultSet,
+)
 from whylogs.api.logger.segment_processing import segment_processing
 from whylogs.api.store import ProfileStore
 from whylogs.api.writer import Writer, Writers
 from whylogs.core import DatasetProfile, DatasetSchema
 from whylogs.core.errors import LoggingError
 from whylogs.core.input_resolver import _pandas_or_dict
-from whylogs.core.metadata import _populate_common_profile_metadata
+from whylogs.core.metadata import (
+    _populate_common_profile_metadata,
+    _safe_merge_metadata,
+)
 from whylogs.core.stubs import pd
 
 logger = logging.getLogger(__name__)
 
 
 class BasicCache(object):
     _cache: Dict[DatasetSchema, DatasetProfile] = {}
@@ -99,30 +106,33 @@
         if active_schema:
             pandas, row = _pandas_or_dict(obj, pandas, row)
             obj = None
             pandas, row = active_schema._run_udfs(pandas, row)
 
         # If segments are defined use segment_processing to return a SegmentedResultSet
         if active_schema and active_schema.segments:
-            segmented_results = segment_processing(
+            segmented_results: SegmentedResultSet = segment_processing(
                 schema=active_schema,
                 obj=obj,
                 pandas=pandas,
                 row=row,
                 segment_cache=self._segment_cache,
             )
             # Update the existing segmented_results metadata with the trace_id and other keys if not present
             _populate_common_profile_metadata(segmented_results.metadata, trace_id=trace_id, tags=tags)
+            _safe_merge_metadata(default_metadata=segmented_results.metadata, incoming_metadata=active_schema.metadata)
             return segmented_results
 
         profiles = self._get_matching_profiles(obj, pandas=pandas, row=row, schema=active_schema)
 
         for prof in profiles:
             prof.track(obj, pandas=pandas, row=row, execute_udfs=False)
             prof._metadata = _populate_common_profile_metadata(prof._metadata, trace_id=trace_id, tags=tags)
+            if active_schema:
+                _safe_merge_metadata(prof._metadata, active_schema.metadata)
 
         first_profile = profiles[0]
         if name is not None:
             if first_profile._metadata is None:
                 first_profile._metadata = dict()
             first_profile._metadata["name"] = name
         return ProfileResultSet(first_profile)
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/result_set.py` & `whylogs-1.4.0rc0/whylogs/api/logger/result_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from logging import getLogger
 from typing import Any, Dict, List, Optional, Tuple, Union
 
+from whylabs_client.model.segment_tag import SegmentTag
+
 from whylogs.api.reader import Reader, Readers
-from whylogs.api.writer import Writer, Writers
 from whylogs.api.writer.writer import Writable
 from whylogs.core import DatasetProfile, DatasetProfileView, Segment
 from whylogs.core.metrics.metrics import Metric
 from whylogs.core.model_performance_metrics import ModelPerformanceMetrics
 from whylogs.core.segmentation_partition import SegmentationPartition
 from whylogs.core.utils import ensure_timezone
 from whylogs.core.view.dataset_profile_view import _MODEL_PERFORMANCE
 from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
+from whylogs.migration.converters import _generate_segment_tags_metadata
 
 logger = getLogger(__name__)
 
 
 def _merge_metrics(
     lhs_metrics: Optional[Dict[str, Any]], rhs_metrics: Optional[Dict[str, Any]]
 ) -> Optional[Dict[str, Any]]:
@@ -108,89 +110,78 @@
 
 def _merge_partitions(
     lhs_partitions: List[SegmentationPartition], rhs_partitions: List[SegmentationPartition]
 ) -> List[SegmentationPartition]:
     return list(set(lhs_partitions).union(set(rhs_partitions)))
 
 
-class ResultSetWriter:
-    """
-    Result of a logging call.
-    A result set might contain one or multiple profiles or profile views.
-    """
-
-    def __init__(self, results: "ResultSet", writer: Writer):
-        self._result_set = results
-        self._writer = writer
-
-    def option(self, **kwargs: Any) -> "ResultSetWriter":
-        self._writer.option(**kwargs)
-        return self
-
-    def write(self, **kwargs: Any) -> List:
-        # multi-profile writer
-        files = self._result_set.get_writables()
-        statuses: List[Tuple[bool, str]] = list()
-        if not files:
-            logger.warning("Attempt to write a result set with no writables returned, nothing written!")
-            return statuses
-        if hasattr(self._writer, "_reference_profile_name"):
-            if self._writer._reference_profile_name is not None and isinstance(self._result_set, SegmentedResultSet):
-                # a segmented reference profile name needs to have access to the complete result set
-                response = self._writer.write(file=self._result_set, **kwargs)
-                statuses.append(response)
-                return statuses
-        logger.debug(f"About to write {len(files)} files:")
-        # TODO: special handling of large number of files, handle throttling
-        for view in files:
-            response = self._writer.write(file=view, **kwargs)
-            statuses.append(response)
-        logger.debug(f"Completed writing {len(files)} files!")
-
-        return statuses
-
-
 class ResultSetReader:
     def __init__(self, reader: Reader) -> None:
         self._reader = reader
 
     def option(self, **kwargs: Any) -> "ResultSetReader":
         self._reader.option(**kwargs)
         return self
 
     def read(self, **kwargs: Any) -> "ResultSet":
         return self._reader.read(**kwargs)
 
 
-class ResultSet(ABC):
+def _flatten_tags(tags: Union[List, Dict]) -> List[SegmentTag]:
+    if type(tags[0]) == list:
+        result: List[SegmentTag] = []
+        for t in tags:
+            result.append(_flatten_tags(t))
+        return result
+
+    return [SegmentTag(t["key"], t["value"]) for t in tags]
+
+
+class ResultSet(Writable, ABC):
     """
     A holder object for profiling results.
 
     A whylogs.log call can result in more than one profile. This wrapper class
     simplifies the navigation among these profiles.
 
     Note that currently we only hold one profile but we're planning to add other
     kinds of profiles such as segmented profiles here.
     """
 
+    def _get_default_filename(self) -> str:
+        view = self.view()
+        if view is None:
+            raise ValueError("No ResultSet view available")
+        return view._get_default_filename()
+
+    def get_default_path(self) -> Optional[str]:
+        view = self.view()
+        if view is None:
+            raise ValueError("No ResultSet view available")
+        return view.get_default_path()
+
+    def write(
+        self, path: Optional[str] = None, filename: Optional[str] = None, **kwargs: Any
+    ) -> Tuple[bool, Union[str, List[str]]]:
+        view = self.view()
+        if view is None:
+            raise ValueError("No ResultSet view available")
+        return view.write(path, filename, **kwargs)
+
     @staticmethod
     def read(multi_profile_file: str) -> "ResultSet":
         # TODO: parse multiple profile
         view = DatasetProfileView.read(multi_profile_file)
         return ViewResultSet(view=view)
 
     @staticmethod
     def reader(name: str = "local") -> "ResultSetReader":
         reader = Readers.get(name)
         return ResultSetReader(reader=reader)
 
-    def writer(self, name: str = "local") -> "ResultSetWriter":
-        writer = Writers.get(name)
-        return ResultSetWriter(results=self, writer=writer)
-
     @abstractmethod
     def view(self) -> Optional[DatasetProfileView]:
         pass
 
     @abstractmethod
     def profile(self) -> Optional[DatasetProfile]:
         pass
@@ -277,15 +268,15 @@
 
     def set_dataset_timestamp(self, dataset_timestamp: datetime) -> None:
         ensure_timezone(dataset_timestamp)
         view = self.view()
         if view is None:
             raise ValueError("Cannot set timestamp on a view result set without a view!")
         else:
-            view.set_dataset_timestamp(dataset_timestamp)
+            view.dataset_timestamp = dataset_timestamp
 
 
 class ProfileResultSet(ResultSet):
     def __init__(self, profile: DatasetProfile) -> None:
         self._profile = profile
 
     def profile(self) -> Optional[DatasetProfile]:
@@ -348,14 +339,122 @@
                     for key in single_dictionary:
                         return single_dictionary[key]
 
         raise ValueError(
             f"A profile was requested from a segmented result set without specifying which segment to return: {self._segments}"
         )
 
+    def get_writables(self) -> Optional[List[Writable]]:
+        results: Optional[List[Writable]] = None
+        if self._segments:
+            results = []
+            logger.info(f"Building list of: {self.count} SegmentedDatasetProfileViews in SegmentedResultSet.")
+            # TODO: handle more than one partition
+            if not self.partitions:
+                raise ValueError(
+                    f"Building list of: {self.count} SegmentedDatasetProfileViews in SegmentedResultSet but no partitions found: {self.partitions}."
+                )
+            if len(self.partitions) > 1:
+                logger.error(
+                    f"Building list of: {self.count} SegmentedDatasetProfileViews in SegmentedResultSet but found more than one partition: "
+                    f"{self.partitions}. Using first partition only!!"
+                )
+            first_partition = self.partitions[0]
+            segments = self.segments_in_partition(first_partition)
+            if segments:
+                for segment_key in segments:
+                    profile = segments[segment_key]
+                    metric = self.get_model_performance_metrics_for_segment(segment_key)
+                    if metric:
+                        profile.add_model_performance_metrics(metric)
+                        logger.debug(
+                            f"Found model performance metrics: {metric}, adding to segmented profile: {segment_key}."
+                        )
+                    view = profile.view() if isinstance(profile, DatasetProfile) else profile
+                    segmented_profile = SegmentedDatasetProfileView(
+                        profile_view=view, segment=segment_key, partition=first_partition
+                    )
+                    if self.metadata:
+                        segmented_profile.metadata.update(self.metadata)
+                    results.append(segmented_profile)
+            else:
+                logger.warning(
+                    f"Found no segments in partition: {first_partition} even though we have: {self.count} segments overall"
+                )
+            logger.info(f"From list of: {self.count} SegmentedDatasetProfileViews using {len(results)}")
+        else:
+            logger.warning(
+                f"Attempt to build segmented results for writing but there are no segments in this result set: {self._segments}. returning None."
+            )
+        return results
+
+    def get_whylabs_tags(self) -> List[SegmentTag]:
+        views = self.get_writables()
+        if views is None:
+            logger.warning("SegmentedResultSet contains no segments")
+            return []
+
+        if self._partitions is None:
+            logger.warning("SegmentedResultSet contains no partitions.")
+            return []
+
+        partitions: List[Any] = self.partitions  # type: ignore
+        if len(partitions) > 1:
+            logger.warning(
+                "SegmentedResultSet contains more than one partition. Only the first partition will be uploaded. "
+            )
+        partition = partitions[0]
+        whylabs_tags = list()
+        for view in views:
+            view_tags = list()
+            if view.partition.id != partition.id:
+                continue
+            _, segment_tags, _ = _generate_segment_tags_metadata(view.segment, view.partition)
+            for segment_tag in segment_tags:
+                tag_key = segment_tag.key.replace("whylogs.tag.", "")
+                tag_value = segment_tag.value
+                view_tags.append({"key": tag_key, "value": tag_value})
+            whylabs_tags.append(view_tags)
+
+        return _flatten_tags(whylabs_tags)
+
+    def get_timestamps(self) -> List[Optional[datetime]]:
+        views = self.get_writables()
+        if views is None:
+            logger.warning("SegmentedResultSet contains no segments")
+            return []
+
+        times = list()
+        for view in views:
+            times.append(view.dataset_timestamp)
+        return times
+
+    def _get_default_filename(self) -> str:
+        return ""  # unused, the segment Wriables are called
+
+    def write(
+        self, path: Optional[str] = None, filename: Optional[str] = None, **kwargs: Any
+    ) -> Tuple[bool, Union[str, List[str]]]:
+        all_success = True
+        files = []
+        writables = self.get_writables()  # TODO: support mulit-segment files
+        if writables is None:
+            raise ValueError("No results to write")
+        if len(writables) > 1 and filename is not None:
+            raise ValueError("Cannot specify filename for multiple files")
+
+        for writable in writables:
+            success, written_files = writable.write(path, filename, **kwargs)
+            all_success = all_success and success
+            if isinstance(written_files, list):
+                files += written_files
+            else:
+                files.append(written_files)
+        return all_success, files
+
     @property
     def dataset_properties(self) -> Optional[Dict[str, Any]]:
         return self._dataset_properties
 
     @property
     def dataset_metrics(self) -> Optional[Dict[str, Any]]:
         return self._metrics
@@ -427,58 +526,14 @@
                     logger.error(
                         f"Unexpected type: {type(profile)} -> {profile}, cannot check for model performance metrics."
                     )
                     return None
             return view.model_performance_metrics
         return None
 
-    def get_writables(self) -> Optional[List[Writable]]:
-        results: Optional[List[Writable]] = None
-        if self._segments:
-            results = []
-            logger.info(f"Building list of: {self.count} SegmentedDatasetProfileViews in SegmentedResultSet.")
-            # TODO: handle more than one partition
-            if not self.partitions:
-                raise ValueError(
-                    f"Building list of: {self.count} SegmentedDatasetProfileViews in SegmentedResultSet but no partitions found: {self.partitions}."
-                )
-            if len(self.partitions) > 1:
-                logger.error(
-                    f"Building list of: {self.count} SegmentedDatasetProfileViews in SegmentedResultSet but found more than one partition: "
-                    f"{self.partitions}. Using first partition only!!"
-                )
-            first_partition = self.partitions[0]
-            segments = self.segments_in_partition(first_partition)
-            if segments:
-                for segment_key in segments:
-                    profile = segments[segment_key]
-                    metric = self.get_model_performance_metrics_for_segment(segment_key)
-                    if metric:
-                        profile.add_model_performance_metrics(metric)
-                        logger.debug(
-                            f"Found model performance metrics: {metric}, adding to segmented profile: {segment_key}."
-                        )
-                    view = profile.view() if isinstance(profile, DatasetProfile) else profile
-                    segmented_profile = SegmentedDatasetProfileView(
-                        profile_view=view, segment=segment_key, partition=first_partition
-                    )
-                    if self.metadata:
-                        segmented_profile.metadata.update(self.metadata)
-                    results.append(segmented_profile)
-            else:
-                logger.warning(
-                    f"Found no segments in partition: {first_partition} even though we have: {self.count} segments overall"
-                )
-            logger.info(f"From list of: {self.count} SegmentedDatasetProfileViews using {len(results)}")
-        else:
-            logger.warning(
-                f"Attempt to build segmented results for writing but there are no segments in this result set: {self._segments}. returning None."
-            )
-        return results
-
     def add_metrics_for_segment(self, metrics: ModelPerformanceMetrics, segment: Segment) -> None:
         if segment.parent_id in self._segments:
             profile = self._segments[segment.parent_id][segment]
             profile.add_model_performance_metrics(metrics)
 
     @staticmethod
     def zero() -> "SegmentedResultSet":
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/rolling.py` & `whylogs-1.4.0rc0/whylogs/api/logger/rolling.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/segment_cache.py` & `whylogs-1.4.0rc0/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/segment_processing.py` & `whylogs-1.4.0rc0/whylogs/api/logger/segment_processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import math
+from functools import reduce
 from typing import Any, Dict, Iterable, Iterator, List, Mapping, Optional, Tuple
 
 from whylogs.api.logger.result_set import SegmentedResultSet
 from whylogs.api.logger.segment_cache import SegmentCache
 from whylogs.core import DatasetSchema
 from whylogs.core.dataset_profile import DatasetProfile
 from whylogs.core.input_resolver import _pandas_or_dict
@@ -40,28 +42,45 @@
         segment_tuple_key = tuple(str(k) for k in group_key)
     else:
         segment_tuple_key = (str(group_key),)
 
     return Segment(segment_tuple_key, partition_id)
 
 
+def _is_nan(x):
+    try:
+        return math.isnan(x)
+    except TypeError:
+        return False
+
+
 def _process_simple_partition(
     partition_id: str,
     schema: DatasetSchema,
     segments: Dict[Segment, Any],
     columns: List[str],
     pandas: Optional[pd.DataFrame] = None,
     row: Optional[Mapping[str, Any]] = None,
     segment_cache: Optional[SegmentCache] = None,
 ):
     if pandas is not None:
         # simple means we can segment on column values
         grouped_data = pandas.groupby(columns)
         for group in grouped_data.groups.keys():
-            pandas_segment = grouped_data.get_group(group)
+            if isinstance(group, tuple) and any([_is_nan(x) for x in group]):
+                evaluations = []
+                for val, col in zip(group, columns):
+                    if _is_nan(val):
+                        evaluations.append((pandas[col].isna()))
+                    else:
+                        evaluations.append((pandas[col] == val))
+                mask = reduce(lambda x, y: x & y, evaluations)
+                pandas_segment = pandas[mask]
+            else:
+                pandas_segment = grouped_data.get_group(group)
             segment_key = _get_segment_from_group_key(group, partition_id)
             _process_segment(pandas_segment, segment_key, segments, schema, segment_cache)
     elif row:
         # TODO: consider if we need to combine with the column names
         segment_key = Segment(tuple(str(row[element]) for element in columns), partition_id)
         _process_segment(row, segment_key, segments, schema, segment_cache)
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/logger/transient.py` & `whylogs-1.4.0rc0/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,16 @@
         return conf.column_batch_size
     else:
         return None
 
 
 def collect_dataset_profile_view(
     input_df: SparkDataFrame,
-    dataset_timestamp: Optional[int] = None,
-    creation_timestamp: Optional[int] = None,
+    dataset_timestamp: Optional[datetime] = None,
+    creation_timestamp: Optional[datetime] = None,
     schema: Optional[DatasetSchema] = None,
 ) -> DatasetProfileView:
     now = datetime.now(timezone.utc)
 
     _dataset_timestamp = dataset_timestamp or now
     _creation_timestamp = creation_timestamp or now
     if schema and schema.segments:
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.4.0rc0/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,16 +126,16 @@
     logger.warning(f"Skipping segment: could not find partition with id {partition_id} in: {schema.segments}")
     return None
 
 
 def collect_segmented_results(
     input_df: SparkDataFrame,
     schema: DatasetSchema,
-    dataset_timestamp: Optional[int] = None,
-    creation_timestamp: Optional[int] = None,
+    dataset_timestamp: Optional[datetime] = None,
+    creation_timestamp: Optional[datetime] = None,
 ) -> ResultSet:
     now = datetime.now(timezone.utc)
 
     _dataset_timestamp = dataset_timestamp or now
     _creation_timestamp = creation_timestamp or now
     if not schema.segments:
         raise ValueError("Cannot collect segmented results without segments defined in the passed in DatasetSchema")
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/reader/local.py` & `whylogs-1.4.0rc0/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/reader/reader.py` & `whylogs-1.4.0rc0/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/reader/s3.py` & `whylogs-1.4.0rc0/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/store/local_store.py` & `whylogs-1.4.0rc0/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/store/profile_store.py` & `whylogs-1.4.0rc0/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/store/query.py` & `whylogs-1.4.0rc0/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/store/sqlite_store.py` & `whylogs-1.4.0rc0/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/usage_stats/__init__.py` & `whylogs-1.4.0rc0/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/config.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     SessionType,
     parse_api_key,
     parse_api_key_v2,
 )
 
 _DEFAULT_WHYLABS_HOST = "https://api.whylabsapp.com"
 _CONFIG_APP_NAME = "whylogs"
-_INIT_DOCS = "https://docs.whylabs.ai/docs/whylabs-whylogs-init"
+INIT_DOCS = "https://docs.whylabs.ai/docs/whylabs-whylogs-init"
 
 
 class InitException(Exception):
     pass
 
 
 class EnvVariableName(Enum):
@@ -72,14 +72,15 @@
     force_local: Optional[bool] = None
 
 
 class SessionConfig:
     def __init__(self, init_config: Optional[InitConfig] = None) -> None:
         self._init_config = init_config or InitConfig()
         self.logger = logging.getLogger("config")
+        self._ensure_config_exists = False if self._init_config.force_local is True else True
         self.auth_path = (
             Path(self._init_config.config_path) if self._init_config.config_path else self.get_config_file_path()
         )
         self._init_parser()
 
         self.tmp_api_key: Optional[str] = self._init_config.whylabs_api_key
         self.tmp_default_dataset_id: Optional[str] = self._init_config.default_dataset_id
@@ -110,15 +111,19 @@
         env_variable = os.getenv(env_name.value)
         if env_variable is not None:
             return env_variable
 
         return ConfigFile.get_variable_from_config_file(self._config_parser, config_name)
 
     def _load_or_prompt(
-        self, env_name: EnvVariableName, config_name: ConfigVariableName, persist: bool = False, password: bool = True
+        self,
+        env_name: EnvVariableName,
+        config_name: ConfigVariableName,
+        persist: bool = False,
+        password: bool = True,
     ) -> Optional[str]:
         """
         Loads a configuration value like _load_value does, but it will also prompt the user for the value if
         there isn't one in either of those places, assuming we're in a notebook environment. If persist is True,
         the prompt value will also be persisted to the configuration file.
         """
         value = self._load_value(env_name=env_name, config_name=config_name)
@@ -190,37 +195,40 @@
 
     def set_whylabs_refernce_profile_name(self, name: str) -> None:
         self._set_value(ConfigVariableName.WHYLABS_REFERENCE_PROFILE_NAME, name)
 
     def get_whylabs_endpoint(self) -> str:
         return (
             self._load_value(
-                env_name=EnvVariableName.WHYLABS_API_ENDPOINT, config_name=ConfigVariableName.WHYLABS_API_ENDPOINT
+                env_name=EnvVariableName.WHYLABS_API_ENDPOINT,
+                config_name=ConfigVariableName.WHYLABS_API_ENDPOINT,
             )
             or _DEFAULT_WHYLABS_HOST
         )
 
     def set_whylabs_endpoint(self, endpoint: str) -> None:
         self._set_value(ConfigVariableName.WHYLABS_API_ENDPOINT, endpoint)
 
     def get_config_file_path(self) -> Path:
         config_dir_path = os.getenv(EnvVariableName.WHYLOGS_CONFIG_PATH.value)
         if config_dir_path is not None:
             Path(config_dir_path).mkdir(parents=True, exist_ok=True)
         else:
-            config_dir_path = user_config_dir(_CONFIG_APP_NAME, ensure_exists=True)
+            config_dir_path = user_config_dir(_CONFIG_APP_NAME, ensure_exists=self._ensure_config_exists)
 
         config_file_path = os.path.join(config_dir_path, "config.ini")
         path = Path(config_file_path)
-        path.touch(exist_ok=True)
+        if self._ensure_config_exists:
+            path.touch(exist_ok=True)
         return path
 
     def get_default_dataset_id(self) -> Optional[str]:
         return self.tmp_default_dataset_id or self._load_value(
-            env_name=EnvVariableName.WHYLABS_DEFAULT_DATASET_ID, config_name=ConfigVariableName.DEFAULT_DATASET_ID
+            env_name=EnvVariableName.WHYLABS_DEFAULT_DATASET_ID,
+            config_name=ConfigVariableName.DEFAULT_DATASET_ID,
         )
 
     def require_default_dataset_id(self) -> str:
         return self._require("default dataset id", self.get_default_dataset_id())
 
     def set_default_dataset_id(self, dataset_id: str) -> None:
         self._set_value(ConfigVariableName.DEFAULT_DATASET_ID, dataset_id)
@@ -230,40 +238,44 @@
         api_key = self.get_api_key()
         try:
             if api_key is not None:
                 return parse_api_key_v2(api_key).org_id
         except Exception:
             pass
 
-        org_id = self._load_value(env_name=EnvVariableName.WHYLABS_ORG_ID, config_name=ConfigVariableName.ORG_ID)
+        org_id = self._load_value(
+            env_name=EnvVariableName.WHYLABS_ORG_ID,
+            config_name=ConfigVariableName.ORG_ID,
+        )
 
         if org_id is not None:
             return org_id
 
         return org_id
 
     def require_org_id(self) -> str:
         return self._require("org id", self.get_org_id())
 
     def _require(self, name: str, value: Optional[str]) -> str:
         if value is None:
             session_type = self.get_session_type()
             raise ValueError(
                 f"Can't determine {name}. Current session type is {session_type.value}. "
-                f"See {_INIT_DOCS} for instructions on using why.init()."
+                f"See {INIT_DOCS} for instructions on using why.init()."
             )
 
         return value
 
     def set_org_id(self, org_id: str) -> None:
         self._set_value(ConfigVariableName.ORG_ID, org_id)
 
     def get_api_key(self) -> Optional[str]:
         return self.tmp_api_key or self._load_value(
-            env_name=EnvVariableName.WHYLABS_API_KEY, config_name=ConfigVariableName.API_KEY
+            env_name=EnvVariableName.WHYLABS_API_KEY,
+            config_name=ConfigVariableName.API_KEY,
         )
 
     def get_env_api_key(self) -> Optional[str]:
         return os.getenv(EnvVariableName.WHYLABS_API_KEY.value)
 
     def require_api_key(self) -> str:
         return self._require("api key", self.get_api_key())
@@ -274,15 +286,18 @@
     def get_user_guid(self) -> Optional[str]:
         return ConfigFile.get_variable_from_config_file(self._config_parser, ConfigVariableName.USER_GUID)
 
     def set_user_guid(self, user_guid: str) -> None:
         self._set_value(ConfigVariableName.USER_GUID, user_guid)
 
     def get_session_id(self) -> Optional[str]:
-        return self._load_value(env_name=EnvVariableName.WHYLABS_SESSION_ID, config_name=ConfigVariableName.SESSION_ID)
+        return self._load_value(
+            env_name=EnvVariableName.WHYLABS_SESSION_ID,
+            config_name=ConfigVariableName.SESSION_ID,
+        )
 
     def set_session_id(self, sessionId: str) -> None:
         self._set_value(ConfigVariableName.SESSION_ID, sessionId)
 
     def remove_session_id(self) -> None:
         self._remove_value(ConfigVariableName.SESSION_ID)
 
@@ -320,15 +335,18 @@
             f"In production, you should pass the api key as an environment variable {EnvVariableName.WHYLABS_API_KEY.value}, "
             f"the org id as {EnvVariableName.WHYLABS_ORG_ID.value}, and the default dataset id as "
             f"{EnvVariableName.WHYLABS_DEFAULT_DATASET_ID.value}."
         )
 
     def _notify_type_anon(self) -> None:
         anonymous_session_id = self.get_session_id()
-        il.success(f"Using session type: {SessionType.WHYLABS_ANONYMOUS.name}", ignore_suppress=True)
+        il.success(
+            f"Using session type: {SessionType.WHYLABS_ANONYMOUS.name}",
+            ignore_suppress=True,
+        )
         id_text = "<will be generated before upload>" if not anonymous_session_id else anonymous_session_id
         il.option(f"session id: {id_text}", ignore_suppress=True)
 
     def _notify_type_local(self) -> None:
         il.success(
             f"Using session type: {SessionType.LOCAL.name}. "
             "Profiles won't be uploaded or written anywhere automatically.",
@@ -381,15 +399,15 @@
 
         if init_config.allow_local:
             return SessionType.LOCAL
 
         raise InitException(
             "Don't know how to initialize authentication because allow_anonymous=False, allow_local=False, "
             "and there is no WhyLabs api key in the environment, config file, or why.init() call, and this isn't an "
-            f"interactive environment. See {_INIT_DOCS} for instructions on using why.init()."
+            f"interactive environment. See {INIT_DOCS} for instructions on using why.init()."
         )
 
 
 _CONFIG_WHYLABS_SECTION = "whylabs"
 
 
 class ConfigFile:
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/prompts.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/prompts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     LogAsyncRequest,
     LogReferenceRequest,
     LogSessionReferenceResponse,
     SessionsApi,
 )
 
 from whylogs.api.logger.result_set import ResultSet
-from whylogs.api.whylabs.session.config import _INIT_DOCS, SessionConfig
+from whylogs.api.whylabs.session.config import INIT_DOCS, SessionConfig
 from whylogs.api.whylabs.session.lazy import Lazy
 from whylogs.api.whylabs.session.session_types import InteractiveLogger as il
 from whylogs.api.whylabs.session.session_types import NotSupported, SessionType
 from whylogs.api.whylabs.session.whylabs_client_cache import WhylabsClientCache
 from whylogs.core.view.dataset_profile_view import DatasetProfileView
-from whylogs.migration.uncompound import _uncompound_dataset_profile
+from whylogs.migration.uncompound import _uncompound_dataset_profile  # type: ignore
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class UploadResult:
     result: Optional[Any]
@@ -62,15 +62,15 @@
         return self.config
 
     @abstractmethod
     def upload_reference_profiles(self, profile_aliases: Dict[str, ResultSet]) -> Union[UploadResult, NotSupported]:
         raise NotImplementedError()
 
     @abstractmethod
-    def upload_batch_profile(self, profile: ResultSet) -> Union[UploadResult, NotSupported]:
+    def upload_batch_profile(self, result_set: ResultSet) -> Union[UploadResult, NotSupported]:
         raise NotImplementedError()
 
 
 class GuestSession(Session):
     def __init__(self, config: SessionConfig) -> None:
         """
         Get a guest session that uses the id that is in the env, or the config if there is no env.
@@ -109,15 +109,15 @@
             return None
 
         if not self._validate_session_id(session_id):
             self.config.remove_session_id()
             il.warning(
                 f"Session {session_id} is no longer valid, generating a new one. If you want to upload to your WhyLabs "
                 "account then authenticate with an api token using `python -m whylogs.api.whylabs.session.why_init`."
-                f"See {_INIT_DOCS}"
+                f"See {INIT_DOCS}"
             )
             return None
         else:
             return session_id
 
     def _get_or_create_session_id(self) -> str:
         session_id = self._validate_config_session()
@@ -138,32 +138,32 @@
         return user_guid
 
     def _validate_session_id(self, session_id: str) -> bool:
         """
         Check to see if the session id is valid by calling WhyLabs.
         """
         try:
-            request = BatchLogReferenceRequest(
+            request = BatchLogReferenceRequest(  # type: ignore
                 session_id=session_id, references=[LogReferenceRequest(alias="test", datasetTimestamp=0)]
             )
-            self._whylabs_session_api.value.batch_create_reference_profile_upload(
+            self._whylabs_session_api.value.batch_create_reference_profile_upload(  # type: ignore
                 batch_log_reference_request=request, session_id=session_id
             )
             return True
         except ApiException:
             return False
 
     def _create_session_id(self) -> str:
         try:
             user_guid = self._user_guid
-            response: CreateSessionResponse = self._whylabs_session_api.value.create_session(
+            response: CreateSessionResponse = self._whylabs_session_api.value.create_session(  # type: ignore
                 CreateSessionRequest(user_guid)
             )
-            logger.debug(f"Created session {response.id}")
-            return response.id
+            logger.debug(f"Created session {response.id}")  # type: ignore
+            return response.id  # type: ignore
         except ApiException as e:
             logger.error(e)
             raise e
 
     def upload_batch_profile(self, result_set: ResultSet) -> Union[UploadResult, NotSupported]:
         if len(result_set.get_writables() or []) > 1:
             il.warning(
@@ -171,16 +171,16 @@
             )
             return NotSupported()
 
         profile = result_set.view()
         if profile is None:
             raise Exception("Profile did not contain any data.")
         try:
-            if profile._dataset_timestamp is not None:
-                timestamp = int(profile._dataset_timestamp.timestamp() * 1000)
+            if profile._dataset_timestamp is not None:  # type: ignore
+                timestamp = int(profile._dataset_timestamp.timestamp() * 1000)  # type: ignore
             else:
                 timestamp = int(datetime.now(timezone.utc).timestamp() * 1000)
 
             request = LogAsyncRequest(datasetTimestamp=timestamp, dataset="model-1", segment_tags=[])
             session_id = self._get_or_create_session_id()
             response: CreateDatasetProfileUploadResponse = (
                 self._whylabs_session_api.value.create_dataset_profile_upload(session_id, request)
@@ -316,16 +316,22 @@
 
         request: GetProfileObservatoryLinkRequest = GetProfileObservatoryLinkRequest(
             batch_profile_timestamps=list(timestamps), reference_profile_ids=[]
         )
 
         org_id = self.config.require_org_id()
         dataset_id = self.config.require_default_dataset_id()
-        response: GetProfileObservatoryLinkResponse = self._whylabs_log_api.value.get_profile_observatory_link(
-            dataset_id, org_id, request
-        )
 
+        try:
+            response: GetProfileObservatoryLinkResponse = self._whylabs_log_api.value.get_profile_observatory_link(
+                dataset_id, org_id, request
+            )
+        except Exception as e:
+            logger.info(f"Convenience profile links could not be generated for the sucessfully uploading profiles: {e}")
+
+        profile_url = response.observatory_url if response else ""
+        individual_urls = response.individual_observatory_urls if response else None
         return UploadResult(
-            viewing_url=response.observatory_url,
+            viewing_url=profile_url,
             result=result,
-            individual_viewing_urls=response.individual_observatory_urls,
+            individual_viewing_urls=individual_urls,
         )
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 import logging
 from typing import Optional
 
-from whylogs.api.whylabs.session.config import InitConfig, SessionConfig
+from whylogs.api.whylabs.session.config import INIT_DOCS, InitConfig, SessionConfig
 from whylogs.api.whylabs.session.session import (
     ApiKeySession,
     GuestSession,
     LocalSession,
     Session,
 )
 from whylogs.api.whylabs.session.session_types import InteractiveLogger as il
 from whylogs.api.whylabs.session.session_types import SessionType
 
 logger = logging.getLogger(__name__)
 
 
 class SessionManager:
-    __instance: Optional["SessionManager"] = None
+    _instance: Optional["SessionManager"] = None
+    session: Session
 
     def __init__(
         self,
         config: SessionConfig,
     ):
-        self.session: Session
         session_type = config.get_session_type()
         if session_type == SessionType.LOCAL:
             self.session = LocalSession(config)
         elif session_type == SessionType.WHYLABS_ANONYMOUS:
             self.session = GuestSession(config)
         elif session_type == SessionType.WHYLABS:
             self.session = ApiKeySession(config)
         else:
             raise ValueError(f"Unknown session type: {session_type}")
 
     @staticmethod
     def init(session_config: SessionConfig) -> "SessionManager":
-        if SessionManager.__instance is None:
-            SessionManager.__instance = SessionManager(session_config)
+        if SessionManager._instance is None:
+            SessionManager._instance = SessionManager(session_config)
         else:
             logger.debug("SessionManager is already initialized. Ignoring call to init()")
 
-        return SessionManager.__instance
+        return SessionManager._instance
 
     @staticmethod
     def reset() -> None:
-        SessionManager.__instance = None
+        SessionManager._instance = None
 
     @staticmethod
     def get_instance() -> Optional["SessionManager"]:
-        return SessionManager.__instance
+        return SessionManager._instance
 
     @staticmethod
     def is_active() -> bool:
         return SessionManager.get_instance() is not None
 
 
-def init(  # type: ignore
+def init(
     reinit: bool = False,
     allow_anonymous: bool = True,
     allow_local: bool = False,
     whylabs_api_key: Optional[str] = None,
     default_dataset_id: Optional[str] = None,
     config_path: Optional[str] = None,
-    **kwargs,
+    **kwargs: bool,
 ) -> Session:
     """
     Set up authentication for this whylogs logging session. There are three modes that you can authentiate in.
 
     1. WHYLABS: Data is sent to WhyLabs and is associated with a specific WhyLabs account. You can get a WhyLabs api
         key from the WhyLabs Settings page after logging in.
     2. WHYLABS_ANONYMOUS: Data is sent to WhyLabs, but no authentication happens and no WhyLabs account is required.
@@ -97,15 +97,15 @@
             This is a convenience argument so that you don't have to supply the dataset id every time you upload a profile if
             you're only using a single dataset id.
 
     """
     if reinit:
         SessionManager.reset()
 
-    manager: SessionManager = SessionManager._SessionManager__instance  # type: ignore
+    manager: Optional[SessionManager] = SessionManager._instance  # type: ignore
     if manager is not None:
         return manager.session
 
     session_config = SessionConfig(
         InitConfig(
             allow_anonymous=allow_anonymous,
             allow_local=allow_local,
@@ -126,31 +126,28 @@
         logger.warning("Could not create or read configuration file for session. Profiles won't be uploaded.", e)
         raise e
     except Exception as e:
         logger.warning("Could not initialize session", e)
         raise e
 
 
-_INIT_DOCS = "https://docs.whylabs.ai/docs/whylabs-whylogs-init"
-
-
 def get_current_session() -> Optional[Session]:
     manager = SessionManager.get_instance()
     if manager is not None:
         return manager.session
 
     il.warning_once(
-        f"No session found. Call whylogs.init() to initialize a session and authenticate. See {_INIT_DOCS} for more information.",
+        f"No session found. Call whylogs.init() to initialize a session and authenticate. See {INIT_DOCS} for more information.",
         logger.warning,
     )
 
     return None
 
 
-def _default_init() -> Session:
+def default_init() -> Session:
     """
     For internal use. This initializes a default session for the user if they don't call why.init() themselves.
     This will behave as though they called why.init() with no arguments and print out a warning with a link to the docs.
     """
     manager = SessionManager.get_instance()
     if manager is None:
         il.warning_once("Initializing default session because no session was found.", logger.warning)
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/session_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 # This is used to indicate that a result is either a success or a failure
 class NotSupported:
     """
     Indicates that one of the session apis isn't supported for the current session type.
     """
 
 
+LogFunction = Callable[[str], None]
+
+
 class InteractiveLogger:
     """
     Logger for interactive environments.
     """
 
     __warnings: Set[int] = set()
     _is_notebook: bool = False
@@ -34,15 +37,15 @@
         """
         if ignore_suppress:
             return InteractiveLogger._is_notebook
         else:
             return not os.environ.get("WHYLOGS_SUPPRESS_LOG_OUTPUT") and InteractiveLogger._is_notebook
 
     @staticmethod
-    def message(message: str = "", log_fn: Optional[Callable] = None, ignore_suppress: bool = False) -> None:
+    def message(message: str = "", log_fn: Optional[LogFunction] = None, ignore_suppress: bool = False) -> None:
         """
         Log a message only if we're in a notebook environment.
 
         Args:
             message: The message to log
             log_fn: A function to log to instead of printing if we're not in a notebook.
             ignore_suppress: If true, will log even if WHYLOGS_SUPPRESS_LOG_OUTPUT is set. It still needs
@@ -86,22 +89,22 @@
     def failure(message: str, ignore_suppress: bool = False) -> None:
         """
         Log a failure, which has a red x.
         """
         InteractiveLogger.message(f"❌ {message}", ignore_suppress=ignore_suppress)
 
     @staticmethod
-    def warning(message: str, log_fn: Optional[Callable] = None, ignore_suppress: bool = False) -> None:
+    def warning(message: str, log_fn: Optional[LogFunction] = None, ignore_suppress: bool = False) -> None:
         """
         Log a warning, which has a warning sign.
         """
         InteractiveLogger.message(f"⚠️ {message}", log_fn=log_fn, ignore_suppress=ignore_suppress)
 
     @staticmethod
-    def warning_once(message: str, log_fn: Optional[Callable] = None, ignore_suppress: bool = False) -> None:
+    def warning_once(message: str, log_fn: Optional[LogFunction] = None, ignore_suppress: bool = False) -> None:
         """
         Like warning, but only logs once.
         """
         if not InteractiveLogger.__should_log(ignore_suppress=ignore_suppress):
             return
 
         if hash(message) not in InteractiveLogger.__warnings:
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/whylabs_client_cache.py` & `whylogs-1.4.0rc0/whylogs/api/whylabs/session/whylabs_client_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
     """
 
     @property
     def key_id(self) -> str:
         return self._key_id
 
     def __call__(self, config: Configuration) -> None:
-        from whylogs.api.whylabs.session.session_manager import _default_init
+        from whylogs.api.whylabs.session.session_manager import default_init
 
-        session = _default_init()
+        session = default_init()
         session_config = session.config
         api_key = session_config.get_env_api_key()
         self._key_id = self._validate_api_key(api_key)
         assert api_key is not None
         config.api_key = {"ApiKeyAuth": api_key}
 
 
@@ -88,15 +88,15 @@
     @staticmethod
     def reset() -> None:
         WhylabsClientCache.__instance = None
 
     @staticmethod
     def instance() -> "WhylabsClientCache":
         if WhylabsClientCache.__instance is None:
-            # Internally, we'll call _default_init() to initialize the instance wherever we need
+            # Internally, we'll call default_init() to initialize the instance wherever we need
             # a guarantee that one exists.
             raise ValueError("WhylabsClientCache is not initialized. Call why.init() to initialize it.")
         return WhylabsClientCache.__instance
 
     def __init__(self) -> None:
         self._api_client_cache: Dict[ClientCacheConfig, Tuple[ApiClient, KeyRefresher]] = dict()
         self._logger = logging.getLogger(__name__)
@@ -112,17 +112,17 @@
 
     def _create_client(self, cache_config: ClientCacheConfig) -> Tuple[ApiClient, KeyRefresher]:
         """
         Refresh the API client by comparing various configs. We try to
         re-use the client as much as we can since using a new client
         every time can be expensive.
         """
-        from whylogs.api.whylabs.session.session_manager import _default_init
+        from whylogs.api.whylabs.session.session_manager import default_init
 
-        session = _default_init()
+        session = default_init()
         session_config = session.config
         self._proxy = session_config.get_https_proxy() or session_config.get_http_proxy()
 
         config = Configuration()
         config.api_key = {"ApiKeyAuth": ""}
         refresher: KeyRefresher = (
             StaticKeyRefresher(cache_config.api_key)
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/writer/s3.py` & `whylogs-1.4.0rc0/whylogs/api/writer/gcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,103 @@
 import logging
-import tempfile
-from typing import Any, Optional, Tuple
+import os
+from typing import Any, List, Optional, Tuple, Union
 
-import boto3
-from botocore.client import BaseClient
-from botocore.exceptions import ClientError
+from google.cloud import exceptions, storage  # type: ignore
 
-from whylogs.api.usage_stats import emit_usage
 from whylogs.api.writer import Writer
 from whylogs.api.writer.writer import Writable
 from whylogs.core.utils import deprecated_alias
 
 logger = logging.getLogger(__name__)
 
 
-class S3Writer(Writer):
+class GCSWriter(Writer):
     """
-    A WhyLogs writer to upload DatasetProfileViews onto Amazon S3.
+    A whylogs writer to upload DatasetProfileViews onto Google Cloud Storage (GCS).
 
-    >**IMPORTANT**: In order to correctly connect to your Amazon S3 bucket, make sure you have
-    the following environment variables set: `[AWS_ACCESS_KEY_ID, AWS_SECRET_ACCESS_KEY]`
+    >**IMPORTANT**: In order to correctly connect to your GCS container, make sure you have
+    the following environment variables set: `[GOOGLE_APPLICATION_CREDENTIALS]`
 
     Parameters
     ----------
-    s3_client: BaseClient, optional
-        The s3 client used to authenticate and perform operations on the s3 bucket.
-        Should be a BaseClient from the boto3 library
-    base_prefix: str, optional
-        The base file prefix for s3, in order to organize. A placeholder 'profile' will take place if None is provided.
-    bucket_name: str, optional
-        The name of the bucket to connect to. Made optional so the user can also access it
-        via the `option` method
-    object_name: str, optional
-        The s3's object name. It basically states the location where the file goes to.
-        Also made optional, so it can be defined through the `option` method
+    bucket_name = "your-bucket-name"
+    source_file_name = "local/path/to/file"
+    destination_blob_name = "storage-object-name"
+
     Returns
     -------
         None
 
     Examples
     --------
     An example usage of this method can be represented with the simple code above. Here we
     are assuming the user has already assigned a pandas.DataFrame to the `df` variable.
 
     ```python
     import whylogs as why
 
     profile = why.log(pandas=df)
-    profile.writer("s3").option(bucket_name="my_bucket").write()
+    profile.writer("gcs").option(bucket_name="my_bucket").write()
     ```
-
     """
 
     def __init__(
         self,
-        s3_client: Optional[BaseClient] = None,
-        base_prefix: Optional[str] = None,
+        gcs_client: Optional[storage.Client] = None,
+        object_name: Optional[str] = None,  # TODO: drop this
         bucket_name: Optional[str] = None,
-        object_name: Optional[str] = None,
     ):
-        self.s3_client = s3_client or boto3.client("s3")
-        self.base_prefix = base_prefix or "profile"
-        self.bucket_name = bucket_name or ""
-        self.object_name = object_name or None
-        emit_usage("s3_writer")
+        self.gcs_client = gcs_client or storage.Client()
+        self.object_name = object_name
+        self.bucket_name = bucket_name
 
     @deprecated_alias(profile="file")
     def write(
         self,
         file: Writable,
-        dest: Optional[str] = None,
+        dest: Optional[str] = None,  # TODO: this should be used as object_name
         **kwargs: Any,
-    ) -> Tuple[bool, str]:
-        dest = dest or file.get_default_path()  # type: ignore
-        if self.object_name is None:
-            self.object_name = dest
-        try:
-            with tempfile.NamedTemporaryFile() as tmp_file:
-                file.write(path=tmp_file.name)  # type: ignore
-                tmp_file.flush()
-                self.s3_client.upload_file(tmp_file.name, self.bucket_name, self.object_name)
-        except ClientError as e:
-            logging.error(e)
-            return False, str(e)
-        return True, f"Uploaded {tmp_file.name} to {self.bucket_name}/{self.object_name}"
-
-    def option(
-        self,
-        bucket_name: Optional[str] = None,
-        object_name: Optional[str] = None,
-        s3_client: Optional[BaseClient] = None,
-    ) -> "S3Writer":  # type: ignore
+    ) -> Tuple[bool, Union[str, List[Tuple[bool, str]]]]:
+        success, files = file.write(**kwargs)
+        files = [files] if isinstance(files, str) else files
+        if not success:
+            return False, "Writable failed to create temporary file(s)"
+
+        # TODO: support ZipFile ?
+
+        if len(files) > 1 and ((dest or self.object_name) is not None):
+            raise ValueError("Cannot specify dest or object_name for multiple files")
+
+        bucket = self.gcs_client.bucket(self.bucket_name)
+        all_success = True
+        statuses = []
+        for file in files:
+            object_name = dest or self.object_name or file.split(os.sep)[-1]  # TODO: drop self.object_name
+            blob = bucket.blob(object_name)
+            try:
+                blob.upload_from_filename(file)
+                statuses.append((True, f"Uploaded {file} to {self.bucket_name}/{object_name}"))
+                os.remove(file)
+            except exceptions.Forbidden as e:
+                logging.error(e)
+                all_success = False
+                statuses.append((False, f"{str(e)} for uploading {file} to {self.bucket_name}/{object_name}"))
+
+        return all_success, statuses
+
+    def option(self, **kwargs: Any) -> Writer:
+        """
+        bucket_name: str   GCS bucket name to write to
+        object_name: str   GCS object name to create
+        gcs_client: ?      GCS client object
+        """
+        bucket_name = kwargs.get("bucket_name")
+        object_name = kwargs.get("object_name")  # TODO: drop this
+        gcs_client = kwargs.get("gcs_client")
         if bucket_name:
             self.bucket_name = bucket_name
         if object_name:
             self.object_name = object_name
-        if s3_client:
-            self.s3_client = s3_client
+        if gcs_client:
+            self.gcs_client = gcs_client
         return self
```

### Comparing `whylogs-1.3.9.dev0/whylogs/api/writer/whylabs.py` & `whylogs-1.4.0rc0/whylogs/api/writer/whylabs_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,126 +1,102 @@
-import datetime
 import logging
 import os
-import tempfile
+import pprint
 from typing import IO, Any, Dict, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import requests  # type: ignore
 from urllib3 import PoolManager, ProxyManager
 from whylabs_client import ApiClient, Configuration  # type: ignore
 from whylabs_client.api.dataset_profile_api import DatasetProfileApi  # type: ignore
 from whylabs_client.api.feature_weights_api import FeatureWeightsApi  # type: ignore
-from whylabs_client.api.log_api import AsyncLogResponse  # type: ignore
 from whylabs_client.api.log_api import (
     LogApi,
     LogAsyncRequest,
     LogReferenceRequest,
     LogReferenceResponse,
 )
 from whylabs_client.api.models_api import ModelsApi  # type: ignore
+from whylabs_client.api.transactions_api import TransactionsApi
+from whylabs_client.exceptions import NotFoundException
+from whylabs_client.model.async_log_response import AsyncLogResponse
 from whylabs_client.model.column_schema import ColumnSchema  # type: ignore
 from whylabs_client.model.create_reference_profile_request import (  # type: ignore
     CreateReferenceProfileRequest,
 )
+from whylabs_client.model.log_transaction_metadata import LogTransactionMetadata
 from whylabs_client.model.metric_schema import MetricSchema  # type: ignore
 from whylabs_client.model.segment import Segment  # type: ignore
 from whylabs_client.model.segment_tag import SegmentTag  # type: ignore
+from whylabs_client.model.transaction_commit_request import TransactionCommitRequest
+from whylabs_client.model.transaction_log_request import TransactionLogRequest
+from whylabs_client.model.transaction_start_request import TransactionStartRequest
 from whylabs_client.rest import ForbiddenException  # type: ignore
 
-from whylogs.api.logger import log
-from whylogs.api.logger.result_set import ResultSet, SegmentedResultSet
-from whylogs.api.whylabs.session.session_manager import _INIT_DOCS, _default_init
+from whylogs.api.whylabs.session.session_manager import INIT_DOCS, default_init
 from whylogs.api.whylabs.session.whylabs_client_cache import (
     ClientCacheConfig,
     EnvironmentKeyRefresher,
     KeyRefresher,
     WhylabsClientCache,
 )
-from whylogs.api.writer import Writer
-from whylogs.api.writer.writer import Writable
 from whylogs.context.environ import read_bool_env_var
 from whylogs.core import DatasetProfileView
-from whylogs.core.dataset_profile import DatasetProfile
-from whylogs.core.errors import BadConfigError
 from whylogs.core.feature_weights import FeatureWeights
-from whylogs.core.utils import deprecated_alias
 from whylogs.core.utils.utils import get_auth_headers
 from whylogs.core.view.segmented_dataset_profile_view import SegmentedDatasetProfileView
-from whylogs.experimental.performance_estimation.estimation_results import (
-    EstimationResult,
-)
-from whylogs.migration.converters import _generate_segment_tags_metadata
-from whylogs.migration.uncompound import (
-    FeatureFlags,
-    _uncompound_dataset_profile,
-    _uncompound_metric_feature_flag,
-    _uncompound_performance_estimation_feature_flag,
-    _uncompound_performance_estimation_magic_string,
-)
 
 FIVE_MINUTES_IN_SECONDS = 60 * 5
 DAY_IN_SECONDS = 60 * 60 * 24
 FIVE_YEARS_IN_SECONDS = DAY_IN_SECONDS * 365 * 5
 logger = logging.getLogger(__name__)
 WHYLOGS_PREFER_SYNC_KEY = "WHYLOGS_PREFER_SYNC"
 
 _API_CLIENT_CACHE: Dict[str, ApiClient] = dict()
 _UPLOAD_POOLER_CACHE: Dict[str, Union[PoolManager, ProxyManager]] = dict()
 
 _US_WEST2_DOMAIN = "songbird-20201223060057342600000001.s3.us-west-2.amazonaws.com"
 _S3_PUBLIC_DOMAIN = os.environ.get("_WHYLABS_PRIVATE_S3_DOMAIN") or _US_WEST2_DOMAIN
-_WHYLABS_SKIP_CONFIG_READ = os.environ.get("_WHYLABS_SKIP_CONFIG_READ") or False
 
 KNOWN_CUSTOM_PERFORMANCE_METRICS = {
     "mean_average_precision_k_": "mean",
     "accuracy_k_": "mean",
-    "mean_reciprocal_rank": "mean",
+    "reciprocal_rank": "mean",
     "precision_k_": "mean",
     "recall_k_": "mean",
     "top_rank": "mean",
     "average_precision_k_": "mean",
+    "norm_dis_cumul_gain_k_": "mean",
+    "sum_gain_k_": "mean",
 }
 
+KNOWN_CUSTOM_OUTPUT_METRICS = {
+    "mean_average_precision_k_": ("fractional", "continuous"),
+    "accuracy_k_": ("fractional", "continuous"),
+    "reciprocal_rank": ("fractional", "continuous"),
+    "precision_k_": ("fractional", "continuous"),
+    "recall_k_": ("fractional", "continuous"),
+    "top_rank": ("integral", "continuous"),
+    "average_precision_k_": ("fractional", "continuous"),
+    "norm_dis_cumul_gain_k_": ("fractional", "continuous"),
+    "sum_gain_k_": ("fractional", "continuous"),
+}
 
-def _check_whylabs_condition_count_uncompound() -> bool:
-    global _WHYLABS_SKIP_CONFIG_READ
-    if _WHYLABS_SKIP_CONFIG_READ:
-        return True
-    whylabs_config_url = (
-        "https://whylabs-public.s3.us-west-2.amazonaws.com/whylogs_config/whylabs_condition_count_disabled"
-    )
-    logger.info(f"checking: {whylabs_config_url}")
-    try:
-        response = requests.head(whylabs_config_url)
-        logger.info(f"checking: {whylabs_config_url}")
-        logger.info(f"headers are: {response.headers} code: {response.status_code}")
-        if response.status_code == 200:
-            logger.info(
-                "found the whylabs condition count disabled file so running uncompound on condition count metrics"
-            )
-            return True
-        elif response.status_code == 404:
-            logger.info("no whylabs condition count disabled so sending condition count metrics as v1.")
-            return False
-        else:
-            logger.info(f"Got response code {response.status_code} but expected 200, so running uncompound")
-    except Exception:
-        logger.warning("Error trying to read whylabs config, falling back to defaults for uncompounding")
-    _WHYLABS_SKIP_CONFIG_READ = True
-    return True
 
+class TransactionAbortedException(Exception):
+    pass
 
-class WhyLabsWriter(Writer):
+
+class WhyLabsClient:
     f"""
-    A WhyLogs writer to upload DatasetProfileView's onto the WhyLabs platform.
+    An interface for interacting with the WhyLabs platform.
 
-    >**IMPORTANT**: In order to correctly send your profiles over, make sure you have
+    >**IMPORTANT**: In order to correctly interact with WhyLabs, make sure you have
     the following environment variables set: `[WHYLABS_ORG_ID, WHYLABS_API_KEY, WHYLABS_DEFAULT_DATASET_ID]`. You
-    can also follow the authentication instructions for the why.init() method at {_INIT_DOCS}.
+    can also follow the authentication instructions for the why.init() method at {INIT_DOCS}.
     It is highly recommended you don't persist credentials in code!
 
     You shouldn't have to supply these parameters to the writer in practice. You should depend on why.init() to resolve
     the credentials for you. These are here for one-offs and testing convenience.
 
     Parameters
     ----------
@@ -137,24 +113,16 @@
         If not informed, will get the mentioned environment variable instead.
     Returns
     -------
         None
 
     Examples
     --------
-    An example usage of this method can be represented with the simple code above. Here we
-    are assuming the user has already assigned a pandas.DataFrame to the `df` variable.
 
     ```python
-    import whylogs as why
-
-    why.init()
-
-    profile = why.log(pandas=df)
-    profile.writer("whylabs").write()
     ```
 
     """
 
     _key_refresher: KeyRefresher
     _endpoint_hostname: Optional[str] = None
     _s3_private_domain: Optional[str] = None
@@ -166,24 +134,26 @@
         org_id: Optional[str] = None,
         api_key: Optional[str] = None,
         dataset_id: Optional[str] = None,
         api_client: Optional[ApiClient] = None,
         ssl_ca_cert: Optional[str] = None,
         _timeout_seconds: Optional[float] = None,
     ):
-        session = _default_init()  # Force an init if the user didn't do it, it's idempotent
+        session = default_init()  # Force an init if the user didn't do it, it's idempotent
         config = session.config
 
         self._org_id = org_id or config.get_org_id()
         self._dataset_id = dataset_id or config.get_default_dataset_id()
         self._api_key = api_key or config.get_api_key()
+        self._ssl_ca_cert = ssl_ca_cert
         self._feature_weights = None
         self._reference_profile_name = config.get_whylabs_refernce_profile_name()
         self._api_config: Optional[Configuration] = None
         self._prefer_sync = read_bool_env_var(WHYLOGS_PREFER_SYNC_KEY, False)
+        self._transaction_id: Optional[str] = None
 
         _http_proxy = os.environ.get("HTTP_PROXY")
         _https_proxy = os.environ.get("HTTPS_PROXY")
         self._proxy = _https_proxy or _http_proxy
 
         # Enable private access to WhyLabs endpoints
         _private_api_endpoint = config.get_whylabs_private_api_endpoint()
@@ -279,61 +249,64 @@
                 pool_kwargs = {}
             pool_kwargs["assert_hostname"] = endpoint_hostname_override
             pool_kwargs["server_hostname"] = endpoint_hostname_override
             return old_conn_factory(host, port, scheme, pool_kwargs)
 
         self._api_client.rest_client.pool_manager.connection_from_host = new_conn_factory
 
-    def check_interval(self, interval_seconds: int) -> None:
-        if interval_seconds < FIVE_MINUTES_IN_SECONDS:
-            raise BadConfigError("Bad WhyLabsWriter config: interval must be greater or equal to five minutes")
-
-    def option(  # type: ignore
-        self,
-        org_id: Optional[str] = None,
-        dataset_id: Optional[str] = None,
-        api_key: Optional[str] = None,
-        reference_profile_name: Optional[str] = None,
-        configuration: Optional[Configuration] = None,
-        ssl_ca_cert: Optional[str] = None,
-        api_client: Optional[ApiClient] = None,
-        timeout_seconds: Optional[float] = None,
-        prefer_sync: Optional[bool] = None,
-    ) -> "WhyLabsWriter":
+    def option(self, **kwargs) -> "WhyLabsClient":  # type: ignore
         """
 
         Parameters
         ----------
         org_id the organization ID
         dataset_id the dataset Id
         api_key the API key
-        reference_profile_name the name of the reference profile
         configuration the additional configuration for the REST client
 
-        Returns a "WhyLabsWriter" with these options configured
+        org_id: Optional[str] = None,
+        dataset_id: Optional[str] = None,
+        api_key: Optional[str] = None,
+        configuration: Optional[Configuration] = None,
+        ssl_ca_cert: Optional[str] = None,
+        api_client: Optional[ApiClient] = None,
+        timeout_seconds: Optional[float] = None,
+        transaction_id: Optional[str] = None,
+        prefer_sync:
+
+        Returns a "WhyLabsClient" with these options configured
         -------
 
         """
+        org_id = kwargs.get("org_id")
+        dataset_id = kwargs.get("dataset_id")
+        api_key = kwargs.get("api_key")
+        configuration = kwargs.get("configuration")
+        ssl_ca_cert = kwargs.get("ssl_ca_cert")
+        api_client = kwargs.get("api_client")
+        timeout_seconds = kwargs.get("timeout_seconds")
+        prefer_sync = kwargs.get("prefer_sync")
+        transaction_id = kwargs.get("transaction_id")
         if dataset_id is not None:
             self._dataset_id = dataset_id
         if org_id is not None:
             self._org_id = org_id
         if api_key is not None:
             self._api_key = api_key
-        if reference_profile_name is not None:
-            self._reference_profile_name = reference_profile_name
         if configuration is not None:
             raise ValueError("Manual configuration is not supported. Please override the api_client instead")
         if api_client is not None:
             self._custom_api_client = api_client
             self._api_client = None
         if timeout_seconds is not None:
             self._timeout_seconds = timeout_seconds
         if prefer_sync is not None:
             self._prefer_sync = prefer_sync
+        if transaction_id is not None:
+            self._transaction_id = transaction_id
 
         self._cache_config = ClientCacheConfig(
             api_key=self._api_key or self._cache_config.api_key,
             ssl_ca_cert=ssl_ca_cert or self._cache_config.ssl_ca_cert,
             whylabs_api_endpoint=self._cache_config.whylabs_api_endpoint,
             endpoint_hostname=self._cache_config.endpoint_hostname,
         )
@@ -435,39 +408,30 @@
         except Exception as e:
             logger.warning(
                 f"Failed to tag column {column} as custom performance metric for {self._org_id}/{self._dataset_id} to "
                 + f"{self.whylabs_api_endpoint}"
             )
             return False, str(e)
 
-    def write_estimation_result(self, file: EstimationResult, **kwargs: Any) -> Tuple[bool, str]:
-        if _uncompound_performance_estimation_feature_flag():
-            estimation_magic_string = _uncompound_performance_estimation_magic_string()
-            estimation_result_profile = log({f"{estimation_magic_string}accuracy": file.accuracy}).profile()
-            estimation_result_profile.set_dataset_timestamp(file.target_result_timestamp)
-            return self.write(estimation_result_profile.view())
-        return False, str("Performance estimation feature flag is not enabled")
-
     def write_feature_weights(self, file: FeatureWeights, **kwargs: Any) -> Tuple[bool, str]:
         """Put feature weights for the specified dataset.
 
         Parameters
         ----------
         file : FeatureWeights
             FeatureWeights object representing the Feature Weights for the specified dataset
 
         Returns
         -------
         Tuple[bool, str]
             Tuple with a boolean (1-success, 0-fail) and string with the request's status code.
         """
-        self._feature_weights = file.to_dict()
         if kwargs.get("dataset_id") is not None:
             self._dataset_id = kwargs.get("dataset_id")
-        return self._do_upload_feature_weights()
+        return self._do_upload_feature_weights(file)
 
     def get_feature_weights(self, **kwargs: Any) -> Optional[FeatureWeights]:
         """Get latest version for the feature weights for the specified dataset
 
         Returns
         -------
         FeatureWeightResponse
@@ -480,212 +444,76 @@
         feature_weights_set = result.get("segment_weights")
         metadata = result.get("metadata")
         if feature_weights_set and isinstance(feature_weights_set, list):
             feature_weights = FeatureWeights(weights=feature_weights_set[0]["weights"], metadata=metadata)
             return feature_weights
         return None
 
-    def _write_segmented_reference_result_set(self, file: SegmentedResultSet, **kwargs: Any) -> Tuple[bool, str]:
-        """Put segmented reference result set for the specified dataset.
-
-        Parameters
-        ----------
-        file : SegmentedResultSet
-            SegmentedResultSet object representing the segmented reference result set for the specified dataset
-
-        Returns
-        -------
-        Tuple[bool, str]
-        """
-        utc_now = datetime.datetime.now(datetime.timezone.utc)
-
-        files = file.get_writables()
-        partitions = file.partitions
-        if len(partitions) > 1:
-            logger.warning(
-                "SegmentedResultSet contains more than one partition. Only the first partition will be uploaded. "
+    def _set_column_schema(self, column_name: str, column_schema: ColumnSchema):
+        model_api_instance = self._get_or_create_models_client()
+        try:
+            # TODO: remove when whylabs supports merge writes.
+            model_api_instance.put_entity_schema_column(  # type: ignore
+                self._org_id, self._dataset_id, column_name, column_schema=column_schema
             )
-        partition = partitions[0]
-        whylabs_tags = list()
-        for view in files:
-            view_tags = list()
-            dataset_timestamp = view.dataset_timestamp or utc_now
-            if view.partition.id != partition.id:
-                continue
-            _, segment_tags, _ = _generate_segment_tags_metadata(view.segment, view.partition)
-            for segment_tag in segment_tags:
-                tag_key = segment_tag.key.replace("whylogs.tag.", "")
-                tag_value = segment_tag.value
-                view_tags.append({"key": tag_key, "value": tag_value})
-            whylabs_tags.append(view_tags)
-        stamp = dataset_timestamp.timestamp()
-        dataset_timestamp_epoch = int(stamp * 1000)
-        profile_id, upload_urls = self._get_upload_urls_segmented_reference(whylabs_tags, dataset_timestamp_epoch)
-        upload_statuses = list()
-        for view, url in zip(files, upload_urls):
-            with tempfile.NamedTemporaryFile() as tmp_file:
-                if kwargs.get("use_v0") is None or kwargs.get("use_v0"):
-                    view.write(file=tmp_file, use_v0=True)
-                else:
-                    view.write(file=tmp_file)
-                tmp_file.flush()
-                tmp_file.seek(0)
-
-                upload_res = self._do_upload(
-                    dataset_timestamp=dataset_timestamp_epoch,
-                    upload_url=url,
-                    profile_id=profile_id,
-                    profile_file=tmp_file,
-                )
-                upload_statuses.append(upload_res)
-        if all([status[0] for status in upload_statuses]):
-            return upload_statuses[0]
-        else:
-            return False, "Failed to upload all segments"
-
-    def _write_segmented_result_set(self, file: SegmentedResultSet, **kwargs: Any) -> Tuple[bool, str]:
-        """Put segmented result set for the specified dataset.
-
-        Parameters
-        ----------
-        file : SegmentedResultSet
-            SegmentedResultSet object representing the segmented result set for the specified dataset
-
-        Returns
-        -------
-        Tuple[bool, str]
-        """
-        # multi-profile writer
-        files = file.get_writables()
-        messages: List[str] = list()
-        and_status: bool = True
-        if not files:
-            logger.warning("Attempt to write a result set with no writables, nothing written!")
-            return True, ""
-
-        logger.debug(f"About to write {len(files)} files:")
-        # TODO: special handling of large number of files, handle throttling
-        for view in files:
-            bool_status, message = self.write(file=view, **kwargs)
-            and_status = and_status and bool_status
-            messages.append(message)
-        logger.debug(f"Completed writing {len(files)} files!")
+            return (
+                200,
+                f"{column_name} schema set to {column_schema.classifier} {column_schema.data_type} {column_schema.discreteness}",
+            )
+        except ForbiddenException as e:
+            logger.exception(
+                f"Failed to set column outputs {self._org_id}/{self._dataset_id} for column name: ("
+                f"{column_name}) "
+                f"{self.whylabs_api_endpoint}"
+                f" with API token ID: {self.key_id}"
+            )
+            raise e
 
-        return and_status, "; ".join(messages)
+    def _tag_custom_output_metrics(self, view: Union[DatasetProfileView, SegmentedDatasetProfileView]):
+        if isinstance(view, DatasetProfileView):
+            column_names = view.get_columns().keys()
+            for column_name in column_names:
+                for perf_col in KNOWN_CUSTOM_OUTPUT_METRICS:
+                    if column_name.startswith(perf_col):
+                        data_type = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][0]
+                        discreteness = KNOWN_CUSTOM_OUTPUT_METRICS[perf_col][1]
+                        column_schema: ColumnSchema = ColumnSchema(
+                            classifier="output", data_type=data_type, discreteness=discreteness  # type: ignore
+                        )
+                        self._set_column_schema(column_name, column_schema=column_schema)
 
     def _tag_custom_perf_metrics(self, view: Union[DatasetProfileView, SegmentedDatasetProfileView]):
         if isinstance(view, DatasetProfileView):
             column_names = view.get_columns().keys()
             for column_name in column_names:
                 for perf_col in KNOWN_CUSTOM_PERFORMANCE_METRICS:
                     if column_name.startswith(perf_col):
                         metric = KNOWN_CUSTOM_PERFORMANCE_METRICS[perf_col]
                         self.tag_custom_performance_column(column_name, default_metric=metric)
-        return
-
-    @deprecated_alias(profile="file")
-    def write(self, file: Writable, **kwargs: Any) -> Tuple[bool, str]:
-        if isinstance(file, FeatureWeights):
-            return self.write_feature_weights(file, **kwargs)
-        elif isinstance(file, EstimationResult):
-            return self.write_estimation_result(file, **kwargs)
-        elif isinstance(file, ResultSet):
-            if isinstance(file, SegmentedResultSet):
-                if self._reference_profile_name is not None:
-                    return self._write_segmented_reference_result_set(file, **kwargs)
-                else:
-                    return self._write_segmented_result_set(file, **kwargs)
-
-            file = file.profile()
-
-        view = file.view() if isinstance(file, DatasetProfile) else file
-
-        has_segments = isinstance(view, SegmentedDatasetProfileView)
-        has_performance_metrics = view.model_performance_metrics
-        self._tag_custom_perf_metrics(view)
-        if not has_segments and not isinstance(view, DatasetProfileView):
-            raise ValueError(
-                "You must pass either a DatasetProfile or a DatasetProfileView in order to use this writer!"
-            )
-
-        flags = FeatureFlags(_check_whylabs_condition_count_uncompound())
-
-        if _uncompound_metric_feature_flag():
-            if has_segments:
-                updated_profile_view = _uncompound_dataset_profile(view.profile_view, flags)
-                view = SegmentedDatasetProfileView(
-                    profile_view=updated_profile_view, segment=view._segment, partition=view._partition
-                )
-
-            else:
-                view = _uncompound_dataset_profile(view, flags)
-
-        if kwargs.get("dataset_id") is not None:
-            self._dataset_id = kwargs.get("dataset_id")
-
-        with tempfile.NamedTemporaryFile() as tmp_file:
-            # currently whylabs is not ingesting the v1 format of segmented profiles as segmented
-            # so we default to sending them as v0 profiles if the override `use_v0` is not defined,
-            # if `use_v0` is defined then pass that through to control the serialization format.
-            if has_performance_metrics or kwargs.get("use_v0"):
-                view.write(file=tmp_file, use_v0=True)
-            else:
-                view.write(file=tmp_file)
-            tmp_file.flush()
-            tmp_file.seek(0)
-            utc_now = datetime.datetime.now(datetime.timezone.utc)
-            dataset_timestamp = view.dataset_timestamp or utc_now
-            stamp = dataset_timestamp.timestamp()
-            time_delta_seconds = utc_now.timestamp() - stamp
-            if time_delta_seconds < 0:
-                logger.warning(
-                    f"About to upload a profile with a dataset_timestamp that is in the future: "
-                    f"{time_delta_seconds}s old."
-                )
-            if time_delta_seconds > FIVE_YEARS_IN_SECONDS:
-                logger.error(
-                    f"A profile being uploaded to WhyLabs has a dataset_timestamp of({dataset_timestamp}) "
-                    f"compared to current datetime: {utc_now}. Uploads of profiles older than 5 years "
-                    "might not be monitored in WhyLabs and may take up to 24 hours to show up."
-                )
-
-            if stamp <= 0:
-                logger.error(
-                    f"Profiles should have timestamps greater than 0, but found a timestamp of {stamp}"
-                    f" and current timestamp is {utc_now.timestamp()}, this is likely an error."
-                )
-
-            dataset_timestamp_epoch = int(stamp * 1000)
-            response = self._do_upload(
-                dataset_timestamp=dataset_timestamp_epoch,
-                profile_file=tmp_file,
-            )
-        # TODO: retry
-        return response
 
     def _do_get_feature_weights(self):
         """Get latest version for the feature weights for the specified dataset
 
         Returns
         -------
             Response of the GET request, with segmentWeights and metadata.
         """
         result = self._get_column_weights()
         return result
 
-    def _do_upload_feature_weights(self) -> Tuple[bool, str]:
+    def _do_upload_feature_weights(self, file: FeatureWeights) -> Tuple[bool, str]:
         """Put feature weights for the specified dataset.
 
         Returns
         -------
         Tuple[bool, str]
             Tuple with a boolean (1-success, 0-fail) and string with the request's status code.
         """
 
-        result = self._put_feature_weights()
+        result = self._put_feature_weights(file)
         if result == 200:
             return True, str(result)
         else:
             return False, str(result)
 
     def _put_file(self, profile_file: IO[bytes], upload_url: str, dataset_timestamp: int) -> Tuple[bool, str]:
         # TODO: probably want to call this API using asyncio
@@ -699,33 +527,30 @@
         is_successful = False
         if response.status == 200:
             is_successful = True
             logger.info(
                 f"Done uploading {self._org_id}/{self._dataset_id}/{dataset_timestamp} to "
                 f"{self.whylabs_api_endpoint} with API token ID: {self._key_refresher.key_id}"
             )
+        else:
+            logger.warning(
+                f"response from file upload was not 200, instead got: {pprint.pformat(vars(response), indent=4)}"
+            )
+
         return is_successful, response.reason
 
-    def _do_upload(
+    def do_upload(
         self,
         dataset_timestamp: int,
-        upload_url: Optional[str] = None,
-        profile_id: Optional[str] = None,
+        upload_url: str,
+        profile_id: str,
         profile_path: Optional[str] = None,
         profile_file: Optional[IO[bytes]] = None,
     ) -> Tuple[bool, str]:
         assert profile_path or profile_file, "Either a file or file path must be specified when uploading profiles"
-
-        # logger.debug("Generating the upload URL")
-        if upload_url and not profile_id:
-            raise ValueError("If upload_url is specified, profile_id must also be specified")
-        elif profile_id and not upload_url:
-            raise ValueError("If profile_id is specified, upload_url must also be specified")
-        elif not upload_url and not profile_id:
-            upload_url, profile_id = self._get_upload_url(dataset_timestamp=dataset_timestamp)
         try:
             if profile_file:
                 status, reason = self._put_file(profile_file, upload_url, dataset_timestamp)  # type: ignore
                 logger.debug(f"copied file {upload_url} status {status}:{reason}")
                 return status, profile_id  # type: ignore
             elif profile_path:
                 with open(profile_path, "rb") as f:
@@ -734,31 +559,76 @@
                     return status, profile_id  # type: ignore
         except requests.RequestException as e:
             logger.info(
                 f"Failed to upload {self._org_id}/{self._dataset_id}/{dataset_timestamp} to "
                 + f"{self.whylabs_api_endpoint} with API token ID: {self.key_id}. Error occurred: {e}"
             )
             return False, str(e)
-        return False, "Either a profile_file or profile_path must be specified when uploading profiles to WhyLabs!"
+        return False, "Imposible control flow"
 
     def _require(self, name: str, value: Optional[str]) -> None:
         if value is None:
-            session = _default_init()
+            session = default_init()
             session_type = session.get_type().value
             raise ValueError(
                 f"Can't determine {name}. Current session type is {session_type}. "
-                f"See {_INIT_DOCS} for instructions on using why.init()."
+                f"See {INIT_DOCS} for instructions on using why.init()."
             )
 
     def _validate_client(self) -> None:
         self._refresh_client()
         self._require("org id", self._org_id)
         self._require("default dataset id", self._dataset_id)
         self._require("api key", self._cache_config.api_key)
 
+    def _get_or_create_transaction_client(self) -> TransactionsApi:
+        self._refresh_client()
+        assert self._api_client is not None
+        return TransactionsApi(self._api_client)
+
+    def get_transaction_id(self) -> str:
+        client: TransactionsApi = self._get_or_create_transaction_client()
+        request = TransactionStartRequest(dataset_id=self._dataset_id)
+        result: LogTransactionMetadata = client.start_transaction(request)
+        logger.info(f"Starting transaction {result['transaction_id']}, expires {result['expiration_time']}")
+        return result["transaction_id"]
+
+    def commit_transaction(self, id: str) -> None:
+        logger.info(f"Committing transaction {id}")
+        client = self._get_or_create_transaction_client()
+        request = TransactionCommitRequest(verbose=True)
+        # We abandon the transaction if this throws
+        try:
+            client.commit_transaction(id, request)
+        except NotFoundException as e:
+            if "Transaction has been aborted" in str(e):  # TODO: perhaps not the most robust test?
+                logger.error(f"Transaction {id} was aborted; not committing")
+                raise TransactionAbortedException(f"Transaction {id} has been aborted")
+            else:
+                raise e
+
+    def abort_transaction(self, id: str) -> None:
+        logger.info(f"Aborting transaciton {id}")
+        client = self._get_or_create_transaction_client()
+        client.abort_transaction(id)
+
+    def transaction_status(self, id: str) -> Dict[str, Any]:
+        client = self._get_or_create_transaction_client()
+        return client.transaction_status(id)
+
+    def get_upload_url_transaction(
+        self, dataset_timestamp: int, whylabs_tags: List[SegmentTag] = []
+    ) -> Tuple[str, str]:
+        region = os.getenv("WHYLABS_UPLOAD_REGION", None)
+        client: TransactionsApi = self._get_or_create_transaction_client()
+        client.api_client.set_default_header("X-WhyLabs-File-Extension", "BIN")
+        request = TransactionLogRequest(dataset_timestamp=dataset_timestamp, segment_tags=whylabs_tags, region=region)
+        result: AsyncLogResponse = client.log_transaction(self._transaction_id, request)
+        return result.id, result.upload_url
+
     def _get_or_create_feature_weights_client(self) -> FeatureWeightsApi:
         self._validate_client()
         return FeatureWeightsApi(self._api_client)
 
     def _get_or_create_models_client(self) -> ModelsApi:
         self._validate_client()
         return ModelsApi(self._api_client)
@@ -768,35 +638,39 @@
         return LogApi(self._api_client)
 
     def _get_or_create_api_dataset_client(self) -> DatasetProfileApi:
         self._validate_client()
         return DatasetProfileApi(self._api_client)
 
     @staticmethod
-    def _build_log_async_request(dataset_timestamp: int) -> LogAsyncRequest:
-        return LogAsyncRequest(dataset_timestamp=dataset_timestamp, segment_tags=[])
+    def _build_log_async_request(dataset_timestamp: int, region: Optional[str] = None) -> LogAsyncRequest:
+        return LogAsyncRequest(dataset_timestamp=dataset_timestamp, segment_tags=[], region=region)
 
     @staticmethod
-    def _build_log_reference_request(dataset_timestamp: int, alias: Optional[str] = None) -> LogReferenceRequest:
-        return LogReferenceRequest(dataset_timestamp=dataset_timestamp, alias=alias)
+    def _build_log_reference_request(
+        dataset_timestamp: int, alias: Optional[str] = None, region: Optional[str] = None
+    ) -> LogReferenceRequest:
+        return LogReferenceRequest(dataset_timestamp=dataset_timestamp, alias=alias, region=region)
 
     @staticmethod
     def _build_log_segmented_reference_request(
-        dataset_timestamp: int, tags: Optional[dict] = None, alias: Optional[str] = None
+        dataset_timestamp: int, tags: Optional[dict] = None, alias: Optional[str] = None, region: Optional[str] = None
     ) -> LogReferenceRequest:
         segments = list()
         if not alias:
             alias = None
         if tags is not None:
             for segment_tags in tags:
                 segments.append(Segment(tags=[SegmentTag(key=tag["key"], value=tag["value"]) for tag in segment_tags]))
         if not segments:
-            return CreateReferenceProfileRequest(alias=alias, dataset_timestamp=dataset_timestamp)
+            return CreateReferenceProfileRequest(alias=alias, dataset_timestamp=dataset_timestamp, region=region)
         else:
-            return CreateReferenceProfileRequest(alias=alias, dataset_timestamp=dataset_timestamp, segments=segments)
+            return CreateReferenceProfileRequest(
+                alias=alias, dataset_timestamp=dataset_timestamp, segments=segments, region=region
+            )
 
     def _get_column_weights(self):
         feature_weight_api = self._get_or_create_feature_weights_client()
         try:
             result = feature_weight_api.get_column_weights(
                 org_id=self._org_id,
                 dataset_id=self._dataset_id,
@@ -806,22 +680,22 @@
             logger.exception(
                 f"Failed to upload {self._org_id}/{self._dataset_id} to "
                 f"{self.whylabs_api_endpoint}"
                 f" with API token ID: {self.key_id}"
             )
             raise e
 
-    def _put_feature_weights(self):
+    def _put_feature_weights(self, file: FeatureWeights):
         feature_weight_api = self._get_or_create_feature_weights_client()
         try:
             result = feature_weight_api.put_column_weights(
                 org_id=self._org_id,
                 dataset_id=self._dataset_id,
                 body={
-                    "segmentWeights": [self._feature_weights],
+                    "segmentWeights": [file.to_dict()],
                 },
                 _return_http_data_only=False,
             )
             return result[1]
         except ForbiddenException as e:
             logger.exception(
                 f"Failed to upload {self._org_id}/{self._dataset_id} to "
@@ -887,36 +761,64 @@
                 )
                 raise e
         else:
             no_update_made_message = f"column {column_name} was already classified {column_schema.classifier}."
             logger.info(no_update_made_message)
             return (200, no_update_made_message)
 
-    def _post_log_async(self, request: LogAsyncRequest, dataset_timestamp: int) -> AsyncLogResponse:
+    def _post_log_async(
+        self, request: LogAsyncRequest, dataset_timestamp: int, zip_file: bool = False
+    ) -> AsyncLogResponse:
         log_api = self._get_or_create_api_log_client()
+        if zip_file:
+            log_api.api_client.set_default_header("X-WhyLabs-File-Extension", "ZIP")
+        else:
+            log_api.api_client.set_default_header("X-WhyLabs-File-Extension", "BIN")
         try:
             result = log_api.log_async(org_id=self._org_id, dataset_id=self._dataset_id, log_async_request=request)
             return result
         except ForbiddenException as e:
             logger.exception(
                 f"Failed to upload {self._org_id}/{self._dataset_id}/{dataset_timestamp} to "
                 f"{self.whylabs_api_endpoint}"
                 f" with API token ID: {self.key_id}"
             )
             raise e
 
-    def _get_upload_urls_segmented_reference(self, whylabs_tags, dataset_timestamp: int) -> Tuple[str, List[str]]:
+    def _get_upload_urls_segmented_reference(
+        self, whylabs_tags, dataset_timestamp: int, reference_profile_name: str
+    ) -> Tuple[str, List[str]]:
+        region = os.getenv("WHYLABS_UPLOAD_REGION", None)
         request = self._build_log_segmented_reference_request(
-            dataset_timestamp, tags=whylabs_tags, alias=self._reference_profile_name
+            dataset_timestamp, tags=whylabs_tags, alias=reference_profile_name, region=region
+        )
+        res = self._post_log_segmented_reference(
+            request=request,
+            dataset_timestamp=dataset_timestamp,
         )
-        res = self._post_log_segmented_reference(request=request, dataset_timestamp=dataset_timestamp)
         return res["id"], res["upload_urls"]
 
-    def _post_log_segmented_reference(self, request: LogAsyncRequest, dataset_timestamp: int) -> LogReferenceResponse:
+    def _get_upload_url_segmented_reference_zip(
+        self, whylabs_tags, dataset_timestamp: int, reference_profile_name: str
+    ) -> Tuple[str, str]:
+        region = os.getenv("WHYLABS_UPLOAD_REGION", None)
+        request = self._build_log_segmented_reference_request(
+            dataset_timestamp, tags=whylabs_tags, alias=reference_profile_name, region=region
+        )
+        res = self._post_log_segmented_reference(request=request, dataset_timestamp=dataset_timestamp, zip_file=True)
+        return res["id"], res["upload_urls"][0]
+
+    def _post_log_segmented_reference(
+        self, request: LogAsyncRequest, dataset_timestamp: int, zip_file: bool = False
+    ) -> LogReferenceResponse:
         dataset_api = self._get_or_create_api_dataset_client()
+        if zip_file:
+            dataset_api.api_client.set_default_header("X-WhyLabs-File-Extension", "ZIP")
+        else:
+            dataset_api.api_client.set_default_header("X-WhyLabs-File-Extension", "BIN")
         try:
             async_result = dataset_api.create_reference_profile(
                 org_id=self._org_id,
                 dataset_id=self._dataset_id,
                 create_reference_profile_request=request,
                 async_req=not self._prefer_sync,
             )
@@ -946,27 +848,42 @@
             logger.exception(
                 f"Failed to upload {self._org_id}/{self._dataset_id}/{dataset_timestamp} to "
                 f"{self.whylabs_api_endpoint}"
                 f" with API token ID: {self.key_id}"
             )
             raise e
 
-    def _get_upload_url(self, dataset_timestamp: int) -> Tuple[str, str]:
-        if self._reference_profile_name is not None:
-            request = self._build_log_reference_request(dataset_timestamp, alias=self._reference_profile_name)
-            res = self._post_log_reference(request=request, dataset_timestamp=dataset_timestamp)
-        else:
-            request = self._build_log_async_request(dataset_timestamp)
-            res = self._post_log_async(request=request, dataset_timestamp=dataset_timestamp)
-
-        upload_url = res["upload_url"]
+    def get_upload_url_batch_zip(self, dataset_timestamp: int) -> Tuple[str, str]:
+        region = os.getenv("WHYLABS_UPLOAD_REGION", None)
+        request = self._build_log_async_request(dataset_timestamp, region=region)
+        res = self._post_log_async(request=request, dataset_timestamp=dataset_timestamp, zip_file=True)
+        upload_url = self._update_domain(res["upload_url"])
         profile_id = res["id"]
+        return profile_id, upload_url
 
+    def _update_domain(self, upload_url: str) -> str:
         if self._s3_private_domain:
             if _S3_PUBLIC_DOMAIN not in upload_url:
                 raise ValueError(
                     "S3 private domain is enabled but your account is not using S3 upload endpoint. " "Aborting!"
                 )
             upload_url = upload_url.replace(_S3_PUBLIC_DOMAIN, self._s3_private_domain)
             logger.debug(f"Replaced URL with our private domain. New URL: {upload_url}")
+        return upload_url
 
-        return upload_url, profile_id
+    def get_upload_url_unsegmented_reference(
+        self, dataset_timestamp: int, reference_profile_name: str
+    ) -> Tuple[str, str]:
+        region = os.getenv("WHYLABS_UPLOAD_REGION", None)
+        request = self._build_log_reference_request(dataset_timestamp, alias=reference_profile_name, region=region)
+        res = self._post_log_reference(request=request, dataset_timestamp=dataset_timestamp)
+        upload_url = self._update_domain(res["upload_url"])
+        profile_id = res["id"]
+        return profile_id, upload_url
+
+    def get_upload_url_batch(self, dataset_timestamp: int) -> Tuple[str, str]:
+        region = os.getenv("WHYLABS_UPLOAD_REGION", None)
+        request = self._build_log_async_request(dataset_timestamp, region=region)
+        res = self._post_log_async(request=request, dataset_timestamp=dataset_timestamp)
+        upload_url = self._update_domain(res["upload_url"])
+        profile_id = res["id"]
+        return profile_id, upload_url
```

### Comparing `whylogs-1.3.9.dev0/whylogs/core/__init__.py` & `whylogs-1.4.0rc0/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/column_profile.py` & `whylogs-1.4.0rc0/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/configs.py` & `whylogs-1.4.0rc0/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.4.0rc0/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/dataset_profile.py` & `whylogs-1.4.0rc0/whylogs/core/dataset_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
-import os.path
 import time
 from datetime import datetime, timezone
-from typing import Any, Dict, Mapping, Optional, Tuple, Union
+from typing import Any, Dict, List, Mapping, Optional, Tuple, Union
 
 from whylogs.api.writer.writer import Writable
 from whylogs.core.metrics import Metric
 from whylogs.core.model_performance_metrics.model_performance_metrics import (
     ModelPerformanceMetrics,
 )
 from whylogs.core.preprocessing import ColumnProperties
@@ -265,26 +264,25 @@
             metadata=self._metadata,
         )
 
     def flush(self) -> None:
         for col in self._columns.values():
             col.flush()
 
-    @staticmethod
-    def get_default_path(path) -> str:
-        if not path.endswith("bin"):
-            path = os.path.join(path, f"profile.{int(round(time.time() * 1000))}.bin")
-        return path
+    def _get_default_filename(self) -> str:
+        return f"profile.{int(round(time.time() * 1000))}.bin"
 
     @deprecated_alias(path_or_base_dir="path")
-    def write(self, path: Optional[str] = None, **kwargs: Any) -> Tuple[bool, str]:
-        output_path = self.get_default_path(path=path)
-        response = self.view().write(output_path)
-        logger.debug("Wrote profile to path: %s", output_path)
-        return response
+    def write(
+        self, path: Optional[str] = None, filename: Optional[str] = None, **kwargs: Any
+    ) -> Tuple[bool, Union[str, List[str]]]:
+        filename = filename or self._get_default_filename()
+        success, files = self.view().write(path, filename, **kwargs)
+        logger.debug(f"Wrote profile to path: {files}")
+        return success, files
 
     @classmethod
     def read(cls, input_path: str) -> DatasetProfileView:
         return DatasetProfileView.read(input_path)
 
     def __repr__(self) -> str:
         return f"DatasetProfile({len(self._columns)} columns). Schema: {str(self._schema)}"
```

### Comparing `whylogs-1.3.9.dev0/whylogs/core/datatypes.py` & `whylogs-1.4.0rc0/whylogs/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/errors.py` & `whylogs-1.4.0rc0/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/input_resolver.py` & `whylogs-1.4.0rc0/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metadata.py` & `whylogs-1.4.0rc0/whylogs/core/metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import json
 import logging
 from datetime import datetime, timezone
 from typing import Any, Dict, List, Optional
 from uuid import uuid4
 
+from whylogs.context.version import whylogs_version
 from whylogs.core.utils.timestamp_calculations import to_utc_milliseconds
 
 diagnostic_logger = logging.getLogger(__name__)
 
 WHYLABS_TRACE_ID_KEY = "whylabs.traceId"
 CREATION_TIMESTAMP_KEY = "whylogs.creationTimestamp"
 DATASET_TIMESTAMP_KEY = "whylogs.datasetTimestamp"
 USER_TAGS_KEY = "whylogs.user.tags"
 NAME_KEY = "whylogs.name"
+WHYLOGS_VERSION_KEY = "whylogs.version"
 
 
 def _populate_common_profile_metadata(
     metadata: Optional[Dict[str, str]] = None,
     *,
     name: Optional[str] = None,
     trace_id: Optional[str] = None,
@@ -33,15 +35,15 @@
 
     if metadata is None:
         metadata = dict()
     if WHYLABS_TRACE_ID_KEY not in metadata:
         if not trace_id:
             trace_id = str(uuid4())
         metadata[WHYLABS_TRACE_ID_KEY] = trace_id
-    elif metadata[WHYLABS_TRACE_ID_KEY] != trace_id:
+    elif metadata[WHYLABS_TRACE_ID_KEY] != trace_id and trace_id is not None:
         diagnostic_logger.warning(
             f"trace_id was specified as {trace_id} but there is already a trace_id defined "
             f"in metadata[{WHYLABS_TRACE_ID_KEY}]: {metadata[WHYLABS_TRACE_ID_KEY]}"
         )
 
     if CREATION_TIMESTAMP_KEY not in metadata:
         metadata[CREATION_TIMESTAMP_KEY] = str(to_utc_milliseconds(datetime.now(timezone.utc)))
@@ -49,8 +51,29 @@
         metadata[DATASET_TIMESTAMP_KEY] = str(timestamp)
 
     if name and NAME_KEY not in metadata:
         metadata[NAME_KEY] = name
     if tags and USER_TAGS_KEY not in metadata:
         metadata[USER_TAGS_KEY] = json.dumps(sorted(set(tags)))
 
+    if WHYLOGS_VERSION_KEY not in metadata:
+        metadata[WHYLOGS_VERSION_KEY] = whylogs_version
+
     return metadata
+
+
+def _safe_merge_metadata(
+    default_metadata: Optional[Dict[str, str]], incoming_metadata: Optional[Dict[str, str]]
+) -> Dict[str, str]:
+    if default_metadata is None:
+        default_metadata = dict()
+    if not incoming_metadata:
+        return default_metadata
+
+    for key in incoming_metadata:
+        if not default_metadata.get(key):
+            default_metadata[key] = incoming_metadata[key]
+        elif incoming_metadata[key] != default_metadata[key] and incoming_metadata[key]:
+            diagnostic_logger.warning(
+                f"metadata collision on key {key}. Current value is {default_metadata[key]} so ignoring attempt to set to {incoming_metadata[key]}"
+            )
+    return default_metadata
```

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metric_getters.py` & `whylogs-1.4.0rc0/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/__init__.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/aggregators.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/column_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/compound_metric.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/condition_count_metric.py`

 * *Files 26% similar despite different names*

```diff
@@ -54,28 +54,92 @@
 
 def not_relation(relation: Callable[[Any], bool]) -> Callable[[Any], bool]:
     return lambda x: not relation(x)
 
 
 @dataclass(frozen=True)
 class Condition:
+    """
+    Condition to be evaluated by the ConditionCountMetric.
+
+    Parameters
+    ----------
+    relation: Callable[[Any], bool]
+        The predicate to evaluate. The callable is passed a value from the column the
+        ConditionCountMetric is attached to, and returns True if the value satisfies
+        the condition.
+    throw_on_failure: bool
+        If throw_on_failure is true, whylogs will immediately raise a ValueError if
+        data that does not satisfy the condition is logged.
+    log_on_failure: bool
+        If log_on_failure is true, whylogs will log a warning message if data that does not
+        satisfy the conditon is logged.
+    actions: List[Callable[[str, str, Any], None]]
+        A list of callables that will be invoked if data that does not satisfy the conditon
+        is logged. The arguments passed to the callable are the metric's name ("condition_count"),
+        the name of the failed condition, and the value that caused the failure.
+    """
+
     relation: Callable[[Any], bool]
     throw_on_failure: bool = False
     log_on_failure: bool = False
     actions: List[Callable[[str, str, Any], None]] = field(default_factory=list)
 
 
 @dataclass(frozen=True)
 class ConditionCountConfig(MetricConfig):
     conditions: Dict[str, Condition] = field(default_factory=dict)
     exclude_from_serialization: bool = False
 
 
 @dataclass(frozen=True)
 class ConditionCountMetric(Metric):
+    """
+    A whylogs metric that counts how many column entries satisfy a condition.
+
+    Parameters
+    ----------
+    conditions: Dict[str, Condition]
+        The conditions evaluated by the metric. The key is the condition name, and the
+        Condition value specifies the Callable condition predicate to evaluate & count.
+
+    Examples
+    --------
+    This example counts the occurrances of email addresses in the `some_text` column and
+    credit card numbers in the `more_text` column.
+
+    ```
+    import pandas as pd
+    import whylogs as why
+    from whylogs.core.resolvers import STANDARD_RESOLVER
+    from whylogs.core.specialized_resolvers import ConditionCountMetricSpec
+    from whylogs.core.metrics.condition_count_metric import Condition
+    from whylogs.core.relations import Predicate
+    from whylogs.core.schema import DeclarativeSchema
+
+    email_condition = {"contiansEmail": Condition(Predicate().fullmatch("[\\w.]+[\\._]?[a-z0-9]+[@]\\w+[.]\\w{2,3}"))}
+    cc_condition = {"containsCreditCard": Condition(Predicate().matches(".*4[0-9]{12}(?:[0-9]{3})?"))}
+
+    schema = DeclarativeSchema(STANDARD_RESOLVER)
+    schema.add_resolver_spec(column_name="some_text", metrics=[ConditionCountMetricSpec(email_condition)])
+    schema.add_resolver_spec(column_name="more_text", metrics=[ConditionCountMetricspec(cc_condition)])
+
+    df = pd.DataFrame({"some_text": ["not an email", "bob@spam.com"], "more_text": ["frogs", "4000000000000"]})
+    view = why.log(df).view()
+    view.to_pandas()[['condition_count/containsEmail', 'condition_count/containsCreditCard', 'condition_count/total']]
+
+    # results in
+
+               condition_count/containsEmail   condition_count/containsCreditCard      condition_count/total
+    column
+    some_text                            1.0                                  NaN                          2
+    more_text                            NaN                                  1.0                          2
+    ```
+    """
+
     conditions: Dict[str, Condition]
     total: IntegralComponent
     matches: Dict[str, IntegralComponent] = field(default_factory=dict)
     hide_from_serialization: bool = False
 
     @property
     def exclude_from_serialization(self) -> bool:
@@ -126,37 +190,39 @@
         return paths
 
     def columnar_update(self, data: PreprocessedColumn) -> OperationResult:
         if data.len <= 0:
             return OperationResult.ok(0)
 
         count = 0
-        failed_conditions: Set[str] = set()
+        log_conditions: Set[str] = set()
+        throw_conditions: Set[str] = set()
         for datum in list(chain.from_iterable(data.raw_iterator())):
             count += 1
             for cond_name, condition in self.conditions.items():
                 try:
                     if condition.relation(datum):
                         self.matches[cond_name].set(self.matches[cond_name].value + 1)
                     else:
-                        failed_conditions.add(cond_name)
+                        if condition.log_on_failure:
+                            log_conditions.add(cond_name)
+                        if condition.throw_on_failure:
+                            throw_conditions.add(cond_name)
                         for action in condition.actions:
                             action(self.namespace, cond_name, datum)
 
                 except Exception as e:  # noqa
                     logger.debug(e)
-                    failed_conditions.add(cond_name)
 
         self.total.set(self.total.value + count)
-        if failed_conditions:
-            if condition.log_on_failure:
-                logger.warning(f"Condition(s) {', '.join(failed_conditions)} failed")
+        if log_conditions:
+            logger.warning(f"Conditions {', '.join(list(log_conditions))} failed")
 
-            if condition.throw_on_failure:
-                raise ValueError(f"Condition(s) {', '.join(failed_conditions)} failed")
+        if throw_conditions:
+            raise ValueError(f"Condition {', '.join(list(throw_conditions))} failed")
 
         return OperationResult.ok(count)
 
     @classmethod
     def zero(cls, config: Optional[MetricConfig] = None) -> "ConditionCountMetric":
         config = config or ConditionCountConfig()
         if not isinstance(config, ConditionCountConfig):
```

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/decorators.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/deserializers.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/maths.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/metric_components.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/metrics.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/multimetric.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/serializers.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/metrics/unicode_range.py` & `whylogs-1.4.0rc0/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.4.0rc0/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/predicate_parser.py` & `whylogs-1.4.0rc0/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/preprocessing.py` & `whylogs-1.4.0rc0/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.py` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.py` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.py` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.4.0rc0/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/proto/whylogs_messages_pb2.py` & `whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.4.0rc0/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/relations.py` & `whylogs-1.4.0rc0/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/resolvers.py` & `whylogs-1.4.0rc0/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/schema.py` & `whylogs-1.4.0rc0/whylogs/core/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from copy import deepcopy
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Mapping, Optional, Tuple, TypeVar
+from typing import Any, Dict, List, Mapping, Optional, Set, Tuple, TypeVar, Union
 
 import whylogs.core.resolvers as res
 from whylogs.core.datatypes import StandardTypeMapper, TypeMapper
 from whylogs.core.metrics.metrics import Metric, MetricConfig
 from whylogs.core.resolvers import (
     DeclarativeResolver,
     MetricSpec,
@@ -73,24 +73,26 @@
         default_configs: Optional[MetricConfig] = None,
         type_mapper: Optional[TypeMapper] = None,
         resolvers: Optional[Resolver] = None,
         cache_size: int = 1024,
         schema_based_automerge: bool = False,
         segments: Optional[Dict[str, SegmentationPartition]] = None,
         validators: Optional[Dict[str, List[Validator]]] = None,
+        metadata: Optional[Dict[str, str]] = None,
     ) -> None:
         self._columns = dict()
         self.types = types or dict()
         self.default_configs = default_configs or MetricConfig()
         self.type_mapper = type_mapper or StandardTypeMapper()
         self.resolvers = resolvers if resolvers is not None else DeclarativeResolver()
         self.cache_size = cache_size
         self.schema_based_automerge = schema_based_automerge
         self.segments = segments or dict()
         self.validators = validators or dict()
+        self.metadata = metadata or dict()
 
         if self.cache_size < 0:
             logger.warning("Negative cache size value. Disabling caching")
             self.cache_size = 0
 
         if self.cache_size > LARGE_CACHE_SIZE_LIMIT:
             logger.warning(
@@ -118,14 +120,15 @@
         key_dict = vars(self).copy()
         key_dict.pop("_columns")
         keys = key_dict.keys()
         args = {k: deepcopy(self.__dict__[k]) for k in keys if k not in self.types}
         copy = self.__class__(**args)
         copy._columns = deepcopy(self._columns)
         copy.segments = self.segments.copy()
+        copy.metadata = self.metadata.copy()
         return copy
 
     def resolve(
         self,
         *,
         pandas: Optional[pd.DataFrame] = None,
         row: Optional[Mapping[str, Any]] = None,
@@ -225,54 +228,66 @@
     """
 
     def add_resolver(self, resolver_spec: ResolverSpec):
         self.resolvers.add_resolver(resolver_spec)
 
     def add_resolver_spec(
         self,
-        column_name: Optional[str] = None,
+        column_name: Optional[Union[str, Set[str]]] = None,
         column_type: Optional[Any] = None,
         metrics: Optional[List[MetricSpec]] = None,
     ):
+        if column_name is not None and not isinstance(column_name, (str, set)):
+            raise ValueError("column_name must be a stirng or set of strings")
+
+        if isinstance(column_name, set):
+            for name in column_name:
+                spec = ResolverSpec(column_name=name, column_type=column_type, metrics=metrics or [])
+                self.add_resolver(spec)
+            return
+
         spec = ResolverSpec(column_name=column_name, column_type=column_type, metrics=metrics or [])
         self.add_resolver(spec)
 
     def __init__(
         self,
         resolvers: Optional[List[ResolverSpec]] = None,
         types: Optional[Dict[str, Any]] = None,
         default_config: Optional[MetricConfig] = None,
         type_mapper: Optional[TypeMapper] = None,
         cache_size: int = 1024,
         schema_based_automerge: bool = False,
         segments: Optional[Dict[str, SegmentationPartition]] = None,
         validators: Optional[Dict[str, List[Validator]]] = None,
+        metadata: Optional[Dict[str, str]] = None,
     ) -> None:
         if resolvers is None:
             resolvers = res.DEFAULT_RESOLVER
             logger.warning("No columns specified in DeclarativeSchema")
         resolver = DeclarativeResolver(resolvers, default_config)
         super().__init__(
             types=types,
             default_configs=default_config,
             type_mapper=type_mapper,
             resolvers=resolver,
             cache_size=cache_size,
             schema_based_automerge=schema_based_automerge,
             segments=segments,
             validators=validators,
+            metadata=metadata,
         )
 
     def copy(self) -> "DeclarativeSchema":
         copy = DeclarativeSchema(
             [],
             deepcopy(self.types),
             deepcopy(self.default_configs),
             deepcopy(self.type_mapper),
             self.cache_size,
             self.schema_based_automerge,
             self.segments.copy(),
             deepcopy_validators(self.validators),
+            metadata=self.metadata.copy(),
         )
         copy.resolvers = deepcopy(self.resolvers)
         copy._columns = deepcopy(self._columns)
         return copy
```

### Comparing `whylogs-1.3.9.dev0/whylogs/core/segmentation_partition.py` & `whylogs-1.4.0rc0/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/specialized_resolvers.py` & `whylogs-1.4.0rc0/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/stubs.py` & `whylogs-1.4.0rc0/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.4.0rc0/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/utils/stats_calculations.py` & `whylogs-1.4.0rc0/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/utils/utils.py` & `whylogs-1.4.0rc0/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/validators/condition_validator.py` & `whylogs-1.4.0rc0/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/validators/validator.py` & `whylogs-1.4.0rc0/whylogs/core/validators/validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/view/column_profile_view.py` & `whylogs-1.4.0rc0/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.4.0rc0/whylogs/core/view/dataset_profile_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import io
 import logging
+import os
 import tempfile
 from datetime import datetime, timezone
 from enum import Enum
-from typing import Any, BinaryIO, Dict, List, Optional, Tuple
+from typing import Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
 from google.protobuf.message import DecodeError
 
 from whylogs.api.writer.writer import Writable
 from whylogs.core.configs import SummaryConfig
 from whylogs.core.errors import DeserializationError
 from whylogs.core.proto import (
@@ -181,37 +182,40 @@
 
     def get_columns(self, col_names: Optional[List[str]] = None) -> Dict[str, ColumnProfileView]:
         if col_names:
             return {k: self._columns.get(k) for k in col_names}
         else:
             return {k: self._columns.get(k) for k in self._columns}
 
-    def get_default_path(self) -> str:
+    def _get_default_filename(self) -> str:
         return f"profile_{self.creation_timestamp}.bin"
 
-    def write(self, path: Optional[str] = None, **kwargs: Any) -> Tuple[bool, str]:
-        file_to_write = kwargs.get("file")
-        path = file_to_write.name if file_to_write else path or self.get_default_path()
+    def _write(self, out_f: BinaryIO) -> Tuple[bool, str]:
         if self._metrics and _MODEL_PERFORMANCE in self._metrics:
             from whylogs.migration.converters import v1_to_dataset_profile_message_v0
 
             message_v0 = v1_to_dataset_profile_message_v0(self, None, None)
-            if file_to_write:
-                write_delimited_protobuf(file_to_write, message_v0)
-            else:
-                with open(path, "w+b") as out_f:
-                    write_delimited_protobuf(out_f, message_v0)
+            write_delimited_protobuf(out_f, message_v0)
+            return True, out_f.name
 
-            return True, path
-        if file_to_write:
-            self._do_write(file_to_write)
-        else:
-            with open(path, "w+b") as out_f:
-                self._do_write(out_f)
-        return True, path
+        self._do_write(out_f)
+        return True, out_f.name
+
+    def write(
+        self, path: Optional[str] = None, filename: Optional[str] = None, **kwargs: Any
+    ) -> Tuple[bool, Union[str, List[str]]]:
+        file_to_write = kwargs.get("file")
+        if file_to_write is None:
+            path = path if path is not None else self._get_default_path()
+            filename = filename if filename is not None else self._get_default_filename()
+            path = os.path.join(path, filename) if path is not None else filename
+            with Writable._safe_open_write(path, "+b") as out_f:
+                return self._write(out_f)
+
+        return self._write(file_to_write)
 
     @staticmethod
     def _split_tags_and_metadata(
         tags: Optional[Dict[str, str]]
     ) -> Tuple[Optional[Dict[str, str]], Optional[Dict[str, str]]]:
         # nothing to split, return (None, None)
         # for use in serializing dataset property's tags and metadata
@@ -427,21 +431,34 @@
         copy = DatasetProfileView.deserialize(state)
         self._columns = copy._columns
         self._dataset_timestamp = copy._dataset_timestamp
         self._creation_timestamp = copy._creation_timestamp
         self._metrics = copy._metrics
         self._metadata = copy._metadata
 
+    def _is_uncompounded(self, col_name):
+        groups = col_name.split(".")
+        metric = groups[0]
+        if not len(groups) > 1:
+            return False
+        if metric in self._columns.keys():
+            for metric_name in self._columns[metric].get_metric_component_paths():
+                new_metric_name = metric_name.split(":")[0].replace("/", ".")
+                if col_name == new_metric_name:
+                    return True
+        return False
+
     def to_pandas(self, column_metric: Optional[str] = None, cfg: Optional[SummaryConfig] = None) -> pd.DataFrame:
         all_dicts = []
         if self._columns:
             for col_name, col in sorted(self._columns.items()):
-                sum_dict = col.to_summary_dict(column_metric=column_metric, cfg=cfg)
-                sum_dict["column"] = col_name
-                sum_dict["type"] = SummaryType.COLUMN
-                all_dicts.append(dict(sorted(sum_dict.items())))
+                if not self._is_uncompounded(col_name):
+                    sum_dict = col.to_summary_dict(column_metric=column_metric, cfg=cfg)
+                    sum_dict["column"] = col_name
+                    sum_dict["type"] = SummaryType.COLUMN
+                    all_dicts.append(dict(sorted(sum_dict.items())))
             if is_not_stub(pd.DataFrame):
                 df = pd.DataFrame(all_dicts)
                 return df.set_index("column")
             else:
                 raise ImportError("Pandas is not installed. Please install pandas to use this feature.")
         return pd.DataFrame(all_dicts)
```

### Comparing `whylogs-1.3.9.dev0/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.4.0rc0/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import os
 import tempfile
 from datetime import datetime
 from logging import getLogger
-from typing import IO, Any, Dict, Optional, Tuple
+from typing import IO, Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
 from whylogs.api.writer.writer import Writable
 from whylogs.core.proto import (
     ChunkHeader,
     ChunkMessage,
     ChunkOffsets,
     DatasetProfileHeader,
@@ -72,30 +73,24 @@
     def model_performance_metrics(self) -> Any:
         return self.profile_view.model_performance_metrics
 
     @property
     def metadata(self) -> Dict[str, str]:
         return self.profile_view.metadata
 
-    def get_default_path(self) -> str:
+    def _get_default_filename(self) -> str:
         return f"profile_{self._profile_view.creation_timestamp}_{self.get_segment_string()}.bin"
 
     def get_segment_string(self) -> str:
         return f"{self._segment.parent_id}_{'_'.join(self._segment.key)}"
 
-    def _write_as_v0_message(self, path: Optional[str] = None, **kwargs: Any) -> Tuple[bool, str]:
+    def _write_as_v0_message(self, out_f: BinaryIO) -> Tuple[bool, str]:
         message_v0 = v1_to_dataset_profile_message_v0(self.profile_view, self.segment, self.partition)
-        file_to_write = kwargs.get("file")
-        path = file_to_write.name if file_to_write else path or self.get_default_path()
-        if file_to_write:
-            write_delimited_protobuf(file_to_write, message_v0)
-        else:
-            with open(path, "w+b") as out_f:
-                write_delimited_protobuf(out_f, message_v0)
-        return True, path
+        write_delimited_protobuf(out_f, message_v0)
+        return True, out_f.name
 
     def _copy_write(
         self,
         source_profile_file: IO[bytes],
         output_file: IO[bytes],
         total_len: int,
         dataset_segment_header: DatasetSegmentHeader,
@@ -113,18 +108,18 @@
 
         source_profile_file.seek(0)
         while source_profile_file.tell() < total_len:
             buffer = source_profile_file.read(_BUFFER_CHUNK)
             output_file.write(buffer)
         logger.debug(f"Writing segmented profile file: complete! total of {output_file.tell()} bytes written.")
 
-    def _write_v1(self, path: Optional[str] = None, **kwargs: Any) -> Tuple[bool, str]:
+    def _write_v1(self, out_f: BinaryIO) -> Tuple[bool, str]:
         all_metric_component_names = set()
-        file_to_write = kwargs.get("file")
-        path = file_to_write.name if file_to_write else path or self.get_default_path()
+        file_to_write = out_f
+        path = file_to_write.name
 
         # capture the list of all metric component paths
         for col in self.profile_view._columns.values():
             all_metric_component_names.update(col.get_metric_component_paths())
         metric_name_list = list(all_metric_component_names)
         metric_name_list.sort()
         metric_name_indices: Dict[str, int] = {}
@@ -207,23 +202,33 @@
             write_delimited_protobuf(f, dataset_segment_header)
             first_segment_offset = f.tell() - total_len
             dataset_segment_header.offsets[0] = first_segment_offset
 
             # only single segment files at first.
             dataset_segment_header.segments.extend(segments_message_field)
 
-            if file_to_write:
-                self._copy_write(f, file_to_write, total_len, dataset_segment_header, dataset_header)
-            else:
-                with open(path, "w+b") as out_f:
-                    self._copy_write(f, out_f, total_len, dataset_segment_header, dataset_header)
+            self._copy_write(f, file_to_write, total_len, dataset_segment_header, dataset_header)
+
         return True, path
 
-    def write(self, path: Optional[str] = None, **kwargs: Any) -> Tuple[bool, str]:
+    def _write(self, out_f: BinaryIO, **kwargs: Any) -> Tuple[bool, str]:
         if kwargs.get("use_v0") or self.profile_view.model_performance_metrics:
             if self.profile_view.model_performance_metrics:
                 logger.info("Converting segmented profile with performance metrics to v0 format before writing.")
             else:
                 logger.info("writing segmented profile as v0 format.")
-            return self._write_as_v0_message(path, **kwargs)
+            return self._write_as_v0_message(out_f)
         else:
-            return self._write_v1(path, **kwargs)
+            return self._write_v1(out_f)
+
+    def write(
+        self, path: Optional[str] = None, filename: Optional[str] = None, **kwargs: Any
+    ) -> Tuple[bool, Union[str, List[str]]]:
+        out_f = kwargs.get("file")
+        if out_f is not None:
+            return self._write(out_f, **kwargs)
+
+        path = path if path is not None else self._get_default_path()
+        filename = filename if filename is not None else self._get_default_filename()
+        path = os.path.join(path, filename) if path is not None else filename
+        with Writable._safe_open_write(path, "+b") as out_f:
+            return self._write(out_f, **kwargs)
```

### Comparing `whylogs-1.3.9.dev0/whylogs/datasets/base.py` & `whylogs-1.4.0rc0/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/datasets/configs.py` & `whylogs-1.4.0rc0/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.4.0rc0/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/datasets/descr/employee.rst` & `whylogs-1.4.0rc0/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/datasets/descr/weather.rst` & `whylogs-1.4.0rc0/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/datasets/ecommerce.py` & `whylogs-1.4.0rc0/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/datasets/employee.py` & `whylogs-1.4.0rc0/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/datasets/utils.py` & `whylogs-1.4.0rc0/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/datasets/weather.py` & `whylogs-1.4.0rc0/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.4.0rc0/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.4.0rc0/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/core/udf_schema.py` & `whylogs-1.4.0rc0/whylogs/experimental/core/udf_schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -49,53 +49,110 @@
     """
 
     column_names: Optional[List[str]] = None
     udfs: Dict[str, Callable[[Any], Any]] = field(
         default_factory=dict
     )  # new column name -> callable to compute new column value
     column_type: Optional[DataType] = None
+    prefix: Optional[str] = None
+
+    # for multiple output column UDFs
+    udf: Optional[Callable[[Any], Any]] = None
+    name: Optional[str] = None
 
     def __post_init__(self):
         if self.column_type is not None:
             if self.column_names:
                 raise ValueError("UdfSpec cannot specify both column_names and column_type")
         elif self.column_names is None:
             raise ValueError("UdfSpec must specify column_names or column_type")
         elif len(self.column_names) == 0 or not all([isinstance(x, str) for x in self.column_names]):
             raise ValueError("UdfSpec column_names must be a non-empty list of strings")
 
 
 def _apply_udfs_on_row(
     values: Union[List, Dict[str, List]], udfs: Dict, new_columns: Dict[str, Any], input_cols: Collection[str]
 ) -> None:
+    """multiple input columns, single output column"""
     for new_col, udf in udfs.items():
         if new_col in input_cols:
             continue
 
         try:
             new_columns[new_col] = udf(values)[0]
         except Exception:  # noqa
             new_columns[new_col] = None
             logger.exception(f"Evaluating UDF {new_col} failed")
 
 
+def _apply_udf_on_row(
+    name: str,
+    prefix: Optional[str],
+    values: Union[List, Dict[str, List]],
+    udf: Callable,
+    new_columns: Dict[str, Any],
+    input_cols: Collection[str],
+) -> None:
+    """
+    multiple input columns, multiple output columns
+    udf(Union[Dict[str, List], pd.DataFrame]) -> Union[Dict[str, List], pd.DataFrame]
+    """
+
+    try:
+        # TODO: Document assumption: dictionary in -> dictionary out
+        for new_col, value in udf(values).items():
+            new_col = prefix + "." + new_col if prefix else new_col
+            new_columns[new_col] = value[0]
+
+    except Exception as e:  # noqa
+        logger.exception(f"Evaluating UDF {name} failed with error {e}")
+
+
 def _apply_udfs_on_dataframe(
     pandas: pd.DataFrame, udfs: Dict, new_df: pd.DataFrame, input_cols: Collection[str]
 ) -> None:
+    """multiple input columns, single output column"""
     for new_col, udf in udfs.items():
         if new_col in input_cols:
             continue
 
         try:
             new_df[new_col] = pd.Series(udf(pandas))
         except Exception as e:  # noqa
             new_df[new_col] = pd.Series([None])
             logger.exception(f"Evaluating UDF {new_col} failed on columns {pandas.keys()} with error {e}")
 
 
+def _apply_udf_on_dataframe(
+    name: str,
+    prefix: Optional[str],
+    pandas: pd.DataFrame,
+    udf: Callable,
+    new_df: pd.DataFrame,
+    input_cols: Collection[str],
+) -> None:
+    """
+    multiple input columns, multiple output columns
+    udf(Union[Dict[str, List], pd.DataFrame]) -> Union[Dict[str, List], pd.DataFrame]
+    """
+
+    def add_prefix(col):
+        return prefix + "." + col if prefix else col
+
+    try:
+        # TODO: I think it's OKAY if udf returns a dictionary
+        udf_output = pd.DataFrame(udf(pandas))
+        udf_output = udf_output.rename(columns={old: add_prefix(old) for old in udf_output.keys()})
+        for new_col in udf_output.keys():
+            new_df[new_col] = udf_output[new_col]
+    except Exception as e:  # noqa
+        logger.exception(f"Evaluating UDF {name} failed on columns {pandas.keys()} with error {e}")
+        return pd.DataFrame()
+
+
 def _apply_type_udfs(pandas: pd.Series, udfs: Dict, new_df: pd.DataFrame, input_cols: Collection[str]) -> None:
     for new_col, udf in udfs.items():
         if new_col in input_cols:
             continue
 
         try:
             new_df[new_col] = pd.Series(udf(pandas))
@@ -147,46 +204,54 @@
 
     def _run_udfs_on_row(
         self, row: Mapping[str, Any], new_columns: Dict[str, Any], input_cols: Collection[str]
     ) -> None:
         for spec in self.multicolumn_udfs:
             if spec.column_names and set(spec.column_names).issubset(set(row.keys())):
                 inputs = {col: [row[col]] for col in spec.column_names}
-                _apply_udfs_on_row(inputs, spec.udfs, new_columns, input_cols)
+                if spec.udf is not None:
+                    _apply_udf_on_row(spec.name, spec.prefix, inputs, spec.udf, new_columns, input_cols)  # type: ignore
+                else:
+                    _apply_udfs_on_row(inputs, spec.udfs, new_columns, input_cols)
 
         for column, value in row.items():
             why_type = type(self.type_mapper(type(value)))
             for spec in self.type_udfs[why_type]:
                 udfs = {f"{column}.{key}": spec.udfs[key] for key in spec.udfs.keys()}
                 _apply_udfs_on_row([value], udfs, new_columns, input_cols)
 
     def _run_udfs_on_dataframe(self, pandas: pd.DataFrame, new_df: pd.DataFrame, input_cols: Collection[str]) -> None:
         for spec in self.multicolumn_udfs:
             if spec.column_names and set(spec.column_names).issubset(set(pandas.keys())):
-                _apply_udfs_on_dataframe(pandas[spec.column_names], spec.udfs, new_df, input_cols)
+                if spec.udf is not None:
+                    _apply_udf_on_dataframe(
+                        spec.name, spec.prefix, pandas[spec.column_names], spec.udf, new_df, input_cols  # type: ignore
+                    )
+                else:
+                    _apply_udfs_on_dataframe(pandas[spec.column_names], spec.udfs, new_df, input_cols)
 
         for column, dtype in pandas.dtypes.items():
             why_type = type(self.type_mapper(dtype))
             for spec in self.type_udfs[why_type]:
                 udfs = {f"{column}.{key}": spec.udfs[key] for key in spec.udfs.keys()}
                 _apply_type_udfs(pandas[column], udfs, new_df, input_cols)
 
     def _run_udfs(
         self, pandas: Optional[pd.DataFrame] = None, row: Optional[Dict[str, Any]] = None
     ) -> Tuple[Optional[pd.DataFrame], Optional[Mapping[str, Any]]]:
         new_columns = deepcopy(row) if row else None
-        new_df = pd.DataFrame() if pandas is not None else None
+        new_df = pd.DataFrame()
         if row is not None:
             self._run_udfs_on_row(row, new_columns, row.keys())  # type: ignore
 
         if pandas is not None:
             self._run_udfs_on_dataframe(pandas, new_df, pandas.keys())
             new_df = pd.concat([pandas, new_df], axis=1)
 
-        return new_df, new_columns
+        return new_df if pandas is not None else None, new_columns
 
     def apply_udfs(
         self, pandas: Optional[pd.DataFrame] = None, row: Optional[Dict[str, Any]] = None
     ) -> Tuple[Optional[pd.DataFrame], Optional[Mapping[str, Any]]]:
         return self._run_udfs(pandas, row)
 
 
@@ -199,14 +264,54 @@
         _reset_metric_udfs()
 
     global _multicolumn_udfs, _resolver_specs
     _multicolumn_udfs = defaultdict(list)
     _resolver_specs = defaultdict(list)
 
 
+def register_multioutput_udf(
+    col_names: List[str],
+    udf_name: Optional[str] = None,
+    prefix: Optional[str] = None,
+    namespace: Optional[str] = None,
+    schema_name: str = "",
+    no_prefix: bool = False,
+) -> Callable[[Any], Any]:
+    """
+    Decorator to easily configure UDFs for your data set. Decorate your UDF
+    functions, then call generate_udf_dataset_schema() to create a UdfSchema
+    that includes the UDFs configured by your decorator parameters. The decorated
+    function will automatically be a UDF in the UdfSchema.
+
+    Specify udf_name to give the output of the UDF a name. udf_name
+    defautls to the name of the decorated function. Note that all lambdas are
+    named "lambda", so omitting udf_name on more than one lambda will result
+    in name collisions. If you pass a namespace, it will be prepended to the UDF name.
+    Specifying schema_name will register the UDF in a particular schema. If omitted,
+    it will be registered to the defualt schema.
+
+    For multiple output column UDFs, the udf_name is prepended to the column
+    name supplied by the UDF. The signature for multiple output column UDFs
+    is f(Union[Dict[str, List], pd.DataFrame]) -> Union[Dict[str, List], pd.DataFrame]
+    """
+
+    def decorator_register(func):
+        global _multicolumn_udfs
+        name = udf_name or func.__name__
+        name = f"{namespace}.{name}" if namespace else name
+        if no_prefix:
+            output_prefix = None
+        else:
+            output_prefix = prefix if prefix else name
+        _multicolumn_udfs[schema_name].append(UdfSpec(col_names, prefix=output_prefix, udf=func, name=name))
+        return func
+
+    return decorator_register
+
+
 def register_dataset_udf(
     col_names: List[str],
     udf_name: Optional[str] = None,
     metrics: Optional[List[MetricSpec]] = None,
     namespace: Optional[str] = None,
     schema_name: str = "",
     anti_metrics: Optional[List[Metric]] = None,
@@ -242,14 +347,31 @@
             _resolver_specs[schema_name].append(ResolverSpec(name, None, [MetricSpec(m) for m in anti_metrics], True))
 
         return func
 
     return decorator_register
 
 
+def unregister_udf(udf_name: str, namespace: Optional[str] = None, schema_name: str = "") -> None:
+    global _multicolumn_udfs, _resolver_specs
+    name = f"{namespace}.{udf_name}" if namespace else udf_name
+    if schema_name not in _multicolumn_udfs:
+        logger.warn(f"Can't unregister UDF {name} from non-existant schema {schema_name}")
+        return
+
+    found = False
+    for spec in _multicolumn_udfs[schema_name]:
+        if name in spec.udfs:
+            found = True
+            del spec.udfs[name]
+    if not found:
+        logger.warn(f"UDF {name} could not be found for unregistering")
+    _resolver_specs[schema_name] = list(filter(lambda x: x.column_name != name, _resolver_specs[schema_name]))
+
+
 def register_type_udf(
     col_type: Type,
     udf_name: Optional[str] = None,
     namespace: Optional[str] = None,
     schema_name: str = "",
     type_mapper: Optional[TypeMapper] = None,
 ) -> Callable[[Any], Any]:
@@ -289,15 +411,15 @@
 
 def generate_udf_specs(
     other_udf_specs: Optional[List[UdfSpec]] = None,
     schema_name: Union[str, List[str]] = "",
     include_default_schema: bool = True,
 ) -> List[UdfSpec]:
     """
-    Generates a list UdfSpecs that implement the UDFs specified by the
+    Generates a list of UdfSpecs that implement the UDFs specified by the
     @register_dataset_udf, @register_type_udf, and @register_metric_udf
     decorators. You can provide a list of other_udf_specs to include in
     addition to those UDFs registered via the decorator.
 
     For example:
 
     @register_dataset_udf(col_names=["col1"])
```

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/core/validators/condition_validator.py` & `whylogs-1.4.0rc0/whylogs/experimental/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/core/validators/validator.py` & `whylogs-1.4.0rc0/whylogs/experimental/core/validators/validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,27 @@
 from typing import Dict, List, Optional, Union
 
 from whylogs.core.validators import Validator
 
 _validator_udfs: Dict[str, List[Dict[str, List[Validator]]]] = defaultdict(list)
 
 
-def append_validator(schema_name: str, col_name: str, validator: Validator):
+def append_validator(schema_name, col_name: str, validator: Validator):
     global _validator_udfs
-    _validator_udfs[schema_name].append({col_name: [validator]})
+    validator_name = validator.name
+    exists = False
+    # if validator with same name and column exists, replace it
+    for col_validator in _validator_udfs.get(schema_name, []):
+        if col_name in col_validator:
+            for i, v in enumerate(col_validator[col_name]):
+                if v.name == validator_name:
+                    exists = True
+                    col_validator[col_name][i] = validator
+    if not exists:
+        _validator_udfs[schema_name].append({col_name: [validator]})
 
 
 def generate_validators(
     initial_validators: Optional[Dict[str, List[Validator]]],
     schema_name: Union[str, List[str]],
     include_default_schema: bool = True,
 ) -> Dict[str, List[Validator]]:
```

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.4.0rc0/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.4.0rc0/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.4.0rc0/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 from datetime import datetime
 from logging import getLogger
-from typing import Any, Optional
+from typing import Any, List, Optional, Tuple, Union
 
-from whylogs.api.writer import Writer, Writers
+from whylogs.api.writer import Writable
 
 logger = getLogger(__name__)
 
 
-class EstimationResult:
+class EstimationResult(Writable):
     """
     The result of a performance estimation.
     accuracy: The estimated accuracy.
     reference_partition_id: The partition id of the reference result set.
     reference_result_timestamp: The timestamp of the reference result set.
     """
 
     def __init__(
         self,
-        accuracy: Optional[float] = None,
+        accuracy: float,
         reference_partition_id: Optional[str] = None,
         reference_result_timestamp: Optional[datetime] = None,
         target_result_timestamp: Optional[datetime] = None,
     ):
         self.accuracy = accuracy
         self.reference_partition_id = reference_partition_id
         self.reference_result_timestamp = reference_result_timestamp
         self.target_result_timestamp = target_result_timestamp
 
-    def writer(self, name: str = "whylabs") -> "EstimationResultWriter":
-        if name != "whylabs":
-            raise ValueError("Only whylabs writer is currently supported")
-        writer = Writers.get(name)
-        return EstimationResultWriter(results=self, writer=writer)
+    def _get_default_filename(self) -> str:
+        raise ValueError("I'm not a real Writable")
 
+    def _get_default_path(self) -> str:
+        raise ValueError("I'm not a real Writable")
 
-class EstimationResultWriter:
-    def __init__(self, results: EstimationResult, writer: Writer):
-        self._estimation_result = results
-        self._writer = writer
-
-    def write(self, **kwargs: Any) -> None:
-        self._writer.write(file=self._estimation_result, **kwargs)
-        logger.debug("Completed writing estimation result!")
+    def write(self, path: Optional[str] = None, **kwargs: Any) -> Tuple[bool, Union[str, List[str]]]:
+        raise ValueError("I'm not a real Writable")
```

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.4.0rc0/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.4.0rc0/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/extras/image_metric.py` & `whylogs-1.4.0rc0/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/migration/converters.py` & `whylogs-1.4.0rc0/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/migration/uncompound.py` & `whylogs-1.4.0rc0/whylogs/migration/uncompound.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 from whylogs.core import ColumnProfileView, DatasetProfileView
 from whylogs.core.metrics import Metric
-from whylogs.core.metrics.column_metrics import ColumnCountsMetric
+from whylogs.core.metrics.column_metrics import ColumnCountsMetric, TypeCountersMetric
 from whylogs.core.metrics.compound_metric import CompoundMetric
 from whylogs.core.metrics.condition_count_metric import ConditionCountMetric
 from whylogs.core.metrics.metric_components import IntegralComponent
 from whylogs.core.metrics.multimetric import MultiMetric
 
 try:
     from PIL.Image import Image as ImageType  # noqa trigger ImportError if unavailable
@@ -114,39 +114,62 @@
 def _uncompound_condition_count(
     col_name: str, metric_name: str, metric: ConditionCountMetric, flags: Optional[FeatureFlags] = None
 ) -> Dict[str, ColumnProfileView]:
     if not _uncompound_condition_count_feature_flag(flags):
         return dict()
 
     result: Dict[str, ColumnProfileView] = dict()
+    type_metric = TypeCountersMetric(
+        integral=metric.total,  # total condition evaluations
+        fractional=IntegralComponent(0),
+        boolean=IntegralComponent(0),
+        string=IntegralComponent(0),
+        object=IntegralComponent(0),
+        tensor=IntegralComponent(0),
+    )
     for condition_name, count_component in metric.matches.items():
         new_col_name = f"{_condition_count_magic_string()}{col_name}.{condition_name}.total"
         new_metric = ColumnCountsMetric(
             n=metric.total,  # total condition evaluations
             null=IntegralComponent(0),  # unused
             nan=IntegralComponent(0),  # unused
             inf=IntegralComponent(0),  # unused
         )
-        result[new_col_name] = ColumnProfileView({ColumnCountsMetric.get_namespace(): new_metric})
+        result[new_col_name] = ColumnProfileView(
+            {
+                ColumnCountsMetric.get_namespace(): new_metric,
+                TypeCountersMetric.get_namespace(): type_metric,
+            }
+        )
         new_col_name = f"{_condition_count_magic_string()}{col_name}.{condition_name}.matches"
         new_metric = ColumnCountsMetric(
             n=count_component,  # count of evaluations that matched condition
             null=IntegralComponent(0),  # unused
             nan=IntegralComponent(0),  # unused
             inf=IntegralComponent(0),  # unused
         )
-        result[new_col_name] = ColumnProfileView({ColumnCountsMetric.get_namespace(): new_metric})
+        result[new_col_name] = ColumnProfileView(
+            {
+                ColumnCountsMetric.get_namespace(): new_metric,
+                TypeCountersMetric.get_namespace(): type_metric,
+            }
+        )
         new_col_name = f"{_condition_count_magic_string()}{col_name}.{condition_name}.non_matches"
         new_metric = ColumnCountsMetric(
             n=IntegralComponent(metric.total.value - count_component.value),  # evaluations that didn't match
             null=IntegralComponent(0),  # unused
             nan=IntegralComponent(0),  # unused
             inf=IntegralComponent(0),  # unused
         )
-        result[new_col_name] = ColumnProfileView({ColumnCountsMetric.get_namespace(): new_metric})
+        result[new_col_name] = ColumnProfileView(
+            {
+                ColumnCountsMetric.get_namespace(): new_metric,
+                TypeCountersMetric.get_namespace(): type_metric,
+            }
+        )
 
     return result
 
 
 def _uncompound_dataset_profile(prof: DatasetProfileView, flags: Optional[FeatureFlags] = None) -> DatasetProfileView:
     """
     v0 whylabs doesn't understand compound metrics. This creates a new column for
```

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.4.0rc0/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import numpy as np
 from scipy import stats  # type: ignore
 from scipy.spatial.distance import euclidean
 
 from whylogs.core.view.column_profile_view import ColumnProfileView  # type: ignore
 from whylogs.core.view.dataset_profile_view import DatasetProfileView  # type: ignore
+from whylogs.migration.uncompound import _uncompound_dataset_profile
 from whylogs.viz.drift.configs import (
     ChiSquareConfig,
     DriftThresholds,
     HellingerConfig,
     KSTestConfig,
 )
 from whylogs.viz.utils import _calculate_bins
@@ -356,14 +357,16 @@
             if D > D_max:
                 D_max = D
             j += 1
 
         m, n = sorted([target_distribution.get_n(), reference_distribution.get_n()], reverse=True)
         en = m * n / (m + n)
         p_value = stats.distributions.kstwo.sf(D_max, np.round(en))
+        if np.isnan(p_value) or p_value is None:
+            return None
         if with_thresholds:
             drift_category = self._get_drift_category(measure=p_value)
             drift_score = DriftAlgorithmScore(
                 algorithm=self.name,
                 pvalue=p_value,
                 statistic=D_max,
                 thresholds=self._parameter_config.thresholds,
@@ -479,16 +482,18 @@
 
         drift_map = {"legs": Hellinger(hellingerconfig), "weight": Hellinger(hellingerconfig)}
         drift_scores = calculate_drift_scores(
             target_view=target_view, reference_view=ref_view, drift_map=drift_map, with_thresholds=True
         )
     """
     drift_scores: Dict[str, Optional[Dict[str, Any]]] = {}
-    target_view_columns = target_view.get_columns()
-    reference_view_columns = reference_view.get_columns()
+    target_view_uncompounded = _uncompound_dataset_profile(target_view)
+    reference_view_uncompounded = _uncompound_dataset_profile(reference_view)
+    target_view_columns = target_view_uncompounded.get_columns()
+    reference_view_columns = reference_view_uncompounded.get_columns()
     if drift_map:
         for column_name in drift_map.keys():
             if column_name not in target_view_columns.keys():
                 warnings.warn(f"Column {column_name} not found in target profile.")
             if column_name not in reference_view_columns.keys():
                 warnings.warn(f"Column {column_name} not found in reference profile.")
```

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/drift/configs.py` & `whylogs-1.4.0rc0/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/enums/enums.py` & `whylogs-1.4.0rc0/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.4.0rc0/whylogs/viz/extensions/reports/html_report.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 import html
+import os
 from abc import ABC, abstractmethod
-from typing import Any, Optional
+from typing import Any, List, Optional, Tuple, Union
 
 from IPython.core.display import HTML  # type: ignore
 
 from whylogs import DatasetProfileView
-from whylogs.api.writer import Writers
-from whylogs.api.writer.writer import Writable, Writer
+from whylogs.api.writer.writer import Writable
 from whylogs.viz.enums.enums import PageSpec
 
 
 class HTMLReport(Writable, ABC):
     def __init__(
         self,
         ref_view: Optional[DatasetProfileView] = None,
         target_view: Optional[DatasetProfileView] = None,
         height: Optional[str] = None,
     ):
         self.ref_view = ref_view
         self.target_view = target_view
         self.height = height or None
 
-    def writer(self, name: str = "local") -> "HTMLReportWriter":
-        writer = Writers.get(name)
-        return HTMLReportWriter(report=self, writer=writer)
-
     def display(self, template: str, page_spec: PageSpec) -> HTML:
         if not self.height:
             self.height = page_spec.height
         iframe = f"""<div></div><iframe srcdoc="{html.escape(template)}" width=100% height={self.height}
         frameBorder=0></iframe>"""
         display = HTML(iframe)
         return display
 
     @abstractmethod
     def report(self) -> HTML:
         pass
 
-    def write(self, path: Optional[str] = None, **kwargs: Any) -> None:
+    def write(
+        self, path: Optional[str] = None, filename: Optional[str] = None, **kwargs: Any
+    ) -> Tuple[bool, Union[str, List[str]]]:
         """Create HTML file for a given report.
 
         Parameters
         ----------
         path: str, optional
             The path where the HTML reports will be stored to.
 
@@ -52,32 +50,21 @@
             from whylogs.viz import VizProfile, SummaryDriftReport
 
             report = SummaryDriftReport.report()
 
             viz_profile = VizProfile(report=report)
             viz_profile.write(path="path/to/report/Report.html")
         """
-        path = path or self.get_default_path()
+        path = path or self._get_default_path()
+        filename = filename or self._get_default_filename()
+        path = os.path.join(path, filename) if path else filename
         _html = self.report()
         _rendered_html = _html.data
         with self._safe_open_write(path) as file:
             file.write(_rendered_html)
+            return True, file.name
 
     def option(self):
         return self
 
-    def get_default_path(self) -> str:
-        path = "html_reports/ProfileReport.html"
-        return path
-
-
-class HTMLReportWriter(object):
-    def __init__(self, report: HTMLReport, writer: Writer) -> None:
-        self._report = report
-        self._writer = writer
-
-    def option(self, **kwargs) -> "HTMLReportWriter":
-        self._writer.option(**kwargs)
-        return self
-
-    def write(self, **kwargs: Any) -> None:
-        self._writer.write(file=self._report, **kwargs)
+    def _get_default_filename(self) -> str:
+        return "html_reports/ProfileReport.html"
```

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.4.0rc0/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.4.0rc0/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.4.0rc0/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.4.0rc0/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.4.0rc0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.4.0rc0/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.4.0rc0/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/js/d3.min.js` & `whylogs-1.4.0rc0/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/js/handlebars.js` & `whylogs-1.4.0rc0/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.4.0rc0/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.4.0rc0/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index.html` & `whylogs-1.4.0rc0/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.4.0rc0/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/html_template_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 
 
 def _get_compiled_template(template_name: str) -> "Callable":
     template_path = _get_template_path(template_name)
     try:
         from pybars import Compiler  # type: ignore
     except ImportError as e:
+        msg = "Unable to load pybars; install pybars3 to load profile directly from the current session or \
+        pip install whylogs[viz] to install dependencies for this module"
         logger.debug(e, exc_info=True)
-        logger.warning("Unable to load pybars; install pybars3 to load profile directly from the current session ")
-        return lambda _: None  # returns a no-op lambda
+        logger.error(msg)
+        raise ImportError(msg)
 
     with open(template_path, "rt") as file_with_template:
         source = file_with_template.read()
     return Compiler().compile(source)
 
 
 def get_compiled_template(template_name: str) -> "Callable":
```

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.4.0rc0/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9.dev0/PKG-INFO` & `whylogs-1.4.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylogs
-Version: 1.3.9.dev0
+Version: 1.4.0rc0
 Summary: Profile and monitor your ML data pipeline end-to-end
 Home-page: https://docs.whylabs.ai
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -58,15 +58,15 @@
 Requires-Dist: sphinx-autoapi ; extra == "docs"
 Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs"
 Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0) ; extra == "docs"
 Requires-Dist: sphinx-inline-tabs ; (python_version >= "3.8" and python_version < "4") and (extra == "docs")
 Requires-Dist: sphinxext-opengraph (>=0.6.3,<0.7.0) ; extra == "docs"
 Requires-Dist: types-requests (>=2.30.0.0,<3.0.0.0)
 Requires-Dist: typing-extensions (>=3.10) ; python_version < "4"
-Requires-Dist: whylabs-client (>=0.5.6,<0.6.0)
+Requires-Dist: whylabs-client (>=0.6.2,<0.7.0)
 Requires-Dist: whylogs-sketching (>=3.4.1.dev3)
 Description-Content-Type: text/markdown
 
 <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
 <img src="https://i.imgur.com/nv33goV.png" width="35%"/>
 </br>
```


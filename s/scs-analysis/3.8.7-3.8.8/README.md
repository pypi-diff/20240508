# Comparing `tmp/scs_analysis-3.8.7.tar.gz` & `tmp/scs_analysis-3.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs_analysis-3.8.7.tar", last modified: Wed May  1 09:51:06 2024, max compression
+gzip compressed data, was "scs_analysis-3.8.8.tar", last modified: Wed May  8 11:48:09 2024, max compression
```

## Comparing `scs_analysis-3.8.7.tar` & `scs_analysis-3.8.8.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.724794 scs_analysis-3.8.7/
--rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/LICENSE
--rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs_analysis-3.8.7/MANIFEST.in
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-05-01 09:51:06.724563 scs_analysis-3.8.7/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/README.md
--rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/README.rst
--rw-r--r--   0 bruno      (502) admin       (80)      237 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/requirements.txt
--rw-r--r--   0 bruno      (502) admin       (80)       38 2024-05-01 09:51:06.724838 scs_analysis-3.8.7/setup.cfg
--rwxr-xr-x   0 bruno      (502) admin       (80)     5581 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/setup.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.696774 scs_analysis-3.8.7/src/
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.711302 scs_analysis-3.8.7/src/scs_analysis/
--rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/__init__.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs_analysis-3.8.7/src/scs_analysis/alert.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs_analysis-3.8.7/src/scs_analysis/alert_status.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5981 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/aws_byline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs_analysis-3.8.7/src/scs_analysis/aws_client_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/aws_mqtt_client.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7103 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/aws_topic_history.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4140 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/aws_topic_origin.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/aws_topic_publisher.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/aws_upload_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    14779 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/baseline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs_analysis-3.8.7/src/scs_analysis/baseline_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.712662 scs_analysis-3.8.7/src/scs_analysis/chart/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/chart/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6609 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/client_traffic.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.722627 scs_analysis-3.8.7/src/scs_analysis/cmd/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_alert.py
--rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_alert_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-r--r--   0 bruno      (502) admin       (80)     3875 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_origin.py
--rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     4821 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_client_traffic.py
--rw-r--r--   0 bruno      (502) admin       (80)     4760 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_email.py
--rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-r--r--   0 bruno      (502) admin       (80)     4805 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     4539 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-r--r--   0 bruno      (502) admin       (80)     2373 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_report.py
--rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_join.py
--rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-r--r--   0 bruno      (502) admin       (80)     3984 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_controller.py
--rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_monitor_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3454 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_node.py
--rw-r--r--   0 bruno      (502) admin       (80)     5416 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     4679 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-r--r--   0 bruno      (502) admin       (80)     4657 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     6495 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     6209 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisations.py
--rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_error.py
--rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
--rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_gas_density.py
--rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_localize.py
--rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_median.py
--rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_record.py
--rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_single_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_uds.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5912 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6958 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_email.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_user_credentials.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8128 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_user_identity.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     9402 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/cognito_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7640 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/configuration_csv.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3591 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/configuration_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4000 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/configuration_monitor_check.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4110 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/configuration_report.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_collation_summary.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_join.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_reader.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/csv_segmentor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs_analysis-3.8.7/src/scs_analysis/csv_writer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7377 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/device_controller.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5405 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/device_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs_analysis-3.8.7/src/scs_analysis/device_monitor_status.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.723993 scs_analysis-3.8.7/src/scs_analysis/handler/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-r--r--   0 bruno      (502) admin       (80)     2360 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/handler/batch_download_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/configuration_csv_generator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5567 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/handler/csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5903 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/handler/csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/mqtt_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/sample_midpoint.py
--rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/handler/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/histo_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2175 2024-04-30 09:02:59.000000 scs_analysis-3.8.7/src/scs_analysis/localised_datetime.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/monitor_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/multi_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs_analysis-3.8.7/src/scs_analysis/node.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6552 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisation_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5855 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisation_path_roots.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5563 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisation_user_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6565 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisation_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8124 2024-05-01 09:50:59.000000 scs_analysis-3.8.7/src/scs_analysis/organisations.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs_analysis-3.8.7/src/scs_analysis/sample_aggregate.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_average.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_distance.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_duplicates.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_error.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_gas_concentration.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3522 2024-04-14 07:50:13.000000 scs_analysis-3.8.7/src/scs_analysis/sample_gas_density.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/sample_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs_analysis-3.8.7/src/scs_analysis/sample_iso_8601.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_localize.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_low_pass.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_max.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_median.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_midpoint.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_min.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/sample_noise.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_nullify.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/sample_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs_analysis-3.8.7/src/scs_analysis/sample_slope.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_sort.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_stats.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs_analysis-3.8.7/src/scs_analysis/sample_subset.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/sample_time_shift.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs_analysis-3.8.7/src/scs_analysis/socket_receiver.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs_analysis-3.8.7/src/scs_analysis/timer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs_analysis-3.8.7/src/scs_analysis/uds_receiver.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-01 09:51:06.724214 scs_analysis-3.8.7/src/scs_analysis.egg-info/
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)     6234 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (502) admin       (80)        1 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (502) admin       (80)      252 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/requires.txt
--rw-r--r--   0 bruno      (502) admin       (80)       13 2024-05-01 09:51:06.000000 scs_analysis-3.8.7/src/scs_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-08 11:48:09.487435 scs_analysis-3.8.8/
+-rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/LICENSE
+-rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs_analysis-3.8.8/MANIFEST.in
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-05-08 11:48:09.487215 scs_analysis-3.8.8/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/README.md
+-rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/README.rst
+-rw-r--r--   0 bruno      (502) admin       (80)      237 2024-05-08 11:48:01.000000 scs_analysis-3.8.8/requirements.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       38 2024-05-08 11:48:09.487477 scs_analysis-3.8.8/setup.cfg
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5581 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/setup.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-08 11:48:09.459565 scs_analysis-3.8.8/src/
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-08 11:48:09.473671 scs_analysis-3.8.8/src/scs_analysis/
+-rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-05-08 11:48:01.000000 scs_analysis-3.8.8/src/scs_analysis/__init__.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs_analysis-3.8.8/src/scs_analysis/alert.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs_analysis-3.8.8/src/scs_analysis/alert_status.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5981 2024-04-14 07:50:13.000000 scs_analysis-3.8.8/src/scs_analysis/aws_byline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs_analysis-3.8.8/src/scs_analysis/aws_client_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/aws_mqtt_client.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7103 2024-04-14 07:50:13.000000 scs_analysis-3.8.8/src/scs_analysis/aws_topic_history.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4140 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/aws_topic_origin.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/aws_topic_publisher.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/aws_upload_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    14779 2024-04-14 07:50:13.000000 scs_analysis-3.8.8/src/scs_analysis/baseline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs_analysis-3.8.8/src/scs_analysis/baseline_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-08 11:48:09.475254 scs_analysis-3.8.8/src/scs_analysis/chart/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/chart/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/chart/chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/chart/histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/chart/multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/chart/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6578 2024-05-08 11:48:01.000000 scs_analysis-3.8.8/src/scs_analysis/client_traffic.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-08 11:48:09.485156 scs_analysis-3.8.8/src/scs_analysis/cmd/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_alert.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3875 2024-04-14 07:50:13.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_topic_origin.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4824 2024-05-08 11:48:01.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_client_traffic.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4760 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_email.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4805 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4539 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2373 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_configuration_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3984 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_device_controller.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_device_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_device_monitor_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3454 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_node.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5416 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4679 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4657 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6495 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6209 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisations.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_gas_density.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_localize.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_uds.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5912 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/cognito_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6958 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/cognito_email.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs_analysis-3.8.8/src/scs_analysis/cognito_user_credentials.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8225 2024-05-08 11:48:01.000000 scs_analysis-3.8.8/src/scs_analysis/cognito_user_identity.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     9402 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/cognito_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7640 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/configuration_csv.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3591 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/configuration_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4000 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/configuration_monitor_check.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4110 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/configuration_report.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/csv_collation_summary.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/csv_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/csv_join.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/csv_reader.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/csv_segmentor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs_analysis-3.8.8/src/scs_analysis/csv_writer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7377 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/device_controller.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5405 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/device_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs_analysis-3.8.8/src/scs_analysis/device_monitor_status.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-08 11:48:09.486643 scs_analysis-3.8.8/src/scs_analysis/handler/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/handler/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2360 2024-04-14 07:50:13.000000 scs_analysis-3.8.8/src/scs_analysis/handler/batch_download_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5567 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/handler/csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5903 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/handler/csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/handler/mqtt_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/handler/sample_midpoint.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/handler/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/histo_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2175 2024-04-30 09:02:59.000000 scs_analysis-3.8.8/src/scs_analysis/localised_datetime.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/monitor_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/multi_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs_analysis-3.8.8/src/scs_analysis/node.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6552 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/organisation_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5855 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/organisation_path_roots.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5563 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/organisation_user_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6565 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/organisation_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8124 2024-05-01 09:50:59.000000 scs_analysis-3.8.8/src/scs_analysis/organisations.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs_analysis-3.8.8/src/scs_analysis/sample_aggregate.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_average.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_distance.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_duplicates.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_error.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_gas_concentration.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3522 2024-04-14 07:50:13.000000 scs_analysis-3.8.8/src/scs_analysis/sample_gas_density.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/sample_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs_analysis-3.8.8/src/scs_analysis/sample_iso_8601.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_localize.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_low_pass.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_max.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_median.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_midpoint.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_min.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/sample_noise.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_nullify.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/sample_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs_analysis-3.8.8/src/scs_analysis/sample_slope.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_sort.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_stats.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs_analysis-3.8.8/src/scs_analysis/sample_subset.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/sample_time_shift.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs_analysis-3.8.8/src/scs_analysis/socket_receiver.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs_analysis-3.8.8/src/scs_analysis/timer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs_analysis-3.8.8/src/scs_analysis/uds_receiver.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-05-08 11:48:09.486857 scs_analysis-3.8.8/src/scs_analysis.egg-info/
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-05-08 11:48:09.000000 scs_analysis-3.8.8/src/scs_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)     6234 2024-05-08 11:48:09.000000 scs_analysis-3.8.8/src/scs_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        1 2024-05-08 11:48:09.000000 scs_analysis-3.8.8/src/scs_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (502) admin       (80)      252 2024-05-08 11:48:09.000000 scs_analysis-3.8.8/src/scs_analysis.egg-info/requires.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       13 2024-05-08 11:48:09.000000 scs_analysis-3.8.8/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs_analysis-3.8.7/LICENSE` & `scs_analysis-3.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/PKG-INFO` & `scs_analysis-3.8.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.8.7
+Version: 3.8.8
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,15 @@
 Requires-Dist: pypandoc~=1.5
 Requires-Dist: pysftp~=0.2.9
 Requires-Dist: pytz~=2020.1
 Requires-Dist: requests~=2.28.2
 Requires-Dist: scipy~=1.5
 Requires-Dist: setuptools~=50.3.0
 Requires-Dist: tzlocal~=2.1
-Requires-Dist: scs-core~=3.13.4
+Requires-Dist: scs-core~=3.14.0
 Requires-Dist: scs-host-posix~=3.3.1
 Provides-Extra: dev
 Requires-Dist: pypandoc; extra == "dev"
 
 # scs_analysis
 _Information management and analysis utilities for South Coast Science data consumers_
```

### Comparing `scs_analysis-3.8.7/README.md` & `scs_analysis-3.8.8/README.md`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/setup.py` & `scs_analysis-3.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/alert.py` & `scs_analysis-3.8.8/src/scs_analysis/alert.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/alert_status.py` & `scs_analysis-3.8.8/src/scs_analysis/alert_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/aws_byline.py` & `scs_analysis-3.8.8/src/scs_analysis/aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/aws_client_auth.py` & `scs_analysis-3.8.8/src/scs_analysis/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/aws_mqtt_client.py` & `scs_analysis-3.8.8/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/aws_topic_history.py` & `scs_analysis-3.8.8/src/scs_analysis/aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/aws_topic_origin.py` & `scs_analysis-3.8.8/src/scs_analysis/aws_topic_origin.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/aws_topic_publisher.py` & `scs_analysis-3.8.8/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/aws_upload_interval.py` & `scs_analysis-3.8.8/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/baseline.py` & `scs_analysis-3.8.8/src/scs_analysis/baseline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/baseline_conf.py` & `scs_analysis-3.8.8/src/scs_analysis/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/chart/chart.py` & `scs_analysis-3.8.8/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/chart/histo_chart.py` & `scs_analysis-3.8.8/src/scs_analysis/chart/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/chart/multi_chart.py` & `scs_analysis-3.8.8/src/scs_analysis/chart/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/chart/single_chart.py` & `scs_analysis-3.8.8/src/scs_analysis/chart/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/client_traffic.py` & `scs_analysis-3.8.8/src/scs_analysis/client_traffic.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 * --aggregate - (only relevant when specifying a year or month period) statistics are aggregated to totals for the
 period
 
 Statistics are available only for the clients(s) that are visible to the user. Only organisation admins may view
 statistics for whole organisations. Only superusers can view the statistics for all users.
 
 SYNOPSIS
-client_traffic.py [-c CREDENTIALS] -e ENDPOINT { -u | -o [-s] } -p PERIOD [-a] [-i INDENT] [-v]  [CLIENT_1..CLIENT_N]
+Usage: client_traffic.py [-c CREDENTIALS] -e ENDPOINT [{ -u | -o [-s] }] -p PERIOD [-a] [-i INDENT] [-v]
+[CLIENT_1...CLIENT_N]
 
 EXAMPLES
 client_traffic.py -c super -e test1 -o Ricardo -p 2023-08-22
 
 client_traffic.py -v -c super -e TopicHistory -p 2024 -u production@southcoastscience.com | node.py -s | \
 csv_writer.py -v traffic.csv
 
@@ -153,17 +154,14 @@
 
                 if organisation is None:
                     logger.error("the organisation '%s' could not be found." % client)
                     exit(2)
 
                 clients.append(organisation.label)
 
-        else:
-            clients = []
-
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         request = ClientTrafficRequest(cmd.endpoint, clients, cmd.period, cmd.aggregate)
 
         if cmd.organisation:
```

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_alert.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_alert_status.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_origin.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_topic_origin.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_baseline.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_client_traffic.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_client_traffic.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     # --------------------------------------------------------------------------------------------------------------------
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] -e ENDPOINT "
-                                                    "{ -u | -o [-s] } -p PERIOD [-a] "
-                                                    "[-i INDENT] [-v] [CLIENT_1..CLIENT_N]", version=version())
+                                                    "[{ -u | -o [-s] }] -p PERIOD [-a] "
+                                                    "[-i INDENT] [-v] [CLIENT_1...CLIENT_N]", version=version())
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # filters...
         self.__parser.add_option("--endpoint", "-e", type="string", action="store", dest="endpoint",
```

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_email.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_email.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_configuration_report.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_configuration_report.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_join.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_controller.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_device_controller.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_monitor.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_device_monitor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_device_monitor_status.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_node.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_organisations.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_error.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_gas_concentration.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_gas_density.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_gas_density.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_localize.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_median.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_record.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_sort.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_single_chart.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_socket_receiver.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cmd/cmd_uds.py` & `scs_analysis-3.8.8/src/scs_analysis/cmd/cmd_uds.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cognito_devices.py` & `scs_analysis-3.8.8/src/scs_analysis/cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cognito_email.py` & `scs_analysis-3.8.8/src/scs_analysis/cognito_email.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cognito_user_credentials.py` & `scs_analysis-3.8.8/src/scs_analysis/cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cognito_user_identity.py` & `scs_analysis-3.8.8/src/scs_analysis/cognito_user_identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 Created on 24 Nov 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The cognito_user_identity utility is used to create, update and retrieve a AWS Cognito identity for the user.
+The cognito_user_identity utility is used to create, read or update an AWS Cognito identity for the user.
+
+Note that the chosen password must include lower and upper case, numeric and punctuation characters
 
 If the --Create function is used, an email is sent to the new user. The verification link in the email must be
 exercised in order for the account to gain a CONFIRMED status.
 
 SYNOPSIS
 cognito_user_identity.py [-c CREDENTIALS] | -C | -R | -U } [-i INDENT] [-v]
```

### Comparing `scs_analysis-3.8.7/src/scs_analysis/cognito_users.py` & `scs_analysis-3.8.8/src/scs_analysis/cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/configuration_csv.py` & `scs_analysis-3.8.8/src/scs_analysis/configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/configuration_monitor.py` & `scs_analysis-3.8.8/src/scs_analysis/configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/configuration_monitor_check.py` & `scs_analysis-3.8.8/src/scs_analysis/configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/configuration_report.py` & `scs_analysis-3.8.8/src/scs_analysis/configuration_report.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/csv_collation_summary.py` & `scs_analysis-3.8.8/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/csv_collator.py` & `scs_analysis-3.8.8/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/csv_join.py` & `scs_analysis-3.8.8/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/csv_reader.py` & `scs_analysis-3.8.8/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/csv_segmentor.py` & `scs_analysis-3.8.8/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/csv_writer.py` & `scs_analysis-3.8.8/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/device_controller.py` & `scs_analysis-3.8.8/src/scs_analysis/device_controller.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/device_monitor.py` & `scs_analysis-3.8.8/src/scs_analysis/device_monitor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/device_monitor_status.py` & `scs_analysis-3.8.8/src/scs_analysis/device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs_analysis-3.8.8/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs_analysis-3.8.8/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/handler/batch_download_reporter.py` & `scs_analysis-3.8.8/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/handler/configuration_csv_generator.py` & `scs_analysis-3.8.8/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/handler/csv_collator.py` & `scs_analysis-3.8.8/src/scs_analysis/handler/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/handler/csv_segmentor.py` & `scs_analysis-3.8.8/src/scs_analysis/handler/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/handler/mqtt_reporter.py` & `scs_analysis-3.8.8/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/handler/sample_midpoint.py` & `scs_analysis-3.8.8/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/handler/sample_regression.py` & `scs_analysis-3.8.8/src/scs_analysis/handler/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/histo_chart.py` & `scs_analysis-3.8.8/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/localised_datetime.py` & `scs_analysis-3.8.8/src/scs_analysis/localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/monitor_auth.py` & `scs_analysis-3.8.8/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/multi_chart.py` & `scs_analysis-3.8.8/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/node.py` & `scs_analysis-3.8.8/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/organisation_devices.py` & `scs_analysis-3.8.8/src/scs_analysis/organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/organisation_path_roots.py` & `scs_analysis-3.8.8/src/scs_analysis/organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/organisation_user_paths.py` & `scs_analysis-3.8.8/src/scs_analysis/organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/organisation_users.py` & `scs_analysis-3.8.8/src/scs_analysis/organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/organisations.py` & `scs_analysis-3.8.8/src/scs_analysis/organisations.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_aggregate.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_average.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_average.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_collator.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_distance.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_duplicates.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_error.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_gas_concentration.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_gas_density.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_gas_density.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_interval.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_iso_8601.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_localize.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_low_pass.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_max.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_max.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_median.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_median.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_midpoint.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_min.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_min.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_noise.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_nullify.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_paths.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_regression.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_slope.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_sort.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_stats.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_subset.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/sample_time_shift.py` & `scs_analysis-3.8.8/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/single_chart.py` & `scs_analysis-3.8.8/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/socket_receiver.py` & `scs_analysis-3.8.8/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/timer.py` & `scs_analysis-3.8.8/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis/uds_receiver.py` & `scs_analysis-3.8.8/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs_analysis-3.8.7/src/scs_analysis.egg-info/PKG-INFO` & `scs_analysis-3.8.8/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.8.7
+Version: 3.8.8
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,15 @@
 Requires-Dist: pypandoc~=1.5
 Requires-Dist: pysftp~=0.2.9
 Requires-Dist: pytz~=2020.1
 Requires-Dist: requests~=2.28.2
 Requires-Dist: scipy~=1.5
 Requires-Dist: setuptools~=50.3.0
 Requires-Dist: tzlocal~=2.1
-Requires-Dist: scs-core~=3.13.4
+Requires-Dist: scs-core~=3.14.0
 Requires-Dist: scs-host-posix~=3.3.1
 Provides-Extra: dev
 Requires-Dist: pypandoc; extra == "dev"
 
 # scs_analysis
 _Information management and analysis utilities for South Coast Science data consumers_
```

### Comparing `scs_analysis-3.8.7/src/scs_analysis.egg-info/SOURCES.txt` & `scs_analysis-3.8.8/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/data-repo-client-2.61.0.tar.gz` & `tmp/data-repo-client-2.62.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-lphcny5i/data-repo-client-2.61.0.tar", last modified: Tue May  7 17:53:49 2024, max compression
+gzip compressed data, was "/home/runner/work/jade-data-repo/jade-data-repo/data-repo-client/dist/.tmp-fs7tqq0i/data-repo-client-2.62.0.tar", last modified: Wed May  8 18:17:17 2024, max compression
```

## Comparing `data-repo-client-2.61.0.tar` & `data-repo-client-2.62.0.tar`

### file list

```diff
@@ -1,388 +1,388 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    43829 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/data_repo_client/
--rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/data_repo_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/api/admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/api/configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/api/data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   250526 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   470717 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/api/snapshot_access_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   163156 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api/upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/data_repo_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    15870 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/data_repo_client/models/enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_get_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/data_repo_client/models/workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/data_repo_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/data_repo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/data_repo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/data_repo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/data_repo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/data_repo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/data_repo_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:53:49.000000 data-repo-client-2.61.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_access_info_big_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_access_info_big_query_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_access_info_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_access_info_parquet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_access_info_parquet_model_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_add_auth_domain_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_asset_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_billing_profile_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_billing_profile_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_bulk_load_array_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_bulk_load_array_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_bulk_load_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_bulk_load_file_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_bulk_load_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_bulk_load_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_bulk_load_history_model_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_bulk_load_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_bulk_load_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_cloud_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_column_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_column_statistics_double_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_column_statistics_double_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_column_statistics_int_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_column_statistics_int_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_column_statistics_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_column_statistics_text_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_column_statistics_text_model_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_column_statistics_text_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_config_enable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_config_fault_counted_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_config_fault_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_config_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_config_list_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_config_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_config_parameter_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_data_deletion_gcs_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_data_deletion_json_array_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_data_deletion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_data_deletion_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_data_repository_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_request_access_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_schema_column_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_schema_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_schema_update_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_specification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_dataset_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_date_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_delete_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_directory_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_access_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_access_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_alias_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_contents_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_passport_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_drs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_duos_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_duos_firecloud_group_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_duos_firecloud_groups_sync_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_enumerate_billing_profile_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_enumerate_dataset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-07 17:53:43.000000 data-repo-client-2.61.0/test/test_enumerate_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_enumerate_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_enumerate_sort_by_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_file_detail_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_file_load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_file_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_iam_resource_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_inaccessible_workspace_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_ingest_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_ingest_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_int_partition_options_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_journal_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_journal_entry_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_policy_member_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_policy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_profiles_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_query_column_statistics_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_query_data_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_register_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_relationship_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_relationship_term_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_repository_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_repository_configuration_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_repository_status_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_repository_status_model_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_resource_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_resource_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_sam_policy_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_access_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_access_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_access_request_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_count_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_count_response_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_criteria_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_dataset_concept_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_domain_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_domain_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_domain_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_domain_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_feature_value_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_get_concepts_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_parent_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_range_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_range_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_program_data_range_option_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_builder_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_export_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_export_response_model_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_export_response_model_format_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_export_response_model_format_parquet_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_export_response_model_format_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_ids_and_roles_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_link_duos_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_patch_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_preview_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_request_asset_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_request_contents_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_request_model_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_request_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_request_row_id_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_request_row_id_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_retrieve_include_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_snapshot_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_snapshots_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_sql_sort_direction_asc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_sql_sort_direction_desc_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_storage_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_table_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_table_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_tag_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_tag_count_result_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_tag_update_request_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_transaction_close_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_transaction_create_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_transaction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_unauthenticated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_unlock_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-07 17:53:45.000000 data-repo-client-2.61.0/test/test_upgrade_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_upgrade_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_upgrade_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_user_status_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-07 17:53:44.000000 data-repo-client-2.61.0/test/test_workspace_policy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    43869 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41290 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   225812 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22542 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17614 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47273 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   470937 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47274 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31737 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/api/snapshot_access_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188090 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api/upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27140 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8937 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8092 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/data_repo_client/models/config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9156 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12863 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12433 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16039 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/data_repo_client/models/workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/data_repo_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/data_repo_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:17:17.000000 data-repo-client-2.62.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_big_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_big_query_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_parquet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_access_info_parquet_model_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_add_auth_domain_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_asset_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_billing_profile_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_billing_profile_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_array_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_array_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_file_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_history_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_bulk_load_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_cloud_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_double_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_double_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_int_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_int_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_text_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_text_model_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_column_statistics_text_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_config_enable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_config_fault_counted_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 18:17:10.000000 data-repo-client-2.62.0/test/test_config_fault_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_config_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_config_list_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_config_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_config_parameter_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_deletion_gcs_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_deletion_json_array_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_deletion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_deletion_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_data_repository_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_request_access_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_schema_column_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_schema_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_schema_update_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_specification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_dataset_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_date_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_delete_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_directory_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_access_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_access_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_alias_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_contents_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_passport_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_drs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_duos_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_duos_firecloud_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_duos_firecloud_groups_sync_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_billing_profile_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_dataset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_enumerate_sort_by_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_file_detail_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_file_load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_file_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_iam_resource_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_inaccessible_workspace_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_ingest_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_ingest_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_int_partition_options_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_journal_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_journal_entry_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_policy_member_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_policy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_profiles_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_query_column_statistics_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_query_data_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_register_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_relationship_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_relationship_term_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_repository_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_repository_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_repository_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_repository_status_model_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_resource_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_resource_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_sam_policy_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_access_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_access_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_access_request_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_concepts_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_count_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_count_response_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_criteria_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_dataset_concept_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_domain_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_domain_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_domain_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_domain_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_feature_value_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_get_concept_hierarchy_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_parent_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_option_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_builder_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_ids_and_roles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_link_duos_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_patch_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_preview_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_asset_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_contents_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_model_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_row_id_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_request_row_id_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_retrieve_include_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_snapshot_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_snapshots_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_sql_sort_direction_asc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_sql_sort_direction_desc_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_storage_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_table_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_tag_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_tag_count_result_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_tag_update_request_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_transaction_close_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_transaction_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_transaction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_unauthenticated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_unlock_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-08 18:17:12.000000 data-repo-client-2.62.0/test/test_upgrade_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_upgrade_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_upgrade_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_user_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-08 18:17:11.000000 data-repo-client-2.62.0/test/test_workspace_policy_model.py
```

### Comparing `data-repo-client-2.61.0/PKG-INFO` & `data-repo-client-2.62.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.61.0
+Version: 2.62.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.61.0/README.md` & `data-repo-client-2.62.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 The API endpoints are organized by interface. Each interface is separately versioned. <p> **Notes on Naming** <p> All of the reference items are suffixed with \\\"Model\\\". Those names are used as the class names in the generated Java code. It is helpful to distinguish these model classes from other related classes, like the DAO classes and the operation classes. </details>
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 2.61.0
+- Package version: 2.62.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -126,19 +126,16 @@
 *DatasetsApi* | [**close_transaction**](docs/DatasetsApi.md#close_transaction) | **POST** /api/repository/v1/datasets/{id}/transactions/{transactionId} | 
 *DatasetsApi* | [**create_dataset**](docs/DatasetsApi.md#create_dataset) | **POST** /api/repository/v1/datasets | 
 *DatasetsApi* | [**delete_dataset**](docs/DatasetsApi.md#delete_dataset) | **DELETE** /api/repository/v1/datasets/{id} | 
 *DatasetsApi* | [**delete_dataset_policy_member**](docs/DatasetsApi.md#delete_dataset_policy_member) | **DELETE** /api/repository/v1/datasets/{id}/policies/{policyName}/members/{memberEmail} | 
 *DatasetsApi* | [**delete_file**](docs/DatasetsApi.md#delete_file) | **DELETE** /api/repository/v1/datasets/{id}/files/{fileid} | 
 *DatasetsApi* | [**enumerate_datasets**](docs/DatasetsApi.md#enumerate_datasets) | **GET** /api/repository/v1/datasets | 
 *DatasetsApi* | [**enumerate_transactions**](docs/DatasetsApi.md#enumerate_transactions) | **GET** /api/repository/v1/datasets/{id}/transactions | 
-*DatasetsApi* | [**get_concept_hierarchy**](docs/DatasetsApi.md#get_concept_hierarchy) | **GET** /api/repository/v1/datasets/{id}/snapshotBuilder/conceptHierarchy/{conceptId} | 
-*DatasetsApi* | [**get_concepts**](docs/DatasetsApi.md#get_concepts) | **GET** /api/repository/v1/datasets/{id}/snapshotBuilder/concepts/{conceptId} | 
 *DatasetsApi* | [**get_dataset_tags**](docs/DatasetsApi.md#get_dataset_tags) | **GET** /api/repository/v1/datasets/tags | 
 *DatasetsApi* | [**get_load_history_for_load_tag**](docs/DatasetsApi.md#get_load_history_for_load_tag) | **GET** /api/repository/v1/datasets/{id}/files/bulk/{loadTag} | 
-*DatasetsApi* | [**get_snapshot_builder_count**](docs/DatasetsApi.md#get_snapshot_builder_count) | **POST** /api/repository/v1/datasets/{id}/snapshotBuilder/count | 
 *DatasetsApi* | [**ingest_dataset**](docs/DatasetsApi.md#ingest_dataset) | **POST** /api/repository/v1/datasets/{id}/ingest | 
 *DatasetsApi* | [**ingest_file**](docs/DatasetsApi.md#ingest_file) | **POST** /api/repository/v1/datasets/{id}/files | 
 *DatasetsApi* | [**list_files**](docs/DatasetsApi.md#list_files) | **GET** /api/repository/v1/datasets/{id}/files | 
 *DatasetsApi* | [**lock_dataset**](docs/DatasetsApi.md#lock_dataset) | **PUT** /api/repository/v1/datasets/{id}/lock | 
 *DatasetsApi* | [**lookup_dataset_column_statistics_by_id**](docs/DatasetsApi.md#lookup_dataset_column_statistics_by_id) | **GET** /api/repository/v1/datasets/{id}/data/{table}/statistics/{column} | 
 *DatasetsApi* | [**lookup_dataset_data_by_id**](docs/DatasetsApi.md#lookup_dataset_data_by_id) | **GET** /api/repository/v1/datasets/{id}/data/{table} | 
 *DatasetsApi* | [**lookup_file_by_id**](docs/DatasetsApi.md#lookup_file_by_id) | **GET** /api/repository/v1/datasets/{id}/files/{fileid} | 
@@ -149,15 +146,14 @@
 *DatasetsApi* | [**query_dataset_data_by_id**](docs/DatasetsApi.md#query_dataset_data_by_id) | **POST** /api/repository/v1/datasets/{id}/data/{table} | 
 *DatasetsApi* | [**remove_dataset_asset_specifications**](docs/DatasetsApi.md#remove_dataset_asset_specifications) | **DELETE** /api/repository/v1/datasets/{id}/assets/{assetid} | 
 *DatasetsApi* | [**retrieve_dataset**](docs/DatasetsApi.md#retrieve_dataset) | **GET** /api/repository/v1/datasets/{id} | 
 *DatasetsApi* | [**retrieve_dataset_policies**](docs/DatasetsApi.md#retrieve_dataset_policies) | **GET** /api/repository/v1/datasets/{id}/policies | 
 *DatasetsApi* | [**retrieve_dataset_summary**](docs/DatasetsApi.md#retrieve_dataset_summary) | **GET** /api/repository/v1/datasets/{id}/summary | 
 *DatasetsApi* | [**retrieve_transaction**](docs/DatasetsApi.md#retrieve_transaction) | **GET** /api/repository/v1/datasets/{id}/transactions/{transactionId} | 
 *DatasetsApi* | [**retrieve_user_dataset_roles**](docs/DatasetsApi.md#retrieve_user_dataset_roles) | **GET** /api/repository/v1/datasets/{id}/roles | 
-*DatasetsApi* | [**search_concepts**](docs/DatasetsApi.md#search_concepts) | **GET** /api/repository/v1/datasets/{id}/snapshotBuilder/concepts/{domainId}/search | 
 *DatasetsApi* | [**unlock_dataset**](docs/DatasetsApi.md#unlock_dataset) | **PUT** /api/repository/v1/datasets/{id}/unlock | 
 *DatasetsApi* | [**update_dataset_snapshot_builder_settings**](docs/DatasetsApi.md#update_dataset_snapshot_builder_settings) | **POST** /api/repository/v1/datasets/{id}/snapshotBuilder/settings | 
 *DatasetsApi* | [**update_dataset_tags**](docs/DatasetsApi.md#update_dataset_tags) | **PATCH** /api/repository/v1/datasets/{id}/tags | 
 *DatasetsApi* | [**update_schema**](docs/DatasetsApi.md#update_schema) | **POST** /api/repository/v1/datasets/{id}/updateSchema | 
 *DuosApi* | [**retrieve_duos_firecloud_group**](docs/DuosApi.md#retrieve_duos_firecloud_group) | **GET** /api/repository/v1/duos/{duosId} | 
 *DuosApi* | [**retrieve_duos_firecloud_groups**](docs/DuosApi.md#retrieve_duos_firecloud_groups) | **GET** /api/repository/v1/duos | 
 *DuosApi* | [**sync_duos_dataset_authorized_users**](docs/DuosApi.md#sync_duos_dataset_authorized_users) | **PUT** /api/repository/v1/duos/{duosId}/syncAuthorizedUsers | 
@@ -188,26 +184,27 @@
 *RepositoryApi* | [**create_snapshot**](docs/RepositoryApi.md#create_snapshot) | **POST** /api/repository/v1/snapshots | 
 *RepositoryApi* | [**delete_dataset**](docs/RepositoryApi.md#delete_dataset) | **DELETE** /api/repository/v1/datasets/{id} | 
 *RepositoryApi* | [**delete_dataset_policy_member**](docs/RepositoryApi.md#delete_dataset_policy_member) | **DELETE** /api/repository/v1/datasets/{id}/policies/{policyName}/members/{memberEmail} | 
 *RepositoryApi* | [**delete_file**](docs/RepositoryApi.md#delete_file) | **DELETE** /api/repository/v1/datasets/{id}/files/{fileid} | 
 *RepositoryApi* | [**delete_snapshot**](docs/RepositoryApi.md#delete_snapshot) | **DELETE** /api/repository/v1/snapshots/{id} | 
 *RepositoryApi* | [**delete_snapshot_policy_member**](docs/RepositoryApi.md#delete_snapshot_policy_member) | **DELETE** /api/repository/v1/snapshots/{id}/policies/{policyName}/members/{memberEmail} | 
 *RepositoryApi* | [**delete_snapshot_snapshot_builder_settings**](docs/RepositoryApi.md#delete_snapshot_snapshot_builder_settings) | **DELETE** /api/repository/v1/snapshots/{id}/snapshotBuilder/settings | 
+*RepositoryApi* | [**enumerate_concepts**](docs/RepositoryApi.md#enumerate_concepts) | **GET** /api/repository/v1/snapshots/{id}/snapshotBuilder/concepts | 
 *RepositoryApi* | [**enumerate_datasets**](docs/RepositoryApi.md#enumerate_datasets) | **GET** /api/repository/v1/datasets | 
 *RepositoryApi* | [**enumerate_jobs**](docs/RepositoryApi.md#enumerate_jobs) | **GET** /api/repository/v1/jobs | 
 *RepositoryApi* | [**enumerate_snapshots**](docs/RepositoryApi.md#enumerate_snapshots) | **GET** /api/repository/v1/snapshots | 
 *RepositoryApi* | [**enumerate_transactions**](docs/RepositoryApi.md#enumerate_transactions) | **GET** /api/repository/v1/datasets/{id}/transactions | 
 *RepositoryApi* | [**export_snapshot**](docs/RepositoryApi.md#export_snapshot) | **GET** /api/repository/v1/snapshots/{id}/export | 
-*RepositoryApi* | [**get_concept_hierarchy**](docs/RepositoryApi.md#get_concept_hierarchy) | **GET** /api/repository/v1/datasets/{id}/snapshotBuilder/conceptHierarchy/{conceptId} | 
-*RepositoryApi* | [**get_concepts**](docs/RepositoryApi.md#get_concepts) | **GET** /api/repository/v1/datasets/{id}/snapshotBuilder/concepts/{conceptId} | 
+*RepositoryApi* | [**get_concept_children**](docs/RepositoryApi.md#get_concept_children) | **GET** /api/repository/v1/snapshots/{id}/snapshotBuilder/concepts/{conceptId}/children | 
+*RepositoryApi* | [**get_concept_hierarchy**](docs/RepositoryApi.md#get_concept_hierarchy) | **GET** /api/repository/v1/snapshots/{id}/snapshotBuilder/concepts/{conceptId}/hierarchy | 
 *RepositoryApi* | [**get_config**](docs/RepositoryApi.md#get_config) | **GET** /api/repository/v1/configs/{name} | 
 *RepositoryApi* | [**get_config_list**](docs/RepositoryApi.md#get_config_list) | **GET** /api/repository/v1/configs | 
 *RepositoryApi* | [**get_dataset_tags**](docs/RepositoryApi.md#get_dataset_tags) | **GET** /api/repository/v1/datasets/tags | 
 *RepositoryApi* | [**get_load_history_for_load_tag**](docs/RepositoryApi.md#get_load_history_for_load_tag) | **GET** /api/repository/v1/datasets/{id}/files/bulk/{loadTag} | 
-*RepositoryApi* | [**get_snapshot_builder_count**](docs/RepositoryApi.md#get_snapshot_builder_count) | **POST** /api/repository/v1/datasets/{id}/snapshotBuilder/count | 
+*RepositoryApi* | [**get_snapshot_builder_count**](docs/RepositoryApi.md#get_snapshot_builder_count) | **POST** /api/repository/v1/snapshots/{id}/snapshotBuilder/count | 
 *RepositoryApi* | [**get_snapshot_ids_and_roles**](docs/RepositoryApi.md#get_snapshot_ids_and_roles) | **GET** /api/repository/v1/snapshots/roleMap | 
 *RepositoryApi* | [**get_snapshot_snapshot_builder_settings**](docs/RepositoryApi.md#get_snapshot_snapshot_builder_settings) | **GET** /api/repository/v1/snapshots/{id}/snapshotBuilder/settings | 
 *RepositoryApi* | [**get_snapshot_tags**](docs/RepositoryApi.md#get_snapshot_tags) | **GET** /api/repository/v1/snapshots/tags | 
 *RepositoryApi* | [**ingest_dataset**](docs/RepositoryApi.md#ingest_dataset) | **POST** /api/repository/v1/datasets/{id}/ingest | 
 *RepositoryApi* | [**ingest_file**](docs/RepositoryApi.md#ingest_file) | **POST** /api/repository/v1/datasets/{id}/files | 
 *RepositoryApi* | [**link_duos_dataset_to_snapshot**](docs/RepositoryApi.md#link_duos_dataset_to_snapshot) | **PUT** /api/repository/v1/snapshots/{id}/linkDuosDataset/{duosId} | 
 *RepositoryApi* | [**list_files**](docs/RepositoryApi.md#list_files) | **GET** /api/repository/v1/snapshots/{id}/files | 
@@ -237,15 +234,14 @@
 *RepositoryApi* | [**retrieve_job_result**](docs/RepositoryApi.md#retrieve_job_result) | **GET** /api/repository/v1/jobs/{id}/result | 
 *RepositoryApi* | [**retrieve_snapshot**](docs/RepositoryApi.md#retrieve_snapshot) | **GET** /api/repository/v1/snapshots/{id} | 
 *RepositoryApi* | [**retrieve_snapshot_policies**](docs/RepositoryApi.md#retrieve_snapshot_policies) | **GET** /api/repository/v1/snapshots/{id}/policies | 
 *RepositoryApi* | [**retrieve_snapshot_summary**](docs/RepositoryApi.md#retrieve_snapshot_summary) | **GET** /api/repository/v1/snapshots/{id}/summary | 
 *RepositoryApi* | [**retrieve_transaction**](docs/RepositoryApi.md#retrieve_transaction) | **GET** /api/repository/v1/datasets/{id}/transactions/{transactionId} | 
 *RepositoryApi* | [**retrieve_user_dataset_roles**](docs/RepositoryApi.md#retrieve_user_dataset_roles) | **GET** /api/repository/v1/datasets/{id}/roles | 
 *RepositoryApi* | [**retrieve_user_snapshot_roles**](docs/RepositoryApi.md#retrieve_user_snapshot_roles) | **GET** /api/repository/v1/snapshots/{id}/roles | 
-*RepositoryApi* | [**search_concepts**](docs/RepositoryApi.md#search_concepts) | **GET** /api/repository/v1/datasets/{id}/snapshotBuilder/concepts/{domainId}/search | 
 *RepositoryApi* | [**set_config_list**](docs/RepositoryApi.md#set_config_list) | **PUT** /api/repository/v1/configs | 
 *RepositoryApi* | [**set_fault**](docs/RepositoryApi.md#set_fault) | **PUT** /api/repository/v1/configs/{name} | 
 *RepositoryApi* | [**sync_duos_dataset_authorized_users**](docs/RepositoryApi.md#sync_duos_dataset_authorized_users) | **PUT** /api/repository/v1/duos/{duosId}/syncAuthorizedUsers | 
 *RepositoryApi* | [**sync_duos_datasets_authorized_users**](docs/RepositoryApi.md#sync_duos_datasets_authorized_users) | **PUT** /api/repository/v1/duos/syncAuthorizedUsers | 
 *RepositoryApi* | [**unlink_duos_dataset_from_snapshot**](docs/RepositoryApi.md#unlink_duos_dataset_from_snapshot) | **DELETE** /api/repository/v1/snapshots/{id}/unlinkDuosDataset | 
 *RepositoryApi* | [**unlock_dataset**](docs/RepositoryApi.md#unlock_dataset) | **PUT** /api/repository/v1/datasets/{id}/unlock | 
 *RepositoryApi* | [**unlock_snapshot**](docs/RepositoryApi.md#unlock_snapshot) | **PUT** /api/repository/v1/snapshots/{id}/unlock | 
@@ -270,16 +266,20 @@
 *SearchApi* | [**query_snapshot_data_by_id**](docs/SearchApi.md#query_snapshot_data_by_id) | **POST** /api/repository/v1/snapshots/{id}/data/{table} | 
 *SnapshotsApi* | [**add_snapshot_auth_domain**](docs/SnapshotsApi.md#add_snapshot_auth_domain) | **PATCH** /api/repository/v1/snapshots/{id}/authDomain | 
 *SnapshotsApi* | [**add_snapshot_policy_member**](docs/SnapshotsApi.md#add_snapshot_policy_member) | **POST** /api/repository/v1/snapshots/{id}/policies/{policyName}/members | 
 *SnapshotsApi* | [**create_snapshot**](docs/SnapshotsApi.md#create_snapshot) | **POST** /api/repository/v1/snapshots | 
 *SnapshotsApi* | [**delete_snapshot**](docs/SnapshotsApi.md#delete_snapshot) | **DELETE** /api/repository/v1/snapshots/{id} | 
 *SnapshotsApi* | [**delete_snapshot_policy_member**](docs/SnapshotsApi.md#delete_snapshot_policy_member) | **DELETE** /api/repository/v1/snapshots/{id}/policies/{policyName}/members/{memberEmail} | 
 *SnapshotsApi* | [**delete_snapshot_snapshot_builder_settings**](docs/SnapshotsApi.md#delete_snapshot_snapshot_builder_settings) | **DELETE** /api/repository/v1/snapshots/{id}/snapshotBuilder/settings | 
+*SnapshotsApi* | [**enumerate_concepts**](docs/SnapshotsApi.md#enumerate_concepts) | **GET** /api/repository/v1/snapshots/{id}/snapshotBuilder/concepts | 
 *SnapshotsApi* | [**enumerate_snapshots**](docs/SnapshotsApi.md#enumerate_snapshots) | **GET** /api/repository/v1/snapshots | 
 *SnapshotsApi* | [**export_snapshot**](docs/SnapshotsApi.md#export_snapshot) | **GET** /api/repository/v1/snapshots/{id}/export | 
+*SnapshotsApi* | [**get_concept_children**](docs/SnapshotsApi.md#get_concept_children) | **GET** /api/repository/v1/snapshots/{id}/snapshotBuilder/concepts/{conceptId}/children | 
+*SnapshotsApi* | [**get_concept_hierarchy**](docs/SnapshotsApi.md#get_concept_hierarchy) | **GET** /api/repository/v1/snapshots/{id}/snapshotBuilder/concepts/{conceptId}/hierarchy | 
+*SnapshotsApi* | [**get_snapshot_builder_count**](docs/SnapshotsApi.md#get_snapshot_builder_count) | **POST** /api/repository/v1/snapshots/{id}/snapshotBuilder/count | 
 *SnapshotsApi* | [**get_snapshot_ids_and_roles**](docs/SnapshotsApi.md#get_snapshot_ids_and_roles) | **GET** /api/repository/v1/snapshots/roleMap | 
 *SnapshotsApi* | [**get_snapshot_snapshot_builder_settings**](docs/SnapshotsApi.md#get_snapshot_snapshot_builder_settings) | **GET** /api/repository/v1/snapshots/{id}/snapshotBuilder/settings | 
 *SnapshotsApi* | [**get_snapshot_tags**](docs/SnapshotsApi.md#get_snapshot_tags) | **GET** /api/repository/v1/snapshots/tags | 
 *SnapshotsApi* | [**link_duos_dataset_to_snapshot**](docs/SnapshotsApi.md#link_duos_dataset_to_snapshot) | **PUT** /api/repository/v1/snapshots/{id}/linkDuosDataset/{duosId} | 
 *SnapshotsApi* | [**list_files**](docs/SnapshotsApi.md#list_files) | **GET** /api/repository/v1/snapshots/{id}/files | 
 *SnapshotsApi* | [**lock_snapshot**](docs/SnapshotsApi.md#lock_snapshot) | **PUT** /api/repository/v1/snapshots/{id}/lock | 
 *SnapshotsApi* | [**lookup_snapshot_file_by_id**](docs/SnapshotsApi.md#lookup_snapshot_file_by_id) | **GET** /api/repository/v1/snapshots/{id}/files/{fileid} | 
@@ -401,27 +401,27 @@
  - [ResourcePolicyModel](docs/ResourcePolicyModel.md)
  - [SamPolicyModel](docs/SamPolicyModel.md)
  - [SnapshotAccessRequest](docs/SnapshotAccessRequest.md)
  - [SnapshotAccessRequestResponse](docs/SnapshotAccessRequestResponse.md)
  - [SnapshotAccessRequestStatus](docs/SnapshotAccessRequestStatus.md)
  - [SnapshotBuilderCohort](docs/SnapshotBuilderCohort.md)
  - [SnapshotBuilderConcept](docs/SnapshotBuilderConcept.md)
+ - [SnapshotBuilderConceptsResponse](docs/SnapshotBuilderConceptsResponse.md)
  - [SnapshotBuilderCountRequest](docs/SnapshotBuilderCountRequest.md)
  - [SnapshotBuilderCountResponse](docs/SnapshotBuilderCountResponse.md)
  - [SnapshotBuilderCountResponseResult](docs/SnapshotBuilderCountResponseResult.md)
  - [SnapshotBuilderCriteria](docs/SnapshotBuilderCriteria.md)
  - [SnapshotBuilderCriteriaGroup](docs/SnapshotBuilderCriteriaGroup.md)
  - [SnapshotBuilderDatasetConceptSet](docs/SnapshotBuilderDatasetConceptSet.md)
  - [SnapshotBuilderDomainCriteria](docs/SnapshotBuilderDomainCriteria.md)
  - [SnapshotBuilderDomainCriteriaAllOf](docs/SnapshotBuilderDomainCriteriaAllOf.md)
  - [SnapshotBuilderDomainOption](docs/SnapshotBuilderDomainOption.md)
  - [SnapshotBuilderDomainOptionAllOf](docs/SnapshotBuilderDomainOptionAllOf.md)
  - [SnapshotBuilderFeatureValueGroup](docs/SnapshotBuilderFeatureValueGroup.md)
  - [SnapshotBuilderGetConceptHierarchyResponse](docs/SnapshotBuilderGetConceptHierarchyResponse.md)
- - [SnapshotBuilderGetConceptsResponse](docs/SnapshotBuilderGetConceptsResponse.md)
  - [SnapshotBuilderOption](docs/SnapshotBuilderOption.md)
  - [SnapshotBuilderParentConcept](docs/SnapshotBuilderParentConcept.md)
  - [SnapshotBuilderProgramDataListCriteria](docs/SnapshotBuilderProgramDataListCriteria.md)
  - [SnapshotBuilderProgramDataListCriteriaAllOf](docs/SnapshotBuilderProgramDataListCriteriaAllOf.md)
  - [SnapshotBuilderProgramDataListItem](docs/SnapshotBuilderProgramDataListItem.md)
  - [SnapshotBuilderProgramDataListOption](docs/SnapshotBuilderProgramDataListOption.md)
  - [SnapshotBuilderProgramDataListOptionAllOf](docs/SnapshotBuilderProgramDataListOptionAllOf.md)
```

### Comparing `data-repo-client-2.61.0/data_repo_client/__init__.py` & `data-repo-client-2.62.0/data_repo_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.61.0"
+__version__ = "2.62.0"
 
 # import apis into sdk package
 from data_repo_client.api.data_repository_service_api import DataRepositoryServiceApi
 from data_repo_client.api.snapshot_access_request_api import SnapshotAccessRequestApi
 from data_repo_client.api.admin_api import AdminApi
 from data_repo_client.api.configs_api import ConfigsApi
 from data_repo_client.api.datasets_api import DatasetsApi
@@ -141,27 +141,27 @@
 from data_repo_client.models.resource_policy_model import ResourcePolicyModel
 from data_repo_client.models.sam_policy_model import SamPolicyModel
 from data_repo_client.models.snapshot_access_request import SnapshotAccessRequest
 from data_repo_client.models.snapshot_access_request_response import SnapshotAccessRequestResponse
 from data_repo_client.models.snapshot_access_request_status import SnapshotAccessRequestStatus
 from data_repo_client.models.snapshot_builder_cohort import SnapshotBuilderCohort
 from data_repo_client.models.snapshot_builder_concept import SnapshotBuilderConcept
+from data_repo_client.models.snapshot_builder_concepts_response import SnapshotBuilderConceptsResponse
 from data_repo_client.models.snapshot_builder_count_request import SnapshotBuilderCountRequest
 from data_repo_client.models.snapshot_builder_count_response import SnapshotBuilderCountResponse
 from data_repo_client.models.snapshot_builder_count_response_result import SnapshotBuilderCountResponseResult
 from data_repo_client.models.snapshot_builder_criteria import SnapshotBuilderCriteria
 from data_repo_client.models.snapshot_builder_criteria_group import SnapshotBuilderCriteriaGroup
 from data_repo_client.models.snapshot_builder_dataset_concept_set import SnapshotBuilderDatasetConceptSet
 from data_repo_client.models.snapshot_builder_domain_criteria import SnapshotBuilderDomainCriteria
 from data_repo_client.models.snapshot_builder_domain_criteria_all_of import SnapshotBuilderDomainCriteriaAllOf
 from data_repo_client.models.snapshot_builder_domain_option import SnapshotBuilderDomainOption
 from data_repo_client.models.snapshot_builder_domain_option_all_of import SnapshotBuilderDomainOptionAllOf
 from data_repo_client.models.snapshot_builder_feature_value_group import SnapshotBuilderFeatureValueGroup
 from data_repo_client.models.snapshot_builder_get_concept_hierarchy_response import SnapshotBuilderGetConceptHierarchyResponse
-from data_repo_client.models.snapshot_builder_get_concepts_response import SnapshotBuilderGetConceptsResponse
 from data_repo_client.models.snapshot_builder_option import SnapshotBuilderOption
 from data_repo_client.models.snapshot_builder_parent_concept import SnapshotBuilderParentConcept
 from data_repo_client.models.snapshot_builder_program_data_list_criteria import SnapshotBuilderProgramDataListCriteria
 from data_repo_client.models.snapshot_builder_program_data_list_criteria_all_of import SnapshotBuilderProgramDataListCriteriaAllOf
 from data_repo_client.models.snapshot_builder_program_data_list_item import SnapshotBuilderProgramDataListItem
 from data_repo_client.models.snapshot_builder_program_data_list_option import SnapshotBuilderProgramDataListOption
 from data_repo_client.models.snapshot_builder_program_data_list_option_all_of import SnapshotBuilderProgramDataListOptionAllOf
```

### Comparing `data-repo-client-2.61.0/data_repo_client/api/__init__.py` & `data-repo-client-2.62.0/data_repo_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/admin_api.py` & `data-repo-client-2.62.0/data_repo_client/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/configs_api.py` & `data-repo-client-2.62.0/data_repo_client/api/configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/data_repository_service_api.py` & `data-repo-client-2.62.0/data_repo_client/api/data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/datasets_api.py` & `data-repo-client-2.62.0/data_repo_client/api/datasets_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1664,260 +1664,14 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_concept_hierarchy(self, id, concept_id, **kwargs):  # noqa: E501
-        """get_concept_hierarchy  # noqa: E501
-
-        Given a concept ID, return the tree of concepts that contain this concept. A tree is represented as a list of parent IDs and their children, which are concepts.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_concept_hierarchy(id, concept_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int concept_id: A dataset concept id. (required)
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: SnapshotBuilderGetConceptHierarchyResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_concept_hierarchy_with_http_info(id, concept_id, **kwargs)  # noqa: E501
-
-    def get_concept_hierarchy_with_http_info(self, id, concept_id, **kwargs):  # noqa: E501
-        """get_concept_hierarchy  # noqa: E501
-
-        Given a concept ID, return the tree of concepts that contain this concept. A tree is represented as a list of parent IDs and their children, which are concepts.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_concept_hierarchy_with_http_info(id, concept_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int concept_id: A dataset concept id. (required)
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(SnapshotBuilderGetConceptHierarchyResponse, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'id',
-            'concept_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_concept_hierarchy" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_concept_hierarchy`")  # noqa: E501
-        # verify the required parameter 'concept_id' is set
-        if self.api_client.client_side_validation and ('concept_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['concept_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `concept_id` when calling `get_concept_hierarchy`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'concept_id' in local_var_params:
-            path_params['conceptId'] = local_var_params['concept_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotBuilder/conceptHierarchy/{conceptId}', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='SnapshotBuilderGetConceptHierarchyResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def get_concepts(self, id, concept_id, **kwargs):  # noqa: E501
-        """get_concepts  # noqa: E501
-
-        Gets all concepts with the specified concept as their parent.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_concepts(id, concept_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int concept_id: A dataset concept id. (required)
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: SnapshotBuilderGetConceptsResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_concepts_with_http_info(id, concept_id, **kwargs)  # noqa: E501
-
-    def get_concepts_with_http_info(self, id, concept_id, **kwargs):  # noqa: E501
-        """get_concepts  # noqa: E501
-
-        Gets all concepts with the specified concept as their parent.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_concepts_with_http_info(id, concept_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int concept_id: A dataset concept id. (required)
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(SnapshotBuilderGetConceptsResponse, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'id',
-            'concept_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_concepts" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_concepts`")  # noqa: E501
-        # verify the required parameter 'concept_id' is set
-        if self.api_client.client_side_validation and ('concept_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['concept_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `concept_id` when calling `get_concepts`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'concept_id' in local_var_params:
-            path_params['conceptId'] = local_var_params['concept_id']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotBuilder/concepts/{conceptId}', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='SnapshotBuilderGetConceptsResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def get_dataset_tags(self, **kwargs):  # noqa: E501
         """get_dataset_tags  # noqa: E501
 
         Get accessible dataset tags  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_dataset_tags(async_req=True)
@@ -2158,141 +1912,14 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_snapshot_builder_count(self, id, snapshot_builder_count_request, **kwargs):  # noqa: E501
-        """get_snapshot_builder_count  # noqa: E501
-
-        Given a list of snapshot builder cohorts, return the unique participant count for this dataset.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_snapshot_builder_count(id, snapshot_builder_count_request, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param SnapshotBuilderCountRequest snapshot_builder_count_request: The cohorts to count participants in (required)
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: SnapshotBuilderCountResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_snapshot_builder_count_with_http_info(id, snapshot_builder_count_request, **kwargs)  # noqa: E501
-
-    def get_snapshot_builder_count_with_http_info(self, id, snapshot_builder_count_request, **kwargs):  # noqa: E501
-        """get_snapshot_builder_count  # noqa: E501
-
-        Given a list of snapshot builder cohorts, return the unique participant count for this dataset.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_snapshot_builder_count_with_http_info(id, snapshot_builder_count_request, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param SnapshotBuilderCountRequest snapshot_builder_count_request: The cohorts to count participants in (required)
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(SnapshotBuilderCountResponse, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'id',
-            'snapshot_builder_count_request'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_snapshot_builder_count" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_snapshot_builder_count`")  # noqa: E501
-        # verify the required parameter 'snapshot_builder_count_request' is set
-        if self.api_client.client_side_validation and ('snapshot_builder_count_request' not in local_var_params or  # noqa: E501
-                                                        local_var_params['snapshot_builder_count_request'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `snapshot_builder_count_request` when calling `get_snapshot_builder_count`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        if 'snapshot_builder_count_request' in local_var_params:
-            body_params = local_var_params['snapshot_builder_count_request']
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # HTTP header `Content-Type`
-        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotBuilder/count', 'POST',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='SnapshotBuilderCountResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def ingest_dataset(self, id, **kwargs):  # noqa: E501
         """ingest_dataset  # noqa: E501
 
         Ingest data into a dataset table  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.ingest_dataset(id, async_req=True)
@@ -4547,142 +4174,14 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def search_concepts(self, id, domain_id, **kwargs):  # noqa: E501
-        """search_concepts  # noqa: E501
-
-        Searches concepts of the specified domain that match the given searchText.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.search_concepts(id, domain_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int domain_id: The concept ID of the domain (required)
-        :param str search_text: User specified text to search concepts for.
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: SnapshotBuilderGetConceptsResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.search_concepts_with_http_info(id, domain_id, **kwargs)  # noqa: E501
-
-    def search_concepts_with_http_info(self, id, domain_id, **kwargs):  # noqa: E501
-        """search_concepts  # noqa: E501
-
-        Searches concepts of the specified domain that match the given searchText.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.search_concepts_with_http_info(id, domain_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int domain_id: The concept ID of the domain (required)
-        :param str search_text: User specified text to search concepts for.
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(SnapshotBuilderGetConceptsResponse, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'id',
-            'domain_id',
-            'search_text'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method search_concepts" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `search_concepts`")  # noqa: E501
-        # verify the required parameter 'domain_id' is set
-        if self.api_client.client_side_validation and ('domain_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['domain_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `domain_id` when calling `search_concepts`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'domain_id' in local_var_params:
-            path_params['domainId'] = local_var_params['domain_id']  # noqa: E501
-
-        query_params = []
-        if 'search_text' in local_var_params and local_var_params['search_text'] is not None:  # noqa: E501
-            query_params.append(('searchText', local_var_params['search_text']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotBuilder/concepts/{domainId}/search', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='SnapshotBuilderGetConceptsResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def unlock_dataset(self, id, **kwargs):  # noqa: E501
         """unlock_dataset  # noqa: E501
 
         Remove an exclusive or shared lock on the dataset.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.unlock_dataset(id, async_req=True)
```

### Comparing `data-repo-client-2.61.0/data_repo_client/api/duos_api.py` & `data-repo-client-2.62.0/data_repo_client/api/duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/jobs_api.py` & `data-repo-client-2.62.0/data_repo_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/journal_api.py` & `data-repo-client-2.62.0/data_repo_client/api/journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/profiles_api.py` & `data-repo-client-2.62.0/data_repo_client/api/profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/register_api.py` & `data-repo-client-2.62.0/data_repo_client/api/register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/repository_api.py` & `data-repo-client-2.62.0/data_repo_client/api/repository_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2128,14 +2128,142 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def enumerate_concepts(self, id, domain_id, **kwargs):  # noqa: E501
+        """enumerate_concepts  # noqa: E501
+
+        Retrieves concepts of the specified domain and enables filtering concepts given by the searchText.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.enumerate_concepts(id, domain_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param int domain_id: The concept ID of the domain (required)
+        :param str filter_text: User specified text to search concepts for.
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: SnapshotBuilderConceptsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.enumerate_concepts_with_http_info(id, domain_id, **kwargs)  # noqa: E501
+
+    def enumerate_concepts_with_http_info(self, id, domain_id, **kwargs):  # noqa: E501
+        """enumerate_concepts  # noqa: E501
+
+        Retrieves concepts of the specified domain and enables filtering concepts given by the searchText.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.enumerate_concepts_with_http_info(id, domain_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param int domain_id: The concept ID of the domain (required)
+        :param str filter_text: User specified text to search concepts for.
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(SnapshotBuilderConceptsResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'domain_id',
+            'filter_text'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method enumerate_concepts" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `enumerate_concepts`")  # noqa: E501
+        # verify the required parameter 'domain_id' is set
+        if self.api_client.client_side_validation and ('domain_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['domain_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `domain_id` when calling `enumerate_concepts`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+        if 'domain_id' in local_var_params and local_var_params['domain_id'] is not None:  # noqa: E501
+            query_params.append(('domainId', local_var_params['domain_id']))  # noqa: E501
+        if 'filter_text' in local_var_params and local_var_params['filter_text'] is not None:  # noqa: E501
+            query_params.append(('filterText', local_var_params['filter_text']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['oidc']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots/{id}/snapshotBuilder/concepts', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SnapshotBuilderConceptsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def enumerate_datasets(self, **kwargs):  # noqa: E501
         """enumerate_datasets  # noqa: E501
 
         Returns a list of all of the datasets the caller has access to   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.enumerate_datasets(async_req=True)
@@ -2800,62 +2928,62 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_concept_hierarchy(self, id, concept_id, **kwargs):  # noqa: E501
-        """get_concept_hierarchy  # noqa: E501
+    def get_concept_children(self, id, concept_id, **kwargs):  # noqa: E501
+        """get_concept_children  # noqa: E501
 
-        Given a concept ID, return the tree of concepts that contain this concept. A tree is represented as a list of parent IDs and their children, which are concepts.   # noqa: E501
+        Gets all concepts with the specified concept as their parent.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_concept_hierarchy(id, concept_id, async_req=True)
+        >>> thread = api.get_concept_children(id, concept_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int concept_id: A dataset concept id. (required)
+        :param str id: The UUID of the snapshot. (required)
+        :param int concept_id: A snapshot concept id. (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: SnapshotBuilderGetConceptHierarchyResponse
+        :return: SnapshotBuilderConceptsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_concept_hierarchy_with_http_info(id, concept_id, **kwargs)  # noqa: E501
+        return self.get_concept_children_with_http_info(id, concept_id, **kwargs)  # noqa: E501
 
-    def get_concept_hierarchy_with_http_info(self, id, concept_id, **kwargs):  # noqa: E501
-        """get_concept_hierarchy  # noqa: E501
+    def get_concept_children_with_http_info(self, id, concept_id, **kwargs):  # noqa: E501
+        """get_concept_children  # noqa: E501
 
-        Given a concept ID, return the tree of concepts that contain this concept. A tree is represented as a list of parent IDs and their children, which are concepts.   # noqa: E501
+        Gets all concepts with the specified concept as their parent.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_concept_hierarchy_with_http_info(id, concept_id, async_req=True)
+        >>> thread = api.get_concept_children_with_http_info(id, concept_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int concept_id: A dataset concept id. (required)
+        :param str id: The UUID of the snapshot. (required)
+        :param int concept_id: A snapshot concept id. (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(SnapshotBuilderGetConceptHierarchyResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(SnapshotBuilderConceptsResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -2871,26 +2999,26 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_concept_hierarchy" % key
+                    " to method get_concept_children" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_concept_hierarchy`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `get_concept_children`")  # noqa: E501
         # verify the required parameter 'concept_id' is set
         if self.api_client.client_side_validation and ('concept_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['concept_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `concept_id` when calling `get_concept_hierarchy`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `concept_id` when calling `get_concept_children`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
         if 'concept_id' in local_var_params:
@@ -2908,77 +3036,77 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oidc']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotBuilder/conceptHierarchy/{conceptId}', 'GET',
+            '/api/repository/v1/snapshots/{id}/snapshotBuilder/concepts/{conceptId}/children', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='SnapshotBuilderGetConceptHierarchyResponse',  # noqa: E501
+            response_type='SnapshotBuilderConceptsResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_concepts(self, id, concept_id, **kwargs):  # noqa: E501
-        """get_concepts  # noqa: E501
+    def get_concept_hierarchy(self, id, concept_id, **kwargs):  # noqa: E501
+        """get_concept_hierarchy  # noqa: E501
 
-        Gets all concepts with the specified concept as their parent.   # noqa: E501
+        Given a concept ID, return the tree of concepts that contain this concept. A tree is represented as a list of parent IDs and their children, which are concepts.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_concepts(id, concept_id, async_req=True)
+        >>> thread = api.get_concept_hierarchy(id, concept_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int concept_id: A dataset concept id. (required)
+        :param str id: The UUID of the snapshot. (required)
+        :param int concept_id: A snapshot concept id. (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: SnapshotBuilderGetConceptsResponse
+        :return: SnapshotBuilderGetConceptHierarchyResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_concepts_with_http_info(id, concept_id, **kwargs)  # noqa: E501
+        return self.get_concept_hierarchy_with_http_info(id, concept_id, **kwargs)  # noqa: E501
 
-    def get_concepts_with_http_info(self, id, concept_id, **kwargs):  # noqa: E501
-        """get_concepts  # noqa: E501
+    def get_concept_hierarchy_with_http_info(self, id, concept_id, **kwargs):  # noqa: E501
+        """get_concept_hierarchy  # noqa: E501
 
-        Gets all concepts with the specified concept as their parent.   # noqa: E501
+        Given a concept ID, return the tree of concepts that contain this concept. A tree is represented as a list of parent IDs and their children, which are concepts.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.get_concepts_with_http_info(id, concept_id, async_req=True)
+        >>> thread = api.get_concept_hierarchy_with_http_info(id, concept_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int concept_id: A dataset concept id. (required)
+        :param str id: The UUID of the snapshot. (required)
+        :param int concept_id: A snapshot concept id. (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(SnapshotBuilderGetConceptsResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(SnapshotBuilderGetConceptHierarchyResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -2994,26 +3122,26 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_concepts" % key
+                    " to method get_concept_hierarchy" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
                                                         local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `get_concepts`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `get_concept_hierarchy`")  # noqa: E501
         # verify the required parameter 'concept_id' is set
         if self.api_client.client_side_validation and ('concept_id' not in local_var_params or  # noqa: E501
                                                         local_var_params['concept_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `concept_id` when calling `get_concepts`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `concept_id` when calling `get_concept_hierarchy`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
         if 'concept_id' in local_var_params:
@@ -3031,22 +3159,22 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oidc']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotBuilder/concepts/{conceptId}', 'GET',
+            '/api/repository/v1/snapshots/{id}/snapshotBuilder/concepts/{conceptId}/hierarchy', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='SnapshotBuilderGetConceptsResponse',  # noqa: E501
+            response_type='SnapshotBuilderGetConceptHierarchyResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
@@ -3516,22 +3644,22 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_snapshot_builder_count(self, id, snapshot_builder_count_request, **kwargs):  # noqa: E501
         """get_snapshot_builder_count  # noqa: E501
 
-        Given a list of snapshot builder cohorts, return the unique participant count for this dataset.   # noqa: E501
+        Given a list of snapshot builder cohorts, return the unique participant count for this snapshot.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_snapshot_builder_count(id, snapshot_builder_count_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
+        :param str id: The UUID of the snapshot. (required)
         :param SnapshotBuilderCountRequest snapshot_builder_count_request: The cohorts to count participants in (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -3542,22 +3670,22 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.get_snapshot_builder_count_with_http_info(id, snapshot_builder_count_request, **kwargs)  # noqa: E501
 
     def get_snapshot_builder_count_with_http_info(self, id, snapshot_builder_count_request, **kwargs):  # noqa: E501
         """get_snapshot_builder_count  # noqa: E501
 
-        Given a list of snapshot builder cohorts, return the unique participant count for this dataset.   # noqa: E501
+        Given a list of snapshot builder cohorts, return the unique participant count for this snapshot.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_snapshot_builder_count_with_http_info(id, snapshot_builder_count_request, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
+        :param str id: The UUID of the snapshot. (required)
         :param SnapshotBuilderCountRequest snapshot_builder_count_request: The cohorts to count participants in (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -3625,15 +3753,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['oidc']  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotBuilder/count', 'POST',
+            '/api/repository/v1/snapshots/{id}/snapshotBuilder/count', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='SnapshotBuilderCountResponse',  # noqa: E501
@@ -8108,142 +8236,14 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def search_concepts(self, id, domain_id, **kwargs):  # noqa: E501
-        """search_concepts  # noqa: E501
-
-        Searches concepts of the specified domain that match the given searchText.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.search_concepts(id, domain_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int domain_id: The concept ID of the domain (required)
-        :param str search_text: User specified text to search concepts for.
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: SnapshotBuilderGetConceptsResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.search_concepts_with_http_info(id, domain_id, **kwargs)  # noqa: E501
-
-    def search_concepts_with_http_info(self, id, domain_id, **kwargs):  # noqa: E501
-        """search_concepts  # noqa: E501
-
-        Searches concepts of the specified domain that match the given searchText.   # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.search_concepts_with_http_info(id, domain_id, async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool: execute request asynchronously
-        :param str id: The UUID of the dataset. (required)
-        :param int domain_id: The concept ID of the domain (required)
-        :param str search_text: User specified text to search concepts for.
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: tuple(SnapshotBuilderGetConceptsResponse, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'id',
-            'domain_id',
-            'search_text'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method search_concepts" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'id' is set
-        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `search_concepts`")  # noqa: E501
-        # verify the required parameter 'domain_id' is set
-        if self.api_client.client_side_validation and ('domain_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['domain_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `domain_id` when calling `search_concepts`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'id' in local_var_params:
-            path_params['id'] = local_var_params['id']  # noqa: E501
-        if 'domain_id' in local_var_params:
-            path_params['domainId'] = local_var_params['domain_id']  # noqa: E501
-
-        query_params = []
-        if 'search_text' in local_var_params and local_var_params['search_text'] is not None:  # noqa: E501
-            query_params.append(('searchText', local_var_params['search_text']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['oidc']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/repository/v1/datasets/{id}/snapshotBuilder/concepts/{domainId}/search', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='SnapshotBuilderGetConceptsResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
     def set_config_list(self, **kwargs):  # noqa: E501
         """set_config_list  # noqa: E501
 
         Set the a group of configurations  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.set_config_list(async_req=True)
```

### Comparing `data-repo-client-2.61.0/data_repo_client/api/resources_api.py` & `data-repo-client-2.62.0/data_repo_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/search_api.py` & `data-repo-client-2.62.0/data_repo_client/api/search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/snapshot_access_request_api.py` & `data-repo-client-2.62.0/data_repo_client/api/snapshot_access_request_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/snapshots_api.py` & `data-repo-client-2.62.0/data_repo_client/api/snapshots_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -761,14 +761,142 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def enumerate_concepts(self, id, domain_id, **kwargs):  # noqa: E501
+        """enumerate_concepts  # noqa: E501
+
+        Retrieves concepts of the specified domain and enables filtering concepts given by the searchText.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.enumerate_concepts(id, domain_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param int domain_id: The concept ID of the domain (required)
+        :param str filter_text: User specified text to search concepts for.
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: SnapshotBuilderConceptsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.enumerate_concepts_with_http_info(id, domain_id, **kwargs)  # noqa: E501
+
+    def enumerate_concepts_with_http_info(self, id, domain_id, **kwargs):  # noqa: E501
+        """enumerate_concepts  # noqa: E501
+
+        Retrieves concepts of the specified domain and enables filtering concepts given by the searchText.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.enumerate_concepts_with_http_info(id, domain_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param int domain_id: The concept ID of the domain (required)
+        :param str filter_text: User specified text to search concepts for.
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(SnapshotBuilderConceptsResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'domain_id',
+            'filter_text'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method enumerate_concepts" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `enumerate_concepts`")  # noqa: E501
+        # verify the required parameter 'domain_id' is set
+        if self.api_client.client_side_validation and ('domain_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['domain_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `domain_id` when calling `enumerate_concepts`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+        if 'domain_id' in local_var_params and local_var_params['domain_id'] is not None:  # noqa: E501
+            query_params.append(('domainId', local_var_params['domain_id']))  # noqa: E501
+        if 'filter_text' in local_var_params and local_var_params['filter_text'] is not None:  # noqa: E501
+            query_params.append(('filterText', local_var_params['filter_text']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['oidc']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots/{id}/snapshotBuilder/concepts', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SnapshotBuilderConceptsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def enumerate_snapshots(self, **kwargs):  # noqa: E501
         """enumerate_snapshots  # noqa: E501
 
         Returns a list of all of the snapshots to which the caller has access. Access may be granted directly via SAM and/or indirectly via a user's linked RAS passport in Terra.  Snapshot accessibility derived from a linked RAS passport will be attributed to the \"reader\" role.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.enumerate_snapshots(async_req=True)
@@ -1043,14 +1171,387 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_concept_children(self, id, concept_id, **kwargs):  # noqa: E501
+        """get_concept_children  # noqa: E501
+
+        Gets all concepts with the specified concept as their parent.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_concept_children(id, concept_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param int concept_id: A snapshot concept id. (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: SnapshotBuilderConceptsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_concept_children_with_http_info(id, concept_id, **kwargs)  # noqa: E501
+
+    def get_concept_children_with_http_info(self, id, concept_id, **kwargs):  # noqa: E501
+        """get_concept_children  # noqa: E501
+
+        Gets all concepts with the specified concept as their parent.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_concept_children_with_http_info(id, concept_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param int concept_id: A snapshot concept id. (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(SnapshotBuilderConceptsResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'concept_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_concept_children" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `get_concept_children`")  # noqa: E501
+        # verify the required parameter 'concept_id' is set
+        if self.api_client.client_side_validation and ('concept_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['concept_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `concept_id` when calling `get_concept_children`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'concept_id' in local_var_params:
+            path_params['conceptId'] = local_var_params['concept_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['oidc']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots/{id}/snapshotBuilder/concepts/{conceptId}/children', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SnapshotBuilderConceptsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_concept_hierarchy(self, id, concept_id, **kwargs):  # noqa: E501
+        """get_concept_hierarchy  # noqa: E501
+
+        Given a concept ID, return the tree of concepts that contain this concept. A tree is represented as a list of parent IDs and their children, which are concepts.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_concept_hierarchy(id, concept_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param int concept_id: A snapshot concept id. (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: SnapshotBuilderGetConceptHierarchyResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_concept_hierarchy_with_http_info(id, concept_id, **kwargs)  # noqa: E501
+
+    def get_concept_hierarchy_with_http_info(self, id, concept_id, **kwargs):  # noqa: E501
+        """get_concept_hierarchy  # noqa: E501
+
+        Given a concept ID, return the tree of concepts that contain this concept. A tree is represented as a list of parent IDs and their children, which are concepts.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_concept_hierarchy_with_http_info(id, concept_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param int concept_id: A snapshot concept id. (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(SnapshotBuilderGetConceptHierarchyResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'concept_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_concept_hierarchy" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `get_concept_hierarchy`")  # noqa: E501
+        # verify the required parameter 'concept_id' is set
+        if self.api_client.client_side_validation and ('concept_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['concept_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `concept_id` when calling `get_concept_hierarchy`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+        if 'concept_id' in local_var_params:
+            path_params['conceptId'] = local_var_params['concept_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['oidc']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots/{id}/snapshotBuilder/concepts/{conceptId}/hierarchy', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SnapshotBuilderGetConceptHierarchyResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_snapshot_builder_count(self, id, snapshot_builder_count_request, **kwargs):  # noqa: E501
+        """get_snapshot_builder_count  # noqa: E501
+
+        Given a list of snapshot builder cohorts, return the unique participant count for this snapshot.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_snapshot_builder_count(id, snapshot_builder_count_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param SnapshotBuilderCountRequest snapshot_builder_count_request: The cohorts to count participants in (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: SnapshotBuilderCountResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_snapshot_builder_count_with_http_info(id, snapshot_builder_count_request, **kwargs)  # noqa: E501
+
+    def get_snapshot_builder_count_with_http_info(self, id, snapshot_builder_count_request, **kwargs):  # noqa: E501
+        """get_snapshot_builder_count  # noqa: E501
+
+        Given a list of snapshot builder cohorts, return the unique participant count for this snapshot.   # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_snapshot_builder_count_with_http_info(id, snapshot_builder_count_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str id: The UUID of the snapshot. (required)
+        :param SnapshotBuilderCountRequest snapshot_builder_count_request: The cohorts to count participants in (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(SnapshotBuilderCountResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'id',
+            'snapshot_builder_count_request'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_snapshot_builder_count" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'id' is set
+        if self.api_client.client_side_validation and ('id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `get_snapshot_builder_count`")  # noqa: E501
+        # verify the required parameter 'snapshot_builder_count_request' is set
+        if self.api_client.client_side_validation and ('snapshot_builder_count_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['snapshot_builder_count_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `snapshot_builder_count_request` when calling `get_snapshot_builder_count`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in local_var_params:
+            path_params['id'] = local_var_params['id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'snapshot_builder_count_request' in local_var_params:
+            body_params = local_var_params['snapshot_builder_count_request']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['oidc']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/api/repository/v1/snapshots/{id}/snapshotBuilder/count', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SnapshotBuilderCountResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_snapshot_ids_and_roles(self, **kwargs):  # noqa: E501
         """get_snapshot_ids_and_roles  # noqa: E501
 
         Get accessible snapshot IDs mapped to the roles which confer access. Access may be granted directly via Sam and/or indirectly via a user's linked RAS passport in Terra.  Snapshot accessibility derived from a linked RAS passport will be attributed to the \"reader\" role.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_snapshot_ids_and_roles(async_req=True)
```

### Comparing `data-repo-client-2.61.0/data_repo_client/api/unauthenticated_api.py` & `data-repo-client-2.62.0/data_repo_client/api/unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api/upgrade_api.py` & `data-repo-client-2.62.0/data_repo_client/api/upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/api_client.py` & `data-repo-client-2.62.0/data_repo_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.61.0/python'
+        self.user_agent = 'OpenAPI-Generator/2.62.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `data-repo-client-2.61.0/data_repo_client/configuration.py` & `data-repo-client-2.62.0/data_repo_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 2.61.0".\
+               "SDK Package Version: 2.62.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `data-repo-client-2.61.0/data_repo_client/exceptions.py` & `data-repo-client-2.62.0/data_repo_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/__init__.py` & `data-repo-client-2.62.0/data_repo_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,27 +112,27 @@
 from data_repo_client.models.resource_policy_model import ResourcePolicyModel
 from data_repo_client.models.sam_policy_model import SamPolicyModel
 from data_repo_client.models.snapshot_access_request import SnapshotAccessRequest
 from data_repo_client.models.snapshot_access_request_response import SnapshotAccessRequestResponse
 from data_repo_client.models.snapshot_access_request_status import SnapshotAccessRequestStatus
 from data_repo_client.models.snapshot_builder_cohort import SnapshotBuilderCohort
 from data_repo_client.models.snapshot_builder_concept import SnapshotBuilderConcept
+from data_repo_client.models.snapshot_builder_concepts_response import SnapshotBuilderConceptsResponse
 from data_repo_client.models.snapshot_builder_count_request import SnapshotBuilderCountRequest
 from data_repo_client.models.snapshot_builder_count_response import SnapshotBuilderCountResponse
 from data_repo_client.models.snapshot_builder_count_response_result import SnapshotBuilderCountResponseResult
 from data_repo_client.models.snapshot_builder_criteria import SnapshotBuilderCriteria
 from data_repo_client.models.snapshot_builder_criteria_group import SnapshotBuilderCriteriaGroup
 from data_repo_client.models.snapshot_builder_dataset_concept_set import SnapshotBuilderDatasetConceptSet
 from data_repo_client.models.snapshot_builder_domain_criteria import SnapshotBuilderDomainCriteria
 from data_repo_client.models.snapshot_builder_domain_criteria_all_of import SnapshotBuilderDomainCriteriaAllOf
 from data_repo_client.models.snapshot_builder_domain_option import SnapshotBuilderDomainOption
 from data_repo_client.models.snapshot_builder_domain_option_all_of import SnapshotBuilderDomainOptionAllOf
 from data_repo_client.models.snapshot_builder_feature_value_group import SnapshotBuilderFeatureValueGroup
 from data_repo_client.models.snapshot_builder_get_concept_hierarchy_response import SnapshotBuilderGetConceptHierarchyResponse
-from data_repo_client.models.snapshot_builder_get_concepts_response import SnapshotBuilderGetConceptsResponse
 from data_repo_client.models.snapshot_builder_option import SnapshotBuilderOption
 from data_repo_client.models.snapshot_builder_parent_concept import SnapshotBuilderParentConcept
 from data_repo_client.models.snapshot_builder_program_data_list_criteria import SnapshotBuilderProgramDataListCriteria
 from data_repo_client.models.snapshot_builder_program_data_list_criteria_all_of import SnapshotBuilderProgramDataListCriteriaAllOf
 from data_repo_client.models.snapshot_builder_program_data_list_item import SnapshotBuilderProgramDataListItem
 from data_repo_client.models.snapshot_builder_program_data_list_option import SnapshotBuilderProgramDataListOption
 from data_repo_client.models.snapshot_builder_program_data_list_option_all_of import SnapshotBuilderProgramDataListOptionAllOf
```

### Comparing `data-repo-client-2.61.0/data_repo_client/models/access_info_big_query_model.py` & `data-repo-client-2.62.0/data_repo_client/models/access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/access_info_big_query_model_table.py` & `data-repo-client-2.62.0/data_repo_client/models/access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/access_info_model.py` & `data-repo-client-2.62.0/data_repo_client/models/access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/access_info_parquet_model.py` & `data-repo-client-2.62.0/data_repo_client/models/access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/access_info_parquet_model_table.py` & `data-repo-client-2.62.0/data_repo_client/models/access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/add_auth_domain_response_model.py` & `data-repo-client-2.62.0/data_repo_client/models/add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/asset_model.py` & `data-repo-client-2.62.0/data_repo_client/models/asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/asset_table_model.py` & `data-repo-client-2.62.0/data_repo_client/models/asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/billing_profile_model.py` & `data-repo-client-2.62.0/data_repo_client/models/billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/billing_profile_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/billing_profile_update_model.py` & `data-repo-client-2.62.0/data_repo_client/models/billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/bulk_load_array_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/bulk_load_array_result_model.py` & `data-repo-client-2.62.0/data_repo_client/models/bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/bulk_load_file_model.py` & `data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/bulk_load_file_result_model.py` & `data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/bulk_load_file_state.py` & `data-repo-client-2.62.0/data_repo_client/models/bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/bulk_load_history_model.py` & `data-repo-client-2.62.0/data_repo_client/models/bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/bulk_load_history_model_list.py` & `data-repo-client-2.62.0/data_repo_client/models/bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/bulk_load_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/bulk_load_result_model.py` & `data-repo-client-2.62.0/data_repo_client/models/bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/cloud_platform.py` & `data-repo-client-2.62.0/data_repo_client/models/cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/column_model.py` & `data-repo-client-2.62.0/data_repo_client/models/column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/column_statistics_double_model.py` & `data-repo-client-2.62.0/data_repo_client/models/column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/column_statistics_double_model_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/column_statistics_int_model.py` & `data-repo-client-2.62.0/data_repo_client/models/column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/column_statistics_int_model_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/column_statistics_model.py` & `data-repo-client-2.62.0/data_repo_client/models/column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/column_statistics_text_model.py` & `data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/column_statistics_text_model_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/column_statistics_text_value.py` & `data-repo-client-2.62.0/data_repo_client/models/column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/config_enable_model.py` & `data-repo-client-2.62.0/data_repo_client/models/config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/config_fault_counted_model.py` & `data-repo-client-2.62.0/data_repo_client/models/config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/config_fault_model.py` & `data-repo-client-2.62.0/data_repo_client/models/config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/config_group_model.py` & `data-repo-client-2.62.0/data_repo_client/models/config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/config_list_model.py` & `data-repo-client-2.62.0/data_repo_client/models/config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/config_model.py` & `data-repo-client-2.62.0/data_repo_client/models/config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/config_parameter_model.py` & `data-repo-client-2.62.0/data_repo_client/models/config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/data_deletion_gcs_file_model.py` & `data-repo-client-2.62.0/data_repo_client/models/data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/data_deletion_json_array_model.py` & `data-repo-client-2.62.0/data_repo_client/models/data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/data_deletion_request.py` & `data-repo-client-2.62.0/data_repo_client/models/data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/data_deletion_table_model.py` & `data-repo-client-2.62.0/data_repo_client/models/data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_data_model.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_model.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_patch_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_request_access_include_model.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_request_model_policies.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_schema_column_update_model.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_schema_update_model.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_schema_update_model_changes.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_specification_model.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/dataset_summary_model.py` & `data-repo-client-2.62.0/data_repo_client/models/dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/date_partition_options_model.py` & `data-repo-client-2.62.0/data_repo_client/models/date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/delete_response_model.py` & `data-repo-client-2.62.0/data_repo_client/models/delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/directory_detail_model.py` & `data-repo-client-2.62.0/data_repo_client/models/directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_access_method.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_access_url.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_alias_model.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_authorizations.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_checksum.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_contents_object.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_error.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_object.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_passport_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_passport_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/drs_service_info.py` & `data-repo-client-2.62.0/data_repo_client/models/drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/duos_firecloud_group_model.py` & `data-repo-client-2.62.0/data_repo_client/models/duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/duos_firecloud_groups_sync_response.py` & `data-repo-client-2.62.0/data_repo_client/models/duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/enumerate_billing_profile_model.py` & `data-repo-client-2.62.0/data_repo_client/models/enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/enumerate_dataset_model.py` & `data-repo-client-2.62.0/data_repo_client/models/enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/enumerate_snapshot_access_request.py` & `data-repo-client-2.62.0/data_repo_client/models/enumerate_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/enumerate_snapshot_model.py` & `data-repo-client-2.62.0/data_repo_client/models/enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/enumerate_sort_by_param.py` & `data-repo-client-2.62.0/data_repo_client/models/enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/error_model.py` & `data-repo-client-2.62.0/data_repo_client/models/error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/file_detail_model.py` & `data-repo-client-2.62.0/data_repo_client/models/file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/file_load_model.py` & `data-repo-client-2.62.0/data_repo_client/models/file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/file_model.py` & `data-repo-client-2.62.0/data_repo_client/models/file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/file_model_type.py` & `data-repo-client-2.62.0/data_repo_client/models/file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/iam_resource_type_enum.py` & `data-repo-client-2.62.0/data_repo_client/models/iam_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/inaccessible_workspace_policy_model.py` & `data-repo-client-2.62.0/data_repo_client/models/inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/ingest_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/ingest_response_model.py` & `data-repo-client-2.62.0/data_repo_client/models/ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/int_partition_options_model.py` & `data-repo-client-2.62.0/data_repo_client/models/int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/job_model.py` & `data-repo-client-2.62.0/data_repo_client/models/job_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/journal_entry_model.py` & `data-repo-client-2.62.0/data_repo_client/models/journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/policy_member_request.py` & `data-repo-client-2.62.0/data_repo_client/models/policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/policy_model.py` & `data-repo-client-2.62.0/data_repo_client/models/policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/policy_response.py` & `data-repo-client-2.62.0/data_repo_client/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/query_column_statistics_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/query_data_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/relationship_model.py` & `data-repo-client-2.62.0/data_repo_client/models/relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/relationship_term_model.py` & `data-repo-client-2.62.0/data_repo_client/models/relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/repository_configuration_model.py` & `data-repo-client-2.62.0/data_repo_client/models/repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/repository_status_model.py` & `data-repo-client-2.62.0/data_repo_client/models/repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/repository_status_model_systems.py` & `data-repo-client-2.62.0/data_repo_client/models/repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/resource_locks.py` & `data-repo-client-2.62.0/data_repo_client/models/resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/resource_policy_model.py` & `data-repo-client-2.62.0/data_repo_client/models/resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/sam_policy_model.py` & `data-repo-client-2.62.0/data_repo_client/models/sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_access_request.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_access_request_response.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_access_request_status.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_cohort.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_cohort.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_concept.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_count_request.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_count_response.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_count_response_result.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_criteria.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_criteria_group.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_criteria_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_domain_criteria.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_domain_option.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_feature_value_group.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_get_concepts_response.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_concepts_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from data_repo_client.configuration import Configuration
 
 
-class SnapshotBuilderGetConceptsResponse(object):
+class SnapshotBuilderConceptsResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -39,66 +39,66 @@
 
     attribute_map = {
         'result': 'result',
         'sql': 'sql'
     }
 
     def __init__(self, result=None, sql=None, local_vars_configuration=None):  # noqa: E501
-        """SnapshotBuilderGetConceptsResponse - a model defined in OpenAPI"""  # noqa: E501
+        """SnapshotBuilderConceptsResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._result = None
         self._sql = None
         self.discriminator = None
 
         self.result = result
         if sql is not None:
             self.sql = sql
 
     @property
     def result(self):
-        """Gets the result of this SnapshotBuilderGetConceptsResponse.  # noqa: E501
+        """Gets the result of this SnapshotBuilderConceptsResponse.  # noqa: E501
 
 
-        :return: The result of this SnapshotBuilderGetConceptsResponse.  # noqa: E501
+        :return: The result of this SnapshotBuilderConceptsResponse.  # noqa: E501
         :rtype: list[SnapshotBuilderConcept]
         """
         return self._result
 
     @result.setter
     def result(self, result):
-        """Sets the result of this SnapshotBuilderGetConceptsResponse.
+        """Sets the result of this SnapshotBuilderConceptsResponse.
 
 
-        :param result: The result of this SnapshotBuilderGetConceptsResponse.  # noqa: E501
+        :param result: The result of this SnapshotBuilderConceptsResponse.  # noqa: E501
         :type: list[SnapshotBuilderConcept]
         """
         if self.local_vars_configuration.client_side_validation and result is None:  # noqa: E501
             raise ValueError("Invalid value for `result`, must not be `None`")  # noqa: E501
 
         self._result = result
 
     @property
     def sql(self):
-        """Gets the sql of this SnapshotBuilderGetConceptsResponse.  # noqa: E501
+        """Gets the sql of this SnapshotBuilderConceptsResponse.  # noqa: E501
 
 
-        :return: The sql of this SnapshotBuilderGetConceptsResponse.  # noqa: E501
+        :return: The sql of this SnapshotBuilderConceptsResponse.  # noqa: E501
         :rtype: str
         """
         return self._sql
 
     @sql.setter
     def sql(self, sql):
-        """Sets the sql of this SnapshotBuilderGetConceptsResponse.
+        """Sets the sql of this SnapshotBuilderConceptsResponse.
 
 
-        :param sql: The sql of this SnapshotBuilderGetConceptsResponse.  # noqa: E501
+        :param sql: The sql of this SnapshotBuilderConceptsResponse.  # noqa: E501
         :type: str
         """
 
         self._sql = sql
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -130,18 +130,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SnapshotBuilderGetConceptsResponse):
+        if not isinstance(other, SnapshotBuilderConceptsResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SnapshotBuilderGetConceptsResponse):
+        if not isinstance(other, SnapshotBuilderConceptsResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_option.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_parent_concept.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_parent_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_item.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_option.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_option.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_range_option.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_program_data_range_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_request.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_builder_settings.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_ids_and_roles_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_link_duos_dataset_response.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_patch_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_preview_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_preview_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_request_asset_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_request_contents_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_request_model_policies.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_request_query_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_request_row_id_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_row_id_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_request_row_id_table_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_request_row_id_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_retrieve_include_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_source_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/snapshot_summary_model.py` & `data-repo-client-2.62.0/data_repo_client/models/snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/sql_sort_direction_asc_default.py` & `data-repo-client-2.62.0/data_repo_client/models/sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/sql_sort_direction_desc_default.py` & `data-repo-client-2.62.0/data_repo_client/models/sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/storage_resource_model.py` & `data-repo-client-2.62.0/data_repo_client/models/storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/table_data_type.py` & `data-repo-client-2.62.0/data_repo_client/models/table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/table_model.py` & `data-repo-client-2.62.0/data_repo_client/models/table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/tag_count.py` & `data-repo-client-2.62.0/data_repo_client/models/tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/tag_count_result_model.py` & `data-repo-client-2.62.0/data_repo_client/models/tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/tag_update_request_model.py` & `data-repo-client-2.62.0/data_repo_client/models/tag_update_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/transaction_close_model.py` & `data-repo-client-2.62.0/data_repo_client/models/transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/transaction_create_model.py` & `data-repo-client-2.62.0/data_repo_client/models/transaction_create_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/transaction_model.py` & `data-repo-client-2.62.0/data_repo_client/models/transaction_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/unlock_resource_request.py` & `data-repo-client-2.62.0/data_repo_client/models/unlock_resource_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/upgrade_model.py` & `data-repo-client-2.62.0/data_repo_client/models/upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/upgrade_response_model.py` & `data-repo-client-2.62.0/data_repo_client/models/upgrade_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/user_status_info.py` & `data-repo-client-2.62.0/data_repo_client/models/user_status_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/models/workspace_policy_model.py` & `data-repo-client-2.62.0/data_repo_client/models/workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client/rest.py` & `data-repo-client-2.62.0/data_repo_client/rest.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/data_repo_client.egg-info/PKG-INFO` & `data-repo-client-2.62.0/data_repo_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-repo-client
-Version: 2.61.0
+Version: 2.62.0
 Summary: Data Repository API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: team@openapitools.org
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,Data Repository API
```

### Comparing `data-repo-client-2.61.0/data_repo_client.egg-info/SOURCES.txt` & `data-repo-client-2.62.0/data_repo_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -127,27 +127,27 @@
 data_repo_client/models/resource_policy_model.py
 data_repo_client/models/sam_policy_model.py
 data_repo_client/models/snapshot_access_request.py
 data_repo_client/models/snapshot_access_request_response.py
 data_repo_client/models/snapshot_access_request_status.py
 data_repo_client/models/snapshot_builder_cohort.py
 data_repo_client/models/snapshot_builder_concept.py
+data_repo_client/models/snapshot_builder_concepts_response.py
 data_repo_client/models/snapshot_builder_count_request.py
 data_repo_client/models/snapshot_builder_count_response.py
 data_repo_client/models/snapshot_builder_count_response_result.py
 data_repo_client/models/snapshot_builder_criteria.py
 data_repo_client/models/snapshot_builder_criteria_group.py
 data_repo_client/models/snapshot_builder_dataset_concept_set.py
 data_repo_client/models/snapshot_builder_domain_criteria.py
 data_repo_client/models/snapshot_builder_domain_criteria_all_of.py
 data_repo_client/models/snapshot_builder_domain_option.py
 data_repo_client/models/snapshot_builder_domain_option_all_of.py
 data_repo_client/models/snapshot_builder_feature_value_group.py
 data_repo_client/models/snapshot_builder_get_concept_hierarchy_response.py
-data_repo_client/models/snapshot_builder_get_concepts_response.py
 data_repo_client/models/snapshot_builder_option.py
 data_repo_client/models/snapshot_builder_parent_concept.py
 data_repo_client/models/snapshot_builder_program_data_list_criteria.py
 data_repo_client/models/snapshot_builder_program_data_list_criteria_all_of.py
 data_repo_client/models/snapshot_builder_program_data_list_item.py
 data_repo_client/models/snapshot_builder_program_data_list_option.py
 data_repo_client/models/snapshot_builder_program_data_list_option_all_of.py
@@ -307,27 +307,27 @@
 test/test_search_api.py
 test/test_snapshot_access_request.py
 test/test_snapshot_access_request_api.py
 test/test_snapshot_access_request_response.py
 test/test_snapshot_access_request_status.py
 test/test_snapshot_builder_cohort.py
 test/test_snapshot_builder_concept.py
+test/test_snapshot_builder_concepts_response.py
 test/test_snapshot_builder_count_request.py
 test/test_snapshot_builder_count_response.py
 test/test_snapshot_builder_count_response_result.py
 test/test_snapshot_builder_criteria.py
 test/test_snapshot_builder_criteria_group.py
 test/test_snapshot_builder_dataset_concept_set.py
 test/test_snapshot_builder_domain_criteria.py
 test/test_snapshot_builder_domain_criteria_all_of.py
 test/test_snapshot_builder_domain_option.py
 test/test_snapshot_builder_domain_option_all_of.py
 test/test_snapshot_builder_feature_value_group.py
 test/test_snapshot_builder_get_concept_hierarchy_response.py
-test/test_snapshot_builder_get_concepts_response.py
 test/test_snapshot_builder_option.py
 test/test_snapshot_builder_parent_concept.py
 test/test_snapshot_builder_program_data_list_criteria.py
 test/test_snapshot_builder_program_data_list_criteria_all_of.py
 test/test_snapshot_builder_program_data_list_item.py
 test/test_snapshot_builder_program_data_list_option.py
 test/test_snapshot_builder_program_data_list_option_all_of.py
```

### Comparing `data-repo-client-2.61.0/setup.py` & `data-repo-client-2.62.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "data-repo-client"
-VERSION = "2.61.0"
+VERSION = "2.62.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `data-repo-client-2.61.0/test/test_access_info_big_query_model.py` & `data-repo-client-2.62.0/test/test_access_info_big_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_access_info_big_query_model_table.py` & `data-repo-client-2.62.0/test/test_access_info_big_query_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_access_info_model.py` & `data-repo-client-2.62.0/test/test_access_info_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_access_info_parquet_model.py` & `data-repo-client-2.62.0/test/test_access_info_parquet_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_access_info_parquet_model_table.py` & `data-repo-client-2.62.0/test/test_access_info_parquet_model_table.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_add_auth_domain_response_model.py` & `data-repo-client-2.62.0/test/test_add_auth_domain_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_admin_api.py` & `data-repo-client-2.62.0/test/test_admin_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_asset_model.py` & `data-repo-client-2.62.0/test/test_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_asset_table_model.py` & `data-repo-client-2.62.0/test/test_asset_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_billing_profile_model.py` & `data-repo-client-2.62.0/test/test_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_billing_profile_request_model.py` & `data-repo-client-2.62.0/test/test_billing_profile_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_billing_profile_update_model.py` & `data-repo-client-2.62.0/test/test_billing_profile_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_bulk_load_array_request_model.py` & `data-repo-client-2.62.0/test/test_bulk_load_array_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_bulk_load_array_result_model.py` & `data-repo-client-2.62.0/test/test_bulk_load_array_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_bulk_load_file_model.py` & `data-repo-client-2.62.0/test/test_bulk_load_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_bulk_load_file_result_model.py` & `data-repo-client-2.62.0/test/test_bulk_load_file_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_bulk_load_file_state.py` & `data-repo-client-2.62.0/test/test_bulk_load_file_state.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_bulk_load_history_model.py` & `data-repo-client-2.62.0/test/test_bulk_load_history_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_bulk_load_history_model_list.py` & `data-repo-client-2.62.0/test/test_bulk_load_history_model_list.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_bulk_load_request_model.py` & `data-repo-client-2.62.0/test/test_bulk_load_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_bulk_load_result_model.py` & `data-repo-client-2.62.0/test/test_bulk_load_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_cloud_platform.py` & `data-repo-client-2.62.0/test/test_cloud_platform.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_column_model.py` & `data-repo-client-2.62.0/test/test_column_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_column_statistics_double_model.py` & `data-repo-client-2.62.0/test/test_column_statistics_double_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_column_statistics_double_model_all_of.py` & `data-repo-client-2.62.0/test/test_column_statistics_double_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_column_statistics_int_model.py` & `data-repo-client-2.62.0/test/test_column_statistics_int_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_column_statistics_int_model_all_of.py` & `data-repo-client-2.62.0/test/test_column_statistics_int_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_column_statistics_model.py` & `data-repo-client-2.62.0/test/test_column_statistics_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_column_statistics_text_model.py` & `data-repo-client-2.62.0/test/test_column_statistics_text_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_column_statistics_text_model_all_of.py` & `data-repo-client-2.62.0/test/test_column_statistics_text_model_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_column_statistics_text_value.py` & `data-repo-client-2.62.0/test/test_column_statistics_text_value.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_config_enable_model.py` & `data-repo-client-2.62.0/test/test_config_enable_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_config_fault_counted_model.py` & `data-repo-client-2.62.0/test/test_config_fault_counted_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_config_fault_model.py` & `data-repo-client-2.62.0/test/test_config_fault_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_config_group_model.py` & `data-repo-client-2.62.0/test/test_config_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_config_list_model.py` & `data-repo-client-2.62.0/test/test_config_list_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_config_model.py` & `data-repo-client-2.62.0/test/test_config_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_config_parameter_model.py` & `data-repo-client-2.62.0/test/test_config_parameter_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_configs_api.py` & `data-repo-client-2.62.0/test/test_configs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_data_deletion_gcs_file_model.py` & `data-repo-client-2.62.0/test/test_data_deletion_gcs_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_data_deletion_json_array_model.py` & `data-repo-client-2.62.0/test/test_data_deletion_json_array_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_data_deletion_request.py` & `data-repo-client-2.62.0/test/test_data_deletion_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_data_deletion_table_model.py` & `data-repo-client-2.62.0/test/test_data_deletion_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_data_repository_service_api.py` & `data-repo-client-2.62.0/test/test_data_repository_service_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_data_model.py` & `data-repo-client-2.62.0/test/test_dataset_data_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_model.py` & `data-repo-client-2.62.0/test/test_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_patch_request_model.py` & `data-repo-client-2.62.0/test/test_dataset_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_request_access_include_model.py` & `data-repo-client-2.62.0/test/test_dataset_request_access_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_request_model.py` & `data-repo-client-2.62.0/test/test_dataset_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_request_model_policies.py` & `data-repo-client-2.62.0/test/test_dataset_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_schema_column_update_model.py` & `data-repo-client-2.62.0/test/test_dataset_schema_column_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_schema_update_model.py` & `data-repo-client-2.62.0/test/test_dataset_schema_update_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_schema_update_model_changes.py` & `data-repo-client-2.62.0/test/test_dataset_schema_update_model_changes.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_specification_model.py` & `data-repo-client-2.62.0/test/test_dataset_specification_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_dataset_summary_model.py` & `data-repo-client-2.62.0/test/test_dataset_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_datasets_api.py` & `data-repo-client-2.62.0/test/test_datasets_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,44 +102,26 @@
 
     def test_enumerate_transactions(self):
         """Test case for enumerate_transactions
 
         """
         pass
 
-    def test_get_concept_hierarchy(self):
-        """Test case for get_concept_hierarchy
-
-        """
-        pass
-
-    def test_get_concepts(self):
-        """Test case for get_concepts
-
-        """
-        pass
-
     def test_get_dataset_tags(self):
         """Test case for get_dataset_tags
 
         """
         pass
 
     def test_get_load_history_for_load_tag(self):
         """Test case for get_load_history_for_load_tag
 
         """
         pass
 
-    def test_get_snapshot_builder_count(self):
-        """Test case for get_snapshot_builder_count
-
-        """
-        pass
-
     def test_ingest_dataset(self):
         """Test case for ingest_dataset
 
         """
         pass
 
     def test_ingest_file(self):
@@ -240,20 +222,14 @@
 
     def test_retrieve_user_dataset_roles(self):
         """Test case for retrieve_user_dataset_roles
 
         """
         pass
 
-    def test_search_concepts(self):
-        """Test case for search_concepts
-
-        """
-        pass
-
     def test_unlock_dataset(self):
         """Test case for unlock_dataset
 
         """
         pass
 
     def test_update_dataset_snapshot_builder_settings(self):
```

### Comparing `data-repo-client-2.61.0/test/test_date_partition_options_model.py` & `data-repo-client-2.62.0/test/test_date_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_delete_response_model.py` & `data-repo-client-2.62.0/test/test_delete_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_directory_detail_model.py` & `data-repo-client-2.62.0/test/test_directory_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_access_method.py` & `data-repo-client-2.62.0/test/test_drs_access_method.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_access_url.py` & `data-repo-client-2.62.0/test/test_drs_access_url.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_alias_model.py` & `data-repo-client-2.62.0/test/test_drs_alias_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_authorizations.py` & `data-repo-client-2.62.0/test/test_drs_authorizations.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_checksum.py` & `data-repo-client-2.62.0/test/test_drs_checksum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_contents_object.py` & `data-repo-client-2.62.0/test/test_drs_contents_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_error.py` & `data-repo-client-2.62.0/test/test_drs_error.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_object.py` & `data-repo-client-2.62.0/test/test_drs_object.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_passport_request_model.py` & `data-repo-client-2.62.0/test/test_drs_passport_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_drs_service_info.py` & `data-repo-client-2.62.0/test/test_drs_service_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_duos_api.py` & `data-repo-client-2.62.0/test/test_duos_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_duos_firecloud_group_model.py` & `data-repo-client-2.62.0/test/test_duos_firecloud_group_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_duos_firecloud_groups_sync_response.py` & `data-repo-client-2.62.0/test/test_duos_firecloud_groups_sync_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_enumerate_billing_profile_model.py` & `data-repo-client-2.62.0/test/test_enumerate_billing_profile_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_enumerate_dataset_model.py` & `data-repo-client-2.62.0/test/test_enumerate_dataset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_enumerate_snapshot_access_request.py` & `data-repo-client-2.62.0/test/test_enumerate_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_enumerate_snapshot_model.py` & `data-repo-client-2.62.0/test/test_enumerate_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_enumerate_sort_by_param.py` & `data-repo-client-2.62.0/test/test_enumerate_sort_by_param.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_error_model.py` & `data-repo-client-2.62.0/test/test_error_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_file_detail_model.py` & `data-repo-client-2.62.0/test/test_file_detail_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_file_load_model.py` & `data-repo-client-2.62.0/test/test_file_load_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_file_model.py` & `data-repo-client-2.62.0/test/test_file_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_file_model_type.py` & `data-repo-client-2.62.0/test/test_file_model_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_iam_resource_type_enum.py` & `data-repo-client-2.62.0/test/test_iam_resource_type_enum.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_inaccessible_workspace_policy_model.py` & `data-repo-client-2.62.0/test/test_inaccessible_workspace_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_ingest_request_model.py` & `data-repo-client-2.62.0/test/test_ingest_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_ingest_response_model.py` & `data-repo-client-2.62.0/test/test_ingest_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_int_partition_options_model.py` & `data-repo-client-2.62.0/test/test_int_partition_options_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_job_model.py` & `data-repo-client-2.62.0/test/test_job_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_jobs_api.py` & `data-repo-client-2.62.0/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_journal_api.py` & `data-repo-client-2.62.0/test/test_journal_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_journal_entry_model.py` & `data-repo-client-2.62.0/test/test_journal_entry_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_policy_member_request.py` & `data-repo-client-2.62.0/test/test_policy_member_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_policy_model.py` & `data-repo-client-2.62.0/test/test_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_policy_response.py` & `data-repo-client-2.62.0/test/test_policy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_profiles_api.py` & `data-repo-client-2.62.0/test/test_profiles_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_query_column_statistics_request_model.py` & `data-repo-client-2.62.0/test/test_query_column_statistics_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_query_data_request_model.py` & `data-repo-client-2.62.0/test/test_query_data_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_register_api.py` & `data-repo-client-2.62.0/test/test_register_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_relationship_model.py` & `data-repo-client-2.62.0/test/test_relationship_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_relationship_term_model.py` & `data-repo-client-2.62.0/test/test_relationship_term_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_repository_api.py` & `data-repo-client-2.62.0/test/test_repository_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,20 @@
 
     def test_delete_snapshot_snapshot_builder_settings(self):
         """Test case for delete_snapshot_snapshot_builder_settings
 
         """
         pass
 
+    def test_enumerate_concepts(self):
+        """Test case for enumerate_concepts
+
+        """
+        pass
+
     def test_enumerate_datasets(self):
         """Test case for enumerate_datasets
 
         """
         pass
 
     def test_enumerate_jobs(self):
@@ -156,22 +162,22 @@
 
     def test_export_snapshot(self):
         """Test case for export_snapshot
 
         """
         pass
 
-    def test_get_concept_hierarchy(self):
-        """Test case for get_concept_hierarchy
+    def test_get_concept_children(self):
+        """Test case for get_concept_children
 
         """
         pass
 
-    def test_get_concepts(self):
-        """Test case for get_concepts
+    def test_get_concept_hierarchy(self):
+        """Test case for get_concept_hierarchy
 
         """
         pass
 
     def test_get_config(self):
         """Test case for get_config
 
@@ -420,20 +426,14 @@
 
     def test_retrieve_user_snapshot_roles(self):
         """Test case for retrieve_user_snapshot_roles
 
         """
         pass
 
-    def test_search_concepts(self):
-        """Test case for search_concepts
-
-        """
-        pass
-
     def test_set_config_list(self):
         """Test case for set_config_list
 
         """
         pass
 
     def test_set_fault(self):
```

### Comparing `data-repo-client-2.61.0/test/test_repository_configuration_model.py` & `data-repo-client-2.62.0/test/test_repository_configuration_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_repository_status_model.py` & `data-repo-client-2.62.0/test/test_repository_status_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_repository_status_model_systems.py` & `data-repo-client-2.62.0/test/test_repository_status_model_systems.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_resource_locks.py` & `data-repo-client-2.62.0/test/test_resource_locks.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_resource_policy_model.py` & `data-repo-client-2.62.0/test/test_resource_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_resources_api.py` & `data-repo-client-2.62.0/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_sam_policy_model.py` & `data-repo-client-2.62.0/test/test_sam_policy_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_search_api.py` & `data-repo-client-2.62.0/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_access_request.py` & `data-repo-client-2.62.0/test/test_snapshot_access_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_access_request_api.py` & `data-repo-client-2.62.0/test/test_snapshot_access_request_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_access_request_response.py` & `data-repo-client-2.62.0/test/test_snapshot_access_request_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_access_request_status.py` & `data-repo-client-2.62.0/test/test_snapshot_access_request_status.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_cohort.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_cohort.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_concept.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_count_request.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_count_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_count_response.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_count_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_count_response_result.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_count_response_result.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_criteria.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_criteria_group.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_criteria_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_dataset_concept_set.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_dataset_concept_set.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_domain_criteria.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_domain_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_domain_criteria_all_of.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_domain_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_domain_option.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_domain_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_domain_option_all_of.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_domain_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_feature_value_group.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_feature_value_group.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_get_concept_hierarchy_response.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_get_concept_hierarchy_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_get_concepts_response.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_concepts_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,57 +12,57 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import data_repo_client
-from data_repo_client.models.snapshot_builder_get_concepts_response import SnapshotBuilderGetConceptsResponse  # noqa: E501
+from data_repo_client.models.snapshot_builder_concepts_response import SnapshotBuilderConceptsResponse  # noqa: E501
 from data_repo_client.rest import ApiException
 
-class TestSnapshotBuilderGetConceptsResponse(unittest.TestCase):
-    """SnapshotBuilderGetConceptsResponse unit test stubs"""
+class TestSnapshotBuilderConceptsResponse(unittest.TestCase):
+    """SnapshotBuilderConceptsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SnapshotBuilderGetConceptsResponse
+        """Test SnapshotBuilderConceptsResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = data_repo_client.models.snapshot_builder_get_concepts_response.SnapshotBuilderGetConceptsResponse()  # noqa: E501
+        # model = data_repo_client.models.snapshot_builder_concepts_response.SnapshotBuilderConceptsResponse()  # noqa: E501
         if include_optional :
-            return SnapshotBuilderGetConceptsResponse(
+            return SnapshotBuilderConceptsResponse(
                 result = [
                     data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
                         id = 56, 
                         code = '0', 
                         name = '0', 
                         count = 56, 
                         has_children = True, )
                     ], 
                 sql = '0'
             )
         else :
-            return SnapshotBuilderGetConceptsResponse(
+            return SnapshotBuilderConceptsResponse(
                 result = [
                     data_repo_client.models.snapshot_builder_concept.SnapshotBuilderConcept(
                         id = 56, 
                         code = '0', 
                         name = '0', 
                         count = 56, 
                         has_children = True, )
                     ],
         )
 
-    def testSnapshotBuilderGetConceptsResponse(self):
-        """Test SnapshotBuilderGetConceptsResponse"""
+    def testSnapshotBuilderConceptsResponse(self):
+        """Test SnapshotBuilderConceptsResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_option.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_parent_concept.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_parent_concept.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_criteria.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_item.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_item.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_option.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_list_option_all_of.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_list_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_option.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_option_all_of.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_range_criteria.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_criteria.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_criteria_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_range_option.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_option.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_program_data_range_option_all_of.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_program_data_range_option_all_of.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_request.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_builder_settings.py` & `data-repo-client-2.62.0/test/test_snapshot_builder_settings.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_export_response_model.py` & `data-repo-client-2.62.0/test/test_snapshot_export_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_export_response_model_format.py` & `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_export_response_model_format_parquet.py` & `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_export_response_model_format_parquet_location.py` & `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet_location.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py` & `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_parquet_location_tables.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_export_response_model_format_workspace.py` & `data-repo-client-2.62.0/test/test_snapshot_export_response_model_format_workspace.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_ids_and_roles_model.py` & `data-repo-client-2.62.0/test/test_snapshot_ids_and_roles_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_link_duos_dataset_response.py` & `data-repo-client-2.62.0/test/test_snapshot_link_duos_dataset_response.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_model.py` & `data-repo-client-2.62.0/test/test_snapshot_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_patch_request_model.py` & `data-repo-client-2.62.0/test/test_snapshot_patch_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_preview_model.py` & `data-repo-client-2.62.0/test/test_snapshot_preview_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_request_asset_model.py` & `data-repo-client-2.62.0/test/test_snapshot_request_asset_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_request_contents_model.py` & `data-repo-client-2.62.0/test/test_snapshot_request_contents_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_request_model.py` & `data-repo-client-2.62.0/test/test_snapshot_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_request_model_policies.py` & `data-repo-client-2.62.0/test/test_snapshot_request_model_policies.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_request_query_model.py` & `data-repo-client-2.62.0/test/test_snapshot_request_query_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_request_row_id_model.py` & `data-repo-client-2.62.0/test/test_snapshot_request_row_id_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_request_row_id_table_model.py` & `data-repo-client-2.62.0/test/test_snapshot_request_row_id_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_retrieve_include_model.py` & `data-repo-client-2.62.0/test/test_snapshot_retrieve_include_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_source_model.py` & `data-repo-client-2.62.0/test/test_snapshot_source_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshot_summary_model.py` & `data-repo-client-2.62.0/test/test_snapshot_summary_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_snapshots_api.py` & `data-repo-client-2.62.0/test/test_snapshots_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,26 +60,50 @@
 
     def test_delete_snapshot_snapshot_builder_settings(self):
         """Test case for delete_snapshot_snapshot_builder_settings
 
         """
         pass
 
+    def test_enumerate_concepts(self):
+        """Test case for enumerate_concepts
+
+        """
+        pass
+
     def test_enumerate_snapshots(self):
         """Test case for enumerate_snapshots
 
         """
         pass
 
     def test_export_snapshot(self):
         """Test case for export_snapshot
 
         """
         pass
 
+    def test_get_concept_children(self):
+        """Test case for get_concept_children
+
+        """
+        pass
+
+    def test_get_concept_hierarchy(self):
+        """Test case for get_concept_hierarchy
+
+        """
+        pass
+
+    def test_get_snapshot_builder_count(self):
+        """Test case for get_snapshot_builder_count
+
+        """
+        pass
+
     def test_get_snapshot_ids_and_roles(self):
         """Test case for get_snapshot_ids_and_roles
 
         """
         pass
 
     def test_get_snapshot_snapshot_builder_settings(self):
```

### Comparing `data-repo-client-2.61.0/test/test_sql_sort_direction_asc_default.py` & `data-repo-client-2.62.0/test/test_sql_sort_direction_asc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_sql_sort_direction_desc_default.py` & `data-repo-client-2.62.0/test/test_sql_sort_direction_desc_default.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_storage_resource_model.py` & `data-repo-client-2.62.0/test/test_storage_resource_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_table_data_type.py` & `data-repo-client-2.62.0/test/test_table_data_type.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_table_model.py` & `data-repo-client-2.62.0/test/test_table_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_tag_count.py` & `data-repo-client-2.62.0/test/test_tag_count.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_tag_count_result_model.py` & `data-repo-client-2.62.0/test/test_tag_count_result_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_tag_update_request_model.py` & `data-repo-client-2.62.0/test/test_tag_update_request_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_transaction_close_model.py` & `data-repo-client-2.62.0/test/test_transaction_close_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_transaction_create_model.py` & `data-repo-client-2.62.0/test/test_transaction_create_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_transaction_model.py` & `data-repo-client-2.62.0/test/test_transaction_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_unauthenticated_api.py` & `data-repo-client-2.62.0/test/test_unauthenticated_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_unlock_resource_request.py` & `data-repo-client-2.62.0/test/test_unlock_resource_request.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_upgrade_api.py` & `data-repo-client-2.62.0/test/test_upgrade_api.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_upgrade_model.py` & `data-repo-client-2.62.0/test/test_upgrade_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_upgrade_response_model.py` & `data-repo-client-2.62.0/test/test_upgrade_response_model.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_user_status_info.py` & `data-repo-client-2.62.0/test/test_user_status_info.py`

 * *Files identical despite different names*

### Comparing `data-repo-client-2.61.0/test/test_workspace_policy_model.py` & `data-repo-client-2.62.0/test/test_workspace_policy_model.py`

 * *Files identical despite different names*


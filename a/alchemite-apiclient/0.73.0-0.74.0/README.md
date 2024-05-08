# Comparing `tmp/alchemite_apiclient-0.73.0.tar.gz` & `tmp/alchemite_apiclient-0.74.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemite_apiclient-0.73.0.tar", last modified: Wed Apr 10 11:05:58 2024, max compression
+gzip compressed data, was "alchemite_apiclient-0.74.0.tar", last modified: Wed May  8 19:07:32 2024, max compression
```

## Comparing `alchemite_apiclient-0.73.0.tar` & `alchemite_apiclient-0.74.0.tar`

### file list

```diff
@@ -1,749 +1,781 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.890305 alchemite_apiclient-0.73.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5104 2024-04-10 11:05:58.890305 alchemite_apiclient-0.73.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4232 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.790305 alchemite_apiclient-0.73.0/alchemite_apiclient/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25777 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.794305 alchemite_apiclient-0.73.0/alchemite_apiclient/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   126759 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/api/datasets_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35117 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/api/default_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6830 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/api/jobs_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5113 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/api/metrics_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10397 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/api/model_dataset_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   256421 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/api/models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    49883 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/api/projects_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37920 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/api_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.794305 alchemite_apiclient-0.73.0/alchemite_apiclient/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      835 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/apis/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.794305 alchemite_apiclient-0.73.0/alchemite_apiclient/calculated_columns/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1164 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/calculated_columns/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5372 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/calculated_columns/formulae.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18983 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/calculated_columns/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17318 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5079 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16577 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/extensions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.834305 alchemite_apiclient-0.73.0/alchemite_apiclient/model/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14785 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/additive_sensitivity_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15940 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/analyse_validate_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12717 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/analyse_validate_request_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24816 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/analyse_validate_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18046 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12124 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15273 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11771 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14958 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_column_info_stats.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17149 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_model_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12994 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11411 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11432 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11554 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_batch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11605 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13897 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11120 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_response_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16516 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11587 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11749 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_value_nullable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15956 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12121 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_column_info_stats.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16944 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_model_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11999 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11280 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32185 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11519 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset1.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11564 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_calculated_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12627 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_chunk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14079 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_or_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11737 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11898 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14715 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12074 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_request_row_ids.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11619 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_request_sort.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12171 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11530 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_response_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12829 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_sharing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13782 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/datasets_metadata_filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11836 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/datasets_metadata_sort.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14166 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14730 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14585 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14493 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14338 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15173 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14716 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14627 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14486 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11971 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13085 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12788 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dimensionality_reduction_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13230 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dimensionality_reduction_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12799 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_dataset_reduction_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13100 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13072 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_job_reduction_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11829 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13254 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_model_reduction_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11806 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_one_dimension_point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12386 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_three_dimension_point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12093 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_two_dimension_point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12042 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/drpca_reduction_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13785 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/drumap_reduction_type.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12701 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/empty_categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12903 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/empty_continuous_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12586 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/error.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11911 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_all_opt_jobs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15543 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11951 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15300 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11638 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_failed_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15422 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_optimizing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11784 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15176 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11437 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_pending_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16376 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11926 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16185 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16061 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11464 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16265 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_running.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11778 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16322 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11906 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16155 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16031 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16235 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_running.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16951 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_done.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11896 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16871 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_failed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11746 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16672 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_pending.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16876 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_running.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10847 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/histogram_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11881 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/histogram_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12492 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/histogram_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10895 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/histogram_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11435 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_categorical_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12150 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_scalar_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10976 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_target_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11839 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12377 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_vector_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12686 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_vector_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13237 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/importance_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14115 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/impute_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11993 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response200.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11544 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response2001.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11970 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response2002.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11989 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response2003.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12160 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response2004.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11660 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/int_cat_arr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11709 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/job_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11416 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/load_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11473 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/max.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16052 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/metadata_optimization_job.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16802 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/metadata_suggest_additional_job.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16760 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/metadata_suggest_historic_job.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11473 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/min.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36973 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18390 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_column_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_id_stub.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12283 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11754 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_permitted_column_relationships.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11856 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12829 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_sharing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12346 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_status.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12139 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_validation_methods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11775 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12259 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17111 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/models_metadata_filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12102 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/models_metadata_sort.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14076 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11795 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14640 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12340 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11409 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14495 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12142 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11451 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14403 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_product.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12061 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11607 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14248 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15083 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12869 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11581 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14626 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12265 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11958 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14537 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12178 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11981 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14354 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12723 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12307 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/non_empty_categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12381 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/non_empty_continuous_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14270 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/numerical_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16389 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/optimization_job.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17556 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/optimize_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12405 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/ot_sample_def_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12087 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/ot_sample_def_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/ot_sample_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10877 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/ot_set_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13326 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/outliers_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13599 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12854 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11980 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11919 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response_predictions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11857 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11129 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_univariate_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11449 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_dependent_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12668 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_optimize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12120 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13493 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_suggest_additional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13473 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_suggest_historic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14119 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_suggest_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12410 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_suggest_initial_sharing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11353 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_new_columns.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13513 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11670 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_categoricals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14447 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_single_tar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13421 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13415 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14178 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/predict_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12368 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/predict_trendline_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12027 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13814 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11560 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/project_bulk_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11643 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/project_bulk_suggest_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11737 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/project_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11651 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/project_sharing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16555 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/query_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14001 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/query_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12003 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/range.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12844 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10940 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_categorical_column_values.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16961 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_composition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15367 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_composition_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12213 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_continuous.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14847 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_continuous_with_start.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12546 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_discrete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_integer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11515 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_start_prop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12389 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_weighted_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10958 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11402 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/scalar_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11456 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/scalar_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13369 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/sensitivity_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10871 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/set_inputs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11163 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/share_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12251 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/si_sample_def_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/si_sample_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11669 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/string_cat_arr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17287 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_job.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15050 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_metadata_filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11959 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_metadata_sort.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23791 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_parameters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19951 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12048 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24667 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11828 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_request_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11971 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17213 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_job.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13065 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_parameters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15809 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12283 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13828 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_result_samples.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12307 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_job_patch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12045 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_parameters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15230 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12028 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_request_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17939 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11962 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13582 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19333 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11439 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_data_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19913 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_dataset_id.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12068 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21491 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_imputed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13609 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23011 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11525 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14071 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_specific.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17234 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_above_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17234 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_below_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17461 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11507 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_between_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17978 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_exclude_categories.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11673 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17970 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_include_categories.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16619 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11624 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16767 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10952 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/target_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25364 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/train_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11431 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/training_dataset_outliers_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11711 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/training_validation_prediction_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14141 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/validate_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12755 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/validation_split.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12353 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/vector_prediction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12341 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/vector_result.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12338 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/vector_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model/version_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    82086 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/model_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.834305 alchemite_apiclient-0.73.0/alchemite_apiclient/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24834 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14208 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/alchemite_apiclient/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.890305 alchemite_apiclient-0.73.0/alchemite_apiclient.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5104 2024-04-10 11:05:58.000000 alchemite_apiclient-0.73.0/alchemite_apiclient.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28693 2024-04-10 11:05:58.000000 alchemite_apiclient-0.73.0/alchemite_apiclient.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-10 11:05:58.000000 alchemite_apiclient-0.73.0/alchemite_apiclient.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2024-04-10 11:05:58.000000 alchemite_apiclient-0.73.0/alchemite_apiclient.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2024-04-10 11:05:58.000000 alchemite_apiclient-0.73.0/alchemite_apiclient.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.878305 alchemite_apiclient-0.73.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/AbsoluteValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Addition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/AdditiveSensitivityRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1477 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/AnalyseValidateRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1123 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/AnalyseValidateRequestAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5720 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/AnalyseValidateResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2764 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/AnalyseValidateResponseColumnAnalytics.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1313 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColBooleanExpression.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColBooleanLiteral.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      884 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColComparison.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColConstant.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2969 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColExpression.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColIf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColLiteral.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColLogicalCombination.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2296 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColNumericOperation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      595 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CalColReference.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      797 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      990 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CategoricalColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CategoricalColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      959 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CategoricalColumnInfoStats.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1817 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CategoricalModelColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CategoricalModelColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CategoricalPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/CategoricalResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ColumnGroupBatchRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      720 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ColumnGroupPatchRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      600 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ColumnGroupRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ColumnGroupResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      545 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ColumnGroupResponseAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1690 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      624 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ColumnValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ColumnValueNullable.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ContinuousColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      690 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ContinuousColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ContinuousColumnInfoStats.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1656 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ContinuousModelColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ContinuousModelColumnInfoAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Cosine.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      802 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRDatasetReductionData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRDatasetReductionMetadata.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRDatasetReductionMetadataSources.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1038 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRJobReductionMetadata.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      725 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRJobReductionMetadataSources.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1016 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRModelReductionData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DROneDimensionPoint.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRPCAReductionType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRThreeDimensionPoint.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRTwoDimensionPoint.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DRUMAPReductionType.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      578 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Data.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8810 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Dataset.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Dataset1.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      611 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetCalculatedColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetChunk.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetOrData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      530 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetQuery.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1507 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetQueryRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      855 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetQueryRequestRowIDs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetQueryRequestSort.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetQueryResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetQueryResponseResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetSharing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    71423 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1260 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetsMetadataFilters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      605 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DatasetsMetadataSort.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18645 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DefaultApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      791 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgCol.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgColWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgConstantSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      731 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgProduct.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      737 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1190 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgSummandsWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      772 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgWeightedConstSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      756 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgWeightedRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgZeroIfZero.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      661 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColFnArgZeroIfZeroAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DependentColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DimensionalityReductionRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/DimensionalityReductionResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Division.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      881 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/EmptyCategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1021 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/EmptyContinuousColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Equal.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Error.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Exponentiation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetAllOptJobs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1025 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetOptimizeDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      630 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetOptimizeDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetOptimizeFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetOptimizeFailedAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetOptimizeOptimizing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetOptimizeOptimizingAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetOptimizePending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetOptimizePendingAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalFailedAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalPending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalPendingAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalRunning.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalRunningAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestHistoricDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestHistoricDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1169 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestHistoricFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1144 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestHistoricPending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1186 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestHistoricRunning.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestInitialDone.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestInitialDoneAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1351 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestInitialFailed.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestInitialFailedAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1282 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestInitialPending.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1324 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GetSuggestInitialRunning.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Greater.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/GreaterOrEqual.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      447 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistogramCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistogramContinuous.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      991 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistogramRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistogramResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistoricCategoricalPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistoricPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistoricScalarPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistoricTargetFunction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistoricValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistoricVectorPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HistoricVectorValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HyperbolicCosine.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HyperbolicSine.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/HyperbolicTangent.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ImportanceRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1583 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ImputeRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InlineResponse200.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InlineResponse2001.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InlineResponse2002.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      764 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InlineResponse2003.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InlineResponse2004.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/IntCatArr.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InverseCosine.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      535 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InverseHyperbolicCosine.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InverseHyperbolicSine.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InverseHyperbolicTangent.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      522 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InverseSine.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/InverseTangent.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/JobPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4443 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/JobsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Less.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/LessOrEqual.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/LoadRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Logarithm.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Max.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Maximum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Mean.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1177 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/MetadataOptimizationJob.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1369 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/MetadataSuggestAdditionalJob.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/MetadataSuggestHistoricJob.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/MetricsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Min.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Minimum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8785 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Model.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelAnd.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2517 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelColumnInfo.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5231 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelDatasetApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      363 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelIDStub.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelNot.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelOr.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelPermittedColumnRelationships.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelQuery.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelSharing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelStatus.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelValidationMethods.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)   156364 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelsIdAdditiveSensitivityOrigin.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelsIdTrainPermittedColumnRelationships.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2342 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelsMetadataFilters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/ModelsMetadataSort.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/Multiplication.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      773 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgCol.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      679 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgColAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      953 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgColWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgColWeightsAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgColWeightsAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgConstantSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgConstantSumAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgConstantSumAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgProduct.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgProductAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgProductAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      719 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgRatioAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgSummandsWeights.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgSummandsWeightsAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      754 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedConstSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedConstSumAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      698 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      738 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedRatio.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedRatioAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedRatioAllOfArguments.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgZeroIfZero.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColFnArgZeroIfZeroAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NewColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      770 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NonEmptyCategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      843 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NonEmptyContinuousColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      777 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NonEmptyIntegerCategoricalColumn.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NotEqual.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/NumericalFilter.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1254 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/OTSampleDefCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/OTSampleDefContinuous.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/OTSampleDefinition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      494 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/OTSetInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1244 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/OptimizationJob.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2987 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/OptimizeRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2024-04-10 11:05:52.000000 alchemite_apiclient-0.73.0/docs/OutliersRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/OutputToleranceRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/OutputToleranceResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/OutputToleranceResponseFixedInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/OutputToleranceResponsePredictedOutputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/OutputToleranceResponsePredictions.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      741 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/OutputToleranceResponseSampledInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/OutputToleranceUnivariateResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartDependentColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartGetOptimize.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartGetOptimizeDoneResultArray.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1099 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartGetSuggestAdditional.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartGetSuggestHistoric.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartGetSuggestInitial.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      900 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartGetSuggestInitialSharing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartNewColumns.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartTarFnAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartTarFnBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartTarFnBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartTarFnCategoricals.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1979 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartTarFnSingleTar.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartTarFnSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PartTarFnWeightedSum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PredictRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      778 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/PredictTrendlineRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/Prediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/Product.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1086 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/Project.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ProjectBulkModel.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      550 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ProjectBulkSuggestInitial.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ProjectPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ProjectSharing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26229 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ProjectsApi.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/QueryRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/QueryResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      711 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/Range.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SISampleDefCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SISampleDefinition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefCategoricalColumnValues.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2029 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefComposition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefCompositionAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefContinuous.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefContinuousWithStart.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefDiscrete.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefInteger.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefStartProp.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefWeightedCategorical.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SampleDefinition.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ScalarPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ScalarResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SensitivityRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SetInputs.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ShareGroup.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/Sine.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SquareRoot.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/StringCatArr.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/Subtraction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1436 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestAdditionalJob.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1742 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestAdditionalMetadataFilters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestAdditionalMetadataSort.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4837 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestAdditionalParameters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3870 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestAdditionalParametersAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      587 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestAdditionalQuery.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestAdditionalRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestAdditionalRequestAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestAdditionalResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestHistoricJob.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1050 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestHistoricParameters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestHistoricRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      922 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestHistoricResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1358 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestHistoricResultSamples.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      791 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestInitialJobPatch.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestInitialParameters.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestInitialRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      782 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestInitialRequestAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1611 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestInitialResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      393 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestInitialResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingCommon.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2955 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingDataAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3155 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingDatasetID.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      848 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingDatasetIDAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4011 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingImputedData.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingImputedDataAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4589 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      646 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingResponse.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/SuggestMissingSpecific.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/Sum.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/Tangent.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnAboveAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnBelowAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2175 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnBetweenAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2237 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnExcludeCategories.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      612 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnExcludeCategoriesAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2233 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnIncludeCategories.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnIncludeCategoriesAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnSumAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnSumAboveAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnSumBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnSumBelowAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1828 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnSumBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnSumBetweenAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnWeightedSumAbove.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnWeightedSumAboveAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnWeightedSumBelow.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnWeightedSumBelowAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1835 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnWeightedSumBetween.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TarFnWeightedSumBetweenAllOf.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TargetFunction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6402 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TrainRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TrainingDatasetOutliersRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/TrainingValidationPredictionRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1595 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ValidateRequest.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1096 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/ValidationSplit.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/Value.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/VectorPrediction.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/VectorResult.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/VectorValue.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/docs/VersionResponse.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.886305 alchemite_apiclient-0.73.0/example/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   701201 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/adrenergic.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)   243835 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/adrenergic_holdout.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1654 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/adrenergic_row.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/categorical.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/credentials_auth_code_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/credentials_client_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/credentials_pass_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/credentials_pass_prompted_SAMPLE.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4720 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_additive_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4364 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4479 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_calculated.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3943 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2968 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_chunk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4295 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_column_groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      710 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_connect.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5944 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_custom_validation_splits.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5809 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_dimensionality_reduction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      969 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_download.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3608 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_histogram.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4378 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_hyperopt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3996 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_importance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4002 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_metadata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5573 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_optimize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3322 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4949 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_output_tolerance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4910 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_predict_trendline.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4664 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_preload.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4325 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_project.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4229 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3998 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4667 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5510 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_suggest_additional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5546 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_suggest_historic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1979 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_suggest_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4597 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_suggest_missing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3594 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_training_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5292 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_validate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3595 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_validation_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5496 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/example_vector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      759 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/optimize_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/optimize_args_vector.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1290 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/optimize_dependentColumns_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/steels.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/steels_impute.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      854 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/suggest_additional_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/suggest_additional_args_vector.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/suggest_historic_args_steel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/suggest_historic_args_vector.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/suggest_initial_args.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      503 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/example/vector.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-10 11:05:58.890305 alchemite_apiclient-0.73.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1178 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-10 11:05:58.890305 alchemite_apiclient-0.73.0/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_additive_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2591 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2506 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_categorical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10206 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_cce.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1985 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_chunk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2873 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_column_groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_connect.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2255 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_cornercases.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3803 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_custom_validation_splits.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2493 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_dimensionality_reduction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_download.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4072 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_examples.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3634 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_formulae.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_hyperopt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      932 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_importance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_optimize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1848 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_output_tolerance.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1223 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_preload.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_query.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1611 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_sensitivity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_suggest_additional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1152 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_suggest_historic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_suggest_initial.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_suggest_missing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_training_outliers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      833 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_validate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2431 2024-04-10 11:05:53.000000 alchemite_apiclient-0.73.0/test/test_vector.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.927271 alchemite_apiclient-0.74.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5104 2024-05-08 19:07:32.927271 alchemite_apiclient-0.74.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4232 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.783270 alchemite_apiclient-0.74.0/alchemite_apiclient/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27228 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.787270 alchemite_apiclient-0.74.0/alchemite_apiclient/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   126759 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/api/datasets_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35117 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/api/default_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12592 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/api/jobs_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5113 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/api/metrics_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10397 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/api/model_dataset_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   256421 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/api/models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    49883 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/api/projects_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    37920 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/api_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.787270 alchemite_apiclient-0.74.0/alchemite_apiclient/apis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      835 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/apis/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.787270 alchemite_apiclient-0.74.0/alchemite_apiclient/calculated_columns/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1164 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/calculated_columns/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5372 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/calculated_columns/formulae.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18983 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/calculated_columns/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17318 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5079 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16577 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/extensions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.839270 alchemite_apiclient-0.74.0/alchemite_apiclient/model/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14785 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/additive_sensitivity_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15940 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/analyse_validate_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12717 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/analyse_validate_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24816 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/analyse_validate_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18046 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12124 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15273 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11771 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14958 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_column_info_stats.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17149 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_model_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12994 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11411 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11432 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11554 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_batch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11605 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13897 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11120 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_response_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16516 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11587 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11749 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_value_nullable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17661 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/consistent_optimization_job.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15956 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12121 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_column_info_stats.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16944 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_model_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11999 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11280 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32185 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11519 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset1.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11564 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_calculated_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12627 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_chunk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14079 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_or_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11737 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11898 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14715 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12074 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_request_row_ids.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11619 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_request_sort.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12171 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11530 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_response_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12829 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_sharing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13782 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/datasets_metadata_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11836 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/datasets_metadata_sort.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14166 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14730 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14585 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14493 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14338 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15173 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14716 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14627 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14486 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11971 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13085 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12788 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dimensionality_reduction_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13230 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dimensionality_reduction_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12799 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_dataset_reduction_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13100 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13072 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_job_reduction_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11829 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13254 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_model_reduction_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11806 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_one_dimension_point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12386 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_three_dimension_point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12093 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_two_dimension_point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12042 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/drpca_reduction_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13785 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/drumap_reduction_type.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12701 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/empty_categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12903 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/empty_continuous_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12586 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/error.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11911 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_all_opt_jobs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15543 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11951 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16514 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_done_consistent.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15300 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11638 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_failed_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16271 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_failed_consistent.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15422 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_optimizing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11784 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16393 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_optimizing_consistent.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15176 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11437 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_pending_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16147 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_pending_consistent.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16376 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11926 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16185 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16061 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11464 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16265 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_running.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11778 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16443 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_historic_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11906 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16276 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_historic_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16152 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_historic_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16356 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_historic_running.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16951 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_done.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11896 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16871 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_failed.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11746 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16672 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_pending.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16876 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_running.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10847 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/histogram_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11881 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/histogram_continuous.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12492 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/histogram_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10895 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/histogram_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11435 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_categorical_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12150 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11426 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_scalar_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10976 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_target_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11839 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12377 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_vector_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12686 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_vector_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13237 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/importance_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14115 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/impute_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11993 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response200.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11544 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response2001.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11970 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response2002.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11989 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response2003.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12182 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response2004.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12549 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response2005.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11660 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/int_cat_arr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11709 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/job_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12353 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/job_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15205 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/jobs_metadata_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12106 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/jobs_metadata_sort.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11416 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/load_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11473 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/max.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17339 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_optimization_job.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11432 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_optimization_job_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17420 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_suggest_additional_job.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11527 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_suggest_additional_job_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16811 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_suggest_additional_job_old.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17285 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_suggest_historic_job.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11505 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_suggest_historic_job_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11473 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/min.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36973 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18390 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_column_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_id_stub.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12283 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11754 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_permitted_column_relationships.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11856 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12829 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_sharing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12346 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_status.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12139 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_validation_methods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11775 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12259 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17111 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/models_metadata_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12102 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/models_metadata_sort.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14076 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11795 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14640 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12340 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11409 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14495 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12142 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11451 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14403 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_product.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12061 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11607 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14248 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15083 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12869 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11581 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14626 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12265 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11958 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14537 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12178 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11981 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14354 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11941 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12723 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12307 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/non_empty_categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12381 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/non_empty_continuous_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14270 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/numerical_filter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16389 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/optimization_job.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16606 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/optimize_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18970 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/optimize_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11863 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/optimize_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12405 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/ot_sample_def_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12087 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/ot_sample_def_continuous.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/ot_sample_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10877 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/ot_set_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13326 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/outliers_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13599 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12854 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11980 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11919 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response_predictions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11857 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11129 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_univariate_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11449 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_dependent_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12668 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_optimize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13570 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_optimize_consistent.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12120 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13493 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_suggest_additional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13544 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_suggest_historic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14119 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_suggest_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12410 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_suggest_initial_sharing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11353 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_new_columns.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11145 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13513 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11670 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_categoricals.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14447 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_single_tar.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13421 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13415 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14178 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/predict_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12368 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/predict_trendline_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12027 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13814 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11560 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/project_bulk_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11643 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/project_bulk_suggest_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11737 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/project_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11651 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/project_sharing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16555 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/query_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14001 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/query_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12003 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/range.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12844 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10940 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_categorical_column_values.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16961 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_composition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15367 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_composition_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12213 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_continuous.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14847 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_continuous_with_start.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12546 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_discrete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12344 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_integer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11515 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_start_prop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12389 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_weighted_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10958 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11402 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/scalar_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11456 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/scalar_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13369 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/sensitivity_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10871 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/set_inputs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11163 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/share_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12251 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/si_sample_def_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10964 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/si_sample_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11669 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/string_cat_arr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17287 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_job.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15050 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_metadata_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11959 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_metadata_sort.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23791 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19951 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12048 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24667 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11828 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11971 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17490 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_job.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13065 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15809 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12283 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13828 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_result_samples.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12307 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_job_patch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12045 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_parameters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15230 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12028 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_request_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17939 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11962 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13582 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19333 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11439 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_data_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19913 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_dataset_id.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12068 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21491 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_imputed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13609 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23011 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11525 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14071 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_specific.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17234 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_above_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17234 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11445 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_below_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17461 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11507 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_between_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17978 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_exclude_categories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11673 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17970 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_include_categories.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11665 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16392 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11562 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16619 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11624 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16540 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11676 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16767 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11738 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10952 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/target_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25364 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/train_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11431 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/training_dataset_outliers_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11711 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/training_validation_prediction_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14141 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/validate_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12755 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/validation_split.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12353 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/vector_prediction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12341 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/vector_result.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12338 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/vector_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12328 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model/version_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    82086 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/model_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.839270 alchemite_apiclient-0.74.0/alchemite_apiclient/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26285 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14208 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/alchemite_apiclient/rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.927271 alchemite_apiclient-0.74.0/alchemite_apiclient.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5104 2024-05-08 19:07:32.000000 alchemite_apiclient-0.74.0/alchemite_apiclient.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30128 2024-05-08 19:07:32.000000 alchemite_apiclient-0.74.0/alchemite_apiclient.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-08 19:07:32.000000 alchemite_apiclient-0.74.0/alchemite_apiclient.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2024-05-08 19:07:32.000000 alchemite_apiclient-0.74.0/alchemite_apiclient.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2024-05-08 19:07:32.000000 alchemite_apiclient-0.74.0/alchemite_apiclient.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.907271 alchemite_apiclient-0.74.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/AbsoluteValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Addition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/AdditiveSensitivityRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1477 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/AnalyseValidateRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1123 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/AnalyseValidateRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5720 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/AnalyseValidateResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2764 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/AnalyseValidateResponseColumnAnalytics.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1313 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColBooleanExpression.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColBooleanLiteral.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      884 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColComparison.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColConstant.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2969 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColExpression.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColIf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColLiteral.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColLogicalCombination.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2296 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColNumericOperation.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      595 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CalColReference.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      797 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      990 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CategoricalColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CategoricalColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      959 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CategoricalColumnInfoStats.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1817 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CategoricalModelColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CategoricalModelColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      529 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CategoricalPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/CategoricalResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      547 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ColumnGroupBatchRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      720 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ColumnGroupPatchRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      600 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ColumnGroupRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ColumnGroupResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      545 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ColumnGroupResponseAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1690 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      624 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ColumnValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ColumnValueNullable.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1550 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ConsistentOptimizationJob.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ContinuousColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      690 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ContinuousColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ContinuousColumnInfoStats.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1656 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ContinuousModelColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      892 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ContinuousModelColumnInfoAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Cosine.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      802 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRDatasetReductionData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      963 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRDatasetReductionMetadata.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRDatasetReductionMetadataSources.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1038 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRJobReductionMetadata.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      725 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRJobReductionMetadataSources.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1016 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRModelReductionData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DROneDimensionPoint.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      546 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRPCAReductionType.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRThreeDimensionPoint.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRTwoDimensionPoint.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1155 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DRUMAPReductionType.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      578 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Data.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8810 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Dataset.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Dataset1.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      611 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetCalculatedColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetChunk.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetOrData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      530 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetQuery.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1507 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetQueryRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      855 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetQueryRequestRowIDs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetQueryRequestSort.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetQueryResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetQueryResponseResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetSharing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    71423 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1260 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetsMetadataFilters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      605 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DatasetsMetadataSort.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18645 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DefaultApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      791 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgCol.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      971 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgColWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      748 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgConstantSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      731 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgProduct.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      737 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1190 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgSummandsWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      772 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgWeightedConstSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      756 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgWeightedRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgZeroIfZero.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      661 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColFnArgZeroIfZeroAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DependentColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DimensionalityReductionRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/DimensionalityReductionResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Division.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      881 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/EmptyCategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1021 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/EmptyContinuousColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Equal.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Error.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Exponentiation.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetAllOptJobs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1025 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizeDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      630 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizeDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1331 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizeDoneConsistent.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      965 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizeFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizeFailedAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1271 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizeFailedConsistent.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizeOptimizing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizeOptimizingAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1294 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizeOptimizingConsistent.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizePending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizePendingAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1246 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetOptimizePendingConsistent.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1175 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalFailedAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalPending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalPendingAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1192 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalRunning.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalRunningAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1291 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestHistoricDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestHistoricDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1249 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestHistoricFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestHistoricPending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1266 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestHistoricRunning.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1347 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestInitialDone.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestInitialDoneAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1351 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestInitialFailed.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestInitialFailedAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1282 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestInitialPending.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1324 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GetSuggestInitialRunning.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Greater.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/GreaterOrEqual.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      447 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistogramCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistogramContinuous.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      991 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistogramRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistogramResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistoricCategoricalPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistoricPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistoricScalarPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      700 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistoricTargetFunction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistoricValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistoricVectorPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HistoricVectorValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HyperbolicCosine.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HyperbolicSine.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/HyperbolicTangent.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ImportanceRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1583 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ImputeRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InlineResponse200.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InlineResponse2001.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InlineResponse2002.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      764 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InlineResponse2003.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      832 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InlineResponse2004.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      804 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InlineResponse2005.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      316 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/IntCatArr.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InverseCosine.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      535 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InverseHyperbolicCosine.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InverseHyperbolicSine.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InverseHyperbolicTangent.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      522 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InverseSine.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/InverseTangent.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/JobPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/JobQuery.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8591 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/JobsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1907 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/JobsMetadataFilters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/JobsMetadataSort.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Less.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/LessOrEqual.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/LoadRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Logarithm.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Max.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Maximum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Mean.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1520 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/MetadataOptimizationJob.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/MetadataOptimizationJobAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/MetadataSuggestAdditionalJob.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      538 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/MetadataSuggestAdditionalJobAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1372 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/MetadataSuggestAdditionalJobOld.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/MetadataSuggestHistoricJob.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      534 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/MetadataSuggestHistoricJobAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/MetricsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Min.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Minimum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8785 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Model.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelAnd.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2517 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelColumnInfo.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5231 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelDatasetApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      363 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelIDStub.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelNot.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelOr.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelPermittedColumnRelationships.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      507 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelQuery.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelSharing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelStatus.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelValidationMethods.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   155824 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelsIdAdditiveSensitivityOrigin.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelsIdTrainPermittedColumnRelationships.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2342 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelsMetadataFilters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ModelsMetadataSort.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Multiplication.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      773 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgCol.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      679 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgColAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      953 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgColWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgColWeightsAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgColWeightsAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      730 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgConstantSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      636 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgConstantSumAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      599 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgConstantSumAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgProduct.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgProductAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgProductAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      719 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgRatioAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgSummandsWeights.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgSummandsWeightsAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      754 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedConstSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      660 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedConstSumAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      698 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      738 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedRatio.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedRatioAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      852 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedRatioAllOfArguments.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgZeroIfZero.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColFnArgZeroIfZeroAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NewColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      770 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NonEmptyCategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      843 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NonEmptyContinuousColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      777 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NonEmptyIntegerCategoricalColumn.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NotEqual.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/NumericalFilter.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1254 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OTSampleDefCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OTSampleDefContinuous.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OTSampleDefinition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      494 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OTSetInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1244 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OptimizationJob.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2694 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OptimizeParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2987 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OptimizeRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      764 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OptimizeRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OutliersRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OutputToleranceRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      644 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OutputToleranceResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      809 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OutputToleranceResponseFixedInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OutputToleranceResponsePredictedOutputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OutputToleranceResponsePredictions.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      741 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OutputToleranceResponseSampledInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/OutputToleranceUnivariateResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartDependentColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      889 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartGetOptimize.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartGetOptimizeConsistent.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartGetOptimizeDoneResultArray.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1099 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartGetSuggestAdditional.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1173 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartGetSuggestHistoric.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartGetSuggestInitial.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      900 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartGetSuggestInitialSharing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartNewColumns.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartTarFnAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartTarFnBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartTarFnBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      586 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartTarFnCategoricals.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1979 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartTarFnSingleTar.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartTarFnSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PartTarFnWeightedSum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PredictRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      778 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/PredictTrendlineRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      590 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Prediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Product.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1086 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Project.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ProjectBulkModel.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      550 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ProjectBulkSuggestInitial.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ProjectPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ProjectSharing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26229 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ProjectsApi.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/QueryRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      692 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/QueryResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      711 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Range.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      767 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SISampleDefCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SISampleDefinition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefCategoricalColumnValues.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2029 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefComposition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1933 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefCompositionAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefContinuous.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1342 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefContinuousWithStart.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      962 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefDiscrete.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefInteger.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefStartProp.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      784 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefWeightedCategorical.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      531 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SampleDefinition.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      526 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ScalarPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      653 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ScalarResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1196 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SensitivityRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SetInputs.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      512 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ShareGroup.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      514 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Sine.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      521 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SquareRoot.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/StringCatArr.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Subtraction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1436 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestAdditionalJob.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1742 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestAdditionalMetadataFilters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestAdditionalMetadataSort.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4837 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestAdditionalParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3870 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestAdditionalParametersAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      587 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestAdditionalQuery.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestAdditionalRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestAdditionalRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestAdditionalResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1506 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestHistoricJob.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1050 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestHistoricParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestHistoricRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      922 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestHistoricResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1358 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestHistoricResultSamples.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      791 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestInitialJobPatch.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestInitialParameters.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1004 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestInitialRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      782 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestInitialRequestAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1611 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestInitialResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      393 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestInitialResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1440 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingCommon.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2955 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingDataAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3155 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingDatasetID.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      848 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingDatasetIDAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4011 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingImputedData.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingImputedDataAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4589 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      646 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingResponse.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/SuggestMissingSpecific.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Sum.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Tangent.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnAboveAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2101 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      563 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnBelowAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2175 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnBetweenAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2237 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnExcludeCategories.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      612 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnExcludeCategoriesAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2233 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnIncludeCategories.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnIncludeCategoriesAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnSumAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnSumAboveAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1754 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnSumBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      608 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnSumBelowAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1828 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnSumBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      652 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnSumBetweenAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnWeightedSumAbove.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnWeightedSumAboveAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnWeightedSumBelow.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnWeightedSumBelowAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1835 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnWeightedSumBetween.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TarFnWeightedSumBetweenAllOf.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TargetFunction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6402 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TrainRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TrainingDatasetOutliersRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/TrainingValidationPredictionRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1595 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ValidateRequest.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1096 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/ValidationSplit.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/Value.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/VectorPrediction.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/VectorResult.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/VectorValue.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      945 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/docs/VersionResponse.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.919271 alchemite_apiclient-0.74.0/example/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   701201 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/adrenergic.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   243835 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/adrenergic_holdout.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1654 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/adrenergic_row.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      591 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/categorical.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/credentials_auth_code_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/credentials_client_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      167 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/credentials_pass_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/credentials_pass_prompted_SAMPLE.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4720 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_additive_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4364 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4479 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_calculated.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3943 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2968 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_chunk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4295 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_column_groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      710 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_connect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5944 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_custom_validation_splits.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5809 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_dimensionality_reduction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      969 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_download.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3608 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_histogram.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4378 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_hyperopt.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3996 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_importance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4002 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5573 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_optimize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3322 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4949 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_output_tolerance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4910 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_predict_trendline.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4664 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_preload.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4325 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_project.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4229 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3998 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4667 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5510 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_suggest_additional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5546 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_suggest_historic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1979 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_suggest_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4597 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_suggest_missing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3594 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_training_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5292 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_validate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3595 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_validation_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5496 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/example_vector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      759 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/optimize_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/optimize_args_vector.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1290 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/optimize_dependentColumns_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/steels.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/steels_impute.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      854 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/suggest_additional_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/suggest_additional_args_vector.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/suggest_historic_args_steel.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/suggest_historic_args_vector.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/suggest_initial_args.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      503 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/example/vector.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-08 19:07:32.927271 alchemite_apiclient-0.74.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1178 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-08 19:07:32.927271 alchemite_apiclient-0.74.0/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1642 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_additive_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2591 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2506 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_categorical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10206 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_cce.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1985 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_chunk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2873 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_column_groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_connect.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2255 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_cornercases.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3803 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_custom_validation_splits.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1500 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2493 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_dimensionality_reduction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_download.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4072 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_examples.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3634 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_formulae.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_hyperopt.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      932 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_importance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_optimize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1848 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_output_tolerance.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1223 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_preload.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_query.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1611 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_sensitivity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1042 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_suggest_additional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1152 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_suggest_historic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_suggest_initial.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_suggest_missing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_training_outliers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      833 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_validate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2431 2024-05-08 19:07:24.000000 alchemite_apiclient-0.74.0/test/test_vector.py
```

### Comparing `alchemite_apiclient-0.73.0/PKG-INFO` & `alchemite_apiclient-0.74.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemite_apiclient
-Version: 0.73.0
+Version: 0.74.0
 Summary: A python API client for using Alchemite Analytics
 Home-page: 
 Author: Intellegens
 Author-email: Intellegens <support@intellegens.com>
 Project-URL: Homepage, https://intellegens.com
 Project-URL: Docs, https://docs.intellegens.com
 Keywords: Alchemite,Alchemite API,Machine Learning,Artificial Intelligence
@@ -25,15 +25,15 @@
 
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.73.0
+API version: 0.74.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.73.0/README.md` & `alchemite_apiclient-0.74.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.73.0
+API version: 0.74.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/__init__.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
     Contact: support@intellegens.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.73.0"
+__version__ = "0.74.0"
 
 # import ApiClient
 from alchemite_apiclient.api_client import ApiClient
 
 # import Configuration
 from alchemite_apiclient.configuration import Configuration
 
@@ -55,14 +55,15 @@
 from alchemite_apiclient.model.column_group_patch_request import ColumnGroupPatchRequest
 from alchemite_apiclient.model.column_group_request import ColumnGroupRequest
 from alchemite_apiclient.model.column_group_response import ColumnGroupResponse
 from alchemite_apiclient.model.column_group_response_all_of import ColumnGroupResponseAllOf
 from alchemite_apiclient.model.column_info import ColumnInfo
 from alchemite_apiclient.model.column_value import ColumnValue
 from alchemite_apiclient.model.column_value_nullable import ColumnValueNullable
+from alchemite_apiclient.model.consistent_optimization_job import ConsistentOptimizationJob
 from alchemite_apiclient.model.continuous_column_info import ContinuousColumnInfo
 from alchemite_apiclient.model.continuous_column_info_all_of import ContinuousColumnInfoAllOf
 from alchemite_apiclient.model.continuous_column_info_stats import ContinuousColumnInfoStats
 from alchemite_apiclient.model.continuous_model_column_info import ContinuousModelColumnInfo
 from alchemite_apiclient.model.continuous_model_column_info_all_of import ContinuousModelColumnInfoAllOf
 from alchemite_apiclient.model.dr_dataset_reduction_data import DRDatasetReductionData
 from alchemite_apiclient.model.dr_dataset_reduction_metadata import DRDatasetReductionMetadata
@@ -106,20 +107,24 @@
 from alchemite_apiclient.model.dimensionality_reduction_response import DimensionalityReductionResponse
 from alchemite_apiclient.model.empty_categorical_column import EmptyCategoricalColumn
 from alchemite_apiclient.model.empty_continuous_column import EmptyContinuousColumn
 from alchemite_apiclient.model.error import Error
 from alchemite_apiclient.model.get_all_opt_jobs import GetAllOptJobs
 from alchemite_apiclient.model.get_optimize_done import GetOptimizeDone
 from alchemite_apiclient.model.get_optimize_done_all_of import GetOptimizeDoneAllOf
+from alchemite_apiclient.model.get_optimize_done_consistent import GetOptimizeDoneConsistent
 from alchemite_apiclient.model.get_optimize_failed import GetOptimizeFailed
 from alchemite_apiclient.model.get_optimize_failed_all_of import GetOptimizeFailedAllOf
+from alchemite_apiclient.model.get_optimize_failed_consistent import GetOptimizeFailedConsistent
 from alchemite_apiclient.model.get_optimize_optimizing import GetOptimizeOptimizing
 from alchemite_apiclient.model.get_optimize_optimizing_all_of import GetOptimizeOptimizingAllOf
+from alchemite_apiclient.model.get_optimize_optimizing_consistent import GetOptimizeOptimizingConsistent
 from alchemite_apiclient.model.get_optimize_pending import GetOptimizePending
 from alchemite_apiclient.model.get_optimize_pending_all_of import GetOptimizePendingAllOf
+from alchemite_apiclient.model.get_optimize_pending_consistent import GetOptimizePendingConsistent
 from alchemite_apiclient.model.get_suggest_additional_done import GetSuggestAdditionalDone
 from alchemite_apiclient.model.get_suggest_additional_done_all_of import GetSuggestAdditionalDoneAllOf
 from alchemite_apiclient.model.get_suggest_additional_failed import GetSuggestAdditionalFailed
 from alchemite_apiclient.model.get_suggest_additional_failed_all_of import GetSuggestAdditionalFailedAllOf
 from alchemite_apiclient.model.get_suggest_additional_pending import GetSuggestAdditionalPending
 from alchemite_apiclient.model.get_suggest_additional_pending_all_of import GetSuggestAdditionalPendingAllOf
 from alchemite_apiclient.model.get_suggest_additional_running import GetSuggestAdditionalRunning
@@ -149,21 +154,29 @@
 from alchemite_apiclient.model.importance_request import ImportanceRequest
 from alchemite_apiclient.model.impute_request import ImputeRequest
 from alchemite_apiclient.model.inline_response200 import InlineResponse200
 from alchemite_apiclient.model.inline_response2001 import InlineResponse2001
 from alchemite_apiclient.model.inline_response2002 import InlineResponse2002
 from alchemite_apiclient.model.inline_response2003 import InlineResponse2003
 from alchemite_apiclient.model.inline_response2004 import InlineResponse2004
+from alchemite_apiclient.model.inline_response2005 import InlineResponse2005
 from alchemite_apiclient.model.int_cat_arr import IntCatArr
 from alchemite_apiclient.model.job_patch import JobPatch
+from alchemite_apiclient.model.job_query import JobQuery
+from alchemite_apiclient.model.jobs_metadata_filters import JobsMetadataFilters
+from alchemite_apiclient.model.jobs_metadata_sort import JobsMetadataSort
 from alchemite_apiclient.model.load_request import LoadRequest
 from alchemite_apiclient.model.max import Max
 from alchemite_apiclient.model.metadata_optimization_job import MetadataOptimizationJob
+from alchemite_apiclient.model.metadata_optimization_job_all_of import MetadataOptimizationJobAllOf
 from alchemite_apiclient.model.metadata_suggest_additional_job import MetadataSuggestAdditionalJob
+from alchemite_apiclient.model.metadata_suggest_additional_job_all_of import MetadataSuggestAdditionalJobAllOf
+from alchemite_apiclient.model.metadata_suggest_additional_job_old import MetadataSuggestAdditionalJobOld
 from alchemite_apiclient.model.metadata_suggest_historic_job import MetadataSuggestHistoricJob
+from alchemite_apiclient.model.metadata_suggest_historic_job_all_of import MetadataSuggestHistoricJobAllOf
 from alchemite_apiclient.model.min import Min
 from alchemite_apiclient.model.model import Model
 from alchemite_apiclient.model.model_column_info import ModelColumnInfo
 from alchemite_apiclient.model.model_id_stub import ModelIDStub
 from alchemite_apiclient.model.model_patch import ModelPatch
 from alchemite_apiclient.model.model_permitted_column_relationships import ModelPermittedColumnRelationships
 from alchemite_apiclient.model.model_query import ModelQuery
@@ -204,25 +217,28 @@
 from alchemite_apiclient.model.non_empty_integer_categorical_column import NonEmptyIntegerCategoricalColumn
 from alchemite_apiclient.model.numerical_filter import NumericalFilter
 from alchemite_apiclient.model.ot_sample_def_categorical import OTSampleDefCategorical
 from alchemite_apiclient.model.ot_sample_def_continuous import OTSampleDefContinuous
 from alchemite_apiclient.model.ot_sample_definition import OTSampleDefinition
 from alchemite_apiclient.model.ot_set_inputs import OTSetInputs
 from alchemite_apiclient.model.optimization_job import OptimizationJob
+from alchemite_apiclient.model.optimize_parameters import OptimizeParameters
 from alchemite_apiclient.model.optimize_request import OptimizeRequest
+from alchemite_apiclient.model.optimize_request_all_of import OptimizeRequestAllOf
 from alchemite_apiclient.model.outliers_request import OutliersRequest
 from alchemite_apiclient.model.output_tolerance_request import OutputToleranceRequest
 from alchemite_apiclient.model.output_tolerance_response import OutputToleranceResponse
 from alchemite_apiclient.model.output_tolerance_response_fixed_inputs import OutputToleranceResponseFixedInputs
 from alchemite_apiclient.model.output_tolerance_response_predicted_outputs import OutputToleranceResponsePredictedOutputs
 from alchemite_apiclient.model.output_tolerance_response_predictions import OutputToleranceResponsePredictions
 from alchemite_apiclient.model.output_tolerance_response_sampled_inputs import OutputToleranceResponseSampledInputs
 from alchemite_apiclient.model.output_tolerance_univariate_response import OutputToleranceUnivariateResponse
 from alchemite_apiclient.model.part_dependent_columns import PartDependentColumns
 from alchemite_apiclient.model.part_get_optimize import PartGetOptimize
+from alchemite_apiclient.model.part_get_optimize_consistent import PartGetOptimizeConsistent
 from alchemite_apiclient.model.part_get_optimize_done_result_array import PartGetOptimizeDoneResultArray
 from alchemite_apiclient.model.part_get_suggest_additional import PartGetSuggestAdditional
 from alchemite_apiclient.model.part_get_suggest_historic import PartGetSuggestHistoric
 from alchemite_apiclient.model.part_get_suggest_initial import PartGetSuggestInitial
 from alchemite_apiclient.model.part_get_suggest_initial_sharing import PartGetSuggestInitialSharing
 from alchemite_apiclient.model.part_new_columns import PartNewColumns
 from alchemite_apiclient.model.part_tar_fn_above import PartTarFnAbove
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/api/datasets_api.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/api/datasets_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/api/default_api.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/api/default_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/api/metrics_api.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/api/model_dataset_api.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/api/model_dataset_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/api/models_api.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/api/models_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/api/projects_api.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/api_client.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.73.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.74.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/apis/__init__.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/calculated_columns/__init__.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/calculated_columns/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/calculated_columns/formulae.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/calculated_columns/formulae.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/calculated_columns/helpers.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/calculated_columns/helpers.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/configuration.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,16 +403,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.73.0\n"\
-               "SDK Package Version: 0.73.0".\
+               "Version of the API: 0.74.0\n"\
+               "SDK Package Version: 0.74.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/exceptions.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/extensions.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/extensions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/additive_sensitivity_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/additive_sensitivity_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/analyse_validate_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/analyse_validate_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/analyse_validate_request_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/analyse_validate_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/analyse_validate_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/analyse_validate_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/analyse_validate_response_column_analytics.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_column.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_column_info.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_column_info_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_column_info_stats.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_column_info_stats.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_model_column_info.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_model_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_prediction.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/categorical_result.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/categorical_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_batch_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_batch_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_patch_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_patch_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_group_response_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_group_response_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_info.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_value.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/column_value_nullable.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/column_value_nullable.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_column_info.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_column_info_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_column_info_stats.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_column_info_stats.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_model_column_info.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/continuous_model_column_info_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/data.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset1.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset1.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_calculated_columns.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_calculated_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_chunk.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_or_data.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_or_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_patch.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_request_row_ids.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_request_row_ids.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_request_sort.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_request_sort.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_query_response_result.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_query_response_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dataset_sharing.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dataset_sharing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/datasets_metadata_filters.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/datasets_metadata_filters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/datasets_metadata_sort.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/datasets_metadata_sort.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_col.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_col_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_constant_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_product.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_summands_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_const_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_weighted_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_col_fn_arg_zero_if_zero_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dependent_columns.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dependent_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dimensionality_reduction_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dimensionality_reduction_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dimensionality_reduction_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dimensionality_reduction_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_dataset_reduction_data.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_dataset_reduction_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_dataset_reduction_metadata.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_dataset_reduction_metadata_sources.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_job_reduction_metadata.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_job_reduction_metadata.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_job_reduction_metadata_sources.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_model_reduction_data.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_model_reduction_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_one_dimension_point.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_one_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_three_dimension_point.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_three_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/dr_two_dimension_point.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/dr_two_dimension_point.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/drpca_reduction_type.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/drpca_reduction_type.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/drumap_reduction_type.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/drumap_reduction_type.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/empty_categorical_column.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/empty_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/empty_continuous_column.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/empty_continuous_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/error.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/error.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_all_opt_jobs.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_all_opt_jobs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_done.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_done_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_failed.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_failed_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_optimizing.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_optimizing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_optimizing_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_pending.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_optimize_pending_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_pending_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_done.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_failed.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_pending.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_pending_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_running.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_running.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_additional_running_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_done.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_historic_done.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
-            'parameters': (SuggestHistoricParameters,),  # noqa: E501
+            'parameters': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'result': (SuggestHistoricResult,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
@@ -117,27 +117,28 @@
         'notes': 'notes',  # noqa: E501
         'enqueue_time': 'enqueueTime',  # noqa: E501
         'start_time': 'startTime',  # noqa: E501
         'end_time': 'endTime',  # noqa: E501
     }
 
     read_only_vars = {
+        'parameters',  # noqa: E501
         'enqueue_time',  # noqa: E501
         'start_time',  # noqa: E501
         'end_time',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """GetSuggestHistoricDone - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
-            parameters (SuggestHistoricParameters):
+            parameters (bool, date, datetime, dict, float, int, list, str, none_type): The parameters as they were given to the suggest-historic request.
             status (str): defaults to "done", must be one of ["done", ]  # noqa: E501
             result (SuggestHistoricResult):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,15 +240,14 @@
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """GetSuggestHistoricDone - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
-            parameters (SuggestHistoricParameters):
             status (str): defaults to "done", must be one of ["done", ]  # noqa: E501
             result (SuggestHistoricResult):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_historic_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_failed.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_historic_running.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.get_suggest_additional_failed_all_of import GetSuggestAdditionalFailedAllOf
+    from alchemite_apiclient.model.get_suggest_additional_running_all_of import GetSuggestAdditionalRunningAllOf
     from alchemite_apiclient.model.part_get_suggest_historic import PartGetSuggestHistoric
     from alchemite_apiclient.model.suggest_historic_parameters import SuggestHistoricParameters
-    globals()['GetSuggestAdditionalFailedAllOf'] = GetSuggestAdditionalFailedAllOf
+    globals()['GetSuggestAdditionalRunningAllOf'] = GetSuggestAdditionalRunningAllOf
     globals()['PartGetSuggestHistoric'] = PartGetSuggestHistoric
     globals()['SuggestHistoricParameters'] = SuggestHistoricParameters
 
 
-class GetSuggestHistoricFailed(ModelComposed):
+class GetSuggestHistoricRunning(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,59 +85,59 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
-            'parameters': (SuggestHistoricParameters,),  # noqa: E501
+            'parameters': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'status': (str,),  # noqa: E501
-            'detail': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
             'end_time': (int,),  # noqa: E501
+            'progress': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
         'status': 'status',  # noqa: E501
-        'detail': 'detail',  # noqa: E501
         'name': 'name',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'notes': 'notes',  # noqa: E501
         'enqueue_time': 'enqueueTime',  # noqa: E501
         'start_time': 'startTime',  # noqa: E501
         'end_time': 'endTime',  # noqa: E501
+        'progress': 'progress',  # noqa: E501
     }
 
     read_only_vars = {
+        'parameters',  # noqa: E501
         'enqueue_time',  # noqa: E501
         'start_time',  # noqa: E501
         'end_time',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetSuggestHistoricFailed - a model defined in OpenAPI
+        """GetSuggestHistoricRunning - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
-            parameters (SuggestHistoricParameters):
-            status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
-            detail (str):
+            parameters (bool, date, datetime, dict, float, int, list, str, none_type): The parameters as they were given to the suggest-historic request.
+            status (str): defaults to "running", must be one of ["running", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -166,17 +166,18 @@
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
+            progress (float): [optional]  # noqa: E501
         """
 
-        status = kwargs.get('status', "failed")
+        status = kwargs.get('status', "running")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -233,21 +234,19 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetSuggestHistoricFailed - a model defined in OpenAPI
+        """GetSuggestHistoricRunning - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
-            parameters (SuggestHistoricParameters):
-            status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
-            detail (str):
+            status (str): defaults to "running", must be one of ["running", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -276,17 +275,18 @@
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
+            progress (float): [optional]  # noqa: E501
         """
 
-        status = kwargs.get('status', "failed")
+        status = kwargs.get('status', "running")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -342,13 +342,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              GetSuggestAdditionalFailedAllOf,
+              GetSuggestAdditionalRunningAllOf,
               PartGetSuggestHistoric,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_pending.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_pending_consistent.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.get_suggest_additional_pending_all_of import GetSuggestAdditionalPendingAllOf
-    from alchemite_apiclient.model.part_get_suggest_historic import PartGetSuggestHistoric
-    from alchemite_apiclient.model.suggest_historic_parameters import SuggestHistoricParameters
-    globals()['GetSuggestAdditionalPendingAllOf'] = GetSuggestAdditionalPendingAllOf
-    globals()['PartGetSuggestHistoric'] = PartGetSuggestHistoric
-    globals()['SuggestHistoricParameters'] = SuggestHistoricParameters
+    from alchemite_apiclient.model.get_optimize_pending_all_of import GetOptimizePendingAllOf
+    from alchemite_apiclient.model.optimize_parameters import OptimizeParameters
+    from alchemite_apiclient.model.part_get_optimize_consistent import PartGetOptimizeConsistent
+    globals()['GetOptimizePendingAllOf'] = GetOptimizePendingAllOf
+    globals()['OptimizeParameters'] = OptimizeParameters
+    globals()['PartGetOptimizeConsistent'] = PartGetOptimizeConsistent
 
 
-class GetSuggestHistoricPending(ModelComposed):
+class GetOptimizePendingConsistent(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
-            'parameters': (SuggestHistoricParameters,),  # noqa: E501
+            'parameters': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
             'end_time': (int,),  # noqa: E501
@@ -113,27 +113,28 @@
         'notes': 'notes',  # noqa: E501
         'enqueue_time': 'enqueueTime',  # noqa: E501
         'start_time': 'startTime',  # noqa: E501
         'end_time': 'endTime',  # noqa: E501
     }
 
     read_only_vars = {
+        'parameters',  # noqa: E501
         'enqueue_time',  # noqa: E501
         'start_time',  # noqa: E501
         'end_time',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetSuggestHistoricPending - a model defined in OpenAPI
+        """GetOptimizePendingConsistent - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
-            parameters (SuggestHistoricParameters):
+            parameters (bool, date, datetime, dict, float, int, list, str, none_type): The parameters as they were given to the optimize request.
             status (str): defaults to "pending", must be one of ["pending", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -160,17 +161,17 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
-            enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
-            start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
-            end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
+            enqueue_time (int): The Unix Timestamp in seconds when the optimize job enqueued.. [optional]  # noqa: E501
+            start_time (int): The Unix Timestamp in seconds when the optimize job started.. [optional]  # noqa: E501
+            end_time (int): The Unix Timestamp in seconds when the optimize job ended.. [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "pending")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -230,19 +231,18 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetSuggestHistoricPending - a model defined in OpenAPI
+        """GetOptimizePendingConsistent - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
-            parameters (SuggestHistoricParameters):
             status (str): defaults to "pending", must be one of ["pending", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -269,17 +269,17 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
-            enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
-            start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
-            end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
+            enqueue_time (int): The Unix Timestamp in seconds when the optimize job enqueued.. [optional]  # noqa: E501
+            start_time (int): The Unix Timestamp in seconds when the optimize job started.. [optional]  # noqa: E501
+            end_time (int): The Unix Timestamp in seconds when the optimize job ended.. [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "pending")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -338,13 +338,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              GetSuggestAdditionalPendingAllOf,
-              PartGetSuggestHistoric,
+              GetOptimizePendingAllOf,
+              PartGetOptimizeConsistent,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_historic_running.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_running.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,22 +26,24 @@
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from alchemite_apiclient.model.get_suggest_additional_running_all_of import GetSuggestAdditionalRunningAllOf
-    from alchemite_apiclient.model.part_get_suggest_historic import PartGetSuggestHistoric
-    from alchemite_apiclient.model.suggest_historic_parameters import SuggestHistoricParameters
+    from alchemite_apiclient.model.part_get_suggest_initial import PartGetSuggestInitial
+    from alchemite_apiclient.model.part_get_suggest_initial_sharing import PartGetSuggestInitialSharing
+    from alchemite_apiclient.model.suggest_initial_parameters import SuggestInitialParameters
     globals()['GetSuggestAdditionalRunningAllOf'] = GetSuggestAdditionalRunningAllOf
-    globals()['PartGetSuggestHistoric'] = PartGetSuggestHistoric
-    globals()['SuggestHistoricParameters'] = SuggestHistoricParameters
+    globals()['PartGetSuggestInitial'] = PartGetSuggestInitial
+    globals()['PartGetSuggestInitialSharing'] = PartGetSuggestInitialSharing
+    globals()['SuggestInitialParameters'] = SuggestInitialParameters
 
 
-class GetSuggestHistoricRunning(ModelComposed):
+class GetSuggestInitialRunning(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,22 +87,24 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
-            'parameters': (SuggestHistoricParameters,),  # noqa: E501
+            'parameters': (SuggestInitialParameters,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
             'end_time': (int,),  # noqa: E501
+            'project_id': (str,),  # noqa: E501
+            'sharing': (PartGetSuggestInitialSharing,),  # noqa: E501
             'progress': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
@@ -111,31 +115,33 @@
         'status': 'status',  # noqa: E501
         'name': 'name',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'notes': 'notes',  # noqa: E501
         'enqueue_time': 'enqueueTime',  # noqa: E501
         'start_time': 'startTime',  # noqa: E501
         'end_time': 'endTime',  # noqa: E501
+        'project_id': 'projectId',  # noqa: E501
+        'sharing': 'sharing',  # noqa: E501
         'progress': 'progress',  # noqa: E501
     }
 
     read_only_vars = {
         'enqueue_time',  # noqa: E501
         'start_time',  # noqa: E501
         'end_time',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetSuggestHistoricRunning - a model defined in OpenAPI
+        """GetSuggestInitialRunning - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
-            parameters (SuggestHistoricParameters):
+            parameters (SuggestInitialParameters):
             status (str): defaults to "running", must be one of ["running", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -165,14 +171,16 @@
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
+            project_id (str): [optional]  # noqa: E501
+            sharing (PartGetSuggestInitialSharing): [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "running")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -233,19 +241,19 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetSuggestHistoricRunning - a model defined in OpenAPI
+        """GetSuggestInitialRunning - a model defined in OpenAPI
 
         Keyword Args:
             id (str):
-            parameters (SuggestHistoricParameters):
+            parameters (SuggestInitialParameters):
             status (str): defaults to "running", must be one of ["running", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -275,14 +283,16 @@
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
+            project_id (str): [optional]  # noqa: E501
+            sharing (PartGetSuggestInitialSharing): [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "running")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -343,12 +353,12 @@
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               GetSuggestAdditionalRunningAllOf,
-              PartGetSuggestHistoric,
+              PartGetSuggestInitial,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_done.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_done.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_done_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_failed.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_failed.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_failed_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_pending.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_suggest_initial_pending.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/get_suggest_initial_running.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_suggest_additional_job_old.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,25 +25,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.get_suggest_additional_running_all_of import GetSuggestAdditionalRunningAllOf
-    from alchemite_apiclient.model.part_get_suggest_initial import PartGetSuggestInitial
-    from alchemite_apiclient.model.part_get_suggest_initial_sharing import PartGetSuggestInitialSharing
-    from alchemite_apiclient.model.suggest_initial_parameters import SuggestInitialParameters
-    globals()['GetSuggestAdditionalRunningAllOf'] = GetSuggestAdditionalRunningAllOf
-    globals()['PartGetSuggestInitial'] = PartGetSuggestInitial
-    globals()['PartGetSuggestInitialSharing'] = PartGetSuggestInitialSharing
-    globals()['SuggestInitialParameters'] = SuggestInitialParameters
+    from alchemite_apiclient.model.model_id_stub import ModelIDStub
+    from alchemite_apiclient.model.suggest_additional_job import SuggestAdditionalJob
+    from alchemite_apiclient.model.suggest_additional_parameters import SuggestAdditionalParameters
+    from alchemite_apiclient.model.suggest_additional_result import SuggestAdditionalResult
+    globals()['ModelIDStub'] = ModelIDStub
+    globals()['SuggestAdditionalJob'] = SuggestAdditionalJob
+    globals()['SuggestAdditionalParameters'] = SuggestAdditionalParameters
+    globals()['SuggestAdditionalResult'] = SuggestAdditionalResult
 
 
-class GetSuggestInitialRunning(ModelComposed):
+class MetadataSuggestAdditionalJobOld(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,63 +86,68 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'model_id': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'parameters': (SuggestInitialParameters,),  # noqa: E501
+            'parameters': (SuggestAdditionalParameters,),  # noqa: E501
             'status': (str,),  # noqa: E501
+            'result': (SuggestAdditionalResult,),  # noqa: E501
+            'detail': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
             'end_time': (int,),  # noqa: E501
-            'project_id': (str,),  # noqa: E501
-            'sharing': (PartGetSuggestInitialSharing,),  # noqa: E501
             'progress': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
+        'model_id': 'modelId',  # noqa: E501
         'id': 'id',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
         'status': 'status',  # noqa: E501
+        'result': 'result',  # noqa: E501
+        'detail': 'detail',  # noqa: E501
         'name': 'name',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'notes': 'notes',  # noqa: E501
         'enqueue_time': 'enqueueTime',  # noqa: E501
         'start_time': 'startTime',  # noqa: E501
         'end_time': 'endTime',  # noqa: E501
-        'project_id': 'projectId',  # noqa: E501
-        'sharing': 'sharing',  # noqa: E501
         'progress': 'progress',  # noqa: E501
     }
 
     read_only_vars = {
         'enqueue_time',  # noqa: E501
         'start_time',  # noqa: E501
         'end_time',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GetSuggestInitialRunning - a model defined in OpenAPI
+        """MetadataSuggestAdditionalJobOld - a model defined in OpenAPI
 
         Keyword Args:
+            model_id (str): The ID of the model associated with the job.
             id (str):
-            parameters (SuggestInitialParameters):
-            status (str): defaults to "running", must be one of ["running", ]  # noqa: E501
+            parameters (SuggestAdditionalParameters):
+            status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
+            result (SuggestAdditionalResult):
+            detail (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -171,20 +176,18 @@
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
-            project_id (str): [optional]  # noqa: E501
-            sharing (PartGetSuggestInitialSharing): [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
         """
 
-        status = kwargs.get('status', "running")
+        status = kwargs.get('status', "failed")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -241,20 +244,23 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GetSuggestInitialRunning - a model defined in OpenAPI
+        """MetadataSuggestAdditionalJobOld - a model defined in OpenAPI
 
         Keyword Args:
+            model_id (str): The ID of the model associated with the job.
             id (str):
-            parameters (SuggestInitialParameters):
-            status (str): defaults to "running", must be one of ["running", ]  # noqa: E501
+            parameters (SuggestAdditionalParameters):
+            status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
+            result (SuggestAdditionalResult):
+            detail (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -283,20 +289,18 @@
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
-            project_id (str): [optional]  # noqa: E501
-            sharing (PartGetSuggestInitialSharing): [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
         """
 
-        status = kwargs.get('status', "running")
+        status = kwargs.get('status', "failed")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
@@ -352,13 +356,11 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
-              GetSuggestAdditionalRunningAllOf,
-              PartGetSuggestInitial,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/histogram_categorical.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/histogram_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/histogram_continuous.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/histogram_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/histogram_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/histogram_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/histogram_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/histogram_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_categorical_prediction.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_categorical_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_prediction.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_scalar_prediction.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_scalar_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_target_function.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_target_function.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_value.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_vector_prediction.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_vector_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/historic_vector_value.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/historic_vector_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/importance_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/importance_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/impute_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/impute_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response200.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response2001.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response2002.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response2003.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/inline_response2004.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/inline_response2004.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.metadata_suggest_additional_job import MetadataSuggestAdditionalJob
-    globals()['MetadataSuggestAdditionalJob'] = MetadataSuggestAdditionalJob
+    from alchemite_apiclient.model.metadata_suggest_additional_job_old import MetadataSuggestAdditionalJobOld
+    globals()['MetadataSuggestAdditionalJobOld'] = MetadataSuggestAdditionalJobOld
 
 
 class InlineResponse2004(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -83,15 +83,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'total': (int,),  # noqa: E501
-            'result': ([MetadataSuggestAdditionalJob],),  # noqa: E501
+            'result': ([MetadataSuggestAdditionalJobOld],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
@@ -108,15 +108,15 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, total, result, *args, **kwargs):  # noqa: E501
         """InlineResponse2004 - a model defined in OpenAPI
 
         Args:
             total (int): Total number of jobs that matched the given query. Will not consider the offset or limit of the request, meaning this is the total number of jobs if no size restrictions were applied.
-            result ([MetadataSuggestAdditionalJob]): Suggest-additional jobs matching the query, offset, and limit.
+            result ([MetadataSuggestAdditionalJobOld]): Suggest-additional jobs matching the query, offset, and limit.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -195,15 +195,15 @@
 
     @convert_js_args_to_python_args
     def __init__(self, total, result, *args, **kwargs):  # noqa: E501
         """InlineResponse2004 - a model defined in OpenAPI
 
         Args:
             total (int): Total number of jobs that matched the given query. Will not consider the offset or limit of the request, meaning this is the total number of jobs if no size restrictions were applied.
-            result ([MetadataSuggestAdditionalJob]): Suggest-additional jobs matching the query, offset, and limit.
+            result ([MetadataSuggestAdditionalJobOld]): Suggest-additional jobs matching the query, offset, and limit.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/int_cat_arr.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/int_cat_arr.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/job_patch.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/job_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/load_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/load_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/max.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/max.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/metadata_optimization_job.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/get_optimize_failed_consistent.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,25 +25,23 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.model_id_stub import ModelIDStub
-    from alchemite_apiclient.model.optimization_job import OptimizationJob
-    from alchemite_apiclient.model.optimize_request import OptimizeRequest
-    from alchemite_apiclient.model.part_get_optimize_done_result_array import PartGetOptimizeDoneResultArray
-    globals()['ModelIDStub'] = ModelIDStub
-    globals()['OptimizationJob'] = OptimizationJob
-    globals()['OptimizeRequest'] = OptimizeRequest
-    globals()['PartGetOptimizeDoneResultArray'] = PartGetOptimizeDoneResultArray
+    from alchemite_apiclient.model.get_optimize_failed_all_of import GetOptimizeFailedAllOf
+    from alchemite_apiclient.model.optimize_parameters import OptimizeParameters
+    from alchemite_apiclient.model.part_get_optimize_consistent import PartGetOptimizeConsistent
+    globals()['GetOptimizeFailedAllOf'] = GetOptimizeFailedAllOf
+    globals()['OptimizeParameters'] = OptimizeParameters
+    globals()['PartGetOptimizeConsistent'] = PartGetOptimizeConsistent
 
 
-class MetadataOptimizationJob(ModelComposed):
+class GetOptimizeFailedConsistent(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -86,61 +84,60 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'model_id': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'parameters': (OptimizeRequest,),  # noqa: E501
+            'parameters': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'status': (str,),  # noqa: E501
-            'result': (PartGetOptimizeDoneResultArray,),  # noqa: E501
             'detail': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'tags': ([str],),  # noqa: E501
+            'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
             'end_time': (int,),  # noqa: E501
-            'progress': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
     attribute_map = {
-        'model_id': 'modelId',  # noqa: E501
         'id': 'id',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
         'status': 'status',  # noqa: E501
-        'result': 'result',  # noqa: E501
         'detail': 'detail',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'tags': 'tags',  # noqa: E501
+        'notes': 'notes',  # noqa: E501
         'enqueue_time': 'enqueueTime',  # noqa: E501
         'start_time': 'startTime',  # noqa: E501
         'end_time': 'endTime',  # noqa: E501
-        'progress': 'progress',  # noqa: E501
     }
 
     read_only_vars = {
+        'parameters',  # noqa: E501
         'enqueue_time',  # noqa: E501
         'start_time',  # noqa: E501
         'end_time',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """MetadataOptimizationJob - a model defined in OpenAPI
+        """GetOptimizeFailedConsistent - a model defined in OpenAPI
 
         Keyword Args:
-            model_id (str): The ID of the model associated with the job.
             id (str):
-            parameters (OptimizeRequest):
+            parameters (bool, date, datetime, dict, float, int, list, str, none_type): The parameters as they were given to the optimize request.
             status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
-            result (PartGetOptimizeDoneResultArray):
             detail (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -164,18 +161,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            name (str): The job's name. [optional]  # noqa: E501
+            tags ([str]): The tags attached to the job. [optional]  # noqa: E501
+            notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the optimize job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the optimize job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the optimize job ended.. [optional]  # noqa: E501
-            progress (float): [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "failed")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -235,22 +234,19 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """MetadataOptimizationJob - a model defined in OpenAPI
+        """GetOptimizeFailedConsistent - a model defined in OpenAPI
 
         Keyword Args:
-            model_id (str): The ID of the model associated with the job.
             id (str):
-            parameters (OptimizeRequest):
             status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
-            result (PartGetOptimizeDoneResultArray):
             detail (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -274,18 +270,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            name (str): The job's name. [optional]  # noqa: E501
+            tags ([str]): The tags attached to the job. [optional]  # noqa: E501
+            notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the optimize job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the optimize job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the optimize job ended.. [optional]  # noqa: E501
-            progress (float): [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "failed")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -344,11 +342,13 @@
         # classes don't exist yet because their module has not finished
         # loading
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
+              GetOptimizeFailedAllOf,
+              PartGetOptimizeConsistent,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/metadata_suggest_additional_job.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_suggest_additional_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,20 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from alchemite_apiclient.model.metadata_suggest_additional_job_all_of import MetadataSuggestAdditionalJobAllOf
     from alchemite_apiclient.model.model_id_stub import ModelIDStub
     from alchemite_apiclient.model.suggest_additional_job import SuggestAdditionalJob
     from alchemite_apiclient.model.suggest_additional_parameters import SuggestAdditionalParameters
     from alchemite_apiclient.model.suggest_additional_result import SuggestAdditionalResult
+    globals()['MetadataSuggestAdditionalJobAllOf'] = MetadataSuggestAdditionalJobAllOf
     globals()['ModelIDStub'] = ModelIDStub
     globals()['SuggestAdditionalJob'] = SuggestAdditionalJob
     globals()['SuggestAdditionalParameters'] = SuggestAdditionalParameters
     globals()['SuggestAdditionalResult'] = SuggestAdditionalResult
 
 
 class MetadataSuggestAdditionalJob(ModelComposed):
@@ -92,14 +94,15 @@
         return {
             'model_id': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'parameters': (SuggestAdditionalParameters,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'result': (SuggestAdditionalResult,),  # noqa: E501
             'detail': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
             'end_time': (int,),  # noqa: E501
             'progress': (float,),  # noqa: E501
@@ -113,14 +116,15 @@
     attribute_map = {
         'model_id': 'modelId',  # noqa: E501
         'id': 'id',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
         'status': 'status',  # noqa: E501
         'result': 'result',  # noqa: E501
         'detail': 'detail',  # noqa: E501
+        'type': 'type',  # noqa: E501
         'name': 'name',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'notes': 'notes',  # noqa: E501
         'enqueue_time': 'enqueueTime',  # noqa: E501
         'start_time': 'startTime',  # noqa: E501
         'end_time': 'endTime',  # noqa: E501
         'progress': 'progress',  # noqa: E501
@@ -140,14 +144,15 @@
         Keyword Args:
             model_id (str): The ID of the model associated with the job.
             id (str):
             parameters (SuggestAdditionalParameters):
             status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
             result (SuggestAdditionalResult):
             detail (str):
+            type (str): defaults to "suggest-additional", must be one of ["suggest-additional", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -180,14 +185,15 @@
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "failed")
+        type = kwargs.get('type', "suggest-additional")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -253,14 +259,15 @@
         Keyword Args:
             model_id (str): The ID of the model associated with the job.
             id (str):
             parameters (SuggestAdditionalParameters):
             status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
             result (SuggestAdditionalResult):
             detail (str):
+            type (str): defaults to "suggest-additional", must be one of ["suggest-additional", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -293,14 +300,15 @@
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "failed")
+        type = kwargs.get('type', "suggest-additional")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/metadata_suggest_historic_job.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/metadata_suggest_historic_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,18 +88,19 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'model_id': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'parameters': (SuggestHistoricParameters,),  # noqa: E501
+            'parameters': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'result': (SuggestHistoricResult,),  # noqa: E501
             'detail': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
             'end_time': (int,),  # noqa: E501
             'progress': (float,),  # noqa: E501
@@ -113,41 +114,44 @@
     attribute_map = {
         'model_id': 'modelId',  # noqa: E501
         'id': 'id',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
         'status': 'status',  # noqa: E501
         'result': 'result',  # noqa: E501
         'detail': 'detail',  # noqa: E501
+        'type': 'type',  # noqa: E501
         'name': 'name',  # noqa: E501
         'tags': 'tags',  # noqa: E501
         'notes': 'notes',  # noqa: E501
         'enqueue_time': 'enqueueTime',  # noqa: E501
         'start_time': 'startTime',  # noqa: E501
         'end_time': 'endTime',  # noqa: E501
         'progress': 'progress',  # noqa: E501
     }
 
     read_only_vars = {
+        'parameters',  # noqa: E501
         'enqueue_time',  # noqa: E501
         'start_time',  # noqa: E501
         'end_time',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """MetadataSuggestHistoricJob - a model defined in OpenAPI
 
         Keyword Args:
             model_id (str): The ID of the model associated with the job.
             id (str):
-            parameters (SuggestHistoricParameters):
+            parameters (bool, date, datetime, dict, float, int, list, str, none_type): The parameters as they were given to the suggest-historic request.
             status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
             result (SuggestHistoricResult):
             detail (str):
+            type (str): defaults to "suggest-historic", must be one of ["suggest-historic", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -180,14 +184,15 @@
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "failed")
+        type = kwargs.get('type', "suggest-historic")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -249,18 +254,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """MetadataSuggestHistoricJob - a model defined in OpenAPI
 
         Keyword Args:
             model_id (str): The ID of the model associated with the job.
             id (str):
-            parameters (SuggestHistoricParameters):
             status (str): defaults to "failed", must be one of ["failed", ]  # noqa: E501
             result (SuggestHistoricResult):
             detail (str):
+            type (str): defaults to "suggest-historic", must be one of ["suggest-historic", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -293,14 +298,15 @@
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
         """
 
         status = kwargs.get('status', "failed")
+        type = kwargs.get('type', "suggest-historic")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/min.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/min.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/model.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/model.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_column_info.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_column_info.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_id_stub.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_id_stub.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_patch.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_permitted_column_relationships.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_permitted_column_relationships.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_query.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_query.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_sharing.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_sharing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_status.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_status.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/model_validation_methods.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/model_validation_methods.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/models_id_additive_sensitivity_origin.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/models_id_train_permitted_column_relationships.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/models_metadata_filters.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/models_metadata_filters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/models_metadata_sort.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/models_metadata_sort.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_col_weights_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_constant_sum_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_product.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_product.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_product_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_ratio_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_summands_weights_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_const_sum_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_weighted_ratio_all_of_arguments.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/new_columns.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/new_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/non_empty_categorical_column.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/non_empty_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/non_empty_continuous_column.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/non_empty_continuous_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/non_empty_integer_categorical_column.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/numerical_filter.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/numerical_filter.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/optimization_job.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/optimization_job.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/optimize_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/optimize_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     globals()['DependentColumns'] = DependentColumns
     globals()['NewColumns'] = NewColumns
     globals()['SampleDefinition'] = SampleDefinition
     globals()['SetInputs'] = SetInputs
     globals()['TargetFunction'] = TargetFunction
 
 
-class OptimizeRequest(ModelNormal):
+class OptimizeParameters(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -82,16 +82,14 @@
         },
     }
 
     validations = {
         ('num_optimization_samples',): {
             'inclusive_minimum': 1,
         },
-        ('tags',): {
-        },
     }
 
     @cached_property
     def additional_properties_type():  # noqa
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -116,17 +114,14 @@
             'sample_definition': (SampleDefinition,),  # noqa: E501
             'target_function': (TargetFunction,),  # noqa: E501
             'new_columns': (NewColumns,),  # noqa: E501
             'dependent_columns': (DependentColumns,),  # noqa: E501
             'set_inputs': (SetInputs,),  # noqa: E501
             'num_optimization_samples': (int,),  # noqa: E501
             'optimization_method': (str,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'tags': ([str],),  # noqa: E501
-            'notes': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
         return None
 
 
@@ -134,28 +129,25 @@
         'sample_definition': 'sampleDefinition',  # noqa: E501
         'target_function': 'targetFunction',  # noqa: E501
         'new_columns': 'newColumns',  # noqa: E501
         'dependent_columns': 'dependentColumns',  # noqa: E501
         'set_inputs': 'setInputs',  # noqa: E501
         'num_optimization_samples': 'numOptimizationSamples',  # noqa: E501
         'optimization_method': 'optimizationMethod',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'tags': 'tags',  # noqa: E501
-        'notes': 'notes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, sample_definition, target_function, *args, **kwargs):  # noqa: E501
-        """OptimizeRequest - a model defined in OpenAPI
+        """OptimizeParameters - a model defined in OpenAPI
 
         Args:
             sample_definition (SampleDefinition):
             target_function (TargetFunction):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -189,17 +181,14 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             new_columns (NewColumns): [optional]  # noqa: E501
             dependent_columns (DependentColumns): [optional]  # noqa: E501
             set_inputs (SetInputs): [optional]  # noqa: E501
             num_optimization_samples (int): The number of optimization samples that will be considered. Defaults to `1000`. The maximum is set per user and defaults to `10000`. . [optional] if omitted the server will use the default value of 1000  # noqa: E501
             optimization_method (str): The following **global optimization** methods are available: * `\"TPE\"`: Tree-structured Parzen Estimator * `\"random\"`: Random search * `\"alchemite\"`: Use Alchemite's optimize method  > The `\"alchemite\"` method only supports the `\"continuous\"` sample definition type.  The following **local optimization** methods are available: * `\"local alchemite\"`: Use Alchemite's local optimize method * `\"powell\"`: Recommended local optimization method * `\"nelder-mead\"`, `\"l-bfgs-b\"`, `\"bfgs\"`, `\"conjugate gradient\"`, `\"cobyla\"`, `\"slsqp\"`, `\"tnc\"`: Other local optimization methods  > Local optimization only supports the following `\"sample definition\"` types: `\"continuous\"`, `\"continuous or zero\"` and `\"categorical\"`  > The `\"alchemite\"` and `\"local alchemite\"` methods cannot be used with `dependentColumns`; models trained on datasets containing vectors or `calculatedColumns`; or `targetFunctions` other than `\"between\"`, `\"below\"` or `\"above\"` . [optional] if omitted the server will use the default value of "TPE"  # noqa: E501
-            name (str): Optional name to attach to the optimization.. [optional]  # noqa: E501
-            tags ([str]): Optional tags to attach to the optimization. Array should contain unique strings.. [optional]  # noqa: E501
-            notes (str): An optional free field for notes about the optimisation job.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -242,15 +231,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, sample_definition, target_function, *args, **kwargs):  # noqa: E501
-        """OptimizeRequest - a model defined in OpenAPI
+        """OptimizeParameters - a model defined in OpenAPI
 
         Args:
             sample_definition (SampleDefinition):
             target_function (TargetFunction):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -284,17 +273,14 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             new_columns (NewColumns): [optional]  # noqa: E501
             dependent_columns (DependentColumns): [optional]  # noqa: E501
             set_inputs (SetInputs): [optional]  # noqa: E501
             num_optimization_samples (int): The number of optimization samples that will be considered. Defaults to `1000`. The maximum is set per user and defaults to `10000`. . [optional] if omitted the server will use the default value of 1000  # noqa: E501
             optimization_method (str): The following **global optimization** methods are available: * `\"TPE\"`: Tree-structured Parzen Estimator * `\"random\"`: Random search * `\"alchemite\"`: Use Alchemite's optimize method  > The `\"alchemite\"` method only supports the `\"continuous\"` sample definition type.  The following **local optimization** methods are available: * `\"local alchemite\"`: Use Alchemite's local optimize method * `\"powell\"`: Recommended local optimization method * `\"nelder-mead\"`, `\"l-bfgs-b\"`, `\"bfgs\"`, `\"conjugate gradient\"`, `\"cobyla\"`, `\"slsqp\"`, `\"tnc\"`: Other local optimization methods  > Local optimization only supports the following `\"sample definition\"` types: `\"continuous\"`, `\"continuous or zero\"` and `\"categorical\"`  > The `\"alchemite\"` and `\"local alchemite\"` methods cannot be used with `dependentColumns`; models trained on datasets containing vectors or `calculatedColumns`; or `targetFunctions` other than `\"between\"`, `\"below\"` or `\"above\"` . [optional] if omitted the server will use the default value of "TPE"  # noqa: E501
-            name (str): Optional name to attach to the optimization.. [optional]  # noqa: E501
-            tags ([str]): Optional tags to attach to the optimization. Array should contain unique strings.. [optional]  # noqa: E501
-            notes (str): An optional free field for notes about the optimisation job.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/ot_sample_def_categorical.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/ot_sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/ot_sample_def_continuous.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/ot_sample_def_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/ot_sample_definition.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/ot_sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/ot_set_inputs.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/ot_set_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/outliers_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/outliers_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response_predictions.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response_predictions.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/output_tolerance_univariate_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/output_tolerance_univariate_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_dependent_columns.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_dependent_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_optimize.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_optimize_done_result_array.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_suggest_additional.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_suggest_historic.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_optimize_consistent.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from alchemite_apiclient.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from alchemite_apiclient.model.suggest_historic_parameters import SuggestHistoricParameters
-    globals()['SuggestHistoricParameters'] = SuggestHistoricParameters
+    from alchemite_apiclient.model.optimize_parameters import OptimizeParameters
+    globals()['OptimizeParameters'] = OptimizeParameters
 
 
-class PartGetSuggestHistoric(ModelNormal):
+class PartGetOptimizeConsistent(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
-            'parameters': (SuggestHistoricParameters,),  # noqa: E501
+            'parameters': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'tags': ([str],),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
             'end_time': (int,),  # noqa: E501
         }
@@ -111,29 +111,30 @@
         'notes': 'notes',  # noqa: E501
         'enqueue_time': 'enqueueTime',  # noqa: E501
         'start_time': 'startTime',  # noqa: E501
         'end_time': 'endTime',  # noqa: E501
     }
 
     read_only_vars = {
+        'parameters',  # noqa: E501
         'enqueue_time',  # noqa: E501
         'start_time',  # noqa: E501
         'end_time',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, parameters, *args, **kwargs):  # noqa: E501
-        """PartGetSuggestHistoric - a model defined in OpenAPI
+        """PartGetOptimizeConsistent - a model defined in OpenAPI
 
         Args:
             id (str):
-            parameters (SuggestHistoricParameters):
+            parameters (bool, date, datetime, dict, float, int, list, str, none_type): The parameters as they were given to the optimize request.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,17 +162,17 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
-            enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
-            start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
-            end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
+            enqueue_time (int): The Unix Timestamp in seconds when the optimize job enqueued.. [optional]  # noqa: E501
+            start_time (int): The Unix Timestamp in seconds when the optimize job started.. [optional]  # noqa: E501
+            end_time (int): The Unix Timestamp in seconds when the optimize job ended.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -213,21 +214,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, parameters, *args, **kwargs):  # noqa: E501
-        """PartGetSuggestHistoric - a model defined in OpenAPI
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
+        """PartGetOptimizeConsistent - a model defined in OpenAPI
 
         Args:
             id (str):
-            parameters (SuggestHistoricParameters):
-
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -254,17 +253,17 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): The job's name. [optional]  # noqa: E501
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
-            enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
-            start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
-            end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
+            enqueue_time (int): The Unix Timestamp in seconds when the optimize job enqueued.. [optional]  # noqa: E501
+            start_time (int): The Unix Timestamp in seconds when the optimize job started.. [optional]  # noqa: E501
+            end_time (int): The Unix Timestamp in seconds when the optimize job ended.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -283,15 +282,14 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
-        self.parameters = parameters
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_suggest_initial.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_get_suggest_initial_sharing.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_get_suggest_initial_sharing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_new_columns.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_new_columns.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_above.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_below.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_between.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_categoricals.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_categoricals.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_single_tar.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_single_tar.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_sum.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/part_tar_fn_weighted_sum.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/predict_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/predict_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/predict_trendline_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/predict_trendline_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/prediction.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/project.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/project.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/project_bulk_model.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/project_bulk_model.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/project_bulk_suggest_initial.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/project_bulk_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/project_patch.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/project_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/project_sharing.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/project_sharing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/query_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/query_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/query_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/query_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/range.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/range.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_categorical.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_categorical_column_values.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_categorical_column_values.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_composition.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_composition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_composition_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_composition_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_continuous.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_continuous.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_continuous_with_start.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_continuous_with_start.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_discrete.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_discrete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_integer.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_integer.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_start_prop.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_start_prop.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_def_weighted_categorical.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_def_weighted_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sample_definition.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/scalar_prediction.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/scalar_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/scalar_result.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/scalar_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/sensitivity_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/sensitivity_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/set_inputs.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/set_inputs.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/share_group.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/share_group.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/si_sample_def_categorical.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/si_sample_def_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/si_sample_definition.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/si_sample_definition.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/string_cat_arr.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/string_cat_arr.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_job.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_job.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_metadata_filters.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_metadata_filters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_metadata_sort.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_metadata_sort.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_parameters.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_parameters_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_query.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_query.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_request_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_additional_result.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_additional_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_job.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             'tags': ([str],),  # noqa: E501
             'notes': (str,),  # noqa: E501
             'enqueue_time': (int,),  # noqa: E501
             'start_time': (int,),  # noqa: E501
             'end_time': (int,),  # noqa: E501
             'progress': (float,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'parameters': (SuggestHistoricParameters,),  # noqa: E501
+            'parameters': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'status': (str,),  # noqa: E501
             'result': (SuggestHistoricResult,),  # noqa: E501
             'detail': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():  # noqa
@@ -128,14 +128,15 @@
         'detail': 'detail',  # noqa: E501
     }
 
     read_only_vars = {
         'enqueue_time',  # noqa: E501
         'start_time',  # noqa: E501
         'end_time',  # noqa: E501
+        'parameters',  # noqa: E501
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """SuggestHistoricJob - a model defined in OpenAPI
 
@@ -174,15 +175,15 @@
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
-            parameters (SuggestHistoricParameters): [optional]  # noqa: E501
+            parameters (bool, date, datetime, dict, float, int, list, str, none_type): The parameters as they were given to the suggest-historic request.. [optional]  # noqa: E501
             status (str): [optional] if omitted the server will use the default value of "failed"  # noqa: E501
             result (SuggestHistoricResult): [optional]  # noqa: E501
             detail (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -285,15 +286,15 @@
             tags ([str]): The tags attached to the job. [optional]  # noqa: E501
             notes (str): An optional free field for notes about the job.. [optional]  # noqa: E501
             enqueue_time (int): The Unix Timestamp in seconds when the job enqueued.. [optional]  # noqa: E501
             start_time (int): The Unix Timestamp in seconds when the job started.. [optional]  # noqa: E501
             end_time (int): The Unix Timestamp in seconds when the job ended.. [optional]  # noqa: E501
             progress (float): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
-            parameters (SuggestHistoricParameters): [optional]  # noqa: E501
+            parameters (bool, date, datetime, dict, float, int, list, str, none_type): The parameters as they were given to the suggest-historic request.. [optional]  # noqa: E501
             status (str): [optional] if omitted the server will use the default value of "failed"  # noqa: E501
             result (SuggestHistoricResult): [optional]  # noqa: E501
             detail (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_parameters.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_result.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_historic_result_samples.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_historic_result_samples.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_job_patch.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_job_patch.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_parameters.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_parameters.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_request_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_request_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_initial_result.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_initial_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_common.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_common.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_data.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_data_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_data_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_dataset_id.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_dataset_id.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_dataset_id_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_imputed_data.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_imputed_data.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_imputed_data_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/suggest_missing_specific.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/suggest_missing_specific.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_above.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_above_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_below.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_below_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_between.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_between_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_exclude_categories.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_exclude_categories.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_exclude_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_include_categories.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_include_categories.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_include_categories_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_above.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_below.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_between.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_sum_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_above.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_above_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_below.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_below_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_between.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/tar_fn_weighted_sum_between_all_of.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/target_function.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/target_function.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/train_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/train_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/training_dataset_outliers_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/training_dataset_outliers_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/training_validation_prediction_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/training_validation_prediction_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/validate_request.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/validate_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/validation_split.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/validation_split.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/value.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/vector_prediction.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/vector_prediction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/vector_result.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/vector_result.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/vector_value.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/vector_value.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model/version_response.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model/version_response.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/model_utils.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/model_utils.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/models/__init__.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from alchemite_apiclient.model.column_group_patch_request import ColumnGroupPatchRequest
 from alchemite_apiclient.model.column_group_request import ColumnGroupRequest
 from alchemite_apiclient.model.column_group_response import ColumnGroupResponse
 from alchemite_apiclient.model.column_group_response_all_of import ColumnGroupResponseAllOf
 from alchemite_apiclient.model.column_info import ColumnInfo
 from alchemite_apiclient.model.column_value import ColumnValue
 from alchemite_apiclient.model.column_value_nullable import ColumnValueNullable
+from alchemite_apiclient.model.consistent_optimization_job import ConsistentOptimizationJob
 from alchemite_apiclient.model.continuous_column_info import ContinuousColumnInfo
 from alchemite_apiclient.model.continuous_column_info_all_of import ContinuousColumnInfoAllOf
 from alchemite_apiclient.model.continuous_column_info_stats import ContinuousColumnInfoStats
 from alchemite_apiclient.model.continuous_model_column_info import ContinuousModelColumnInfo
 from alchemite_apiclient.model.continuous_model_column_info_all_of import ContinuousModelColumnInfoAllOf
 from alchemite_apiclient.model.dr_dataset_reduction_data import DRDatasetReductionData
 from alchemite_apiclient.model.dr_dataset_reduction_metadata import DRDatasetReductionMetadata
@@ -77,20 +78,24 @@
 from alchemite_apiclient.model.dimensionality_reduction_response import DimensionalityReductionResponse
 from alchemite_apiclient.model.empty_categorical_column import EmptyCategoricalColumn
 from alchemite_apiclient.model.empty_continuous_column import EmptyContinuousColumn
 from alchemite_apiclient.model.error import Error
 from alchemite_apiclient.model.get_all_opt_jobs import GetAllOptJobs
 from alchemite_apiclient.model.get_optimize_done import GetOptimizeDone
 from alchemite_apiclient.model.get_optimize_done_all_of import GetOptimizeDoneAllOf
+from alchemite_apiclient.model.get_optimize_done_consistent import GetOptimizeDoneConsistent
 from alchemite_apiclient.model.get_optimize_failed import GetOptimizeFailed
 from alchemite_apiclient.model.get_optimize_failed_all_of import GetOptimizeFailedAllOf
+from alchemite_apiclient.model.get_optimize_failed_consistent import GetOptimizeFailedConsistent
 from alchemite_apiclient.model.get_optimize_optimizing import GetOptimizeOptimizing
 from alchemite_apiclient.model.get_optimize_optimizing_all_of import GetOptimizeOptimizingAllOf
+from alchemite_apiclient.model.get_optimize_optimizing_consistent import GetOptimizeOptimizingConsistent
 from alchemite_apiclient.model.get_optimize_pending import GetOptimizePending
 from alchemite_apiclient.model.get_optimize_pending_all_of import GetOptimizePendingAllOf
+from alchemite_apiclient.model.get_optimize_pending_consistent import GetOptimizePendingConsistent
 from alchemite_apiclient.model.get_suggest_additional_done import GetSuggestAdditionalDone
 from alchemite_apiclient.model.get_suggest_additional_done_all_of import GetSuggestAdditionalDoneAllOf
 from alchemite_apiclient.model.get_suggest_additional_failed import GetSuggestAdditionalFailed
 from alchemite_apiclient.model.get_suggest_additional_failed_all_of import GetSuggestAdditionalFailedAllOf
 from alchemite_apiclient.model.get_suggest_additional_pending import GetSuggestAdditionalPending
 from alchemite_apiclient.model.get_suggest_additional_pending_all_of import GetSuggestAdditionalPendingAllOf
 from alchemite_apiclient.model.get_suggest_additional_running import GetSuggestAdditionalRunning
@@ -120,21 +125,29 @@
 from alchemite_apiclient.model.importance_request import ImportanceRequest
 from alchemite_apiclient.model.impute_request import ImputeRequest
 from alchemite_apiclient.model.inline_response200 import InlineResponse200
 from alchemite_apiclient.model.inline_response2001 import InlineResponse2001
 from alchemite_apiclient.model.inline_response2002 import InlineResponse2002
 from alchemite_apiclient.model.inline_response2003 import InlineResponse2003
 from alchemite_apiclient.model.inline_response2004 import InlineResponse2004
+from alchemite_apiclient.model.inline_response2005 import InlineResponse2005
 from alchemite_apiclient.model.int_cat_arr import IntCatArr
 from alchemite_apiclient.model.job_patch import JobPatch
+from alchemite_apiclient.model.job_query import JobQuery
+from alchemite_apiclient.model.jobs_metadata_filters import JobsMetadataFilters
+from alchemite_apiclient.model.jobs_metadata_sort import JobsMetadataSort
 from alchemite_apiclient.model.load_request import LoadRequest
 from alchemite_apiclient.model.max import Max
 from alchemite_apiclient.model.metadata_optimization_job import MetadataOptimizationJob
+from alchemite_apiclient.model.metadata_optimization_job_all_of import MetadataOptimizationJobAllOf
 from alchemite_apiclient.model.metadata_suggest_additional_job import MetadataSuggestAdditionalJob
+from alchemite_apiclient.model.metadata_suggest_additional_job_all_of import MetadataSuggestAdditionalJobAllOf
+from alchemite_apiclient.model.metadata_suggest_additional_job_old import MetadataSuggestAdditionalJobOld
 from alchemite_apiclient.model.metadata_suggest_historic_job import MetadataSuggestHistoricJob
+from alchemite_apiclient.model.metadata_suggest_historic_job_all_of import MetadataSuggestHistoricJobAllOf
 from alchemite_apiclient.model.min import Min
 from alchemite_apiclient.model.model import Model
 from alchemite_apiclient.model.model_column_info import ModelColumnInfo
 from alchemite_apiclient.model.model_id_stub import ModelIDStub
 from alchemite_apiclient.model.model_patch import ModelPatch
 from alchemite_apiclient.model.model_permitted_column_relationships import ModelPermittedColumnRelationships
 from alchemite_apiclient.model.model_query import ModelQuery
@@ -175,25 +188,28 @@
 from alchemite_apiclient.model.non_empty_integer_categorical_column import NonEmptyIntegerCategoricalColumn
 from alchemite_apiclient.model.numerical_filter import NumericalFilter
 from alchemite_apiclient.model.ot_sample_def_categorical import OTSampleDefCategorical
 from alchemite_apiclient.model.ot_sample_def_continuous import OTSampleDefContinuous
 from alchemite_apiclient.model.ot_sample_definition import OTSampleDefinition
 from alchemite_apiclient.model.ot_set_inputs import OTSetInputs
 from alchemite_apiclient.model.optimization_job import OptimizationJob
+from alchemite_apiclient.model.optimize_parameters import OptimizeParameters
 from alchemite_apiclient.model.optimize_request import OptimizeRequest
+from alchemite_apiclient.model.optimize_request_all_of import OptimizeRequestAllOf
 from alchemite_apiclient.model.outliers_request import OutliersRequest
 from alchemite_apiclient.model.output_tolerance_request import OutputToleranceRequest
 from alchemite_apiclient.model.output_tolerance_response import OutputToleranceResponse
 from alchemite_apiclient.model.output_tolerance_response_fixed_inputs import OutputToleranceResponseFixedInputs
 from alchemite_apiclient.model.output_tolerance_response_predicted_outputs import OutputToleranceResponsePredictedOutputs
 from alchemite_apiclient.model.output_tolerance_response_predictions import OutputToleranceResponsePredictions
 from alchemite_apiclient.model.output_tolerance_response_sampled_inputs import OutputToleranceResponseSampledInputs
 from alchemite_apiclient.model.output_tolerance_univariate_response import OutputToleranceUnivariateResponse
 from alchemite_apiclient.model.part_dependent_columns import PartDependentColumns
 from alchemite_apiclient.model.part_get_optimize import PartGetOptimize
+from alchemite_apiclient.model.part_get_optimize_consistent import PartGetOptimizeConsistent
 from alchemite_apiclient.model.part_get_optimize_done_result_array import PartGetOptimizeDoneResultArray
 from alchemite_apiclient.model.part_get_suggest_additional import PartGetSuggestAdditional
 from alchemite_apiclient.model.part_get_suggest_historic import PartGetSuggestHistoric
 from alchemite_apiclient.model.part_get_suggest_initial import PartGetSuggestInitial
 from alchemite_apiclient.model.part_get_suggest_initial_sharing import PartGetSuggestInitialSharing
 from alchemite_apiclient.model.part_new_columns import PartNewColumns
 from alchemite_apiclient.model.part_tar_fn_above import PartTarFnAbove
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient/rest.py` & `alchemite_apiclient-0.74.0/alchemite_apiclient/rest.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient.egg-info/PKG-INFO` & `alchemite_apiclient-0.74.0/alchemite_apiclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemite_apiclient
-Version: 0.73.0
+Version: 0.74.0
 Summary: A python API client for using Alchemite Analytics
 Home-page: 
 Author: Intellegens
 Author-email: Intellegens <support@intellegens.com>
 Project-URL: Homepage, https://intellegens.com
 Project-URL: Docs, https://docs.intellegens.com
 Keywords: Alchemite,Alchemite API,Machine Learning,Artificial Intelligence
@@ -25,15 +25,15 @@
 
 # alchemite-apiclient
 
 This is a client for interacting with Alchemite Analytics, an applied machine learning platform to accelerate industrial
 R&D and optimise manufacturing by extracting information from sparce or noisy datasets.
 To obtain a licence for this product, please [contact Intellegens](https://intellegens.com/contact-us/) for more information.
 
-API version: 0.73.0
+API version: 0.74.0
 
 ## Requirements.
 
 Python >=3.8
 
 ## Installation & Usage
 ### pip install
```

### Comparing `alchemite_apiclient-0.73.0/alchemite_apiclient.egg-info/SOURCES.txt` & `alchemite_apiclient-0.74.0/alchemite_apiclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 alchemite_apiclient/model/column_group_patch_request.py
 alchemite_apiclient/model/column_group_request.py
 alchemite_apiclient/model/column_group_response.py
 alchemite_apiclient/model/column_group_response_all_of.py
 alchemite_apiclient/model/column_info.py
 alchemite_apiclient/model/column_value.py
 alchemite_apiclient/model/column_value_nullable.py
+alchemite_apiclient/model/consistent_optimization_job.py
 alchemite_apiclient/model/continuous_column_info.py
 alchemite_apiclient/model/continuous_column_info_all_of.py
 alchemite_apiclient/model/continuous_column_info_stats.py
 alchemite_apiclient/model/continuous_model_column_info.py
 alchemite_apiclient/model/continuous_model_column_info_all_of.py
 alchemite_apiclient/model/data.py
 alchemite_apiclient/model/dataset.py
@@ -96,20 +97,24 @@
 alchemite_apiclient/model/drumap_reduction_type.py
 alchemite_apiclient/model/empty_categorical_column.py
 alchemite_apiclient/model/empty_continuous_column.py
 alchemite_apiclient/model/error.py
 alchemite_apiclient/model/get_all_opt_jobs.py
 alchemite_apiclient/model/get_optimize_done.py
 alchemite_apiclient/model/get_optimize_done_all_of.py
+alchemite_apiclient/model/get_optimize_done_consistent.py
 alchemite_apiclient/model/get_optimize_failed.py
 alchemite_apiclient/model/get_optimize_failed_all_of.py
+alchemite_apiclient/model/get_optimize_failed_consistent.py
 alchemite_apiclient/model/get_optimize_optimizing.py
 alchemite_apiclient/model/get_optimize_optimizing_all_of.py
+alchemite_apiclient/model/get_optimize_optimizing_consistent.py
 alchemite_apiclient/model/get_optimize_pending.py
 alchemite_apiclient/model/get_optimize_pending_all_of.py
+alchemite_apiclient/model/get_optimize_pending_consistent.py
 alchemite_apiclient/model/get_suggest_additional_done.py
 alchemite_apiclient/model/get_suggest_additional_done_all_of.py
 alchemite_apiclient/model/get_suggest_additional_failed.py
 alchemite_apiclient/model/get_suggest_additional_failed_all_of.py
 alchemite_apiclient/model/get_suggest_additional_pending.py
 alchemite_apiclient/model/get_suggest_additional_pending_all_of.py
 alchemite_apiclient/model/get_suggest_additional_running.py
@@ -139,21 +144,29 @@
 alchemite_apiclient/model/importance_request.py
 alchemite_apiclient/model/impute_request.py
 alchemite_apiclient/model/inline_response200.py
 alchemite_apiclient/model/inline_response2001.py
 alchemite_apiclient/model/inline_response2002.py
 alchemite_apiclient/model/inline_response2003.py
 alchemite_apiclient/model/inline_response2004.py
+alchemite_apiclient/model/inline_response2005.py
 alchemite_apiclient/model/int_cat_arr.py
 alchemite_apiclient/model/job_patch.py
+alchemite_apiclient/model/job_query.py
+alchemite_apiclient/model/jobs_metadata_filters.py
+alchemite_apiclient/model/jobs_metadata_sort.py
 alchemite_apiclient/model/load_request.py
 alchemite_apiclient/model/max.py
 alchemite_apiclient/model/metadata_optimization_job.py
+alchemite_apiclient/model/metadata_optimization_job_all_of.py
 alchemite_apiclient/model/metadata_suggest_additional_job.py
+alchemite_apiclient/model/metadata_suggest_additional_job_all_of.py
+alchemite_apiclient/model/metadata_suggest_additional_job_old.py
 alchemite_apiclient/model/metadata_suggest_historic_job.py
+alchemite_apiclient/model/metadata_suggest_historic_job_all_of.py
 alchemite_apiclient/model/min.py
 alchemite_apiclient/model/model.py
 alchemite_apiclient/model/model_column_info.py
 alchemite_apiclient/model/model_id_stub.py
 alchemite_apiclient/model/model_patch.py
 alchemite_apiclient/model/model_permitted_column_relationships.py
 alchemite_apiclient/model/model_query.py
@@ -190,29 +203,32 @@
 alchemite_apiclient/model/new_col_fn_arg_zero_if_zero_all_of.py
 alchemite_apiclient/model/new_columns.py
 alchemite_apiclient/model/non_empty_categorical_column.py
 alchemite_apiclient/model/non_empty_continuous_column.py
 alchemite_apiclient/model/non_empty_integer_categorical_column.py
 alchemite_apiclient/model/numerical_filter.py
 alchemite_apiclient/model/optimization_job.py
+alchemite_apiclient/model/optimize_parameters.py
 alchemite_apiclient/model/optimize_request.py
+alchemite_apiclient/model/optimize_request_all_of.py
 alchemite_apiclient/model/ot_sample_def_categorical.py
 alchemite_apiclient/model/ot_sample_def_continuous.py
 alchemite_apiclient/model/ot_sample_definition.py
 alchemite_apiclient/model/ot_set_inputs.py
 alchemite_apiclient/model/outliers_request.py
 alchemite_apiclient/model/output_tolerance_request.py
 alchemite_apiclient/model/output_tolerance_response.py
 alchemite_apiclient/model/output_tolerance_response_fixed_inputs.py
 alchemite_apiclient/model/output_tolerance_response_predicted_outputs.py
 alchemite_apiclient/model/output_tolerance_response_predictions.py
 alchemite_apiclient/model/output_tolerance_response_sampled_inputs.py
 alchemite_apiclient/model/output_tolerance_univariate_response.py
 alchemite_apiclient/model/part_dependent_columns.py
 alchemite_apiclient/model/part_get_optimize.py
+alchemite_apiclient/model/part_get_optimize_consistent.py
 alchemite_apiclient/model/part_get_optimize_done_result_array.py
 alchemite_apiclient/model/part_get_suggest_additional.py
 alchemite_apiclient/model/part_get_suggest_historic.py
 alchemite_apiclient/model/part_get_suggest_initial.py
 alchemite_apiclient/model/part_get_suggest_initial_sharing.py
 alchemite_apiclient/model/part_new_columns.py
 alchemite_apiclient/model/part_tar_fn_above.py
@@ -345,14 +361,15 @@
 docs/ColumnGroupPatchRequest.md
 docs/ColumnGroupRequest.md
 docs/ColumnGroupResponse.md
 docs/ColumnGroupResponseAllOf.md
 docs/ColumnInfo.md
 docs/ColumnValue.md
 docs/ColumnValueNullable.md
+docs/ConsistentOptimizationJob.md
 docs/ContinuousColumnInfo.md
 docs/ContinuousColumnInfoAllOf.md
 docs/ContinuousColumnInfoStats.md
 docs/ContinuousModelColumnInfo.md
 docs/ContinuousModelColumnInfoAllOf.md
 docs/Cosine.md
 docs/DRDatasetReductionData.md
@@ -402,20 +419,24 @@
 docs/EmptyContinuousColumn.md
 docs/Equal.md
 docs/Error.md
 docs/Exponentiation.md
 docs/GetAllOptJobs.md
 docs/GetOptimizeDone.md
 docs/GetOptimizeDoneAllOf.md
+docs/GetOptimizeDoneConsistent.md
 docs/GetOptimizeFailed.md
 docs/GetOptimizeFailedAllOf.md
+docs/GetOptimizeFailedConsistent.md
 docs/GetOptimizeOptimizing.md
 docs/GetOptimizeOptimizingAllOf.md
+docs/GetOptimizeOptimizingConsistent.md
 docs/GetOptimizePending.md
 docs/GetOptimizePendingAllOf.md
+docs/GetOptimizePendingConsistent.md
 docs/GetSuggestAdditionalDone.md
 docs/GetSuggestAdditionalDoneAllOf.md
 docs/GetSuggestAdditionalFailed.md
 docs/GetSuggestAdditionalFailedAllOf.md
 docs/GetSuggestAdditionalPending.md
 docs/GetSuggestAdditionalPendingAllOf.md
 docs/GetSuggestAdditionalRunning.md
@@ -450,33 +471,41 @@
 docs/ImportanceRequest.md
 docs/ImputeRequest.md
 docs/InlineResponse200.md
 docs/InlineResponse2001.md
 docs/InlineResponse2002.md
 docs/InlineResponse2003.md
 docs/InlineResponse2004.md
+docs/InlineResponse2005.md
 docs/IntCatArr.md
 docs/InverseCosine.md
 docs/InverseHyperbolicCosine.md
 docs/InverseHyperbolicSine.md
 docs/InverseHyperbolicTangent.md
 docs/InverseSine.md
 docs/InverseTangent.md
 docs/JobPatch.md
+docs/JobQuery.md
 docs/JobsApi.md
+docs/JobsMetadataFilters.md
+docs/JobsMetadataSort.md
 docs/Less.md
 docs/LessOrEqual.md
 docs/LoadRequest.md
 docs/Logarithm.md
 docs/Max.md
 docs/Maximum.md
 docs/Mean.md
 docs/MetadataOptimizationJob.md
+docs/MetadataOptimizationJobAllOf.md
 docs/MetadataSuggestAdditionalJob.md
+docs/MetadataSuggestAdditionalJobAllOf.md
+docs/MetadataSuggestAdditionalJobOld.md
 docs/MetadataSuggestHistoricJob.md
+docs/MetadataSuggestHistoricJobAllOf.md
 docs/MetricsApi.md
 docs/Min.md
 docs/Minimum.md
 docs/Model.md
 docs/ModelAnd.md
 docs/ModelColumnInfo.md
 docs/ModelDatasetApi.md
@@ -526,25 +555,28 @@
 docs/NotEqual.md
 docs/NumericalFilter.md
 docs/OTSampleDefCategorical.md
 docs/OTSampleDefContinuous.md
 docs/OTSampleDefinition.md
 docs/OTSetInputs.md
 docs/OptimizationJob.md
+docs/OptimizeParameters.md
 docs/OptimizeRequest.md
+docs/OptimizeRequestAllOf.md
 docs/OutliersRequest.md
 docs/OutputToleranceRequest.md
 docs/OutputToleranceResponse.md
 docs/OutputToleranceResponseFixedInputs.md
 docs/OutputToleranceResponsePredictedOutputs.md
 docs/OutputToleranceResponsePredictions.md
 docs/OutputToleranceResponseSampledInputs.md
 docs/OutputToleranceUnivariateResponse.md
 docs/PartDependentColumns.md
 docs/PartGetOptimize.md
+docs/PartGetOptimizeConsistent.md
 docs/PartGetOptimizeDoneResultArray.md
 docs/PartGetSuggestAdditional.md
 docs/PartGetSuggestHistoric.md
 docs/PartGetSuggestInitial.md
 docs/PartGetSuggestInitialSharing.md
 docs/PartNewColumns.md
 docs/PartTarFnAbove.md
```

### Comparing `alchemite_apiclient-0.73.0/docs/AbsoluteValue.md` & `alchemite_apiclient-0.74.0/docs/AbsoluteValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Addition.md` & `alchemite_apiclient-0.74.0/docs/Addition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/AdditiveSensitivityRequest.md` & `alchemite_apiclient-0.74.0/docs/AdditiveSensitivityRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/AnalyseValidateRequest.md` & `alchemite_apiclient-0.74.0/docs/AnalyseValidateRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/AnalyseValidateRequestAllOf.md` & `alchemite_apiclient-0.74.0/docs/AnalyseValidateRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/AnalyseValidateResponse.md` & `alchemite_apiclient-0.74.0/docs/AnalyseValidateResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/AnalyseValidateResponseColumnAnalytics.md` & `alchemite_apiclient-0.74.0/docs/AnalyseValidateResponseColumnAnalytics.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColBooleanExpression.md` & `alchemite_apiclient-0.74.0/docs/CalColBooleanExpression.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColBooleanLiteral.md` & `alchemite_apiclient-0.74.0/docs/CalColBooleanLiteral.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColComparison.md` & `alchemite_apiclient-0.74.0/docs/CalColComparison.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColConstant.md` & `alchemite_apiclient-0.74.0/docs/CalColConstant.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColExpression.md` & `alchemite_apiclient-0.74.0/docs/CalColExpression.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColIf.md` & `alchemite_apiclient-0.74.0/docs/CalColIf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColLiteral.md` & `alchemite_apiclient-0.74.0/docs/CalColLiteral.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColLogicalCombination.md` & `alchemite_apiclient-0.74.0/docs/CalColLogicalCombination.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColNumericOperation.md` & `alchemite_apiclient-0.74.0/docs/CalColNumericOperation.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CalColReference.md` & `alchemite_apiclient-0.74.0/docs/CalColReference.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CategoricalColumn.md` & `alchemite_apiclient-0.74.0/docs/CategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CategoricalColumnInfo.md` & `alchemite_apiclient-0.74.0/docs/CategoricalColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CategoricalColumnInfoAllOf.md` & `alchemite_apiclient-0.74.0/docs/CategoricalColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CategoricalColumnInfoStats.md` & `alchemite_apiclient-0.74.0/docs/CategoricalColumnInfoStats.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CategoricalModelColumnInfo.md` & `alchemite_apiclient-0.74.0/docs/CategoricalModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CategoricalModelColumnInfoAllOf.md` & `alchemite_apiclient-0.74.0/docs/CategoricalModelColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CategoricalPrediction.md` & `alchemite_apiclient-0.74.0/docs/CategoricalPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/CategoricalResult.md` & `alchemite_apiclient-0.74.0/docs/CategoricalResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ColumnGroupBatchRequest.md` & `alchemite_apiclient-0.74.0/docs/ColumnGroupBatchRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ColumnGroupPatchRequest.md` & `alchemite_apiclient-0.74.0/docs/ColumnGroupPatchRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ColumnGroupRequest.md` & `alchemite_apiclient-0.74.0/docs/ColumnGroupRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ColumnGroupResponse.md` & `alchemite_apiclient-0.74.0/docs/ColumnGroupResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ColumnGroupResponseAllOf.md` & `alchemite_apiclient-0.74.0/docs/ColumnGroupResponseAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ColumnInfo.md` & `alchemite_apiclient-0.74.0/docs/ColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ColumnValue.md` & `alchemite_apiclient-0.74.0/docs/ColumnValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ColumnValueNullable.md` & `alchemite_apiclient-0.74.0/docs/ColumnValueNullable.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ContinuousColumnInfo.md` & `alchemite_apiclient-0.74.0/docs/ContinuousColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ContinuousColumnInfoAllOf.md` & `alchemite_apiclient-0.74.0/docs/ContinuousColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ContinuousColumnInfoStats.md` & `alchemite_apiclient-0.74.0/docs/ContinuousColumnInfoStats.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ContinuousModelColumnInfo.md` & `alchemite_apiclient-0.74.0/docs/ContinuousModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ContinuousModelColumnInfoAllOf.md` & `alchemite_apiclient-0.74.0/docs/ContinuousModelColumnInfoAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Cosine.md` & `alchemite_apiclient-0.74.0/docs/Cosine.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRDatasetReductionData.md` & `alchemite_apiclient-0.74.0/docs/DRDatasetReductionData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRDatasetReductionMetadata.md` & `alchemite_apiclient-0.74.0/docs/DRDatasetReductionMetadata.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRDatasetReductionMetadataSources.md` & `alchemite_apiclient-0.74.0/docs/DRDatasetReductionMetadataSources.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRJobReductionMetadata.md` & `alchemite_apiclient-0.74.0/docs/DRJobReductionMetadata.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRJobReductionMetadataSources.md` & `alchemite_apiclient-0.74.0/docs/DRJobReductionMetadataSources.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRModelReductionData.md` & `alchemite_apiclient-0.74.0/docs/DRModelReductionData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRPCAReductionType.md` & `alchemite_apiclient-0.74.0/docs/DRPCAReductionType.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRThreeDimensionPoint.md` & `alchemite_apiclient-0.74.0/docs/DRThreeDimensionPoint.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRTwoDimensionPoint.md` & `alchemite_apiclient-0.74.0/docs/DRTwoDimensionPoint.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DRUMAPReductionType.md` & `alchemite_apiclient-0.74.0/docs/DRUMAPReductionType.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Data.md` & `alchemite_apiclient-0.74.0/docs/Data.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Dataset.md` & `alchemite_apiclient-0.74.0/docs/Dataset.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Dataset1.md` & `alchemite_apiclient-0.74.0/docs/Dataset1.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetCalculatedColumns.md` & `alchemite_apiclient-0.74.0/docs/DatasetCalculatedColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetChunk.md` & `alchemite_apiclient-0.74.0/docs/DatasetChunk.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetOrData.md` & `alchemite_apiclient-0.74.0/docs/DatasetOrData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetPatch.md` & `alchemite_apiclient-0.74.0/docs/DatasetPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetQuery.md` & `alchemite_apiclient-0.74.0/docs/DatasetQuery.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetQueryRequest.md` & `alchemite_apiclient-0.74.0/docs/DatasetQueryRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetQueryRequestRowIDs.md` & `alchemite_apiclient-0.74.0/docs/DatasetQueryRequestRowIDs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetQueryRequestSort.md` & `alchemite_apiclient-0.74.0/docs/DatasetQueryRequestSort.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetQueryResponseResult.md` & `alchemite_apiclient-0.74.0/docs/DatasetQueryResponseResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetSharing.md` & `alchemite_apiclient-0.74.0/docs/DatasetSharing.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetsApi.md` & `alchemite_apiclient-0.74.0/docs/DatasetsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetsMetadataFilters.md` & `alchemite_apiclient-0.74.0/docs/DatasetsMetadataFilters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DatasetsMetadataSort.md` & `alchemite_apiclient-0.74.0/docs/DatasetsMetadataSort.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DefaultApi.md` & `alchemite_apiclient-0.74.0/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgCol.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgCol.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgColWeights.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgColWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgConstantSum.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgConstantSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgProduct.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgProduct.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgRatio.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgSummandsWeights.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgSummandsWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgWeightedConstSum.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgWeightedConstSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgWeightedRatio.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgWeightedRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgZeroIfZero.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgZeroIfZero.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColFnArgZeroIfZeroAllOf.md` & `alchemite_apiclient-0.74.0/docs/DependentColFnArgZeroIfZeroAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DependentColumns.md` & `alchemite_apiclient-0.74.0/docs/DependentColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DimensionalityReductionRequest.md` & `alchemite_apiclient-0.74.0/docs/DimensionalityReductionRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/DimensionalityReductionResponse.md` & `alchemite_apiclient-0.74.0/docs/DimensionalityReductionResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Division.md` & `alchemite_apiclient-0.74.0/docs/Division.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/EmptyCategoricalColumn.md` & `alchemite_apiclient-0.74.0/docs/EmptyCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/EmptyContinuousColumn.md` & `alchemite_apiclient-0.74.0/docs/EmptyContinuousColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Equal.md` & `alchemite_apiclient-0.74.0/docs/Equal.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Error.md` & `alchemite_apiclient-0.74.0/docs/Error.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Exponentiation.md` & `alchemite_apiclient-0.74.0/docs/Exponentiation.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetOptimizeDone.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizeDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetOptimizeDoneAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizeDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetOptimizeFailed.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizeFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetOptimizeFailedAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizeFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetOptimizeOptimizing.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizeOptimizing.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetOptimizeOptimizingAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizeOptimizingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetOptimizePending.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizePending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetOptimizePendingAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizePendingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalDone.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalDoneAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalFailed.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalFailedAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalPending.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalPendingAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalPendingAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalRunning.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestAdditionalRunningAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestAdditionalRunningAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestHistoricDone.md` & `alchemite_apiclient-0.74.0/docs/MetadataSuggestAdditionalJob.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-# GetSuggestHistoricDone
+# MetadataSuggestAdditionalJob
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
+**model_id** | **str** | The ID of the model associated with the job. | 
 **id** | **str** |  | 
-**parameters** | [**SuggestHistoricParameters**](SuggestHistoricParameters.md) |  | 
-**result** | [**SuggestHistoricResult**](SuggestHistoricResult.md) |  | 
-**status** | **str** |  | defaults to "done"
+**parameters** | [**SuggestAdditionalParameters**](SuggestAdditionalParameters.md) |  | 
+**result** | [**SuggestAdditionalResult**](SuggestAdditionalResult.md) |  | 
+**detail** | **str** |  | 
+**status** | **str** |  | defaults to "failed"
+**type** | **str** |  | defaults to "suggest-additional"
 **name** | **str** | The job&#39;s name | [optional] 
 **tags** | **[str]** | The tags attached to the job | [optional] 
 **notes** | **str** | An optional free field for notes about the job. | [optional] 
 **enqueue_time** | **int** | The Unix Timestamp in seconds when the job enqueued. | [optional] [readonly] 
 **start_time** | **int** | The Unix Timestamp in seconds when the job started. | [optional] [readonly] 
 **end_time** | **int** | The Unix Timestamp in seconds when the job ended. | [optional] [readonly] 
+**progress** | **float** |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestHistoricDoneAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestHistoricDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestHistoricFailed.md` & `alchemite_apiclient-0.74.0/docs/MetadataSuggestHistoricJob.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-# GetSuggestHistoricFailed
+# MetadataSuggestHistoricJob
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
+**model_id** | **str** | The ID of the model associated with the job. | 
 **id** | **str** |  | 
-**parameters** | [**SuggestHistoricParameters**](SuggestHistoricParameters.md) |  | 
+**parameters** | **bool, date, datetime, dict, float, int, list, str, none_type** | The parameters as they were given to the suggest-historic request. | [readonly] 
+**result** | [**SuggestHistoricResult**](SuggestHistoricResult.md) |  | 
 **detail** | **str** |  | 
 **status** | **str** |  | defaults to "failed"
+**type** | **str** |  | defaults to "suggest-historic"
 **name** | **str** | The job&#39;s name | [optional] 
 **tags** | **[str]** | The tags attached to the job | [optional] 
 **notes** | **str** | An optional free field for notes about the job. | [optional] 
 **enqueue_time** | **int** | The Unix Timestamp in seconds when the job enqueued. | [optional] [readonly] 
 **start_time** | **int** | The Unix Timestamp in seconds when the job started. | [optional] [readonly] 
 **end_time** | **int** | The Unix Timestamp in seconds when the job ended. | [optional] [readonly] 
+**progress** | **float** |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestHistoricPending.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizePendingConsistent.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# GetSuggestHistoricPending
+# GetOptimizePendingConsistent
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **id** | **str** |  | 
-**parameters** | [**SuggestHistoricParameters**](SuggestHistoricParameters.md) |  | 
+**parameters** | **bool, date, datetime, dict, float, int, list, str, none_type** | The parameters as they were given to the optimize request. | [readonly] 
 **status** | **str** |  | defaults to "pending"
 **name** | **str** | The job&#39;s name | [optional] 
 **tags** | **[str]** | The tags attached to the job | [optional] 
 **notes** | **str** | An optional free field for notes about the job. | [optional] 
-**enqueue_time** | **int** | The Unix Timestamp in seconds when the job enqueued. | [optional] [readonly] 
-**start_time** | **int** | The Unix Timestamp in seconds when the job started. | [optional] [readonly] 
-**end_time** | **int** | The Unix Timestamp in seconds when the job ended. | [optional] [readonly] 
+**enqueue_time** | **int** | The Unix Timestamp in seconds when the optimize job enqueued. | [optional] [readonly] 
+**start_time** | **int** | The Unix Timestamp in seconds when the optimize job started. | [optional] [readonly] 
+**end_time** | **int** | The Unix Timestamp in seconds when the optimize job ended. | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestHistoricRunning.md` & `alchemite_apiclient-0.74.0/docs/GetOptimizeOptimizingConsistent.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# GetSuggestHistoricRunning
+# GetOptimizeOptimizingConsistent
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **id** | **str** |  | 
-**parameters** | [**SuggestHistoricParameters**](SuggestHistoricParameters.md) |  | 
-**status** | **str** |  | defaults to "running"
+**parameters** | **bool, date, datetime, dict, float, int, list, str, none_type** | The parameters as they were given to the optimize request. | [readonly] 
+**status** | **str** |  | defaults to "optimizing"
 **name** | **str** | The job&#39;s name | [optional] 
 **tags** | **[str]** | The tags attached to the job | [optional] 
 **notes** | **str** | An optional free field for notes about the job. | [optional] 
-**enqueue_time** | **int** | The Unix Timestamp in seconds when the job enqueued. | [optional] [readonly] 
-**start_time** | **int** | The Unix Timestamp in seconds when the job started. | [optional] [readonly] 
-**end_time** | **int** | The Unix Timestamp in seconds when the job ended. | [optional] [readonly] 
+**enqueue_time** | **int** | The Unix Timestamp in seconds when the optimize job enqueued. | [optional] [readonly] 
+**start_time** | **int** | The Unix Timestamp in seconds when the optimize job started. | [optional] [readonly] 
+**end_time** | **int** | The Unix Timestamp in seconds when the optimize job ended. | [optional] [readonly] 
 **progress** | **float** |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestInitialDone.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestInitialDone.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestInitialDoneAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestInitialDoneAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestInitialFailed.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestInitialFailed.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestInitialFailedAllOf.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestInitialFailedAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestInitialPending.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestInitialPending.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GetSuggestInitialRunning.md` & `alchemite_apiclient-0.74.0/docs/GetSuggestInitialRunning.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Greater.md` & `alchemite_apiclient-0.74.0/docs/Greater.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/GreaterOrEqual.md` & `alchemite_apiclient-0.74.0/docs/GreaterOrEqual.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HistogramContinuous.md` & `alchemite_apiclient-0.74.0/docs/HistogramContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HistogramRequest.md` & `alchemite_apiclient-0.74.0/docs/HistogramRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HistoricCategoricalPrediction.md` & `alchemite_apiclient-0.74.0/docs/HistoricCategoricalPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HistoricPrediction.md` & `alchemite_apiclient-0.74.0/docs/HistoricPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HistoricScalarPrediction.md` & `alchemite_apiclient-0.74.0/docs/HistoricScalarPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HistoricTargetFunction.md` & `alchemite_apiclient-0.74.0/docs/HistoricTargetFunction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HistoricValue.md` & `alchemite_apiclient-0.74.0/docs/HistoricValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HistoricVectorPrediction.md` & `alchemite_apiclient-0.74.0/docs/HistoricVectorPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HistoricVectorValue.md` & `alchemite_apiclient-0.74.0/docs/HistoricVectorValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HyperbolicCosine.md` & `alchemite_apiclient-0.74.0/docs/HyperbolicCosine.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HyperbolicSine.md` & `alchemite_apiclient-0.74.0/docs/HyperbolicSine.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/HyperbolicTangent.md` & `alchemite_apiclient-0.74.0/docs/HyperbolicTangent.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ImportanceRequest.md` & `alchemite_apiclient-0.74.0/docs/ImportanceRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ImputeRequest.md` & `alchemite_apiclient-0.74.0/docs/ImputeRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InlineResponse200.md` & `alchemite_apiclient-0.74.0/docs/InlineResponse200.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InlineResponse2001.md` & `alchemite_apiclient-0.74.0/docs/InlineResponse2001.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InlineResponse2002.md` & `alchemite_apiclient-0.74.0/docs/InlineResponse2002.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InlineResponse2003.md` & `alchemite_apiclient-0.74.0/docs/InlineResponse2003.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InlineResponse2004.md` & `alchemite_apiclient-0.74.0/docs/InlineResponse2004.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # InlineResponse2004
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **total** | **int** | Total number of jobs that matched the given query. Will not consider the offset or limit of the request, meaning this is the total number of jobs if no size restrictions were applied. | 
-**result** | [**[MetadataSuggestAdditionalJob]**](MetadataSuggestAdditionalJob.md) | Suggest-additional jobs matching the query, offset, and limit. | 
+**result** | [**[MetadataSuggestAdditionalJobOld]**](MetadataSuggestAdditionalJobOld.md) | Suggest-additional jobs matching the query, offset, and limit. | 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.73.0/docs/InverseCosine.md` & `alchemite_apiclient-0.74.0/docs/InverseCosine.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InverseHyperbolicCosine.md` & `alchemite_apiclient-0.74.0/docs/InverseHyperbolicCosine.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InverseHyperbolicSine.md` & `alchemite_apiclient-0.74.0/docs/InverseHyperbolicSine.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InverseHyperbolicTangent.md` & `alchemite_apiclient-0.74.0/docs/InverseHyperbolicTangent.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InverseSine.md` & `alchemite_apiclient-0.74.0/docs/InverseSine.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/InverseTangent.md` & `alchemite_apiclient-0.74.0/docs/InverseTangent.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/JobPatch.md` & `alchemite_apiclient-0.74.0/docs/JobPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/LessOrEqual.md` & `alchemite_apiclient-0.74.0/docs/LessOrEqual.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Logarithm.md` & `alchemite_apiclient-0.74.0/docs/Logarithm.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Max.md` & `alchemite_apiclient-0.74.0/docs/Max.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Maximum.md` & `alchemite_apiclient-0.74.0/docs/Maximum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Mean.md` & `alchemite_apiclient-0.74.0/docs/Mean.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/MetadataOptimizationJob.md` & `alchemite_apiclient-0.74.0/docs/MetadataOptimizationJob.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **model_id** | **str** | The ID of the model associated with the job. | 
 **id** | **str** |  | 
-**parameters** | [**OptimizeRequest**](OptimizeRequest.md) |  | 
+**parameters** | **bool, date, datetime, dict, float, int, list, str, none_type** | The parameters as they were given to the optimize request. | [readonly] 
 **result** | [**PartGetOptimizeDoneResultArray**](PartGetOptimizeDoneResultArray.md) |  | 
 **detail** | **str** |  | 
 **status** | **str** |  | defaults to "failed"
+**type** | **str** |  | defaults to "optimize"
+**name** | **str** | The job&#39;s name | [optional] 
+**tags** | **[str]** | The tags attached to the job | [optional] 
+**notes** | **str** | An optional free field for notes about the job. | [optional] 
 **enqueue_time** | **int** | The Unix Timestamp in seconds when the optimize job enqueued. | [optional] [readonly] 
 **start_time** | **int** | The Unix Timestamp in seconds when the optimize job started. | [optional] [readonly] 
 **end_time** | **int** | The Unix Timestamp in seconds when the optimize job ended. | [optional] [readonly] 
 **progress** | **float** |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.73.0/docs/MetadataSuggestAdditionalJob.md` & `alchemite_apiclient-0.74.0/docs/MetadataSuggestAdditionalJobOld.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# MetadataSuggestAdditionalJob
+# MetadataSuggestAdditionalJobOld
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **model_id** | **str** | The ID of the model associated with the job. | 
 **id** | **str** |  |
```

### Comparing `alchemite_apiclient-0.73.0/docs/MetadataSuggestHistoricJob.md` & `alchemite_apiclient-0.74.0/docs/SuggestHistoricJob.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# MetadataSuggestHistoricJob
+# SuggestHistoricJob
 
+The metadata and, if available, results for the job
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**model_id** | **str** | The ID of the model associated with the job. | 
-**id** | **str** |  | 
-**parameters** | [**SuggestHistoricParameters**](SuggestHistoricParameters.md) |  | 
-**result** | [**SuggestHistoricResult**](SuggestHistoricResult.md) |  | 
-**detail** | **str** |  | 
-**status** | **str** |  | defaults to "failed"
 **name** | **str** | The job&#39;s name | [optional] 
 **tags** | **[str]** | The tags attached to the job | [optional] 
 **notes** | **str** | An optional free field for notes about the job. | [optional] 
 **enqueue_time** | **int** | The Unix Timestamp in seconds when the job enqueued. | [optional] [readonly] 
 **start_time** | **int** | The Unix Timestamp in seconds when the job started. | [optional] [readonly] 
 **end_time** | **int** | The Unix Timestamp in seconds when the job ended. | [optional] [readonly] 
 **progress** | **float** |  | [optional] 
+**id** | **str** |  | [optional] 
+**parameters** | **bool, date, datetime, dict, float, int, list, str, none_type** | The parameters as they were given to the suggest-historic request. | [optional] [readonly] 
+**status** | **str** |  | [optional]  if omitted the server will use the default value of "failed"
+**result** | [**SuggestHistoricResult**](SuggestHistoricResult.md) |  | [optional] 
+**detail** | **str** |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.73.0/docs/MetricsApi.md` & `alchemite_apiclient-0.74.0/docs/MetricsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Min.md` & `alchemite_apiclient-0.74.0/docs/Min.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Minimum.md` & `alchemite_apiclient-0.74.0/docs/Minimum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Model.md` & `alchemite_apiclient-0.74.0/docs/Model.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelAnd.md` & `alchemite_apiclient-0.74.0/docs/ModelAnd.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelColumnInfo.md` & `alchemite_apiclient-0.74.0/docs/ModelColumnInfo.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelDatasetApi.md` & `alchemite_apiclient-0.74.0/docs/ModelDatasetApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelNot.md` & `alchemite_apiclient-0.74.0/docs/ModelNot.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelOr.md` & `alchemite_apiclient-0.74.0/docs/ModelOr.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelPatch.md` & `alchemite_apiclient-0.74.0/docs/ModelPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelPermittedColumnRelationships.md` & `alchemite_apiclient-0.74.0/docs/ModelPermittedColumnRelationships.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelSharing.md` & `alchemite_apiclient-0.74.0/docs/ModelSharing.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelsApi.md` & `alchemite_apiclient-0.74.0/docs/ModelsApi.md`

 * *Files 0% similar despite different names*

```diff
@@ -1320,38 +1320,15 @@
 
 # Please see readme for details about the contents of credentials.json
 # Enter a context with an instance of the API client
 with alchemite_apiclient.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = models_api.ModelsApi(api_client)
     id = "00112233-4455-6677-8899-aabbccddeeff" # str | Unique identifier for the model.
-    optimize_request = OptimizeRequest(
-        sample_definition=SampleDefinition(
-            key=None,
-        ),
-        target_function=TargetFunction(
-            key=None,
-        ),
-        new_columns=NewColumns([
-            None,
-        ]),
-        dependent_columns=DependentColumns([
-            None,
-        ]),
-        set_inputs=SetInputs(
-            key=None,
-        ),
-        num_optimization_samples=1000,
-        optimization_method="TPE",
-        name="name_example",
-        tags=[
-            "tags_example",
-        ],
-        notes="notes_example",
-    ) # OptimizeRequest | 
+    optimize_request = OptimizeRequest(None) # OptimizeRequest | 
 
     # example passing only required values which don't have defaults set
     try:
         # Optimize for specified targets using set of constraints
         api_response = api_instance.models_id_optimize_post(id, optimize_request)
         pprint(api_response)
     except alchemite_apiclient.ApiException as e:
```

### Comparing `alchemite_apiclient-0.73.0/docs/ModelsIdAdditiveSensitivityOrigin.md` & `alchemite_apiclient-0.74.0/docs/ModelsIdAdditiveSensitivityOrigin.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelsIdTrainPermittedColumnRelationships.md` & `alchemite_apiclient-0.74.0/docs/ModelsIdTrainPermittedColumnRelationships.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelsMetadataFilters.md` & `alchemite_apiclient-0.74.0/docs/ModelsMetadataFilters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ModelsMetadataSort.md` & `alchemite_apiclient-0.74.0/docs/ModelsMetadataSort.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Multiplication.md` & `alchemite_apiclient-0.74.0/docs/Multiplication.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgCol.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgCol.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgColAllOf.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgColAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgColWeights.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgColWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgColWeightsAllOf.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgColWeightsAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgColWeightsAllOfArguments.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgColWeightsAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgConstantSum.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgConstantSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgConstantSumAllOf.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgConstantSumAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgConstantSumAllOfArguments.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgConstantSumAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgProduct.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgProduct.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgProductAllOf.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgProductAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgProductAllOfArguments.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgProductAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgRatio.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgRatioAllOf.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgRatioAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgSummandsWeights.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgSummandsWeights.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgSummandsWeightsAllOf.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgSummandsWeightsAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgSummandsWeightsAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedConstSum.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedConstSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedConstSumAllOf.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedConstSumAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedConstSumAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedRatio.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedRatio.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedRatioAllOf.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedRatioAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgWeightedRatioAllOfArguments.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgWeightedRatioAllOfArguments.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgZeroIfZero.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgZeroIfZero.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColFnArgZeroIfZeroAllOf.md` & `alchemite_apiclient-0.74.0/docs/NewColFnArgZeroIfZeroAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NewColumns.md` & `alchemite_apiclient-0.74.0/docs/NewColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NonEmptyCategoricalColumn.md` & `alchemite_apiclient-0.74.0/docs/NonEmptyCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NonEmptyContinuousColumn.md` & `alchemite_apiclient-0.74.0/docs/NonEmptyContinuousColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NonEmptyIntegerCategoricalColumn.md` & `alchemite_apiclient-0.74.0/docs/NonEmptyIntegerCategoricalColumn.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NotEqual.md` & `alchemite_apiclient-0.74.0/docs/NotEqual.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/NumericalFilter.md` & `alchemite_apiclient-0.74.0/docs/NumericalFilter.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OTSampleDefCategorical.md` & `alchemite_apiclient-0.74.0/docs/OTSampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OTSampleDefContinuous.md` & `alchemite_apiclient-0.74.0/docs/OTSampleDefContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OTSampleDefinition.md` & `alchemite_apiclient-0.74.0/docs/OTSampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OptimizationJob.md` & `alchemite_apiclient-0.74.0/docs/OptimizationJob.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OptimizeRequest.md` & `alchemite_apiclient-0.74.0/docs/OptimizeRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OutliersRequest.md` & `alchemite_apiclient-0.74.0/docs/OutliersRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OutputToleranceRequest.md` & `alchemite_apiclient-0.74.0/docs/OutputToleranceRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OutputToleranceResponse.md` & `alchemite_apiclient-0.74.0/docs/OutputToleranceResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OutputToleranceResponseFixedInputs.md` & `alchemite_apiclient-0.74.0/docs/OutputToleranceResponseFixedInputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OutputToleranceResponsePredictedOutputs.md` & `alchemite_apiclient-0.74.0/docs/OutputToleranceResponsePredictedOutputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OutputToleranceResponsePredictions.md` & `alchemite_apiclient-0.74.0/docs/OutputToleranceResponsePredictions.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/OutputToleranceResponseSampledInputs.md` & `alchemite_apiclient-0.74.0/docs/OutputToleranceResponseSampledInputs.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartDependentColumns.md` & `alchemite_apiclient-0.74.0/docs/PartDependentColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartGetOptimize.md` & `alchemite_apiclient-0.74.0/docs/PartGetOptimize.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartGetSuggestAdditional.md` & `alchemite_apiclient-0.74.0/docs/PartGetSuggestAdditional.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartGetSuggestHistoric.md` & `alchemite_apiclient-0.74.0/docs/PartGetSuggestHistoric.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # PartGetSuggestHistoric
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **id** | **str** |  | 
-**parameters** | [**SuggestHistoricParameters**](SuggestHistoricParameters.md) |  | 
+**parameters** | **bool, date, datetime, dict, float, int, list, str, none_type** | The parameters as they were given to the suggest-historic request. | [readonly] 
 **name** | **str** | The job&#39;s name | [optional] 
 **tags** | **[str]** | The tags attached to the job | [optional] 
 **notes** | **str** | An optional free field for notes about the job. | [optional] 
 **enqueue_time** | **int** | The Unix Timestamp in seconds when the job enqueued. | [optional] [readonly] 
 **start_time** | **int** | The Unix Timestamp in seconds when the job started. | [optional] [readonly] 
 **end_time** | **int** | The Unix Timestamp in seconds when the job ended. | [optional] [readonly] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
```

### Comparing `alchemite_apiclient-0.73.0/docs/PartGetSuggestInitial.md` & `alchemite_apiclient-0.74.0/docs/PartGetSuggestInitial.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartGetSuggestInitialSharing.md` & `alchemite_apiclient-0.74.0/docs/PartGetSuggestInitialSharing.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartNewColumns.md` & `alchemite_apiclient-0.74.0/docs/PartNewColumns.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartTarFnBetween.md` & `alchemite_apiclient-0.74.0/docs/PartTarFnBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartTarFnCategoricals.md` & `alchemite_apiclient-0.74.0/docs/PartTarFnCategoricals.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartTarFnSingleTar.md` & `alchemite_apiclient-0.74.0/docs/PartTarFnSingleTar.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartTarFnSum.md` & `alchemite_apiclient-0.74.0/docs/PartTarFnSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PartTarFnWeightedSum.md` & `alchemite_apiclient-0.74.0/docs/PartTarFnWeightedSum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PredictRequest.md` & `alchemite_apiclient-0.74.0/docs/PredictRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/PredictTrendlineRequest.md` & `alchemite_apiclient-0.74.0/docs/PredictTrendlineRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Prediction.md` & `alchemite_apiclient-0.74.0/docs/Prediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Product.md` & `alchemite_apiclient-0.74.0/docs/Product.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Project.md` & `alchemite_apiclient-0.74.0/docs/Project.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ProjectBulkSuggestInitial.md` & `alchemite_apiclient-0.74.0/docs/ProjectBulkSuggestInitial.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ProjectPatch.md` & `alchemite_apiclient-0.74.0/docs/ProjectPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ProjectSharing.md` & `alchemite_apiclient-0.74.0/docs/ProjectSharing.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ProjectsApi.md` & `alchemite_apiclient-0.74.0/docs/ProjectsApi.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/QueryRequest.md` & `alchemite_apiclient-0.74.0/docs/QueryRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/QueryResponse.md` & `alchemite_apiclient-0.74.0/docs/QueryResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Range.md` & `alchemite_apiclient-0.74.0/docs/Range.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SISampleDefCategorical.md` & `alchemite_apiclient-0.74.0/docs/SISampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SISampleDefinition.md` & `alchemite_apiclient-0.74.0/docs/SISampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefCategorical.md` & `alchemite_apiclient-0.74.0/docs/SampleDefCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefCategoricalColumnValues.md` & `alchemite_apiclient-0.74.0/docs/SampleDefCategoricalColumnValues.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefComposition.md` & `alchemite_apiclient-0.74.0/docs/SampleDefComposition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefCompositionAllOf.md` & `alchemite_apiclient-0.74.0/docs/SampleDefCompositionAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefContinuous.md` & `alchemite_apiclient-0.74.0/docs/SampleDefContinuous.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefContinuousWithStart.md` & `alchemite_apiclient-0.74.0/docs/SampleDefContinuousWithStart.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefDiscrete.md` & `alchemite_apiclient-0.74.0/docs/SampleDefDiscrete.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefInteger.md` & `alchemite_apiclient-0.74.0/docs/SampleDefInteger.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefStartProp.md` & `alchemite_apiclient-0.74.0/docs/SampleDefStartProp.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefWeightedCategorical.md` & `alchemite_apiclient-0.74.0/docs/SampleDefWeightedCategorical.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SampleDefinition.md` & `alchemite_apiclient-0.74.0/docs/SampleDefinition.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ScalarPrediction.md` & `alchemite_apiclient-0.74.0/docs/ScalarPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ScalarResult.md` & `alchemite_apiclient-0.74.0/docs/ScalarResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SensitivityRequest.md` & `alchemite_apiclient-0.74.0/docs/SensitivityRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ShareGroup.md` & `alchemite_apiclient-0.74.0/docs/ShareGroup.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Sine.md` & `alchemite_apiclient-0.74.0/docs/Sine.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SquareRoot.md` & `alchemite_apiclient-0.74.0/docs/SquareRoot.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Subtraction.md` & `alchemite_apiclient-0.74.0/docs/Subtraction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestAdditionalJob.md` & `alchemite_apiclient-0.74.0/docs/SuggestAdditionalJob.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestAdditionalMetadataFilters.md` & `alchemite_apiclient-0.74.0/docs/SuggestAdditionalMetadataFilters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestAdditionalMetadataSort.md` & `alchemite_apiclient-0.74.0/docs/SuggestAdditionalMetadataSort.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestAdditionalParameters.md` & `alchemite_apiclient-0.74.0/docs/SuggestAdditionalParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestAdditionalParametersAllOf.md` & `alchemite_apiclient-0.74.0/docs/SuggestAdditionalParametersAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestAdditionalQuery.md` & `alchemite_apiclient-0.74.0/docs/SuggestAdditionalQuery.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestAdditionalRequest.md` & `alchemite_apiclient-0.74.0/docs/SuggestAdditionalRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestAdditionalRequestAllOf.md` & `alchemite_apiclient-0.74.0/docs/SuggestAdditionalRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestHistoricJob.md` & `alchemite_apiclient-0.74.0/docs/ConsistentOptimizationJob.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# SuggestHistoricJob
+# ConsistentOptimizationJob
 
 The metadata and, if available, results for the job
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **name** | **str** | The job&#39;s name | [optional] 
 **tags** | **[str]** | The tags attached to the job | [optional] 
 **notes** | **str** | An optional free field for notes about the job. | [optional] 
-**enqueue_time** | **int** | The Unix Timestamp in seconds when the job enqueued. | [optional] [readonly] 
-**start_time** | **int** | The Unix Timestamp in seconds when the job started. | [optional] [readonly] 
-**end_time** | **int** | The Unix Timestamp in seconds when the job ended. | [optional] [readonly] 
+**enqueue_time** | **int** | The Unix Timestamp in seconds when the optimize job enqueued. | [optional] [readonly] 
+**start_time** | **int** | The Unix Timestamp in seconds when the optimize job started. | [optional] [readonly] 
+**end_time** | **int** | The Unix Timestamp in seconds when the optimize job ended. | [optional] [readonly] 
 **progress** | **float** |  | [optional] 
 **id** | **str** |  | [optional] 
-**parameters** | [**SuggestHistoricParameters**](SuggestHistoricParameters.md) |  | [optional] 
+**parameters** | **bool, date, datetime, dict, float, int, list, str, none_type** | The parameters as they were given to the optimize request. | [optional] [readonly] 
 **status** | **str** |  | [optional]  if omitted the server will use the default value of "failed"
-**result** | [**SuggestHistoricResult**](SuggestHistoricResult.md) |  | [optional] 
+**result** | [**PartGetOptimizeDoneResultArray**](PartGetOptimizeDoneResultArray.md) |  | [optional] 
 **detail** | **str** |  | [optional] 
 **any string name** | **bool, date, datetime, dict, float, int, list, str, none_type** | any string name can be used but the value must be the correct type | [optional]
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestHistoricParameters.md` & `alchemite_apiclient-0.74.0/docs/SuggestHistoricParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestHistoricRequest.md` & `alchemite_apiclient-0.74.0/docs/SuggestHistoricRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestHistoricResult.md` & `alchemite_apiclient-0.74.0/docs/SuggestHistoricResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestHistoricResultSamples.md` & `alchemite_apiclient-0.74.0/docs/SuggestHistoricResultSamples.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestInitialJobPatch.md` & `alchemite_apiclient-0.74.0/docs/SuggestInitialJobPatch.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestInitialParameters.md` & `alchemite_apiclient-0.74.0/docs/SuggestInitialParameters.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestInitialRequest.md` & `alchemite_apiclient-0.74.0/docs/SuggestInitialRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestInitialRequestAllOf.md` & `alchemite_apiclient-0.74.0/docs/SuggestInitialRequestAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestInitialResponse.md` & `alchemite_apiclient-0.74.0/docs/SuggestInitialResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingCommon.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingCommon.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingData.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingDataAllOf.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingDataAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingDatasetID.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingDatasetID.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingDatasetIDAllOf.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingDatasetIDAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingImputedData.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingImputedData.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingImputedDataAllOf.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingImputedDataAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingRequest.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingResponse.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/SuggestMissingSpecific.md` & `alchemite_apiclient-0.74.0/docs/SuggestMissingSpecific.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Sum.md` & `alchemite_apiclient-0.74.0/docs/Sum.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Tangent.md` & `alchemite_apiclient-0.74.0/docs/Tangent.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnAbove.md` & `alchemite_apiclient-0.74.0/docs/TarFnAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnAboveAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnBelow.md` & `alchemite_apiclient-0.74.0/docs/TarFnBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnBelowAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnBetween.md` & `alchemite_apiclient-0.74.0/docs/TarFnBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnBetweenAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnExcludeCategories.md` & `alchemite_apiclient-0.74.0/docs/TarFnExcludeCategories.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnExcludeCategoriesAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnExcludeCategoriesAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnIncludeCategories.md` & `alchemite_apiclient-0.74.0/docs/TarFnIncludeCategories.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnIncludeCategoriesAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnIncludeCategoriesAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnSumAbove.md` & `alchemite_apiclient-0.74.0/docs/TarFnSumAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnSumAboveAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnSumAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnSumBelow.md` & `alchemite_apiclient-0.74.0/docs/TarFnSumBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnSumBelowAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnSumBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnSumBetween.md` & `alchemite_apiclient-0.74.0/docs/TarFnSumBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnSumBetweenAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnSumBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnWeightedSumAbove.md` & `alchemite_apiclient-0.74.0/docs/TarFnWeightedSumAbove.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnWeightedSumAboveAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnWeightedSumAboveAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnWeightedSumBelow.md` & `alchemite_apiclient-0.74.0/docs/TarFnWeightedSumBelow.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnWeightedSumBelowAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnWeightedSumBelowAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnWeightedSumBetween.md` & `alchemite_apiclient-0.74.0/docs/TarFnWeightedSumBetween.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TarFnWeightedSumBetweenAllOf.md` & `alchemite_apiclient-0.74.0/docs/TarFnWeightedSumBetweenAllOf.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TargetFunction.md` & `alchemite_apiclient-0.74.0/docs/TargetFunction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TrainRequest.md` & `alchemite_apiclient-0.74.0/docs/TrainRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/TrainingValidationPredictionRequest.md` & `alchemite_apiclient-0.74.0/docs/TrainingValidationPredictionRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ValidateRequest.md` & `alchemite_apiclient-0.74.0/docs/ValidateRequest.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/ValidationSplit.md` & `alchemite_apiclient-0.74.0/docs/ValidationSplit.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/Value.md` & `alchemite_apiclient-0.74.0/docs/Value.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/VectorPrediction.md` & `alchemite_apiclient-0.74.0/docs/VectorPrediction.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/VectorResult.md` & `alchemite_apiclient-0.74.0/docs/VectorResult.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/VectorValue.md` & `alchemite_apiclient-0.74.0/docs/VectorValue.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/docs/VersionResponse.md` & `alchemite_apiclient-0.74.0/docs/VersionResponse.md`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/adrenergic.csv` & `alchemite_apiclient-0.74.0/example/adrenergic.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/adrenergic_holdout.csv` & `alchemite_apiclient-0.74.0/example/adrenergic_holdout.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/adrenergic_row.csv` & `alchemite_apiclient-0.74.0/example/adrenergic_row.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/categorical.csv` & `alchemite_apiclient-0.74.0/example/categorical.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_additive_sensitivity.py` & `alchemite_apiclient-0.74.0/example/example_additive_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_basic.py` & `alchemite_apiclient-0.74.0/example/example_basic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_calculated.py` & `alchemite_apiclient-0.74.0/example/example_calculated.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_categorical.py` & `alchemite_apiclient-0.74.0/example/example_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_chunk.py` & `alchemite_apiclient-0.74.0/example/example_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_column_groups.py` & `alchemite_apiclient-0.74.0/example/example_column_groups.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_connect.py` & `alchemite_apiclient-0.74.0/example/example_connect.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_custom_validation_splits.py` & `alchemite_apiclient-0.74.0/example/example_custom_validation_splits.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_delete.py` & `alchemite_apiclient-0.74.0/example/example_delete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_dimensionality_reduction.py` & `alchemite_apiclient-0.74.0/example/example_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_download.py` & `alchemite_apiclient-0.74.0/example/example_download.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_histogram.py` & `alchemite_apiclient-0.74.0/example/example_histogram.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_hyperopt.py` & `alchemite_apiclient-0.74.0/example/example_hyperopt.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_importance.py` & `alchemite_apiclient-0.74.0/example/example_importance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_metadata.py` & `alchemite_apiclient-0.74.0/example/example_metadata.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_optimize.py` & `alchemite_apiclient-0.74.0/example/example_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_outliers.py` & `alchemite_apiclient-0.74.0/example/example_outliers.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_output_tolerance.py` & `alchemite_apiclient-0.74.0/example/example_output_tolerance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_predict_trendline.py` & `alchemite_apiclient-0.74.0/example/example_predict_trendline.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_preload.py` & `alchemite_apiclient-0.74.0/example/example_preload.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_project.py` & `alchemite_apiclient-0.74.0/example/example_project.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_query.py` & `alchemite_apiclient-0.74.0/example/example_query.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_report.py` & `alchemite_apiclient-0.74.0/example/example_report.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_sensitivity.py` & `alchemite_apiclient-0.74.0/example/example_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_suggest_additional.py` & `alchemite_apiclient-0.74.0/example/example_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_suggest_historic.py` & `alchemite_apiclient-0.74.0/example/example_suggest_historic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_suggest_initial.py` & `alchemite_apiclient-0.74.0/example/example_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_suggest_missing.py` & `alchemite_apiclient-0.74.0/example/example_suggest_missing.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_training_outliers.py` & `alchemite_apiclient-0.74.0/example/example_training_outliers.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_validate.py` & `alchemite_apiclient-0.74.0/example/example_validate.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_validation_request.py` & `alchemite_apiclient-0.74.0/example/example_validation_request.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/example_vector.py` & `alchemite_apiclient-0.74.0/example/example_vector.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/optimize_args_steel.json` & `alchemite_apiclient-0.74.0/example/optimize_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/optimize_dependentColumns_args_steel.json` & `alchemite_apiclient-0.74.0/example/optimize_dependentColumns_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/steels.csv` & `alchemite_apiclient-0.74.0/example/steels.csv`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/example/suggest_additional_args_steel.json` & `alchemite_apiclient-0.74.0/example/suggest_additional_args_steel.json`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/pyproject.toml` & `alchemite_apiclient-0.74.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alchemite_apiclient"
-version = "0.73.0"
+version = "0.74.0"
 authors = [
   { name="Intellegens", email="support@intellegens.com" },
 ]
 description = "A python API client for using Alchemite Analytics"
 keywords = ["Alchemite", "Alchemite API", "Machine Learning", "Artificial Intelligence"]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `alchemite_apiclient-0.73.0/setup.py` & `alchemite_apiclient-0.74.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "alchemite-apiclient"
-VERSION = "0.73.0"
+VERSION = "0.74.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `alchemite_apiclient-0.73.0/test/test_additive_sensitivity.py` & `alchemite_apiclient-0.74.0/test/test_additive_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_basic.py` & `alchemite_apiclient-0.74.0/test/test_basic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_categorical.py` & `alchemite_apiclient-0.74.0/test/test_categorical.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_cce.py` & `alchemite_apiclient-0.74.0/test/test_cce.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_chunk.py` & `alchemite_apiclient-0.74.0/test/test_chunk.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_column_groups.py` & `alchemite_apiclient-0.74.0/test/test_column_groups.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_cornercases.py` & `alchemite_apiclient-0.74.0/test/test_cornercases.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_custom_validation_splits.py` & `alchemite_apiclient-0.74.0/test/test_custom_validation_splits.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_delete.py` & `alchemite_apiclient-0.74.0/test/test_delete.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_dimensionality_reduction.py` & `alchemite_apiclient-0.74.0/test/test_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_download.py` & `alchemite_apiclient-0.74.0/test/test_download.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_examples.py` & `alchemite_apiclient-0.74.0/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_formulae.py` & `alchemite_apiclient-0.74.0/test/test_formulae.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_hyperopt.py` & `alchemite_apiclient-0.74.0/test/test_hyperopt.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_importance.py` & `alchemite_apiclient-0.74.0/test/test_importance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_optimize.py` & `alchemite_apiclient-0.74.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_output_tolerance.py` & `alchemite_apiclient-0.74.0/test/test_output_tolerance.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_preload.py` & `alchemite_apiclient-0.74.0/test/test_preload.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_query.py` & `alchemite_apiclient-0.74.0/test/test_query.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_sensitivity.py` & `alchemite_apiclient-0.74.0/test/test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_suggest_additional.py` & `alchemite_apiclient-0.74.0/test/test_suggest_additional.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_suggest_historic.py` & `alchemite_apiclient-0.74.0/test/test_suggest_historic.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_suggest_initial.py` & `alchemite_apiclient-0.74.0/test/test_suggest_initial.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_validate.py` & `alchemite_apiclient-0.74.0/test/test_validate.py`

 * *Files identical despite different names*

### Comparing `alchemite_apiclient-0.73.0/test/test_vector.py` & `alchemite_apiclient-0.74.0/test/test_vector.py`

 * *Files identical despite different names*


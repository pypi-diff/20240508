# Comparing `tmp/brickflows-0.9.1.tar.gz` & `tmp/brickflows-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brickflows-0.9.1.tar", max compression
+gzip compressed data, was "brickflows-0.9.2.tar", max compression
```

## Comparing `brickflows-0.9.1.tar` & `brickflows-0.9.2.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0    11357 2023-08-11 01:43:57.947290 brickflows-0.9.1/LICENSE
--rw-r--r--   0        0        0     1678 2023-08-11 01:43:57.947290 brickflows-0.9.1/README.md
--rw-r--r--   0        0        0    10685 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/__init__.py
--rw-r--r--   0        0        0        0 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/bundles/__init__.py
--rw-r--r--   0        0        0    99617 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/bundles/model.py
--rw-r--r--   0        0        0    12544 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/cli/__init__.py
--rw-r--r--   0        0        0     7146 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/cli/bundles.py
--rw-r--r--   0        0        0     1697 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/cli/commands.py
--rw-r--r--   0        0        0     5427 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/cli/configure.py
--rw-r--r--   0        0        0      314 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/cli/constants.py
--rw-r--r--   0        0        0      733 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/cli/entrypoint.template
--rw-r--r--   0        0        0     1007 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/cli/gitignore_template.txt
--rw-r--r--   0        0        0    20684 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/cli/projects.py
--rw-r--r--   0        0        0     1772 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/codegen/__init__.py
--rw-r--r--   0        0        0     2847 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/codegen/cdktf_aspects.py
--rw-r--r--   0        0        0    23669 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/codegen/databricks_bundle.py
--rw-r--r--   0        0        0     9012 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/codegen/hashicorp_cdktf.py
--rw-r--r--   0        0        0      530 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/context/__init__.py
--rw-r--r--   0        0        0    15256 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/context/context.py
--rw-r--r--   0        0        0     1370 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/engine/__init__.py
--rw-r--r--   0        0        0     7527 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/engine/compute.py
--rw-r--r--   0        0        0      987 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/engine/hooks.py
--rw-r--r--   0        0        0    12666 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/engine/project.py
--rw-r--r--   0        0        0    26936 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/engine/task.py
--rw-r--r--   0        0        0      825 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/engine/utils.py
--rw-r--r--   0        0        0    14321 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/engine/workflow.py
--rw-r--r--   0        0        0       78 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/hints/__init__.py
--rw-r--r--   0        0        0      151 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/hints/hint.py
--rw-r--r--   0        0        0       85 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/hints/py.typed
--rw-r--r--   0        0        0     2639 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/resolver/__init__.py
--rw-r--r--   0        0        0       48 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/tf/__init__.py
--rw-r--r--   0        0        0     6300 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/tf/databricks/__init__.py
--rw-r--r--   0        0        0      385 2023-08-11 01:43:57.947290 brickflows-0.9.1/brickflow/tf/databricks/_jsii/__init__.py
--rw-r--r--   0        0        0  1419975 2023-08-11 01:43:57.955290 brickflows-0.9.1/brickflow/tf/databricks/_jsii/databricks@0.0.0.jsii.tgz
--rw-r--r--   0        0        0    24222 2023-08-11 01:43:57.955290 brickflows-0.9.1/brickflow/tf/databricks/aws_s3_mount/__init__.py
--rw-r--r--   0        0        0    35846 2023-08-11 01:43:57.955290 brickflows-0.9.1/brickflow/tf/databricks/azure_adls_gen1_mount/__init__.py
--rw-r--r--   0        0        0    38484 2023-08-11 01:43:57.955290 brickflows-0.9.1/brickflow/tf/databricks/azure_adls_gen2_mount/__init__.py
--rw-r--r--   0        0        0    33033 2023-08-11 01:43:57.955290 brickflows-0.9.1/brickflow/tf/databricks/azure_blob_mount/__init__.py
--rw-r--r--   0        0        0    35859 2023-08-11 01:43:57.955290 brickflows-0.9.1/brickflow/tf/databricks/catalog/__init__.py
--rw-r--r--   0        0        0   356377 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/cluster/__init__.py
--rw-r--r--   0        0        0    22801 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/cluster_policy/__init__.py
--rw-r--r--   0        0        0    24053 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_aws_assume_role_policy/__init__.py
--rw-r--r--   0        0        0    25692 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_aws_bucket_policy/__init__.py
--rw-r--r--   0        0        0    18317 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_aws_crossaccount_policy/__init__.py
--rw-r--r--   0        0        0    17510 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_catalogs/__init__.py
--rw-r--r--   0        0        0   383999 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_cluster/__init__.py
--rw-r--r--   0        0        0    17678 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_cluster_policy/__init__.py
--rw-r--r--   0        0        0    18153 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_clusters/__init__.py
--rw-r--r--   0        0        0    16415 2023-08-11 01:43:57.959290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_current_user/__init__.py
--rw-r--r--   0        0        0    20280 2023-08-11 01:43:57.963290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_dbfs_file/__init__.py
--rw-r--r--   0        0        0    29262 2023-08-11 01:43:57.963290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_dbfs_file_paths/__init__.py
--rw-r--r--   0        0        0    19416 2023-08-11 01:43:57.963290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_directory/__init__.py
--rw-r--r--   0        0        0    50299 2023-08-11 01:43:57.963290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_group/__init__.py
--rw-r--r--   0        0        0   208643 2023-08-11 01:43:57.963290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_instance_pool/__init__.py
--rw-r--r--   0        0        0  1487868 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_job/__init__.py
--rw-r--r--   0        0        0    17582 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_jobs/__init__.py
--rw-r--r--   0        0        0    17885 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_mws_credentials/__init__.py
--rw-r--r--   0        0        0    17844 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_mws_workspaces/__init__.py
--rw-r--r--   0        0        0    50750 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_node_type/__init__.py
--rw-r--r--   0        0        0    26006 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_notebook/__init__.py
--rw-r--r--   0        0        0    29431 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_notebook_paths/__init__.py
--rw-r--r--   0        0        0    19580 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_schemas/__init__.py
--rw-r--r--   0        0        0    32010 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_service_principal/__init__.py
--rw-r--r--   0        0        0    20943 2023-08-11 01:43:57.967290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_service_principals/__init__.py
--rw-r--r--   0        0        0    89539 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_share/__init__.py
--rw-r--r--   0        0        0    17560 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_shares/__init__.py
--rw-r--r--   0        0        0    42275 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_spark_version/__init__.py
--rw-r--r--   0        0        0    95058 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_sql_warehouse/__init__.py
--rw-r--r--   0        0        0    20451 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_sql_warehouses/__init__.py
--rw-r--r--   0        0        0    21596 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_tables/__init__.py
--rw-r--r--   0        0        0    20644 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_user/__init__.py
--rw-r--r--   0        0        0    21555 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_views/__init__.py
--rw-r--r--   0        0        0    15594 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/data_databricks_zones/__init__.py
--rw-r--r--   0        0        0    23774 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/dbfs_file/__init__.py
--rw-r--r--   0        0        0    22201 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/directory/__init__.py
--rw-r--r--   0        0        0    35163 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/entitlements/__init__.py
--rw-r--r--   0        0        0    30935 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/external_location/__init__.py
--rw-r--r--   0        0        0    25028 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/git_credential/__init__.py
--rw-r--r--   0        0        0    34318 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/global_init_script/__init__.py
--rw-r--r--   0        0        0    53757 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/grants/__init__.py
--rw-r--r--   0        0        0    36782 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/group/__init__.py
--rw-r--r--   0        0        0    19757 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/group_instance_profile/__init__.py
--rw-r--r--   0        0        0    19102 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/group_member/__init__.py
--rw-r--r--   0        0        0    18873 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/group_role/__init__.py
--rw-r--r--   0        0        0   167050 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/instance_pool/__init__.py
--rw-r--r--   0        0        0    26435 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/instance_profile/__init__.py
--rw-r--r--   0        0        0    24075 2023-08-11 01:43:57.971290 brickflows-0.9.1/brickflow/tf/databricks/ip_access_list/__init__.py
--rw-r--r--   0        0        0  1379143 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/job/__init__.py
--rw-r--r--   0        0        0    52597 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/library/__init__.py
--rw-r--r--   0        0        0    51913 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/metastore/__init__.py
--rw-r--r--   0        0        0    22270 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/metastore_assignment/__init__.py
--rw-r--r--   0        0        0    77162 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/metastore_data_access/__init__.py
--rw-r--r--   0        0        0    37293 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/mlflow_experiment/__init__.py
--rw-r--r--   0        0        0    45677 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/mlflow_model/__init__.py
--rw-r--r--   0        0        0    51243 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/mlflow_webhook/__init__.py
--rw-r--r--   0        0        0    79706 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/model_serving/__init__.py
--rw-r--r--   0        0        0   117494 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/mount/__init__.py
--rw-r--r--   0        0        0    22015 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/mws_credentials/__init__.py
--rw-r--r--   0        0        0    45478 2023-08-11 01:43:57.979290 brickflows-0.9.1/brickflow/tf/databricks/mws_customer_managed_keys/__init__.py
--rw-r--r--   0        0        0    40817 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/mws_log_delivery/__init__.py
--rw-r--r--   0        0        0    82561 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/mws_networks/__init__.py
--rw-r--r--   0        0        0    22040 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/mws_permission_assignment/__init__.py
--rw-r--r--   0        0        0    36697 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/mws_private_access_settings/__init__.py
--rw-r--r--   0        0        0    22716 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/mws_storage_configurations/__init__.py
--rw-r--r--   0        0        0    54494 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/mws_vpc_endpoint/__init__.py
--rw-r--r--   0        0        0   144041 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/mws_workspaces/__init__.py
--rw-r--r--   0        0        0    32345 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/notebook/__init__.py
--rw-r--r--   0        0        0    22022 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/obo_token/__init__.py
--rw-r--r--   0        0        0    19781 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/permission_assignment/__init__.py
--rw-r--r--   0        0        0    81600 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/permissions/__init__.py
--rw-r--r--   0        0        0   303704 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/pipeline/__init__.py
--rw-r--r--   0        0        0    70803 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/provider/__init__.py
--rw-r--r--   0        0        0    23878 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/provider_resource/__init__.py
--rw-r--r--   0        0        0        1 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/py.typed
--rw-r--r--   0        0        0    62588 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/recipient/__init__.py
--rw-r--r--   0        0        0    35117 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/repo/__init__.py
--rw-r--r--   0        0        0    33244 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/schema/__init__.py
--rw-r--r--   0        0        0    21077 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/secret/__init__.py
--rw-r--r--   0        0        0    20955 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/secret_acl/__init__.py
--rw-r--r--   0        0        0    32103 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/secret_scope/__init__.py
--rw-r--r--   0        0        0    51654 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/service_principal/__init__.py
--rw-r--r--   0        0        0    19664 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/service_principal_role/__init__.py
--rw-r--r--   0        0        0    22252 2023-08-11 01:43:57.983290 brickflows-0.9.1/brickflow/tf/databricks/service_principal_secret/__init__.py
--rw-r--r--   0        0        0    87031 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/share/__init__.py
--rw-r--r--   0        0        0    40696 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/sql_alert/__init__.py
--rw-r--r--   0        0        0    21407 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/sql_dashboard/__init__.py
--rw-r--r--   0        0        0   101946 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/sql_endpoint/__init__.py
--rw-r--r--   0        0        0    29766 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/sql_global_config/__init__.py
--rw-r--r--   0        0        0    50873 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/sql_permissions/__init__.py
--rw-r--r--   0        0        0   216752 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/sql_query/__init__.py
--rw-r--r--   0        0        0    30068 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/sql_visualization/__init__.py
--rw-r--r--   0        0        0    68475 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/sql_widget/__init__.py
--rw-r--r--   0        0        0    75666 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/storage_credential/__init__.py
--rw-r--r--   0        0        0    73232 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/table/__init__.py
--rw-r--r--   0        0        0    26507 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/token/__init__.py
--rw-r--r--   0        0        0    49965 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/user/__init__.py
--rw-r--r--   0        0        0    19689 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/user_instance_profile/__init__.py
--rw-r--r--   0        0        0    18805 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/user_role/__init__.py
--rw-r--r--   0        0        0    17999 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/databricks/workspace_conf/__init__.py
--rw-r--r--   0        0        0      598 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/random/__init__.py
--rw-r--r--   0        0        0      377 2023-08-11 01:43:57.987290 brickflows-0.9.1/brickflow/tf/random/_jsii/__init__.py
--rw-r--r--   0        0        0  1205649 2023-08-11 01:43:57.991290 brickflows-0.9.1/brickflow/tf/random/_jsii/random@0.0.0.jsii.tgz
--rw-r--r--   0        0        0    20651 2023-08-11 01:43:57.991290 brickflows-0.9.1/brickflow/tf/random/id/__init__.py
--rw-r--r--   0        0        0    21403 2023-08-11 01:43:57.991290 brickflows-0.9.1/brickflow/tf/random/integer/__init__.py
--rw-r--r--   0        0        0    46047 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow/tf/random/password/__init__.py
--rw-r--r--   0        0        0    22022 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow/tf/random/pet/__init__.py
--rw-r--r--   0        0        0     5304 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow/tf/random/provider/__init__.py
--rw-r--r--   0        0        0        1 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow/tf/random/py.typed
--rw-r--r--   0        0        0    23921 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow/tf/random/shuffle/__init__.py
--rw-r--r--   0        0        0    46058 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow/tf/random/string_resource/__init__.py
--rw-r--r--   0        0        0    15398 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow/tf/random/uuid/__init__.py
--rw-r--r--   0        0        0     1636 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/__init__.py
--rw-r--r--   0        0        0     2558 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/brickflow_task_plugin.py
--rw-r--r--   0        0        0     2786 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/context/__init__.py
--rw-r--r--   0        0        0   176743 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/cron-utils-9.2.0.jar
--rw-r--r--   0        0        0     3572 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/cronhelper.py
--rw-r--r--   0        0        0     5808 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/operators/__init__.py
--rw-r--r--   0        0        0     7338 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/operators/external_tasks.py
--rw-r--r--   0        0        0     3644 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/operators/native_operators.py
--rw-r--r--   0        0        0        0 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/vendor/__init__.py
--rw-r--r--   0        0        0     3238 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/vendor/context.py
--rw-r--r--   0        0        0    12073 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/vendor/timetable.py
--rw-r--r--   0        0        0     7647 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/airflow/vendor/timezone.py
--rw-r--r--   0        0        0        0 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/databricks/__init__.py
--rw-r--r--   0        0        0     5633 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/databricks/workflow_dependency_sensor.py
--rw-r--r--   0        0        0     5500 2023-08-11 01:43:57.995290 brickflows-0.9.1/brickflow_plugins/secrets/__init__.py
--rw-r--r--   0        0        0     3084 2023-08-11 01:45:11.387931 brickflows-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2862 1970-01-01 00:00:00.000000 brickflows-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-11 02:52:07.964040 brickflows-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1678 2023-08-11 02:52:07.964040 brickflows-0.9.2/README.md
+-rw-r--r--   0        0        0    10685 2023-08-11 02:52:07.964040 brickflows-0.9.2/brickflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-11 02:52:07.964040 brickflows-0.9.2/brickflow/bundles/__init__.py
+-rw-r--r--   0        0        0    99617 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/bundles/model.py
+-rw-r--r--   0        0        0    12547 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/cli/__init__.py
+-rw-r--r--   0        0        0     7146 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/cli/bundles.py
+-rw-r--r--   0        0        0     1697 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/cli/commands.py
+-rw-r--r--   0        0        0     5427 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/cli/configure.py
+-rw-r--r--   0        0        0      314 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/cli/constants.py
+-rw-r--r--   0        0        0      733 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/cli/entrypoint.template
+-rw-r--r--   0        0        0     1007 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/cli/gitignore_template.txt
+-rw-r--r--   0        0        0    20684 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/cli/projects.py
+-rw-r--r--   0        0        0     1816 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/codegen/__init__.py
+-rw-r--r--   0        0        0     2847 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/codegen/cdktf_aspects.py
+-rw-r--r--   0        0        0    23790 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/codegen/databricks_bundle.py
+-rw-r--r--   0        0        0     9012 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/codegen/hashicorp_cdktf.py
+-rw-r--r--   0        0        0      530 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/context/__init__.py
+-rw-r--r--   0        0        0    15256 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/context/context.py
+-rw-r--r--   0        0        0     1370 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/engine/__init__.py
+-rw-r--r--   0        0        0     7527 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/engine/compute.py
+-rw-r--r--   0        0        0      987 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/engine/hooks.py
+-rw-r--r--   0        0        0    12666 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/engine/project.py
+-rw-r--r--   0        0        0    26936 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/engine/task.py
+-rw-r--r--   0        0        0      825 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/engine/utils.py
+-rw-r--r--   0        0        0    14321 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/engine/workflow.py
+-rw-r--r--   0        0        0       78 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/hints/__init__.py
+-rw-r--r--   0        0        0      151 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/hints/hint.py
+-rw-r--r--   0        0        0       85 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/hints/py.typed
+-rw-r--r--   0        0        0     2639 2023-08-11 02:52:07.968040 brickflows-0.9.2/brickflow/resolver/__init__.py
+-rw-r--r--   0        0        0       48 2023-08-11 02:52:07.972040 brickflows-0.9.2/brickflow/tf/__init__.py
+-rw-r--r--   0        0        0     6300 2023-08-11 02:52:07.972040 brickflows-0.9.2/brickflow/tf/databricks/__init__.py
+-rw-r--r--   0        0        0      385 2023-08-11 02:52:07.972040 brickflows-0.9.2/brickflow/tf/databricks/_jsii/__init__.py
+-rw-r--r--   0        0        0  1419975 2023-08-11 02:52:07.984040 brickflows-0.9.2/brickflow/tf/databricks/_jsii/databricks@0.0.0.jsii.tgz
+-rw-r--r--   0        0        0    24222 2023-08-11 02:52:07.984040 brickflows-0.9.2/brickflow/tf/databricks/aws_s3_mount/__init__.py
+-rw-r--r--   0        0        0    35846 2023-08-11 02:52:07.984040 brickflows-0.9.2/brickflow/tf/databricks/azure_adls_gen1_mount/__init__.py
+-rw-r--r--   0        0        0    38484 2023-08-11 02:52:07.984040 brickflows-0.9.2/brickflow/tf/databricks/azure_adls_gen2_mount/__init__.py
+-rw-r--r--   0        0        0    33033 2023-08-11 02:52:07.984040 brickflows-0.9.2/brickflow/tf/databricks/azure_blob_mount/__init__.py
+-rw-r--r--   0        0        0    35859 2023-08-11 02:52:07.988040 brickflows-0.9.2/brickflow/tf/databricks/catalog/__init__.py
+-rw-r--r--   0        0        0   356377 2023-08-11 02:52:07.988040 brickflows-0.9.2/brickflow/tf/databricks/cluster/__init__.py
+-rw-r--r--   0        0        0    22801 2023-08-11 02:52:07.988040 brickflows-0.9.2/brickflow/tf/databricks/cluster_policy/__init__.py
+-rw-r--r--   0        0        0    24053 2023-08-11 02:52:07.988040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_aws_assume_role_policy/__init__.py
+-rw-r--r--   0        0        0    25692 2023-08-11 02:52:07.988040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_aws_bucket_policy/__init__.py
+-rw-r--r--   0        0        0    18317 2023-08-11 02:52:07.992040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_aws_crossaccount_policy/__init__.py
+-rw-r--r--   0        0        0    17510 2023-08-11 02:52:07.992040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_catalogs/__init__.py
+-rw-r--r--   0        0        0   383999 2023-08-11 02:52:07.992040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_cluster/__init__.py
+-rw-r--r--   0        0        0    17678 2023-08-11 02:52:07.992040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_cluster_policy/__init__.py
+-rw-r--r--   0        0        0    18153 2023-08-11 02:52:07.992040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_clusters/__init__.py
+-rw-r--r--   0        0        0    16415 2023-08-11 02:52:07.992040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_current_user/__init__.py
+-rw-r--r--   0        0        0    20280 2023-08-11 02:52:07.992040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_dbfs_file/__init__.py
+-rw-r--r--   0        0        0    29262 2023-08-11 02:52:07.992040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_dbfs_file_paths/__init__.py
+-rw-r--r--   0        0        0    19416 2023-08-11 02:52:08.000040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_directory/__init__.py
+-rw-r--r--   0        0        0    50299 2023-08-11 02:52:08.000040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_group/__init__.py
+-rw-r--r--   0        0        0   208643 2023-08-11 02:52:08.000040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_instance_pool/__init__.py
+-rw-r--r--   0        0        0  1487868 2023-08-11 02:52:08.008040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_job/__init__.py
+-rw-r--r--   0        0        0    17582 2023-08-11 02:52:08.008040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_jobs/__init__.py
+-rw-r--r--   0        0        0    17885 2023-08-11 02:52:08.008040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_mws_credentials/__init__.py
+-rw-r--r--   0        0        0    17844 2023-08-11 02:52:08.008040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_mws_workspaces/__init__.py
+-rw-r--r--   0        0        0    50750 2023-08-11 02:52:08.008040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_node_type/__init__.py
+-rw-r--r--   0        0        0    26006 2023-08-11 02:52:08.008040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_notebook/__init__.py
+-rw-r--r--   0        0        0    29431 2023-08-11 02:52:08.008040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_notebook_paths/__init__.py
+-rw-r--r--   0        0        0    19580 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_schemas/__init__.py
+-rw-r--r--   0        0        0    32010 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_service_principal/__init__.py
+-rw-r--r--   0        0        0    20943 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_service_principals/__init__.py
+-rw-r--r--   0        0        0    89539 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_share/__init__.py
+-rw-r--r--   0        0        0    17560 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_shares/__init__.py
+-rw-r--r--   0        0        0    42275 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_spark_version/__init__.py
+-rw-r--r--   0        0        0    95058 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_sql_warehouse/__init__.py
+-rw-r--r--   0        0        0    20451 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_sql_warehouses/__init__.py
+-rw-r--r--   0        0        0    21596 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_tables/__init__.py
+-rw-r--r--   0        0        0    20644 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_user/__init__.py
+-rw-r--r--   0        0        0    21555 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_views/__init__.py
+-rw-r--r--   0        0        0    15594 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/data_databricks_zones/__init__.py
+-rw-r--r--   0        0        0    23774 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/dbfs_file/__init__.py
+-rw-r--r--   0        0        0    22201 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/directory/__init__.py
+-rw-r--r--   0        0        0    35163 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/entitlements/__init__.py
+-rw-r--r--   0        0        0    30935 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/external_location/__init__.py
+-rw-r--r--   0        0        0    25028 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/git_credential/__init__.py
+-rw-r--r--   0        0        0    34318 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/global_init_script/__init__.py
+-rw-r--r--   0        0        0    53757 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/grants/__init__.py
+-rw-r--r--   0        0        0    36782 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/group/__init__.py
+-rw-r--r--   0        0        0    19757 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/group_instance_profile/__init__.py
+-rw-r--r--   0        0        0    19102 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/group_member/__init__.py
+-rw-r--r--   0        0        0    18873 2023-08-11 02:52:08.012040 brickflows-0.9.2/brickflow/tf/databricks/group_role/__init__.py
+-rw-r--r--   0        0        0   167050 2023-08-11 02:52:08.016040 brickflows-0.9.2/brickflow/tf/databricks/instance_pool/__init__.py
+-rw-r--r--   0        0        0    26435 2023-08-11 02:52:08.016040 brickflows-0.9.2/brickflow/tf/databricks/instance_profile/__init__.py
+-rw-r--r--   0        0        0    24075 2023-08-11 02:52:08.016040 brickflows-0.9.2/brickflow/tf/databricks/ip_access_list/__init__.py
+-rw-r--r--   0        0        0  1379143 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/job/__init__.py
+-rw-r--r--   0        0        0    52597 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/library/__init__.py
+-rw-r--r--   0        0        0    51913 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/metastore/__init__.py
+-rw-r--r--   0        0        0    22270 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/metastore_assignment/__init__.py
+-rw-r--r--   0        0        0    77162 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/metastore_data_access/__init__.py
+-rw-r--r--   0        0        0    37293 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/mlflow_experiment/__init__.py
+-rw-r--r--   0        0        0    45677 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/mlflow_model/__init__.py
+-rw-r--r--   0        0        0    51243 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/mlflow_webhook/__init__.py
+-rw-r--r--   0        0        0    79706 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/model_serving/__init__.py
+-rw-r--r--   0        0        0   117494 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/mount/__init__.py
+-rw-r--r--   0        0        0    22015 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/mws_credentials/__init__.py
+-rw-r--r--   0        0        0    45478 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/mws_customer_managed_keys/__init__.py
+-rw-r--r--   0        0        0    40817 2023-08-11 02:52:08.024041 brickflows-0.9.2/brickflow/tf/databricks/mws_log_delivery/__init__.py
+-rw-r--r--   0        0        0    82561 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/mws_networks/__init__.py
+-rw-r--r--   0        0        0    22040 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/mws_permission_assignment/__init__.py
+-rw-r--r--   0        0        0    36697 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/mws_private_access_settings/__init__.py
+-rw-r--r--   0        0        0    22716 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/mws_storage_configurations/__init__.py
+-rw-r--r--   0        0        0    54494 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/mws_vpc_endpoint/__init__.py
+-rw-r--r--   0        0        0   144041 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/mws_workspaces/__init__.py
+-rw-r--r--   0        0        0    32345 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/notebook/__init__.py
+-rw-r--r--   0        0        0    22022 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/obo_token/__init__.py
+-rw-r--r--   0        0        0    19781 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/permission_assignment/__init__.py
+-rw-r--r--   0        0        0    81600 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/permissions/__init__.py
+-rw-r--r--   0        0        0   303704 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/pipeline/__init__.py
+-rw-r--r--   0        0        0    70803 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/provider/__init__.py
+-rw-r--r--   0        0        0    23878 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/provider_resource/__init__.py
+-rw-r--r--   0        0        0        1 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/py.typed
+-rw-r--r--   0        0        0    62588 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/recipient/__init__.py
+-rw-r--r--   0        0        0    35117 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/repo/__init__.py
+-rw-r--r--   0        0        0    33244 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/schema/__init__.py
+-rw-r--r--   0        0        0    21077 2023-08-11 02:52:08.028041 brickflows-0.9.2/brickflow/tf/databricks/secret/__init__.py
+-rw-r--r--   0        0        0    20955 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/secret_acl/__init__.py
+-rw-r--r--   0        0        0    32103 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/secret_scope/__init__.py
+-rw-r--r--   0        0        0    51654 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/service_principal/__init__.py
+-rw-r--r--   0        0        0    19664 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/service_principal_role/__init__.py
+-rw-r--r--   0        0        0    22252 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/service_principal_secret/__init__.py
+-rw-r--r--   0        0        0    87031 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/share/__init__.py
+-rw-r--r--   0        0        0    40696 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/sql_alert/__init__.py
+-rw-r--r--   0        0        0    21407 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/sql_dashboard/__init__.py
+-rw-r--r--   0        0        0   101946 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/sql_endpoint/__init__.py
+-rw-r--r--   0        0        0    29766 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/sql_global_config/__init__.py
+-rw-r--r--   0        0        0    50873 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/sql_permissions/__init__.py
+-rw-r--r--   0        0        0   216752 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/sql_query/__init__.py
+-rw-r--r--   0        0        0    30068 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/sql_visualization/__init__.py
+-rw-r--r--   0        0        0    68475 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/sql_widget/__init__.py
+-rw-r--r--   0        0        0    75666 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/storage_credential/__init__.py
+-rw-r--r--   0        0        0    73232 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/table/__init__.py
+-rw-r--r--   0        0        0    26507 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/token/__init__.py
+-rw-r--r--   0        0        0    49965 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/user/__init__.py
+-rw-r--r--   0        0        0    19689 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/user_instance_profile/__init__.py
+-rw-r--r--   0        0        0    18805 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/user_role/__init__.py
+-rw-r--r--   0        0        0    17999 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/databricks/workspace_conf/__init__.py
+-rw-r--r--   0        0        0      598 2023-08-11 02:52:08.032041 brickflows-0.9.2/brickflow/tf/random/__init__.py
+-rw-r--r--   0        0        0      377 2023-08-11 02:52:08.036041 brickflows-0.9.2/brickflow/tf/random/_jsii/__init__.py
+-rw-r--r--   0        0        0  1205649 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/_jsii/random@0.0.0.jsii.tgz
+-rw-r--r--   0        0        0    20651 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/id/__init__.py
+-rw-r--r--   0        0        0    21403 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/integer/__init__.py
+-rw-r--r--   0        0        0    46047 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/password/__init__.py
+-rw-r--r--   0        0        0    22022 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/pet/__init__.py
+-rw-r--r--   0        0        0     5304 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/provider/__init__.py
+-rw-r--r--   0        0        0        1 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/py.typed
+-rw-r--r--   0        0        0    23921 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/shuffle/__init__.py
+-rw-r--r--   0        0        0    46058 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/string_resource/__init__.py
+-rw-r--r--   0        0        0    15398 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow/tf/random/uuid/__init__.py
+-rw-r--r--   0        0        0     1636 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow_plugins/airflow/__init__.py
+-rw-r--r--   0        0        0     2558 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow_plugins/airflow/brickflow_task_plugin.py
+-rw-r--r--   0        0        0     2786 2023-08-11 02:52:08.040041 brickflows-0.9.2/brickflow_plugins/airflow/context/__init__.py
+-rw-r--r--   0        0        0   176743 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/airflow/cron-utils-9.2.0.jar
+-rw-r--r--   0        0        0     3572 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/airflow/cronhelper.py
+-rw-r--r--   0        0        0     5808 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/airflow/operators/__init__.py
+-rw-r--r--   0        0        0     7338 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/airflow/operators/external_tasks.py
+-rw-r--r--   0        0        0     3644 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/airflow/operators/native_operators.py
+-rw-r--r--   0        0        0        0 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/airflow/vendor/__init__.py
+-rw-r--r--   0        0        0     3238 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/airflow/vendor/context.py
+-rw-r--r--   0        0        0    12073 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/airflow/vendor/timetable.py
+-rw-r--r--   0        0        0     7647 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/airflow/vendor/timezone.py
+-rw-r--r--   0        0        0        0 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/databricks/__init__.py
+-rw-r--r--   0        0        0     5633 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/databricks/workflow_dependency_sensor.py
+-rw-r--r--   0        0        0     5500 2023-08-11 02:52:08.044041 brickflows-0.9.2/brickflow_plugins/secrets/__init__.py
+-rw-r--r--   0        0        0     3084 2023-08-11 02:53:45.984861 brickflows-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2862 1970-01-01 00:00:00.000000 brickflows-0.9.2/PKG-INFO
```

### Comparing `brickflows-0.9.1/LICENSE` & `brickflows-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/README.md` & `brickflows-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/__init__.py` & `brickflows-0.9.2/brickflow/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/bundles/model.py` & `brickflows-0.9.2/brickflow/bundles/model.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/cli/__init__.py` & `brickflows-0.9.2/brickflow/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             rv = click.Group.get_command(self, ctx, cmd_name)
             if rv is not None:
                 return rv
             raise ctx.fail(f"No such command '{cmd_name}'.")
 
 
 @click.group(invoke_without_command=True, no_args_is_help=True, cls=CdktfCmd)
-@click.version_option(prog_name="brickflows")
+@click.version_option(package_name="brickflows")
 def cli() -> None:
     """CLI for managing Databricks Workflows"""
 
 
 cli.add_command(projects)  # type: ignore
 # TODO: init is deprecated, remove in next major release
 cli.add_command(init)  # type: ignore
```

### Comparing `brickflows-0.9.1/brickflow/cli/bundles.py` & `brickflows-0.9.2/brickflow/cli/bundles.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/cli/commands.py` & `brickflows-0.9.2/brickflow/cli/commands.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/cli/configure.py` & `brickflows-0.9.2/brickflow/cli/configure.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/cli/entrypoint.template` & `brickflows-0.9.2/brickflow/cli/entrypoint.template`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/cli/gitignore_template.txt` & `brickflows-0.9.2/brickflow/cli/gitignore_template.txt`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/cli/projects.py` & `brickflows-0.9.2/brickflow/cli/projects.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/codegen/__init__.py` & `brickflows-0.9.2/brickflow/codegen/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 class DatabricksDefaultClusterTagKeys(Enum):
     ENVIRONMENT = "environment"
     DEPLOYED_BY = "deployed_by"
     BRICKFLOW_PROJECT_NAME = "brickflow_project_name"
     BRICKFLOW_DEPLOYMENT_MODE = "brickflow_deployment_mode"
     DATABRICKS_TF_PROVIDER_VERSION = "databricks_tf_provider_version"
+    BRICKFLOW_VERSION = "brickflow_version"
 
 
 BRICKFLOW_BUILTIN_DEPLOY_TAGS = {
     "brickflow_version": get_brickflow_version()
     or "undefined",  # certain scenarios get_brickflow_version maybe None
 }
```

### Comparing `brickflows-0.9.1/brickflow/codegen/cdktf_aspects.py` & `brickflows-0.9.2/brickflow/codegen/cdktf_aspects.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/codegen/databricks_bundle.py` & `brickflows-0.9.2/brickflow/codegen/databricks_bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Task,
     TaskType,
     BrickflowDefaultEnvs,
     ctx,
     _ilog,
     get_bundles_project_env,
     BrickflowEnvVars,
+    get_brickflow_version,
 )
 from brickflow.bundles.model import (
     Jobs,
     JobsSchedule,
     JobsTasks,
     JobsPermissions,
     JobsGitSource,
@@ -88,14 +89,15 @@
 
     def _get_default_tags(self, ci: CodegenInterface) -> Dict[str, str]:
         return {
             DatabricksDefaultClusterTagKeys.ENVIRONMENT.value: ctx.env,
             DatabricksDefaultClusterTagKeys.DEPLOYED_BY.value: self._get_current_user_alphanumeric(),
             DatabricksDefaultClusterTagKeys.BRICKFLOW_PROJECT_NAME.value: ci.project.name,
             DatabricksDefaultClusterTagKeys.BRICKFLOW_DEPLOYMENT_MODE.value: "Databricks Asset Bundles",
+            DatabricksDefaultClusterTagKeys.BRICKFLOW_VERSION.value: get_brickflow_version(),
         }
 
     def _rewrite_name(self, name: str) -> str:
         if ctx.is_local() is True:
             return f"{self._get_current_user_alphanumeric()}_{name}"
         else:
             return f"{ctx.env}_{name}"
```

### Comparing `brickflows-0.9.1/brickflow/codegen/hashicorp_cdktf.py` & `brickflows-0.9.2/brickflow/codegen/hashicorp_cdktf.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/context/__init__.py` & `brickflows-0.9.2/brickflow/context/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/context/context.py` & `brickflows-0.9.2/brickflow/context/context.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/engine/__init__.py` & `brickflows-0.9.2/brickflow/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/engine/compute.py` & `brickflows-0.9.2/brickflow/engine/compute.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/engine/hooks.py` & `brickflows-0.9.2/brickflow/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/engine/project.py` & `brickflows-0.9.2/brickflow/engine/project.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/engine/task.py` & `brickflows-0.9.2/brickflow/engine/task.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/engine/utils.py` & `brickflows-0.9.2/brickflow/engine/utils.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/engine/workflow.py` & `brickflows-0.9.2/brickflow/engine/workflow.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/resolver/__init__.py` & `brickflows-0.9.2/brickflow/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/_jsii/databricks@0.0.0.jsii.tgz` & `brickflows-0.9.2/brickflow/tf/databricks/_jsii/databricks@0.0.0.jsii.tgz`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/aws_s3_mount/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/aws_s3_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/azure_adls_gen1_mount/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/azure_adls_gen1_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/azure_adls_gen2_mount/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/azure_adls_gen2_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/azure_blob_mount/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/azure_blob_mount/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/catalog/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/cluster/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/cluster_policy/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/cluster_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_aws_assume_role_policy/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_aws_assume_role_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_aws_bucket_policy/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_aws_bucket_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_aws_crossaccount_policy/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_aws_crossaccount_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_catalogs/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_catalogs/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_cluster/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_cluster_policy/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_cluster_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_clusters/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_current_user/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_current_user/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_dbfs_file/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_dbfs_file/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_dbfs_file_paths/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_dbfs_file_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_directory/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_directory/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_group/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_group/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_instance_pool/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_instance_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_job/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_job/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_jobs/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_mws_credentials/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_mws_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_mws_workspaces/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_mws_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_node_type/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_node_type/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_notebook/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_notebook_paths/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_notebook_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_schemas/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_service_principal/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_service_principals/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_service_principals/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_share/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_share/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_shares/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_shares/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_spark_version/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_spark_version/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_sql_warehouse/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_sql_warehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_sql_warehouses/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_sql_warehouses/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_tables/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_user/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_user/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_views/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_views/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/data_databricks_zones/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/data_databricks_zones/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/dbfs_file/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/dbfs_file/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/directory/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/entitlements/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/entitlements/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/external_location/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/external_location/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/git_credential/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/git_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/global_init_script/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/global_init_script/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/grants/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/group/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/group/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/group_instance_profile/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/group_instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/group_member/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/group_member/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/group_role/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/group_role/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/instance_pool/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/instance_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/instance_profile/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/ip_access_list/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/ip_access_list/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/job/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/job/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/library/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/library/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/metastore/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/metastore_assignment/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/metastore_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/metastore_data_access/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/metastore_data_access/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mlflow_experiment/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mlflow_experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mlflow_model/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mlflow_model/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mlflow_webhook/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mlflow_webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/model_serving/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mount/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mount/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mws_credentials/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mws_credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mws_customer_managed_keys/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mws_customer_managed_keys/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mws_log_delivery/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mws_log_delivery/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mws_networks/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mws_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mws_permission_assignment/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mws_permission_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mws_private_access_settings/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mws_private_access_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mws_storage_configurations/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mws_storage_configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mws_vpc_endpoint/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mws_vpc_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/mws_workspaces/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/mws_workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/notebook/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/obo_token/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/obo_token/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/permission_assignment/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/permission_assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/permissions/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/pipeline/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/provider/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/provider_resource/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/provider_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/recipient/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/recipient/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/repo/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/schema/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/secret/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/secret_acl/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/secret_acl/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/secret_scope/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/secret_scope/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/service_principal/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/service_principal/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/service_principal_role/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/service_principal_role/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/service_principal_secret/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/service_principal_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/share/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/share/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/sql_alert/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/sql_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/sql_dashboard/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/sql_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/sql_endpoint/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/sql_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/sql_global_config/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/sql_global_config/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/sql_permissions/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/sql_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/sql_query/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/sql_query/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/sql_visualization/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/sql_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/sql_widget/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/sql_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/storage_credential/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/storage_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/table/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/table/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/token/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/token/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/user/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/user/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/user_instance_profile/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/user_instance_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/user_role/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/user_role/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/databricks/workspace_conf/__init__.py` & `brickflows-0.9.2/brickflow/tf/databricks/workspace_conf/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/__init__.py` & `brickflows-0.9.2/brickflow/tf/random/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/_jsii/random@0.0.0.jsii.tgz` & `brickflows-0.9.2/brickflow/tf/random/_jsii/random@0.0.0.jsii.tgz`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/id/__init__.py` & `brickflows-0.9.2/brickflow/tf/random/id/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/integer/__init__.py` & `brickflows-0.9.2/brickflow/tf/random/integer/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/password/__init__.py` & `brickflows-0.9.2/brickflow/tf/random/password/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/pet/__init__.py` & `brickflows-0.9.2/brickflow/tf/random/pet/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/provider/__init__.py` & `brickflows-0.9.2/brickflow/tf/random/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/shuffle/__init__.py` & `brickflows-0.9.2/brickflow/tf/random/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/string_resource/__init__.py` & `brickflows-0.9.2/brickflow/tf/random/string_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow/tf/random/uuid/__init__.py` & `brickflows-0.9.2/brickflow/tf/random/uuid/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/__init__.py` & `brickflows-0.9.2/brickflow_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/brickflow_task_plugin.py` & `brickflows-0.9.2/brickflow_plugins/airflow/brickflow_task_plugin.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/context/__init__.py` & `brickflows-0.9.2/brickflow_plugins/airflow/context/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/cron-utils-9.2.0.jar` & `brickflows-0.9.2/brickflow_plugins/airflow/cron-utils-9.2.0.jar`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/cronhelper.py` & `brickflows-0.9.2/brickflow_plugins/airflow/cronhelper.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/operators/__init__.py` & `brickflows-0.9.2/brickflow_plugins/airflow/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/operators/external_tasks.py` & `brickflows-0.9.2/brickflow_plugins/airflow/operators/external_tasks.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/operators/native_operators.py` & `brickflows-0.9.2/brickflow_plugins/airflow/operators/native_operators.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/vendor/context.py` & `brickflows-0.9.2/brickflow_plugins/airflow/vendor/context.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/vendor/timetable.py` & `brickflows-0.9.2/brickflow_plugins/airflow/vendor/timetable.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/airflow/vendor/timezone.py` & `brickflows-0.9.2/brickflow_plugins/airflow/vendor/timezone.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/databricks/workflow_dependency_sensor.py` & `brickflows-0.9.2/brickflow_plugins/databricks/workflow_dependency_sensor.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/brickflow_plugins/secrets/__init__.py` & `brickflows-0.9.2/brickflow_plugins/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `brickflows-0.9.1/pyproject.toml` & `brickflows-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brickflows"
-version = "0.9.1"
+version = "0.9.2"
 description = "Deploy scalable workflows to databricks using python"
 authors = ["Ashok Singamaneni, Sriharsha Tikkireddy"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/Nike-Inc/brickflow"
 repository = "https://github.com/Nike-Inc/brickflow"
 packages = [
```

### Comparing `brickflows-0.9.1/PKG-INFO` & `brickflows-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brickflows
-Version: 0.9.1
+Version: 0.9.2
 Summary: Deploy scalable workflows to databricks using python
 Home-page: https://github.com/Nike-Inc/brickflow
 License: Apache-2.0
 Author: Ashok Singamaneni, Sriharsha Tikkireddy
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


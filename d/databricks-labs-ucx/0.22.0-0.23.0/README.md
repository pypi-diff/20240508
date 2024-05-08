# Comparing `tmp/databricks_labs_ucx-0.22.0.tar.gz` & `tmp/databricks_labs_ucx-0.23.0.tar.gz`

## Comparing `databricks_labs_ucx-0.22.0.tar` & `databricks_labs_ucx-0.23.0.tar`

### file list

```diff
@@ -1,158 +1,172 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/__about__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/__init__.py
--rw-r--r--   0        0        0    15778 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/account.py
--rw-r--r--   0        0        0    17561 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/cli.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/config.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/configure.py
--rw-r--r--   0        0        0    30383 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/install.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/runtime.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/__init__.py
--rw-r--r--   0        0        0    15955 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/aws.py
--rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/azure.py
--rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/clusters.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/crawlers.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/init_scripts.py
--rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/jobs.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/pipelines.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/secrets.py
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/workflows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/aws/__init__.py
--rw-r--r--   0        0        0    15761 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/aws/access.py
--rw-r--r--   0        0        0     7240 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/aws/credentials.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/__init__.py
--rw-r--r--   0        0        0    12115 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/access.py
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/credentials.py
--rw-r--r--   0        0        0     9045 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/locations.py
--rw-r--r--   0        0        0    23838 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/__init__.py
--rw-r--r--   0        0        0    12357 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/application.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/cli_command.py
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/workflow_task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/__init__.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/crawlers.py
--rw-r--r--   0        0        0    15609 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/dashboards.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/tasks.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/utils.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/__init__.py
--rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/catalog_schema.py
--rw-r--r--   0        0        0    27049 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/grants.py
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/locations.py
--rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/mapping.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/migration_status.py
--rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_migrate.py
--rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_move.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_size.py
--rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/tables.py
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/tables.scala
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/udfs.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/verification.py
--rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/view_migrate.py
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/workflows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/__init__.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/hms_lineage.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/logs.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/mixins.py
--rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/policy.py
--rw-r--r--   0        0        0    31795 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/workflows.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/__init__.py
--rw-r--r--   0        0        0    45618 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/fixtures.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/redash.py
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/wspath.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/azure/05_0_azure_service_principals.sql
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/00_2_is_metastore_assigned.sql
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/00_4_is_incompatible_submit_run_detected.sql
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/01_2_group_migration.sql
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/01_5_group_migration_complexity.sql
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/02_2_uc_data_modeling.sql
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/02_5_uc_data_modeling_complexity.sql
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_2_data_migration_summary.sql
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_0_compatibility.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_1_count_total_databases.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_2_count_table_failures.sql
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_3_count_total_tables.sql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_4_count_external_locations.sql
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_5_count_total_views.sql
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00___assessment_overview.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/01_0_count_jobs.sql
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/05_0_object_readiness.sql
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/05_2_assessment_summary.sql
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/05___findings_summary.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10___data_summary.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/15_0_external_locations.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/15_3_mount_points.sql
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/15___storage_summary.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/20_0_cluster_policies.sql
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/20_0_clusters.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/20___compute_summary.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_0_job_summary.md
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_3_job_details.sql
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_3_jobs.sql
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_4_submit_runs.sql
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_5_submit_runs.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/40_0_pipelines.sql
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/40_3_global_init_scripts.sql
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/40___last_summary.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/README.md
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/code_patterns.sql
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/grant_detail.sql
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/misc_patterns.sql
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/objects.sql
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/table_estimates.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/__init__.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/base.py
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/dbfs.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/dependencies.py
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/dependency_loaders.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/dependency_resolvers.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/files.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/languages.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/lsp.py
--rw-r--r--   0        0        0    14297 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/notebook.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/notebook_linter.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/notebook_migrator.py
--rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/pyspark.py
--rw-r--r--   0        0        0     9613 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/python_linter.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/queries.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/redash.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/site_packages.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/table_creation.py
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/whitelist.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.4.0_added_log_dir.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/base.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/clusters.py
--rw-r--r--   0        0        0    18659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/generic.py
--rw-r--r--   0        0        0    34574 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/groups.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/listing.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/manager.py
--rw-r--r--   0        0        0    12376 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/redash.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/scim.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/secrets.py
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/tacl.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/workflows.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/LICENSE
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/NOTICE
--rw-r--r--   0        0        0    60336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/README.md
--rw-r--r--   0        0        0    28386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/pyproject.toml
--rw-r--r--   0        0        0    62011 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/__about__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/__init__.py
+-rw-r--r--   0        0        0    19819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/cli.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/config.py
+-rw-r--r--   0        0        0    30024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/install.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/runtime.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/__init__.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/aggregate.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/metastores.py
+-rw-r--r--   0        0        0    14043 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/workspaces.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/__init__.py
+-rw-r--r--   0        0        0    16138 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/aws.py
+-rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/azure.py
+-rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/clusters.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/crawlers.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/init_scripts.py
+-rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/jobs.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/pipelines.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/secrets.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/__init__.py
+-rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/access.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/credentials.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/locations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/__init__.py
+-rw-r--r--   0        0        0    17739 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/access.py
+-rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/credentials.py
+-rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/locations.py
+-rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/account_cli.py
+-rw-r--r--   0        0        0    15204 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/application.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/workflow_task.py
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/workspace_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/__init__.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/crawlers.py
+-rw-r--r--   0        0        0    15783 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/dashboards.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/tasks.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/catalog_schema.py
+-rw-r--r--   0        0        0    29222 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/grants.py
+-rw-r--r--   0        0        0    20209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/locations.py
+-rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/mapping.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/migration_status.py
+-rw-r--r--   0        0        0    21566 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_migrate.py
+-rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_move.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_size.py
+-rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/tables.py
+-rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/tables.scala
+-rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/udfs.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/verification.py
+-rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/view_migrate.py
+-rw-r--r--   0        0        0     8835 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/__init__.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/hms_lineage.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/logs.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/mixins.py
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/policy.py
+-rw-r--r--   0        0        0    33434 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/workflows.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/__init__.py
+-rw-r--r--   0        0        0    47232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/fixtures.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/redash.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/wspath.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/azure/05_0_azure_service_principals.sql
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/00_4_is_incompatible_submit_run_detected.sql
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/01_2_group_migration.sql
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/01_5_group_migration_complexity.sql
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/02_2_uc_data_modeling.sql
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/02_5_uc_data_modeling_complexity.sql
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_2_data_migration_summary.sql
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_0_compatibility.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_1_count_total_databases.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_2_count_table_failures.sql
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_3_count_total_tables.sql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_4_count_external_locations.sql
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_5_count_total_views.sql
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00_6_count_total_udfs.sql
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/00___assessment_overview.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/01_0_count_jobs.sql
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/05_0_object_readiness.sql
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/05_2_assessment_summary.sql
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/05___findings_summary.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_all_udfs.sql
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10___data_summary.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/15_0_external_locations.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/15_3_mount_points.sql
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/15___storage_summary.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/20_0_cluster_policies.sql
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/20_0_clusters.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/20___compute_summary.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_0_job_summary.md
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_3_job_details.sql
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_3_jobs.sql
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_4_submit_runs.sql
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/30_5_submit_runs.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40_0_pipelines.sql
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40_3_global_init_scripts.sql
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40___last_summary.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/README.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/migration/main/00_0_migration_overview.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/migration/main/01_0_data_object_migration_status.md
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/migration/main/01_1_data_object_migration_status.sql
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/code_patterns.sql
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/grant_detail.sql
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/misc_patterns.sql
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/objects.sql
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/table_estimates.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/__init__.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/ast_helpers.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/base.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/dbfs.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/files.py
+-rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/graph.py
+-rw-r--r--   0        0        0    10736 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/jobs.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/languages.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/lsp.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/path_lookup.py
+-rw-r--r--   0        0        0    16508 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/pyspark.py
+-rw-r--r--   0        0        0    11559 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/python_linter.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/queries.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/redash.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/site_packages.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/spark_connect.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/table_creation.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/whitelist.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/__init__.py
+-rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/cells.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/loaders.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/migrator.py
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/sources.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.23.0_add_assessment_to_udf.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.4.0_added_log_dir.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/__init__.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/base.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/clusters.py
+-rw-r--r--   0        0        0    18962 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/generic.py
+-rw-r--r--   0        0        0    34574 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/groups.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/listing.py
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/manager.py
+-rw-r--r--   0        0        0    12579 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/redash.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/scim.py
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/secrets.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/tacl.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/workflows.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/LICENSE
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/NOTICE
+-rw-r--r--   0        0        0    65891 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/README.md
+-rw-r--r--   0        0        0    28523 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/pyproject.toml
+-rw-r--r--   0        0        0    67566 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.23.0/PKG-INFO
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/account.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/account/workspaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 import logging
 from typing import ClassVar
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.tui import Prompts
-from databricks.sdk import AccountClient, WorkspaceClient
-from databricks.sdk.errors import NotFound, ResourceConflict, PermissionDenied
+from databricks.sdk import WorkspaceClient, Workspace, AccountClient
+from databricks.sdk.errors import NotFound, PermissionDenied, ResourceConflict
 from databricks.sdk.service.iam import ComplexValue, Group, Patch, PatchOp, PatchSchema
-from databricks.sdk.service.provisioning import Workspace
-from databricks.sdk.service.settings import DefaultNamespaceSetting, StringMessage
 
 logger = logging.getLogger(__name__)
 
 
 class AccountWorkspaces:
-    _tlds: ClassVar[dict[str, str]] = {
-        "aws": "cloud.databricks.com",
-        "azure": "azuredatabricks.net",
-        "gcp": "gcp.databricks.com",
-    }
-
     SYNC_FILE_NAME: ClassVar[str] = "workspaces.json"
 
-    def __init__(self, account_client: AccountClient, new_workspace_client=WorkspaceClient):
-        # TODO: new_workspace_client is a design flaw, remove it
-        self._new_workspace_client = new_workspace_client
+    def __init__(self, account_client: AccountClient, include_workspace_ids: list[int] | None = None):
         self._ac = account_client
+        self._include_workspace_ids = include_workspace_ids if include_workspace_ids else []
 
     def _workspaces(self):
-        return self._ac.workspaces.list()
-
-    def _get_cloud(self) -> str:
-        if self._ac.config.is_azure:
-            return "azure"
-        if self._ac.config.is_gcp:
-            return "gcp"
-        return "aws"
+        for workspace in self._ac.workspaces.list():
+            if self._include_workspace_ids and workspace.workspace_id not in self._include_workspace_ids:
+                logger.debug(f"Skipping {workspace.workspace_name} ({workspace.workspace_id}): not in include list")
+                continue
+            yield workspace
 
     def client_for(self, workspace: Workspace) -> WorkspaceClient:
-        return self._ac.get_workspace_client(workspace)
+        try:
+            # get_workspace_client will raise an exception since it calls config.init_auth()
+            return self._ac.get_workspace_client(workspace)
+        except (PermissionDenied, NotFound, ValueError) as err:
+            # on azure, we can retry with azure-cli auth
+            if self._ac.config.is_azure and self._ac.config.auth_type != "azure-cli":
+                current_auth_type = self._ac.config.auth_type
+                self._ac.config.auth_type = "azure-cli"
+                try:
+                    ws = self._ac.get_workspace_client(workspace)
+                except (PermissionDenied, NotFound, ValueError) as exc:
+                    raise PermissionDenied(f"Failed to create client for {workspace.deployment_name}: {exc}") from exc
+                finally:
+                    self._ac.config.auth_type = current_auth_type
+                return ws
+            raise PermissionDenied(f"Failed to create client for {workspace.deployment_name}: {err}") from err
 
-    def workspace_clients(self, workspaces: list[Workspace] | None) -> list[WorkspaceClient]:
+    def workspace_clients(self, workspaces: list[Workspace] | None = None) -> list[WorkspaceClient]:
         """
         Return a list of WorkspaceClient for each configured workspace in the account
         :return: list[WorkspaceClient]
         """
         if workspaces is None:
-            workspaces = self._workspaces()
+            workspaces = self.get_accessible_workspaces()
         clients = []
         for workspace in workspaces:
             ws = self.client_for(workspace)
             clients.append(ws)
         return clients
 
     def sync_workspace_info(self, workspaces: list[Workspace] | None = None):
@@ -79,32 +82,60 @@
 
             if not acc_group or not valid_group.members or not acc_group.id:
                 continue
             if len(valid_group.members) > 0:
                 self._add_members_to_acc_group(self._ac, acc_group.id, group_name, valid_group)
             logger.info(f"Group {group_name} created in the account")
 
+    def get_accessible_workspaces(self) -> list[Workspace]:
+        """
+        Get all workspaces that the user has access to
+        :return: list[Workspace]
+        """
+        accessible_workspaces = []
+        for workspace in self._ac.workspaces.list():
+            if self._can_administer(workspace):
+                accessible_workspaces.append(workspace)
+        return accessible_workspaces
+
+    def _can_administer(self, workspace: Workspace) -> bool:
+        try:
+            # check if user has access to workspace
+            ws = self.client_for(workspace)
+        except (PermissionDenied, NotFound, ValueError) as err:
+            logger.warning(f"{workspace.deployment_name}: Encounter error {err}. Skipping...")
+            return False
+        current_user = ws.current_user.me()
+        if current_user.groups is None:
+            return False
+        # check if user is a workspace admin
+        if "admins" not in [g.display for g in current_user.groups]:
+            logger.warning(
+                f"{workspace.deployment_name}: User {current_user.user_name} is not a workspace admin. Skipping..."
+            )
+            return False
+        return True
+
     def _try_create_account_groups(
         self, group_name: str, acc_groups: dict[str | None, list[ComplexValue] | None]
     ) -> Group | None:
         try:
             if group_name in acc_groups:
                 logger.info(f"Group {group_name} already exist in the account, ignoring")
                 return None
             return self._ac.groups.create(display_name=group_name)
         except ResourceConflict:
             logger.info(f"Group {group_name} already exist in the account, ignoring")
             return None
 
     def _get_valid_workspaces_ids(self, workspace_ids: list[int] | None = None) -> list[int]:
-        if not workspace_ids:
-            logger.info("No workspace ids provided, using current workspace instead")
-            return [self._new_workspace_client().get_workspace_id()]
-
         all_workspace_ids = [workspace.workspace_id for workspace in self._workspaces()]
+        if not workspace_ids:
+            return all_workspace_ids
+        # TODO: remove this method and rely on _include_workspace_ids
 
         valid_workspace_ids = []
         for workspace_id in workspace_ids:
             if workspace_id in all_workspace_ids:
                 valid_workspace_ids.append(workspace_id)
             else:
                 logger.info(f"Workspace id {workspace_id} not found on the account")
@@ -123,15 +154,16 @@
             logger.debug(f"Adding {len(chunk)} members to acc group {group_name}")
             acc_client.groups.patch(
                 acc_group_id,
                 operations=[Patch(op=PatchOp.ADD, path="members", value=[x.as_dict() for x in chunk])],
                 schemas=[PatchSchema.URN_IETF_PARAMS_SCIM_API_MESSAGES_2_0_PATCH_OP],
             )
 
-    def _chunks(self, lst, chunk_size):
+    @staticmethod
+    def _chunks(lst, chunk_size):
         """Yield successive n-sized chunks from lst."""
         for i in range(0, len(lst), chunk_size):
             yield lst[i : i + chunk_size]
 
     def _get_valid_workspaces_groups(self, prompts: Prompts, workspace_ids: list[int]) -> dict[str, Group]:
         all_workspaces_groups: dict[str, Group] = {}
 
@@ -166,27 +198,29 @@
                 ):
                     all_workspaces_groups[f"{workspace.workspace_name}_{group_name}"] = full_workspace_group
                     continue
             logger.info(f"Found new group {group_name}")
             all_workspaces_groups[group_name] = full_workspace_group
         logger.info(f"Found a total of {len(all_workspaces_groups)} groups to migrate to the account")
 
-    def _is_group_out_of_scope(self, group: Group) -> bool:
+    @staticmethod
+    def _is_group_out_of_scope(group: Group) -> bool:
         if group.display_name in {"users", "admins", "account users"}:
             logger.debug(f"Group {group.display_name} is a system group, ignoring")
             return True
         meta = group.meta
         if not meta:
             return False
         if meta.resource_type != "WorkspaceGroup":
             logger.debug(f"Group {group.display_name} is an account group, ignoring")
             return True
         return False
 
-    def _has_same_members(self, group_1: Group, group_2: Group) -> bool:
+    @staticmethod
+    def _has_same_members(group_1: Group, group_2: Group) -> bool:
         ws_members_set_1 = set([m.display for m in group_1.members] if group_1.members else [])
         ws_members_set_2 = set([m.display for m in group_2.members] if group_2.members else [])
         return not bool((ws_members_set_1 - ws_members_set_2).union(ws_members_set_2 - ws_members_set_1))
 
     def _get_account_groups(self) -> dict[str | None, list[ComplexValue] | None]:
         logger.debug("Listing groups in account")
         acc_groups = {}
@@ -198,15 +232,16 @@
                 continue
             logger.debug(f"Found account group {full_account_group.display_name}")
             acc_groups[full_account_group.display_name] = full_account_group.members
 
         logger.info(f"{len(acc_groups)} account groups found")
         return acc_groups
 
-    def _safe_groups_get(self, interface, group_id) -> Group | None:
+    @staticmethod
+    def _safe_groups_get(interface, group_id) -> Group | None:
         try:
             if not group_id:
                 return None
             return interface.groups.get(group_id)
         except NotFound:
             logger.info(f"Group {group_id} has been deleted")
             return None
@@ -255,91 +290,7 @@
             answer = prompts.question("Next workspace id", valid_number=True, default="stop")
             if answer == "stop":
                 break
             workspace_id = int(answer)
         for installation in Installation.existing(self._ws, 'ucx'):
             installation.save(workspaces, filename=AccountWorkspaces.SYNC_FILE_NAME)
         logger.info("Synchronised workspace id mapping for installations on current workspace")
-
-
-class AccountMetastores:
-    def __init__(
-        self,
-        account_client: AccountClient,
-    ):
-        self._ac = account_client
-
-    def show_all_metastores(self, workspace_id: str | None = None):
-        location = None
-        if workspace_id:
-            logger.info(f"Workspace ID: {workspace_id}")
-            location = self._get_region(int(workspace_id))
-        logger.info("Matching metastores are:")
-        for metastore in self._get_all_metastores(location).keys():
-            logger.info(metastore)
-
-    def assign_metastore(
-        self,
-        prompts: Prompts,
-        str_workspace_id: str | None = None,
-        metastore_id: str | None = None,
-        default_catalog: str | None = None,
-    ):
-        if not str_workspace_id:
-            workspace_choices = self._get_all_workspaces()
-            workspace_id = prompts.choice_from_dict("Please select a workspace:", workspace_choices)
-        else:
-            workspace_id = int(str_workspace_id)
-        if not metastore_id:
-            # search for all matching metastores
-            metastore_choices = self._get_all_metastores(self._get_region(workspace_id))
-            if len(metastore_choices) == 0:
-                raise ValueError(f"No matching metastore found for workspace {workspace_id}")
-            # if there are multiple matches, prompt users to select one
-            if len(metastore_choices) > 1:
-                metastore_id = prompts.choice_from_dict(
-                    "Multiple metastores found, please select one:", metastore_choices
-                )
-            else:
-                metastore_id = list(metastore_choices.values())[0]
-        if metastore_id is not None:
-            self._ac.metastore_assignments.create(workspace_id, metastore_id)
-        # set the default catalog using the default_namespace setting API
-        if default_catalog is not None:
-            self._set_default_catalog(workspace_id, default_catalog)
-
-    def _get_region(self, workspace_id: int) -> str:
-        workspace = self._ac.workspaces.get(workspace_id)
-        if self._ac.config.is_aws:
-            return str(workspace.aws_region)
-        return str(workspace.location)
-
-    def _get_all_workspaces(self) -> dict[str, int]:
-        output = dict[str, int]()
-        for workspace in self._ac.workspaces.list():
-            if workspace.workspace_id:
-                output[f"{workspace.workspace_name} - {workspace.workspace_id}"] = workspace.workspace_id
-        return dict(sorted(output.items()))
-
-    def _get_all_metastores(self, location: str | None = None) -> dict[str, str]:
-        output = dict[str, str]()
-        for metastore in self._ac.metastores.list():
-            if location is None or metastore.region == location:
-                output[f"{metastore.name} - {metastore.metastore_id}"] = str(metastore.metastore_id)
-        return dict(sorted(output.items()))
-
-    def _set_default_catalog(self, workspace_id: int, default_catalog: str):
-        if default_catalog == "":
-            return
-        workspace = self._ac.workspaces.get(int(workspace_id))
-        default_namespace = self._ac.get_workspace_client(workspace).settings.default_namespace
-        # needs to get the etag first, before patching the setting
-        try:
-            etag = default_namespace.get().etag
-        except NotFound as err:
-            # if not found, the etag is returned in the header
-            etag = err.details[0].metadata.get("etag")
-        default_namespace.update(
-            allow_missing=True,
-            field_mask="namespace.value",
-            setting=DefaultNamespaceSetting(etag=etag, namespace=StringMessage(default_catalog)),
-        )
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/cli.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from databricks.labs.blueprint.cli import App
 from databricks.labs.blueprint.entrypoint import get_logger
 from databricks.labs.blueprint.installation import Installation, SerdeError
 from databricks.labs.blueprint.tui import Prompts
 from databricks.sdk import AccountClient, WorkspaceClient
 from databricks.sdk.errors import NotFound
 
-from databricks.labs.ucx.account import AccountWorkspaces
 from databricks.labs.ucx.config import WorkspaceConfig
-from databricks.labs.ucx.contexts.cli_command import AccountContext, WorkspaceContext
+from databricks.labs.ucx.contexts.account_cli import AccountContext
+from databricks.labs.ucx.contexts.workspace_cli import WorkspaceContext
 from databricks.labs.ucx.hive_metastore.tables import What
 
 ucx = App(__file__)
 logger = get_logger(__file__)
 
 CANT_FIND_UCX_MSG = (
     "Couldn't find UCX configuration in the user's home folder. "
@@ -87,36 +87,42 @@
     """upload workspace config to all workspaces in the account where ucx is installed"""
     logger.info(f"Account ID: {a.config.account_id}")
     ctx = AccountContext(a)
     ctx.account_workspaces.sync_workspace_info()
 
 
 @ucx.command(is_account=True)
+def report_account_compatibility(a: AccountClient, ctx: AccountContext | None = None, **named_parameters):
+    """upload workspace config to all workspaces in the account where ucx is installed"""
+    if not ctx:
+        ctx = AccountContext(a, named_parameters)
+    ctx.account_aggregate.readiness_report()
+
+
+@ucx.command(is_account=True)
 def create_account_groups(
-    a: AccountClient, prompts: Prompts, workspace_ids: str | None = None, new_workspace_client=WorkspaceClient
+    a: AccountClient,
+    prompts: Prompts,
+    ctx: AccountContext | None = None,
+    **named_parameters,
 ):
     """
     Crawl all workspaces configured in workspace_ids, then creates account level groups if a WS local group is not present
     in the account.
     If workspace_ids is not specified, it will create account groups for all workspaces configured in the account.
 
     The following scenarios are supported, if a group X:
-    - Exist in workspaces A,B,C and it has same members in there, it will be created in the account
+    - Exist in workspaces A,B,C, and it has same members in there, it will be created in the account
     - Exist in workspaces A,B but not in C, it will be created in the account
     - Exist in workspaces A,B,C. It has same members in A,B, but not in C. Then, X and C_X will be created in the
     account
     """
-
-    logger.info(f"Account ID: {a.config.account_id}")
-    if workspace_ids is not None:
-        workspace_id_list = [int(x.strip()) for x in workspace_ids.split(",")]
-    else:
-        workspace_id_list = None
-    workspaces = AccountWorkspaces(a, new_workspace_client)
-    workspaces.create_account_level_groups(prompts, workspace_id_list)
+    if not ctx:
+        ctx = AccountContext(a, named_parameters)
+    ctx.account_workspaces.create_account_level_groups(prompts, ctx.workspace_ids)
 
 
 @ucx.command
 def manual_workspace_info(w: WorkspaceClient, prompts: Prompts):
     """only supposed to be run if cannot get admins to run `databricks labs ucx sync-workspace-info`"""
     ctx = WorkspaceContext(w)
     ctx.workspace_info.manual_workspace_info(prompts)
@@ -279,22 +285,43 @@
         logger.info(f"Instance profile and bucket info saved {instance_role_path}")
         logger.info("Generating UC roles and bucket permission info")
         return ctx.aws_resource_permissions.save_uc_compatible_roles()
     raise ValueError("Unsupported cloud provider")
 
 
 @ucx.command
+def create_missing_principals(
+    w: WorkspaceClient,
+    prompts: Prompts,
+    ctx: WorkspaceContext | None = None,
+    single_role: bool = True,
+    **named_parameters,
+):
+    """Not supported for Azure.
+    For AWS, this command identifies all the S3 locations that are missing a UC compatible role and creates them.
+    By default, it will create a single role for all S3. Set the optional single_role parameter to False, to create one role per S3 location.
+    """
+    if not ctx:
+        ctx = WorkspaceContext(w, named_parameters)
+    if ctx.is_aws:
+        return ctx.iam_role_creation.run(prompts, single_role=single_role)
+    raise ValueError("Unsupported cloud provider")
+
+
+@ucx.command
 def migrate_credentials(w: WorkspaceClient, prompts: Prompts, ctx: WorkspaceContext | None = None, **named_parameters):
-    """For Azure, this command migrates Azure Service Principals, which have Storage Blob Data Contributor,
-    Storage Blob Data Reader, Storage Blob Data Owner roles on ADLS Gen2 locations that are being used in
-    Databricks, to UC storage credentials.
-    The Azure Service Principals to location mapping are listed in
-    {install_folder}/.ucx/azure_storage_account_info.csv which is generated by principal_prefix_access command.
-    Please review the file and delete the Service Principals you do not want to be migrated.
-    The command will only migrate the Service Principals that have client secret stored in Databricks Secret.
+    """For Azure, this command prompts to i) create UC storage credentials for the access connectors with a
+    managed identity created for each storage account present in the ADLS Gen2 locations, the access connectors are
+    granted Storage Blob Data Contributor permissions on their corresponding storage account, to prepare for adopting to
+    use Databricks' best practice for using access connectors to authenticate with external storage, and ii) to migrate
+    Azure Service Principals, which have Storage Blob Data Contributor, Storage Blob Data Reader, Storage Blob Data
+    Owner roles on ADLS Gen2 locations that are being used in Databricks, to UC storage credentials. The Azure Service
+    Principals to location mapping are listed in {install_folder}/.ucx/azure_storage_account_info.csv which is generated
+    by principal_prefix_access command. Please review the file and delete the Service Principals you do not want to be
+    migrated. The command will only migrate the Service Principals that have client secret stored in Databricks Secret.
     For AWS, this command migrates AWS Instance Profiles that are being used in Databricks, to UC storage credentials.
     The AWS Instance Profiles to location mapping are listed in
     {install_folder}/.ucx/aws_instance_profile_info.csv which is generated by principal_prefix_access command.
     Please review the file and delete the Instance Profiles you do not want to be migrated.
     Pass aws_profile for aws.
     """
     if not ctx:
@@ -311,18 +338,16 @@
     """This command creates UC external locations. The candidate locations to be created are extracted from
     guess_external_locations task in the assessment job. You can run validate_external_locations command to check
     the candidate locations. Please make sure the credentials haven migrated before running this command. The command
     will only create the locations that have corresponded UC Storage Credentials.
     """
     if not ctx:
         ctx = WorkspaceContext(w, named_parameters)
-    if ctx.is_azure:
-        return ctx.azure_external_locations_migration.run()
-    if ctx.is_aws:
-        return ctx.aws_resource_permissions.create_external_locations()
+    if ctx.is_azure or ctx.is_aws:
+        return ctx.external_locations_migration.run()
     raise ValueError("Unsupported cloud provider")
 
 
 @ucx.command
 def create_catalogs_schemas(w: WorkspaceClient, prompts: Prompts):
     """Create UC catalogs and schemas based on the destinations created from create_table_mapping command."""
     ctx = WorkspaceContext(w)
@@ -399,15 +424,15 @@
     ctx.account_metastores.assign_metastore(ctx.prompts, workspace_id, metastore_id, default_catalog)
 
 
 @ucx.command
 def migrate_tables(w: WorkspaceClient, prompts: Prompts, *, ctx: WorkspaceContext | None = None):
     """
     Trigger the migrate-tables workflow and, optionally, the migrate-external-hiveserde-tables-in-place-experimental
-    workflow.
+    workflow and migrate-external-tables-ctas.
     """
     if ctx is None:
         ctx = WorkspaceContext(w)
     deployed_workflows = ctx.deployed_workflows
     deployed_workflows.run_workflow("migrate-tables")
 
     tables = ctx.tables_crawler.snapshot()
@@ -416,10 +441,33 @@
         percentage_hiveserde_tables = len(hiveserde_tables) / len(tables) * 100
         if prompts.confirm(
             f"Found {len(hiveserde_tables)} ({percentage_hiveserde_tables:.2f}%) hiveserde tables, do you want to run "
             f"the migrate-external-hiveserde-tables-in-place-experimental workflow?"
         ):
             deployed_workflows.run_workflow("migrate-external-hiveserde-tables-in-place-experimental")
 
+    external_ctas_tables = [table for table in tables if table.what == What.EXTERNAL_NO_SYNC]
+    if len(external_ctas_tables) > 0:
+        percentage_external_ctas_tables = len(external_ctas_tables) / len(tables) * 100
+        if prompts.confirm(
+            f"Found {len(external_ctas_tables)} ({percentage_external_ctas_tables:.2f}%) external tables which cannot be migrated using sync"
+            f", do you want to run the migrate-external-tables-ctas workflow?"
+        ):
+            deployed_workflows.run_workflow("migrate-external-tables-ctas")
+
+
+@ucx.command
+def migrate_dbsql_dashboards(w: WorkspaceClient, dashboard_id: str | None = None):
+    """Migrate table references in DBSQL Dashboard queries"""
+    ctx = WorkspaceContext(w)
+    ctx.redash.migrate_dashboards(dashboard_id)
+
+
+@ucx.command
+def revert_dbsql_dashboards(w: WorkspaceClient, dashboard_id: str | None = None):
+    """Revert migrated DBSQL Dashboard queries back to their original state"""
+    ctx = WorkspaceContext(w)
+    ctx.redash.revert_dashboards(dashboard_id)
+
 
 if __name__ == "__main__":
     ucx()
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/config.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
     override_clusters: dict[str, str] | None = None
     policy_id: str | None = None
     num_days_submit_runs_history: int = 30
     uber_spn_id: str | None = None
     uber_instance_profile: str | None = None
 
-    # Flag to see if terraform has been used for deploying certain entities
-    is_terraform_used: bool = False
+    is_terraform_used: bool = False  # Not used, keep for backwards compatability
 
     # Whether the assessment should capture a specific list of databases, if not specified, it will list all databases.
     include_databases: list[str] | None = None
 
     # Whether the tables in mounts crawler should crawl a specific list of mounts.
     # If not specified, it will list all mounts.
     include_mounts: list[str] | None = None
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/install.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/install.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import webbrowser
 from datetime import timedelta
 from functools import cached_property
 from typing import Any
 
 import databricks.sdk.errors
-from databricks.labs.blueprint.entrypoint import get_logger
+from databricks.labs.blueprint.entrypoint import get_logger, is_in_debug
 from databricks.labs.blueprint.installation import Installation, SerdeError
 from databricks.labs.blueprint.installer import InstallState
 from databricks.labs.blueprint.parallel import ManyError, Threads
 from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.blueprint.upgrades import Upgrades
 from databricks.labs.blueprint.wheels import (
     ProductInfo,
@@ -42,29 +42,31 @@
 from databricks.labs.ucx.__about__ import __version__
 from databricks.labs.ucx.assessment.azure import AzureServicePrincipalInfo
 from databricks.labs.ucx.assessment.clusters import ClusterInfo, PolicyInfo
 from databricks.labs.ucx.assessment.init_scripts import GlobalInitScriptInfo
 from databricks.labs.ucx.assessment.jobs import JobInfo, SubmitRunInfo
 from databricks.labs.ucx.assessment.pipelines import PipelineInfo
 from databricks.labs.ucx.config import WorkspaceConfig
-from databricks.labs.ucx.contexts.cli_command import AccountContext, WorkspaceContext
+from databricks.labs.ucx.contexts.account_cli import AccountContext
+from databricks.labs.ucx.contexts.workspace_cli import WorkspaceContext
 from databricks.labs.ucx.framework.dashboards import DashboardFromFiles
 from databricks.labs.ucx.framework.tasks import Task
 from databricks.labs.ucx.hive_metastore.grants import Grant
 from databricks.labs.ucx.hive_metastore.locations import ExternalLocation, Mount
 from databricks.labs.ucx.hive_metastore.migration_status import MigrationStatus
 from databricks.labs.ucx.hive_metastore.table_size import TableSize
 from databricks.labs.ucx.hive_metastore.tables import Table, TableError
 from databricks.labs.ucx.hive_metastore.udfs import Udf
 from databricks.labs.ucx.installer.hms_lineage import HiveMetastoreLineageEnabler
 from databricks.labs.ucx.installer.logs import LogRecord
 from databricks.labs.ucx.installer.mixins import InstallationMixin
 from databricks.labs.ucx.installer.policy import ClusterPolicyInstaller
 from databricks.labs.ucx.installer.workflows import WorkflowsDeployment
 from databricks.labs.ucx.runtime import Workflows
+from databricks.labs.ucx.source_code.jobs import JobProblem
 from databricks.labs.ucx.workspace_access.base import Permissions
 from databricks.labs.ucx.workspace_access.generic import WorkspaceObjectInfo
 from databricks.labs.ucx.workspace_access.groups import ConfigureGroups, MigratedGroup
 
 TAG_STEP = "step"
 WAREHOUSE_PREFIX = "Unity Catalog Migration"
 NUM_USER_ATTEMPTS = 10  # number of attempts user gets at answering a question
@@ -96,14 +98,15 @@
             functools.partial(table, "table_size", TableSize),
             functools.partial(table, "table_failures", TableError),
             functools.partial(table, "workspace_objects", WorkspaceObjectInfo),
             functools.partial(table, "permissions", Permissions),
             functools.partial(table, "submit_runs", SubmitRunInfo),
             functools.partial(table, "policies", PolicyInfo),
             functools.partial(table, "migration_status", MigrationStatus),
+            functools.partial(table, "workflow_problems", JobProblem),
             functools.partial(table, "udfs", Udf),
             functools.partial(table, "logs", LogRecord),
         ],
     )
     deployer.deploy_view("objects", "queries/views/objects.sql")
     deployer.deploy_view("grant_detail", "queries/views/grant_detail.sql")
     deployer.deploy_view("table_estimates", "queries/views/table_estimates.sql")
@@ -193,36 +196,38 @@
         return config
 
     def _is_testing(self):
         return self.product_info.product_name() != "ucx"
 
     def _prompt_for_new_installation(self) -> WorkspaceConfig:
         logger.info("Please answer a couple of questions to configure Unity Catalog migration")
+        default_database = "ucx"
+        # if a workspace is configured to use external hive metastore, the majority of the time that metastore will be
+        # shared with other workspaces. we need to add the suffix to ensure uniqueness of the inventory database
+        if self.policy_installer.has_ext_hms():
+            default_database = f"ucx_{self.workspace_client.get_workspace_id()}"
         inventory_database = self.prompts.question(
-            "Inventory Database stored in hive_metastore", default="ucx", valid_regex=r"^\w+$"
+            "Inventory Database stored in hive_metastore", default=default_database, valid_regex=r"^\w+$"
         )
         log_level = self.prompts.question("Log level", default="INFO").upper()
         num_threads = int(self.prompts.question("Number of threads", default="8", valid_number=True))
         configure_groups = ConfigureGroups(self.prompts)
         configure_groups.run()
-        # Check if terraform is being used
-        is_terraform_used = self.prompts.confirm("Do you use Terraform to deploy your infrastructure?")
         include_databases = self._select_databases()
         trigger_job = self.prompts.confirm("Do you want to trigger assessment job after installation?")
         return WorkspaceConfig(
             inventory_database=inventory_database,
             workspace_group_regex=configure_groups.workspace_group_regex,
             workspace_group_replace=configure_groups.workspace_group_replace,
             account_group_regex=configure_groups.account_group_regex,
             group_match_by_external_id=configure_groups.group_match_by_external_id,  # type: ignore[arg-type]
             include_group_names=configure_groups.include_group_names,
             renamed_group_prefix=configure_groups.renamed_group_prefix,
             log_level=log_level,
             num_threads=num_threads,
-            is_terraform_used=is_terraform_used,
             include_databases=include_databases,
             trigger_job=trigger_job,
         )
 
     def _compare_remote_local_versions(self):
         try:
             local_version = self.product_info.released_version()
@@ -263,14 +268,16 @@
             self._compare_remote_local_versions()
             if self._confirm_force_install():
                 return self._configure_new_installation(default_config)
             self._apply_upgrades()
             return config
         except NotFound as err:
             logger.debug(f"Cannot find previous installation: {err}")
+        except (PermissionDenied, SerdeError, ValueError, AttributeError):
+            logger.warning(f"Existing installation at {self.installation.install_folder()} is corrupted. Skipping...")
         return self._configure_new_installation(default_config)
 
     def replace_config(self, **changes: Any) -> WorkspaceConfig | None:
         """
         Persist the list of workspaces where UCX is successfully installed in the config
         """
         try:
@@ -382,15 +389,16 @@
         for installation in Installation.existing(self.workspace_client, self.product_info.product_name()):
             try:
                 config = installation.load(WorkspaceConfig)
                 if config.inventory_database == inventory_database:
                     raise AlreadyExists(
                         f"Inventory database '{inventory_database}' already exists in another installation"
                     )
-            except (PermissionDenied, NotFound, SerdeError):
+            except (PermissionDenied, NotFound, SerdeError, ValueError, AttributeError):
+                logger.warning(f"Existing installation at {installation.install_folder()} is corrupted. Skipping...")
                 continue
 
 
 class WorkspaceInstallation(InstallationMixin):
     def __init__(  # pylint: disable=too-many-arguments
         self,
         config: WorkspaceConfig,
@@ -460,15 +468,15 @@
 
     def run(self):
         logger.info(f"Installing UCX v{self._product_info.version()}")
         install_tasks = [self._create_database]
         if not self._skip_dashboards:
             install_tasks.append(self._create_dashboards)
         Threads.strict("installing components", install_tasks)
-        readme_url = self._workflows_installer.create_jobs(self._prompts)
+        readme_url = self._workflows_installer.create_jobs()
         if not self._is_account_install and self._prompts.confirm(f"Open job overview in your browser? {readme_url}"):
             webbrowser.open(readme_url)
         logger.info(f"Installation completed successfully! Please refer to the {readme_url} for the next steps.")
 
         if self.config.trigger_job:
             logger.info("Triggering the assessment workflow")
             self._trigger_workflow("assessment")
@@ -598,52 +606,24 @@
         if self.account_client.config.is_account_client:
             return self.account_client
         w = WorkspaceClient(product="ucx", product_version=__version__)
         host = w.config.environment.deployment_url("accounts")
         account_id = self.prompts.question("Please provide the Databricks account id")
         return AccountClient(host=host, account_id=account_id, product="ucx", product_version=__version__)
 
-    def _can_administer(self, workspace: Workspace):
-        try:
-            # check if user is a workspace admin
-            ws = self.account_client.get_workspace_client(workspace)
-            current_user = ws.current_user.me()
-            if current_user.groups is None:
-                return False
-            if "admins" not in [g.display for g in current_user.groups]:
-                logger.warning(
-                    f"{workspace.deployment_name}: User {current_user.user_name} is not a workspace admin. Skipping..."
-                )
-                return False
-            # check if user has access to workspace
-        except (PermissionDenied, NotFound, ValueError) as err:
-            logger.warning(f"{workspace.deployment_name}: Encounter error {err}. Skipping...")
-            return False
-        return True
-
-    def _get_accessible_workspaces(self):
-        """
-        Get all workspaces that the user has access to
-        """
-        accessible_workspaces = []
-        for workspace in self.account_client.workspaces.list():
-            if self._can_administer(workspace):
-                accessible_workspaces.append(workspace)
-        return accessible_workspaces
-
     def _get_installer(self, workspace: Workspace) -> WorkspaceInstaller:
         workspace_client = self.account_client.get_workspace_client(workspace)
         logger.info(f"Installing UCX on workspace {workspace.deployment_name}")
         return WorkspaceInstaller(workspace_client).replace(product_info=self.product_info, prompts=self.prompts)
 
     def install_on_account(self):
         ctx = AccountContext(self._get_safe_account_client())
         default_config = None
         confirmed = False
-        accessible_workspaces = self._get_accessible_workspaces()
+        accessible_workspaces = self.account_workspaces.get_accessible_workspaces()
         msg = "\n".join([w.deployment_name for w in accessible_workspaces])
         installed_workspaces = []
         if not self.prompts.confirm(
             f"UCX has detected the following workspaces available to install. \n{msg}\nDo you want to continue?"
         ):
             return
 
@@ -671,15 +651,16 @@
 
         # upload the json dump of workspace info in the .ucx folder
         ctx.account_workspaces.sync_workspace_info(installed_workspaces)
 
 
 if __name__ == "__main__":
     logger = get_logger(__file__)
-
+    if is_in_debug():
+        logging.getLogger('databricks').setLevel(logging.DEBUG)
     env = dict(os.environ.items())
     force_install = env.get("UCX_FORCE_INSTALL")
     if force_install == "account":
         account_installer = AccountInstaller(AccountClient(product="ucx", product_version=__version__))
         account_installer.install_on_account()
     else:
         workspace_installer = WorkspaceInstaller(WorkspaceClient(product="ucx", product_version=__version__))
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/runtime.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/runtime.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from databricks.labs.ucx.installer.logs import TaskLogger
 from databricks.labs.ucx.hive_metastore.workflows import (
     MigrateTablesInMounts,
     TableMigration,
     MigrateHiveSerdeTablesInPlace,
     MigrateExternalTablesCTAS,
 )
+from databricks.labs.ucx.source_code.workflows import ExperimentalWorkflowLinter
 from databricks.labs.ucx.workspace_access.workflows import (
     GroupMigration,
     PermissionsMigrationAPI,
     RemoveWorkspaceLocalGroups,
     ValidateGroupPermissions,
 )
 
@@ -46,14 +47,15 @@
                 TableMigration(),
                 MigrateHiveSerdeTablesInPlace(),
                 MigrateExternalTablesCTAS(),
                 ValidateGroupPermissions(),
                 RemoveWorkspaceLocalGroups(),
                 MigrateTablesInMounts(),
                 PermissionsMigrationAPI(),
+                ExperimentalWorkflowLinter(),
                 Failing(),
             ]
         )
 
     def tasks(self) -> list[Task]:
         return self._tasks
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/aws.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,23 @@
 class AWSPolicyAction:
     resource_type: str
     privilege: str
     resource_path: str
 
 
 @dataclass
+class AWSUCRoleCandidate:
+    """Candidates for UC IAM roles with the paths they have access to"""
+
+    role_name: str
+    policy_name: str
+    resource_paths: list[str]
+
+
+@dataclass
 class AWSRoleAction:
     role_arn: str
     resource_type: str
     privilege: str
     resource_path: str
 
     @property
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/azure.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/azure.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/clusters.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/clusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import logging
 from collections.abc import Iterable
 from dataclasses import dataclass
 
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
-from databricks.sdk.errors import NotFound
+from databricks.sdk.errors import NotFound, BadRequest
 from databricks.sdk.service.compute import (
     ClusterDetails,
     ClusterSource,
     DataSecurityMode,
     DbfsStorageInfo,
     InitScriptInfo,
     LocalFileInfo,
@@ -84,29 +84,29 @@
                     if len(split) != INIT_SCRIPT_LOCAL_PATH:
                         return None
                     with open(split[1], "r", encoding="utf-8") as file:
                         data = file.read()
                     return data
 
             return None
-        except NotFound:
+        except (NotFound, BadRequest):
             return None
 
     def _check_cluster_init_script(self, init_scripts: list[InitScriptInfo], source: str) -> list[str]:
         failures: list[str] = []
         for init_script_info in init_scripts:
             init_script_data = self._get_init_script_data(init_script_info)
             failures.extend(self.check_init_script(init_script_data, source))
         return failures
 
     def _check_spark_conf(self, conf: dict[str, str], source: str) -> list[str]:
         failures: list[str] = []
-        for k in INCOMPATIBLE_SPARK_CONFIG_KEYS:
-            if k in conf:
-                failures.append(f"unsupported config: {k}")
+        for key, error in INCOMPATIBLE_SPARK_CONFIG_KEYS.items():
+            if key in conf:
+                failures.append(f"{error}: {key} in {source}.")
         for value in conf.values():
             if "dbfs:/mnt" in value or "/dbfs/mnt" in value:
                 failures.append(f"using DBFS mount in configuration: {value}")
         # Checking if Azure cluster config is present in spark config
         if azure_sp_conf_present_check(conf):
             failures.append(f"{AZURE_SP_CONF_FAILURE_MSG} {source}.")
         return failures
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/crawlers.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/crawlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import re
 
 logger = logging.getLogger(__name__)
 
-INCOMPATIBLE_SPARK_CONFIG_KEYS = [
-    "spark.databricks.passthrough.enabled",
-    "spark.hadoop.javax.jdo.option.ConnectionURL",
-    "spark.databricks.hive.metastore.glueCatalog.enabled",
-]
+INCOMPATIBLE_SPARK_CONFIG_KEYS = {
+    "spark.databricks.passthrough.enabled": "Uses passthrough config",
+    "spark.hadoop.javax.jdo.option.ConnectionURL": "Uses external Hive metastore config",
+    "spark.databricks.hive.metastore.glueCatalog.enabled": "Uses Glue catalog config",
+}
 
 AZURE_SP_CONF = [
     "fs.azure.account.auth.type",
     "fs.azure.account.oauth.provider.type",
     "fs.azure.account.oauth2.client.id",
     "fs.azure.account.oauth2.client.secret",
     "fs.azure.account.oauth2.client.endpoint",
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/init_scripts.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/init_scripts.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/jobs.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/jobs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/pipelines.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/pipelines.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/secrets.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/secrets.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/workflows.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/assessment/workflows.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/aws/access.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/aws/access.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,107 +4,109 @@
 from collections.abc import Iterable
 from functools import partial
 from pathlib import PurePath
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.parallel import Threads
 from databricks.labs.blueprint.tui import Prompts
-from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound, ResourceDoesNotExist
 from databricks.sdk.service.compute import Policy
 
 from databricks.labs.ucx.assessment.aws import (
     AWSInstanceProfile,
     AWSResources,
     AWSRoleAction,
     logger,
+    AWSUCRoleCandidate,
 )
 from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.hive_metastore import ExternalLocations
-from databricks.labs.ucx.hive_metastore.locations import ExternalLocation
 
 
 class AWSResourcePermissions:
-    UC_ROLES_FILE_NAMES: typing.ClassVar[str] = "uc_roles_access.csv"
-    INSTANCE_PROFILES_FILE_NAMES: typing.ClassVar[str] = "aws_instance_profile_info.csv"
+    UC_ROLES_FILE_NAME: typing.ClassVar[str] = "uc_roles_access.csv"
+    INSTANCE_PROFILES_FILE_NAME: typing.ClassVar[str] = "aws_instance_profile_info.csv"
 
     def __init__(
         self,
         installation: Installation,
         ws: WorkspaceClient,
-        backend: SqlBackend,
         aws_resources: AWSResources,
         external_locations: ExternalLocations,
-        schema: str,
         aws_account_id=None,
         kms_key=None,
     ):
         self._installation = installation
         self._aws_resources = aws_resources
-        self._backend = backend
         self._ws = ws
         self._locations = external_locations
-        self._schema = schema
         self._aws_account_id = aws_account_id
         self._kms_key = kms_key
-        self._filename = self.INSTANCE_PROFILES_FILE_NAMES
 
-    def create_uc_roles_cli(self, *, single_role=True, role_name="UC_ROLE", policy_name="UC_POLICY"):
-        # Get the missing paths
-        # Identify the S3 prefixes
-        # Create the roles and policies for the missing S3 prefixes
-        # If single_role is True, create a single role and policy for all the missing S3 prefixes
-        # If single_role is False, create a role and policy for each missing S3 prefix
+    def list_uc_roles(self, *, single_role=True, role_name="UC_ROLE", policy_name="UC_POLICY"):
+        """
+        Get the missing paths
+        Identify the S3 prefixes
+        Create the roles and policies for the missing S3 prefixes
+        If single_role is True, create a single role and policy for all the missing S3 prefixes
+        If single_role is False, create a role and policy for each missing S3 prefix
+        """
+        roles: list[AWSUCRoleCandidate] = []
         missing_paths = self._identify_missing_paths()
         s3_prefixes = set()
         for missing_path in missing_paths:
             match = re.match(AWSResources.S3_PATH_REGEX, missing_path)
             if match:
                 s3_prefixes.add(missing_path)
         if single_role:
-            if self._aws_resources.create_uc_role(role_name):
-                self._aws_resources.put_role_policy(
-                    role_name, policy_name, s3_prefixes, self._aws_account_id, self._kms_key
-                )
+            roles.append(AWSUCRoleCandidate(role_name, policy_name, list(s3_prefixes)))
         else:
             for idx, s3_prefix in enumerate(sorted(list(s3_prefixes))):
-                if self._aws_resources.create_uc_role(f"{role_name}-{idx+1}"):
-                    self._aws_resources.put_role_policy(
-                        f"{role_name}-{idx+1}",
-                        f"{policy_name}-{idx+1}",
-                        {s3_prefix},
-                        self._aws_account_id,
-                        self._kms_key,
-                    )
+                roles.append(AWSUCRoleCandidate(f"{role_name}_{idx+1}", policy_name, [s3_prefix]))
+        return roles
+
+    def create_uc_roles(self, roles: list[AWSUCRoleCandidate]):
+        roles_created = []
+        for role in roles:
+            if self._aws_resources.create_uc_role(role.role_name):
+                self._aws_resources.put_role_policy(
+                    role.role_name,
+                    role.policy_name,
+                    set(role.resource_paths),
+                    self._aws_account_id,
+                    self._kms_key,
+                )
+                roles_created.append(role)
+        return roles_created
 
     def update_uc_role_trust_policy(self, role_name, external_id="0000"):
         return self._aws_resources.update_uc_trust_role(role_name, external_id)
 
     def save_uc_compatible_roles(self):
         uc_role_access = list(self._get_role_access())
         if len(uc_role_access) == 0:
             logger.warning("No mapping was generated.")
             return None
-        return self._installation.save(uc_role_access, filename=self.UC_ROLES_FILE_NAMES)
+        return self._installation.save(uc_role_access, filename=self.UC_ROLES_FILE_NAME)
 
     def load_uc_compatible_roles(self):
         try:
-            role_actions = self._installation.load(list[AWSRoleAction], filename=self.UC_ROLES_FILE_NAMES)
+            role_actions = self._installation.load(list[AWSRoleAction], filename=self.UC_ROLES_FILE_NAME)
         except ResourceDoesNotExist:
             self.save_uc_compatible_roles()
-            role_actions = self._installation.load(list[AWSRoleAction], filename=self.UC_ROLES_FILE_NAMES)
+            role_actions = self._installation.load(list[AWSRoleAction], filename=self.UC_ROLES_FILE_NAME)
         return role_actions
 
     def save_instance_profile_permissions(self) -> str | None:
         instance_profile_access = list(self._get_instance_profiles_access())
         if len(instance_profile_access) == 0:
             logger.warning("No mapping was generated.")
             return None
-        return self._installation.save(instance_profile_access, filename=self.INSTANCE_PROFILES_FILE_NAMES)
+        return self._installation.save(instance_profile_access, filename=self.INSTANCE_PROFILES_FILE_NAME)
 
     def role_exists(self, role_name: str) -> bool:
         return self._aws_resources.role_exists(role_name)
 
     def _get_instance_profiles(self) -> Iterable[AWSInstanceProfile]:
         instance_profiles = self._ws.instance_profiles.list()
         result_instance_profiles = []
@@ -177,51 +179,14 @@
                     matching_role = True
                     continue
             if matching_role:
                 continue
             missing_paths.add(external_location.location)
         return missing_paths
 
-    @staticmethod
-    def _identify_missing_external_locations(
-        external_locations: Iterable[ExternalLocation],
-        existing_paths: list[str],
-        compatible_roles: list[AWSRoleAction],
-    ) -> set[tuple[str, str]]:
-        # Get recommended external locations
-        # Get existing external locations
-        # Get list of paths from get_uc_compatible_roles
-        # Identify recommended external location paths that don't have an external location and return them
-        missing_paths = set()
-        for external_location in external_locations:
-            existing = False
-            for path in existing_paths:
-                if path in external_location.location:
-                    existing = True
-                    continue
-            if existing:
-                continue
-            new_path = PurePath(external_location.location)
-            matching_role = None
-            for role in compatible_roles:
-                if new_path.match(role.resource_path + "/*"):
-                    matching_role = role.role_arn
-                    continue
-            if matching_role:
-                missing_paths.add((external_location.location, matching_role))
-
-        return missing_paths
-
-    def _get_existing_credentials_dict(self):
-        credentials = self._ws.storage_credentials.list()
-        credentials_dict = {}
-        for credential in credentials:
-            credentials_dict[credential.aws_iam_role.role_arn] = credential.name
-        return credentials_dict
-
     def _get_cluster_policy(self, policy_id: str | None) -> Policy:
         if not policy_id:
             msg = "Cluster policy not found in UCX config"
             logger.error(msg)
             raise NotFound(msg) from None
         try:
             return self._ws.cluster_policies.get(policy_id=policy_id)
@@ -246,39 +211,27 @@
         definition_dict["aws_attributes.instance_profile_arn"] = {
             "type": "fixed",
             "value": iam_instance_profile.instance_profile_arn,
         }
 
         self._ws.cluster_policies.edit(str(policy.policy_id), str(policy.name), definition=json.dumps(definition_dict))
 
-    def create_external_locations(self, location_init="UCX_location"):
-        # For each path find out the role that has access to it
-        # Find out the credential that is pointing to this path
-        # Create external location for the path using the credential identified
-        credential_dict = self._get_existing_credentials_dict()
-        external_locations = self._locations.snapshot()
-        existing_external_locations = self._ws.external_locations.list()
-        existing_paths = [external_location.url for external_location in existing_external_locations]
-        compatible_roles = self.load_uc_compatible_roles()
-        missing_paths = self._identify_missing_external_locations(external_locations, existing_paths, compatible_roles)
-        external_location_names = [external_location.name for external_location in existing_external_locations]
-        external_location_num = 1
-        for path, role_arn in missing_paths:
-            if role_arn not in credential_dict:
-                logger.error(f"Missing credential for role {role_arn} for path {path}")
-                continue
-            while True:
-                external_location_name = f"{location_init}_{external_location_num}"
-                if external_location_name not in external_location_names:
-                    break
-                external_location_num += 1
-            self._ws.external_locations.create(
-                external_location_name, path, credential_dict[role_arn], skip_validation=True
-            )
-            external_location_num += 1
+    def _update_sql_dac_with_instance_profile(self, iam_instance_profile: AWSInstanceProfile, prompts: Prompts):
+        warehouse_config = self._ws.warehouses.get_workspace_warehouse_config()
+        if warehouse_config.instance_profile_arn is not None:
+            if not prompts.confirm(
+                f"There is an existing instance profile {warehouse_config.instance_profile_arn} specified in the "
+                f"workspace warehouse config. Do you want UCX to to update it with the uber instance profile?"
+            ):
+                return
+        self._ws.warehouses.set_workspace_warehouse_config(
+            data_access_config=warehouse_config.data_access_config,
+            sql_configuration_parameters=warehouse_config.sql_configuration_parameters,
+            instance_profile_arn=iam_instance_profile.instance_profile_arn,
+        )
 
     def get_instance_profile(self, instance_profile_name: str) -> AWSInstanceProfile | None:
         instance_profile_arn = self._aws_resources.get_instance_profile(instance_profile_name)
 
         if not instance_profile_arn:
             return None
 
@@ -340,10 +293,11 @@
         iam_instance_profile = self.get_instance_profile(iam_role_name)
         if not iam_instance_profile:
             return
         try:
             config.uber_instance_profile = iam_instance_profile.instance_profile_arn
             self._installation.save(config)
             self._update_cluster_policy_with_instance_profile(cluster_policy, iam_instance_profile)
+            self._update_sql_dac_with_instance_profile(iam_instance_profile, prompts)
             logger.info(f"Cluster policy \"{cluster_policy.name}\" updated successfully")
         except PermissionError:
             self._aws_resources.delete_instance_profile(iam_role_name, iam_role_name)
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/access.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/access.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import json
 import logging
+import re
 import uuid
+from collections.abc import ValuesView
 from dataclasses import dataclass
 from functools import partial
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.parallel import ManyError, Threads
 from databricks.labs.blueprint.tui import Prompts
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound, ResourceAlreadyExists
 from databricks.sdk.service.catalog import Privilege
+from databricks.sdk.service.sql import EndpointConfPair
 
 from databricks.labs.ucx.azure.resources import (
     AccessConnector,
     AzureResources,
+    AzureRoleAssignment,
     PrincipalSecret,
     StorageAccount,
 )
 from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.hive_metastore.locations import ExternalLocations
 
-
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class StoragePermissionMapping:
     prefix: str
     client_id: str
     principal: str
     privilege: str
     type: str
+    default_network_action: str = "Unknown"  # "Deny", "Allow" or "Unknown"
     # Need this directory_id/tenant_id when create UC storage credentials using service principal
     directory_id: str | None = None
 
 
 class AzureResourcePermissions:
     FILENAME = 'azure_storage_account_info.csv'
 
@@ -50,36 +54,84 @@
         self._azurerm = azurerm
         self._ws = ws
         self._levels = {
             "Storage Blob Data Contributor": Privilege.WRITE_FILES,
             "Storage Blob Data Owner": Privilege.WRITE_FILES,
             "Storage Blob Data Reader": Privilege.READ_FILES,
         }
+        self._permission_levels = {
+            "Microsoft.Storage/storageAccounts/blobServices/containers/write": Privilege.WRITE_FILES,
+            "Microsoft.Storage/storageAccounts/blobServices/containers/blobs/write": Privilege.WRITE_FILES,
+            "Microsoft.Storage/storageAccounts/blobServices/containers/read": Privilege.READ_FILES,
+            "Microsoft.Storage/storageAccounts/blobServices/containers/blobs/read": Privilege.READ_FILES,
+        }
+
+    def _get_permission_level(self, permission_to_match: str) -> Privilege | None:
+        # String might contain '*', check for wildcard match
+        pattern = re.sub(r'\*', '.*', permission_to_match)
+        permission_compiled = re.compile(pattern)
+        for each_level, privilege_level in self._permission_levels.items():
+            # Check for storage blob permission with regex to account for star pattern
+            match = permission_compiled.match(each_level)
+            # If a match is found, return the privilege level, no need to check for lower levels
+            if match:
+                return privilege_level
+        return None
+
+    def _get_custom_role_privilege(self, role_permissions: list[str]) -> Privilege | None:
+        # If both read and write privileges are found, only write privilege will be considered
+        higher_privilege = None
+        for each_permission in role_permissions:
+            privilege = self._get_permission_level(each_permission)
+            if privilege is None:
+                continue
+            # WRITE_FILES is the higher permission, don't need to check further
+            if privilege == Privilege.WRITE_FILES:
+                return privilege
+            if privilege == Privilege.READ_FILES:
+                higher_privilege = privilege
+        return higher_privilege
+
+    def _get_role_privilege(self, role_assignment: AzureRoleAssignment) -> Privilege | None:
+        privilege = None
+        # Check for custom role permissions on the storage accounts
+        if role_assignment.role_permissions:
+            privilege = self._get_custom_role_privilege(role_assignment.role_permissions)
+        elif role_assignment.role_name in self._levels:
+            privilege = self._levels[role_assignment.role_name]
+        return privilege
 
-    def _map_storage(self, storage: StorageAccount) -> list[StoragePermissionMapping]:
+    def _map_storage(self, storage: StorageAccount) -> ValuesView[StoragePermissionMapping]:
         logger.info(f"Fetching role assignment for {storage.name}")
-        out = []
+        principal_spm_mapping: dict[str, StoragePermissionMapping] = {}
         for container in self._azurerm.containers(storage.id):
             for role_assignment in self._azurerm.role_assignments(str(container)):
+                # Skip the role assignments that already have WRITE_FILES privilege
+                spm_mapping_key = f"{container.container}_{role_assignment.principal.client_id}"
+                if (
+                    spm_mapping_key in principal_spm_mapping
+                    and principal_spm_mapping[spm_mapping_key].privilege == Privilege.WRITE_FILES.value
+                ):
+                    continue
                 # one principal may be assigned multiple roles with overlapping dataActions, hence appearing
                 # here in duplicates. hence, role name -> permission level is not enough for the perfect scenario.
-                if role_assignment.role_name not in self._levels:
+                returned_privilege = self._get_role_privilege(role_assignment)
+                if not returned_privilege:
                     continue
-                privilege = self._levels[role_assignment.role_name].value
-                out.append(
-                    StoragePermissionMapping(
-                        prefix=f"abfss://{container.container}@{container.storage_account}.dfs.core.windows.net/",
-                        client_id=role_assignment.principal.client_id,
-                        principal=role_assignment.principal.display_name,
-                        privilege=privilege,
-                        type=role_assignment.principal.type,
-                        directory_id=role_assignment.principal.directory_id,
-                    )
+                privilege = returned_privilege.value
+                principal_spm_mapping[spm_mapping_key] = StoragePermissionMapping(
+                    prefix=f"abfss://{container.container}@{container.storage_account}.dfs.core.windows.net/",
+                    client_id=role_assignment.principal.client_id,
+                    principal=role_assignment.principal.display_name,
+                    privilege=privilege,
+                    type=role_assignment.principal.type,
+                    default_network_action=storage.default_network_action,
+                    directory_id=role_assignment.principal.directory_id,
                 )
-        return out
+        return principal_spm_mapping.values()
 
     def save_spn_permissions(self) -> str | None:
         used_storage_accounts = self._get_storage_accounts()
         if len(used_storage_accounts) == 0:
             logger.warning(
                 "There are no external table present with azure storage account. "
                 "Please check if assessment job is run"
@@ -116,15 +168,15 @@
             policy_dict[f"spark_conf.fs.azure.account.oauth2.client.endpoint.{storage.name}.dfs.core.windows.net"] = (
                 self._policy_config(endpoint)
             )
             policy_dict[f"spark_conf.fs.azure.account.auth.type.{storage.name}.dfs.core.windows.net"] = (
                 self._policy_config("OAuth")
             )
             policy_dict[f"spark_conf.fs.azure.account.oauth2.client.secret.{storage.name}.dfs.core.windows.net"] = (
-                self._policy_config(f"{{secrets/{inventory_database}/uber_principal_secret}}")
+                self._policy_config("{{secrets/" + inventory_database + "/uber_principal_secret}}")
             )
         return json.dumps(policy_dict)
 
     @staticmethod
     def _policy_config(value: str):
         return {"type": "fixed", "value": value}
 
@@ -147,14 +199,56 @@
                 )
             if cluster_policy.name is not None:
                 self._ws.cluster_policies.edit(policy_id, cluster_policy.name, definition=policy_definition)
         except NotFound:
             msg = f"cluster policy {policy_id} not found, please run UCX installation to create UCX cluster policy"
             raise NotFound(msg) from None
 
+    def _update_sql_dac_with_spn(
+        self,
+        storage_account_info: list[StorageAccount],
+        uber_principal: PrincipalSecret,
+        inventory_database: str,
+    ):
+
+        warehouse_config = self._ws.warehouses.get_workspace_warehouse_config()
+        sql_dac = warehouse_config.data_access_config
+        if sql_dac is None:
+            sql_dac = []
+        tenant_id = self._azurerm.tenant_id()
+        endpoint = f"https://login.microsoftonline.com/{tenant_id}/oauth2/token"
+        for storage in storage_account_info:
+            sql_dac.extend(
+                [
+                    EndpointConfPair(
+                        f"spark_conf.fs.azure.account.oauth2.client.id.{storage.name}.dfs.core.windows.net",
+                        uber_principal.client.client_id,
+                    ),
+                    EndpointConfPair(
+                        f"spark_conf.fs.azure.account.oauth.provider.type.{storage.name}.dfs.core.windows.net",
+                        "org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider",
+                    ),
+                    EndpointConfPair(
+                        f"spark_conf.fs.azure.account.oauth2.client.endpoint.{storage.name}.dfs.core.windows.net",
+                        endpoint,
+                    ),
+                    EndpointConfPair(
+                        f"spark_conf.fs.azure.account.auth.type.{storage.name}.dfs.core.windows.net", "OAuth"
+                    ),
+                    EndpointConfPair(
+                        f"spark_conf.fs.azure.account.oauth2.client.secret.{storage.name}.dfs.core.windows.net",
+                        "{{secrets/" + inventory_database + "/uber_principal_secret}}",
+                    ),
+                ]
+            )
+        self._ws.warehouses.set_workspace_warehouse_config(
+            data_access_config=sql_dac,
+            sql_configuration_parameters=warehouse_config.sql_configuration_parameters,
+        )
+
     def create_uber_principal(self, prompts: Prompts):
         config = self._installation.load(WorkspaceConfig)
         inventory_database = config.inventory_database
         display_name = f"unity-catalog-migration-{inventory_database}-{self._ws.get_workspace_id()}"
         uber_principal_name = prompts.question(
             "Enter a name for the uber service principal to be created", default=display_name
         )
@@ -186,33 +280,46 @@
         )
         try:
             self._apply_storage_permission(
                 uber_principal.client.object_id, "STORAGE_BLOB_DATA_CONTRIBUTOR", *storage_account_info
             )
             self._installation.save(config)
             self._update_cluster_policy_with_spn(policy_id, storage_account_info, uber_principal, inventory_database)
+            self._update_sql_dac_with_spn(storage_account_info, uber_principal, inventory_database)
         except PermissionError:
             self._azurerm.delete_service_principal(uber_principal.client.object_id)
         logger.info(f"Update UCX cluster policy {policy_id} with spn connection details for storage accounts")
 
     def _create_access_connector_for_storage_account(
         self, storage_account: StorageAccount, role_name: str = "STORAGE_BLOB_DATA_READER"
-    ) -> AccessConnector:
+    ) -> tuple[AccessConnector, str]:
         access_connector = self._azurerm.create_or_update_access_connector(
             storage_account.id.subscription_id,
             storage_account.id.resource_group,
             f"ac-{storage_account.name}",
             storage_account.location,
             tags={"CreatedBy": "ucx"},
             wait_for_provisioning=True,
         )
         self._apply_storage_permission(access_connector.principal_id, role_name, storage_account)
-        return access_connector
 
-    def create_access_connectors_for_storage_accounts(self) -> list[AccessConnector]:
+        container = next(self._azurerm.containers(storage_account.id), None)
+        if container is None:
+            url = f"abfss://{storage_account.name}.dfs.core.windows.net/"
+        else:
+            url = f"abfss://{container.container}@{container.storage_account}.dfs.core.windows.net/"
+
+        return access_connector, url
+
+    def create_access_connectors_for_storage_accounts(self) -> list[tuple[AccessConnector, str]]:
+        """Create access connectors for storage accounts
+
+        Returns:
+            list[AccessConnector, str] : The access connectors with a storage url to which it has access.
+        """
         used_storage_accounts = self._get_storage_accounts()
         if len(used_storage_accounts) == 0:
             logger.warning(
                 "There are no external table present with azure storage account. "
                 "Please check if assessment job is run"
             )
             return []
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/locations.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/locations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import logging
 from urllib.parse import urlparse
 
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors.platform import InvalidParameterValue, PermissionDenied
-
 from databricks.labs.ucx.azure.access import AzureResourcePermissions
 from databricks.labs.ucx.azure.resources import AzureResources
 from databricks.labs.ucx.hive_metastore import ExternalLocations
+from databricks.labs.ucx.hive_metastore.grants import PrincipalACL
+
 
 logger = logging.getLogger(__name__)
 
 
 class ExternalLocationsMigration:
     def __init__(
         self,
         ws: WorkspaceClient,
         hms_locations: ExternalLocations,
         resource_permissions: AzureResourcePermissions,
         azurerm: AzureResources,
+        principal_acl: PrincipalACL,
     ):
         self._ws = ws
         self._hms_locations = hms_locations
         self._resource_permissions = resource_permissions
         self._azurerm = azurerm
+        self._principal_acl = principal_acl
 
     def _app_id_credential_name_mapping(self) -> tuple[dict[str, str], dict[str, str]]:
         # list all storage credentials.
         # generate the managed identity/service principal application id to credential name mapping.
         # return one mapping for all non read-only credentials and one mapping for all read-only credentials
         # TODO: considering put this logic into the StorageCredentialManager
         app_id_mapping_write = {}
@@ -72,14 +75,41 @@
         prefix_mapping_read = {}
         for permission_mapping in self._resource_permissions.load():
             if permission_mapping.client_id in app_id_mapping_write:
                 prefix_mapping_write[permission_mapping.prefix] = app_id_mapping_write[permission_mapping.client_id]
                 continue
             if permission_mapping.client_id in app_id_mapping_read:
                 prefix_mapping_read[permission_mapping.prefix] = app_id_mapping_read[permission_mapping.client_id]
+
+        all_storage_accounts = list(self._azurerm.storage_accounts())
+        for storage_credential in self._ws.storage_credentials.list():
+            # Filter storage credentials for access connectors created by UCX
+            if not (
+                storage_credential.name is not None
+                and storage_credential.name.startswith("ac-")
+                and storage_credential.comment is not None
+                and storage_credential.comment == "Created by UCX"
+            ):
+                continue
+
+            storage_account_name = storage_credential.name.removeprefix("ac-")
+            storage_accounts = [st for st in all_storage_accounts if st.name == storage_account_name]
+            if len(storage_accounts) == 0:
+                logger.warning(
+                    f"Storage account {storage_account_name} for access connector {storage_credential.name} not found, "
+                    "therefore, not able to create external locations for this storage account using the access "
+                    "connector."
+                )
+                continue
+
+            for container in self._azurerm.containers(storage_accounts[0].id):
+                storage_url = f"abfss://{container.container}@{container.storage_account}.dfs.core.windows.net/"
+                # UCX assigns created access connectors the "STORAGE_BLOB_DATA_CONTRIBUTOR" role on the storage account
+                prefix_mapping_write[storage_url] = storage_credential.name
+
         return prefix_mapping_write, prefix_mapping_read
 
     def _create_location_name(self, location_url: str) -> str:
         # generate the UC external location name
         before_at, _, after_at = location_url.partition('@')
         container_name = before_at.removeprefix("abfss://")
         res_name = after_at.replace(".dfs.core.windows.net", "").rstrip("/").replace("/", "_")
@@ -167,14 +197,15 @@
         migrated_loc_urls = []
         for location_url in missing_loc_urls:
             migrated_loc_url = self._create_external_location(location_url, prefix_mapping_write, prefix_mapping_read)
             if migrated_loc_url:
                 migrated_loc_urls.append(migrated_loc_url)
 
         leftover_loc_urls = [url for url in missing_loc_urls if url not in migrated_loc_urls]
+        self._principal_acl.apply_location_acl()
         if leftover_loc_urls:
             logger.info(
                 "External locations below are not created in UC. You may check following cases and rerun this command:"
                 "1. Please check the output of 'migrate_credentials' command for storage credentials migration failure."
                 "2. If you use service principal in extra_config when create dbfs mount or use service principal "
                 "in your code directly for storage access, UCX cannot automatically migrate them to storage credential."
                 "Please manually create those storage credentials first."
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/resources.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/azure/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,29 +106,32 @@
 
 
 @dataclass
 class StorageAccount:
     id: AzureResource
     name: str
     location: str
+    default_network_action: str  # "Unknown", "Deny" or "Allow"
 
     @classmethod
     def from_raw_resource(cls, raw: RawResource) -> "StorageAccount":
         if raw.id is None:
             raise KeyError(f"Missing id: {raw}")
 
         name = raw.get("name", "")
         if name == "":
             raise KeyError(f"Missing name: {raw}")
 
         location = raw.get("location", "")
         if location == "":
             raise KeyError(f"Missing location: {raw}")
 
-        storage_account = cls(id=raw.id, name=name, location=location)
+        default_network_action = raw.get("properties", {}).get("networkAcls", {}).get("defaultAction", "Unknown")
+
+        storage_account = cls(id=raw.id, name=name, location=location, default_network_action=default_network_action)
         return storage_account
 
 
 @dataclass
 class PrincipalSecret:
     client: Principal
     secret: str
@@ -136,14 +139,23 @@
 
 @dataclass
 class AzureRoleAssignment:
     resource: AzureResource
     scope: AzureResource
     principal: Principal
     role_name: str
+    role_type: str
+    role_permissions: list[str]
+
+
+@dataclass
+class AzureRoleDetails:
+    role_name: str | None
+    role_type: str
+    role_permissions: list[str]
 
 
 @dataclass
 class AccessConnector:
     id: AzureResource
     name: str
     location: str
@@ -266,15 +278,15 @@
 class AzureResources:
     def __init__(self, azure_mgmt: AzureAPIClient, azure_graph: AzureAPIClient, include_subscriptions=None):
         if not include_subscriptions:
             include_subscriptions = []
         self._mgmt = azure_mgmt
         self._graph = azure_graph
         self._include_subscriptions = include_subscriptions
-        self._role_definitions = {}  # type: dict[str, str]
+        self._role_definitions = {}  # type: dict[str, AzureRoleDetails]
         self._principals: dict[str, Principal | None] = {}
 
     def _get_subscriptions(self) -> Iterable[AzureSubscription]:
         for subscription in self._mgmt.get("/subscriptions", "2022-12-01").get("value", []):
             yield AzureSubscription(
                 name=subscription["displayName"],
                 subscription_id=subscription["subscriptionId"],
@@ -431,35 +443,51 @@
             return None
         role_definition_id = assignment_properties.get("roleDefinitionId")
         if not role_definition_id:
             return None
         scope = assignment_properties.get("scope")
         if not scope:
             return None
-        role_name = self._role_name(role_definition_id)
+        role_details = self._role_name(role_definition_id)
+        role_name = role_details.role_name
         if not role_name:
             return None
         principal = self._get_principal(principal_id)
         if not principal:
             return None
         if scope == "/":
             scope = resource_id
         return AzureRoleAssignment(
-            resource=AzureResource(resource_id), scope=AzureResource(scope), principal=principal, role_name=role_name
+            resource=AzureResource(resource_id),
+            scope=AzureResource(scope),
+            principal=principal,
+            role_name=role_name,
+            role_type=role_details.role_type,
+            role_permissions=role_details.role_permissions,
         )
 
-    def _role_name(self, role_definition_id) -> str | None:
+    def _role_name(self, role_definition_id) -> AzureRoleDetails:
         if role_definition_id not in self._role_definitions:
             role_definition = self._mgmt.get(role_definition_id, "2022-04-01")
             definition_properties = role_definition.get("properties", {})
-            role_name: str = definition_properties.get("roleName")
+            role_name = definition_properties.get("roleName")
             if not role_name:
-                return None
-            self._role_definitions[role_definition_id] = role_name
-        return self._role_definitions.get(role_definition_id)
+                return AzureRoleDetails(role_name=None, role_type='BuiltInRole', role_permissions=[])
+            role_type = definition_properties.get("type", "BuiltInRole")
+            role_permissions = []
+            if role_type == 'CustomRole':
+                role_permissions_list = definition_properties.get("permissions", [])
+                for each_role_permissions in role_permissions_list:
+                    role_permissions = each_role_permissions.get("actions", []) + each_role_permissions.get(
+                        "dataActions", []
+                    )
+            self._role_definitions[role_definition_id] = AzureRoleDetails(
+                role_name=role_name, role_type=role_type, role_permissions=role_permissions
+            )
+        return self._role_definitions[role_definition_id]
 
     def managed_identity_client_id(
         self, access_connector_id: str, user_assigned_identity_id: str | None = None
     ) -> str | None:
         # get te client_id/application_id of the managed identity used in the access connector
         try:
             identity = self._mgmt.get(access_connector_id, "2023-05-01").get("identity")
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/application.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/application.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 import abc
 import logging
 from datetime import timedelta
 from functools import cached_property
+from pathlib import Path
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.installer import InstallState
+from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.blueprint.wheels import ProductInfo, WheelsV2
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import AccountClient, WorkspaceClient, core
 from databricks.sdk.service import sql
 
-from databricks.labs.ucx.account import WorkspaceInfo
+from databricks.labs.ucx.account.workspaces import WorkspaceInfo
 from databricks.labs.ucx.assessment.azure import AzureServicePrincipalCrawler
 from databricks.labs.ucx.aws.credentials import CredentialManager
 from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.hive_metastore import ExternalLocations, Mounts, TablesCrawler
 from databricks.labs.ucx.hive_metastore.catalog_schema import CatalogSchema
 from databricks.labs.ucx.hive_metastore.grants import (
     AzureACL,
     GrantsCrawler,
     PrincipalACL,
     AwsACL,
 )
 from databricks.labs.ucx.hive_metastore.mapping import TableMapping
+from databricks.labs.ucx.hive_metastore.migration_status import MigrationIndex
 from databricks.labs.ucx.hive_metastore.table_migrate import (
     MigrationStatusRefresher,
     TablesMigrator,
 )
 from databricks.labs.ucx.hive_metastore.table_move import TableMove
 from databricks.labs.ucx.hive_metastore.udfs import UdfsCrawler
 from databricks.labs.ucx.hive_metastore.verification import VerifyHasMetastore
 from databricks.labs.ucx.installer.workflows import DeployedWorkflows
+from databricks.labs.ucx.source_code.jobs import WorkflowLinter
+from databricks.labs.ucx.source_code.notebooks.loaders import (
+    NotebookResolver,
+    NotebookLoader,
+)
+from databricks.labs.ucx.source_code.files import FileLoader, LocalFileResolver
+from databricks.labs.ucx.source_code.path_lookup import PathLookup
+from databricks.labs.ucx.source_code.graph import DependencyResolver
+from databricks.labs.ucx.source_code.whitelist import WhitelistResolver, Whitelist
+from databricks.labs.ucx.source_code.site_packages import SitePackageResolver, SitePackages
 from databricks.labs.ucx.source_code.languages import Languages
+from databricks.labs.ucx.source_code.redash import Redash
 from databricks.labs.ucx.workspace_access import generic, redash
 from databricks.labs.ucx.workspace_access.groups import GroupManager
 from databricks.labs.ucx.workspace_access.manager import PermissionManager
 from databricks.labs.ucx.workspace_access.scim import ScimSupport
 from databricks.labs.ucx.workspace_access.secrets import SecretScopesSupport
 from databricks.labs.ucx.workspace_access.tacl import TableAclSupport
 
@@ -161,16 +175,17 @@
 
     @cached_property
     def scim_entitlements_support(self):
         return ScimSupport(self.workspace_client, include_object_permissions=self.config.include_object_permissions)
 
     @cached_property
     def secret_scope_acl_support(self):
-        # Secret ACLs are not used much in tests, so skipping include_object_permissions
-        return SecretScopesSupport(self.workspace_client)
+        return SecretScopesSupport(
+            self.workspace_client, include_object_permissions=self.config.include_object_permissions
+        )
 
     @cached_property
     def legacy_table_acl_support(self):
         return TableAclSupport(
             self.grants_crawler,
             self.sql_backend,
             include_object_permissions=self.config.include_object_permissions,
@@ -304,14 +319,15 @@
     @cached_property
     def catalog_schema(self):
         return CatalogSchema(self.workspace_client, self.table_mapping, self.principal_acl, self.sql_backend)
 
     @cached_property
     def languages(self):
         index = self.tables_migrator.index()
+        # TODO: initialize Languages every time, because it has CurrentSessionState for the cache
         return Languages(index)
 
     @cached_property
     def verify_timeout(self):
         return timedelta(minutes=2)
 
     @cached_property
@@ -329,7 +345,75 @@
     @cached_property
     def workspace_info(self):
         return WorkspaceInfo(self.installation, self.workspace_client)
 
     @cached_property
     def verify_has_metastore(self):
         return VerifyHasMetastore(self.workspace_client)
+
+    @cached_property
+    def notebook_loader(self) -> NotebookLoader:
+        return NotebookLoader()
+
+    @cached_property
+    def notebook_resolver(self):
+        return NotebookResolver(self.notebook_loader)
+
+    @cached_property
+    def site_packages(self):
+        # TODO: actually load the site packages
+        return SitePackages([])
+
+    @cached_property
+    def path_lookup(self):
+        # TODO find a solution to enable a different cwd per job/task (maybe it's not necessary or possible?)
+        return PathLookup.from_sys_path(Path.cwd())
+
+    @cached_property
+    def file_loader(self):
+        return FileLoader()
+
+    @cached_property
+    def site_packages_resolver(self):
+        return SitePackageResolver(self.site_packages, self.file_loader, self.path_lookup)
+
+    @cached_property
+    def whitelist(self):
+        # TODO: fill in the whitelist
+        return Whitelist()
+
+    @cached_property
+    def whitelist_resolver(self):
+        return WhitelistResolver(self.whitelist)
+
+    @cached_property
+    def file_resolver(self):
+        return LocalFileResolver(self.file_loader)
+
+    @cached_property
+    def dependency_resolver(self):
+        # TODO: link back self.site_packages_resolver
+        resolvers = [self.notebook_resolver, self.file_resolver, self.whitelist_resolver]
+        return DependencyResolver(resolvers, self.path_lookup)
+
+    @cached_property
+    def workflow_linter(self):
+        return WorkflowLinter(
+            self.workspace_client,
+            self.dependency_resolver,
+            self.path_lookup,
+            MigrationIndex([]),  # TODO: bring back self.tables_migrator.index()
+        )
+
+    @cached_property
+    def redash(self):
+        return Redash(
+            self.migration_status_refresher.index(),
+            self.workspace_client,
+            self.installation,
+        )
+
+
+class CliContext(GlobalContext, abc.ABC):
+    @cached_property
+    def prompts(self) -> Prompts:
+        return Prompts()
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/cli_command.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/workspace_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-import abc
-import logging
 import os
 import shutil
 from functools import cached_property
 
-from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.lsql.backends import SqlBackend, StatementExecutionBackend
-from databricks.sdk import AccountClient, WorkspaceClient
+from databricks.sdk import WorkspaceClient
 
-from databricks.labs.ucx.account import AccountWorkspaces, AccountMetastores
 from databricks.labs.ucx.assessment.aws import run_command, AWSResources
 from databricks.labs.ucx.aws.access import AWSResourcePermissions
-from databricks.labs.ucx.aws.credentials import IamRoleMigration
+from databricks.labs.ucx.aws.credentials import IamRoleMigration, IamRoleCreation
 from databricks.labs.ucx.azure.access import AzureResourcePermissions
-from databricks.labs.ucx.azure.credentials import ServicePrincipalMigration, StorageCredentialManager
+from databricks.labs.ucx.azure.credentials import StorageCredentialManager, ServicePrincipalMigration
 from databricks.labs.ucx.azure.locations import ExternalLocationsMigration
+from databricks.labs.ucx.aws.locations import AWSExternalLocationsMigration
 from databricks.labs.ucx.azure.resources import AzureAPIClient, AzureResources
-from databricks.labs.ucx.contexts.application import GlobalContext
+from databricks.labs.ucx.contexts.application import CliContext
 from databricks.labs.ucx.source_code.files import LocalFileMigrator
 from databricks.labs.ucx.workspace_access.clusters import ClusterAccess
 
-logger = logging.getLogger(__name__)
-
-
-class CliContext(GlobalContext, abc.ABC):
-    @cached_property
-    def prompts(self) -> Prompts:
-        return Prompts()
-
 
 class WorkspaceContext(CliContext):
     def __init__(self, ws: WorkspaceClient, named_parameters: dict[str, str] | None = None):
         super().__init__(named_parameters)
         self._ws = ws
 
     @cached_property
@@ -108,21 +97,31 @@
             self.workspace_client,
             self.azure_resource_permissions,
             self.azure_service_principal_crawler,
             self.azure_credential_manager,
         )
 
     @cached_property
-    def azure_external_locations_migration(self):
-        return ExternalLocationsMigration(
-            self.workspace_client,
-            self.external_locations,
-            self.azure_resource_permissions,
-            self.azure_resources,
-        )
+    def external_locations_migration(self):
+        if self.is_aws:
+            return AWSExternalLocationsMigration(
+                self.workspace_client,
+                self.external_locations,
+                self.aws_resource_permissions,
+                self.principal_acl,
+            )
+        if self.is_azure:
+            return ExternalLocationsMigration(
+                self.workspace_client,
+                self.external_locations,
+                self.azure_resource_permissions,
+                self.azure_resources,
+                self.principal_acl,
+            )
+        raise NotImplementedError
 
     @cached_property
     def aws_cli_run_command(self):
         # this is a convenience method for unit testing
         if not shutil.which("aws"):
             raise ValueError("Couldn't find AWS CLI in path. Please install the CLI from https://aws.amazon.com/cli/")
         return run_command
@@ -146,40 +145,28 @@
         return AWSResources(self.aws_profile, self.aws_cli_run_command)
 
     @cached_property
     def aws_resource_permissions(self):
         return AWSResourcePermissions(
             self.installation,
             self.workspace_client,
-            self.sql_backend,
             self.aws_resources,
             self.external_locations,
-            self.inventory_database,
             self.named_parameters.get("aws_account_id"),
             self.named_parameters.get("kms_key"),
         )
 
     @cached_property
     def iam_role_migration(self):
         return IamRoleMigration(
             self.installation,
             self.aws_resource_permissions,
             self.iam_credential_manager,
         )
 
-
-class AccountContext(CliContext):
-    def __init__(self, ac: AccountClient, named_parameters: dict[str, str] | None = None):
-        super().__init__(named_parameters)
-        self._ac = ac
-
     @cached_property
-    def account_client(self) -> AccountClient:
-        return self._ac
-
-    @cached_property
-    def account_workspaces(self):
-        return AccountWorkspaces(self.account_client)
-
-    @cached_property
-    def account_metastores(self):
-        return AccountMetastores(self.account_client)
+    def iam_role_creation(self):
+        return IamRoleCreation(
+            self.installation,
+            self.workspace_client,
+            self.aws_resource_permissions,
+        )
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/workflow_task.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/contexts/workflow_task.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/crawlers.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/crawlers.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/dashboards.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/dashboards.py`

 * *Files 4% similar despite different names*

```diff
@@ -295,17 +295,17 @@
             return None
         query_meta = {
             "data_source_id": data_source_id,
             "name": f"{dashboard_name} - {query.name}",
             "query": query.query,
         }
         if query.key in self._state.queries:
-            return self._ws.queries.update(self._state.queries[query.key], **query_meta, run_as_role=None)
+            return self._ws.queries.update(self._state.queries[query.key], **query_meta, tags=None, run_as_role=None)
 
-        deployed_query = self._ws.queries.create(parent=parent, run_as_role=RunAsRole.VIEWER, **query_meta)
+        deployed_query = self._ws.queries.create(parent=parent, run_as_role=RunAsRole.VIEWER, **query_meta, tags=None)
         assert deployed_query.id is not None
         self._ws.dbsql_permissions.set(
             ObjectTypePlural.QUERIES,
             deployed_query.id,
             access_control_list=[AccessControl(group_name="users", permission_level=PermissionLevel.CAN_RUN)],
         )
         self._state.queries[query.key] = deployed_query.id
@@ -318,25 +318,29 @@
         *,
         items_per_page: int = 25,
         condensed=True,
         with_row_number=False,
         description: str | None = None,
         search_by: str | None = None,
     ) -> dict:
+        if search_by is not None:
+            search_by_columns = set(search_by.split(","))
+        else:
+            search_by_columns = set()
         return {
             "type": "TABLE",
             "name": name,
             "description": description,
             "options": {
                 "itemsPerPage": items_per_page,
                 "condensed": condensed,
                 "withRowNumber": with_row_number,
                 "version": 2,
                 "columns": [
-                    VizColumn(name=x, title=x, allowSearch=x == search_by).as_dict() for x in columns.split(",")
+                    VizColumn(name=x, title=x, allowSearch=x in search_by_columns).as_dict() for x in columns.split(",")
                 ],
             },
         }
 
     @staticmethod
     def _counter_viz_args(  # pylint: disable=too-many-arguments
         name: str,
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/tasks.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/tasks.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/utils.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/framework/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/catalog_schema.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/catalog_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+import collections
 import logging
+from dataclasses import replace
 from pathlib import PurePath
-import dataclasses
 
 from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.labs.ucx.hive_metastore.grants import PrincipalACL, Grant
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
+from databricks.sdk.service.catalog import SchemaInfo
 
 from databricks.labs.ucx.hive_metastore.mapping import TableMapping
 
 logger = logging.getLogger(__name__)
 
 
 class CatalogSchema:
@@ -46,40 +48,30 @@
         catalog_grants: set[Grant] = set()
         new_grants = []
         src_trg_schema_mapping = self._get_database_source_target_mapping()
         grants = self._principal_grants.get_interactive_cluster_grants()
         # filter on grants to only get database level grants
         database_grants = [grant for grant in grants if grant.table is None and grant.view is None]
         for db_grant in database_grants:
-            new_grants.append(
-                dataclasses.replace(
-                    db_grant,
-                    # replace source database with taget UC database
-                    database=src_trg_schema_mapping[db_grant.database]['target_schema'],
-                    # replace hive_metastore with target UC catalog
-                    catalog=src_trg_schema_mapping[db_grant.database]['target_catalog'],
-                )
-            )
+            for schema in src_trg_schema_mapping[db_grant.database]:
+                new_grants.append(replace(db_grant, catalog=schema.catalog_name, database=schema.name))
         for grant in new_grants:
-            catalog_grants.add(dataclasses.replace(grant, database=None))
+            catalog_grants.add(replace(grant, database=None))
         new_grants.extend(catalog_grants)
         return new_grants
 
-    def _get_database_source_target_mapping(self) -> dict[str, dict]:
-        """generate a dictionary of source database in hive_metastore and its
-        mapping of target UC catalog and schema from the table mappings."""
-        src_trg_schema_mapping: dict[str, dict] = {}
+    def _get_database_source_target_mapping(self) -> dict[str, list[SchemaInfo]]:
+        """Generate a dictionary of source database in hive_metastore and its
+        mapping of target UC catalog and schema combinations from the table mappings."""
+        src_trg_schema_mapping: dict[str, list[SchemaInfo]] = collections.defaultdict(list)
         table_mappings = self._table_mapping.load()
-        for mappings in table_mappings:
-            if mappings.src_schema not in src_trg_schema_mapping:
-                src_trg_schema_mapping[mappings.src_schema] = {
-                    'target_catalog': mappings.catalog_name,
-                    'target_schema': mappings.dst_schema,
-                }
-                continue
+        for table_mapping in table_mappings:
+            schema = SchemaInfo(catalog_name=table_mapping.catalog_name, name=table_mapping.dst_schema)
+            if schema not in src_trg_schema_mapping[table_mapping.src_schema]:
+                src_trg_schema_mapping[table_mapping.src_schema].append(schema)
         return src_trg_schema_mapping
 
     def _create_catalog_validate(self, catalog, prompts: Prompts):
         logger.info(f"Creating UC catalog: {catalog}")
         # create catalogs
         attempts = 3
         while True:
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/grants.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/grants.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 from functools import partial
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.parallel import ManyError, Threads
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import ResourceDoesNotExist, NotFound
-from databricks.sdk.service.catalog import ExternalLocationInfo, SchemaInfo, TableInfo
+from databricks.sdk.service.catalog import (
+    ExternalLocationInfo,
+    SchemaInfo,
+    TableInfo,
+    Privilege,
+    PermissionsChange,
+    SecurableType,
+)
 from databricks.sdk.service.compute import ClusterSource, DataSecurityMode
 
 from databricks.labs.ucx.assessment.aws import AWSRoleAction
 from databricks.labs.ucx.assessment.azure import (
     AzureServicePrincipalCrawler,
     AzureServicePrincipalInfo,
 )
@@ -32,17 +39,17 @@
 from databricks.labs.ucx.hive_metastore.tables import Table, TablesCrawler
 from databricks.labs.ucx.hive_metastore.udfs import UdfsCrawler
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
-class ClusterLocationMapping:
-    cluster_id: str
-    locations: dict[str, str]
+class LocationACL:
+    location_name: str
+    principal: str
 
 
 @dataclass(frozen=True)
 class Grant:
     principal: str
     action_type: str
     catalog: str | None = None
@@ -387,15 +394,16 @@
                 "No external location found, If hive metastore tables are created in external storage, "
                 "ensure migrate-locations cli cmd is run to create the required locations."
             )
             logger.error(msg)
             raise ResourceDoesNotExist(msg) from None
 
         permission_mappings = self._installation.load(
-            list[AWSRoleAction], filename=AWSResourcePermissions.INSTANCE_PROFILES_FILE_NAMES
+            list[AWSRoleAction],
+            filename=AWSResourcePermissions.INSTANCE_PROFILES_FILE_NAME,
         )
         if len(permission_mappings) == 0:
             # if permission mapping is empty, raise an error to run principal_prefix cmd
             msg = (
                 "No instance profile permission file found. Please ensure principal-prefix-access cli "
                 "cmd is run to create the instance profile permission file."
             )
@@ -405,16 +413,16 @@
         for cluster_id, role_name in cluster_instance_profiles.items():
             eligible_locations.update(self._get_external_locations(role_name, external_locations, permission_mappings))
             if len(eligible_locations) == 0:
                 continue
             cluster_locations[cluster_id] = eligible_locations
         return cluster_locations
 
+    @staticmethod
     def _get_external_locations(
-        self,
         role_name: str,
         external_locations: list[ExternalLocationInfo],
         permission_mappings: list[AWSRoleAction],
     ) -> dict[str, str]:
         matching_location = {}
         for location in external_locations:
             if location.url is None:
@@ -595,20 +603,64 @@
         grants.extend(database_grants)
 
         return grants
 
     def _get_cluster_principal_mapping(self, cluster_id: str) -> list[str]:
         # gets all the users,groups,spn which have access to the clusters and returns a dataclass of that mapping
         principal_list = []
-        cluster_permission = self._ws.permissions.get("clusters", cluster_id)
+        try:
+            cluster_permission = self._ws.permissions.get("clusters", cluster_id)
+        except ResourceDoesNotExist:
+            return []
         if cluster_permission.access_control_list is None:
             return []
         for acl in cluster_permission.access_control_list:
             if acl.user_name is not None:
                 principal_list.append(acl.user_name)
             if acl.group_name is not None:
                 if acl.group_name == "admins":
                     continue
                 principal_list.append(acl.group_name)
             if acl.service_principal_name is not None:
                 principal_list.append(acl.service_principal_name)
         return principal_list
+
+    def apply_location_acl(self):
+        """
+        Check the interactive cluster and the principals mapped to it
+        identifies the spn or instance profile configured for the interactive cluster
+        identifies any location the spn/instance profile have access to (read or write)
+        applies create_external_table, create_external_volume and read_files permission for all location
+        to the principal
+        """
+        logger.info(
+            "Applying permission for external location (CREATE EXTERNAL TABLE, "
+            "CREATE EXTERNAL VOLUME and READ_FILES for existing eligible interactive cluster users"
+        )
+        # get the eligible location mapped for each interactive cluster
+        for cluster_id, locations in self._cluster_locations.items():
+            # get interactive cluster users
+            principals = self._get_cluster_principal_mapping(cluster_id)
+            if len(principals) == 0:
+                continue
+            for location_url in locations.keys():
+                # get the location name for the given url
+                location_name = self._get_location_name(location_url)
+                if location_name is None:
+                    continue
+                self._update_location_permissions(location_name, principals)
+        logger.info("Applied all the permission on external location")
+
+    def _update_location_permissions(self, location_name: str, principals: list[str]):
+        permissions = [Privilege.CREATE_EXTERNAL_TABLE, Privilege.CREATE_EXTERNAL_VOLUME, Privilege.READ_FILES]
+        changes = [PermissionsChange(add=permissions, principal=principal) for principal in principals]
+        self._ws.grants.update(
+            SecurableType.EXTERNAL_LOCATION,
+            location_name,
+            changes=changes,
+        )
+
+    def _get_location_name(self, location_url: str):
+        for location in self._ws.external_locations.list():
+            if location.url == location_url:
+                return location.name
+        return None
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/locations.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/locations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import logging
 import os
 import re
 from collections.abc import Iterable, Sequence
 from dataclasses import dataclass
-from functools import partial
 from typing import ClassVar
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.lsql import Row
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
 from databricks.sdk.service.catalog import ExternalLocationInfo
 from databricks.sdk.dbutils import FileInfo
-from databricks.labs.ucx.framework.crawlers import CrawlerBase, Result, ResultFn
+from databricks.labs.ucx.framework.crawlers import CrawlerBase
 from databricks.labs.ucx.framework.utils import escape_sql_identifier
 from databricks.labs.ucx.hive_metastore.tables import Table
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -281,42 +280,48 @@
 
         irrelevant_patterns = {'_SUCCESS', '_committed_', '_started_'}
         if exclude_paths_in_mount:
             irrelevant_patterns.update(exclude_paths_in_mount)
         self._fiter_paths = irrelevant_patterns
 
     def snapshot(self) -> list[Table]:
-        return self._snapshot(partial(self._try_load), partial(self._crawl))
-
-    def _snapshot(self, fetcher: ResultFn, loader: ResultFn) -> list[Result]:
         logger.debug(f"[{self.full_name}] fetching {self._table} inventory")
         cached_results = []
         try:
-            cached_results = list(fetcher())
+            cached_results = list(self._try_load())
         except NotFound:
             pass
+        table_paths = self._get_tables_paths_from_assessment(cached_results)
         logger.debug(f"[{self.full_name}] crawling new batch for {self._table}")
-        loaded_records = list(loader())
+        loaded_records = list(self._crawl(table_paths))
         if len(cached_results) > 0:
             loaded_records = loaded_records + cached_results
-        self._append_records(loaded_records)
+        self._overwrite_records(loaded_records)
         return loaded_records
 
-    def _append_records(self, items: Sequence[Table]):
-        logger.debug(f"[{self.full_name}] found {len(items)} new records for {self._table}")
-        self._backend.save_table(self.full_name, items, Table, mode="overwrite")
-
     def _try_load(self) -> Iterable[Table]:
         """Tries to load table information from the database or throws TABLE_OR_VIEW_NOT_FOUND error"""
         for row in self._fetch(
             f"SELECT * FROM {escape_sql_identifier(self.full_name)} WHERE NOT STARTSWITH(database, '{self.TABLE_IN_MOUNT_DB}')"
         ):
             yield Table(*row)
 
-    def _crawl(self):
+    def _get_tables_paths_from_assessment(self, loaded_records: Iterable[Table]) -> dict[str, str]:
+        seen = {}
+        for rec in loaded_records:
+            if not rec.location:
+                continue
+            seen[rec.location] = rec.key
+        return seen
+
+    def _overwrite_records(self, items: Sequence[Table]):
+        logger.debug(f"[{self.full_name}] found {len(items)} new records for {self._table}")
+        self._backend.save_table(self.full_name, items, Table, mode="overwrite")
+
+    def _crawl(self, table_paths_from_assessment: dict[str, str]):
         all_mounts = self._mounts_crawler.snapshot()
         all_tables = []
         for mount in all_mounts:
             if self._include_mounts and mount.name not in self._include_mounts:
                 logger.info(f"Filtering mount {mount.name}")
                 continue
             table_paths = {}
@@ -324,60 +329,86 @@
                 for path in self._include_paths_in_mount:
                     table_paths.update(self._find_delta_log_folders(path))
             else:
                 table_paths = self._find_delta_log_folders(mount.name)
 
             for path, entry in table_paths.items():
                 guess_table = os.path.basename(path)
+                table_location = self._get_table_location(mount, path)
+
+                # A table in mount may have already been identified by the assessment job because they're on the current workspace HMS
+                # We filter those tables as we give better support to migrate those tables to UC
+                if table_location in table_paths_from_assessment:
+                    logger.info(
+                        f"Path {path} is identified as a table in mount, but is present in current workspace as a registered table {table_paths_from_assessment[table_location]}"
+                    )
+                    continue
+                if path in table_paths_from_assessment:
+                    logger.info(
+                        f"Path {path} is identified as a table in mount, but is present in current workspace as a registered table {table_paths_from_assessment[path]}"
+                    )
+                    continue
                 table = Table(
                     catalog="hive_metastore",
                     database=f"{self.TABLE_IN_MOUNT_DB}{mount.name.replace('/mnt/', '').replace('/', '_')}",
                     name=guess_table,
                     object_type="EXTERNAL",
                     table_format=entry.format,
-                    location=path.replace(f"dbfs:{mount.name}/", mount.source),
+                    location=table_location,
                     is_partitioned=entry.is_partitioned,
                 )
                 all_tables.append(table)
+        logger.info(f"Found a total of {len(all_tables)} tables in mount points")
         return all_tables
 
+    def _get_table_location(self, mount: Mount, path: str):
+        """
+        There can be different cases for mounts:
+            - Mount(name='/mnt/things/a', source='abfss://things@labsazurethings.dfs.core.windows.net/a')
+            - Mount(name='/mnt/mount' source='abfss://container@dsss.net/')
+            Both must return the complete source with a forward slash in the end
+        """
+        if mount.source.endswith("/"):
+            return path.replace(f"dbfs:{mount.name}/", mount.source)
+        return path.replace(f"dbfs:{mount.name}", mount.source)
+
     def _find_delta_log_folders(self, root_dir: str, delta_log_folders=None) -> dict:
         if delta_log_folders is None:
             delta_log_folders = {}
         logger.info(f"Listing {root_dir}")
         file_infos = self._dbutils.fs.ls(root_dir)
         for file_info in file_infos:
             if self._is_irrelevant(file_info.name) or file_info.path == root_dir:
                 logger.debug(f"Path {file_info.path} is irrelevant")
                 continue
 
             root_path = os.path.dirname(root_dir)
             previous_entry = delta_log_folders.get(root_path)
+            table_in_mount = self._assess_path(file_info)
+
             if previous_entry:
                 # Happens when first folder was _delta_log and next folders are partitioned folder
-                if (
-                    previous_entry.format == "DELTA"
-                    and self._is_partitioned(file_info.name)
-                    and not previous_entry.is_partitioned
-                ):
+                if previous_entry.format == "DELTA" and self._is_partitioned(file_info.name):
                     delta_log_folders[root_path] = TableInMount(format=previous_entry.format, is_partitioned=True)
+                # Happens when previous entries where partitioned folders and the current one is delta_log
+                if previous_entry.is_partitioned and table_in_mount and table_in_mount.format == "DELTA":
+                    delta_log_folders[root_path] = TableInMount(format=table_in_mount.format, is_partitioned=True)
                 continue
 
             if self._is_partitioned(file_info.name):
-                table_in_mount = self._find_partition_file_format(file_info.path)
-                if table_in_mount:
-                    delta_log_folders[root_path] = table_in_mount
+                partition_format = self._find_partition_file_format(file_info.path)
+                if partition_format:
+                    delta_log_folders[root_path] = partition_format
                 continue
 
-            table_in_mount = self._assess_path(file_info)
-            if table_in_mount:
-                delta_log_folders[root_path] = table_in_mount
-            else:
+            if not table_in_mount:
                 self._find_delta_log_folders(file_info.path, delta_log_folders)
+                continue
 
+            delta_log_folders[root_path] = table_in_mount
         return delta_log_folders
 
     def _find_partition_file_format(self, root_dir: str) -> TableInMount | None:
         logger.info(f"Listing {root_dir}")
         file_infos = self._dbutils.fs.ls(root_dir)
         for file_info in file_infos:
             path_extension = self._assess_path(file_info)
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/mapping.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.parallel import Threads
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import BadRequest, NotFound, ResourceConflict
 from databricks.sdk.service.catalog import TableInfo, SchemaInfo
 
-from databricks.labs.ucx.account import WorkspaceInfo
+from databricks.labs.ucx.account.workspaces import WorkspaceInfo
 from databricks.labs.ucx.framework.utils import escape_sql_identifier
 from databricks.labs.ucx.hive_metastore import TablesCrawler
 from databricks.labs.ucx.hive_metastore.tables import Table
 
 logger = logging.getLogger(__name__)
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/migration_status.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/migration_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,16 @@
     def index(self) -> MigrationIndex:
         return MigrationIndex(list(self.snapshot()))
 
     def get_seen_tables(self) -> dict[str, str]:
         seen_tables: dict[str, str] = {}
         for schema in self._iter_schemas():
             try:
-                tables = self._ws.tables.list(catalog_name=schema.catalog_name, schema_name=schema.name)
+                # ws.tables.list returns Iterator[TableInfo], so we need to convert it to a list in order to catch the exception
+                tables = list(self._ws.tables.list(catalog_name=schema.catalog_name, schema_name=schema.name))
             except NotFound:
                 logger.warning(
                     f"Schema {schema.catalog_name}.{schema.name} no longer exists. Skipping checking its migration status."
                 )
                 continue
             for table in tables:
                 if not table.properties:
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_migrate.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,42 +25,47 @@
     HiveSerdeType,
 )
 from databricks.labs.ucx.hive_metastore.view_migrate import (
     ViewsMigrationSequencer,
     ViewToMigrate,
 )
 from databricks.labs.ucx.workspace_access.groups import GroupManager, MigratedGroup
+from databricks.sdk.errors.platform import BadRequest, NotFound
 
 logger = logging.getLogger(__name__)
 
 
 class TablesMigrator:
     def __init__(
         self,
         table_crawler: TablesCrawler,
         grant_crawler: GrantsCrawler,
         ws: WorkspaceClient,
         backend: SqlBackend,
         table_mapping: TableMapping,
         group_manager: GroupManager,
-        migration_status_refresher: 'MigrationStatusRefresher',
+        migration_status_refresher: MigrationStatusRefresher,
         principal_grants: PrincipalACL,
     ):
         self._tc = table_crawler
         self._gc = grant_crawler
         self._backend = backend
         self._ws = ws
         self._tm = table_mapping
         self._group = group_manager
         self._migration_status_refresher = migration_status_refresher
         self._seen_tables: dict[str, str] = {}
         self._principal_grants = principal_grants
 
     def index(self):
-        # TODO: remove this method
+        return self._migration_status_refresher.index()
+
+    def index_full_refresh(self):
+        # when we want the latest up-to-date status, e.g. to determine whether views dependencies have been migrated
+        self._migration_status_refresher.reset()
         return self._migration_status_refresher.index()
 
     def migrate_tables(
         self,
         what: What,
         acl_strategy: list[AclMigrationWhat] | None = None,
         mounts_crawler: Mounts | None = None,
@@ -111,17 +116,16 @@
         if not tasks:
             logger.info(f"No tables found to migrate with type {what.name}")
         # the below is useful for testing
         return tasks
 
     def _migrate_views(self, acl_strategy, all_grants_to_migrate, all_migrated_groups, all_principal_grants):
         tables_to_migrate = self._tm.get_tables_to_migrate(self._tc)
-        self._migration_status_refresher.reset()
         all_tasks = []
-        sequencer = ViewsMigrationSequencer(tables_to_migrate, self.index())
+        sequencer = ViewsMigrationSequencer(tables_to_migrate, self.index_full_refresh())
         batches = sequencer.sequence_batches()
         for batch in batches:
             tasks = []
             for view in batch:
                 grants = self._compute_grants(
                     view.src, acl_strategy, all_grants_to_migrate, all_migrated_groups, all_principal_grants
                 )
@@ -129,15 +133,14 @@
                     partial(
                         self._migrate_view,
                         view,
                         grants,
                     )
                 )
             Threads.strict("migrate views", tasks)
-            self._migration_status_refresher.reset()
             all_tasks.extend(tasks)
         return all_tasks
 
     def _compute_grants(
         self, table: Table, acl_strategy, all_grants_to_migrate, all_migrated_groups, all_principal_grants
     ):
         if acl_strategy is None:
@@ -195,15 +198,15 @@
             return self._migrate_view_table(src_view, grants)
         logger.info(f"View {src_view.src.key} is not supported for migration")
         return True
 
     def _view_can_be_migrated(self, view: ViewToMigrate):
         # dependencies have already been computed, therefore an empty dict is good enough
         for table in view.dependencies:
-            if not self.index().get(table.schema, table.name):
+            if not self.index_full_refresh().get(table.schema, table.name):
                 logger.info(f"View {view.src.key} cannot be migrated because {table.key} is not migrated yet")
                 return False
         return True
 
     def _migrate_view_table(self, src_view: ViewToMigrate, grants: list[Grant] | None = None):
         view_migrate_sql = self._sql_migrate_view(src_view)
         logger.debug(f"Migrating view {src_view.src.key} to using SQL query: {view_migrate_sql}")
@@ -213,16 +216,16 @@
         return self._migrate_acl(src_view.src, src_view.rule, grants)
 
     def _sql_migrate_view(self, src_view: ViewToMigrate) -> str:
         # We have to fetch create statement this way because of columns in:
         # CREATE VIEW x.y (col1, col2) AS SELECT * FROM w.t
         create_statement = self._backend.fetch(f"SHOW CREATE TABLE {src_view.src.safe_sql_key}")
         src_view.src.view_text = next(iter(create_statement))["createtab_stmt"]
-        migration_index = self._migration_status_refresher.index()
-        return src_view.sql_migrate_view(migration_index)
+        # this does not require the index to be refreshed because the dependencies have already been validated
+        return src_view.sql_migrate_view(self.index())
 
     def _migrate_external_table(self, src_table: Table, rule: Rule, grants: list[Grant] | None = None):
         target_table_key = rule.as_uc_table_key
         table_migrate_sql = src_table.sql_migrate_external(target_table_key)
         logger.debug(f"Migrating external table {src_table.key} to using SQL query: {table_migrate_sql}")
         # have to wrap the fetch result with iter() for now, because StatementExecutionBackend returns iterator but RuntimeBackend returns list.
         sync_result = next(iter(self._backend.fetch(table_migrate_sql)))
@@ -306,15 +309,18 @@
             return True
         for grant in grants:
             acl_migrate_sql = grant.uc_grant_sql(src.kind, rule.as_uc_table_key)
             if acl_migrate_sql is None:
                 logger.warning(f"Cannot identify UC grant for {src.kind} {rule.as_uc_table_key}. Skipping.")
                 continue
             logger.debug(f"Migrating acls on {rule.as_uc_table_key} using SQL query: {acl_migrate_sql}")
-            self._backend.execute(acl_migrate_sql)
+            try:
+                self._backend.execute(acl_migrate_sql)
+            except (BadRequest, NotFound) as e:
+                logger.warning(f"Failed to migrate ACL for {src.key} to {rule.as_uc_table_key}: {e}")
         return True
 
     def _table_already_migrated(self, target) -> bool:
         return target in self._seen_tables
 
     def _get_tables_to_revert(self, schema: str | None = None, table: str | None = None) -> list[Table]:
         schema = schema.lower() if schema else None
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_move.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_move.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_size.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/table_size.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/tables.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/tables.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/tables.scala` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/tables.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/verification.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/verification.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/view_migrate.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/hive_metastore/view_migrate.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/hms_lineage.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/hms_lineage.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/logs.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/logs.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/mixins.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/mixins.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/policy.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,33 +19,42 @@
         self._installation = installation
         self._prompts = prompts
 
     @staticmethod
     def _policy_config(value: str):
         return {"type": "fixed", "value": value}
 
+    def has_ext_hms(self) -> bool:
+        policies_with_external_hms = list(self._get_cluster_policies_with_external_hive_metastores())
+        if len(policies_with_external_hms) > 0:
+            return True
+        warehouse_config = self._get_warehouse_config_with_external_hive_metastore()
+        if warehouse_config is not None:
+            return True
+        return False
+
     def create(self, inventory_database: str) -> tuple[str, str, dict, str | None]:
         instance_profile = ""
         spark_conf_dict = {}
         # get instance pool id to be put into the cluster policy
         instance_pool_id = self._get_instance_pool_id()
         policies_with_external_hms = list(self._get_cluster_policies_with_external_hive_metastores())
         if len(policies_with_external_hms) > 0 and self._prompts.confirm(
-            "We have identified one or more cluster policies set up for an external metastore"
+            "We have identified one or more cluster policies set up for an external metastore. "
             "Would you like to set UCX to connect to the external metastore?"
         ):
             logger.info("Setting up an external metastore")
             cluster_policies = {conf.name: conf.definition for conf in policies_with_external_hms}
             if len(cluster_policies) >= 1:
                 cluster_policy = json.loads(self._prompts.choice_from_dict("Choose a cluster policy", cluster_policies))
                 instance_profile, spark_conf_dict = self._extract_external_hive_metastore_conf(cluster_policy)
         else:
             warehouse_config = self._get_warehouse_config_with_external_hive_metastore()
             if warehouse_config and self._prompts.confirm(
-                "We have identified the workspace warehouse is set up for an external metastore"
+                "We have identified the workspace warehouse is set up for an external metastore. "
                 "Would you like to set UCX to connect to the external metastore?"
             ):
                 logger.info("Setting up an external metastore")
                 instance_profile, spark_conf_dict = self._extract_external_hive_metastore_sql_conf(warehouse_config)
         policy_name = f"Unity Catalog Migration ({inventory_database}) ({self._ws.current_user.me().user_name})"
         policies = self._ws.cluster_policies.list()
         for policy in policies:
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/workflows.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/installer/workflows.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 import os.path
 import re
 import sys
 import webbrowser
 from collections.abc import Iterator
 from dataclasses import replace
@@ -9,15 +11,14 @@
 from io import StringIO
 from pathlib import Path
 from typing import Any
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.installer import InstallState
 from databricks.labs.blueprint.parallel import ManyError
-from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.blueprint.wheels import ProductInfo, WheelsV2
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import (
     Aborted,
     AlreadyExists,
     BadRequest,
     Cancelled,
@@ -41,15 +42,14 @@
 from databricks.sdk.retries import retried
 from databricks.sdk.service import compute, jobs
 from databricks.sdk.service.jobs import RunLifeCycleState, RunResultState
 from databricks.sdk.service.workspace import ObjectType
 
 import databricks
 from databricks.labs.ucx.config import WorkspaceConfig
-from databricks.labs.ucx.configure import ConfigureClusterOverrides
 from databricks.labs.ucx.framework.tasks import Task
 from databricks.labs.ucx.installer.logs import PartialLogRecord, parse_logs
 from databricks.labs.ucx.installer.mixins import InstallationMixin
 
 logger = logging.getLogger(__name__)
 
 EXTRA_TASK_PARAMS = {
@@ -214,17 +214,19 @@
             assert workflow is not None
             _, latest_run = self._latest_job_run(workflow)
         self._relay_logs(workflow, latest_run.run_id)
 
     def _relay_logs(self, workflow, run_id):
         for record in self._fetch_logs(workflow, run_id):
             task_logger = logging.getLogger(record.component)
+            MaxedStreamHandler.install_handler(task_logger)
             task_logger.setLevel(logger.getEffectiveLevel())
             log_level = logging.getLevelName(record.level)
             task_logger.log(log_level, record.message)
+        MaxedStreamHandler.uninstall_handlers()
 
     def _fetch_logs(self, workflow: str, run_id: str) -> Iterator[PartialLogRecord]:
         log_path = f'{self._install_state.install_folder()}/logs/{workflow}'
         run_folders = []
         for run_folder in self._ws.workspace.list(log_path):
             if not run_folder.path or run_folder.object_type != ObjectType.DIRECTORY:
                 continue
@@ -395,16 +397,16 @@
         self._product_info = product_info
         self._verify_timeout = verify_timeout
         self._tasks = tasks
         self._this_file = Path(__file__)
         self._skip_dashboards = skip_dashboards
         super().__init__(config, installation, ws)
 
-    def create_jobs(self, prompts):
-        remote_wheel = self._upload_wheel(prompts)
+    def create_jobs(self):
+        remote_wheel = self._upload_wheel()
         desired_workflows = {t.workflow for t in self._tasks if t.cloud_compatible(self._ws.config)}
         wheel_runner = None
 
         if self._config.override_clusters:
             wheel_runner = self._upload_wheel_runner(remote_wheel)
         for workflow_name in desired_workflows:
             settings = self._job_settings(workflow_name, remote_wheel)
@@ -518,25 +520,16 @@
                 return self._deploy_workflow(step_name, settings)
         logger.info(f"Creating new job configuration for step={step_name}")
         new_job = self._ws.jobs.create(**settings)
         assert new_job.job_id is not None
         self._install_state.jobs[step_name] = str(new_job.job_id)
         return None
 
-    def _upload_wheel(self, prompts: Prompts):
+    def _upload_wheel(self):
         with self._wheels:
-            try:
-                self._wheels.upload_to_dbfs()
-            except PermissionDenied as err:
-                if not prompts:
-                    raise RuntimeWarning("no Prompts instance found") from err
-                logger.warning(f"Uploading wheel file to DBFS failed, DBFS is probably write protected. {err}")
-                configure_cluster_overrides = ConfigureClusterOverrides(self._ws, prompts.choice_from_dict)
-                self._config.override_clusters = configure_cluster_overrides.configure()
-                self._installation.save(self._config)
             return self._wheels.upload_to_wsfs()
 
     def _upload_wheel_runner(self, remote_wheel: str):
         # TODO: we have to be doing this workaround until ES-897453 is solved in the platform
         code = TEST_RUNNER_NOTEBOOK.format(remote_wheel=remote_wheel, config_file=self._config_file).encode("utf8")
         return self._installation.upload(f"wheels/wheel-test-runner-{self._product_info.version()}.py", code)
 
@@ -631,20 +624,15 @@
                     "config": f"/Workspace{self._config_file}",
                 }
                 | EXTRA_TASK_PARAMS,
             ),
         )
 
     def _job_wheel_task(self, jobs_task: jobs.Task, workflow: str, remote_wheel: str) -> jobs.Task:
-        if jobs_task.job_cluster_key is not None and "table_migration" in jobs_task.job_cluster_key:
-            # Shared mode cluster cannot use dbfs, need to use WSFS
-            libraries = [compute.Library(whl=f"/Workspace{remote_wheel}")]
-        else:
-            # TODO: https://github.com/databrickslabs/ucx/issues/1098
-            libraries = [compute.Library(whl=f"dbfs:{remote_wheel}")]
+        libraries = [compute.Library(whl=f"/Workspace{remote_wheel}")]
         named_parameters = {
             "config": f"/Workspace{self._config_file}",
             "workflow": workflow,
             "task": jobs_task.task_key,
         }
         return replace(
             jobs_task,
@@ -717,7 +705,76 @@
             f"[{self._name(step_name)}]({self._ws.config.host}#job/{job_id})"
             for step_name, job_id in self._install_state.jobs.items()
         )
         content = DEBUG_NOTEBOOK.format(
             remote_wheel=remote_wheel, readme_link=readme_link, job_links=job_links, config_file=self._config_file
         ).encode("utf8")
         self._installation.upload('DEBUG.py', content)
+
+
+class MaxedStreamHandler(logging.StreamHandler):
+
+    MAX_STREAM_SIZE = 2**20 - 2**6  # 1 Mb minus some buffer
+    _installed_handlers: dict[str, tuple[logging.Logger, MaxedStreamHandler]] = {}
+
+    @classmethod
+    def install_handler(cls, logger_: logging.Logger):
+        if logger_.handlers:
+            # already installed ?
+            installed = next((h for h in logger_.handlers if isinstance(h, MaxedStreamHandler)), None)
+            if installed:
+                return
+            # any handler to override ?
+            handler = next((h for h in logger_.handlers if isinstance(h, logging.StreamHandler)), None)
+            if handler:
+                to_install = MaxedStreamHandler(cls.MAX_STREAM_SIZE, handler)
+                cls._installed_handlers[logger_.name] = (logger_, to_install)
+                logger_.removeHandler(handler)
+                logger_.addHandler(to_install)
+                return
+        if logger_.parent:
+            cls.install_handler(logger_.parent)
+        if logger_.root:
+            cls.install_handler(logger_.root)
+
+    @classmethod
+    def uninstall_handlers(cls):
+        for pair in cls._installed_handlers.values():
+            logger_ = pair[0]
+            handler = pair[1]
+            logger_.removeHandler(handler)
+            logger_.addHandler(handler.original_handler)
+        cls._installed_handlers.clear()
+
+    def __init__(self, max_bytes: int, original_handler: logging.StreamHandler):
+        super().__init__()
+        self._max_bytes = max_bytes
+        self._sent_bytes = 0
+        self._original_handler = original_handler
+
+    @property
+    def original_handler(self):
+        return self._original_handler
+
+    def emit(self, record):
+        try:
+            msg = self.format(record) + self.terminator
+            if self._prevent_overflow(msg):
+                return
+            self.stream.write(msg)
+            self.flush()
+        except RecursionError:  # See issue 36272
+            raise
+        # the below is copied from Python source
+        # so ensuring not to break the logging logic
+        # pylint: disable=broad-exception-caught
+        except Exception:
+            self.handleError(record)
+
+    def _prevent_overflow(self, msg: str):
+        data = msg.encode("utf-8")
+        if self._sent_bytes + len(data) > self._max_bytes:
+            # ensure readers are aware of why the logs are incomplete
+            self.stream.write(f"MAX LOGS SIZE REACHED: {self._sent_bytes} bytes!!!")
+            self.flush()
+            return True
+        return False
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/fixtures.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,17 @@
     ServingEndpointDetailed,
 )
 from databricks.sdk.service.sql import (
     CreateWarehouseRequestWarehouseType,
     GetResponse,
     ObjectTypePlural,
     Query,
-    QueryInfo,
+    Dashboard,
+    WidgetOptions,
+    WidgetPosition,
 )
 from databricks.sdk.service.workspace import ImportFormat, Language
 
 from databricks.labs.ucx.workspace_access.groups import MigratedGroup
 
 # this file will get to databricks-labs-pytester project and be maintained/refactored there
 # pylint: disable=redefined-outer-name,too-many-try-statements,import-outside-toplevel,unnecessary-lambda,too-complex,invalid-name
@@ -554,22 +556,24 @@
     yield from factory("secret scope acl", create, lambda x: ws.secrets.delete_acl(x[0], x[1]))
 
 
 @pytest.fixture
 def make_notebook(ws, make_random):
     def create(
         *,
-        path: str | None = None,
+        path: str | Path | None = None,
         content: BinaryIO | None = None,
         language: Language = Language.PYTHON,
         format: ImportFormat = ImportFormat.SOURCE,  # pylint:  disable=redefined-builtin
         overwrite: bool = False,
     ) -> str:
         if path is None:
             path = f"/Users/{ws.current_user.me().user_name}/sdk-{make_random(4)}"
+        elif isinstance(path, pathlib.Path):
+            path = str(path)
         if content is None:
             content = io.BytesIO(b"print(1)")
         path = str(path)
         ws.workspace.upload(path, content, language=language, format=format, overwrite=overwrite)
         return path
 
     yield from factory("notebook", create, lambda x: ws.workspace.delete(x))
@@ -750,51 +754,41 @@
         return ws.instance_pools.create(instance_pool_name, node_type_id, **kwargs)
 
     yield from factory("instance pool", create, lambda item: ws.instance_pools.delete(item.instance_pool_id))
 
 
 @pytest.fixture
 def make_job(ws, make_random, make_notebook):
-    def create(**kwargs):
+    def create(notebook_path: str | Path | None = None, **kwargs):
         task_spark_conf = None
         if "name" not in kwargs:
             kwargs["name"] = f"sdk-{make_random(4)}"
         if "spark_conf" in kwargs:
             task_spark_conf = kwargs["spark_conf"]
             kwargs.pop("spark_conf")
+        if isinstance(notebook_path, pathlib.Path):
+            notebook_path = str(notebook_path)
+        if not notebook_path:
+            notebook_path = make_notebook()
+        assert notebook_path is not None
         if "tasks" not in kwargs:
-            if task_spark_conf:
-                kwargs["tasks"] = [
-                    jobs.Task(
-                        task_key=make_random(4),
-                        description=make_random(4),
-                        new_cluster=compute.ClusterSpec(
-                            num_workers=1,
-                            node_type_id=ws.clusters.select_node_type(local_disk=True, min_memory_gb=16),
-                            spark_version=ws.clusters.select_spark_version(latest=True),
-                            spark_conf=task_spark_conf,
-                        ),
-                        notebook_task=jobs.NotebookTask(notebook_path=make_notebook()),
-                        timeout_seconds=0,
-                    )
-                ]
-            else:
-                kwargs["tasks"] = [
-                    jobs.Task(
-                        task_key=make_random(4),
-                        description=make_random(4),
-                        new_cluster=compute.ClusterSpec(
-                            num_workers=1,
-                            node_type_id=ws.clusters.select_node_type(local_disk=True, min_memory_gb=16),
-                            spark_version=ws.clusters.select_spark_version(latest=True),
-                        ),
-                        notebook_task=jobs.NotebookTask(notebook_path=make_notebook()),
-                        timeout_seconds=0,
-                    )
-                ]
+            kwargs["tasks"] = [
+                jobs.Task(
+                    task_key=make_random(4),
+                    description=make_random(4),
+                    new_cluster=compute.ClusterSpec(
+                        num_workers=1,
+                        node_type_id=ws.clusters.select_node_type(local_disk=True, min_memory_gb=16),
+                        spark_version=ws.clusters.select_spark_version(latest=True),
+                        spark_conf=task_spark_conf,
+                    ),
+                    notebook_task=jobs.NotebookTask(notebook_path=str(notebook_path)),
+                    timeout_seconds=0,
+                )
+            ]
         job = ws.jobs.create(**kwargs)
         logger.info(f"Job: {ws.config.host}#job/{job.job_id}")
         return job
 
     yield from factory("job", create, lambda item: ws.jobs.delete(item.job_id))
 
 
@@ -1067,30 +1061,49 @@
             else:
                 raise e
 
     yield from factory("table", create, remove)
 
 
 @pytest.fixture
-def make_udf(sql_backend, make_schema, make_random) -> Generator[Callable[..., FunctionInfo], None, None]:
+def make_udf(
+    ws,
+    env_or_skip,
+    sql_backend,
+    make_schema,
+    make_random,
+) -> Generator[Callable[..., FunctionInfo], None, None]:
     def create(
-        *, catalog_name="hive_metastore", schema_name: str | None = None, name: str | None = None
+        *,
+        catalog_name="hive_metastore",
+        schema_name: str | None = None,
+        name: str | None = None,
+        hive_udf: bool = False,
     ) -> FunctionInfo:
         if schema_name is None:
             schema = make_schema(catalog_name=catalog_name)
             catalog_name = schema.catalog_name
             schema_name = schema.name
 
         if name is None:
             name = f"ucx_T{make_random(4)}".lower()
 
         full_name = f"{catalog_name}.{schema_name}.{name}".lower()
-        ddl = f"CREATE FUNCTION {full_name}(x INT) RETURNS FLOAT CONTAINS SQL DETERMINISTIC RETURN 0;"
-
-        sql_backend.execute(ddl)
+        if hive_udf:
+            cmd_exec = CommandExecutor(
+                ws.clusters,
+                ws.command_execution,
+                lambda: env_or_skip("TEST_DEFAULT_CLUSTER_ID"),
+                language=compute.Language.SQL,
+            )
+            ddl = f"CREATE FUNCTION {full_name} AS 'org.apache.hadoop.hive.ql.udf.generic.GenericUDFAbs';"
+            cmd_exec.run(ddl)
+        else:
+            ddl = f"CREATE FUNCTION {full_name}(x INT) RETURNS FLOAT CONTAINS SQL DETERMINISTIC RETURN 0;"
+            sql_backend.execute(ddl)
         udf_info = FunctionInfo(
             catalog_name=catalog_name,
             schema_name=schema_name,
             name=name,
             full_name=full_name,
         )
 
@@ -1107,21 +1120,22 @@
                 raise e
 
     yield from factory("table", create, remove)
 
 
 @pytest.fixture
 def make_query(ws, make_table, make_random):
-    def create() -> QueryInfo:
+    def create() -> Query:
         table = make_table()
         query_name = f"ucx_query_Q{make_random(4)}"
         query = ws.queries.create(
-            name=f"{query_name}",
+            name=query_name,
             description="TEST QUERY FOR UCX",
             query=f"SELECT * FROM {table.schema_name}.{table.name}",
+            tags=["original_query_tag"],
         )
         logger.info(f"Query Created {query_name}: {ws.config.host}/sql/editor/{query.id}")
         return query
 
     def remove(query: Query):
         try:
             ws.queries.delete(query_id=query.id)
@@ -1249,7 +1263,53 @@
     def remove(path: str):
         if ws.config.is_aws:
             cmd_exec.run(f"dbutils.fs.rm('{path}', recurse=True)")
         else:
             ws.dbfs.delete(path, recursive=True)
 
     yield from factory("make_storage_dir", create, remove)
+
+
+@pytest.fixture
+def make_dashboard(ws, make_random, make_query):
+    def create() -> Dashboard:
+        query = make_query()
+        viz = ws.query_visualizations.create(
+            type="table",
+            query_id=query.id,
+            options={
+                "itemsPerPage": 1,
+                "condensed": True,
+                "withRowNumber": False,
+                "version": 2,
+                "columns": [
+                    {"name": "id", "title": "id", "allowSearch": True},
+                ],
+            },
+        )
+
+        dashboard_name = f"ucx_D{make_random(4)}"
+        dashboard = ws.dashboards.create(name=dashboard_name, tags=["original_dashboard_tag"])
+        ws.dashboard_widgets.create(
+            dashboard_id=dashboard.id,
+            visualization_id=viz.id,
+            width=1,
+            options=WidgetOptions(
+                title="",
+                position=WidgetPosition(
+                    col=0,
+                    row=0,
+                    size_x=3,
+                    size_y=3,
+                ),
+            ),
+        )
+        logger.info(f"Dashboard Created {dashboard_name}: {ws.config.host}/sql/dashboards/{dashboard.id}")
+        return dashboard
+
+    def remove(dashboard: Dashboard):
+        try:
+            ws.dashboards.delete(dashboard_id=dashboard.id)
+        except RuntimeError as e:
+            logger.info(f"Can't delete dashboard {e}")
+
+    yield from factory("dashboard", create, remove)
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/redash.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/redash.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/wspath.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/mixins/wspath.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import locale
 import logging
 import os
 import pathlib
 from functools import cached_property
 
 # pylint: disable-next=import-private-name
-from pathlib import Path, _PosixFlavour, _Accessor  # type: ignore
+from pathlib import Path, _PosixFlavour  # type: ignore
 from urllib.parse import quote_from_bytes as urlquote_from_bytes
 from io import BytesIO, StringIO
 
 from databricks.sdk import WorkspaceClient
-from databricks.sdk.errors import NotFound
+from databricks.sdk.errors import NotFound, DatabricksError
 from databricks.sdk.service.workspace import ObjectInfo, ObjectType, ExportFormat, ImportFormat, Language
 
 logger = logging.getLogger(__name__)
 
 
 class _DatabricksFlavour(_PosixFlavour):
     def __init__(self, ws: WorkspaceClient):
@@ -70,15 +70,15 @@
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         pass
 
 
-class _DatabricksAccessor(_Accessor):
+class _DatabricksAccessor:
     chmod = _na('accessor.chmod')
     getcwd = _na('accessor.getcwd')
     group = _na('accessor.group')
     link = _na('accessor.link')
     mkdir = _na('accessor.mkdir')
     owner = _na('accessor.owner')
     readlink = _na('accessor.readlink')
@@ -282,16 +282,19 @@
         """Return the file extension. If the file is a notebook, return the suffix based on the language."""
         suffix = super().suffix
         if suffix:
             return suffix
         if not self.is_notebook():
             return ""
         for sfx, lang in self._SUFFIXES.items():
-            if self._object_info.language == lang:
-                return sfx
+            try:
+                if self._object_info.language == lang:
+                    return sfx
+            except DatabricksError:
+                return ""
         return ""
 
     def __lt__(self, other: pathlib.PurePath):
         if not isinstance(other, pathlib.PurePath):
             return NotImplemented
         return self.as_posix() < other.as_posix()
 
@@ -309,20 +312,29 @@
     is_char_device = _return_false
     is_fifo = _return_false
     is_socket = _return_false
     is_mount = _return_false
     is_junction = _return_false
 
     def is_dir(self):
-        return self._object_info.object_type == ObjectType.DIRECTORY
+        try:
+            return self._object_info.object_type == ObjectType.DIRECTORY
+        except DatabricksError:
+            return False
 
     def is_file(self):
-        return self._object_info.object_type == ObjectType.FILE
+        try:
+            return self._object_info.object_type == ObjectType.FILE
+        except DatabricksError:
+            return False
 
     def is_notebook(self):
-        return self._object_info.object_type == ObjectType.NOTEBOOK
+        try:
+            return self._object_info.object_type == ObjectType.NOTEBOOK
+        except DatabricksError:
+            return False
 
     def __eq__(self, other):
         return isinstance(other, Path) and self.as_posix() == other.as_posix()
 
     def __hash__(self):
         return Path.__hash__(self)
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 -- widget title=Metastore assignment, row=0, col=0, size_x=2, size_y=8
 
 ## 1 - Metastore assignment
 
 The first step of adopting is UC is attaching your current workspace to a UC metastore.
 
-This section automatically detects if your workspace has been attached to a UC metastore, and also detects jobs that can potentially fail when attaching the workspace to the metastore.
+This section assumes that your workspace has been attached to a UC metastore, it and also detects jobs that can potentially fail when attaching the workspace to the metastore.
 
-Follow the docs below to attach your workspace to the metastore:
+If you haven't created a metastore yet, follow the docs below to attach your workspace to the metastore:
 
 [[AWS]](https://docs.databricks.com/en/data-governance/unity-catalog/enable-workspaces.html)  
 [[Azure]](https://learn.microsoft.com/en-us/azure/databricks/data-governance/unity-catalog/enable-workspaces)  
 [[GCP]](https://docs.gcp.databricks.com/data-governance/unity-catalog/enable-workspaces.html)
 
-If any incompatible submit runs has been detected, please follow the steps highlighted below:
+If any incompatible submit runs has been detected, follow the steps highlighted below:
 
 1. Find out the incompatible jobs in your local orchestrator based on the object_id identified by UCX
 2. Change the job configuration to include the following in the ClusterInfo:   “data_security_mode”: “NONE”
-3. Alternatively:
-    1. Create Cluster Policy for External Orchestrators and set “data_security_mode”: “NONE”
-    2. Assign Cluster Policy to Service Principals
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 -- widget title=Table estimates, row=2, col=0, size_x=2, size_y=8
 ## 3 - UC Data modeling
 
 The third step of a successful UC migration is defining your target data model on UC.  
-This step is required in order to choose in which catalogs yout existing data in Hive Metastore will land.
+This step is required in order to choose in which catalogs the existing data in Hive Metastore will land.
 
 As a starting point, consider creating a catalog that has the same name as your workspace. 
 For example, a table `database.table1` will land in the `workspace_name.database.table1` table.
 
 The complexity factor is relative to the number of databases and tables identified during the assessment.
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 -- viz type=table, name=Table Types, search_by=name, columns=name,type,format,storage,is_delta,location
--- widget title=Table Types, row=14, col=0, size_x=8, size_y=8
+-- widget title=Table Types, row=13, col=0, size_x=8, size_y=8
 SELECT CONCAT(tables.`database`, '.', tables.name) AS name,
        object_type AS type,
        table_format AS format,
        CASE
            WHEN STARTSWITH(location, "dbfs:/mnt") THEN "DBFS MOUNT"
            WHEN STARTSWITH(location, "/dbfs/mnt") THEN "DBFS MOUNT"
            WHEN STARTSWITH(location, "dbfs:/databricks-datasets") THEN "Databricks Demo Dataset"
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/code_patterns.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/code_patterns.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/grant_detail.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/grant_detail.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/misc_patterns.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/misc_patterns.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/objects.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/objects.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/table_estimates.sql` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/queries/views/table_estimates.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/base.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import abstractmethod
 from collections.abc import Iterable
 from dataclasses import dataclass
 
 # Code mapping between LSP, PyLint, and our own diagnostics:
 # | LSP                       | PyLint     | Our            |
 # |---------------------------|------------|----------------|
@@ -80,29 +82,32 @@
 
     @abstractmethod
     def apply(self, code: str) -> str: ...
 
 
 # The default schema to use when the schema is not specified in a table reference
 # See: https://spark.apache.org/docs/3.0.0-preview/sql-ref-syntax-qry-select-usedb.html
+DEFAULT_CATALOG = 'hive_metastore'
 DEFAULT_SCHEMA = 'default'
 
 
 @dataclass
 class CurrentSessionState:
     """
     A data class that represents the current state of a session.
 
     This class can be used to track various aspects of a session, such as the current schema.
 
     Attributes:
+        catalog (str): The current schema of the session. If not provided, it defaults to 'DEFAULT_CATALOG'.
         schema (str): The current schema of the session. If not provided, it defaults to 'DEFAULT_SCHEMA'.
     """
 
     schema: str = DEFAULT_SCHEMA
+    catalog: str = DEFAULT_CATALOG
 
 
 class SequentialLinter(Linter):
     def __init__(self, linters: list[Linter]):
         self._linters = linters
 
     def lint(self, code: str) -> Iterable[Advice]:
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/dbfs.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/dbfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def lint(self, code: str) -> Iterable[Advice]:
         """
         Lints the code looking for file system paths that are deprecated
         """
         tree = ast.parse(code)
         visitor = DetectDbfsVisitor()
         visitor.visit(tree)
-        return visitor.get_advices()
+        yield from visitor.get_advices()
 
 
 class FromDbfsFolder(Linter):
     def __init__(self):
         self._dbfs_prefixes = ["/dbfs/mnt", "dbfs:/", "/mnt/", "/dbfs/", "/"]
 
     @staticmethod
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/languages.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/languages.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from databricks.labs.ucx.source_code.pyspark import SparkSql
 from databricks.labs.ucx.source_code.queries import FromTable
 from databricks.labs.ucx.source_code.dbfs import DBFSUsageLinter, FromDbfsFolder
 from databricks.labs.ucx.source_code.table_creation import DBRv8d0Linter
 
 
 class Languages:
-    def __init__(self, index: MigrationIndex):
+    def __init__(self, index: MigrationIndex, session_state: CurrentSessionState | None = None):
         self._index = index
-        session_state = CurrentSessionState()
+        session_state = CurrentSessionState() if not session_state else session_state
         from_table = FromTable(index, session_state=session_state)
         dbfs_from_folder = FromDbfsFolder()
         self._linters = {
             Language.PYTHON: SequentialLinter(
                 [
                     SparkSql(from_table, index),
                     DBFSUsageLinter(),
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/lsp.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/lsp.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/notebook.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/notebooks/cells.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-from __future__ import annotations  # for type hints
+from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from ast import parse as parse_python
-from collections.abc import Callable
 from enum import Enum
 from pathlib import Path
+from sqlglot import parse as parse_sql, ParseError as SQLParseError
 
-from sqlglot import ParseError as SQLParseError
-from sqlglot import parse as parse_sql
 from databricks.sdk.service.workspace import Language
+from databricks.labs.ucx.source_code.graph import DependencyGraph, DependencyProblem
 
-from databricks.labs.ucx.source_code.dependencies import (
-    DependencyGraph,
-    DependencyProblem,
-)
-from databricks.labs.ucx.source_code.dependency_loaders import SourceContainer
-
-
-logger = logging.getLogger(__name__)
 # use a specific logger for sqlglot warnings so we can disable them selectively
 sqlglot_logger = logging.getLogger(f"{__name__}.sqlglot")
 
 NOTEBOOK_HEADER = "Databricks notebook source"
 CELL_SEPARATOR = "COMMAND ----------"
 MAGIC_PREFIX = 'MAGIC'
 LANGUAGE_PREFIX = '%'
@@ -58,17 +49,19 @@
     def language(self) -> CellLanguage:
         raise NotImplementedError()
 
     @abstractmethod
     def is_runnable(self) -> bool:
         raise NotImplementedError()
 
-    @abstractmethod
-    def build_dependency_graph(self, parent: DependencyGraph, problem_collector: Callable[[DependencyProblem], None]):
-        raise NotImplementedError()
+    def build_dependency_graph(self, _: DependencyGraph) -> list[DependencyProblem]:
+        return []
+
+    def __repr__(self):
+        return f"{self.language.name}: {self._original_code[:20]}"
 
 
 class PythonCell(Cell):
 
     @property
     def language(self):
         return CellLanguage.PYTHON
@@ -76,43 +69,37 @@
     def is_runnable(self) -> bool:
         try:
             tree = parse_python(self._original_code)
             return tree is not None
         except SyntaxError:
             return True
 
-    def build_dependency_graph(self, parent: DependencyGraph, problem_collector: Callable[[DependencyProblem], None]):
-        parent.build_graph_from_python_source(self._original_code, problem_collector)
+    def build_dependency_graph(self, parent: DependencyGraph) -> list[DependencyProblem]:
+        return parent.build_graph_from_python_source(self._original_code)
 
 
 class RCell(Cell):
 
     @property
     def language(self):
         return CellLanguage.R
 
     def is_runnable(self) -> bool:
         return True  # TODO
 
-    def build_dependency_graph(self, parent: DependencyGraph, problem_collector: Callable[[DependencyProblem], None]):
-        pass  # not in scope
-
 
 class ScalaCell(Cell):
 
     @property
     def language(self):
         return CellLanguage.SCALA
 
     def is_runnable(self) -> bool:
         return True  # TODO
 
-    def build_dependency_graph(self, parent: DependencyGraph, problem_collector: Callable[[DependencyProblem], None]):
-        pass  # TODO
-
 
 class SQLCell(Cell):
 
     @property
     def language(self):
         return CellLanguage.SQL
 
@@ -120,104 +107,88 @@
         try:
             statements = parse_sql(self._original_code)
             return len(statements) > 0
         except SQLParseError as e:
             sqlglot_logger.warning(f"Failed to parse SQL using 'sqlglot': {self._original_code}", exc_info=e)
             return True
 
-    def build_dependency_graph(self, parent: DependencyGraph, problem_collector: Callable[[DependencyProblem], None]):
-        pass  # not in scope
-
 
 class MarkdownCell(Cell):
 
     @property
     def language(self):
         return CellLanguage.MARKDOWN
 
     def is_runnable(self) -> bool:
         return True  # TODO
 
-    def build_dependency_graph(self, parent: DependencyGraph, problem_collector: Callable[[DependencyProblem], None]):
-        pass  # not in scope
-
 
 class RunCell(Cell):
 
     @property
     def language(self):
         return CellLanguage.RUN
 
     def is_runnable(self) -> bool:
         return True  # TODO
 
-    def build_dependency_graph(self, parent: DependencyGraph, problem_collector: Callable[[DependencyProblem], None]):
+    def build_dependency_graph(self, parent: DependencyGraph) -> list[DependencyProblem]:
         command = f'{LANGUAGE_PREFIX}{self.language.magic_name}'
         lines = self._original_code.split('\n')
         for idx, line in enumerate(lines):
             start = line.index(command)
             if start >= 0:
                 path = line[start + len(command) :]
                 path = path.strip().strip("'").strip('"')
                 if len(path) == 0:
                     continue
-                problems: list[DependencyProblem] = []
-                parent.register_notebook(Path(path), problems.append)
+                notebook_path = Path(path)
                 start_line = self._original_offset + idx + 1
-                for problem in problems:
-                    problem = problem.replace(
-                        start_line=start_line, start_col=0, end_line=start_line, end_col=len(line)
-                    )
-                    problem_collector(problem)
-                return
+                problems = parent.register_notebook(notebook_path)
+                return [
+                    problem.replace(start_line=start_line, start_col=0, end_line=start_line, end_col=len(line))
+                    for problem in problems
+                ]
         start_line = self._original_offset + 1
         problem = DependencyProblem(
-            'dependency-check',
+            'invalid-run-cell',
             "Missing notebook path in %run command",
             start_line=start_line,
             start_col=0,
             end_line=start_line,
             end_col=len(self._original_code),
         )
-        problem_collector(problem)
+        return [problem]
 
     def migrate_notebook_path(self):
         pass
 
 
 class ShellCell(Cell):
 
     @property
     def language(self):
         return CellLanguage.SHELL
 
     def is_runnable(self) -> bool:
         return True  # TODO
 
-    def build_dependency_graph(self, parent: DependencyGraph, problem_collector: Callable[[DependencyProblem], None]):
-        pass  # nothing to do
-
-    def migrate_notebook_path(self):
-        pass  # nothing to do
-
 
 class PipCell(Cell):
 
     @property
     def language(self):
         return CellLanguage.PIP
 
     def is_runnable(self) -> bool:
         return True  # TODO
 
-    def build_dependency_graph(self, parent: DependencyGraph, problem_collector: Callable[[DependencyProblem], None]):
-        pass  # nothing to do
-
-    def migrate_notebook_path(self):
-        pass
+    def build_dependency_graph(self, _: DependencyGraph) -> list[DependencyProblem]:
+        # TODO: https://github.com/databrickslabs/ucx/issues/1642
+        return []
 
 
 class CellLanguage(Enum):
     # long magic_names must come first to avoid shorter ones being matched
     PYTHON = Language.PYTHON, 'python', '#', True, PythonCell
     SCALA = Language.SCALA, 'scala', '//', True, ScalaCell
     SQL = Language.SQL, 'sql', '--', True, SQLCell
@@ -234,14 +205,18 @@
         self._magic_name = args[1]
         self._comment_prefix = args[2]
         # PI stands for Processing Instruction
         self._requires_isolated_pi = args[3]
         self._new_cell = args[4]
 
     @property
+    def file_magic_header(self):
+        return f"{self._comment_prefix} {NOTEBOOK_HEADER}"
+
+    @property
     def language(self) -> Language:
         return self._language
 
     @property
     def magic_name(self) -> str:
         return self._magic_name
 
@@ -280,16 +255,15 @@
         return None
 
     def new_cell(self, source: str, original_offset: int) -> Cell:
         return self._new_cell(source, original_offset)
 
     def extract_cells(self, source: str) -> list[Cell] | None:
         lines = source.split('\n')
-        header = f"{self.comment_prefix} {NOTEBOOK_HEADER}"
-        if not lines[0].startswith(header):
+        if not lines[0].startswith(self.file_magic_header):
             raise ValueError("Not a Databricks notebook source!")
 
         def make_cell(cell_lines: list[str], start: int):
             # trim leading blank lines
             while len(cell_lines) > 0 and len(cell_lines[0]) == 0:
                 cell_lines.pop(0)
                 start += 1
@@ -363,60 +337,7 @@
                 lines[i] = line[comment_pi_prefix_len:]
                 continue
             line = f"{self.comment_prefix} {MAGIC_PREFIX} {line}"
             lines[i] = line
         if code.endswith('./'):
             lines.append('\n')
         return "\n".join(lines)
-
-
-class Notebook(SourceContainer):
-
-    @staticmethod
-    def parse(path: str, source: str, default_language: Language) -> Notebook:
-        default_cell_language = CellLanguage.of_language(default_language)
-        cells = default_cell_language.extract_cells(source)
-        if cells is None:
-            raise ValueError(f"Could not parse Notebook: {path}")
-        return Notebook(path, source, default_language, cells, source.endswith('\n'))
-
-    def __init__(self, path: str, source: str, language: Language, cells: list[Cell], ends_with_lf):
-        self._path = path
-        self._source = source
-        self._language = language
-        self._cells = cells
-        self._ends_with_lf = ends_with_lf
-
-    @property
-    def path(self) -> str:
-        return self._path
-
-    @property
-    def cells(self) -> list[Cell]:
-        return self._cells
-
-    @property
-    def original_code(self) -> str:
-        return self._source
-
-    def to_migrated_code(self):
-        default_language = CellLanguage.of_language(self._language)
-        header = f"{default_language.comment_prefix} {NOTEBOOK_HEADER}"
-        sources = [header]
-        for i, cell in enumerate(self._cells):
-            migrated_code = cell.migrated_code
-            if cell.language is not default_language:
-                migrated_code = default_language.wrap_with_magic(migrated_code, cell.language)
-            sources.append(migrated_code)
-            if i < len(self._cells) - 1:
-                sources.append('')
-                sources.append(f'{default_language.comment_prefix} {CELL_SEPARATOR}')
-                sources.append('')
-        if self._ends_with_lf:
-            sources.append('')  # following join will append lf
-        return '\n'.join(sources)
-
-    def build_dependency_graph(self, parent: DependencyGraph) -> None:
-        problems: list[DependencyProblem] = []
-        for cell in self._cells:
-            cell.build_dependency_graph(parent, problems.append)
-        parent.add_problems(problems)
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/pyspark.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/pyspark.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,36 +8,15 @@
     Advice,
     Advisory,
     Deprecation,
     Fixer,
     Linter,
 )
 from databricks.labs.ucx.source_code.queries import FromTable
-
-
-class AstHelper:
-    @staticmethod
-    def get_full_function_name(node):
-        if isinstance(node.func, ast.Attribute):
-            return AstHelper._get_value(node.func)
-
-        if isinstance(node.func, ast.Name):
-            return node.func.id
-
-        return None
-
-    @staticmethod
-    def _get_value(node):
-        if isinstance(node.value, ast.Name):
-            return node.value.id + '.' + node.attr
-
-        if isinstance(node.value, ast.Attribute):
-            return AstHelper._get_value(node.value) + '.' + node.attr
-
-        return None
+from databricks.labs.ucx.source_code.ast_helpers import AstHelper
 
 
 @dataclass
 class Matcher(ABC):
     method_name: str
     min_args: int
     max_args: int
@@ -247,14 +226,15 @@
 
         # see https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.Catalog.html
         spark_catalog_matchers = [
             TableNameMatcher("cacheTable", 1, 2, 0, "tableName"),
             TableNameMatcher("createTable", 1, 1000, 0, "tableName"),
             TableNameMatcher("createExternalTable", 1, 1000, 0, "tableName"),
             TableNameMatcher("getTable", 1, 1, 0),
+            TableNameMatcher("table", 1, 1, 0),
             TableNameMatcher("isCached", 1, 1, 0),
             TableNameMatcher("listColumns", 1, 2, 0, "tableName"),
             TableNameMatcher("tableExists", 1, 2, 0, "tableName"),
             TableNameMatcher("recoverPartitions", 1, 1, 0),
             TableNameMatcher("refreshTable", 1, 1, 0),
             TableNameMatcher("uncacheTable", 1, 1, 0),
             ReturnValueMatcher("listTables", 0, 2, -1),
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/python_linter.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/python_linter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import abc
 import ast
 import logging
 from collections.abc import Iterable
-from typing import TypeVar, Generic
+from typing import TypeVar, Generic, cast
 
 from databricks.labs.ucx.source_code.base import Linter, Advice, Advisory
 
 logger = logging.getLogger(__name__)
 
 
 class MatchingVisitor(ast.NodeVisitor):
@@ -59,43 +59,66 @@
             raise NotImplementedError(str(type(node)))
         if next_node is None:
             # is this the last node to match ?
             return len(self._match_nodes) - 1 == depth
         return self._matches(next_node, depth + 1)
 
 
-class SysPath(abc.ABC):
+class NodeBase(abc.ABC):
 
-    def __init__(self, path: str):
+    def __init__(self, node: ast.AST):
+        self._node = node
+
+    @property
+    def node(self):
+        return self._node
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__}: {ast.unparse(self._node)}>"
+
+
+class SysPathChange(NodeBase, abc.ABC):
+
+    def __init__(self, node: ast.AST, path: str, is_append: bool):
+        super().__init__(node)
         self._path = path
+        self._is_append = is_append
+
+    @property
+    def node(self):
+        return self._node
 
     @property
     def path(self):
         return self._path
 
+    @property
+    def is_append(self):
+        return self._is_append
+
 
 # path directly added to sys.path
-class AbsolutePath(SysPath):
+class AbsolutePath(SysPathChange):
     pass
 
 
 # path added to sys.path using os.path.abspath
-class RelativePath(SysPath):
+class RelativePath(SysPathChange):
     pass
 
 
 class SysPathVisitor(ast.NodeVisitor):
 
     def __init__(self):
         self._aliases: dict[str, str] = {}
-        self._appended_paths: list[SysPath] = []
+        self._syspath_changes: list[SysPathChange] = []
 
     @property
-    def appended_paths(self):
-        return self._appended_paths
+    def syspath_changes(self):
+        return self._syspath_changes
 
     def visit_Import(self, node: ast.Import):
         for alias in node.names:
             if alias.name in {"sys", "os"}:
                 self._aliases[alias.name] = alias.asname or alias.name
 
     def visit_ImportFrom(self, node: ast.ImportFrom):
@@ -105,43 +128,47 @@
             return
         for alias in node.names:
             if alias.name == interesting_alias[1]:
                 self._aliases[f"{node.module}.{interesting_alias[1]}"] = alias.asname or alias.name
                 break
 
     def visit_Call(self, node: ast.Call):
+        func = cast(ast.Attribute, node.func)
         # check for 'sys.path.append'
-        if not self._match_aliases(node.func, ["sys", "path", "append"]):
+        if not (
+            self._match_aliases(func, ["sys", "path", "append"]) or self._match_aliases(func, ["sys", "path", "insert"])
+        ):
             return
-        appended = node.args[0]
-        if isinstance(appended, ast.Constant):
-            self._appended_paths.append(AbsolutePath(appended.value))
-        elif isinstance(appended, ast.Call):
-            self._append_relative_path(appended)
+        is_append = func.attr == "append"
+        changed = node.args[0] if is_append else node.args[1]
+        if isinstance(changed, ast.Constant):
+            self._syspath_changes.append(AbsolutePath(node, changed.value, is_append))
+        elif isinstance(changed, ast.Call):
+            self._visit_relative_path(changed, is_append)
 
     def _match_aliases(self, node: ast.AST, names: list[str]):
         if isinstance(node, ast.Attribute):
             if node.attr != names[-1]:
                 return False
             if len(names) == 1:
                 return True
             return self._match_aliases(node.value, names[0 : len(names) - 1])
         if isinstance(node, ast.Name):
             full_name = ".".join(names)
             alias = self._aliases.get(full_name, full_name)
             return node.id == alias
         return False
 
-    def _append_relative_path(self, node: ast.Call):
+    def _visit_relative_path(self, node: ast.Call, is_append: bool):
         # check for 'os.path.abspath'
         if not self._match_aliases(node.func, ["os", "path", "abspath"]):
             return
-        appended = node.args[0]
-        if isinstance(appended, ast.Constant):
-            self._appended_paths.append(RelativePath(appended.value))
+        changed = node.args[0]
+        if isinstance(changed, ast.Constant):
+            self._syspath_changes.append(RelativePath(changed, changed.value, is_append))
 
 
 T = TypeVar("T", bound=ast.AST)
 
 
 # disclaimer this class is NOT thread-safe
 class ASTLinter(Generic[T]):
@@ -155,18 +182,18 @@
         self._root: ast.AST = root
 
     def locate(self, node_type: type[T], match_nodes: list[tuple[str, type]]) -> list[T]:
         visitor = MatchingVisitor(node_type, match_nodes)
         visitor.visit(self._root)
         return visitor.matched_nodes
 
-    def collect_appended_sys_paths(self):
+    def collect_sys_paths_changes(self):
         visitor = SysPathVisitor()
         visitor.visit(self._root)
-        return visitor.appended_paths
+        return visitor.syspath_changes
 
     def extract_callchain(self) -> ast.Call | None:
         """If 'node' is an assignment or expression, extract its full call-chain (if it has one)"""
         call = None
         if isinstance(self._root, ast.Assign):
             call = self._root.value
         elif isinstance(self._root, ast.Expr):
@@ -212,21 +239,47 @@
     def is_none(self) -> bool:
         """Check if the given AST expression is the None constant"""
         assert isinstance(self._root, ast.expr)
         if not isinstance(self._root, ast.Constant):
             return False
         return self._root.value is None
 
+    def __repr__(self):
+        truncate_after = 32
+        code = ast.unparse(self._root)
+        if len(code) > truncate_after:
+            code = code[0:truncate_after] + "..."
+        return f"<ASTLinter: {code}>"
+
+
+class ImportSource(NodeBase):
+
+    def __init__(self, node: ast.AST, name: str):
+        super().__init__(node)
+        self.name = name
+
+
+class NotebookRunCall(NodeBase):
+
+    def __init__(self, node: ast.Call):
+        super().__init__(node)
+
+    def get_constant_path(self) -> str | None:
+        path = PythonLinter.get_dbutils_notebook_run_path_arg(cast(ast.Call, self.node))
+        if isinstance(path, ast.Constant):
+            return path.value.strip().strip("'").strip('"')
+        return None
+
 
 class PythonLinter(Linter):
 
     def lint(self, code: str) -> Iterable[Advice]:
         linter = ASTLinter.parse(code)
         nodes = self.list_dbutils_notebook_run_calls(linter)
-        return [self._convert_dbutils_notebook_run_to_advice(node) for node in nodes]
+        return [self._convert_dbutils_notebook_run_to_advice(node.node) for node in nodes]
 
     @classmethod
     def _convert_dbutils_notebook_run_to_advice(cls, node: ast.AST) -> Advisory:
         assert isinstance(node, ast.Call)
         path = cls.get_dbutils_notebook_run_path_arg(node)
         if isinstance(path, ast.Constant):
             return Advisory(
@@ -250,25 +303,31 @@
     def get_dbutils_notebook_run_path_arg(node: ast.Call):
         if len(node.args) > 0:
             return node.args[0]
         arg = next(kw for kw in node.keywords if kw.arg == "path")
         return arg.value if arg is not None else None
 
     @staticmethod
-    def list_dbutils_notebook_run_calls(linter: ASTLinter) -> list[ast.Call]:
-        return linter.locate(ast.Call, [("run", ast.Attribute), ("notebook", ast.Attribute), ("dbutils", ast.Name)])
+    def list_dbutils_notebook_run_calls(linter: ASTLinter) -> list[NotebookRunCall]:
+        calls = linter.locate(ast.Call, [("run", ast.Attribute), ("notebook", ast.Attribute), ("dbutils", ast.Name)])
+        return [NotebookRunCall(call) for call in calls]
 
     @staticmethod
-    def list_import_sources(linter: ASTLinter) -> list[tuple[str, ast.AST]]:
-        nodes = linter.locate(ast.Import, [])
-        tuples = [(alias.name, node) for node in nodes for alias in node.names]
-        nodes = linter.locate(ast.ImportFrom, [])
-        tuples.extend((node.module, node) for node in nodes)
-        nodes = linter.locate(ast.Call, [("import_module", ast.Attribute), ("importlib", ast.Name)])
-        tuples.extend((node.args[0].value, node) for node in nodes)
-        nodes = linter.locate(ast.Call, [("__import__", ast.Attribute), ("importlib", ast.Name)])
-        tuples.extend((node.args[0].value, node) for node in nodes)
-        return tuples
+    def list_import_sources(linter: ASTLinter) -> list[ImportSource]:
+        # TODO: make this code more robust, because it fails detecting imports on UCX codebase
+        try:  # pylint: disable=too-many-try-statements
+            nodes = linter.locate(ast.Import, [])
+            sources = [ImportSource(node, alias.name) for node in nodes for alias in node.names]
+            nodes = linter.locate(ast.ImportFrom, [])
+            sources.extend(ImportSource(node, node.module) for node in nodes)
+            nodes = linter.locate(ast.Call, [("import_module", ast.Attribute), ("importlib", ast.Name)])
+            sources.extend(ImportSource(node, node.args[0].value) for node in nodes)
+            nodes = linter.locate(ast.Call, [("__import__", ast.Attribute), ("importlib", ast.Name)])
+            sources.extend(ImportSource(node, node.args[0].value) for node in nodes)
+            return sources
+        except Exception as e:  # pylint: disable=broad-except
+            logger.warning(f"{linter} imports: {e}")
+            return []
 
     @staticmethod
-    def list_appended_sys_paths(linter: ASTLinter) -> list[SysPath]:
-        return linter.collect_appended_sys_paths()
+    def list_sys_path_changes(linter: ASTLinter) -> list[SysPathChange]:
+        return linter.collect_sys_paths_changes()
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/queries.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         show how sqlglot represents them:::
 
                 catalog.schema.table    -> Table(catalog='catalog', db='schema', this='table')
                 schema.table                 -> Table(catalog='', db='schema', this='table')
                 table                               -> Table(catalog='', db='', this='table')
         """
         self._index: MigrationIndex = index
-        self._session_state: CurrentSessionState = session_state if session_state else CurrentSessionState()
+        self._session_state: CurrentSessionState = session_state
 
     def name(self) -> str:
         return 'table-migrate'
 
     @property
     def schema(self):
         return self._session_state.schema
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/table_creation.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/source_code/table_creation.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/base.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
     @abstractmethod
     def object_types(self) -> set[str]:
         """This method returns a set of strings, that represent object types that are applicable by this instance."""
 
 
 class StaticListing:
-    """This class is only supposed to be used in testing scenarios."""
+    """This class is only supposed to be used in testing scenarios.
+    It returns a static list of permissions specific object types, that can be used to test the ACL support classes."""
 
     def __init__(self, include_object_permissions: list[str], object_types: set[str]):
         self._include_object_permissions = include_object_permissions
         self._object_types = object_types
 
     def __iter__(self):
         for pair in self._include_object_permissions:
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/clusters.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/clusters.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/generic.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,29 +51,34 @@
         self._object_type = object_type
 
     def object_types(self) -> set[str]:
         return {self._object_type}
 
     def __iter__(self):
         started = datetime.datetime.now()
-        for item in self._func():
-            yield GenericPermissionsInfo(getattr(item, self._id_attribute), self._object_type)
+        try:
+            for item in self._func():
+                yield GenericPermissionsInfo(getattr(item, self._id_attribute), self._object_type)
+        except NotFound as e:
+            logger.error(f"Listing {self._object_type} failed: {e}")
         since = datetime.datetime.now() - started
         logger.info(f"Listed {self._object_type} in {since}")
 
     def __repr__(self):
         return f"Listing({self._object_type} via {self._func.__qualname__})"
 
 
 class GenericPermissionsSupport(AclSupport):
     def __init__(
         self,
         ws: WorkspaceClient,
         listings: list[Listing],
         verify_timeout: timedelta | None = timedelta(minutes=1),
+        # this parameter is for testing scenarios only - [{object_type}:{object_id}]
+        # it will use StaticListing class to return only object ids that has the same object type
         include_object_permissions: list[str] | None = None,
     ):
         self._ws = ws
         self._listings = listings
         self._verify_timeout = verify_timeout
         self._include_object_permissions = include_object_permissions
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/groups.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/groups.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/listing.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/listing.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/manager.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/manager.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/redash.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/redash.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         set_permissions_timeout: timedelta | None = timedelta(minutes=1),
         # Group information in Redash are cached for up to 10 minutes causing inconsistencies.
         # If a group is renamed, the old name may still be returned by the dbsql get permissions api.
         # Note that the update/set API is strongly consistent and is not affected by this behaviour.
         # The validation step should keep retrying for at least 10 mins until the get api returns the new group name.
         # More details here: https://databricks.atlassian.net/browse/ES-992619
         verify_timeout: timedelta | None = timedelta(minutes=11),
+        # this parameter is for testing scenarios only - [{object_type}:{object_id}]
+        # it will use StaticListing class to return only object ids that has the same object type
         include_object_permissions: list[str] | None = None,
     ):
         self._ws = ws
         self._listings = listings
         self._set_permissions_timeout = set_permissions_timeout
         self._verify_timeout = verify_timeout
         self._include_object_permissions = include_object_permissions
@@ -69,15 +71,15 @@
         assert permissions_response.access_control_list is not None
         mentioned_groups = [acl.group_name for acl in permissions_response.access_control_list]
         return any(g in mentioned_groups for g in [info.name_in_workspace for info in migration_state.groups])
 
     def get_crawler_tasks(self):
         if self._include_object_permissions:
             for item in StaticListing(self._include_object_permissions, self.object_types()):
-                yield partial(self._crawler_task, item.object_id, item.object_type)
+                yield partial(self._crawler_task, item.object_id, sql.ObjectTypePlural(item.object_type))
             return
         for listing in self._listings:
             for item in listing:
                 yield partial(self._crawler_task, item.object_id, item.request_type)
 
     def object_types(self) -> set[str]:
         all_object_types = set()
@@ -187,17 +189,16 @@
         set_retried_check = set_retry_on_value_error(self._safe_set_permissions)
         set_retried_check(object_type, object_id, acl)
 
         retry_on_value_error = retried(on=[InternalError, NotFound], timeout=self._verify_timeout)
         retried_check = retry_on_value_error(self._verify)
         return retried_check(object_type, object_id, acl)
 
-    def _prepare_new_acl(
-        self, acl: list[sql.AccessControl], migration_state: MigrationState
-    ) -> list[sql.AccessControl]:
+    @staticmethod
+    def _prepare_new_acl(acl: list[sql.AccessControl], migration_state: MigrationState) -> list[sql.AccessControl]:
         """
         Please note the comment above on how we apply these permissions.
         Permissions are set/replaced and not updated/patched, therefore all existing ACLs need to be collected
         including users and temp/backup groups.
         """
         acl_requests: list[sql.AccessControl] = []
         for access_control in acl:
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/scim.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/scim.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/secrets.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/secrets.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,39 +6,51 @@
 
 from databricks.labs.blueprint.limiter import rate_limited
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.retries import retried
 from databricks.sdk.service import workspace
 from databricks.sdk.service.workspace import AclItem
 
-from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions
+from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions, StaticListing
 from databricks.labs.ucx.workspace_access.groups import MigrationState
 
 logger = logging.getLogger(__name__)
 
 
 class SecretScopesSupport(AclSupport):
-    def __init__(self, ws: WorkspaceClient, verify_timeout: timedelta | None = None):
+    def __init__(
+        self,
+        ws: WorkspaceClient,
+        verify_timeout: timedelta | None = None,
+        # this parameter is for testing scenarios only - [{object_type}:{object_id}]
+        # it will use StaticListing class to return only object ids that has the same object type
+        include_object_permissions: list[str] | None = None,
+    ):
         self._ws = ws
         if verify_timeout is None:
             verify_timeout = timedelta(minutes=2)
         self._verify_timeout = verify_timeout
+        self._include_object_permissions = include_object_permissions
 
     def get_crawler_tasks(self):
-        scopes = self._ws.secrets.list_scopes()
-
         def _crawler_task(scope: workspace.SecretScope):
             assert scope.name is not None
             acl_items = self._ws.secrets.list_acls(scope.name)
             return Permissions(
                 object_id=scope.name,
                 object_type="secrets",
                 raw=json.dumps([item.as_dict() for item in acl_items]),
             )
 
+        if self._include_object_permissions:
+            for item in StaticListing(self._include_object_permissions, self.object_types()):
+                yield partial(_crawler_task, workspace.SecretScope(name=item.object_id))
+            return
+
+        scopes = self._ws.secrets.list_scopes()
         for scope in scopes:
             yield partial(_crawler_task, scope)
 
     def object_types(self) -> set[str]:
         return {"secrets"}
 
     def get_apply_task(self, item: Permissions, migration_state: MigrationState):
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/tacl.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/tacl.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 class TableAclSupport(AclSupport):
     def __init__(
         self,
         grants_crawler: GrantsCrawler,
         sql_backend: SqlBackend,
         verify_timeout: timedelta | None = timedelta(minutes=1),
+        # this parameter is for testing scenarios only - [{object_type}:{object_id}]
+        # it will use StaticListing class to return only object ids that has the same object type
         include_object_permissions: list[str] | None = None,
     ):
         self._grants_crawler = grants_crawler
         self._sql_backend = sql_backend
         self._verify_timeout = verify_timeout
         self._include_object_permissions = include_object_permissions
```

### Comparing `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/workflows.py` & `databricks_labs_ucx-0.23.0/databricks/labs/ucx/workspace_access/workflows.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/.gitignore` & `databricks_labs_ucx-0.23.0/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/LICENSE` & `databricks_labs_ucx-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/NOTICE` & `databricks_labs_ucx-0.23.0/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.22.0/README.md` & `databricks_labs_ucx-0.23.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Databricks Labs UCX
 ===
 ![UCX by Databricks Labs](docs/logo-no-background.png)
 
-The companion for upgrading to Unity Catalog. After [installation](#install-ucx), ensure to [trigger](#ensure-assessment-run-command) the [assessment workflow](#assessment-workflow), 
-so that you'll be able to [scope the migration](docs/assessment.md) and execute the [group migration workflow](#group-migration-workflow). 
-[`<installation_path>/README`](#readme-notebook) contains further instructions and explanations of these workflows. 
-Then you can execute [table migration workflow](#table-migration-workflow).
-More workflows, like notebook code migration is coming in the future releases. 
-UCX exposes a number of command line utilities accessible via `databricks labs ucx`.
+The companion for upgrading to Unity Catalog. 
+
+After [installation](#install-ucx), ensure to [trigger](#ensure-assessment-run-command) the [assessment workflow](#assessment-workflow), 
+so that you'll be able to [scope the migration](docs/assessment.md) and execute the [group migration workflow](#group-migration-workflow).
+
+The [README notebook](#readme-notebook), which can be found in the installation folder contains further instructions and explanations of the different ucx workflows & dashboards. 
+Once the migration is scoped, you can start executing the [table migration workflow](#table-migration-workflow).
+
+More workflows, like notebook code migration are coming in future releases.
+
+UCX also provides a number of command line utilities accessible via `databricks labs ucx`.
 
 For questions, troubleshooting or bug fixes, please see our [troubleshooting guide](docs/troubleshooting.md) or submit [an issue](https://github.com/databrickslabs/ucx/issues). 
 See [contributing instructions](CONTRIBUTING.md) to help improve this project.
 
-[![build](https://github.com/databrickslabs/ucx/actions/workflows/push.yml/badge.svg)](https://github.com/databrickslabs/ucx/actions/workflows/push.yml) [![codecov](https://codecov.io/github/databrickslabs/ucx/graph/badge.svg?token=p0WKAfW5HQ)](https://codecov.io/github/databrickslabs/ucx)  [![lines of code](https://tokei.rs/b1/github/databrickslabs/ucx)]([https://codecov.io/github/databrickslabs/ucx](https://github.com/databrickslabs/ucx))
+[![build](https://github.com/databrickslabs/ucx/actions/workflows/push.yml/badge.svg)](https://github.com/databrickslabs/ucx/actions/workflows/push.yml) [![codecov](https://codecov.io/github/databrickslabs/ucx/graph/badge.svg?token=p0WKAfW5HQ)](https://codecov.io/github/databrickslabs/ucx)  ![linesofcode](https://aschey.tech/tokei/github/databrickslabs/ucx?category=code)
 
 <!-- TOC -->
 * [Databricks Labs UCX](#databricks-labs-ucx)
 * [Installation](#installation)
   * [Authenticate Databricks CLI](#authenticate-databricks-cli)
   * [Install UCX](#install-ucx)
   * [[ADVANCED] Force install over existing UCX](#advanced-force-install-over-existing-ucx)
@@ -37,33 +42,37 @@
 * [Utility commands](#utility-commands)
   * [`logs` command](#logs-command)
   * [`ensure-assessment-run` command](#ensure-assessment-run-command)
   * [`repair-run` command](#repair-run-command)
   * [`workflows` command](#workflows-command)
   * [`open-remote-config` command](#open-remote-config-command)
   * [`installations` command](#installations-command)
+  * [`report-account-compatibility` command](#report-account-compatibility-command)
 * [Metastore related commands](#metastore-related-commands)
   * [`show-all-metastores` command](#show-all-metastores-command)
   * [`assign-metastore` command](#assign-metastore-command)
 * [Table migration commands](#table-migration-commands)
   * [`principal-prefix-access` command](#principal-prefix-access-command)
     * [Access for AWS S3 Buckets](#access-for-aws-s3-buckets)
     * [Access for Azure Storage Accounts](#access-for-azure-storage-accounts)
   * [`create-uber-principal` command](#create-uber-principal-command)
   * [`migrate-credentials` command](#migrate-credentials-command)
   * [`validate-external-locations` command](#validate-external-locations-command)
   * [`migrate-locations` command](#migrate-locations-command)
   * [`create-table-mapping` command](#create-table-mapping-command)
   * [`skip` command](#skip-command)
-  * [`revert-migrated-tables` command](#revert-migrated-tables-command)
   * [`create-catalogs-schemas` command](#create-catalogs-schemas-command)
+  * [`migrate-tables` command](#migrate-tables-command)
+  * [`revert-migrated-tables` command](#revert-migrated-tables-command)
   * [`move` command](#move-command)
   * [`alias` command](#alias-command)
 * [Code migration commands](#code-migration-commands)
   * [`migrate-local-code` command](#migrate-local-code-command)
+  * [`migrate-dbsql-dashboards` command](#migrate-dbsql-dashboards-command)
+  * [`revert-dbsql-dashboards` command](#revert-dbsql-dashboards-command)
 * [Cross-workspace installations](#cross-workspace-installations)
   * [`sync-workspace-info` command](#sync-workspace-info-command)
   * [`manual-workspace-info` command](#manual-workspace-info-command)
   * [`create-account-groups` command](#create-account-groups-command)
   * [`validate-groups-membership` command](#validate-groups-membership-command)
   * [`cluster-remap` command](#cluster-remap-command)
   * [`revert-cluster-remap` command](#revert-cluster-remap-command)
@@ -77,15 +86,15 @@
 - Python 3.10 or later. See [Windows](https://www.python.org/downloads/windows/) instructions.
 - Network access to your Databricks Workspace used for the [installation process](#install-ucx).
 - Network access to the Internet for [pypi.org](https://pypi.org) and [github.com](https://github.com) from machine running the installation.
 - Databricks Workspace Administrator privileges for the user, that runs the installation. Running UCX as a Service Principal is not supported.
 - Account level Identity Setup. See instructions for [AWS](https://docs.databricks.com/en/administration-guide/users-groups/best-practices.html), [Azure](https://learn.microsoft.com/en-us/azure/databricks/administration-guide/users-groups/best-practices), and [GCP](https://docs.gcp.databricks.com/administration-guide/users-groups/best-practices.html).
 - Unity Catalog Metastore Created (per region). See instructions for [AWS](https://docs.databricks.com/en/data-governance/unity-catalog/create-metastore.html), [Azure](https://learn.microsoft.com/en-us/azure/databricks/data-governance/unity-catalog/create-metastore), and [GCP](https://docs.gcp.databricks.com/data-governance/unity-catalog/create-metastore.html).
 - If your Databricks Workspace relies on an external Hive Metastore (such as AWS Glue), make sure to read [this guide](docs/external_hms_glue.md).
-- Databricks Workspace has to have network access to [pypi.org](https://pypi.org) to download `databricks-sdk` and `pyyaml` packages.
+- Databricks Workspace has to have network access to [pypi.org](https://pypi.org) to download `databricks-sdk`, `databricks-labs-lsql`, `databricks-labs-blueprint`, `sqlglot` and `pyyaml` packages.
 - A PRO or Serverless SQL Warehouse to render the [report](docs/assessment.md) for the [assessment workflow](#assessment-workflow).
 
 Once you [install UCX](#install-ucx), you can proceed to the [assessment workflow](#assessment-workflow) to ensure 
 the compatibility of your workspace with Unity Catalog.
 
 [[back to top](#databricks-labs-ucx)]
 
@@ -371,33 +380,37 @@
 ```mermaid
 flowchart TB
     subgraph CLI
       sync-workspace-info[sync-workspace-info] --> create_table_mapping[create-table-mapping]
       create_table_mapping[create-table-mapping] --> create_catalogs_schemas[create-catalogs-schemas]
       create_uber_principal[create-uber-principal]
       principal_prefix_access[principal-prefix-access] --> migrate_credentials[migrate-credentials]
-      migrate_credentials --> migrate_locations[migrate-locations]
+      migrate_credentials --> validate-external-locations[validate-external-locations]
+      validate-external-locations --> migrate_locations[migrate-locations]
       migrate_locations --> create_catalogs_schemas
     end
     
     create_uber_principal --> workflow
     create_table_mapping --> workflow
     create_catalogs_schemas --> workflow
     
     subgraph workflow[Table Migration Workflows]
       subgraph mt_workflow[workflow: migrate-tables]
         dbfs_root_delta_mt_task[migrate_dbfs_root_delta_tables]
+        dbfs_root_non_delta_mt_task[migrate_dbfs_root_non_delta_tables]
         external_tables_sync_mt_task[migrate_external_tables_sync]
         view_mt_task[roadmap: migrate_views]
         dbfs_root_delta_mt_task --> view_mt_task
+        dbfs_root_non_delta_mt_task --> view_mt_task
         external_tables_sync_mt_task --> view_mt_task
       end
       
       subgraph mt_ctas_wf[roadmap workflow: migrate-tables-ctas]
         ctas_mt_task[migrate_tables_ctas] --> view_mt_task_ctas[roadmap: migrate_views]
+        ctas_mt_task[migrate_hiveserde_ctas] --> view_mt_task_ctas[roadmap: migrate_views]
       end
   
       subgraph mt_serde_inplace_wf[roadmap workflow: migrate-external-hiveserde-tables-in-place-experimental]
         serde_inplace_mt_task[migrate_external_hiveserde_tables_in_place_experimental] --> view_mt_task_inplace[roadmap: migrate_views]
       end
   
       subgraph mt_in_mounts_wf[roadmap workflow: migrate-tables-in-mounts-experimental]
@@ -408,45 +421,50 @@
     
     classDef roadmap stroke:Green,stroke-width:2px,color:Green,stroke-dasharray: 8 3
     class view_mt_task roadmap;
     class mt_ctas_wf,ctas_mt_task,view_mt_task_ctas roadmap;
     class mt_serde_inplace_wf,serde_inplace_mt_task,view_mt_task_inplace roadmap;
     class mt_in_mounts_wf,scan_tables_in_mounts_experimental_task,migrate_tables_in_mounts_experimental roadmap;
 ```
+
+After a UCX table migration is executed, the migration dashboard will be populated with migration status information.
 More details can be found in the [design of table migration](docs/table_upgrade.md)
 
 ### Dependency CLI commands
 - [`create-table-mapping`](#create-table-mapping-command) - Create `mapping.csv` which will be used by the workflow to identify the targets catalog, schema, table of the HMS table to be migrated. User should review and update the mapping file accordingly before proceeding with the migration workflow.
 - [`principal-prefix-access`](#principal-prefix-access-command) - Identify all the storages used in the workspace and corresponding Azure Service Principal or IAM role that are used in the workspace. It outputs `azure_storage_account_info.csv` or `uc_roles_access.csv` which will be later used by [`migrate-credentials`](#migrate-credentials-command) command to create UC storage credentials. The csv can be edited to control which IAM roles or Azure Service Principals should be used to create UC storage credentials later.
 - [`migrate-credentials`](#migrate-credentials-command) - Create UC storage credentials based on the Azure Service Principal or IAM role (`azure_storage_account_info.csv` or `uc_roles_access.csv`) identified by [`principal-prefix-access`](#principal-prefix-access-command) command.
 - [`migrate-locations`](#migrate-locations-command) - Create missing external locations in the Unity Catalog. 
 - [`create-catalogs-schemas`](#create-catalogs-schemas-command) - Create missing catalogs and schemas in the Unity Catalog. The candidate catalogs and schemas is based on `mapping.csv`
 - [`create-uber-principal`](#create-uber-principal-command) - Create an Uber Principal with access to all storages used in the workspace. This principal will be used by the workflow job cluster to migrate all the tables in the workspace.
+- [`migrate-tables`](#migrate-tables-command) - Kick off the tables migration workflows.
 
 [`create-table-mapping`](#create-table-mapping-command) and [`create-uber-principal`](#create-uber-principal-command) are required to run the workflow. While other commands are optional, as long as the UC storage credentials, external locations, catalogs and schemas needed for successful migration are created.
 
 To control the scope of the table migration, consider utilizing a combination of editing `mapping.csv`, employing [`skip`](#skip-command) command, and [`revert-migrated-tables`](#revert-migrated-tables-command) command.
 
 See more details in [Table migration commands](#table-migration-commands)
 
 ### Table Migration Workflow Tasks
-- `migrate_dbfs_root_delta_tables` - Migrate delta tables from the DBFS root using deep clone, along with legacy table ACL migrated if any.
-- `migrate_external_tables_sync` - Migrate external tables using [`SYNC`](https://docs.databricks.com/en/sql/language-manual/sql-ref-syntax-aux-sync.html) command, along with legacy table ACL migrated if any.
+There are 3 main table migration workflows, targeting different table types. All table migration workflows are designed to migrate legacy table ACLs if existed, as well as downstream views that depend on the migrated tables.
+- `migrate-tables` - Migrate DBFS root Delta tables & external tables using SYNC
+  - `migrate_dbfs_root_delta_tables` - Migrate Delta tables from the DBFS root using deep clone.
+  - `migrate_external_tables_sync` - Migrate external tables using [`SYNC`](https://docs.databricks.com/en/sql/language-manual/sql-ref-syntax-aux-sync.html) command. This does not create copy of the tables.
+- `migrate-external-hiveserde-tables-in-place-experimental` - Experimental in-place migration of HiveSerde tables. HiveSerDe tables include ParquetHiveSerDe, OrcSerde, AvroSerDe, LazySimpleSerDe, JsonSerDe, OpenCSVSerde tables.
+  - `migrate_external_hiveserde_tables_in_place_experimental` - Migrate HiveSerde tables in place.
 - Following workflows/tasks are on the roadmap and being developed:
-  - Migrate view
-  - Migrate tables using CTAS
-  - Optionally and experimentally in place migrate ParquetHiveSerDe, OrcSerde, AvroSerDe, LazySimpleSerDe, JsonSerDe, OpenCSVSerde tables.
+  - Migrate tables using CTAS 
   - Experimentally migrate Delta and Parquet data found in dbfs mount but not registered as Hive Metastore table into UC tables.
 
 ### Other considerations
 - You may need to run the workflow multiple times to ensure all the tables are migrated successfully in phases.
-- If your delta tables in DBFS root have large number of files, consider:
-  - Setting higher Min and Max workers for auto-scale when being asked during the UCX installation. More nodes/cores in the cluster means more concurrency for calling cloud storage api to copy files when deep cloning the delta tables.
-  - Setting higher "Parallelism for migrating dbfs root delta tables with deep clone" (default 200) when being asked during the UCX installation. This controls the number of Spark task/partition to be created for deep clone.
-- Consider create an instance pool, and set the instance pool id when being asked during the UCX installation. This instance pool will be put into the cluster policy used by all UCX workflows job clusters.
+- If your Delta tables in DBFS root have a large number of files, consider:
+  - Setting higher `Min` and `Max workers for auto-scale` when being asked during the UCX installation. More cores in the cluster means more concurrency for calling cloud storage API to copy files when deep cloning the Delta tables.
+  - Setting higher `Parallelism for migrating DBFS root Delta tables with deep clone` (default 200) when being asked during the UCX installation. This controls the number of Spark tasks/partitions to be created for deep clone.
+- Consider creating an instance pool, and setting its id when prompted during the UCX installation. This instance pool will be specified in the cluster policy used by all UCX workflows job clusters.
 - You may also manually edit the job cluster configration per job or per task after the workflows are deployed.
 
 [[back to top](#databricks-labs-ucx)]
 
 # Utility commands
 
 ## `logs` command
@@ -537,15 +555,14 @@
   * `default_catalog`: An optional string representing the default catalog name.
   * `log_level`: An optional string representing the log level.
   * `workspace_start_path`: A string representing the starting path for notebooks and directories crawler in the workspace.
   * `instance_profile`: An optional string representing the name of the instance profile.
   * `spark_conf`: An optional dictionary of Spark configuration properties.
   * `override_clusters`: An optional dictionary mapping job cluster names to existing cluster IDs.
   * `policy_id`: An optional string representing the ID of the cluster policy.
-  * `is_terraform_used`: A boolean value indicating whether some workspace resources are managed by Terraform.
   * `include_databases`: An optional list of strings representing the names of databases to include for migration.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `installations` command
 
 ```text
@@ -565,14 +582,38 @@
 This command displays the [installations](#installation) by different users on the same workspace. It fetches all 
 the installations where the `ucx` package is installed and prints their details in JSON format. This command is useful 
 for administrators who want to see which users have installed `ucx` and where. It can also be used to debug issues 
 related to multiple installations of `ucx` on the same workspace.
 
 [[back to top](#databricks-labs-ucx)]
 
+
+## `report-account-compatibility` command
+
+```text
+databricks labs ucx report-account-compatibility --profile labs-azure-account
+12:56:09  INFO [databricks.sdk] Using Azure CLI authentication with AAD tokens
+12:56:09  INFO [d.l.u.account.aggregate] Generating readiness report
+12:56:10  INFO [databricks.sdk] Using Azure CLI authentication with AAD tokens
+12:56:10  INFO [databricks.sdk] Using Azure CLI authentication with AAD tokens
+12:56:15  INFO [databricks.sdk] Using Azure CLI authentication with AAD tokens
+12:56:15  INFO [d.l.u.account.aggregate] Querying Schema ucx
+12:56:21  WARN [d.l.u.account.aggregate] Workspace 4045495039142306 does not have UCX installed
+12:56:21  INFO [d.l.u.account.aggregate] UC compatibility: 30.303030303030297% (69/99)
+12:56:21  INFO [d.l.u.account.aggregate] cluster type not supported : LEGACY_TABLE_ACL: 22 objects
+12:56:21  INFO [d.l.u.account.aggregate] cluster type not supported : LEGACY_SINGLE_USER: 24 objects
+12:56:21  INFO [d.l.u.account.aggregate] unsupported config: spark.hadoop.javax.jdo.option.ConnectionURL: 10 objects
+12:56:21  INFO [d.l.u.account.aggregate] Uses azure service principal credentials config in cluster.: 1 objects
+12:56:21  INFO [d.l.u.account.aggregate] No isolation shared clusters not supported in UC: 1 objects
+12:56:21  INFO [d.l.u.account.aggregate] Data is in DBFS Root: 23 objects
+12:56:21  INFO [d.l.u.account.aggregate] Non-DELTA format: UNKNOWN: 5 objects
+```
+
+[[back to top](#databricks-labs-ucx)]
+
 # Metastore related commands
 
 These commands are used to assign a Unity Catalog metastore to a workspace. The metastore assignment is a pre-requisite
 for any further migration steps.
 
 [[back to top](#databricks-labs-ucx)]
 
@@ -580,15 +621,15 @@
 
 ```text
 databricks labs ucx show-all-metastores [--workspace-id <workspace-id>]
 ```
 
 This command lists all the metastores available to be assigned to a workspace. If no workspace is specified, it lists
 all the metastores available in the account. This command is useful when there are multiple metastores available within
-a region and you want to see which ones are available for assignment.
+a region, and you want to see which ones are available for assignment.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `assign-metastore` command
 
 ```text
 databricks labs ucx assign-metastore --workspace-id <workspace-id> [--metastore-id <metastore-id>]
@@ -616,15 +657,15 @@
 the [`validate-external-locations` command](#validate-external-locations-command).
 You'll need to create the [uber principal](#create-uber-principal-command) with the _**access to all storage**_ used to tables in 
 the workspace, so that you can migrate all the tables. If you already have the principal, you can skip this step.
 
 Ask your Databricks Account admin to run the [`sync-workspace-info` command](#sync-workspace-info-command) to sync the
 workspace information with the UCX installations. Once the workspace information is synced, you can run the 
 [`create-table-mapping` command](#create-table-mapping-command) to align your tables with the Unity Catalog,
-[create catalogs and schemas](#create-catalogs-schemas-command) and start the migration. During multiple runs of
+[create catalogs and schemas](#create-catalogs-schemas-command) and start the migration using [`migrate-tables` command](#migrate-tables-command). During multiple runs of
 the table migration workflow, you can use the [`revert-migrated-tables` command](#revert-migrated-tables-command) to 
 revert the tables that were migrated in the previous run. You can also skip the tables that you don't want to migrate 
 using the [`skip` command](#skip-command).
 
 Once you're done with the table migration, proceed to the [code migration](#code-migration-commands).
 
 [[back to top](#databricks-labs-ucx)]
@@ -659,49 +700,63 @@
 ### Access for Azure Storage Accounts
 
 ```commandline
 databricks labs ucx principal-prefix-access --subscription-id test-subscription-id
 ```
 
 Use to identify all storage account used by tables, identify the relevant Azure service principals and their permissions 
-on each storage account. This requires Azure CLI to be installed and configured via `az login`. 
+on each storage account. The command is used to identify Azure Service Principals, which have `Storage Blob Data Contributor`,
+`Storage Blob Data Reader`, `Storage Blob Data Owner` roles, or custom read/write roles on ADLS Gen2 locations that are being 
+used in Databricks. This requires Azure CLI to be installed and configured via `az login`. It outputs azure_storage_account_info.csv
+which will be later used by migrate-credentials command to create UC storage credentials.
 
 Once done, proceed to the [`migrate-credentials` command](#migrate-credentials-command).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `create-uber-principal` command
 
 ```text
 databricks labs ucx create-uber-principal [--subscription-id X]
 ```
 
-**Requires Cloud IAM admin privileges.** Once the [`assessment` workflow](#assessment-workflow) complete, you should run 
-this command to creates a service principal with the _**read-only access to all storage**_ used by tables in this 
-workspace and configure the [UCX Cluster Policy](#installation) with the details of it. Once migration is complete, this
-service principal should be unprovisioned. On Azure, it creates a principal with `Storage Blob Data Reader` role 
-assignment on every storage account using Azure Resource Manager APIs.
+**Requires Cloud IAM admin privileges.** 
+
+Once the [`assessment` workflow](#assessment-workflow) complete, you should run this command to create a service principal with the 
+_**read-only access to all storage**_ used by tables in this workspace. It will also configure the 
+[UCX Cluster Policy](#installation) & SQL Warehouse data access configuration to use this service principal for migration 
+workflows. Once migration is complete, this service principal should be unprovisioned. 
+
+On Azure, it creates a principal with `Storage Blob Data Contributor` role assignment on every storage account using 
+Azure Resource Manager APIs.
 
 This command is one of prerequisites for the [table migration workflow](#table-migration-workflow).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `migrate-credentials` command
 
 ```commandline
 databricks labs ucx migrate-credentials
 ```
 
-For Azure, this command migrate Azure Service Principals, which have `Storage Blob Data Contributor`,
-`Storage Blob Data Reader`, `Storage Blob Data Owner` roles on ADLS Gen2 locations that are being used in
-Databricks, to UC storage credentials. The Azure Service Principals to location mapping are listed 
-in `/Users/{user_name}/.ucx/azure_storage_account_info.csv` which is generated 
-by [`principal-prefix-access` command](#principal-prefix-access-command). 
-Please review the file and delete the Service Principals you do not want to be migrated.
-The command will only migrate the Service Principals that have client secret stored in Databricks Secret.
+For Azure, this command prompts to confirm performing the following credential migration steps:
+1. [RECOMMENDED] For each storage account, create access connectors with managed identities that have the
+   `Storage Blob Data Contributor` role on the respective storage account. A storage credential is created for each 
+    access connector.
+2. Migrate Azure Service Principals, which have `Storage Blob Data Contributor`,
+   `Storage Blob Data Reader`, `Storage Blob Data Owner`, or custom roles on ADLS Gen2 locations that are being used in
+   Databricks, to UC storage credentials. The Azure Service Principals to location mapping are listed
+   in `/Users/{user_name}/.ucx/azure_storage_account_info.csv` which is generated by
+   [`principal-prefix-access` command](#principal-prefix-access-command). Please review the file and delete the Service
+   Principals you do not want to be migrated. The command will only migrate the Service Principals that have client
+   secret stored in Databricks Secret.
+
+  **Warning**: Service principals used to access storage accounts behind firewalls might cause connectivity issues. We
+  recommend to use access connectors instead.
 
 Once you're done with this command, run [`validate-external-locations` command](#validate-external-locations-command) after this one.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `validate-external-locations` command
 
@@ -763,48 +818,61 @@
 
 ## `skip` command
 
 ```text
 databricks labs ucx skip --schema X [--table Y]  
 ```
 
-Anywhere after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
+Anytime after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
 
 This command allows users to skip certain schemas or tables during the [table migration](#table-migration-workflow) process.
 The command takes `--schema` and optionally `--table` flags to specify the schema and table to skip. If no `--table` flag 
 is provided, all tables in the specified HMS database are skipped.
-This command is useful to temporarily disable migration on a particular schema or table.
+This command is useful to temporarily disable migration of a particular schema or table.
 
 Once you're done with table migration, proceed to the [code migration](#code-migration-commands).
 
 [[back to top](#databricks-labs-ucx)]
 
-## `revert-migrated-tables` command
+## `create-catalogs-schemas` command
 
 ```text
-databricks labs ucx revert-migrated-tables --schema X --table Y [--delete-managed]  
+databricks labs ucx create-catalogs-schemas
 ```
+After [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command to have the required UC catalogs and schemas created.
+This command is supposed to be run before migrating tables to UC using [table migration workflow](#table-migration-workflow).
+
+[[back to top](#databricks-labs-ucx)]
 
-Anywhere after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
+## `migrate-tables` command
 
-This command removes the `upgraded_from` property on a migrated table for re-migration in the [table migration](#table-migration-workflow) process. 
-This command is useful for developers and administrators who want to revert the migration of a table. It can also be used 
-to debug issues related to table migration.
+```text
+databricks labs ucx migrate-tables
+```
 
-Go back to the [`create-table-mapping` command](#create-table-mapping-command) after you're done with this command.
+Anytime after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
+
+This command kicks off the [table migration](#table-migration-workflow) process. It triggers the `migrate-tables` workflow, 
+and if there are HiveSerDe tables detected, prompt whether to trigger the `migrate-external-hiveserde-tables-in-place-experimental` workflow.
 
 [[back to top](#databricks-labs-ucx)]
 
-## `create-catalogs-schemas` command
+## `revert-migrated-tables` command
 
 ```text
-databricks labs ucx create-catalogs-schemas
+databricks labs ucx revert-migrated-tables --schema X --table Y [--delete-managed]  
 ```
-After [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command to have the required UC catalogs and schemas created.
-This command is supposed to be run before migrating tables to UC using [table migration workflow](#table-migration-workflow).
+
+Anytime after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
+
+This command removes the `upgraded_from` property on a migrated table for re-migration in the [table migration](#table-migration-workflow) process. 
+This command is useful for developers and administrators who want to revert the migration of a table. It can also be used 
+to debug issues related to table migration.
+
+Go back to the [`create-table-mapping` command](#create-table-mapping-command) after you're done with this command.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `move` command
 
 ```text
 databricks labs ucx move --from-catalog A --from-schema B --from-table C --to-catalog D --to-schema E  
@@ -859,14 +927,46 @@
 **(Experimental)** Once [table migration](#table-migration-workflow) is complete, you can run this command to 
 migrate all python and SQL files in the current working directory. This command is highly experimental and
 at the moment only supports Python and SQL files and discards code comments and formatting during 
 the automated transformation process.
 
 [[back to top](#databricks-labs-ucx)]
 
+## `migrate-dbsql-dashboards` command
+
+```text
+databricks labs ucx migrate-dbsql-dashboards [--dashboard-id <dashboard-id>]
+```
+
+**(Experimental)** Once [table migration](#table-migration-workflow) is complete, you can run this command to 
+migrate all Databricks SQL dashboards in the workspace. At this moment, this command is highly experimental and discards
+formatting during the automated transformation process.
+
+This command tags dashboards & queries that have been migrated with `migrated by UCX` tag. The original queries are
+also backed up in the ucx installation folder, to allow for easy rollback (see [`revert-dbsql-dashboards` command](#revert-dbsql-dashboards-command)).
+
+This command can be run with `--dashboard-id` flag to migrate a specific dashboard.
+
+This command is incremental and can be run multiple times to migrate new dashboards.
+
+[[back to top](#databricks-labs-ucx)]
+
+## `revert-dbsql-dashboards` command
+
+```text
+databricks labs ucx revert-dbsql-dashboards [--dashboard-id <dashboard-id>]
+```
+
+**(Experimental)** This command reverts the migration of Databricks SQL dashboards in the workspace, after
+`migrate-dbsql-dashboards` command is executed.
+
+This command can be run with `--dashboard-id` flag to migrate a specific dashboard.
+
+[[back to top](#databricks-labs-ucx)]
+
 # Cross-workspace installations
 
 When installing UCX across multiple workspaces, administrators need to keep UCX configurations in sync.
 UCX will prompt you to select an account profile that has been defined in `~/.databrickscfg`. If you don't have one,
 authenticate your machine with:
 
 * `databricks auth login --host https://accounts.cloud.databricks.com/` (AWS)
@@ -999,15 +1099,15 @@
 21:31:29  INFO [d.labs.ucx] Reverting the Remapping of the Clusters from UC
 21:31:33  INFO [d.labs.ucx] 0301-055912-4ske39iq
 21:31:33  INFO [d.labs.ucx] 0306-121015-v1llqff6
 Please provide the cluster id's as comma separated value from the above list (default: <ALL>):
 ```
 
 If a customer want's to revert the cluster remap done using the [`cluster-remap` command](#cluster-remap-command) they can use this command to revert 
-its configuration from UC to original one.It will iterate through the list of clusters from the back up folder and reverts the 
+its configuration from UC to original one.It will iterate through the list of clusters from the backup folder and reverts the 
 cluster configurations to original one.This will also ask the user to provide the list of clusters that has to be reverted as a prompt.
 By default, it will revert all the clusters present in the backup folder
 
 [[back to top](#databricks-labs-ucx)]
 
 # Star History
```

### Comparing `databricks_labs_ucx-0.22.0/pyproject.toml` & `databricks_labs_ucx-0.23.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,19 @@
     "Intended Audience :: System Administrators",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 
-dependencies = ["databricks-sdk~=0.26.0",
+dependencies = ["databricks-sdk~=0.27.0",
                 "databricks-labs-lsql~=0.4.0",
                 "databricks-labs-blueprint~=0.4.3",
                 "PyYAML>=6.0.0,<7.0.0",
-                "sqlglot>=23.9,<23.12"]
+                "sqlglot>=23.9,<23.15"]
 
 [project.entry-points.databricks]
 runtime = "databricks.labs.ucx.runtime:main"
 
 [project.urls]
 Issues = "https://github.com/databricks/ucx/issues"
 Source = "https://github.com/databricks/ucx"
@@ -85,19 +85,19 @@
 
 [tool.hatch.envs.default.scripts]
 test        = "pytest -n 4 --cov src --cov-report=xml --timeout 30 tests/unit --durations 20"
 coverage    = "pytest -n auto --cov src tests/unit --timeout 30 --cov-report=html --durations 20"
 integration = "pytest -n 10 --cov src tests/integration --durations 20"
 fmt         = ["black .",
                "ruff check . --fix",
-               "mypy --disable-error-code 'annotation-unchecked' .",
+               "mypy --disable-error-code 'annotation-unchecked' --exclude 'tests/unit/source_code/samples/*' .",
                "pylint --output-format=colorized -j 0 src tests"]
 verify      = ["black --check .",
                "ruff .",
-               "mypy .",
+               "mypy --exclude 'tests/unit/source_code/samples/*' .",
                "pylint --output-format=colorized -j 0 src tests"]
 lint         = ["pylint --output-format=colorized -j 0 src tests"]
 
 [tool.pytest.ini_options]
 # TODO: remove `-p no:warnings`
 addopts = "--no-header -p no:warnings"
 cache_dir = ".venv/pytest-cache"
@@ -107,14 +107,15 @@
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
 cache-dir = ".venv/ruff-cache"
 target-version = "py310"
 line-length = 120
+exclude = ["tests/unit/source_code/samples/*"]
 
 [tool.ruff.lint]
 ignore = [
     # Allow boolean positional values in function calls, like `dict.get(... True)`
     "FBT003",
     # Ignore checks for possible passwords and SQL statement construction
     "S105", "S106", "S107", "S603", "S608",
```

### Comparing `databricks_labs_ucx-0.22.0/PKG-INFO` & `databricks_labs_ucx-0.23.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-ucx
-Version: 0.22.0
+Version: 0.23.0
 Summary: UCX - Unity Catalog Migration Toolkit
 Project-URL: Issues, https://github.com/databricks/ucx/issues
 Project-URL: Source, https://github.com/databricks/ucx
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 Maintainer-email: Serge Smertin <serge.smertin@databricks.com>, Liran Bareket <liran.bareket@databricks.com>, Marcin Wojtyczka <marcin.wojtyczka@databricks.com>, Ziyuan Qin <ziyuan.qin@databricks.com>, William Conti <william.conti@databricks.com>, Hari Selvarajan <hari.selvarajan@databricks.com>, Vuong Nguyen <vuong.nguyen@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
@@ -23,34 +23,39 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Requires-Dist: databricks-labs-blueprint~=0.4.3
 Requires-Dist: databricks-labs-lsql~=0.4.0
-Requires-Dist: databricks-sdk~=0.26.0
+Requires-Dist: databricks-sdk~=0.27.0
 Requires-Dist: pyyaml<7.0.0,>=6.0.0
-Requires-Dist: sqlglot<23.12,>=23.9
+Requires-Dist: sqlglot<23.15,>=23.9
 Description-Content-Type: text/markdown
 
 Databricks Labs UCX
 ===
 ![UCX by Databricks Labs](docs/logo-no-background.png)
 
-The companion for upgrading to Unity Catalog. After [installation](#install-ucx), ensure to [trigger](#ensure-assessment-run-command) the [assessment workflow](#assessment-workflow), 
-so that you'll be able to [scope the migration](docs/assessment.md) and execute the [group migration workflow](#group-migration-workflow). 
-[`<installation_path>/README`](#readme-notebook) contains further instructions and explanations of these workflows. 
-Then you can execute [table migration workflow](#table-migration-workflow).
-More workflows, like notebook code migration is coming in the future releases. 
-UCX exposes a number of command line utilities accessible via `databricks labs ucx`.
+The companion for upgrading to Unity Catalog. 
+
+After [installation](#install-ucx), ensure to [trigger](#ensure-assessment-run-command) the [assessment workflow](#assessment-workflow), 
+so that you'll be able to [scope the migration](docs/assessment.md) and execute the [group migration workflow](#group-migration-workflow).
+
+The [README notebook](#readme-notebook), which can be found in the installation folder contains further instructions and explanations of the different ucx workflows & dashboards. 
+Once the migration is scoped, you can start executing the [table migration workflow](#table-migration-workflow).
+
+More workflows, like notebook code migration are coming in future releases.
+
+UCX also provides a number of command line utilities accessible via `databricks labs ucx`.
 
 For questions, troubleshooting or bug fixes, please see our [troubleshooting guide](docs/troubleshooting.md) or submit [an issue](https://github.com/databrickslabs/ucx/issues). 
 See [contributing instructions](CONTRIBUTING.md) to help improve this project.
 
-[![build](https://github.com/databrickslabs/ucx/actions/workflows/push.yml/badge.svg)](https://github.com/databrickslabs/ucx/actions/workflows/push.yml) [![codecov](https://codecov.io/github/databrickslabs/ucx/graph/badge.svg?token=p0WKAfW5HQ)](https://codecov.io/github/databrickslabs/ucx)  [![lines of code](https://tokei.rs/b1/github/databrickslabs/ucx)]([https://codecov.io/github/databrickslabs/ucx](https://github.com/databrickslabs/ucx))
+[![build](https://github.com/databrickslabs/ucx/actions/workflows/push.yml/badge.svg)](https://github.com/databrickslabs/ucx/actions/workflows/push.yml) [![codecov](https://codecov.io/github/databrickslabs/ucx/graph/badge.svg?token=p0WKAfW5HQ)](https://codecov.io/github/databrickslabs/ucx)  ![linesofcode](https://aschey.tech/tokei/github/databrickslabs/ucx?category=code)
 
 <!-- TOC -->
 * [Databricks Labs UCX](#databricks-labs-ucx)
 * [Installation](#installation)
   * [Authenticate Databricks CLI](#authenticate-databricks-cli)
   * [Install UCX](#install-ucx)
   * [[ADVANCED] Force install over existing UCX](#advanced-force-install-over-existing-ucx)
@@ -71,33 +76,37 @@
 * [Utility commands](#utility-commands)
   * [`logs` command](#logs-command)
   * [`ensure-assessment-run` command](#ensure-assessment-run-command)
   * [`repair-run` command](#repair-run-command)
   * [`workflows` command](#workflows-command)
   * [`open-remote-config` command](#open-remote-config-command)
   * [`installations` command](#installations-command)
+  * [`report-account-compatibility` command](#report-account-compatibility-command)
 * [Metastore related commands](#metastore-related-commands)
   * [`show-all-metastores` command](#show-all-metastores-command)
   * [`assign-metastore` command](#assign-metastore-command)
 * [Table migration commands](#table-migration-commands)
   * [`principal-prefix-access` command](#principal-prefix-access-command)
     * [Access for AWS S3 Buckets](#access-for-aws-s3-buckets)
     * [Access for Azure Storage Accounts](#access-for-azure-storage-accounts)
   * [`create-uber-principal` command](#create-uber-principal-command)
   * [`migrate-credentials` command](#migrate-credentials-command)
   * [`validate-external-locations` command](#validate-external-locations-command)
   * [`migrate-locations` command](#migrate-locations-command)
   * [`create-table-mapping` command](#create-table-mapping-command)
   * [`skip` command](#skip-command)
-  * [`revert-migrated-tables` command](#revert-migrated-tables-command)
   * [`create-catalogs-schemas` command](#create-catalogs-schemas-command)
+  * [`migrate-tables` command](#migrate-tables-command)
+  * [`revert-migrated-tables` command](#revert-migrated-tables-command)
   * [`move` command](#move-command)
   * [`alias` command](#alias-command)
 * [Code migration commands](#code-migration-commands)
   * [`migrate-local-code` command](#migrate-local-code-command)
+  * [`migrate-dbsql-dashboards` command](#migrate-dbsql-dashboards-command)
+  * [`revert-dbsql-dashboards` command](#revert-dbsql-dashboards-command)
 * [Cross-workspace installations](#cross-workspace-installations)
   * [`sync-workspace-info` command](#sync-workspace-info-command)
   * [`manual-workspace-info` command](#manual-workspace-info-command)
   * [`create-account-groups` command](#create-account-groups-command)
   * [`validate-groups-membership` command](#validate-groups-membership-command)
   * [`cluster-remap` command](#cluster-remap-command)
   * [`revert-cluster-remap` command](#revert-cluster-remap-command)
@@ -111,15 +120,15 @@
 - Python 3.10 or later. See [Windows](https://www.python.org/downloads/windows/) instructions.
 - Network access to your Databricks Workspace used for the [installation process](#install-ucx).
 - Network access to the Internet for [pypi.org](https://pypi.org) and [github.com](https://github.com) from machine running the installation.
 - Databricks Workspace Administrator privileges for the user, that runs the installation. Running UCX as a Service Principal is not supported.
 - Account level Identity Setup. See instructions for [AWS](https://docs.databricks.com/en/administration-guide/users-groups/best-practices.html), [Azure](https://learn.microsoft.com/en-us/azure/databricks/administration-guide/users-groups/best-practices), and [GCP](https://docs.gcp.databricks.com/administration-guide/users-groups/best-practices.html).
 - Unity Catalog Metastore Created (per region). See instructions for [AWS](https://docs.databricks.com/en/data-governance/unity-catalog/create-metastore.html), [Azure](https://learn.microsoft.com/en-us/azure/databricks/data-governance/unity-catalog/create-metastore), and [GCP](https://docs.gcp.databricks.com/data-governance/unity-catalog/create-metastore.html).
 - If your Databricks Workspace relies on an external Hive Metastore (such as AWS Glue), make sure to read [this guide](docs/external_hms_glue.md).
-- Databricks Workspace has to have network access to [pypi.org](https://pypi.org) to download `databricks-sdk` and `pyyaml` packages.
+- Databricks Workspace has to have network access to [pypi.org](https://pypi.org) to download `databricks-sdk`, `databricks-labs-lsql`, `databricks-labs-blueprint`, `sqlglot` and `pyyaml` packages.
 - A PRO or Serverless SQL Warehouse to render the [report](docs/assessment.md) for the [assessment workflow](#assessment-workflow).
 
 Once you [install UCX](#install-ucx), you can proceed to the [assessment workflow](#assessment-workflow) to ensure 
 the compatibility of your workspace with Unity Catalog.
 
 [[back to top](#databricks-labs-ucx)]
 
@@ -405,33 +414,37 @@
 ```mermaid
 flowchart TB
     subgraph CLI
       sync-workspace-info[sync-workspace-info] --> create_table_mapping[create-table-mapping]
       create_table_mapping[create-table-mapping] --> create_catalogs_schemas[create-catalogs-schemas]
       create_uber_principal[create-uber-principal]
       principal_prefix_access[principal-prefix-access] --> migrate_credentials[migrate-credentials]
-      migrate_credentials --> migrate_locations[migrate-locations]
+      migrate_credentials --> validate-external-locations[validate-external-locations]
+      validate-external-locations --> migrate_locations[migrate-locations]
       migrate_locations --> create_catalogs_schemas
     end
     
     create_uber_principal --> workflow
     create_table_mapping --> workflow
     create_catalogs_schemas --> workflow
     
     subgraph workflow[Table Migration Workflows]
       subgraph mt_workflow[workflow: migrate-tables]
         dbfs_root_delta_mt_task[migrate_dbfs_root_delta_tables]
+        dbfs_root_non_delta_mt_task[migrate_dbfs_root_non_delta_tables]
         external_tables_sync_mt_task[migrate_external_tables_sync]
         view_mt_task[roadmap: migrate_views]
         dbfs_root_delta_mt_task --> view_mt_task
+        dbfs_root_non_delta_mt_task --> view_mt_task
         external_tables_sync_mt_task --> view_mt_task
       end
       
       subgraph mt_ctas_wf[roadmap workflow: migrate-tables-ctas]
         ctas_mt_task[migrate_tables_ctas] --> view_mt_task_ctas[roadmap: migrate_views]
+        ctas_mt_task[migrate_hiveserde_ctas] --> view_mt_task_ctas[roadmap: migrate_views]
       end
   
       subgraph mt_serde_inplace_wf[roadmap workflow: migrate-external-hiveserde-tables-in-place-experimental]
         serde_inplace_mt_task[migrate_external_hiveserde_tables_in_place_experimental] --> view_mt_task_inplace[roadmap: migrate_views]
       end
   
       subgraph mt_in_mounts_wf[roadmap workflow: migrate-tables-in-mounts-experimental]
@@ -442,45 +455,50 @@
     
     classDef roadmap stroke:Green,stroke-width:2px,color:Green,stroke-dasharray: 8 3
     class view_mt_task roadmap;
     class mt_ctas_wf,ctas_mt_task,view_mt_task_ctas roadmap;
     class mt_serde_inplace_wf,serde_inplace_mt_task,view_mt_task_inplace roadmap;
     class mt_in_mounts_wf,scan_tables_in_mounts_experimental_task,migrate_tables_in_mounts_experimental roadmap;
 ```
+
+After a UCX table migration is executed, the migration dashboard will be populated with migration status information.
 More details can be found in the [design of table migration](docs/table_upgrade.md)
 
 ### Dependency CLI commands
 - [`create-table-mapping`](#create-table-mapping-command) - Create `mapping.csv` which will be used by the workflow to identify the targets catalog, schema, table of the HMS table to be migrated. User should review and update the mapping file accordingly before proceeding with the migration workflow.
 - [`principal-prefix-access`](#principal-prefix-access-command) - Identify all the storages used in the workspace and corresponding Azure Service Principal or IAM role that are used in the workspace. It outputs `azure_storage_account_info.csv` or `uc_roles_access.csv` which will be later used by [`migrate-credentials`](#migrate-credentials-command) command to create UC storage credentials. The csv can be edited to control which IAM roles or Azure Service Principals should be used to create UC storage credentials later.
 - [`migrate-credentials`](#migrate-credentials-command) - Create UC storage credentials based on the Azure Service Principal or IAM role (`azure_storage_account_info.csv` or `uc_roles_access.csv`) identified by [`principal-prefix-access`](#principal-prefix-access-command) command.
 - [`migrate-locations`](#migrate-locations-command) - Create missing external locations in the Unity Catalog. 
 - [`create-catalogs-schemas`](#create-catalogs-schemas-command) - Create missing catalogs and schemas in the Unity Catalog. The candidate catalogs and schemas is based on `mapping.csv`
 - [`create-uber-principal`](#create-uber-principal-command) - Create an Uber Principal with access to all storages used in the workspace. This principal will be used by the workflow job cluster to migrate all the tables in the workspace.
+- [`migrate-tables`](#migrate-tables-command) - Kick off the tables migration workflows.
 
 [`create-table-mapping`](#create-table-mapping-command) and [`create-uber-principal`](#create-uber-principal-command) are required to run the workflow. While other commands are optional, as long as the UC storage credentials, external locations, catalogs and schemas needed for successful migration are created.
 
 To control the scope of the table migration, consider utilizing a combination of editing `mapping.csv`, employing [`skip`](#skip-command) command, and [`revert-migrated-tables`](#revert-migrated-tables-command) command.
 
 See more details in [Table migration commands](#table-migration-commands)
 
 ### Table Migration Workflow Tasks
-- `migrate_dbfs_root_delta_tables` - Migrate delta tables from the DBFS root using deep clone, along with legacy table ACL migrated if any.
-- `migrate_external_tables_sync` - Migrate external tables using [`SYNC`](https://docs.databricks.com/en/sql/language-manual/sql-ref-syntax-aux-sync.html) command, along with legacy table ACL migrated if any.
+There are 3 main table migration workflows, targeting different table types. All table migration workflows are designed to migrate legacy table ACLs if existed, as well as downstream views that depend on the migrated tables.
+- `migrate-tables` - Migrate DBFS root Delta tables & external tables using SYNC
+  - `migrate_dbfs_root_delta_tables` - Migrate Delta tables from the DBFS root using deep clone.
+  - `migrate_external_tables_sync` - Migrate external tables using [`SYNC`](https://docs.databricks.com/en/sql/language-manual/sql-ref-syntax-aux-sync.html) command. This does not create copy of the tables.
+- `migrate-external-hiveserde-tables-in-place-experimental` - Experimental in-place migration of HiveSerde tables. HiveSerDe tables include ParquetHiveSerDe, OrcSerde, AvroSerDe, LazySimpleSerDe, JsonSerDe, OpenCSVSerde tables.
+  - `migrate_external_hiveserde_tables_in_place_experimental` - Migrate HiveSerde tables in place.
 - Following workflows/tasks are on the roadmap and being developed:
-  - Migrate view
-  - Migrate tables using CTAS
-  - Optionally and experimentally in place migrate ParquetHiveSerDe, OrcSerde, AvroSerDe, LazySimpleSerDe, JsonSerDe, OpenCSVSerde tables.
+  - Migrate tables using CTAS 
   - Experimentally migrate Delta and Parquet data found in dbfs mount but not registered as Hive Metastore table into UC tables.
 
 ### Other considerations
 - You may need to run the workflow multiple times to ensure all the tables are migrated successfully in phases.
-- If your delta tables in DBFS root have large number of files, consider:
-  - Setting higher Min and Max workers for auto-scale when being asked during the UCX installation. More nodes/cores in the cluster means more concurrency for calling cloud storage api to copy files when deep cloning the delta tables.
-  - Setting higher "Parallelism for migrating dbfs root delta tables with deep clone" (default 200) when being asked during the UCX installation. This controls the number of Spark task/partition to be created for deep clone.
-- Consider create an instance pool, and set the instance pool id when being asked during the UCX installation. This instance pool will be put into the cluster policy used by all UCX workflows job clusters.
+- If your Delta tables in DBFS root have a large number of files, consider:
+  - Setting higher `Min` and `Max workers for auto-scale` when being asked during the UCX installation. More cores in the cluster means more concurrency for calling cloud storage API to copy files when deep cloning the Delta tables.
+  - Setting higher `Parallelism for migrating DBFS root Delta tables with deep clone` (default 200) when being asked during the UCX installation. This controls the number of Spark tasks/partitions to be created for deep clone.
+- Consider creating an instance pool, and setting its id when prompted during the UCX installation. This instance pool will be specified in the cluster policy used by all UCX workflows job clusters.
 - You may also manually edit the job cluster configration per job or per task after the workflows are deployed.
 
 [[back to top](#databricks-labs-ucx)]
 
 # Utility commands
 
 ## `logs` command
@@ -571,15 +589,14 @@
   * `default_catalog`: An optional string representing the default catalog name.
   * `log_level`: An optional string representing the log level.
   * `workspace_start_path`: A string representing the starting path for notebooks and directories crawler in the workspace.
   * `instance_profile`: An optional string representing the name of the instance profile.
   * `spark_conf`: An optional dictionary of Spark configuration properties.
   * `override_clusters`: An optional dictionary mapping job cluster names to existing cluster IDs.
   * `policy_id`: An optional string representing the ID of the cluster policy.
-  * `is_terraform_used`: A boolean value indicating whether some workspace resources are managed by Terraform.
   * `include_databases`: An optional list of strings representing the names of databases to include for migration.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `installations` command
 
 ```text
@@ -599,14 +616,38 @@
 This command displays the [installations](#installation) by different users on the same workspace. It fetches all 
 the installations where the `ucx` package is installed and prints their details in JSON format. This command is useful 
 for administrators who want to see which users have installed `ucx` and where. It can also be used to debug issues 
 related to multiple installations of `ucx` on the same workspace.
 
 [[back to top](#databricks-labs-ucx)]
 
+
+## `report-account-compatibility` command
+
+```text
+databricks labs ucx report-account-compatibility --profile labs-azure-account
+12:56:09  INFO [databricks.sdk] Using Azure CLI authentication with AAD tokens
+12:56:09  INFO [d.l.u.account.aggregate] Generating readiness report
+12:56:10  INFO [databricks.sdk] Using Azure CLI authentication with AAD tokens
+12:56:10  INFO [databricks.sdk] Using Azure CLI authentication with AAD tokens
+12:56:15  INFO [databricks.sdk] Using Azure CLI authentication with AAD tokens
+12:56:15  INFO [d.l.u.account.aggregate] Querying Schema ucx
+12:56:21  WARN [d.l.u.account.aggregate] Workspace 4045495039142306 does not have UCX installed
+12:56:21  INFO [d.l.u.account.aggregate] UC compatibility: 30.303030303030297% (69/99)
+12:56:21  INFO [d.l.u.account.aggregate] cluster type not supported : LEGACY_TABLE_ACL: 22 objects
+12:56:21  INFO [d.l.u.account.aggregate] cluster type not supported : LEGACY_SINGLE_USER: 24 objects
+12:56:21  INFO [d.l.u.account.aggregate] unsupported config: spark.hadoop.javax.jdo.option.ConnectionURL: 10 objects
+12:56:21  INFO [d.l.u.account.aggregate] Uses azure service principal credentials config in cluster.: 1 objects
+12:56:21  INFO [d.l.u.account.aggregate] No isolation shared clusters not supported in UC: 1 objects
+12:56:21  INFO [d.l.u.account.aggregate] Data is in DBFS Root: 23 objects
+12:56:21  INFO [d.l.u.account.aggregate] Non-DELTA format: UNKNOWN: 5 objects
+```
+
+[[back to top](#databricks-labs-ucx)]
+
 # Metastore related commands
 
 These commands are used to assign a Unity Catalog metastore to a workspace. The metastore assignment is a pre-requisite
 for any further migration steps.
 
 [[back to top](#databricks-labs-ucx)]
 
@@ -614,15 +655,15 @@
 
 ```text
 databricks labs ucx show-all-metastores [--workspace-id <workspace-id>]
 ```
 
 This command lists all the metastores available to be assigned to a workspace. If no workspace is specified, it lists
 all the metastores available in the account. This command is useful when there are multiple metastores available within
-a region and you want to see which ones are available for assignment.
+a region, and you want to see which ones are available for assignment.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `assign-metastore` command
 
 ```text
 databricks labs ucx assign-metastore --workspace-id <workspace-id> [--metastore-id <metastore-id>]
@@ -650,15 +691,15 @@
 the [`validate-external-locations` command](#validate-external-locations-command).
 You'll need to create the [uber principal](#create-uber-principal-command) with the _**access to all storage**_ used to tables in 
 the workspace, so that you can migrate all the tables. If you already have the principal, you can skip this step.
 
 Ask your Databricks Account admin to run the [`sync-workspace-info` command](#sync-workspace-info-command) to sync the
 workspace information with the UCX installations. Once the workspace information is synced, you can run the 
 [`create-table-mapping` command](#create-table-mapping-command) to align your tables with the Unity Catalog,
-[create catalogs and schemas](#create-catalogs-schemas-command) and start the migration. During multiple runs of
+[create catalogs and schemas](#create-catalogs-schemas-command) and start the migration using [`migrate-tables` command](#migrate-tables-command). During multiple runs of
 the table migration workflow, you can use the [`revert-migrated-tables` command](#revert-migrated-tables-command) to 
 revert the tables that were migrated in the previous run. You can also skip the tables that you don't want to migrate 
 using the [`skip` command](#skip-command).
 
 Once you're done with the table migration, proceed to the [code migration](#code-migration-commands).
 
 [[back to top](#databricks-labs-ucx)]
@@ -693,49 +734,63 @@
 ### Access for Azure Storage Accounts
 
 ```commandline
 databricks labs ucx principal-prefix-access --subscription-id test-subscription-id
 ```
 
 Use to identify all storage account used by tables, identify the relevant Azure service principals and their permissions 
-on each storage account. This requires Azure CLI to be installed and configured via `az login`. 
+on each storage account. The command is used to identify Azure Service Principals, which have `Storage Blob Data Contributor`,
+`Storage Blob Data Reader`, `Storage Blob Data Owner` roles, or custom read/write roles on ADLS Gen2 locations that are being 
+used in Databricks. This requires Azure CLI to be installed and configured via `az login`. It outputs azure_storage_account_info.csv
+which will be later used by migrate-credentials command to create UC storage credentials.
 
 Once done, proceed to the [`migrate-credentials` command](#migrate-credentials-command).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `create-uber-principal` command
 
 ```text
 databricks labs ucx create-uber-principal [--subscription-id X]
 ```
 
-**Requires Cloud IAM admin privileges.** Once the [`assessment` workflow](#assessment-workflow) complete, you should run 
-this command to creates a service principal with the _**read-only access to all storage**_ used by tables in this 
-workspace and configure the [UCX Cluster Policy](#installation) with the details of it. Once migration is complete, this
-service principal should be unprovisioned. On Azure, it creates a principal with `Storage Blob Data Reader` role 
-assignment on every storage account using Azure Resource Manager APIs.
+**Requires Cloud IAM admin privileges.** 
+
+Once the [`assessment` workflow](#assessment-workflow) complete, you should run this command to create a service principal with the 
+_**read-only access to all storage**_ used by tables in this workspace. It will also configure the 
+[UCX Cluster Policy](#installation) & SQL Warehouse data access configuration to use this service principal for migration 
+workflows. Once migration is complete, this service principal should be unprovisioned. 
+
+On Azure, it creates a principal with `Storage Blob Data Contributor` role assignment on every storage account using 
+Azure Resource Manager APIs.
 
 This command is one of prerequisites for the [table migration workflow](#table-migration-workflow).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `migrate-credentials` command
 
 ```commandline
 databricks labs ucx migrate-credentials
 ```
 
-For Azure, this command migrate Azure Service Principals, which have `Storage Blob Data Contributor`,
-`Storage Blob Data Reader`, `Storage Blob Data Owner` roles on ADLS Gen2 locations that are being used in
-Databricks, to UC storage credentials. The Azure Service Principals to location mapping are listed 
-in `/Users/{user_name}/.ucx/azure_storage_account_info.csv` which is generated 
-by [`principal-prefix-access` command](#principal-prefix-access-command). 
-Please review the file and delete the Service Principals you do not want to be migrated.
-The command will only migrate the Service Principals that have client secret stored in Databricks Secret.
+For Azure, this command prompts to confirm performing the following credential migration steps:
+1. [RECOMMENDED] For each storage account, create access connectors with managed identities that have the
+   `Storage Blob Data Contributor` role on the respective storage account. A storage credential is created for each 
+    access connector.
+2. Migrate Azure Service Principals, which have `Storage Blob Data Contributor`,
+   `Storage Blob Data Reader`, `Storage Blob Data Owner`, or custom roles on ADLS Gen2 locations that are being used in
+   Databricks, to UC storage credentials. The Azure Service Principals to location mapping are listed
+   in `/Users/{user_name}/.ucx/azure_storage_account_info.csv` which is generated by
+   [`principal-prefix-access` command](#principal-prefix-access-command). Please review the file and delete the Service
+   Principals you do not want to be migrated. The command will only migrate the Service Principals that have client
+   secret stored in Databricks Secret.
+
+  **Warning**: Service principals used to access storage accounts behind firewalls might cause connectivity issues. We
+  recommend to use access connectors instead.
 
 Once you're done with this command, run [`validate-external-locations` command](#validate-external-locations-command) after this one.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `validate-external-locations` command
 
@@ -797,48 +852,61 @@
 
 ## `skip` command
 
 ```text
 databricks labs ucx skip --schema X [--table Y]  
 ```
 
-Anywhere after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
+Anytime after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
 
 This command allows users to skip certain schemas or tables during the [table migration](#table-migration-workflow) process.
 The command takes `--schema` and optionally `--table` flags to specify the schema and table to skip. If no `--table` flag 
 is provided, all tables in the specified HMS database are skipped.
-This command is useful to temporarily disable migration on a particular schema or table.
+This command is useful to temporarily disable migration of a particular schema or table.
 
 Once you're done with table migration, proceed to the [code migration](#code-migration-commands).
 
 [[back to top](#databricks-labs-ucx)]
 
-## `revert-migrated-tables` command
+## `create-catalogs-schemas` command
 
 ```text
-databricks labs ucx revert-migrated-tables --schema X --table Y [--delete-managed]  
+databricks labs ucx create-catalogs-schemas
 ```
+After [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command to have the required UC catalogs and schemas created.
+This command is supposed to be run before migrating tables to UC using [table migration workflow](#table-migration-workflow).
+
+[[back to top](#databricks-labs-ucx)]
 
-Anywhere after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
+## `migrate-tables` command
 
-This command removes the `upgraded_from` property on a migrated table for re-migration in the [table migration](#table-migration-workflow) process. 
-This command is useful for developers and administrators who want to revert the migration of a table. It can also be used 
-to debug issues related to table migration.
+```text
+databricks labs ucx migrate-tables
+```
 
-Go back to the [`create-table-mapping` command](#create-table-mapping-command) after you're done with this command.
+Anytime after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
+
+This command kicks off the [table migration](#table-migration-workflow) process. It triggers the `migrate-tables` workflow, 
+and if there are HiveSerDe tables detected, prompt whether to trigger the `migrate-external-hiveserde-tables-in-place-experimental` workflow.
 
 [[back to top](#databricks-labs-ucx)]
 
-## `create-catalogs-schemas` command
+## `revert-migrated-tables` command
 
 ```text
-databricks labs ucx create-catalogs-schemas
+databricks labs ucx revert-migrated-tables --schema X --table Y [--delete-managed]  
 ```
-After [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command to have the required UC catalogs and schemas created.
-This command is supposed to be run before migrating tables to UC using [table migration workflow](#table-migration-workflow).
+
+Anytime after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
+
+This command removes the `upgraded_from` property on a migrated table for re-migration in the [table migration](#table-migration-workflow) process. 
+This command is useful for developers and administrators who want to revert the migration of a table. It can also be used 
+to debug issues related to table migration.
+
+Go back to the [`create-table-mapping` command](#create-table-mapping-command) after you're done with this command.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `move` command
 
 ```text
 databricks labs ucx move --from-catalog A --from-schema B --from-table C --to-catalog D --to-schema E  
@@ -893,14 +961,46 @@
 **(Experimental)** Once [table migration](#table-migration-workflow) is complete, you can run this command to 
 migrate all python and SQL files in the current working directory. This command is highly experimental and
 at the moment only supports Python and SQL files and discards code comments and formatting during 
 the automated transformation process.
 
 [[back to top](#databricks-labs-ucx)]
 
+## `migrate-dbsql-dashboards` command
+
+```text
+databricks labs ucx migrate-dbsql-dashboards [--dashboard-id <dashboard-id>]
+```
+
+**(Experimental)** Once [table migration](#table-migration-workflow) is complete, you can run this command to 
+migrate all Databricks SQL dashboards in the workspace. At this moment, this command is highly experimental and discards
+formatting during the automated transformation process.
+
+This command tags dashboards & queries that have been migrated with `migrated by UCX` tag. The original queries are
+also backed up in the ucx installation folder, to allow for easy rollback (see [`revert-dbsql-dashboards` command](#revert-dbsql-dashboards-command)).
+
+This command can be run with `--dashboard-id` flag to migrate a specific dashboard.
+
+This command is incremental and can be run multiple times to migrate new dashboards.
+
+[[back to top](#databricks-labs-ucx)]
+
+## `revert-dbsql-dashboards` command
+
+```text
+databricks labs ucx revert-dbsql-dashboards [--dashboard-id <dashboard-id>]
+```
+
+**(Experimental)** This command reverts the migration of Databricks SQL dashboards in the workspace, after
+`migrate-dbsql-dashboards` command is executed.
+
+This command can be run with `--dashboard-id` flag to migrate a specific dashboard.
+
+[[back to top](#databricks-labs-ucx)]
+
 # Cross-workspace installations
 
 When installing UCX across multiple workspaces, administrators need to keep UCX configurations in sync.
 UCX will prompt you to select an account profile that has been defined in `~/.databrickscfg`. If you don't have one,
 authenticate your machine with:
 
 * `databricks auth login --host https://accounts.cloud.databricks.com/` (AWS)
@@ -1033,15 +1133,15 @@
 21:31:29  INFO [d.labs.ucx] Reverting the Remapping of the Clusters from UC
 21:31:33  INFO [d.labs.ucx] 0301-055912-4ske39iq
 21:31:33  INFO [d.labs.ucx] 0306-121015-v1llqff6
 Please provide the cluster id's as comma separated value from the above list (default: <ALL>):
 ```
 
 If a customer want's to revert the cluster remap done using the [`cluster-remap` command](#cluster-remap-command) they can use this command to revert 
-its configuration from UC to original one.It will iterate through the list of clusters from the back up folder and reverts the 
+its configuration from UC to original one.It will iterate through the list of clusters from the backup folder and reverts the 
 cluster configurations to original one.This will also ask the user to provide the list of clusters that has to be reverted as a prompt.
 By default, it will revert all the clusters present in the backup folder
 
 [[back to top](#databricks-labs-ucx)]
 
 # Star History
```


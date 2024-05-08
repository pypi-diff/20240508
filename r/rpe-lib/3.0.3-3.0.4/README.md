# Comparing `tmp/rpe-lib-3.0.3.tar.gz` & `tmp/rpe-lib-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpe-lib-3.0.3.tar", last modified: Fri Apr 19 21:11:56 2024, max compression
+gzip compressed data, was "rpe-lib-3.0.4.tar", last modified: Wed May  8 17:44:50 2024, max compression
```

## Comparing `rpe-lib-3.0.3.tar` & `rpe-lib-3.0.4.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.258701 rpe-lib-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.234701 rpe-lib-3.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.234701 rpe-lib-3.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-19 21:11:56.258701 rpe-lib-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.238701 rpe-lib-3.0.3/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/exclusions.rego
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.242701 rpe-lib-3.0.3/policy/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/_util.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/appengine_instances_disallow_debug_mode.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/bigquery_datasets_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/bigquery_datasets_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/bigtable_instances_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/bigtable_instances_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_default_service_account.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/cloudresourcemanager_projects_require_all_audit_logs.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_disks_disallow_unapproved_images.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_firewalls_disallow_public_management_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_firewalls_require_logging.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_subnets_require_private_google_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/compute_subnetworks_require_flow_logging.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_clusters_disallow_kubernetes_dashboard.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_clusters_disallow_legacy_abac.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_clusters_require_stackdriver_logging.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_clusters_require_stackdriver_monitoring.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_nodepools_require_autoupgrade_and_autorepair.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/container_nodepools_require_cos_image.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_disallow_default_serviceaccount.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_disallow_extended_use.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_approved_image.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_job_logging.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_kerberos.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_stackdriver_logging.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_yarn_logging.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/pubsub_subscriptions_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/pubsub_subscriptions_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/pubsub_topics_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/pubsub_topics_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/sql_instances_disallow_public_network_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/sql_instances_require_backup_configuration.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/sql_instances_require_ssl.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/storage_buckets_disallow_authenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/storage_buckets_disallow_unauthenticated_public_access.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/storage_buckets_require_object_versioning.rego
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.246701 rpe-lib-3.0.3/policy/gcp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/appengine_instances_disallow_debug_mode_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/bigquery_datasets_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/bigquery_datasets_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/bigtable_instances_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/bigtable_instances_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_default_service_account_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_disks_disallow_unapproved_images_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_firewalls_disallow_public_management_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_firewalls_require_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_subnets_require_private_google_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/compute_subnetworks_require_flow_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_clusters_disallow_kubernetes_dashboard_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_clusters_disallow_legacy_abac_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_clusters_require_stackdriver_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_clusters_require_stackdriver_monitoring_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_nodepools_require_autoupgrade_and_autorepair_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/container_nodepools_require_cos_image_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_disallow_default_serviceaccount_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_disallow_extended_use_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_approved_image_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_job_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_kerberos_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_stackdriver_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_yarn_logging_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/pubsub_subscriptions_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/pubsub_subscriptions_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/pubsub_topics_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/pubsub_topics_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/sql_instances_disallow_public_network_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/sql_instances_require_backup_configuration_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/sql_instances_require_ssl_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_disallow_authenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_disallow_unauthenticated_public_access_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_require_object_versioning_test.rego
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/policies.rego
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/policy/util.rego
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe/engines/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/engines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/engines/opa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/engines/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17188 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/gcp_auditlogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/micromanager.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/extractors/pubsub_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/resources/__init__.pyc
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    35199 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/resources/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/rpe/rpe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/rpe_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-19 21:11:55.000000 rpe-lib-3.0.3/rpe_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-19 21:11:56.000000 rpe-lib-3.0.3/rpe_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:11:55.000000 rpe-lib-3.0.3/rpe_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 21:11:55.000000 rpe-lib-3.0.3/rpe_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 21:11:55.000000 rpe-lib-3.0.3/rpe_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:11:56.258701 rpe-lib-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.250701 rpe-lib-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:11:56.258701 rpe-lib-3.0.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/app-engine-debug.json
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/bigtable-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/bq-ds-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/cloudfunctions-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/cloudsql-protoPayload.request.body.json
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/cloudsql-protoPayload.request.resource.instanceName.instanceId.json
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/cloudsql-resource.labels.json
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute-firewalls-enable-logs-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute-hardened-images.json
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute-subnetworks-enable-flow-logs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute-subnetworks-set-private-ip-google-access.json
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_2.json
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_instance_micromanager.json
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_networks_insert_1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_networks_insert_2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/compute_networks_insert_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataflow-job-step.json
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataform-create-repository.json
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataform-create-workspace.json
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataform-update-repository.json
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/datafusion-create-instance.json
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/datafusion-update-instance.json
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/dataproc_createcluster.json
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/gke-cluster-update.json
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/gke-nodepool-set.json
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/memorystore-redis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/project_get_iam.json
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/project_set_iam.json
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/pubsub-subscription-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/pubsub-topic-set-iam-policy.json
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/servicemanagement-activate-service.json
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/servicemanagement-deactivate-service.json
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/servicemanagement-disable-service.json
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/servicemanagement-enable-service.json
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/serviceusage-batchenable.json
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/serviceusage-disable.json
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/serviceusage-enable.json
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/storage_bucket_delete.json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/storage_bucket_micromanager.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/storage_bucket_no_metadata_micromanager.json
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/data/storage_bucket_update.json
--rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/test_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/test_gcp_resource_inferred_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18739 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tests/test_resources_cai.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-19 21:11:41.000000 rpe-lib-3.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.266684 rpe-lib-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.242684 rpe-lib-3.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.246684 rpe-lib-3.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-08 17:44:50.266684 rpe-lib-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.246684 rpe-lib-3.0.4/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/exclusions.rego
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.250684 rpe-lib-3.0.4/policy/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/_util.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/appengine_instances_disallow_debug_mode.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/bigquery_datasets_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/bigquery_datasets_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/bigtable_instances_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/bigtable_instances_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/cloudfunctions_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/cloudfunctions_disallow_default_service_account.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/cloudfunctions_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/cloudresourcemanager_projects_require_all_audit_logs.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/compute_disks_disallow_unapproved_images.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/compute_firewalls_disallow_public_management_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/compute_firewalls_require_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/compute_subnets_require_private_google_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/compute_subnetworks_require_flow_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/container_clusters_disallow_kubernetes_dashboard.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/container_clusters_disallow_legacy_abac.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/container_clusters_require_stackdriver_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/container_clusters_require_stackdriver_monitoring.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/container_nodepools_require_autoupgrade_and_autorepair.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/container_nodepools_require_cos_image.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/dataproc_clusters_disallow_default_serviceaccount.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/dataproc_clusters_disallow_extended_use.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_approved_image.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_job_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_kerberos.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_stackdriver_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_yarn_logging.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/pubsub_subscriptions_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/pubsub_subscriptions_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/pubsub_topics_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/pubsub_topics_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/sql_instances_disallow_public_network_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/sql_instances_require_backup_configuration.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/sql_instances_require_ssl.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/storage_buckets_disallow_authenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/storage_buckets_disallow_unauthenticated_public_access.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/storage_buckets_require_object_versioning.rego
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.254684 rpe-lib-3.0.4/policy/gcp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/appengine_instances_disallow_debug_mode_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/bigquery_datasets_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/bigquery_datasets_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/bigtable_instances_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/bigtable_instances_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/cloudfunctions_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/cloudfunctions_disallow_default_service_account_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/cloudfunctions_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/compute_disks_disallow_unapproved_images_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/compute_firewalls_disallow_public_management_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/compute_firewalls_require_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/compute_subnets_require_private_google_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/compute_subnetworks_require_flow_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/container_clusters_disallow_kubernetes_dashboard_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/container_clusters_disallow_legacy_abac_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/container_clusters_require_stackdriver_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/container_clusters_require_stackdriver_monitoring_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/container_nodepools_require_autoupgrade_and_autorepair_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/container_nodepools_require_cos_image_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_disallow_default_serviceaccount_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_disallow_extended_use_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_approved_image_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_job_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_kerberos_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_stackdriver_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_yarn_logging_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/pubsub_subscriptions_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/pubsub_subscriptions_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/pubsub_topics_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/pubsub_topics_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/sql_instances_disallow_public_network_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/sql_instances_require_backup_configuration_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/sql_instances_require_ssl_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/storage_buckets_disallow_authenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/storage_buckets_disallow_unauthenticated_public_access_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/gcp/tests/storage_buckets_require_object_versioning_test.rego
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/policies.rego
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/policy/util.rego
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.254684 rpe-lib-3.0.4/rpe/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.258684 rpe-lib-3.0.4/rpe/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/engines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/engines/opa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/engines/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.258684 rpe-lib-3.0.4/rpe/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17188 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/extractors/gcp_auditlogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/extractors/micromanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/extractors/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/extractors/pubsub_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.258684 rpe-lib-3.0.4/rpe/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/resources/__init__.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35210 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/resources/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/rpe/rpe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.258684 rpe-lib-3.0.4/rpe_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-08 17:44:49.000000 rpe-lib-3.0.4/rpe_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-08 17:44:50.000000 rpe-lib-3.0.4/rpe_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:44:49.000000 rpe-lib-3.0.4/rpe_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 17:44:49.000000 rpe-lib-3.0.4/rpe_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 17:44:49.000000 rpe-lib-3.0.4/rpe_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:44:50.266684 rpe-lib-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.258684 rpe-lib-3.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:44:50.266684 rpe-lib-3.0.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/app-engine-debug.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/bigtable-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/bq-ds-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/cloudfunctions-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/cloudsql-protoPayload.request.body.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/cloudsql-protoPayload.request.resource.instanceName.instanceId.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/cloudsql-resource.labels.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute-firewalls-enable-logs-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute-hardened-images.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute-subnetworks-enable-flow-logs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute-subnetworks-set-private-ip-google-access.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute_instance_micromanager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute_networks_insert_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute_networks_insert_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/compute_networks_insert_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/dataflow-job-step.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/dataform-create-repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/dataform-create-workspace.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/dataform-update-repository.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/datafusion-create-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/datafusion-update-instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/dataproc_createcluster.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/gke-cluster-update.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/gke-nodepool-set.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/memorystore-redis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/project_get_iam.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/project_set_iam.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/pubsub-subscription-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/pubsub-topic-set-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/servicemanagement-activate-service.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/servicemanagement-deactivate-service.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/servicemanagement-disable-service.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/servicemanagement-enable-service.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/serviceusage-batchenable.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/serviceusage-disable.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/serviceusage-enable.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/storage_bucket_delete.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/storage_bucket_micromanager.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/storage_bucket_no_metadata_micromanager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/data/storage_bucket_update.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/test_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/test_gcp_resource_inferred_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18739 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tests/test_resources_cai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-08 17:44:39.000000 rpe-lib-3.0.4/tox.ini
```

### Comparing `rpe-lib-3.0.3/.github/workflows/build.yml` & `rpe-lib-3.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/.github/workflows/release.yml` & `rpe-lib-3.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/CONTRIBUTING.md` & `rpe-lib-3.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/LICENSE` & `rpe-lib-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/PKG-INFO` & `rpe-lib-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpe-lib
-Version: 3.0.3
+Version: 3.0.4
 Summary: A resource policy evaluation library
 Home-page: https://github.com/cleardataeng/resource-policy-evaluation-library
 Author: Joe Ceresini
 License: Apache 2.0
 Description: # resource-policy-evaluation-library
         
         rpe-lib is made up of `Policy Engines (rpe.engines.Engine)`, `Resources (rpe.resources.Resource)`, and `Extractors (rpe.resources.Extractor)`.
```

### Comparing `rpe-lib-3.0.3/README.md` & `rpe-lib-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/config.yaml` & `rpe-lib-3.0.4/policy/config.yaml`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/exclusions.rego` & `rpe-lib-3.0.4/policy/exclusions.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/appengine_instances_disallow_debug_mode.rego` & `rpe-lib-3.0.4/policy/gcp/appengine_instances_disallow_debug_mode.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/bigquery_datasets_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/bigquery_datasets_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/bigquery_datasets_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/bigquery_datasets_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/bigtable_instances_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/bigtable_instances_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/bigtable_instances_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/bigtable_instances_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/cloudfunctions_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_default_service_account.rego` & `rpe-lib-3.0.4/policy/gcp/cloudfunctions_disallow_default_service_account.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/cloudfunctions_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/cloudfunctions_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/cloudresourcemanager_projects_require_all_audit_logs.rego` & `rpe-lib-3.0.4/policy/gcp/cloudresourcemanager_projects_require_all_audit_logs.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/compute_disks_disallow_unapproved_images.rego` & `rpe-lib-3.0.4/policy/gcp/compute_disks_disallow_unapproved_images.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/compute_firewalls_disallow_public_management_access.rego` & `rpe-lib-3.0.4/policy/gcp/compute_firewalls_disallow_public_management_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/compute_firewalls_require_logging.rego` & `rpe-lib-3.0.4/policy/gcp/compute_firewalls_require_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/compute_subnets_require_private_google_access.rego` & `rpe-lib-3.0.4/policy/gcp/compute_subnets_require_private_google_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/compute_subnetworks_require_flow_logging.rego` & `rpe-lib-3.0.4/policy/gcp/compute_subnetworks_require_flow_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/container_clusters_disallow_kubernetes_dashboard.rego` & `rpe-lib-3.0.4/policy/gcp/container_clusters_disallow_kubernetes_dashboard.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/container_clusters_disallow_legacy_abac.rego` & `rpe-lib-3.0.4/policy/gcp/container_clusters_disallow_legacy_abac.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/container_clusters_require_stackdriver_logging.rego` & `rpe-lib-3.0.4/policy/gcp/container_clusters_require_stackdriver_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/container_clusters_require_stackdriver_monitoring.rego` & `rpe-lib-3.0.4/policy/gcp/container_clusters_require_stackdriver_monitoring.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/container_nodepools_require_autoupgrade_and_autorepair.rego` & `rpe-lib-3.0.4/policy/gcp/container_nodepools_require_autoupgrade_and_autorepair.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/container_nodepools_require_cos_image.rego` & `rpe-lib-3.0.4/policy/gcp/container_nodepools_require_cos_image.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_disallow_default_serviceaccount.rego` & `rpe-lib-3.0.4/policy/gcp/dataproc_clusters_disallow_default_serviceaccount.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_disallow_extended_use.rego` & `rpe-lib-3.0.4/policy/gcp/dataproc_clusters_disallow_extended_use.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_approved_image.rego` & `rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_approved_image.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_job_logging.rego` & `rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_job_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_kerberos.rego` & `rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_kerberos.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_stackdriver_logging.rego` & `rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_stackdriver_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/dataproc_clusters_require_yarn_logging.rego` & `rpe-lib-3.0.4/policy/gcp/dataproc_clusters_require_yarn_logging.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/pubsub_subscriptions_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/pubsub_subscriptions_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/pubsub_subscriptions_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/pubsub_subscriptions_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/pubsub_topics_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/pubsub_topics_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/pubsub_topics_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/pubsub_topics_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/sql_instances_disallow_public_network_access.rego` & `rpe-lib-3.0.4/policy/gcp/sql_instances_disallow_public_network_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/sql_instances_require_backup_configuration.rego` & `rpe-lib-3.0.4/policy/gcp/sql_instances_require_backup_configuration.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/sql_instances_require_ssl.rego` & `rpe-lib-3.0.4/policy/gcp/sql_instances_require_ssl.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/storage_buckets_disallow_authenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/storage_buckets_disallow_authenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/storage_buckets_disallow_unauthenticated_public_access.rego` & `rpe-lib-3.0.4/policy/gcp/storage_buckets_disallow_unauthenticated_public_access.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/storage_buckets_require_object_versioning.rego` & `rpe-lib-3.0.4/policy/gcp/storage_buckets_require_object_versioning.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/appengine_instances_disallow_debug_mode_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/appengine_instances_disallow_debug_mode_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/bigquery_datasets_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/bigquery_datasets_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/bigquery_datasets_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/bigquery_datasets_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/bigtable_instances_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/bigtable_instances_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/bigtable_instances_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/bigtable_instances_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/cloudfunctions_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_default_service_account_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/cloudfunctions_disallow_default_service_account_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/cloudfunctions_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/cloudfunctions_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/compute_disks_disallow_unapproved_images_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/compute_disks_disallow_unapproved_images_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/compute_firewalls_disallow_public_management_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/compute_firewalls_disallow_public_management_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/compute_firewalls_require_logging_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/compute_firewalls_require_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/compute_subnets_require_private_google_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/compute_subnets_require_private_google_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/compute_subnetworks_require_flow_logging_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/compute_subnetworks_require_flow_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/container_clusters_disallow_kubernetes_dashboard_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/container_clusters_disallow_kubernetes_dashboard_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/container_clusters_disallow_legacy_abac_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/container_clusters_disallow_legacy_abac_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/container_clusters_require_stackdriver_logging_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/container_clusters_require_stackdriver_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/container_clusters_require_stackdriver_monitoring_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/container_clusters_require_stackdriver_monitoring_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/container_nodepools_require_autoupgrade_and_autorepair_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/container_nodepools_require_autoupgrade_and_autorepair_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/container_nodepools_require_cos_image_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/container_nodepools_require_cos_image_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_disallow_default_serviceaccount_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_disallow_default_serviceaccount_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_disallow_extended_use_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_disallow_extended_use_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_approved_image_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_approved_image_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_job_logging_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_job_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_kerberos_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_kerberos_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_stackdriver_logging_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_stackdriver_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/dataproc_clusters_require_yarn_logging_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/dataproc_clusters_require_yarn_logging_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/pubsub_subscriptions_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/pubsub_subscriptions_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/pubsub_subscriptions_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/pubsub_subscriptions_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/pubsub_topics_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/pubsub_topics_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/pubsub_topics_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/pubsub_topics_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/sql_instances_disallow_public_network_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/sql_instances_disallow_public_network_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/sql_instances_require_backup_configuration_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/sql_instances_require_backup_configuration_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/sql_instances_require_ssl_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/sql_instances_require_ssl_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_disallow_authenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/storage_buckets_disallow_authenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_disallow_unauthenticated_public_access_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/storage_buckets_disallow_unauthenticated_public_access_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/gcp/tests/storage_buckets_require_object_versioning_test.rego` & `rpe-lib-3.0.4/policy/gcp/tests/storage_buckets_require_object_versioning_test.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/policies.rego` & `rpe-lib-3.0.4/policy/policies.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/policy/util.rego` & `rpe-lib-3.0.4/policy/util.rego`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/__init__.py` & `rpe-lib-3.0.4/rpe/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/engines/__init__.py` & `rpe-lib-3.0.4/rpe/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/engines/opa.py` & `rpe-lib-3.0.4/rpe/engines/opa.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/engines/python.py` & `rpe-lib-3.0.4/rpe/engines/python.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/exceptions.py` & `rpe-lib-3.0.4/rpe/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/extractors/__init__.py` & `rpe-lib-3.0.4/rpe/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/extractors/gcp_auditlogs.py` & `rpe-lib-3.0.4/rpe/extractors/gcp_auditlogs.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/extractors/micromanager.py` & `rpe-lib-3.0.4/rpe/extractors/micromanager.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/extractors/models.py` & `rpe-lib-3.0.4/rpe/extractors/models.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/extractors/pubsub_metadata.py` & `rpe-lib-3.0.4/rpe/extractors/pubsub_metadata.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/policy.py` & `rpe-lib-3.0.4/rpe/policy.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/resources/__init__.py` & `rpe-lib-3.0.4/rpe/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/resources/__init__.pyc` & `rpe-lib-3.0.4/rpe/resources/__init__.pyc`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/resources/base.py` & `rpe-lib-3.0.4/rpe/resources/base.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe/resources/gcp.py` & `rpe-lib-3.0.4/rpe/resources/gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,15 @@
         return self._resource_metadata
 
     # Determine what remediation steps to take, allow for future remediation specifications
     def remediate(self, remediation):
         # Check for an update spec version, default to version 1
         remediation_spec = remediation.get("_remediation_spec", "")
 
-        if remediation_spec in ["v2beta1", "v2"]:
+        if remediation_spec in ["v2beta1", "v2", "v1beta1"]:
             required_keys = ["method", "params"]
 
             for step in remediation.get("steps", []):
                 if not all(k in step for k in required_keys):
                     raise InvalidRemediationSpecStep()
 
                 method_name = step.get("method")
```

### Comparing `rpe-lib-3.0.3/rpe/rpe.py` & `rpe-lib-3.0.4/rpe/rpe.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/rpe_lib.egg-info/PKG-INFO` & `rpe-lib-3.0.4/rpe_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpe-lib
-Version: 3.0.3
+Version: 3.0.4
 Summary: A resource policy evaluation library
 Home-page: https://github.com/cleardataeng/resource-policy-evaluation-library
 Author: Joe Ceresini
 License: Apache 2.0
 Description: # resource-policy-evaluation-library
         
         rpe-lib is made up of `Policy Engines (rpe.engines.Engine)`, `Resources (rpe.resources.Resource)`, and `Extractors (rpe.resources.Extractor)`.
```

### Comparing `rpe-lib-3.0.3/rpe_lib.egg-info/SOURCES.txt` & `rpe-lib-3.0.4/rpe_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/setup.py` & `rpe-lib-3.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/__init__.py` & `rpe-lib-3.0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/app-engine-debug.json` & `rpe-lib-3.0.4/tests/data/app-engine-debug.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/bigtable-set-iam-policy.json` & `rpe-lib-3.0.4/tests/data/bigtable-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/bq-ds-set-iam-policy.json` & `rpe-lib-3.0.4/tests/data/bq-ds-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/cloudfunctions-set-iam-policy.json` & `rpe-lib-3.0.4/tests/data/cloudfunctions-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/cloudsql-protoPayload.request.body.json` & `rpe-lib-3.0.4/tests/data/cloudsql-protoPayload.request.body.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/cloudsql-protoPayload.request.resource.instanceName.instanceId.json` & `rpe-lib-3.0.4/tests/data/cloudsql-protoPayload.request.resource.instanceName.instanceId.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/cloudsql-resource.labels.json` & `rpe-lib-3.0.4/tests/data/cloudsql-resource.labels.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute-firewalls-enable-logs-policy.json` & `rpe-lib-3.0.4/tests/data/compute-firewalls-enable-logs-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute-hardened-images.json` & `rpe-lib-3.0.4/tests/data/compute-hardened-images.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute-subnetworks-enable-flow-logs.json` & `rpe-lib-3.0.4/tests/data/compute-subnetworks-enable-flow-logs.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute-subnetworks-set-private-ip-google-access.json` & `rpe-lib-3.0.4/tests/data/compute-subnetworks-set-private-ip-google-access.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_1.json` & `rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_1.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_2.json` & `rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_2.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_3.json` & `rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_3.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_4.json` & `rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_4.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute_instance_creation_logs_5.json` & `rpe-lib-3.0.4/tests/data/compute_instance_creation_logs_5.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute_networks_insert_1.json` & `rpe-lib-3.0.4/tests/data/compute_networks_insert_1.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute_networks_insert_2.json` & `rpe-lib-3.0.4/tests/data/compute_networks_insert_2.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/compute_networks_insert_3.json` & `rpe-lib-3.0.4/tests/data/compute_networks_insert_3.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/dataflow-job-step.json` & `rpe-lib-3.0.4/tests/data/dataflow-job-step.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/dataform-create-repository.json` & `rpe-lib-3.0.4/tests/data/dataform-create-repository.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/dataform-create-workspace.json` & `rpe-lib-3.0.4/tests/data/dataform-create-workspace.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/dataform-update-repository.json` & `rpe-lib-3.0.4/tests/data/dataform-update-repository.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/datafusion-create-instance.json` & `rpe-lib-3.0.4/tests/data/datafusion-create-instance.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/datafusion-update-instance.json` & `rpe-lib-3.0.4/tests/data/datafusion-update-instance.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/dataproc_createcluster.json` & `rpe-lib-3.0.4/tests/data/dataproc_createcluster.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/gke-cluster-update.json` & `rpe-lib-3.0.4/tests/data/gke-cluster-update.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/gke-nodepool-set.json` & `rpe-lib-3.0.4/tests/data/gke-nodepool-set.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/memorystore-redis.json` & `rpe-lib-3.0.4/tests/data/memorystore-redis.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/project_get_iam.json` & `rpe-lib-3.0.4/tests/data/project_get_iam.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/project_set_iam.json` & `rpe-lib-3.0.4/tests/data/project_set_iam.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/pubsub-subscription-set-iam-policy.json` & `rpe-lib-3.0.4/tests/data/pubsub-subscription-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/pubsub-topic-set-iam-policy.json` & `rpe-lib-3.0.4/tests/data/pubsub-topic-set-iam-policy.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/servicemanagement-activate-service.json` & `rpe-lib-3.0.4/tests/data/servicemanagement-activate-service.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/servicemanagement-deactivate-service.json` & `rpe-lib-3.0.4/tests/data/servicemanagement-deactivate-service.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/servicemanagement-disable-service.json` & `rpe-lib-3.0.4/tests/data/servicemanagement-disable-service.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/servicemanagement-enable-service.json` & `rpe-lib-3.0.4/tests/data/servicemanagement-enable-service.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/serviceusage-batchenable.json` & `rpe-lib-3.0.4/tests/data/serviceusage-batchenable.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/serviceusage-disable.json` & `rpe-lib-3.0.4/tests/data/serviceusage-disable.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/serviceusage-enable.json` & `rpe-lib-3.0.4/tests/data/serviceusage-enable.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/storage_bucket_delete.json` & `rpe-lib-3.0.4/tests/data/storage_bucket_delete.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/data/storage_bucket_update.json` & `rpe-lib-3.0.4/tests/data/storage_bucket_update.json`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/test_extractors.py` & `rpe-lib-3.0.4/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/test_gcp_resource_inferred_data.py` & `rpe-lib-3.0.4/tests/test_gcp_resource_inferred_data.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/test_resources.py` & `rpe-lib-3.0.4/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `rpe-lib-3.0.3/tests/test_resources_cai.py` & `rpe-lib-3.0.4/tests/test_resources_cai.py`

 * *Files identical despite different names*


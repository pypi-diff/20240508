# Comparing `tmp/nuvla_job_engine-4.0.5.tar.gz` & `tmp/nuvla_job_engine-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvla_job_engine-4.0.5.tar", max compression
+gzip compressed data, was "nuvla_job_engine-4.0.6.tar", max compression
```

## Comparing `nuvla_job_engine-4.0.5.tar` & `nuvla_job_engine-4.0.6.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0    11357 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/LICENSE
--rw-r--r--   0        0        0     4588 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/README.md
--rw-r--r--   0        0        0       74 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/__init__.py
--rw-r--r--   0        0        0       24 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/job_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/__init__.py
--rw-r--r--   0        0        0     1340 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/connector.py
--rw-r--r--   0        0        0    11757 2024-04-30 09:09:30.085070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_compose.py
--rw-r--r--   0        0        0    33689 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_machine.py
--rw-r--r--   0        0        0    15017 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_service.py
--rw-r--r--   0        0        0     8401 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_stack.py
--rwxr-xr-x   0        0        0     1412 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/install-rancher.sh
--rw-r--r--   0        0        0     1713 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/k8s-install.sh
--rw-r--r--   0        0        0     1432 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/portainer-k8s.yaml
--rw-r--r--   0        0        0      774 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/portainer-swarm.yaml
--rw-r--r--   0        0        0       68 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/ssh-add-keys.sh
--rw-r--r--   0        0        0     2868 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/helm_driver.py
--rw-r--r--   0        0        0    28909 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/k8s_driver.py
--rw-r--r--   0        0        0    25028 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/kubernetes.py
--rw-r--r--   0        0        0      322 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/__init__.py
--rw-r--r--   0        0        0      641 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/helper.py
--rw-r--r--   0        0        0    11681 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/machine.py
--rw-r--r--   0        0        0    28734 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/nuvlabox.py
--rw-r--r--   0        0        0     5380 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/registry.py
--rw-r--r--   0        0        0     3668 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/connector/utils.py
--rw-r--r--   0        0        0       95 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/__init__.py
--rw-r--r--   0        0        0     1989 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/__init__.py
--rwxr-xr-x   0        0        0     2999 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/application_docker_compose_validate.py
--rwxr-xr-x   0        0        0      320 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_deployment_set_start.py
--rwxr-xr-x   0        0        0     1686 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py
--rwxr-xr-x   0        0        0      322 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_deployment_set_update.py
--rwxr-xr-x   0        0        0      711 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py
--rwxr-xr-x   0        0        0      692 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_stop_deployment.py
--rwxr-xr-x   0        0        0      908 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_update_deployment.py
--rwxr-xr-x   0        0        0     1298 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/cancel_children_jobs.py
--rwxr-xr-x   0        0        0     4269 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_provision.py
--rwxr-xr-x   0        0        0     1719 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_start.py
--rwxr-xr-x   0        0        0     1644 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_stop.py
--rwxr-xr-x   0        0        0     2601 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_terminate.py
--rwxr-xr-x   0        0        0     2982 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/component_image_state.py
--rwxr-xr-x   0        0        0     8667 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/credential_check.py
--rw-r--r--   0        0        0     3129 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/dct_check.py
--rw-r--r--   0        0        0     2831 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_log_fetch.py
--rwxr-xr-x   0        0        0      345 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_set_delete.py
--rwxr-xr-x   0        0        0      421 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_set_force_delete.py
--rwxr-xr-x   0        0        0     5402 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_start.py
--rwxr-xr-x   0        0        0     7341 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_state.py
--rw-r--r--   0        0        0     3207 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_stop.py
--rw-r--r--   0        0        0     4010 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_update.py
--rwxr-xr-x   0        0        0      366 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/dummy_test_action.py
--rw-r--r--   0        0        0      729 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/handle_trial_end.py
--rwxr-xr-x   0        0        0     1051 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/jobs_cleanup.py
--rw-r--r--   0        0        0     3553 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/monitor_bulk_job.py
--rw-r--r--   0        0        0      697 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/notify_coupon_end.py
--rwxr-xr-x   0        0        0     2803 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py
--rwxr-xr-x   0        0        0      692 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_check_api.py
--rwxr-xr-x   0        0        0      867 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_cluster.py
--rwxr-xr-x   0        0        0     2100 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py
--rwxr-xr-x   0        0        0     4570 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_decommission.py
--rwxr-xr-x   0        0        0     1856 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py
--rwxr-xr-x   0        0        0     1273 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py
--rw-r--r--   0        0        0     1279 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py
--rwxr-xr-x   0        0        0     1247 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_reboot.py
--rwxr-xr-x   0        0        0     4425 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_releases.py
--rwxr-xr-x   0        0        0     1280 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py
--rwxr-xr-x   0        0        0     2515 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py
--rwxr-xr-x   0        0        0     2429 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py
--rwxr-xr-x   0        0        0     1633 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_update.py
--rw-r--r--   0        0        0      849 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/register_usage_record.py
--rwxr-xr-x   0        0        0     3059 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/service_image_state.py
--rw-r--r--   0        0        0        0 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_action.py
--rwxr-xr-x   0        0        0      854 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_deployment.py
--rwxr-xr-x   0        0        0     8840 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py
--rwxr-xr-x   0        0        0     1289 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/deployment_set_remove.py
--rw-r--r--   0        0        0    11037 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/deployment_utils.py
--rw-r--r--   0        0        0     4008 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/resource_log_fetch.py
--rwxr-xr-x   0        0        0     9633 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/vulnerabilities_database.py
--rw-r--r--   0        0        0     7390 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/base.py
--rw-r--r--   0        0        0     2107 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distribution.py
--rw-r--r--   0        0        0     1989 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/__init__.py
--rwxr-xr-x   0        0        0     1500 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/component_image_state.py
--rwxr-xr-x   0        0        0     2296 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state.py
--rwxr-xr-x   0        0        0     1214 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state_new.py
--rwxr-xr-x   0        0        0     2479 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state_old.py
--rwxr-xr-x   0        0        0      408 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/dummy_action.py
--rwxr-xr-x   0        0        0     2907 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/handle_trial_end.py
--rwxr-xr-x   0        0        0      440 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/jobs_cleanup.py
--rwxr-xr-x   0        0        0     1803 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py
--rwxr-xr-x   0        0        0     1754 2024-04-30 09:09:30.089070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/notify_coupon_end.py
--rwxr-xr-x   0        0        0      487 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/nuvlabox_cluster_cleanup.py
--rwxr-xr-x   0        0        0     1435 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/nuvlabox_offline.py
--rwxr-xr-x   0        0        0      475 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/nuvlabox_releases.py
--rwxr-xr-x   0        0        0     1210 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py
--rwxr-xr-x   0        0        0     2464 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/register_usage_record.py
--rwxr-xr-x   0        0        0     3119 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py
--rwxr-xr-x   0        0        0     1556 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/service_image_state.py
--rwxr-xr-x   0        0        0      503 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/vulnerabilities_database.py
--rw-r--r--   0        0        0        0 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributor/__init__.py
--rw-r--r--   0        0        0     1400 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributor/distributor.py
--rw-r--r--   0        0        0        0 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/executor/__init__.py
--rw-r--r--   0        0        0     4365 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/executor/executor.py
--rw-r--r--   0        0        0    10814 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/job.py
--rw-r--r--   0        0        0     1975 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/util.py
--rw-r--r--   0        0        0      186 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/job_engine/job/version.py
--rwxr-xr-x   0        0        0     2708 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/job_deployment_state_push.py
--rwxr-xr-x   0        0        0      208 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/job_distributor.py
--rwxr-xr-x   0        0        0      197 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/job_executor.py
--rwxr-xr-x   0        0        0     1967 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/job_restore.py
--rwxr-xr-x   0        0        0      186 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/nuvla/scripts/pause.py
--rw-r--r--   0        0        0     1204 2024-04-30 09:09:30.093070 nuvla_job_engine-4.0.5/pyproject.toml
--rw-r--r--   0        0        0     5632 1970-01-01 00:00:00.000000 nuvla_job_engine-4.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/LICENSE
+-rw-r--r--   0        0        0     4586 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/README.md
+-rw-r--r--   0        0        0       74 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/__init__.py
+-rw-r--r--   0        0        0     1340 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/connector.py
+-rw-r--r--   0        0        0    11757 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/docker_compose.py
+-rw-r--r--   0        0        0    33689 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/docker_machine.py
+-rw-r--r--   0        0        0    15017 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/docker_service.py
+-rw-r--r--   0        0        0     8401 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/docker_stack.py
+-rwxr-xr-x   0        0        0     1412 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/extra/install-rancher.sh
+-rw-r--r--   0        0        0     1713 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/extra/k8s-install.sh
+-rw-r--r--   0        0        0     1432 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/extra/portainer-k8s.yaml
+-rw-r--r--   0        0        0      774 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/extra/portainer-swarm.yaml
+-rw-r--r--   0        0        0       68 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/extra/ssh-add-keys.sh
+-rw-r--r--   0        0        0     2868 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/helm_driver.py
+-rw-r--r--   0        0        0    28909 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/k8s_driver.py
+-rw-r--r--   0        0        0    24927 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/kubernetes.py
+-rw-r--r--   0        0        0      322 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/machine/__init__.py
+-rw-r--r--   0        0        0      641 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/machine/helper.py
+-rw-r--r--   0        0        0    11681 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/machine/machine.py
+-rw-r--r--   0        0        0    28734 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/nuvlabox.py
+-rw-r--r--   0        0        0     5380 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/registry.py
+-rw-r--r--   0        0        0     3668 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/connector/utils.py
+-rw-r--r--   0        0        0       95 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/__init__.py
+-rw-r--r--   0        0        0     1989 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/__init__.py
+-rwxr-xr-x   0        0        0     2999 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/application_docker_compose_validate.py
+-rwxr-xr-x   0        0        0      320 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_deployment_set_start.py
+-rwxr-xr-x   0        0        0     1686 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py
+-rwxr-xr-x   0        0        0      322 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_deployment_set_update.py
+-rwxr-xr-x   0        0        0      711 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py
+-rwxr-xr-x   0        0        0      692 2024-05-08 15:30:56.317318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_stop_deployment.py
+-rwxr-xr-x   0        0        0      908 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_update_deployment.py
+-rwxr-xr-x   0        0        0     1298 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/cancel_children_jobs.py
+-rwxr-xr-x   0        0        0     4269 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/coe_provision.py
+-rwxr-xr-x   0        0        0     1719 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/coe_start.py
+-rwxr-xr-x   0        0        0     1644 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/coe_stop.py
+-rwxr-xr-x   0        0        0     2601 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/coe_terminate.py
+-rwxr-xr-x   0        0        0     2982 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/component_image_state.py
+-rwxr-xr-x   0        0        0     8667 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/credential_check.py
+-rw-r--r--   0        0        0     3129 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/dct_check.py
+-rw-r--r--   0        0        0     2831 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_log_fetch.py
+-rwxr-xr-x   0        0        0      345 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_set_delete.py
+-rwxr-xr-x   0        0        0      421 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_set_force_delete.py
+-rwxr-xr-x   0        0        0     5402 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_start.py
+-rwxr-xr-x   0        0        0     7341 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_state.py
+-rw-r--r--   0        0        0     3207 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_stop.py
+-rw-r--r--   0        0        0     4010 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_update.py
+-rwxr-xr-x   0        0        0      366 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/dummy_test_action.py
+-rw-r--r--   0        0        0      729 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/handle_trial_end.py
+-rwxr-xr-x   0        0        0     1051 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/jobs_cleanup.py
+-rw-r--r--   0        0        0     3553 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/monitor_bulk_job.py
+-rw-r--r--   0        0        0      697 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/notify_coupon_end.py
+-rwxr-xr-x   0        0        0     2803 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py
+-rwxr-xr-x   0        0        0      692 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_check_api.py
+-rwxr-xr-x   0        0        0      867 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_cluster.py
+-rwxr-xr-x   0        0        0     2100 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py
+-rwxr-xr-x   0        0        0     4570 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_decommission.py
+-rwxr-xr-x   0        0        0     1856 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py
+-rwxr-xr-x   0        0        0     1273 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py
+-rw-r--r--   0        0        0     1287 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py
+-rwxr-xr-x   0        0        0     1247 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_reboot.py
+-rwxr-xr-x   0        0        0     4425 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_releases.py
+-rwxr-xr-x   0        0        0     1280 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py
+-rwxr-xr-x   0        0        0     2515 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py
+-rwxr-xr-x   0        0        0     2429 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py
+-rwxr-xr-x   0        0        0     1633 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_update.py
+-rw-r--r--   0        0        0      849 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/register_usage_record.py
+-rwxr-xr-x   0        0        0     3059 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/service_image_state.py
+-rw-r--r--   0        0        0        0 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/__init__.py
+-rw-r--r--   0        0        0     1574 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/bulk_action.py
+-rwxr-xr-x   0        0        0      854 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/bulk_deployment.py
+-rwxr-xr-x   0        0        0     8840 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py
+-rwxr-xr-x   0        0        0     1289 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/deployment_set_remove.py
+-rw-r--r--   0        0        0    11037 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/deployment_utils.py
+-rw-r--r--   0        0        0     4008 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/resource_log_fetch.py
+-rwxr-xr-x   0        0        0     9633 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/vulnerabilities_database.py
+-rw-r--r--   0        0        0     7838 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/base.py
+-rw-r--r--   0        0        0     2107 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distribution.py
+-rw-r--r--   0        0        0     1989 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/__init__.py
+-rwxr-xr-x   0        0        0     1500 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/component_image_state.py
+-rwxr-xr-x   0        0        0     2296 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/deployment_state.py
+-rwxr-xr-x   0        0        0     1214 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/deployment_state_new.py
+-rwxr-xr-x   0        0        0     2479 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/deployment_state_old.py
+-rwxr-xr-x   0        0        0      408 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/dummy_action.py
+-rwxr-xr-x   0        0        0     2907 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/handle_trial_end.py
+-rwxr-xr-x   0        0        0      440 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/jobs_cleanup.py
+-rwxr-xr-x   0        0        0     1803 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py
+-rwxr-xr-x   0        0        0     1754 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/notify_coupon_end.py
+-rwxr-xr-x   0        0        0      487 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/nuvlabox_cluster_cleanup.py
+-rwxr-xr-x   0        0        0     1435 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/nuvlabox_offline.py
+-rwxr-xr-x   0        0        0      475 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/nuvlabox_releases.py
+-rwxr-xr-x   0        0        0     1210 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py
+-rwxr-xr-x   0        0        0     2464 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/register_usage_record.py
+-rwxr-xr-x   0        0        0     3119 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py
+-rwxr-xr-x   0        0        0     1556 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/service_image_state.py
+-rwxr-xr-x   0        0        0      503 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/vulnerabilities_database.py
+-rw-r--r--   0        0        0        0 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributor/__init__.py
+-rw-r--r--   0        0        0     1400 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributor/distributor.py
+-rw-r--r--   0        0        0        0 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/executor/__init__.py
+-rw-r--r--   0        0        0     4391 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/executor/executor.py
+-rw-r--r--   0        0        0    10902 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/job.py
+-rw-r--r--   0        0        0     1975 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/util.py
+-rw-r--r--   0        0        0      186 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/job_engine/job/version.py
+-rwxr-xr-x   0        0        0     2708 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/scripts/job_deployment_state_push.py
+-rwxr-xr-x   0        0        0      208 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/scripts/job_distributor.py
+-rwxr-xr-x   0        0        0      197 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/scripts/job_executor.py
+-rwxr-xr-x   0        0        0     1967 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/scripts/job_restore.py
+-rwxr-xr-x   0        0        0      186 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/nuvla/scripts/pause.py
+-rw-r--r--   0        0        0     1204 2024-05-08 15:30:56.321318 nuvla_job_engine-4.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5630 1970-01-01 00:00:00.000000 nuvla_job_engine-4.0.6/PKG-INFO
```

### Comparing `nuvla_job_engine-4.0.5/LICENSE` & `nuvla_job_engine-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/README.md` & `nuvla_job_engine-4.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ## Contributing
 
 ### Source Code Changes
 
 To contribute code to this repository, please follow these steps:
 
- 1. Create a branch from master with a descriptive, kebab-cased name
+ 1. Create a branch from main with a descriptive, kebab-cased name
     to hold all your changes.
 
  2. Follow the developer guidelines concerning formatting, etc. when
     modifying the code.
    
  3. Once the changes are ready to be reviewed, create a GitHub pull
     request.  With the pull request, provide a description of the
```

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/connector.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/connector.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_compose.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/docker_compose.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_machine.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/docker_machine.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_service.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/docker_service.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/docker_stack.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/docker_stack.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/install-rancher.sh` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/extra/install-rancher.sh`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/k8s-install.sh` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/extra/k8s-install.sh`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/portainer-k8s.yaml` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/extra/portainer-k8s.yaml`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/extra/portainer-swarm.yaml` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/extra/portainer-swarm.yaml`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/helm_driver.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/helm_driver.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/k8s_driver.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/k8s_driver.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/kubernetes.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 from ..job.job import Job
 from .connector import Connector, should_connect
 from .utils import join_stderr_stdout
 
 log = logging.getLogger('k8s_connector')
 log.setLevel(logging.DEBUG)
 
-NUVLAEDGE_SHARED_PATH = "/srv/nuvlaedge/shared"
-NUVLAEDGE_STATUS_FILE = os.path.join(NUVLAEDGE_SHARED_PATH, '.nuvlabox_status')
+
 NE_STATUS_COLLECTION = 'nuvlabox-status'
 
 
 class OperationNotAllowed(Exception):
     pass
 
 
@@ -147,18 +146,18 @@
         self.api = job.api
 
         self.nuvlabox_id = self.job['target-resource']['href']
 
         self._nuvlabox = None
         self._nuvlabox_status = None
 
-        self.k8s = Kubernetes.from_path_to_k8s_creds(NUVLAEDGE_SHARED_PATH)
+        self.k8s = Kubernetes.from_path_to_k8s_creds(job.nuvlaedge_shared_path)
         self.k8s.state_debug()
 
-        self.helm = Helm(NUVLAEDGE_SHARED_PATH)
+        self.helm = Helm(job.nuvlaedge_shared_path)
 
     def connect(self):
         self.k8s.connect()
 
     def clear_connection(self, connect_result):
         self.k8s.clear_connection(connect_result)
 
@@ -494,15 +493,15 @@
             raise ValueError('This action is only supported by pull mode')
 
         self.job = job
         self.api = job.api
 
         self.nuvlabox_resource = self.api.get(kwargs.get("nuvlabox_id"))
 
-        self.k8s = Kubernetes.from_path_to_k8s_creds(NUVLAEDGE_SHARED_PATH)
+        self.k8s = Kubernetes.from_path_to_k8s_creds(job.nuvlaedge_shared_path)
         self.k8s.state_debug()
 
     def connect(self):
         self.k8s.connect()
 
     def clear_connection(self, _):
         self.k8s.clear_connection(None)
@@ -685,16 +684,16 @@
         self.job.update_job(
             status_message='The SSH public key add/revoke has failed.')
         return 2
 
 
 class K8sLogging:
 
-    def __init__(self):
-        self.k8s = Kubernetes.from_path_to_k8s_creds(NUVLAEDGE_SHARED_PATH)
+    def __init__(self, job: Job):
+        self.k8s = Kubernetes.from_path_to_k8s_creds(job.nuvlaedge_shared_path)
         self.k8s.state_debug()
 
     def log(self, component: str, since: str, lines: int, namespace='') -> str:
         """
         Get the logs for a specific component.
 
         :param component: the component for which to get the logs
```

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/helper.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/machine/helper.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/machine/machine.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/machine/machine.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/nuvlabox.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/nuvlabox.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/registry.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/registry.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/connector/utils.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/connector/utils.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/__init__.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/application_docker_compose_validate.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/application_docker_compose_validate.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_deployment_set_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_force_delete_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_stop_deployment.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_stop_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/bulk_update_deployment.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/bulk_update_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/cancel_children_jobs.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/cancel_children_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_provision.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/coe_provision.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_start.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/coe_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_stop.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/coe_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/coe_terminate.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/coe_terminate.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/component_image_state.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/component_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/credential_check.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/credential_check.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/dct_check.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/dct_check.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_log_fetch.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_log_fetch.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_start.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_state.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_stop.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_stop.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/deployment_update.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/deployment_update.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/handle_trial_end.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/handle_trial_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/jobs_cleanup.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/jobs_cleanup.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/monitor_bulk_job.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/monitor_bulk_job.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/notify_coupon_end.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/notify_coupon_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_add_ssh_key.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_check_api.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_check_api.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_cluster.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_cluster.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_cluster_cleanup.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_decommission.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_decommission.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_disable_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_enable_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_log_fetch.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     @property
     def connector(self):
 
         if not self._connector:
             if os.getenv('KUBERNETES_SERVICE_HOST'):
                 logging.debug("Kubernetes connector used.")
                 try:
-                    self._connector = k8s.K8sLogging()
+                    self._connector = k8s.K8sLogging(self.job)
                 except Exception as e:
                     logging.error(f'Kubernetes error:\n{str(e)}')
             else:
                 self._connector = \
                     nb.NuvlaBox(
                         api=self.api,
                         nuvlabox_id=self.resource_log_parent,
```

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_reboot.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_reboot.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_releases.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_releases.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_restart_stream.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_revoke_ssh_key.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_scalability_start.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/nuvlabox_update.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/nuvlabox_update.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/register_usage_record.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/register_usage_record.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/service_image_state.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/service_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_action.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/bulk_action.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_deployment.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/bulk_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/bulk_deployment_set_apply.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/deployment_set_remove.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/deployment_set_remove.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/deployment_utils.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/utils/resource_log_fetch.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/utils/resource_log_fetch.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/actions/vulnerabilities_database.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/actions/vulnerabilities_database.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/base.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,20 @@
         required_args.add_argument('--api-secret', dest='api_secret', help='Nuvla API Key Secret',
                                    metavar='API_SECRET')
 
         parser.add_argument('--api-insecure', dest='api_insecure', default=False,
                             action='store_true',
                             help='Do not check Nuvla certificate')
 
+        # NuvlaEdge fs is required here since version 2.14.0 because the shared directory changed. For the moment,
+        # we are keeping the default value as /srv/nuvlaedge/shared. NuvlaEdge should pass the correct value
+        parser.add_argument('--nuvlaedge-fs', dest='nuvlaedge_fs',
+                            default='/srv/nuvlaedge/shared/',
+                            help='NuvlaEdge data directory (default: /srv/nuvlaedge/shared)')
+
         parser.add_argument('--api-authn-header', dest='api_authn_header', default=None,
                             help='Set header for internal authentication')
 
         parser.add_argument('--name', dest='name', metavar='NAME', default=None,
                             help='Base name for this process')
 
         parser.add_argument('--statsd', dest='statsd', metavar='STATSD',
```

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distribution.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distribution.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/__init__.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/component_image_state.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/component_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/deployment_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state_new.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/deployment_state_new.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/deployment_state_old.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/deployment_state_old.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/handle_trial_end.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/handle_trial_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/monitor_bulk_jobs.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/notify_coupon_end.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/notify_coupon_end.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/nuvlabox_offline.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/nuvlabox_offline.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/refresh_customer_subscription_cache.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/register_usage_record.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/register_usage_record.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/register_usage_record_new_deployment.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributions/service_image_state.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributions/service_image_state.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/distributor/distributor.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/distributor/distributor.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/executor/executor.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/executor/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 
 import sys
 import logging
 
 from requests.adapters import HTTPAdapter
 
+
 from ..actions import get_action, ActionNotImplemented
 from ..actions.utils.bulk_action import BulkAction
 from ..base import Base
 from ..job import Job, JobUpdateError, \
     JOB_FAILED, JOB_SUCCESS, JOB_QUEUED, JOB_RUNNING
 from ..util import override, retry_kazoo_queue_op, status_message_from_exception
 
+
 CONNECTION_POOL_SIZE = 4
 
 
 class LocalOneJobQueue(object):
 
     def __init__(self, job_id):
         self.job_id = job_id
@@ -52,15 +54,15 @@
         is_single_job_only = isinstance(queue, LocalOneJobQueue)
         api_http_adapter = HTTPAdapter(pool_maxsize=CONNECTION_POOL_SIZE,
                                        pool_connections=CONNECTION_POOL_SIZE)
         self.api.session.mount('http://', api_http_adapter)
         self.api.session.mount('https://', api_http_adapter)
 
         while not Executor.stop_event.is_set():
-            job = Job(self.api, queue)
+            job = Job(self.api, queue, self.args.nuvlaedge_fs)
 
             if job.nothing_to_do:
                 if is_single_job_only:
                     break
                 else:
                     continue
```

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/job.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,23 @@
     def __init__(self, reason):
         super(JobUpdateError, self).__init__(reason)
         self.reason = reason
 
 
 class Job(dict):
 
-    def __init__(self, api, queue):
+    def __init__(self, api, queue, nuvlaedge_shared_path=None):
         super(Job, self).__init__()
         self.nothing_to_do = False
         self.id = None
         self.cimi_job = None
         self.queue = queue
         self.api = api
+        self.nuvlaedge_shared_path = nuvlaedge_shared_path
+
         self._context = None
         self._payload = None
         self._engine_version = version_to_tuple(engine_version)
         if self._engine_version[0] < 2:
             self._engine_version_min = (0, 0, 1)
         elif self._engine_version[0] == 4:
             # For job-engine 4.x, we support jobs with version 2.x and 3.x
```

### Comparing `nuvla_job_engine-4.0.5/nuvla/job_engine/job/util.py` & `nuvla_job_engine-4.0.6/nuvla/job_engine/job/util.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/scripts/job_deployment_state_push.py` & `nuvla_job_engine-4.0.6/nuvla/scripts/job_deployment_state_push.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/nuvla/scripts/job_restore.py` & `nuvla_job_engine-4.0.6/nuvla/scripts/job_restore.py`

 * *Files identical despite different names*

### Comparing `nuvla_job_engine-4.0.5/pyproject.toml` & `nuvla_job_engine-4.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nuvla-job-engine"
-version = "4.0.5"
+version = "4.0.6"
 description = "Nuvla Job Engine."
 license = "Apache-2.0"
 authors = ["SixSq SA <support@sixsq.com>"]
 maintainers = ["Ignacio Penas <nacho@sixsq.com>"]
 readme = "README.md"
 repository = "https://github.com/nuvla/job-engine"
 classifiers = [
```

### Comparing `nuvla_job_engine-4.0.5/PKG-INFO` & `nuvla_job_engine-4.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvla-job-engine
-Version: 4.0.5
+Version: 4.0.6
 Summary: Nuvla Job Engine.
 Home-page: https://github.com/nuvla/job-engine
 License: Apache-2.0
 Author: SixSq SA
 Author-email: support@sixsq.com
 Maintainer: Ignacio Penas
 Maintainer-email: nacho@sixsq.com
@@ -44,15 +44,15 @@
 
 ## Contributing
 
 ### Source Code Changes
 
 To contribute code to this repository, please follow these steps:
 
- 1. Create a branch from master with a descriptive, kebab-cased name
+ 1. Create a branch from main with a descriptive, kebab-cased name
     to hold all your changes.
 
  2. Follow the developer guidelines concerning formatting, etc. when
     modifying the code.
    
  3. Once the changes are ready to be reviewed, create a GitHub pull
     request.  With the pull request, provide a description of the
```


# Comparing `tmp/rally-4.0.0.tar.gz` & `tmp/rally-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rally-4.0.0.tar", last modified: Mon Jan 15 13:44:58 2024, max compression
+gzip compressed data, was "rally-4.1.0.tar", last modified: Wed May  8 05:39:27 2024, max compression
```

## Comparing `rally-4.0.0.tar` & `rally-4.1.0.tar`

### file list

```diff
@@ -1,775 +1,775 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.712249 rally-4.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-01-15 13:44:30.000000 rally-4.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-01-15 13:44:30.000000 rally-4.0.0/.dockerignore
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.540242 rally-4.0.0/.zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-01-15 13:44:30.000000 rally-4.0.0/.zuul.d/docker-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-01-15 13:44:30.000000 rally-4.0.0/.zuul.d/install-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2024-01-15 13:44:30.000000 rally-4.0.0/.zuul.d/python-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2024-01-15 13:44:30.000000 rally-4.0.0/.zuul.d/zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17551 2024-01-15 13:44:58.000000 rally-4.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15674 2024-01-15 13:44:30.000000 rally-4.0.0/CHANGELOG.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2024-01-15 13:44:30.000000 rally-4.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   159325 2024-01-15 13:44:57.000000 rally-4.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3692 2024-01-15 13:44:30.000000 rally-4.0.0/DOCKER_README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2024-01-15 13:44:30.000000 rally-4.0.0/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2024-01-15 13:44:30.000000 rally-4.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5947 2024-01-15 13:44:58.712249 rally-4.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4001 2024-01-15 13:44:30.000000 rally-4.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2024-01-15 13:44:30.000000 rally-4.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.540242 rally-4.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1292 2024-01-15 13:44:30.000000 rally-4.0.0/doc/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.544242 rally-4.0.0/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8055 2024-01-15 13:44:30.000000 rally-4.0.0/doc/ext/cli_reference.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2024-01-15 13:44:30.000000 rally-4.0.0/doc/ext/include_vars.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16313 2024-01-15 13:44:30.000000 rally-4.0.0/doc/ext/plugin_reference.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2024-01-15 13:44:30.000000 rally-4.0.0/doc/ext/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.544242 rally-4.0.0/doc/feature_request/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/capture_task_logging.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/check_queue_perfdata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/comparing_results_of_2_tasks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/distributed_load_generation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/explicitly_specify_existing_users_for_scenarios.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/historical_performance_data.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.548243 rally-4.0.0/doc/feature_request/implemented/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/implemented/LDAP_support.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/implemented/add_possibility_to_specify_concurrency_for_tempest.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2361 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/implemented/stop_scenario_after_several_errors.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/installation_script_enhancements.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/installing_isolated.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/launch_specific_benchmark.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/multi_scenarios_load_gen.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/multiple_attach_volume.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/persistence_benchmark_env.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2024-01-15 13:44:30.000000 rally-4.0.0/doc/feature_request/production_ready_cleanup.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.548243 rally-4.0.0/doc/release_notes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.556243 rally-4.0.0/doc/release_notes/archive/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.0.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.0.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3786 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.0.3.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7345 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.0.4.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13260 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.1.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.1.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6107 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.1.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22893 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.10.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.10.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10366 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.11.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2904 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.11.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2534 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.11.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.12.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.12.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4818 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.2.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5616 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.3.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.3.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.3.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.3.3.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8588 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.4.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13852 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.5.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7624 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.6.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5842 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.7.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10065 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.8.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.8.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5551 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.9.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.9.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v0.9.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive/v1.0.0.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/archive.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2024-01-15 13:44:30.000000 rally-4.0.0/doc/release_notes/latest.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-01-15 13:44:30.000000 rally-4.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.556243 rally-4.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6758 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.520241 rally-4.0.0/doc/source/_templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.556243 rally-4.0.0/doc/source/_templates/openstackrally/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.556243 rally-4.0.0/doc/source/_templates/openstackrally/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/_templates/openstackrally/_static/img.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/_templates/openstackrally/layout.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       27 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/_templates/openstackrally/theme.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/cli_reference.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9577 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2296 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/contribute.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/feature_requests.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.576244 rally-4.0.0/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18652 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Amqp_rpc_single_reply_queue.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64751 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Hook-Aggregated-Report.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    88398 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Hook-Per-Hook-Report.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38695 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Hook-Results.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    95868 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Rally-Actions.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29546 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Rally-Plugins.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   127052 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Rally-UseCases.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   175620 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Rally_Architecture.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   168071 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Rally_Distributed_Runner.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   105436 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Rally_QA.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67056 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Rally_VM_list.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   116187 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Rally_snapshot_vm.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59267 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Rally_who_is_using.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   118771 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Abort-on-SLA-task-1.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   133861 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Abort-on-SLA-task-2.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   188455 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Collage.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48010 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Multiple-Configurations-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44839 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Multiple-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39473 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40004 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-SLA-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    73756 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-SLA-Scenario.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    76785 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Scenario-Atomic.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   111232 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Scenario-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20517 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Actions-durations.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24204 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Distribution.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77249 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Failures.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   103829 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Input-file.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8784 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Load-profile.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   101257 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28224 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-SLA.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55099 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Scenario-Data-Aggregated.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25172 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration-profiler.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    82653 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20731 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Subtask-configuration.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34215 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Task-Total-durations.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    74855 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Trends-Atomic-actions.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21142 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Trends-Configuration.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25032 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Trends-Overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    75196 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Trends-Total.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9812 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Trends-single-run.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81001 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Verify-filter-by-status.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    98165 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Verify-for-4-Verifications.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26831 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Verify-toggle-tags.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    84067 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Verify-tracebacks.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   134147 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/images/Report-Verify-xfail.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.576244 rally-4.0.0/doc/source/install_and_upgrade/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/install_and_upgrade/db_migrations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/install_and_upgrade/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1390 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/install_and_upgrade/install.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.576244 rally-4.0.0/doc/source/overview/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4941 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/overview/glossary.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/overview/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6449 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/overview/overview.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/overview/user_stories.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.580244 rally-4.0.0/doc/source/plugins/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.580244 rally-4.0.0/doc/source/plugins/implementation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4729 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/plugins/implementation/context_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11825 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/plugins/implementation/hook_and_trigger_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/plugins/implementation/runner_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/plugins/implementation/scenario_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/plugins/implementation/sla_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2615 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/plugins/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/plugins/plugin_reference.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.580244 rally-4.0.0/doc/source/project_info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9725 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/project_info/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/project_info/release_notes.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.580244 rally-4.0.0/doc/source/quick_start/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5535 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/gates.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.584244 rally-4.0.0/doc/source/quick_start/tutorial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2778 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_10_profiling_openstack_internals.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13823 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_1_setting_up_env_and_running_benchmark_from_samples.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9129 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_2_input_task_format.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5211 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_3_benchmarking_with_existing_users.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5731 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_4_adding_success_criteria_for_benchmarks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10059 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_5_task_templates.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6075 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_6_aborting_load_generation_on_sla_failure.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8178 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_7_working_with_multple_openstack_clouds.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8103 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_8_discovering_more_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45288 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial/step_9_verifying_cloud_via_tempest_verifier.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/quick_start/tutorial.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.584244 rally-4.0.0/doc/source/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10006 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/task/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.584244 rally-4.0.0/doc/source/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/verification/cli_reference.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.584244 rally-4.0.0/doc/source/verification/howto/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3773 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/verification/howto/add_new_reporter.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4453 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/verification/howto/add_support_for_new_tool.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/verification/howto/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16640 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/verification/howto/migrate_from_old_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/verification/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3075 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/verification/overview.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4254 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/verification/reports.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3626 2024-01-15 13:44:30.000000 rally-4.0.0/doc/source/verification/verifiers.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.584244 rally-4.0.0/doc/specs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.588244 rally-4.0.0/doc/specs/implemented/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2713 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/class-based-scenarios.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4492 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/consistent_resource_names.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10835 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/db_refactoring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6472 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/deployment_type.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7816 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/hook_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/improve_atomic_actions_format.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11368 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/improve_scenario_output_format.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10567 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/new_rally_input_task_format.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/osprofiler.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/pluggable_validators.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1466 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/sla_pd_plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/split_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3017 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/task_and_verification_export.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30381 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/implemented/verification_refactoring.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.592244 rally-4.0.0/doc/specs/in-progress/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/in-progress/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7564 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/in-progress/cleanup_refactoring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5158 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/in-progress/distributed_runner.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11197 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/in-progress/pluggable-types.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11188 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/in-progress/raas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11465 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/in-progress/refactor_scenario_utils.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2024-01-15 13:44:30.000000 rally-4.0.0/doc/specs/template.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.520241 rally-4.0.0/doc/user_stories/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.592244 rally-4.0.0/doc/user_stories/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6391 2024-01-15 13:44:30.000000 rally-4.0.0/doc/user_stories/keystone/authenticate.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.592244 rally-4.0.0/doc/user_stories/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8685 2024-01-15 13:44:30.000000 rally-4.0.0/doc/user_stories/nova/boot_server.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.592244 rally-4.0.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2024-01-15 13:44:30.000000 rally-4.0.0/etc/motd_for_docker
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.592244 rally-4.0.0/etc/rally/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-01-15 13:44:30.000000 rally-4.0.0/etc/rally/rally-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11258 2024-01-15 13:44:30.000000 rally-4.0.0/etc/rally/rally.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4643 2024-01-15 13:44:30.000000 rally-4.0.0/etc/rally.bash_completion
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.592244 rally-4.0.0/rally/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.596244 rally-4.0.0/rally/aas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-01-15 13:44:30.000000 rally-4.0.0/rally/aas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    54948 2024-01-15 13:44:30.000000 rally-4.0.0/rally/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.600245 rally-4.0.0/rally/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27181 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/cliutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.600245 rally-4.0.0/rally/cli/commands/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/commands/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/commands/db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15083 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/commands/deployment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13986 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/commands/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4609 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/commands/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37124 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/commands/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40419 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/commands/verify.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6286 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/envutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9054 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/task_results_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2024-01-15 13:44:30.000000 rally-4.0.0/rally/cli/yamlutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.604245 rally-4.0.0/rally/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2699 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/broker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/cfg.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.604245 rally-4.0.0/rally/common/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24554 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.604245 rally-4.0.0/rally/common/db/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.616245 rally-4.0.0/rally/common/db/migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7920 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_01_ca3626f62937_init_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_03_3177d36ea270_merge_credentials_from_users_and_admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5678 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_04_4ef544102ba7_change_task_status_enum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15421 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_04_e654a0648db0_refactor_task_results.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2938 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_07_54e844ebfbc3_update_deployment_configs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_08_32fada9b2fde_remove_admin_domain_name.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3700 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_09_08e1515a576c_fix_invalid_verification_logs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_09_6ad4f426f005_add_hooks_to_task_result.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7712 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_11_484cd9413e66_new_db_schema_for_verification_component.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2016_12_37fdbb373e8d_fix_test_results_for_verifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_01_a6f364988fc2_change_tag_type_enum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_01_f33f4610dcda_change_verification_statuses.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_02_92aaaa2a6bb3_refactor_credentials.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3450 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_06_35fe16d4ab1c_update_tasks_based_on_workloads.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_06_c517b0011857_fill_missed_workload_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2642 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_07_7948b83229f6_workload_min_max_durations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_08_fab4f4f31f8a_fill_missed_workload_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2221 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_09_046a38742e89_port_configs_to_new_formats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_09_e0a5df2c5153_upsize_the_size_of_task_title.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5002 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_10_4394bdc32cfd_fill_missed_workload_info_r3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_10_9a18c6fe265c_rename_namespace_to_platform.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8561 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_10_dc46687661df_update_contexts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2017_12_a43700a813a5_add_env_platforms_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2018_01_44169f4d455e_deleted_worker_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2018_01_7287df262dbc_move_deployment_to_env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2018_02_95208e4eface_add_config_field_to_env_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7918 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2018_02_bc908ac9a1fc_move_deployment_to_env_2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/migrations/versions/2018_02_dc0fe6de6786_update_old_deployment_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11978 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5325 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/sa_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5099 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/db/schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/fileutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.616245 rally-4.0.0/rally/common/io/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/io/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5509 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/io/junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9452 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/io/subunit_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11272 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/logging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.616245 rally-4.0.0/rally/common/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6637 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/objects/deploy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24513 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/objects/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3248 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/objects/verification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/objects/verifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.616245 rally-4.0.0/rally/common/plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5846 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/plugin/discover.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4372 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/plugin/info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4549 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/plugin/meta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7390 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/plugin/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/sshutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7808 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/streaming_algorithms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26149 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10594 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-01-15 13:44:30.000000 rally-4.0.0/rally/common/yamlutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6911 2024-01-15 13:44:30.000000 rally-4.0.0/rally/consts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.620246 rally-4.0.0/rally/env/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/env/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25830 2024-01-15 13:44:30.000000 rally-4.0.0/rally/env/env_mgr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3978 2024-01-15 13:44:30.000000 rally-4.0.0/rally/env/platform.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6680 2024-01-15 13:44:30.000000 rally-4.0.0/rally/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.620246 rally-4.0.0/rally/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.620246 rally-4.0.0/rally/plugins/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.620246 rally-4.0.0/rally/plugins/common/exporters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/exporters/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.620246 rally-4.0.0/rally/plugins/common/exporters/elastic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/exporters/elastic/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      936 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/exporters/elastic/client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      940 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/exporters/elastic/exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/exporters/elastic/flatten.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/exporters/html.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/exporters/json_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/exporters/junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/exporters/trends.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.620246 rally-4.0.0/rally/plugins/common/hook/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/hook/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/hook/sys_call.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.624246 rally-4.0.0/rally/plugins/common/hook/triggers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/hook/triggers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/hook/triggers/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/hook/triggers/periodic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.624246 rally-4.0.0/rally/plugins/common/runners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/runners/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/runners/constant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/runners/rps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/runners/serial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.624246 rally-4.0.0/rally/plugins/common/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/scenarios/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.624246 rally-4.0.0/rally/plugins/common/scenarios/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/scenarios/dummy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/scenarios/dummy/dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.624246 rally-4.0.0/rally/plugins/common/scenarios/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/scenarios/requests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/scenarios/requests/http_requests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/scenarios/requests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.628246 rally-4.0.0/rally/plugins/common/sla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/sla/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/sla/failure_rate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/sla/iteration_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/sla/max_average_duration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/sla/max_average_duration_per_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/sla/outliers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/sla/performance_degradation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17661 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.628246 rally-4.0.0/rally/plugins/common/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/verification/reporters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/common/verification/testr.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.628246 rally-4.0.0/rally/plugins/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.628246 rally-4.0.0/rally/plugins/task/contexts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/contexts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/contexts/dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.628246 rally-4.0.0/rally/plugins/task/exporters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.632246 rally-4.0.0/rally/plugins/task/exporters/elastic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/elastic/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6196 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/elastic/client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16360 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/elastic/exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/elastic/flatten.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/html.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5596 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/json_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3560 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4587 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/old_json_results.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1406 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/exporters/trends.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.632246 rally-4.0.0/rally/plugins/task/hook_triggers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/hook_triggers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/hook_triggers/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2702 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/hook_triggers/periodic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.632246 rally-4.0.0/rally/plugins/task/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/hooks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2562 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/hooks/sys_call.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.632246 rally-4.0.0/rally/plugins/task/runners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/runners/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14074 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/runners/constant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11662 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/runners/rps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3062 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/runners/serial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.632246 rally-4.0.0/rally/plugins/task/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/scenarios/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.632246 rally-4.0.0/rally/plugins/task/scenarios/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/scenarios/dummy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11367 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/scenarios/dummy/dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.632246 rally-4.0.0/rally/plugins/task/scenarios/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/scenarios/requests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/scenarios/requests/http_requests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/scenarios/requests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.636246 rally-4.0.0/rally/plugins/task/sla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/sla/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/sla/failure_rate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/sla/iteration_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/sla/max_average_duration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3150 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/sla/max_average_duration_per_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4536 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/sla/outliers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/sla/performance_degradation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/task/types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.636246 rally-4.0.0/rally/plugins/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18676 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/verification/reporters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5791 2024-01-15 13:44:30.000000 rally-4.0.0/rally/plugins/verification/testr.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.640246 rally-4.0.0/rally/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4535 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11493 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21517 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/engine.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3544 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7062 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/functional.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8619 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/hook.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.644246 rally-4.0.0/rally/task/processing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/processing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35112 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/processing/charts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16819 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/processing/plot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3080 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/processing/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9895 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/runner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7474 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/scenario.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14956 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6007 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/sla.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15607 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/task_cfg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8847 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2024-01-15 13:44:30.000000 rally-4.0.0/rally/task/validation.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.644246 rally-4.0.0/rally/ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.644246 rally-4.0.0/rally/ui/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2802 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/base.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.644246 rally-4.0.0/rally/ui/templates/ci/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/ci/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2138 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/ci/index_verify.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.648247 rally-4.0.0/rally/ui/templates/libs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/libs/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   124229 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/libs/angular.1.3.3.min.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   148039 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/libs/d3.3.4.13.min.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8796 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   188436 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.648247 rally-4.0.0/rally/ui/templates/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10234 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/task/directive_widget.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31337 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/task/report.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17746 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/task/trends.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.648247 rally-4.0.0/rally/ui/templates/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12229 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/templates/verification/report.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2024-01-15 13:44:30.000000 rally-4.0.0/rally/ui/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.648247 rally-4.0.0/rally/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3532 2024-01-15 13:44:30.000000 rally-4.0.0/rally/utils/encodeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10988 2024-01-15 13:44:30.000000 rally-4.0.0/rally/utils/sshutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2024-01-15 13:44:30.000000 rally-4.0.0/rally/utils/strutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.652247 rally-4.0.0/rally/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2024-01-15 13:44:30.000000 rally-4.0.0/rally/verification/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16784 2024-01-15 13:44:30.000000 rally-4.0.0/rally/verification/manager.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3035 2024-01-15 13:44:30.000000 rally-4.0.0/rally/verification/reporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2024-01-15 13:44:30.000000 rally-4.0.0/rally/verification/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.592244 rally-4.0.0/rally-jobs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.596244 rally-4.0.0/rally-jobs/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2024-01-15 13:44:30.000000 rally-4.0.0/rally-jobs/plugins/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally-jobs/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2024-01-15 13:44:30.000000 rally-4.0.0/rally-jobs/plugins/fake_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2024-01-15 13:44:30.000000 rally-4.0.0/rally-jobs/plugins/rally_profile.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.596244 rally-4.0.0/rally-jobs/plugins/test_relative_import/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/rally-jobs/plugins/test_relative_import/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2024-01-15 13:44:30.000000 rally-4.0.0/rally-jobs/plugins/test_relative_import/zzz.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11899 2024-01-15 13:44:30.000000 rally-4.0.0/rally-jobs/self-rally.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.596244 rally-4.0.0/rally.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5947 2024-01-15 13:44:58.000000 rally-4.0.0/rally.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25799 2024-01-15 13:44:58.000000 rally-4.0.0/rally.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-15 13:44:58.000000 rally-4.0.0/rally.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-01-15 13:44:58.000000 rally-4.0.0/rally.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-15 13:44:58.000000 rally-4.0.0/rally.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-01-15 13:44:58.000000 rally-4.0.0/rally.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2024-01-15 13:44:58.000000 rally-4.0.0/rally.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2024-01-15 13:44:58.000000 rally-4.0.0/rally.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1496 2024-01-15 13:44:30.000000 rally-4.0.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.652247 rally-4.0.0/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-01-15 13:44:30.000000 rally-4.0.0/samples/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.652247 rally-4.0.0/samples/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.652247 rally-4.0.0/samples/tasks/contexts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/contexts/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/contexts/dummy-context.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/contexts/dummy-context.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.652247 rally-4.0.0/samples/tasks/runners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/runners/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.652247 rally-4.0.0/samples/tasks/runners/constant/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/runners/constant/constant-for-duration.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/runners/constant/constant-for-duration.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/runners/constant/constant-timeout.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/runners/constant/constant-timeout.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.656247 rally-4.0.0/samples/tasks/runners/rps/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/runners/rps/rps.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/runners/rps/rps.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.656247 rally-4.0.0/samples/tasks/runners/serial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/runners/serial/serial.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/runners/serial/serial.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.656247 rally-4.0.0/samples/tasks/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.660247 rally-4.0.0/samples/tasks/scenarios/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-exception-probability.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-exception-probability.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-exception.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-exception.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-failure.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-failure.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-output.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-output.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-random-action.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-random-action.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/dummy/dummy.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.660247 rally-4.0.0/samples/tasks/scenarios/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/requests/check-random-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/requests/check-random-request.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/requests/check-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/scenarios/requests/check-request.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.660247 rally-4.0.0/samples/tasks/sla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/sla/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/sla/dummy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-01-15 13:44:30.000000 rally-4.0.0/samples/tasks/sla/dummy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-01-15 13:44:58.712249 rally-4.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2024-01-15 13:44:30.000000 rally-4.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2024-01-15 13:44:30.000000 rally-4.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.664247 rally-4.0.0/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2024-01-15 13:44:30.000000 rally-4.0.0/tests/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.664247 rally-4.0.0/tests/ci/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2323 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/cover.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.664247 rally-4.0.0/tests/ci/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/docker-build-and-check.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/docker-build-check-and-push.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1531 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/rally-install-pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/rally-install-run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.532242 rally-4.0.0/tests/ci/playbooks/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.532242 rally-4.0.0/tests/ci/playbooks/roles/docker-build-image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.668247 rally-4.0.0/tests/ci/playbooks/roles/docker-build-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/roles/docker-build-image/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.668247 rally-4.0.0/tests/ci/playbooks/roles/docker-build-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.532242 rally-4.0.0/tests/ci/playbooks/roles/docker-push-image/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.668247 rally-4.0.0/tests/ci/playbooks/roles/docker-push-image/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/roles/docker-push-image/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.668247 rally-4.0.0/tests/ci/playbooks/roles/docker-push-image/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.532242 rally-4.0.0/tests/ci/playbooks/roles/rally-tox/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.668247 rally-4.0.0/tests/ci/playbooks/roles/rally-tox/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/roles/rally-tox/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.668247 rally-4.0.0/tests/ci/playbooks/roles/rally-tox/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/roles/rally-tox/files/find_python_for_tox_env.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.668247 rally-4.0.0/tests/ci/playbooks/roles/rally-tox/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/roles/rally-tox/tasks/install.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/roles/rally-tox/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/roles/rally-tox/tasks/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/tox-install.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/playbooks/tox-run.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3993 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/pytest_launcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/rally_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4012 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/rally_self_job.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/render.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13962 2024-01-15 13:44:30.000000 rally-4.0.0/tests/ci/sync_requirements.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.672248 rally-4.0.0/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.672248 rally-4.0.0/tests/functional/extra/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.672248 rally-4.0.0/tests/functional/extra/fake_dir1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/extra/fake_dir1/fake_plugin1.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.672248 rally-4.0.0/tests/functional/extra/fake_dir2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/extra/fake_dir2/fake_plugin2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/extra/fake_platforms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2044 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/extra/fake_verify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/extra/test_fake_scenario.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/test_cli_deployment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3216 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/test_cli_env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/test_cli_functional.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/test_cli_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58028 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/test_cli_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5542 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/test_cli_verify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/test_lib_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7839 2024-01-15 13:44:30.000000 rally-4.0.0/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.672248 rally-4.0.0/tests/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20461 2024-01-15 13:44:30.000000 rally-4.0.0/tests/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.676248 rally-4.0.0/tests/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/samples/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7006 2024-01-15 13:44:30.000000 rally-4.0.0/tests/samples/test_task_samples.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.676248 rally-4.0.0/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.680248 rally-4.0.0/tests/unit/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.680248 rally-4.0.0/tests/unit/cli/commands/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/commands/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/commands/test_db.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    23141 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/commands/test_deployment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/commands/test_docstrings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21802 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/commands/test_env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/commands/test_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50082 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/commands/test_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36667 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/commands/test_verify.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37060 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/test_cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5589 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/test_envutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9219 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/test_task_results_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/cli/test_yamlutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.684248 rally-4.0.0/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.684248 rally-4.0.0/tests/unit/common/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38662 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/db/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   111129 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/db/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5796 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/db/test_migrations_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5995 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/db/test_types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.684248 rally-4.0.0/tests/unit/common/io/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/io/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3470 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/io/subunit_v2.stream
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2334 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/io/test_junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/io/test_subunit_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.688248 rally-4.0.0/tests/unit/common/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8664 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/objects/test_deploy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26722 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/objects/test_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6230 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/objects/test_verification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/objects/test_verifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.688248 rally-4.0.0/tests/unit/common/plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/plugin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9817 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/plugin/test_discover.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4208 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/plugin/test_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5204 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/plugin/test_meta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8028 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/plugin/test_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2822 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/test_broker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12226 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/test_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1558 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/test_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10136 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/test_streaming_algorithms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27264 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6137 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/test_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/common/test_version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.688248 rally-4.0.0/tests/unit/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/doc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/doc/test_docker_readme.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6020 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/doc/test_docstrings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/doc/test_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8647 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/doc/test_jsonschemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4530 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/doc/test_specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/doc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.692248 rally-4.0.0/tests/unit/env/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/env/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31964 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/env/test_env_mgr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/env/test_platform.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4637 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.692248 rally-4.0.0/tests/unit/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.692248 rally-4.0.0/tests/unit/plugins/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18275 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/common/test_validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.692248 rally-4.0.0/tests/unit/plugins/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.692248 rally-4.0.0/tests/unit/plugins/task/contexts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/contexts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/contexts/test_dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.696249 rally-4.0.0/tests/unit/plugins/task/exporters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4766 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/dummy_data.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.696249 rally-4.0.0/tests/unit/plugins/task/exporters/elastic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/elastic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8347 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/elastic/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20745 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/elastic/test_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/elastic/test_flatten.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/junit_report.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/test_html.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5144 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/test_json_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/test_junit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5414 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/test_old_json_results.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/exporters/test_trends.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.696249 rally-4.0.0/tests/unit/plugins/task/hook_triggers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/hook_triggers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2774 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/hook_triggers/test_event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3498 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/hook_triggers/test_periodic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.696249 rally-4.0.0/tests/unit/plugins/task/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/hooks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5058 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/hooks/test_sys_call.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.700249 rally-4.0.0/tests/unit/plugins/task/runners/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/runners/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13700 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/runners/test_constant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13691 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/runners/test_rps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2937 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/runners/test_serial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.700249 rally-4.0.0/tests/unit/plugins/task/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/scenarios/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.700249 rally-4.0.0/tests/unit/plugins/task/scenarios/dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/scenarios/dummy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9988 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/scenarios/dummy/test_dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.700249 rally-4.0.0/tests/unit/plugins/task/scenarios/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/scenarios/requests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/scenarios/requests/test_http_requests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/scenarios/requests/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.704249 rally-4.0.0/tests/unit/plugins/task/sla/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/sla/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4983 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/sla/test_failure_rate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/sla/test_iteration_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/sla/test_max_average_duration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5397 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/sla/test_max_average_duration_per_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5363 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/sla/test_outliers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3428 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/sla/test_performance_degradation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3558 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/task/test_types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.704249 rally-4.0.0/tests/unit/plugins/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/verification/junit_report.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18394 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/verification/test_reporters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17456 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/plugins/verification/test_testr.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.708249 rally-4.0.0/tests/unit/task/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.708249 rally-4.0.0/tests/unit/task/processing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/processing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47254 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/processing/test_charts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33744 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/processing/test_plot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4654 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/processing/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4935 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13920 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43094 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3213 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9481 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_functional.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13184 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_hook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9218 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_runner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6440 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_scenario.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9279 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6932 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_sla.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11894 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_task_cfg.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5377 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23353 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/task/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    90112 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test_ddt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14649 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12518 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test_mock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2569 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test_pytest_launcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test_test_ddt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14784 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/test_test_mock.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.708249 rally-4.0.0/tests/unit/ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/ui/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/ui/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.708249 rally-4.0.0/tests/unit/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/utils/test_encodeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14089 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/utils/test_sshutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7744 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/utils/test_strutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:58.712249 rally-4.0.0/tests/unit/verification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/verification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/verification/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15834 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/verification/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3241 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/verification/test_reporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3837 2024-01-15 13:44:30.000000 rally-4.0.0/tests/unit/verification/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5976 2024-01-15 13:44:30.000000 rally-4.0.0/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2024-01-15 13:44:30.000000 rally-4.0.0/upper-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.177061 rally-4.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-05-08 05:38:59.000000 rally-4.1.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-05-08 05:38:59.000000 rally-4.1.0/.dockerignore
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.029010 rally-4.1.0/.zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-05-08 05:38:59.000000 rally-4.1.0/.zuul.d/docker-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-05-08 05:38:59.000000 rally-4.1.0/.zuul.d/install-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2626 2024-05-08 05:38:59.000000 rally-4.1.0/.zuul.d/python-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2024-05-08 05:38:59.000000 rally-4.1.0/.zuul.d/zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17591 2024-05-08 05:39:26.000000 rally-4.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15873 2024-05-08 05:38:59.000000 rally-4.1.0/CHANGELOG.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2024-05-08 05:38:59.000000 rally-4.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   159589 2024-05-08 05:39:26.000000 rally-4.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3693 2024-05-08 05:38:59.000000 rally-4.1.0/DOCKER_README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2024-05-08 05:38:59.000000 rally-4.1.0/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10273 2024-05-08 05:38:59.000000 rally-4.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5947 2024-05-08 05:39:27.177061 rally-4.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4001 2024-05-08 05:38:59.000000 rally-4.1.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2024-05-08 05:38:59.000000 rally-4.1.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.029010 rally-4.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1292 2024-05-08 05:38:59.000000 rally-4.1.0/doc/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.029010 rally-4.1.0/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8055 2024-05-08 05:38:59.000000 rally-4.1.0/doc/ext/cli_reference.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2024-05-08 05:38:59.000000 rally-4.1.0/doc/ext/include_vars.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16313 2024-05-08 05:38:59.000000 rally-4.1.0/doc/ext/plugin_reference.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2024-05-08 05:38:59.000000 rally-4.1.0/doc/ext/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.033011 rally-4.1.0/doc/feature_request/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/capture_task_logging.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/check_queue_perfdata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/comparing_results_of_2_tasks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/distributed_load_generation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/explicitly_specify_existing_users_for_scenarios.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/historical_performance_data.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.033011 rally-4.1.0/doc/feature_request/implemented/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/implemented/LDAP_support.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/implemented/add_possibility_to_specify_concurrency_for_tempest.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2361 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/implemented/stop_scenario_after_several_errors.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/installation_script_enhancements.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/installing_isolated.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/launch_specific_benchmark.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/multi_scenarios_load_gen.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/multiple_attach_volume.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/persistence_benchmark_env.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2024-05-08 05:38:59.000000 rally-4.1.0/doc/feature_request/production_ready_cleanup.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.033011 rally-4.1.0/doc/release_notes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.041014 rally-4.1.0/doc/release_notes/archive/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.0.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5852 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.0.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3786 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.0.3.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7345 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.0.4.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13260 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.1.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.1.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6107 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.1.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22893 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.10.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.10.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10366 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.11.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2904 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.11.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2534 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.11.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3702 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.12.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.12.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4818 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.2.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5616 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.3.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.3.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.3.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.3.3.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8588 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.4.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13852 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.5.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7624 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.6.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5842 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.7.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10065 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.8.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.8.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5551 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.9.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.9.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v0.9.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive/v1.0.0.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/archive.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2024-05-08 05:38:59.000000 rally-4.1.0/doc/release_notes/latest.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-05-08 05:38:59.000000 rally-4.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.041014 rally-4.1.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6758 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/Makefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.005001 rally-4.1.0/doc/source/_templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.045015 rally-4.1.0/doc/source/_templates/openstackrally/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.045015 rally-4.1.0/doc/source/_templates/openstackrally/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/_templates/openstackrally/_static/img.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2429 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/_templates/openstackrally/layout.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       27 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/_templates/openstackrally/theme.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/cli_reference.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9577 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2296 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/contribute.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/feature_requests.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.061021 rally-4.1.0/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18652 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Amqp_rpc_single_reply_queue.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64751 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Hook-Aggregated-Report.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    88398 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Hook-Per-Hook-Report.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38695 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Hook-Results.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    95868 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Rally-Actions.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29546 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Rally-Plugins.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   127052 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Rally-UseCases.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   175620 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Rally_Architecture.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   168071 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Rally_Distributed_Runner.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   105436 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Rally_QA.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67056 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Rally_VM_list.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   116187 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Rally_snapshot_vm.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59267 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Rally_who_is_using.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   118771 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Abort-on-SLA-task-1.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   133861 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Abort-on-SLA-task-2.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   188455 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Collage.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48010 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Multiple-Configurations-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44839 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Multiple-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39473 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40004 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-SLA-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    73756 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-SLA-Scenario.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    76785 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Scenario-Atomic.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   111232 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Scenario-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20517 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Actions-durations.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24204 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Distribution.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77249 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Failures.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   103829 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Input-file.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8784 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Load-profile.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101257 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28224 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-SLA.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55099 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Scenario-Data-Aggregated.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25172 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration-profiler.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82653 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20731 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Subtask-configuration.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34215 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Task-Total-durations.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    74855 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Trends-Atomic-actions.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21142 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Trends-Configuration.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25032 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Trends-Overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    75196 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Trends-Total.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9812 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Trends-single-run.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81001 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Verify-filter-by-status.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    98165 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Verify-for-4-Verifications.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26831 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Verify-toggle-tags.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    84067 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Verify-tracebacks.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   134147 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/images/Report-Verify-xfail.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.061021 rally-4.1.0/doc/source/install_and_upgrade/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/install_and_upgrade/db_migrations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/install_and_upgrade/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1390 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/install_and_upgrade/install.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.061021 rally-4.1.0/doc/source/overview/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4941 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/overview/glossary.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/overview/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6449 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/overview/overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/overview/user_stories.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.061021 rally-4.1.0/doc/source/plugins/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.061021 rally-4.1.0/doc/source/plugins/implementation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4729 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/plugins/implementation/context_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11825 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/plugins/implementation/hook_and_trigger_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/plugins/implementation/runner_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/plugins/implementation/scenario_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/plugins/implementation/sla_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2615 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/plugins/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/plugins/plugin_reference.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.065022 rally-4.1.0/doc/source/project_info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9725 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/project_info/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/project_info/release_notes.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.065022 rally-4.1.0/doc/source/quick_start/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5535 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/gates.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.065022 rally-4.1.0/doc/source/quick_start/tutorial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2778 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_10_profiling_openstack_internals.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13823 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_1_setting_up_env_and_running_benchmark_from_samples.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9129 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_2_input_task_format.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5211 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_3_benchmarking_with_existing_users.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5731 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_4_adding_success_criteria_for_benchmarks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10059 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_5_task_templates.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6075 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_6_aborting_load_generation_on_sla_failure.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8178 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_7_working_with_multple_openstack_clouds.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8103 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_8_discovering_more_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45288 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial/step_9_verifying_cloud_via_tempest_verifier.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/quick_start/tutorial.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.065022 rally-4.1.0/doc/source/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10006 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/task/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.069023 rally-4.1.0/doc/source/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/verification/cli_reference.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.069023 rally-4.1.0/doc/source/verification/howto/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3773 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/verification/howto/add_new_reporter.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4453 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/verification/howto/add_support_for_new_tool.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/verification/howto/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16640 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/verification/howto/migrate_from_old_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/verification/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3075 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/verification/overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4254 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/verification/reports.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3626 2024-05-08 05:38:59.000000 rally-4.1.0/doc/source/verification/verifiers.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.069023 rally-4.1.0/doc/specs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.073025 rally-4.1.0/doc/specs/implemented/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2713 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/class-based-scenarios.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4492 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/consistent_resource_names.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10835 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/db_refactoring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6472 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/deployment_type.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7816 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/hook_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/improve_atomic_actions_format.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11368 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/improve_scenario_output_format.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10567 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/new_rally_input_task_format.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/osprofiler.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/pluggable_validators.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1466 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/sla_pd_plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1679 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/split_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3017 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/task_and_verification_export.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30381 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/implemented/verification_refactoring.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.073025 rally-4.1.0/doc/specs/in-progress/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/in-progress/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7564 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/in-progress/cleanup_refactoring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5158 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/in-progress/distributed_runner.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11197 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/in-progress/pluggable-types.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11188 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/in-progress/raas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11465 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/in-progress/refactor_scenario_utils.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2024-05-08 05:38:59.000000 rally-4.1.0/doc/specs/template.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.009003 rally-4.1.0/doc/user_stories/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.073025 rally-4.1.0/doc/user_stories/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6391 2024-05-08 05:38:59.000000 rally-4.1.0/doc/user_stories/keystone/authenticate.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.073025 rally-4.1.0/doc/user_stories/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8685 2024-05-08 05:38:59.000000 rally-4.1.0/doc/user_stories/nova/boot_server.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.077026 rally-4.1.0/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2024-05-08 05:38:59.000000 rally-4.1.0/etc/motd_for_docker
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.077026 rally-4.1.0/etc/rally/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-05-08 05:38:59.000000 rally-4.1.0/etc/rally/rally-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11258 2024-05-08 05:38:59.000000 rally-4.1.0/etc/rally/rally.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4643 2024-05-08 05:38:59.000000 rally-4.1.0/etc/rally.bash_completion
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.077026 rally-4.1.0/rally/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.081028 rally-4.1.0/rally/aas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-05-08 05:38:59.000000 rally-4.1.0/rally/aas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    54948 2024-05-08 05:38:59.000000 rally-4.1.0/rally/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.081028 rally-4.1.0/rally/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27181 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/cliutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.085029 rally-4.1.0/rally/cli/commands/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/commands/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/commands/db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15083 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/commands/deployment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13986 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/commands/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4609 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/commands/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37124 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/commands/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40419 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/commands/verify.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6286 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/envutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9054 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/task_results_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2024-05-08 05:38:59.000000 rally-4.1.0/rally/cli/yamlutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.085029 rally-4.1.0/rally/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2699 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/broker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/cfg.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.089030 rally-4.1.0/rally/common/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24418 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.089030 rally-4.1.0/rally/common/db/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.093032 rally-4.1.0/rally/common/db/migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7920 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_01_ca3626f62937_init_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_03_3177d36ea270_merge_credentials_from_users_and_admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5678 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_04_4ef544102ba7_change_task_status_enum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15421 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_04_e654a0648db0_refactor_task_results.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2938 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_07_54e844ebfbc3_update_deployment_configs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_08_32fada9b2fde_remove_admin_domain_name.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3700 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_09_08e1515a576c_fix_invalid_verification_logs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_09_6ad4f426f005_add_hooks_to_task_result.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7712 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_11_484cd9413e66_new_db_schema_for_verification_component.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2016_12_37fdbb373e8d_fix_test_results_for_verifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_01_a6f364988fc2_change_tag_type_enum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_01_f33f4610dcda_change_verification_statuses.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_02_92aaaa2a6bb3_refactor_credentials.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3450 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_06_35fe16d4ab1c_update_tasks_based_on_workloads.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_06_c517b0011857_fill_missed_workload_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2642 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_07_7948b83229f6_workload_min_max_durations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_08_fab4f4f31f8a_fill_missed_workload_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_09_046a38742e89_port_configs_to_new_formats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_09_e0a5df2c5153_upsize_the_size_of_task_title.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5031 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_10_4394bdc32cfd_fill_missed_workload_info_r3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_10_9a18c6fe265c_rename_namespace_to_platform.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8561 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_10_dc46687661df_update_contexts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2017_12_a43700a813a5_add_env_platforms_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2018_01_44169f4d455e_deleted_worker_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2018_01_7287df262dbc_move_deployment_to_env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2018_02_95208e4eface_add_config_field_to_env_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7912 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2018_02_bc908ac9a1fc_move_deployment_to_env_2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/migrations/versions/2018_02_dc0fe6de6786_update_old_deployment_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11932 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5325 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/sa_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5099 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/db/schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/fileutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.097033 rally-4.1.0/rally/common/io/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/io/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5509 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/io/junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9452 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/io/subunit_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11272 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/logging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.097033 rally-4.1.0/rally/common/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6637 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/objects/deploy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24513 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/objects/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3248 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/objects/verification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/objects/verifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.097033 rally-4.1.0/rally/common/plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5846 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/plugin/discover.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4372 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/plugin/info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4549 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/plugin/meta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7390 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/plugin/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/sshutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7808 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/streaming_algorithms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26149 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10594 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-05-08 05:38:59.000000 rally-4.1.0/rally/common/yamlutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6911 2024-05-08 05:38:59.000000 rally-4.1.0/rally/consts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.097033 rally-4.1.0/rally/env/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/env/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25830 2024-05-08 05:38:59.000000 rally-4.1.0/rally/env/env_mgr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3978 2024-05-08 05:38:59.000000 rally-4.1.0/rally/env/platform.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6680 2024-05-08 05:38:59.000000 rally-4.1.0/rally/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.097033 rally-4.1.0/rally/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.101034 rally-4.1.0/rally/plugins/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.101034 rally-4.1.0/rally/plugins/common/exporters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/exporters/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.101034 rally-4.1.0/rally/plugins/common/exporters/elastic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/exporters/elastic/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      936 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/exporters/elastic/client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      940 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/exporters/elastic/exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/exporters/elastic/flatten.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/exporters/html.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/exporters/json_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/exporters/junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/exporters/trends.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.101034 rally-4.1.0/rally/plugins/common/hook/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/hook/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/hook/sys_call.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.101034 rally-4.1.0/rally/plugins/common/hook/triggers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/hook/triggers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/hook/triggers/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/hook/triggers/periodic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.105036 rally-4.1.0/rally/plugins/common/runners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/runners/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/runners/constant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/runners/rps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/runners/serial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.105036 rally-4.1.0/rally/plugins/common/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/scenarios/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.105036 rally-4.1.0/rally/plugins/common/scenarios/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/scenarios/dummy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/scenarios/dummy/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.105036 rally-4.1.0/rally/plugins/common/scenarios/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/scenarios/requests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/scenarios/requests/http_requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/scenarios/requests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.105036 rally-4.1.0/rally/plugins/common/sla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/sla/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/sla/failure_rate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/sla/iteration_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/sla/max_average_duration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/sla/max_average_duration_per_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/sla/outliers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/sla/performance_degradation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17661 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.105036 rally-4.1.0/rally/plugins/common/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/verification/reporters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/common/verification/testr.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.109037 rally-4.1.0/rally/plugins/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.109037 rally-4.1.0/rally/plugins/task/contexts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/contexts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/contexts/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.109037 rally-4.1.0/rally/plugins/task/exporters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.109037 rally-4.1.0/rally/plugins/task/exporters/elastic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/elastic/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6196 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/elastic/client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16360 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/elastic/exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/elastic/flatten.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/html.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5596 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/json_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3560 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4587 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/old_json_results.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1406 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/exporters/trends.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.109037 rally-4.1.0/rally/plugins/task/hook_triggers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/hook_triggers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/hook_triggers/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2702 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/hook_triggers/periodic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.113039 rally-4.1.0/rally/plugins/task/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/hooks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2562 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/hooks/sys_call.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.113039 rally-4.1.0/rally/plugins/task/runners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/runners/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14074 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/runners/constant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11593 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/runners/rps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3062 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/runners/serial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.113039 rally-4.1.0/rally/plugins/task/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/scenarios/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.113039 rally-4.1.0/rally/plugins/task/scenarios/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/scenarios/dummy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11367 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/scenarios/dummy/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.113039 rally-4.1.0/rally/plugins/task/scenarios/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/scenarios/requests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/scenarios/requests/http_requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1566 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/scenarios/requests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.117040 rally-4.1.0/rally/plugins/task/sla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/sla/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/sla/failure_rate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/sla/iteration_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/sla/max_average_duration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3150 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/sla/max_average_duration_per_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4536 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/sla/outliers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/sla/performance_degradation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/task/types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.117040 rally-4.1.0/rally/plugins/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18676 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/verification/reporters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5791 2024-05-08 05:38:59.000000 rally-4.1.0/rally/plugins/verification/testr.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.121041 rally-4.1.0/rally/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4535 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11493 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21517 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/engine.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3544 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7062 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/functional.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8619 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/hook.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.121041 rally-4.1.0/rally/task/processing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/processing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35112 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/processing/charts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16819 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/processing/plot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3080 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/processing/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9895 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/runner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7474 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/scenario.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14956 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6007 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/sla.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15607 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/task_cfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8847 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15050 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2024-05-08 05:38:59.000000 rally-4.1.0/rally/task/validation.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.121041 rally-4.1.0/rally/ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.121041 rally-4.1.0/rally/ui/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2802 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/base.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.121041 rally-4.1.0/rally/ui/templates/ci/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3886 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/ci/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2138 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/ci/index_verify.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.121041 rally-4.1.0/rally/ui/templates/libs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/libs/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   124229 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/libs/angular.1.3.3.min.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   148039 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/libs/d3.3.4.13.min.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8796 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   188436 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.125043 rally-4.1.0/rally/ui/templates/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10234 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/task/directive_widget.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31337 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/task/report.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17746 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/task/trends.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.125043 rally-4.1.0/rally/ui/templates/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12229 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/templates/verification/report.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2024-05-08 05:38:59.000000 rally-4.1.0/rally/ui/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.125043 rally-4.1.0/rally/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3532 2024-05-08 05:38:59.000000 rally-4.1.0/rally/utils/encodeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10988 2024-05-08 05:38:59.000000 rally-4.1.0/rally/utils/sshutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2024-05-08 05:38:59.000000 rally-4.1.0/rally/utils/strutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.125043 rally-4.1.0/rally/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2024-05-08 05:38:59.000000 rally-4.1.0/rally/verification/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16784 2024-05-08 05:38:59.000000 rally-4.1.0/rally/verification/manager.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3035 2024-05-08 05:38:59.000000 rally-4.1.0/rally/verification/reporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3055 2024-05-08 05:38:59.000000 rally-4.1.0/rally/verification/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.077026 rally-4.1.0/rally-jobs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.077026 rally-4.1.0/rally-jobs/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2024-05-08 05:38:59.000000 rally-4.1.0/rally-jobs/plugins/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally-jobs/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2024-05-08 05:38:59.000000 rally-4.1.0/rally-jobs/plugins/fake_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2024-05-08 05:38:59.000000 rally-4.1.0/rally-jobs/plugins/rally_profile.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.077026 rally-4.1.0/rally-jobs/plugins/test_relative_import/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/rally-jobs/plugins/test_relative_import/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2024-05-08 05:38:59.000000 rally-4.1.0/rally-jobs/plugins/test_relative_import/zzz.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11899 2024-05-08 05:38:59.000000 rally-4.1.0/rally-jobs/self-rally.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.081028 rally-4.1.0/rally.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5947 2024-05-08 05:39:26.000000 rally-4.1.0/rally.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25799 2024-05-08 05:39:27.000000 rally-4.1.0/rally.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-08 05:39:26.000000 rally-4.1.0/rally.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-05-08 05:39:26.000000 rally-4.1.0/rally.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-08 05:39:26.000000 rally-4.1.0/rally.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-05-08 05:39:26.000000 rally-4.1.0/rally.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2024-05-08 05:39:26.000000 rally-4.1.0/rally.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2024-05-08 05:39:26.000000 rally-4.1.0/rally.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1496 2024-05-08 05:38:59.000000 rally-4.1.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.125043 rally-4.1.0/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-05-08 05:38:59.000000 rally-4.1.0/samples/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.125043 rally-4.1.0/samples/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.129044 rally-4.1.0/samples/tasks/contexts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/contexts/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/contexts/dummy-context.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/contexts/dummy-context.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.129044 rally-4.1.0/samples/tasks/runners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/runners/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.129044 rally-4.1.0/samples/tasks/runners/constant/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/runners/constant/constant-for-duration.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/runners/constant/constant-for-duration.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/runners/constant/constant-timeout.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/runners/constant/constant-timeout.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.129044 rally-4.1.0/samples/tasks/runners/rps/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/runners/rps/rps.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/runners/rps/rps.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.129044 rally-4.1.0/samples/tasks/runners/serial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/runners/serial/serial.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/runners/serial/serial.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.129044 rally-4.1.0/samples/tasks/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.133046 rally-4.1.0/samples/tasks/scenarios/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-exception-probability.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-exception-probability.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-exception.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-exception.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-failure.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-failure.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-output.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-output.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-random-action.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-random-action.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-random-fail-in-atomic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy-timed-atomic-actions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/dummy/dummy.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.133046 rally-4.1.0/samples/tasks/scenarios/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/requests/check-random-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/requests/check-random-request.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/requests/check-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/scenarios/requests/check-request.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.133046 rally-4.1.0/samples/tasks/sla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/sla/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/sla/dummy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-05-08 05:38:59.000000 rally-4.1.0/samples/tasks/sla/dummy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-05-08 05:39:27.177061 rally-4.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2024-05-08 05:38:59.000000 rally-4.1.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1059 2024-05-08 05:38:59.000000 rally-4.1.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.137047 rally-4.1.0/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2355 2024-05-08 05:38:59.000000 rally-4.1.0/tests/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.137047 rally-4.1.0/tests/ci/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2323 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/cover.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.137047 rally-4.1.0/tests/ci/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/docker-build-and-check.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/docker-build-check-and-push.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/rally-install-pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/rally-install-run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.017006 rally-4.1.0/tests/ci/playbooks/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.017006 rally-4.1.0/tests/ci/playbooks/roles/docker-build-image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.137047 rally-4.1.0/tests/ci/playbooks/roles/docker-build-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/roles/docker-build-image/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.137047 rally-4.1.0/tests/ci/playbooks/roles/docker-build-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.017006 rally-4.1.0/tests/ci/playbooks/roles/docker-push-image/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.141048 rally-4.1.0/tests/ci/playbooks/roles/docker-push-image/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/roles/docker-push-image/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.141048 rally-4.1.0/tests/ci/playbooks/roles/docker-push-image/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.017006 rally-4.1.0/tests/ci/playbooks/roles/rally-tox/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.141048 rally-4.1.0/tests/ci/playbooks/roles/rally-tox/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/roles/rally-tox/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.141048 rally-4.1.0/tests/ci/playbooks/roles/rally-tox/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/roles/rally-tox/files/find_python_for_tox_env.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.141048 rally-4.1.0/tests/ci/playbooks/roles/rally-tox/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/roles/rally-tox/tasks/install.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/roles/rally-tox/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/roles/rally-tox/tasks/run.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/tox-install.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/playbooks/tox-run.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3993 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/pytest_launcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/rally_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4012 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/rally_self_job.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/render.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13962 2024-05-08 05:38:59.000000 rally-4.1.0/tests/ci/sync_requirements.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.141048 rally-4.1.0/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.145050 rally-4.1.0/tests/functional/extra/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.145050 rally-4.1.0/tests/functional/extra/fake_dir1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/extra/fake_dir1/fake_plugin1.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.145050 rally-4.1.0/tests/functional/extra/fake_dir2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/extra/fake_dir2/fake_plugin2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/extra/fake_platforms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2044 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/extra/fake_verify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/extra/test_fake_scenario.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1299 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/test_cli_deployment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3213 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/test_cli_env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/test_cli_functional.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2799 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/test_cli_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57886 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/test_cli_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/test_cli_verify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/test_lib_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7839 2024-05-08 05:38:59.000000 rally-4.1.0/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.145050 rally-4.1.0/tests/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20461 2024-05-08 05:38:59.000000 rally-4.1.0/tests/hacking/checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.145050 rally-4.1.0/tests/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/samples/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7006 2024-05-08 05:38:59.000000 rally-4.1.0/tests/samples/test_task_samples.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.149051 rally-4.1.0/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.149051 rally-4.1.0/tests/unit/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.149051 rally-4.1.0/tests/unit/cli/commands/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/commands/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/commands/test_db.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    23141 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/commands/test_deployment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/commands/test_docstrings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21802 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/commands/test_env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/commands/test_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50080 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/commands/test_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36667 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/commands/test_verify.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37060 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/test_cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5589 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/test_envutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9219 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/test_task_results_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/cli/test_yamlutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.153052 rally-4.1.0/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.153052 rally-4.1.0/tests/unit/common/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38662 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/db/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   112349 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/db/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5646 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/db/test_migrations_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5995 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/db/test_types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.153052 rally-4.1.0/tests/unit/common/io/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/io/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3470 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/io/subunit_v2.stream
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2334 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/io/test_junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5861 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/io/test_subunit_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.157054 rally-4.1.0/tests/unit/common/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8664 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/objects/test_deploy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26718 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/objects/test_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6230 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/objects/test_verification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/objects/test_verifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.157054 rally-4.1.0/tests/unit/common/plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/plugin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9817 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/plugin/test_discover.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4208 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/plugin/test_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5204 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/plugin/test_meta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8028 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/plugin/test_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2822 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/test_broker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12226 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/test_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1570 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/test_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10136 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/test_streaming_algorithms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27261 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6137 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/test_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/common/test_version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.157054 rally-4.1.0/tests/unit/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/doc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/doc/test_docker_readme.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6020 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/doc/test_docstrings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3086 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/doc/test_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8647 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/doc/test_jsonschemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4530 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/doc/test_specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/doc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.161055 rally-4.1.0/tests/unit/env/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/env/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31964 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/env/test_env_mgr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/env/test_platform.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4637 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.161055 rally-4.1.0/tests/unit/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.161055 rally-4.1.0/tests/unit/plugins/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18275 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/common/test_validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.161055 rally-4.1.0/tests/unit/plugins/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.161055 rally-4.1.0/tests/unit/plugins/task/contexts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/contexts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/contexts/test_dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.161055 rally-4.1.0/tests/unit/plugins/task/exporters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4766 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/dummy_data.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.165057 rally-4.1.0/tests/unit/plugins/task/exporters/elastic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/elastic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8347 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/elastic/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20745 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/elastic/test_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/elastic/test_flatten.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/junit_report.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/test_html.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5144 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/test_json_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/test_junit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5414 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/test_old_json_results.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/exporters/test_trends.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.165057 rally-4.1.0/tests/unit/plugins/task/hook_triggers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/hook_triggers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2774 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/hook_triggers/test_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3498 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/hook_triggers/test_periodic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.165057 rally-4.1.0/tests/unit/plugins/task/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/hooks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5058 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/hooks/test_sys_call.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.165057 rally-4.1.0/tests/unit/plugins/task/runners/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/runners/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13700 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/runners/test_constant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13675 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/runners/test_rps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2937 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/runners/test_serial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.165057 rally-4.1.0/tests/unit/plugins/task/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/scenarios/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.165057 rally-4.1.0/tests/unit/plugins/task/scenarios/dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/scenarios/dummy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9988 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/scenarios/dummy/test_dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.169058 rally-4.1.0/tests/unit/plugins/task/scenarios/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/scenarios/requests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/scenarios/requests/test_http_requests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/scenarios/requests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.169058 rally-4.1.0/tests/unit/plugins/task/sla/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/sla/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4983 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/sla/test_failure_rate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/sla/test_iteration_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3181 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/sla/test_max_average_duration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5397 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/sla/test_max_average_duration_per_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5363 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/sla/test_outliers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3428 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/sla/test_performance_degradation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3558 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/task/test_types.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.169058 rally-4.1.0/tests/unit/plugins/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/verification/junit_report.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18394 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/verification/test_reporters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17452 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/plugins/verification/test_testr.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.173059 rally-4.1.0/tests/unit/task/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.173059 rally-4.1.0/tests/unit/task/processing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/processing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47254 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/processing/test_charts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33744 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/processing/test_plot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4654 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/processing/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4935 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13920 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43094 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3213 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9339 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_functional.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13184 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_hook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9213 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_runner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6440 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_scenario.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9279 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6932 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_sla.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11894 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_task_cfg.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5377 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23353 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/task/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4159 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90112 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test_ddt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14649 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12518 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test_mock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2569 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test_pytest_launcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test_test_ddt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14129 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/test_test_mock.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.173059 rally-4.1.0/tests/unit/ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/ui/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/ui/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.177061 rally-4.1.0/tests/unit/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/utils/test_encodeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14089 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/utils/test_sshutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7744 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/utils/test_strutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:39:27.177061 rally-4.1.0/tests/unit/verification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/verification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/verification/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15834 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/verification/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3241 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/verification/test_reporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3837 2024-05-08 05:38:59.000000 rally-4.1.0/tests/unit/verification/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5070 2024-05-08 05:38:59.000000 rally-4.1.0/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2024-05-08 05:38:59.000000 rally-4.1.0/upper-constraints.txt
```

### Comparing `rally-4.0.0/.zuul.d/docker-jobs.yaml` & `rally-4.1.0/.zuul.d/docker-jobs.yaml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/.zuul.d/install-jobs.yaml` & `rally-4.1.0/.zuul.d/install-jobs.yaml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/.zuul.d/python-jobs.yaml` & `rally-4.1.0/.zuul.d/python-jobs.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -87,14 +87,26 @@
       Run unit test for rally project.
 
       Uses tox with the ``py311`` environment.
     vars:
       tox_env: py311
 
 - job:
+    name: rally-tox-py311-sqlalchemy14
+    parent: rally-tox-py311
+    vars:
+      tox_env: py311-sa14
+
+- job:
+    name: rally-tox-py311-sqlalchemy2
+    parent: rally-tox-py311
+    vars:
+      tox_env: py311-sa2
+
+- job:
     name: rally-tox-samples
     parent: rally-tox-base
     description: |
       Run unit test for rally project.
 
       Uses tox with the ``samples`` environment.
     vars:
```

### Comparing `rally-4.0.0/.zuul.d/zuul.yaml` & `rally-4.1.0/.zuul.d/zuul.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,16 @@
       jobs:
         - rally-tox-cover
         - rally-tox-docs
         - rally-tox-pep8
         - rally-tox-py38
         - rally-tox-py39
         - rally-tox-py310
-        - rally-tox-py311
+        - rally-tox-py311-sqlalchemy14
+        - rally-tox-py311-sqlalchemy2
         - rally-tox-samples
         - rally-tox-functional
         - rally-tox-self
         - rally-install-ubuntu-focal
         - rally-install-ubuntu-jammy
         - rally-install-centos-8s
         - rally-install-centos-9s
@@ -25,15 +26,16 @@
       jobs:
         - rally-tox-cover
         - rally-tox-docs
         - rally-tox-pep8
         - rally-tox-py38
         - rally-tox-py39
         - rally-tox-py310
-        - rally-tox-py311
+        - rally-tox-py311-sqlalchemy14
+        - rally-tox-py311-sqlalchemy2
         - rally-tox-functional
         - rally-tox-self
         - rally-install-ubuntu-focal
         - rally-install-ubuntu-jammy
         - rally-install-centos-8s
         - rally-install-centos-9s
     post:
```

### Comparing `rally-4.0.0/AUTHORS` & `rally-4.1.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 Andreas Jaeger <aj@suse.com>
 Andrew F. Ly <afly@us.ibm.com>
 Andrew McDermott <andrew.mcdermott@linaro.org>
 Andrey <agrebennikov@mirantis.com>
 Andrey Kurilin <akurilin@mirantis.com>
 Andrey Kurilin <andr.kurilin@gmail.com>
 Andrey Pavlov <andrey.mp@gmail.com>
+Andriy Kurilin <andr.kurilin@gmail.com>
 Andy Botting <andy@andybotting.com>
 Angus Lees <gus@inodes.org>
 Anh Tran <anhtt@vn.fujitsu.com>
 Anthony Lee <anthony.mic.lee@hp.com>
 Anthony Washington <anthony.washington@intel.com>
 Anton Arefiev <aarefiev@mirantis.com>
 Anton Frolov <frolov.anton@gmail.com>
```

### Comparing `rally-4.0.0/CHANGELOG.rst` & `rally-4.1.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,28 @@
     - **Deprecated** for soon-to-be removed features/plugins.
     - **Removed** for now removed features/plugins.
     - **Fixed** for any bug fixes.
 
 .. Release notes for existing releases are MUTABLE! If there is something that
    was missed or can be improved, feel free to change it!
 
+[4.1.0] - 2024-04-29
+--------------------
+
+Changed
+~~~~~~~
+
+* Add support for SQLAlchemy 2.0
+
+Fixed
+~~~~~
+
+* Correct `python_requires` version to indicate correct minimum supported
+  python version
+
 [4.0.0] - 2024-01-10
 --------------------
 
 Fixed
 ~~~~~
 
 * Parsing subunit v2 stream (rally-verify component) when the result is
```

### Comparing `rally-4.0.0/CONTRIBUTING.rst` & `rally-4.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/ChangeLog` & `rally-4.1.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+4.1.0
+-----
+
+* Propose 4.1.0 release
+* Remove redundant db ignore warnings
+* Use unittest.TestCase instead of testtools.TestCase
+* Add support for SQLAlchemy 2.0
+* Revert "Remove usage of LegacyEngineFacade"
+* Update u-c file
+* Remove usage of LegacyEngineFacade
+
 4.0.0
 -----
 
 * Rename 3.5.0 release to 4.0.0
 * Update release notes for rally 3.5.0
 * use draft-7 jsonschema validator
 * Improve required\_context validator to support platforms
```

### Comparing `rally-4.0.0/DOCKER_README.md` & `rally-4.1.0/DOCKER_README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # What is Rally/xRally
 
 Rally is tool & framework that allows one to write simple plugins and combine
 them in complex tests scenarios that allows to perform all kinds of testing!
 
 # The purpose of xrally image or how to use it
 
-**xrally** image bases on the official python3.9-slim docker image.
+**xrally** image bases on the official python3.11-slim docker image.
 It provides raw xrally framework with only in-tree plugins (no
 pre-installed plugins for Kubernetes, OpenStack, etc).
 
 You can use this image as a base image and extend it with installation of
 additional plugins:
 
     # It is an example of Dockerfile for xrally/xrally_docker image. There are
     #   only 2 critical lines: `FROM instruction` and the last line is a check
     #   for rally user is used.
     #
     # Tags of the image are the same as releases of xRally/Rally
-    FROM xrally/xrally:4.0.0
+    FROM xrally/xrally:4.1.0
     
     # "rally" user (which is selected by-default) is owner of "/rally" directory,
     #   so there is no need to call chown or switch the user
     COPY . /rally/xrally_docker
     WORKDIR /rally/xrally_docker
     
     # to install package system-wide, we need to temporary switch to root user
@@ -36,16 +36,16 @@
 details)
 
 # How to run xrally container
 
 First, you need to pull the container. We suggest using the last tagged 
 version:
 
-    # pull the 4.0.0 image (the latest release at the point of writing the note)
-    $ docker pull xrally/xrally:4.0.0
+    # pull the 4.1.0 image (the latest release at the point of writing the note)
+    $ docker pull xrally/xrally:4.1.0
 
 **WARNING: never attach folders and volumes to `/rally` inside the container. It can break everything.**
 
 The default configuration file is located at `/etc/rally/rally.conf`. You
 should not be aware of it. If you want to override some options, use
 `/home/rally/.rally/rally.conf` location instead. Rally does not load all
 configuration files, so the primary one will be used.
@@ -53,15 +53,15 @@
 The default place for rally database file is `/home/rally/.rally/rally.sqlite`.
 To make the storage persistent across all container runs, you may want to use
 docker volumes or mount the directory.
 
 * use docker volumes. It is the easiest way. You just need to do something like:
 
       $ docker volume create --name rally_volume
-      $ docker run -v rally_volume:/home/rally/.rally xrally/xrally:4.0.0 env create --name "foo"
+      $ docker run -v rally_volume:/home/rally/.rally xrally/xrally:4.1.0 env create --name "foo"
 
 
 * mount outer directory inside the container
 
       # you can create directory in whatever you want to place, but you
       # may wish to make the data available for all users
       $ sudo mkdir /var/lib/rally_container
```

### Comparing `rally-4.0.0/Dockerfile` & `rally-4.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/LICENSE` & `rally-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/PKG-INFO` & `rally-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rally
-Version: 4.0.0
+Version: 4.1.0
 Summary: Generic Testing Framework & Tool that unifies all types of testing.
 Home-page: https://rally.readthedocs.io/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: =====
         Rally
@@ -132,11 +132,11 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: test
```

### Comparing `rally-4.0.0/README.rst` & `rally-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/bindep.txt` & `rally-4.1.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/README.rst` & `rally-4.1.0/doc/README.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/ext/cli_reference.py` & `rally-4.1.0/doc/ext/cli_reference.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/ext/include_vars.py` & `rally-4.1.0/doc/ext/include_vars.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/ext/plugin_reference.py` & `rally-4.1.0/doc/ext/plugin_reference.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/ext/utils.py` & `rally-4.1.0/doc/ext/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/check_queue_perfdata.rst` & `rally-4.1.0/doc/feature_request/check_queue_perfdata.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/explicitly_specify_existing_users_for_scenarios.rst` & `rally-4.1.0/doc/feature_request/explicitly_specify_existing_users_for_scenarios.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/historical_performance_data.rst` & `rally-4.1.0/doc/feature_request/historical_performance_data.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/implemented/LDAP_support.rst` & `rally-4.1.0/doc/feature_request/implemented/LDAP_support.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/implemented/add_possibility_to_specify_concurrency_for_tempest.rst` & `rally-4.1.0/doc/feature_request/implemented/add_possibility_to_specify_concurrency_for_tempest.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/implemented/stop_scenario_after_several_errors.rst` & `rally-4.1.0/doc/feature_request/implemented/stop_scenario_after_several_errors.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/installation_script_enhancements.rst` & `rally-4.1.0/doc/feature_request/installation_script_enhancements.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/installing_isolated.rst` & `rally-4.1.0/doc/feature_request/installing_isolated.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/launch_specific_benchmark.rst` & `rally-4.1.0/doc/feature_request/launch_specific_benchmark.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/multi_scenarios_load_gen.rst` & `rally-4.1.0/doc/feature_request/multi_scenarios_load_gen.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/persistence_benchmark_env.rst` & `rally-4.1.0/doc/feature_request/persistence_benchmark_env.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/feature_request/production_ready_cleanup.rst` & `rally-4.1.0/doc/feature_request/production_ready_cleanup.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.0.1.rst` & `rally-4.1.0/doc/release_notes/archive/v0.0.1.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.0.2.rst` & `rally-4.1.0/doc/release_notes/archive/v0.0.2.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.0.3.rst` & `rally-4.1.0/doc/release_notes/archive/v0.0.3.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.0.4.rst` & `rally-4.1.0/doc/release_notes/archive/v0.0.4.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.1.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.1.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.1.1.rst` & `rally-4.1.0/doc/release_notes/archive/v0.1.1.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.1.2.rst` & `rally-4.1.0/doc/release_notes/archive/v0.1.2.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.10.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.10.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.10.1.rst` & `rally-4.1.0/doc/release_notes/archive/v0.10.1.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.11.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.11.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.11.1.rst` & `rally-4.1.0/doc/release_notes/archive/v0.11.1.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.11.2.rst` & `rally-4.1.0/doc/release_notes/archive/v0.11.2.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.12.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.12.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.12.1.rst` & `rally-4.1.0/doc/release_notes/archive/v0.12.1.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.2.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.2.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.3.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.3.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.3.1.rst` & `rally-4.1.0/doc/release_notes/archive/v0.3.1.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.3.2.rst` & `rally-4.1.0/doc/release_notes/archive/v0.3.2.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.3.3.rst` & `rally-4.1.0/doc/release_notes/archive/v0.3.3.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.4.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.4.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.5.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.5.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.6.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.6.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.7.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.7.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.8.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.8.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.8.1.rst` & `rally-4.1.0/doc/release_notes/archive/v0.8.1.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.9.0.rst` & `rally-4.1.0/doc/release_notes/archive/v0.9.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.9.1.rst` & `rally-4.1.0/doc/release_notes/archive/v0.9.1.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v0.9.2.rst` & `rally-4.1.0/doc/release_notes/archive/v0.9.2.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/archive/v1.0.0.rst` & `rally-4.1.0/doc/release_notes/archive/v1.0.0.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/release_notes/latest.rst` & `rally-4.1.0/doc/release_notes/latest.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/Makefile` & `rally-4.1.0/doc/source/Makefile`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/_templates/openstackrally/layout.html` & `rally-4.1.0/doc/source/_templates/openstackrally/layout.html`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/conf.py` & `rally-4.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/contribute.rst` & `rally-4.1.0/doc/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/feature_requests.rst` & `rally-4.1.0/doc/source/feature_requests.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Amqp_rpc_single_reply_queue.png` & `rally-4.1.0/doc/source/images/Amqp_rpc_single_reply_queue.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Hook-Aggregated-Report.png` & `rally-4.1.0/doc/source/images/Hook-Aggregated-Report.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Hook-Per-Hook-Report.png` & `rally-4.1.0/doc/source/images/Hook-Per-Hook-Report.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Hook-Results.png` & `rally-4.1.0/doc/source/images/Hook-Results.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Rally-Actions.png` & `rally-4.1.0/doc/source/images/Rally-Actions.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Rally-Plugins.png` & `rally-4.1.0/doc/source/images/Rally-Plugins.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Rally-UseCases.png` & `rally-4.1.0/doc/source/images/Rally-UseCases.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Rally_Architecture.png` & `rally-4.1.0/doc/source/images/Rally_Architecture.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Rally_Distributed_Runner.png` & `rally-4.1.0/doc/source/images/Rally_Distributed_Runner.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Rally_QA.png` & `rally-4.1.0/doc/source/images/Rally_QA.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Rally_VM_list.png` & `rally-4.1.0/doc/source/images/Rally_VM_list.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Rally_snapshot_vm.png` & `rally-4.1.0/doc/source/images/Rally_snapshot_vm.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Rally_who_is_using.png` & `rally-4.1.0/doc/source/images/Rally_who_is_using.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Abort-on-SLA-task-1.png` & `rally-4.1.0/doc/source/images/Report-Abort-on-SLA-task-1.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Abort-on-SLA-task-2.png` & `rally-4.1.0/doc/source/images/Report-Abort-on-SLA-task-2.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Collage.png` & `rally-4.1.0/doc/source/images/Report-Collage.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Multiple-Configurations-Overview.png` & `rally-4.1.0/doc/source/images/Report-Multiple-Configurations-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Multiple-Overview.png` & `rally-4.1.0/doc/source/images/Report-Multiple-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Overview.png` & `rally-4.1.0/doc/source/images/Report-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-SLA-Overview.png` & `rally-4.1.0/doc/source/images/Report-SLA-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-SLA-Scenario.png` & `rally-4.1.0/doc/source/images/Report-SLA-Scenario.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Scenario-Atomic.png` & `rally-4.1.0/doc/source/images/Report-Scenario-Atomic.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Scenario-Overview.png` & `rally-4.1.0/doc/source/images/Report-Scenario-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Actions-durations.png` & `rally-4.1.0/doc/source/images/Report-Task-Actions-durations.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Distribution.png` & `rally-4.1.0/doc/source/images/Report-Task-Distribution.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Failures.png` & `rally-4.1.0/doc/source/images/Report-Task-Failures.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Input-file.png` & `rally-4.1.0/doc/source/images/Report-Task-Input-file.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Load-profile.png` & `rally-4.1.0/doc/source/images/Report-Task-Load-profile.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Overview.png` & `rally-4.1.0/doc/source/images/Report-Task-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-SLA.png` & `rally-4.1.0/doc/source/images/Report-Task-SLA.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Scenario-Data-Aggregated.png` & `rally-4.1.0/doc/source/images/Report-Task-Scenario-Data-Aggregated.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration-profiler.png` & `rally-4.1.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration-profiler.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration.png` & `rally-4.1.0/doc/source/images/Report-Task-Scenario-Data-Per-iteration.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Subtask-configuration.png` & `rally-4.1.0/doc/source/images/Report-Task-Subtask-configuration.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Task-Total-durations.png` & `rally-4.1.0/doc/source/images/Report-Task-Total-durations.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Trends-Atomic-actions.png` & `rally-4.1.0/doc/source/images/Report-Trends-Atomic-actions.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Trends-Configuration.png` & `rally-4.1.0/doc/source/images/Report-Trends-Configuration.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Trends-Overview.png` & `rally-4.1.0/doc/source/images/Report-Trends-Overview.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Trends-Total.png` & `rally-4.1.0/doc/source/images/Report-Trends-Total.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Trends-single-run.png` & `rally-4.1.0/doc/source/images/Report-Trends-single-run.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Verify-filter-by-status.png` & `rally-4.1.0/doc/source/images/Report-Verify-filter-by-status.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Verify-for-4-Verifications.png` & `rally-4.1.0/doc/source/images/Report-Verify-for-4-Verifications.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Verify-toggle-tags.png` & `rally-4.1.0/doc/source/images/Report-Verify-toggle-tags.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Verify-tracebacks.png` & `rally-4.1.0/doc/source/images/Report-Verify-tracebacks.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/images/Report-Verify-xfail.png` & `rally-4.1.0/doc/source/images/Report-Verify-xfail.png`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/index.rst` & `rally-4.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/install_and_upgrade/db_migrations.rst` & `rally-4.1.0/doc/source/install_and_upgrade/db_migrations.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/install_and_upgrade/index.rst` & `rally-4.1.0/doc/source/install_and_upgrade/index.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/install_and_upgrade/install.rst` & `rally-4.1.0/doc/source/install_and_upgrade/install.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/overview/glossary.rst` & `rally-4.1.0/doc/source/overview/glossary.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/overview/index.rst` & `rally-4.1.0/doc/source/overview/index.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/overview/overview.rst` & `rally-4.1.0/doc/source/overview/overview.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/overview/user_stories.rst` & `rally-4.1.0/doc/source/overview/user_stories.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/plugins/implementation/context_plugin.rst` & `rally-4.1.0/doc/source/plugins/implementation/context_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/plugins/implementation/hook_and_trigger_plugins.rst` & `rally-4.1.0/doc/source/plugins/implementation/hook_and_trigger_plugins.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/plugins/implementation/runner_plugin.rst` & `rally-4.1.0/doc/source/plugins/implementation/runner_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/plugins/implementation/scenario_plugin.rst` & `rally-4.1.0/doc/source/plugins/implementation/scenario_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/plugins/implementation/sla_plugin.rst` & `rally-4.1.0/doc/source/plugins/implementation/sla_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/plugins/index.rst` & `rally-4.1.0/doc/source/plugins/index.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/project_info/index.rst` & `rally-4.1.0/doc/source/project_info/index.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/project_info/release_notes.rst` & `rally-4.1.0/doc/source/project_info/release_notes.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/gates.rst` & `rally-4.1.0/doc/source/quick_start/gates.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/index.rst` & `rally-4.1.0/doc/source/quick_start/index.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_10_profiling_openstack_internals.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_10_profiling_openstack_internals.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_1_setting_up_env_and_running_benchmark_from_samples.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_1_setting_up_env_and_running_benchmark_from_samples.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_2_input_task_format.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_2_input_task_format.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_3_benchmarking_with_existing_users.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_3_benchmarking_with_existing_users.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_4_adding_success_criteria_for_benchmarks.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_4_adding_success_criteria_for_benchmarks.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_5_task_templates.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_5_task_templates.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_6_aborting_load_generation_on_sla_failure.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_6_aborting_load_generation_on_sla_failure.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_7_working_with_multple_openstack_clouds.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_7_working_with_multple_openstack_clouds.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_8_discovering_more_plugins.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_8_discovering_more_plugins.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial/step_9_verifying_cloud_via_tempest_verifier.rst` & `rally-4.1.0/doc/source/quick_start/tutorial/step_9_verifying_cloud_via_tempest_verifier.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/quick_start/tutorial.rst` & `rally-4.1.0/doc/source/quick_start/tutorial.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/task/index.rst` & `rally-4.1.0/doc/source/task/index.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/verification/cli_reference.rst` & `rally-4.1.0/doc/source/verification/cli_reference.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/verification/howto/add_new_reporter.rst` & `rally-4.1.0/doc/source/verification/howto/add_new_reporter.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/verification/howto/add_support_for_new_tool.rst` & `rally-4.1.0/doc/source/verification/howto/add_support_for_new_tool.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/verification/howto/migrate_from_old_design.rst` & `rally-4.1.0/doc/source/verification/howto/migrate_from_old_design.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/verification/index.rst` & `rally-4.1.0/doc/source/verification/index.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/verification/overview.rst` & `rally-4.1.0/doc/source/verification/overview.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/verification/reports.rst` & `rally-4.1.0/doc/source/verification/reports.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/source/verification/verifiers.rst` & `rally-4.1.0/doc/source/verification/verifiers.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/README.rst` & `rally-4.1.0/doc/specs/README.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/class-based-scenarios.rst` & `rally-4.1.0/doc/specs/implemented/class-based-scenarios.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/consistent_resource_names.rst` & `rally-4.1.0/doc/specs/implemented/consistent_resource_names.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/db_refactoring.rst` & `rally-4.1.0/doc/specs/implemented/db_refactoring.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/deployment_type.rst` & `rally-4.1.0/doc/specs/implemented/deployment_type.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/hook_plugins.rst` & `rally-4.1.0/doc/specs/implemented/hook_plugins.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/improve_atomic_actions_format.rst` & `rally-4.1.0/doc/specs/implemented/improve_atomic_actions_format.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/improve_scenario_output_format.rst` & `rally-4.1.0/doc/specs/implemented/improve_scenario_output_format.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/new_rally_input_task_format.rst` & `rally-4.1.0/doc/specs/implemented/new_rally_input_task_format.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/osprofiler.rst` & `rally-4.1.0/doc/specs/implemented/osprofiler.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/pluggable_validators.rst` & `rally-4.1.0/doc/specs/implemented/pluggable_validators.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/sla_pd_plugin.rst` & `rally-4.1.0/doc/specs/implemented/sla_pd_plugin.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/split_plugins.rst` & `rally-4.1.0/doc/specs/implemented/split_plugins.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/task_and_verification_export.rst` & `rally-4.1.0/doc/specs/implemented/task_and_verification_export.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/implemented/verification_refactoring.rst` & `rally-4.1.0/doc/specs/implemented/verification_refactoring.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/in-progress/cleanup_refactoring.rst` & `rally-4.1.0/doc/specs/in-progress/cleanup_refactoring.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/in-progress/distributed_runner.rst` & `rally-4.1.0/doc/specs/in-progress/distributed_runner.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/in-progress/pluggable-types.rst` & `rally-4.1.0/doc/specs/in-progress/pluggable-types.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/in-progress/raas.rst` & `rally-4.1.0/doc/specs/in-progress/raas.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/in-progress/refactor_scenario_utils.rst` & `rally-4.1.0/doc/specs/in-progress/refactor_scenario_utils.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/specs/template.rst` & `rally-4.1.0/doc/specs/template.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/user_stories/keystone/authenticate.rst` & `rally-4.1.0/doc/user_stories/keystone/authenticate.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/doc/user_stories/nova/boot_server.rst` & `rally-4.1.0/doc/user_stories/nova/boot_server.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/etc/motd_for_docker` & `rally-4.1.0/etc/motd_for_docker`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/etc/rally/rally.conf.sample` & `rally-4.1.0/etc/rally/rally.conf.sample`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/etc/rally.bash_completion` & `rally-4.1.0/etc/rally.bash_completion`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/api.py` & `rally-4.1.0/rally/api.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/cliutils.py` & `rally-4.1.0/rally/cli/cliutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/commands/db.py` & `rally-4.1.0/rally/cli/commands/db.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/commands/deployment.py` & `rally-4.1.0/rally/cli/commands/deployment.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/commands/env.py` & `rally-4.1.0/rally/cli/commands/env.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/commands/plugin.py` & `rally-4.1.0/rally/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/commands/task.py` & `rally-4.1.0/rally/cli/commands/task.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/commands/verify.py` & `rally-4.1.0/rally/cli/commands/verify.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/envutils.py` & `rally-4.1.0/rally/cli/envutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/main.py` & `rally-4.1.0/rally/cli/main.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/task_results_loader.py` & `rally-4.1.0/rally/cli/task_results_loader.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/cli/yamlutils.py` & `rally-4.1.0/rally/cli/yamlutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/broker.py` & `rally-4.1.0/rally/common/broker.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/cfg.py` & `rally-4.1.0/rally/common/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 # NOTE(andreykurilin): In near future we are planning to get rid of
 #   oslo_config. As a first step, let's hardcode the interface of it
 
 from oslo_config import cfg
-from oslo_config import fixture  # noqa
 
 
 CONF = cfg.CONF
 ConfigOpts = cfg.ConfigOpts
 
 find_config_dirs = cfg.find_config_dirs
 find_config_files = cfg.find_config_files
```

### Comparing `rally-4.0.0/rally/common/db/__init__.py` & `rally-4.1.0/rally/common/db/__init__.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/alembic.ini` & `rally-4.1.0/rally/common/db/alembic.ini`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/api.py` & `rally-4.1.0/rally/common/db/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,19 +39,20 @@
                        pool of available hardware (Default: True)
 
 """
 
 import datetime as dt
 import functools
 import tempfile
+import threading
 import time
 
 from oslo_db import exception as db_exc
 from oslo_db import options as db_options
-from oslo_db.sqlalchemy import session as db_session
+from oslo_db.sqlalchemy import enginefacade
 import sqlalchemy as sa
 import sqlalchemy.orm   # noqa
 
 from rally.common import cfg
 from rally.common.db import models
 from rally import consts
 from rally import exceptions
@@ -61,44 +62,40 @@
 CONF = cfg.CONF
 
 db_options.set_defaults(
     CONF, connection="sqlite:///%s/rally.sqlite" % tempfile.gettempdir())
 
 _FACADE = None
 _SESSION_MAKER = None
+_CONTEXT = None
 
 
-def _create_facade_lazily():
+def _get_facade():
     global _FACADE
 
     if _FACADE is None:
-        _FACADE = db_session.EngineFacade.from_config(CONF)
+        ctx = enginefacade.transaction_context()
+        ctx.configure(
+            sqlite_fk=False,
+            expire_on_commit=False
+        )
+        _FACADE = ctx.writer
 
     return _FACADE
 
 
 def get_engine():
-    facade = _create_facade_lazily()
-    return facade.get_engine()
-
-
-def get_session():
-    global _SESSION_MAKER
-
-    if not _SESSION_MAKER:
-        _SESSION_MAKER = sa.orm.sessionmaker()
-        _SESSION_MAKER.configure(bind=get_engine())
-
-    return _SESSION_MAKER()
+    return _get_facade().get_engine()
 
 
 def engine_reset():
-    global _FACADE, _SESSION_MAKER
+    global _FACADE, _CONTEXT
+
     _FACADE = None
-    _SESSION_MAKER = None
+    _CONTEXT = None
 
 
 def serialize(data):
     if data is None:
         return None
     if isinstance(data, (int,
                          str,
@@ -119,28 +116,27 @@
         for k in data:
             result[k] = serialize(data[k])
         return result
 
     raise ValueError("Failed to serialize %r data type." % type(data).__name__)
 
 
+def _get_context():
+    global _CONTEXT
+    if _CONTEXT is None:
+        _CONTEXT = threading.local()
+    return _CONTEXT
+
+
 def with_session(f):
 
     @functools.wraps(f)
     def wrapper(*args, **kwargs):
-        session = get_session()
-        session.expire_on_commit = False
-        try:
+        with _get_facade().using(_get_context()) as session:
             result = f(session, *args, **kwargs)
-            session.commit()
-        except Exception:
-            session.rollback()
-            raise
-        finally:
-            session.close()
 
         return serialize(result)
 
     return wrapper
 
 
 @with_session
@@ -198,15 +194,15 @@
 
     return task
 
 
 @with_session
 def task_get_status(session, uuid=None):
     task = (session.query(models.Task)
-                   .options(sa.orm.load_only("status"))
+                   .options(sa.orm.load_only(models.Task.status))
                    .filter_by(uuid=uuid).first())
     if not task:
         raise exceptions.DBRecordNotFound(
             criteria="uuid: %s" % uuid, table="tasks")
 
     return task.status
 
@@ -300,15 +296,15 @@
     if tags:
         uuids = _uuids_by_tags_get(session, consts.TagType.TASK, tags)
         if not uuids:
             return []
         query = query.filter(models.Task.uuid.in_(uuids))
 
     if uuids_only:
-        query = query.options(sa.orm.load_only("uuid"))
+        query = query.options(sa.orm.load_only(models.Task.uuid))
 
     for task in query.all():
         task = task.as_dict()
         if not uuids_only:
             task["tags"] = sorted(tags_get(task["uuid"], consts.TagType.TASK))
         tasks.append(task)
 
@@ -520,15 +516,15 @@
     return env
 
 
 @with_session
 def env_get_status(session, uuid):
     resp = (session.query(models.Env)
                    .filter_by(uuid=uuid)
-                   .options(sa.orm.load_only("status"))
+                   .options(sa.orm.load_only(models.Env.status))
                    .first())
     if not resp:
         raise exceptions.DBRecordNotFound(
             criteria="uuid: %s" % uuid, table="envs")
     return resp.status
```

### Comparing `rally-4.0.0/rally/common/db/migrations/README.rst` & `rally-4.1.0/rally/common/db/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/env.py` & `rally-4.1.0/rally/common/db/migrations/env.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def run_migrations_online():
     """Run migrations in 'online' mode.
 
     In this scenario we need to create an Engine
     and associate a connection with the context.
     """
     engine = api.get_engine()
-    with engine.connect() as connection:
+    with engine.begin() as connection:
         context.configure(connection=connection,
                           render_as_batch=True,
                           target_metadata=target_metadata)
         with context.begin_transaction():
             context.run_migrations()
```

### Comparing `rally-4.0.0/rally/common/db/migrations/script.py.mako` & `rally-4.1.0/rally/common/db/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_01_ca3626f62937_init_migration.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_01_ca3626f62937_init_migration.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_03_3177d36ea270_merge_credentials_from_users_and_admin.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_03_3177d36ea270_merge_credentials_from_users_and_admin.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_04_4ef544102ba7_change_task_status_enum.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_04_4ef544102ba7_change_task_status_enum.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_04_e654a0648db0_refactor_task_results.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_04_e654a0648db0_refactor_task_results.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_07_54e844ebfbc3_update_deployment_configs.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_07_54e844ebfbc3_update_deployment_configs.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_08_32fada9b2fde_remove_admin_domain_name.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_08_32fada9b2fde_remove_admin_domain_name.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_09_08e1515a576c_fix_invalid_verification_logs.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_09_08e1515a576c_fix_invalid_verification_logs.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_09_6ad4f426f005_add_hooks_to_task_result.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_09_6ad4f426f005_add_hooks_to_task_result.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_11_484cd9413e66_new_db_schema_for_verification_component.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_11_484cd9413e66_new_db_schema_for_verification_component.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2016_12_37fdbb373e8d_fix_test_results_for_verifications.py` & `rally-4.1.0/rally/common/db/migrations/versions/2016_12_37fdbb373e8d_fix_test_results_for_verifications.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_01_a6f364988fc2_change_tag_type_enum.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_01_a6f364988fc2_change_tag_type_enum.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_01_f33f4610dcda_change_verification_statuses.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_01_f33f4610dcda_change_verification_statuses.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_02_92aaaa2a6bb3_refactor_credentials.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_02_92aaaa2a6bb3_refactor_credentials.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_06_35fe16d4ab1c_update_tasks_based_on_workloads.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_06_35fe16d4ab1c_update_tasks_based_on_workloads.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_06_c517b0011857_fill_missed_workload_info.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_06_c517b0011857_fill_missed_workload_info.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_07_7948b83229f6_workload_min_max_durations.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_07_7948b83229f6_workload_min_max_durations.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_08_fab4f4f31f8a_fill_missed_workload_info.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_08_fab4f4f31f8a_fill_missed_workload_info.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_09_046a38742e89_port_configs_to_new_formats.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_09_046a38742e89_port_configs_to_new_formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 )
 
 
 def upgrade():
     connection = op.get_bind()
 
     for workload in connection.execute(workload_helper.select()):
-        runner = json.loads(workload["runner"])
+        runner = json.loads(workload.runner)
         runner.pop("type")
         values = {"runner": json.dumps(runner)}
-        hooks = workload["hooks"]
+        hooks = workload.hooks
         if hooks:
             values["hooks"] = []
             for hook in json.loads(hooks):
                 hook_cfg = hook["config"]
                 trigger_cfg = hook_cfg["trigger"]
                 hook["config"] = {
                     "description": hook_cfg.get("description"),
```

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_09_e0a5df2c5153_upsize_the_size_of_task_title.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_09_e0a5df2c5153_upsize_the_size_of_task_title.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_10_4394bdc32cfd_fill_missed_workload_info_r3.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_10_4394bdc32cfd_fill_missed_workload_info_r3.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,17 @@
 
 
 def upgrade():
     connection = op.get_bind()
 
     for workload in connection.execute(workload_helper.select()):
         full_data = []
-        for wdata in connection.execute(workload_data_helper.select(
-                workload_data_helper.c.workload_uuid == workload.uuid)):
+        for wdata in connection.execute(
+                workload_data_helper.select().where(
+                    workload_data_helper.c.workload_uuid == workload.uuid)):
             chunk_data = wdata.chunk_data["raw"]
 
             require_updating = False
             for itr in chunk_data:
                 if "output" not in itr:
                     itr["output"] = {"additive": [], "complete": []}
                     if ("scenario_output" in itr
```

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_10_9a18c6fe265c_rename_namespace_to_platform.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_10_9a18c6fe265c_rename_namespace_to_platform.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_10_dc46687661df_update_contexts.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_10_dc46687661df_update_contexts.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2017_12_a43700a813a5_add_env_platforms_tables.py` & `rally-4.1.0/rally/common/db/migrations/versions/2017_12_a43700a813a5_add_env_platforms_tables.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2018_01_44169f4d455e_deleted_worker_table.py` & `rally-4.1.0/rally/common/db/migrations/versions/2018_01_44169f4d455e_deleted_worker_table.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2018_01_7287df262dbc_move_deployment_to_env.py` & `rally-4.1.0/rally/common/db/migrations/versions/2018_01_7287df262dbc_move_deployment_to_env.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2018_02_95208e4eface_add_config_field_to_env_models.py` & `rally-4.1.0/rally/common/db/migrations/versions/2018_02_95208e4eface_add_config_field_to_env_models.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2018_02_bc908ac9a1fc_move_deployment_to_env_2.py` & `rally-4.1.0/rally/common/db/migrations/versions/2018_02_bc908ac9a1fc_move_deployment_to_env_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,18 +127,18 @@
 def upgrade():
     connection = op.get_bind()
     inspector = sa.inspect(connection)
     if "deployments" not in inspector.get_table_names():
         # 7287df262dbc did not fail. nothing to do
         return
 
-    envs = [env["uuid"] for env in connection.execute(envs_helper.select())]
+    envs = [env.uuid for env in connection.execute(envs_helper.select())]
 
     for deployment in connection.execute(deployments_helper.select()):
-        if deployment["uuid"] in envs:
+        if deployment.uuid in envs:
             # this deployment had been migrated by 7287df262dbc. Nothing to do
             continue
         status = "FAILED TO CREATE"
         spec = deployment.config
         extras = {}
         platform_data = None
         if isinstance(spec, dict) and (
```

### Comparing `rally-4.0.0/rally/common/db/migrations/versions/2018_02_dc0fe6de6786_update_old_deployment_config.py` & `rally-4.1.0/rally/common/db/migrations/versions/2018_02_dc0fe6de6786_update_old_deployment_config.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/models.py` & `rally-4.1.0/rally/common/db/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 """
 SQLAlchemy models for rally data.
 """
 import datetime as dt
 import uuid
 
 import sqlalchemy as sa
-import sqlalchemy.ext.declarative
 import sqlalchemy.orm   # noqa (used as sa.orm)
 
 from rally.common.db import sa_types
 from rally import consts
 
 
-BASE = sa.ext.declarative.declarative_base()
+BASE = sa.orm.declarative_base()
 
 
 def UUID():
     return str(uuid.uuid4())
 
 
 class RallyBase(object):
```

### Comparing `rally-4.0.0/rally/common/db/sa_types.py` & `rally-4.1.0/rally/common/db/sa_types.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/db/schema.py` & `rally-4.1.0/rally/common/db/schema.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/fileutils.py` & `rally-4.1.0/rally/common/fileutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/io/junit.py` & `rally-4.1.0/rally/common/io/junit.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/io/subunit_v2.py` & `rally-4.1.0/rally/common/io/subunit_v2.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/logging.py` & `rally-4.1.0/rally/common/logging.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/objects/__init__.py` & `rally-4.1.0/rally/common/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/objects/deploy.py` & `rally-4.1.0/rally/common/objects/deploy.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/objects/task.py` & `rally-4.1.0/rally/common/objects/task.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/objects/verification.py` & `rally-4.1.0/rally/common/objects/verification.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/objects/verifier.py` & `rally-4.1.0/rally/common/objects/verifier.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/opts.py` & `rally-4.1.0/rally/common/opts.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/plugin/discover.py` & `rally-4.1.0/rally/common/plugin/discover.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/plugin/info.py` & `rally-4.1.0/rally/common/plugin/info.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/plugin/meta.py` & `rally-4.1.0/rally/common/plugin/meta.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/plugin/plugin.py` & `rally-4.1.0/rally/common/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/sshutils.py` & `rally-4.1.0/rally/common/sshutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/streaming_algorithms.py` & `rally-4.1.0/rally/common/streaming_algorithms.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/utils.py` & `rally-4.1.0/rally/common/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/validation.py` & `rally-4.1.0/rally/common/validation.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/version.py` & `rally-4.1.0/rally/common/version.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/common/yamlutils.py` & `rally-4.1.0/rally/common/yamlutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/consts.py` & `rally-4.1.0/rally/consts.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/env/env_mgr.py` & `rally-4.1.0/rally/env/env_mgr.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/env/platform.py` & `rally-4.1.0/rally/env/platform.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/exceptions.py` & `rally-4.1.0/rally/exceptions.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/__init__.py` & `rally-4.1.0/rally/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/exporters/elastic/client.py` & `rally-4.1.0/rally/plugins/common/exporters/elastic/client.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/exporters/elastic/exporter.py` & `rally-4.1.0/rally/plugins/common/exporters/elastic/exporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/exporters/elastic/flatten.py` & `rally-4.1.0/rally/plugins/common/exporters/elastic/flatten.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/exporters/html.py` & `rally-4.1.0/rally/plugins/common/exporters/html.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/exporters/json_exporter.py` & `rally-4.1.0/rally/plugins/common/exporters/json_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/exporters/junit.py` & `rally-4.1.0/rally/plugins/common/exporters/junit.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/exporters/trends.py` & `rally-4.1.0/rally/plugins/common/exporters/trends.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/hook/sys_call.py` & `rally-4.1.0/rally/plugins/common/hook/sys_call.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/hook/triggers/event.py` & `rally-4.1.0/rally/plugins/common/hook/triggers/event.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/hook/triggers/periodic.py` & `rally-4.1.0/rally/plugins/common/hook/triggers/periodic.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/runners/constant.py` & `rally-4.1.0/rally/plugins/common/runners/constant.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/runners/rps.py` & `rally-4.1.0/rally/plugins/common/runners/rps.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/runners/serial.py` & `rally-4.1.0/rally/plugins/common/runners/serial.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/scenarios/dummy/dummy.py` & `rally-4.1.0/rally/plugins/common/scenarios/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/scenarios/requests/http_requests.py` & `rally-4.1.0/rally/plugins/common/scenarios/requests/http_requests.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/scenarios/requests/utils.py` & `rally-4.1.0/rally/plugins/common/scenarios/requests/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/sla/failure_rate.py` & `rally-4.1.0/rally/plugins/common/sla/failure_rate.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/sla/iteration_time.py` & `rally-4.1.0/rally/plugins/common/sla/iteration_time.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/sla/max_average_duration.py` & `rally-4.1.0/rally/plugins/common/sla/max_average_duration.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/sla/max_average_duration_per_atomic.py` & `rally-4.1.0/rally/plugins/common/sla/max_average_duration_per_atomic.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/sla/outliers.py` & `rally-4.1.0/rally/plugins/common/sla/outliers.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/sla/performance_degradation.py` & `rally-4.1.0/rally/plugins/common/sla/performance_degradation.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/types.py` & `rally-4.1.0/rally/plugins/common/types.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/validators.py` & `rally-4.1.0/rally/plugins/common/validators.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/verification/reporters.py` & `rally-4.1.0/rally/plugins/common/verification/reporters.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/common/verification/testr.py` & `rally-4.1.0/rally/plugins/common/verification/testr.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/contexts/dummy.py` & `rally-4.1.0/rally/plugins/task/contexts/dummy.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/exporters/elastic/client.py` & `rally-4.1.0/rally/plugins/task/exporters/elastic/client.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/exporters/elastic/exporter.py` & `rally-4.1.0/rally/plugins/task/exporters/elastic/exporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/exporters/elastic/flatten.py` & `rally-4.1.0/rally/plugins/task/exporters/elastic/flatten.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/exporters/html.py` & `rally-4.1.0/rally/plugins/task/exporters/html.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/exporters/json_exporter.py` & `rally-4.1.0/rally/plugins/task/exporters/json_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/exporters/junit.py` & `rally-4.1.0/rally/plugins/task/exporters/junit.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/exporters/old_json_results.py` & `rally-4.1.0/rally/plugins/task/exporters/old_json_results.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/exporters/trends.py` & `rally-4.1.0/rally/plugins/task/exporters/trends.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/hook_triggers/event.py` & `rally-4.1.0/rally/plugins/task/hook_triggers/event.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/hook_triggers/periodic.py` & `rally-4.1.0/rally/plugins/task/hook_triggers/periodic.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/hooks/sys_call.py` & `rally-4.1.0/rally/plugins/task/hooks/sys_call.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/runners/constant.py` & `rally-4.1.0/rally/plugins/task/runners/constant.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/runners/rps.py` & `rally-4.1.0/rally/plugins/task/runners/rps.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,27 @@
     def validate(self, context, config, plugin_cls, plugin_cfg):
         if isinstance(plugin_cfg["rps"], dict):
             if plugin_cfg["rps"]["end"] < plugin_cfg["rps"]["start"]:
                 msg = "rps end value must not be less than rps start value."
                 return self.fail(msg)
 
 
+def _runs_per_second(rps_cfg, start_timer, number_of_processes):
+    """At the given second return desired rps."""
+
+    if not isinstance(rps_cfg, dict):
+        return float(rps_cfg) / number_of_processes
+    stage_order = (time.time() - start_timer) / rps_cfg.get(
+        "duration", 1) - 1
+    rps = (float(rps_cfg["start"] + rps_cfg["step"] * stage_order)
+           / number_of_processes)
+
+    return min(rps, float(rps_cfg["end"]))
+
+
 @validation.add("check_rps")
 @runner.configure(name="rps")
 class RPSScenarioRunner(runner.ScenarioRunner):
     """Scenario runner that does the job with specified frequency.
 
     Every single scenario iteration is executed with specified frequency
     (runs per second) in a pool of processes. The scenario will be
@@ -228,26 +241,14 @@
         timeout = self.config.get("timeout", 0)  # 0 means no timeout
         iteration_gen = utils.RAMInt()
 
         cpu_count = multiprocessing.cpu_count()
         max_cpu_used = min(cpu_count,
                            self.config.get("max_cpu_count", cpu_count))
 
-        def runs_per_second(rps_cfg, start_timer, number_of_processes):
-            """At the given second return desired rps."""
-
-            if not isinstance(rps_cfg, dict):
-                return float(rps_cfg) / number_of_processes
-            stage_order = (time.time() - start_timer) / rps_cfg.get(
-                "duration", 1) - 1
-            rps = (float(rps_cfg["start"] + rps_cfg["step"] * stage_order)
-                   / number_of_processes)
-
-            return min(rps, float(rps_cfg["end"]))
-
         processes_to_start = min(max_cpu_used, times,
                                  self.config.get("max_concurrency", times))
         times_per_worker, times_overhead = divmod(times, processes_to_start)
 
         # Determine concurrency per worker
         concurrency_per_worker, concurrency_overhead = divmod(
             self.config.get("max_concurrency", times), processes_to_start)
@@ -278,15 +279,15 @@
             """
             while True:
                 yield (
                     result_queue, iteration_gen, timeout,
                     times_per_worker + (times_overhead and 1),
                     concurrency_per_worker + (concurrency_overhead and 1),
                     context, cls, method_name, args, event_queue,
-                    self.aborted, runs_per_second, self.config["rps"],
+                    self.aborted, _runs_per_second, self.config["rps"],
                     processes_to_start
                 )
                 if times_overhead:
                     times_overhead -= 1
                 if concurrency_overhead:
                     concurrency_overhead -= 1
```

### Comparing `rally-4.0.0/rally/plugins/task/runners/serial.py` & `rally-4.1.0/rally/plugins/task/runners/serial.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/scenarios/dummy/dummy.py` & `rally-4.1.0/rally/plugins/task/scenarios/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/scenarios/requests/http_requests.py` & `rally-4.1.0/rally/plugins/task/scenarios/requests/http_requests.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/scenarios/requests/utils.py` & `rally-4.1.0/rally/plugins/task/scenarios/requests/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/sla/failure_rate.py` & `rally-4.1.0/rally/plugins/task/sla/failure_rate.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/sla/iteration_time.py` & `rally-4.1.0/rally/plugins/task/sla/iteration_time.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/sla/max_average_duration.py` & `rally-4.1.0/rally/plugins/task/sla/max_average_duration.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/sla/max_average_duration_per_atomic.py` & `rally-4.1.0/rally/plugins/task/sla/max_average_duration_per_atomic.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/sla/outliers.py` & `rally-4.1.0/rally/plugins/task/sla/outliers.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/sla/performance_degradation.py` & `rally-4.1.0/rally/plugins/task/sla/performance_degradation.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/task/types.py` & `rally-4.1.0/rally/plugins/task/types.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/verification/reporters.py` & `rally-4.1.0/rally/plugins/verification/reporters.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/plugins/verification/testr.py` & `rally-4.1.0/rally/plugins/verification/testr.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/atomic.py` & `rally-4.1.0/rally/task/atomic.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/context.py` & `rally-4.1.0/rally/task/context.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/engine.py` & `rally-4.1.0/rally/task/engine.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/exporter.py` & `rally-4.1.0/rally/task/exporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/functional.py` & `rally-4.1.0/rally/task/functional.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/hook.py` & `rally-4.1.0/rally/task/hook.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/processing/charts.py` & `rally-4.1.0/rally/task/processing/charts.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/processing/plot.py` & `rally-4.1.0/rally/task/processing/plot.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/processing/utils.py` & `rally-4.1.0/rally/task/processing/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/runner.py` & `rally-4.1.0/rally/task/runner.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/scenario.py` & `rally-4.1.0/rally/task/scenario.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/service.py` & `rally-4.1.0/rally/task/service.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/sla.py` & `rally-4.1.0/rally/task/sla.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/task_cfg.py` & `rally-4.1.0/rally/task/task_cfg.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/types.py` & `rally-4.1.0/rally/task/types.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/utils.py` & `rally-4.1.0/rally/task/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/task/validation.py` & `rally-4.1.0/rally/task/validation.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/base.html` & `rally-4.1.0/rally/ui/templates/base.html`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/ci/index.html` & `rally-4.1.0/rally/ui/templates/ci/index.html`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/ci/index_verify.html` & `rally-4.1.0/rally/ui/templates/ci/index_verify.html`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/libs/angular.1.3.3.min.js` & `rally-4.1.0/rally/ui/templates/libs/angular.1.3.3.min.js`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/libs/d3.3.4.13.min.js` & `rally-4.1.0/rally/ui/templates/libs/d3.3.4.13.min.js`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.css` & `rally-4.1.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.css`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.js` & `rally-4.1.0/rally/ui/templates/libs/nv.d3.1.1.15-beta.min.js`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/task/directive_widget.js` & `rally-4.1.0/rally/ui/templates/task/directive_widget.js`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/task/report.html` & `rally-4.1.0/rally/ui/templates/task/report.html`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/task/trends.html` & `rally-4.1.0/rally/ui/templates/task/trends.html`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/templates/verification/report.html` & `rally-4.1.0/rally/ui/templates/verification/report.html`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/ui/utils.py` & `rally-4.1.0/rally/ui/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/utils/encodeutils.py` & `rally-4.1.0/rally/utils/encodeutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/utils/sshutils.py` & `rally-4.1.0/rally/utils/sshutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/utils/strutils.py` & `rally-4.1.0/rally/utils/strutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/verification/context.py` & `rally-4.1.0/rally/verification/context.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/verification/manager.py` & `rally-4.1.0/rally/verification/manager.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/verification/reporter.py` & `rally-4.1.0/rally/verification/reporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally/verification/utils.py` & `rally-4.1.0/rally/verification/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally-jobs/plugins/fake_plugin.py` & `rally-4.1.0/rally-jobs/plugins/fake_plugin.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally-jobs/plugins/rally_profile.py` & `rally-4.1.0/rally-jobs/plugins/rally_profile.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally-jobs/plugins/test_relative_import/zzz.py` & `rally-4.1.0/rally-jobs/plugins/test_relative_import/zzz.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally-jobs/self-rally.yaml` & `rally-4.1.0/rally-jobs/self-rally.yaml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/rally.egg-info/PKG-INFO` & `rally-4.1.0/rally.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rally
-Version: 4.0.0
+Version: 4.1.0
 Summary: Generic Testing Framework & Tool that unifies all types of testing.
 Home-page: https://rally.readthedocs.io/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: =====
         Rally
@@ -132,11 +132,11 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: test
```

### Comparing `rally-4.0.0/rally.egg-info/SOURCES.txt` & `rally-4.1.0/rally.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/requirements.txt` & `rally-4.1.0/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 paramiko!=2.9.0,!=2.9.1                                # LGPL
 pbr!=2.1.0                                             # Apache Software License
 PrettyTable!=3.4.0                                     # BSD (3 clause)
 pyOpenSSL                                              # Apache License, Version 2.0
 PyYAML                                                 # MIT
 python-subunit                                         # Apache-2.0 or BSD
 requests!=2.20.0,!=2.24.0                              # Apache License, Version 2.0
-SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,<2.0.0       # MIT
+SQLAlchemy>=1.4.0                                      # MIT
 virtualenv!=16.3.0                                     # MIT
```

### Comparing `rally-4.0.0/samples/tasks/README.rst` & `rally-4.1.0/samples/tasks/README.rst`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/samples/tasks/scenarios/requests/check-random-request.json` & `rally-4.1.0/samples/tasks/scenarios/requests/check-random-request.json`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/samples/tasks/scenarios/requests/check-request.json` & `rally-4.1.0/samples/tasks/scenarios/requests/check-request.json`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/samples/tasks/sla/dummy.json` & `rally-4.1.0/samples/tasks/sla/dummy.json`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/setup.cfg` & `rally-4.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 summary = Generic Testing Framework & Tool that unifies all types of testing.
 description_file = 
 	README.rst
 author = OpenStack
 author_email = openstack-discuss@lists.openstack.org
 home_page = https://rally.readthedocs.io/
 license = Apache License, Version 2.0
-requires_python = >=3.6
+requires_python = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
```

### Comparing `rally-4.0.0/setup.py` & `rally-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/test-requirements.txt` & `rally-4.1.0/test-requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # The order of packages is significant, because pip processes them in the order
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
 
-hacking>=3.0                                           # Apache Software License
+hacking>=4.0                                           # Apache Software License
 
+fixtures                                               # Apache Software License/BSD License
 pytest                                                 # MIT
 # py.test plugin for measuring coverage.
 pytest-cov                                             # MIT
 # py.test plugin for generating HTML reports
-pytest-html                                            # Mozilla Public License 2.0 (MPL 2.0)
+pytest-html                                            # MIT
 # py.test xdist plugin for distributed testing and loop-on-failing modes
 pytest-xdist                                           # MIT
 
 ddt                                                    # MIT
-testtools                                              # MIT
 
-testresources                                          # UNKNOWN
-
-docutils<0.18                                          # public domain, Python, 2-Clause BSD, GPL 3 (see COPYING.txt)
+docutils                                               # BSD License/GNU General Public License (GPL)/Python Software Foundation License
 Pygments                                               # BSD-2-Clause
```

### Comparing `rally-4.0.0/tests/README.rst` & `rally-4.1.0/tests/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,37 +12,37 @@
 The goal of unit tests is to ensure that internal parts of the code work properly.
 All internal methods should be fully covered by unit tests with a reasonable mocks usage.
 
 
 About Rally unit tests:
 
 - All `unit tests <http://en.wikipedia.org/wiki/Unit_testing>`_ are located inside /tests/unit/*
-- Tests are written on top of: *testtools* and *mock* libs
+- Tests are written on top of: *unittest* lib
 - `Tox <https://tox.readthedocs.org/en/latest/>`_ is used to run unit tests
 
 
 To run unit tests locally::
 
   $ pip install tox
   $ tox
 
-To run py27, py34, py35 or pep8 only::
+To run py311 or pep8 only::
 
   $ tox -e <name>
 
-  # NOTE: <name> is one of py27, py34, py35 or pep8
+  # NOTE: <name> is one of py311 or pep8
 
-To run py27/py34/py35 against mysql or psql
+To run py311 against mysql or psql
 
   $ export RALLY_UNITTEST_DB_URL="mysql://user:secret@localhost/rally"
-  $ tox -epy27
+  $ tox -epy311
 
-To run specific test of py27/py34/py35::
+To run specific test of py311::
 
-  $ tox -e py27 -- tests.unit.test_osclients
+  $ tox -e py311 -- tests.unit.test_osclients
 
 To get test coverage::
 
   $ tox -e cover
 
   # NOTE: Results will be in ./cover/index.html
```

### Comparing `rally-4.0.0/tests/ci/cover.sh` & `rally-4.1.0/tests/ci/cover.sh`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml` & `rally-4.1.0/tests/ci/playbooks/fetch-html-and-json-reports.yaml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/playbooks/rally-install-pre.yaml` & `rally-4.1.0/tests/ci/playbooks/rally-install-pre.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -2,45 +2,68 @@
   name: Prepare host to install Rally
   tasks:
     - name: Uninstall python3-pyyaml (CentOS 8 & 9)
       become: true
       package:
         state: absent
         name: python3-pyyaml
+      when:
+        - ansible_distribution == "CentOS"
 
     - name: Install python3.8-dev (Ubuntu 20.04)
       become: true
       package:
         state: present
         name: python3.8-dev
       when: ansible_distribution == "Ubuntu" and ansible_distribution_version == "20.04"
 
     - name: Install python3.10-dev (Ubuntu 22.04)
       become: true
       package:
         state: present
         name: python3.10-dev
-      when: ansible_distribution == "Ubuntu" and ansible_distribution_version == "22.04"
+      when:
+        - ansible_distribution == "Ubuntu"
+        - ansible_distribution_version == "22.04"
+
+    - name: Install python3.8-devel (Centos 8)
+      become: true
+      package:
+        state: present
+        name: python38-devel
+      when:
+        - ansible_distribution == "CentOS"
+        - ansible_distribution_version | int < 9
+
+    - name: Change default python3 to be python3.8 (Centos 8)
+      become: true
+      shell: |
+        set -x
+        set -e
+
+        echo "alias python3='python3.8'" >> ~/.bashrc"
+        echo "alias python3='python3.8'" >> ~zuul/.bashrc"
+        whereis python3.8
+        ls /usr/bin/python*
+        update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.8 100
+        update-alternatives --set python3 /usr/bin/python3.8
+      when:
+        - ansible_distribution == "CentOS"
+        - ansible_distribution_version | int < 9
 
     - name: Install pip3 if needed
       become: true
       shell:
         executable: /bin/bash
         chdir: '{{ zuul.project.src_dir }}'
         cmd: |
           set -e
-          python_version=`python3 --version`
-          python_version=`echo $python_version |awk '{print $2}'`
+          python_version=`python3 --version | awk '{print $2}'`
           echo $python_version
-          if [[ $python_version =~ ^3.6 ]]; then
-              pip_url=https://bootstrap.pypa.io/pip/3.6/get-pip.py
-          else
-              pip_url=https://bootstrap.pypa.io/get-pip.py
-          fi
-          curl $pip_url -o /tmp/get-pip.py
+          curl https://bootstrap.pypa.io/get-pip.py -o /tmp/get-pip.py
           python3 /tmp/get-pip.py
 
     - name: Install bindep
       become: true
       shell: pip3 install --upgrade bindep
 
     - name: Prepare rally plugins stored at home dir
```

### Comparing `rally-4.0.0/tests/ci/playbooks/rally-install-run.yaml` & `rally-4.1.0/tests/ci/playbooks/rally-install-run.yaml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml` & `rally-4.1.0/tests/ci/playbooks/roles/docker-build-image/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml` & `rally-4.1.0/tests/ci/playbooks/roles/docker-push-image/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/playbooks/roles/rally-tox/files/find_python_for_tox_env.py` & `rally-4.1.0/tests/ci/playbooks/roles/rally-tox/files/find_python_for_tox_env.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/playbooks/roles/rally-tox/tasks/install.yaml` & `rally-4.1.0/tests/ci/playbooks/roles/rally-tox/tasks/install.yaml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/pytest_launcher.py` & `rally-4.1.0/tests/ci/pytest_launcher.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/rally_app.py` & `rally-4.1.0/tests/ci/rally_app.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/rally_self_job.py` & `rally-4.1.0/tests/ci/rally_self_job.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/render.py` & `rally-4.1.0/tests/ci/render.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/ci/sync_requirements.py` & `rally-4.1.0/tests/ci/sync_requirements.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/functional/extra/fake_dir1/fake_plugin1.py` & `rally-4.1.0/tests/functional/extra/fake_dir1/fake_plugin1.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/functional/extra/fake_dir2/fake_plugin2.py` & `rally-4.1.0/tests/functional/extra/fake_dir2/fake_plugin2.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/functional/extra/fake_platforms.py` & `rally-4.1.0/tests/functional/extra/fake_platforms.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/functional/extra/fake_verify.py` & `rally-4.1.0/tests/functional/extra/fake_verify.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/functional/test_cli_deployment.py` & `rally-4.1.0/tests/functional/test_cli_deployment.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import os
-
-import testtools
+import unittest
 
 from tests.functional import utils
 
 
-class DeploymentTestCase(testtools.TestCase):
+class DeploymentTestCase(unittest.TestCase):
 
     def test_create_deployment_from_env(self):
         os.environ.update(
             {
                 "OS_AUTH_URL": "http://fake",
                 "OS_USERNAME": "fake",
                 "OS_PASSWORD": "fake"
```

### Comparing `rally-4.0.0/tests/functional/test_cli_env.py` & `rally-4.1.0/tests/functional/test_cli_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import json
 import os
 import tempfile
-
-import testtools
+import unittest
 
 from tests.functional import utils
 
 
-class EnvTestCase(testtools.TestCase):
+class EnvTestCase(unittest.TestCase):
 
     def test_create_no_spec(self):
         rally = utils.Rally()
         rally("env create --name empty --description de")
         self.assertIn("empty", rally("env list"))
         env_data = rally("env show --json", getjson=True)
         self.assertEqual("empty", env_data["name"])
```

### Comparing `rally-4.0.0/tests/functional/test_cli_functional.py` & `rally-4.1.0/tests/functional/test_cli_functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import subprocess
-
-import testtools
+import unittest
 
 from rally.utils import encodeutils
 
 
-class CLITestCase(testtools.TestCase):
+class CLITestCase(unittest.TestCase):
 
     def test_rally_cli(self):
         try:
             subprocess.check_output(["rally"], stderr=subprocess.STDOUT)
         except subprocess.CalledProcessError as e:
             output = encodeutils.safe_decode(e.output)
         else:
```

### Comparing `rally-4.0.0/tests/functional/test_cli_plugin.py` & `rally-4.1.0/tests/functional/test_cli_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,57 +9,58 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-import testtools
+import unittest
 
 from tests.functional import utils
 
 
-class PluginTestCase(testtools.TestCase):
+class PluginTestCase(unittest.TestCase):
 
     def test_show_one(self):
         rally = utils.Rally()
         result = rally("plugin show Dummy.dummy")
         self.assertIn("NAME", result)
         self.assertIn("PLATFORM", result)
         self.assertIn("Dummy.dummy", result)
         self.assertIn("MODULE", result)
 
     def test_show_multiple(self):
         rally = utils.Rally()
-        result = self.assertRaises(utils.RallyCliError,
-                                   rally, "plugin show Dummy")
+        with self.assertRaises(utils.RallyCliError) as e_ctx:
+            rally("plugin show Dummy")
+        result = e_ctx.exception
         self.assertIn("Multiple plugins found:", result.output)
         self.assertIn("Dummy.dummy", result.output)
         self.assertIn("Dummy.dummy_exception", result.output)
         self.assertIn("Dummy.dummy_random_fail_in_atomic", result.output)
 
     def test_show_not_found(self):
         rally = utils.Rally()
         name = "Dummy666666"
-        result = self.assertRaises(utils.RallyCliError,
-                                   rally, "plugin show %s" % name)
-        self.assertIn("Plugin %s not found" % name, result.output)
+        with self.assertRaises(utils.RallyCliError) as e_ctx:
+            rally(f"plugin show {name}")
+        self.assertIn("Plugin %s not found" % name, e_ctx.exception.output)
 
     def test_show_not_found_in_specific_platform(self):
         rally = utils.Rally()
         name = "Dummy"
         platform = "non_existing"
-        result = self.assertRaises(
-            utils.RallyCliError,
-            rally, "plugin show --name %(name)s --platform %(platform)s"
-                   % {"name": name, "platform": platform})
+
+        with self.assertRaises(utils.RallyCliError) as e_ctx:
+            rally(f"plugin show --name {name} --platform {platform}")
+
         self.assertIn(
             "Plugin %(name)s@%(platform)s not found"
             % {"name": name, "platform": platform},
-            result.output)
+            e_ctx.exception.output)
 
     def test_list(self):
         rally = utils.Rally()
         result = rally("plugin list Dummy")
         self.assertIn("Dummy.dummy", result)
         self.assertIn("Dummy.dummy_exception", result)
         self.assertIn("Dummy.dummy_random_fail_in_atomic", result)
```

### Comparing `rally-4.0.0/tests/functional/test_cli_task.py` & `rally-4.1.0/tests/functional/test_cli_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 #    under the License.
 
 import json
 import os
 import re
 import threading
 import time
+import unittest
 from unittest import mock
 
 import jsonschema
 import pytest
-import testtools
 
 from rally import api
 from tests.functional import utils
 
 
 FAKE_TASK_UUID = "87ab639d-4968-4638-b9a1-07774c32484a"
 
 
-class TaskTestCase(testtools.TestCase):
+class TaskTestCase(unittest.TestCase):
 
     def _get_sample_task_config(self):
         return {
             "Dummy.dummy_random_fail_in_atomic": [
                 {
                     "runner": {
                         "type": "constant",
@@ -206,19 +206,18 @@
         self.assertIn("Dummy.dummy", detailed)
         detailed_iterations_data = rally("task detailed --iterations-data")
         self.assertNotIn("n/a", detailed_iterations_data)
 
     def test_start_with_empty_config(self):
         rally = utils.Rally()
         config = utils.TaskConfig(None)
-        err = self.assertRaises(
-            utils.RallyCliError,
-            rally, "task start --task %s" % config.filename)
+        with self.assertRaises(utils.RallyCliError) as e_ctx:
+            rally(f"task start --task {config.filename}")
         self.assertIn("Task config is invalid: `It is empty`",
-                      err.output)
+                      e_ctx.exception.output)
 
     def test_results(self):
         rally = utils.Rally()
         cfg = self._get_sample_task_config()
         config = utils.TaskConfig(cfg)
         rally("task start --task %s" % config.filename)
         self.assertIn("result", rally("task results"))
@@ -261,19 +260,20 @@
     def test_detailed_with_wrong_task_id(self):
         rally = utils.Rally()
         self.assertRaises(utils.RallyCliError,
                           rally, "task detailed --uuid %s" % FAKE_TASK_UUID)
 
     def test_report_with_wrong_task_id(self):
         rally = utils.Rally()
-        e = self.assertRaises(utils.RallyCliError,
-                              rally, "task report --uuid %s" % FAKE_TASK_UUID)
+
+        with self.assertRaises(utils.RallyCliError) as e_ctx:
+            rally(f"task report --uuid {FAKE_TASK_UUID}")
         self.assertIn(
-            "Record for uuid: %s not found in table task" % FAKE_TASK_UUID,
-            str(e))
+            f"Record for uuid: {FAKE_TASK_UUID} not found in table task",
+            str(e_ctx.exception))
 
     def test_sla_check_with_wrong_task_id(self):
         rally = utils.Rally()
         self.assertRaises(utils.RallyCliError,
                           rally, "task sla-check --uuid %s" % FAKE_TASK_UUID)
 
     def test_status_with_wrong_task_id(self):
@@ -908,24 +908,22 @@
                         "concurrency": 1
                     },
                 }
             ]
         }
         self._test_start_abort_on_sla_failure(cfg, times)
 
-    def _start_task_in_new_thread(self, rally, cfg, report_file):
+    def _start_task_in_new_thread(self, rally, cfg, suffix):
         deployment_id = utils.get_global("RALLY_DEPLOYMENT", rally.env)
         config = utils.TaskConfig(cfg)
         cmd = (("task start --task %(task_file)s "
                 "--deployment %(deployment_id)s") %
                {"task_file": config.filename,
                 "deployment_id": deployment_id})
-        report_path = os.path.join(
-            os.environ.get("REPORTS_ROOT", "rally-cli-output-files"),
-            "TaskTestCase", report_file)
+        report_path = rally.gen_report_path(suffix=suffix)
         task = threading.Thread(target=rally, args=(cmd, ),
                                 kwargs={"report_path": report_path})
         task.start()
         uuid = None
         while not uuid:
             if not uuid:
                 uuid = utils.get_global("RALLY_TASK", rally.env)
@@ -946,15 +944,15 @@
                         "times": RUNNER_TIMES
                     }
                 }
             ]
         }
         rally = utils.Rally()
         task, uuid = self._start_task_in_new_thread(
-            rally, cfg, "test_abort-thread_with_abort.txt")
+            rally, cfg, "-thread_with_abort")
         rally("task abort %s" % uuid)
         task.join()
         results = rally("task results", getjson=True)
         iterations_completed = len(results[0]["result"])
         # NOTE(msdubov): check that the task is really stopped before
         #                the specified number of iterations
         self.assertLess(iterations_completed, RUNNER_TIMES)
@@ -980,15 +978,15 @@
                         "times": 10,
                     }
                 }
             ]
         }
         rally = utils.Rally()
         task, uuid = self._start_task_in_new_thread(
-            rally, cfg, "test_abort_soft-thread_with_soft_abort.txt")
+            rally, cfg, suffix="-thread_with_soft_abort")
         rally("task abort --soft")
         task.join()
         results = rally("task results", getjson=True)
         iterations_completed = len(results[0]["result"])
         self.assertEqual(3, iterations_completed)
         self.assertEqual(1, len(results))
         self.assertIn("aborted", rally("task status"))
@@ -1097,15 +1095,15 @@
                "--deployment %(deployment_id)s") %
               {"task_file": config.filename,
                "deployment_id": deployment_id})
         self.assertRaises(utils.RallyCliError, rally,
                           "task restart --scenario fake.fake_scenario")
 
 
-class SLATestCase(testtools.TestCase):
+class SLATestCase(unittest.TestCase):
 
     def _get_sample_task_config(self, max_seconds_per_iteration=4,
                                 failure_rate_max=0):
         return {
             "Dummy.dummy": [
                 {
                     "args": {
@@ -1124,20 +1122,19 @@
             ]
         }
 
     def test_sla_fail(self):
         rally = utils.Rally()
         cfg = self._get_sample_task_config(max_seconds_per_iteration=0.001)
         config = utils.TaskConfig(cfg)
-        err = self.assertRaises(
-            utils.RallyCliError,
-            rally, "task start --task %s" % config.filename)
-        output = err.output
+
+        with self.assertRaises(utils.RallyCliError) as e_ctx:
+            rally(f"task start --task {config.filename}")
         self.assertIn("At least one workload did not pass SLA criteria.",
-                      output)
+                      e_ctx.exception.output)
         self.assertRaises(utils.RallyCliError, rally, "task sla-check")
 
     def test_sla_success(self):
         rally = utils.Rally()
         config = utils.TaskConfig(self._get_sample_task_config())
         rally("task start --task %s" % config.filename)
         rally("task sla-check")
@@ -1151,15 +1148,15 @@
              "detail": mock.ANY,
              "pos": 0, "status": "PASS"}
         ]
         data = rally("task sla-check --json", getjson=True, no_logs=True)
         self.assertEqual(expected, data)
 
 
-class SLAExtraFlagsTestCase(testtools.TestCase):
+class SLAExtraFlagsTestCase(unittest.TestCase):
 
     def test_abort_on_sla_fail(self):
         rally = utils.Rally()
         cfg = {
             "Dummy.dummy_exception": [
                 {
                     "args": {},
@@ -1183,17 +1180,17 @@
              "detail": "Task was aborted due to SLA failure(s).",
              "pos": 0, "status": "FAIL"},
             {"benchmark": "Dummy.dummy_exception",
              "criterion": "failure_rate",
              "detail": mock.ANY,
              "pos": 0, "status": "FAIL"}
         ]
-        e = self.assertRaises(utils.RallyCliError,
-                              rally, "task sla-check --json", getjson=True)
-        self.assertEqual(expected, json.loads(e.output))
+        with self.assertRaises(utils.RallyCliError) as e_ctx:
+            rally("task sla-check --json", getjson=True)
+        self.assertEqual(expected, json.loads(e_ctx.exception.output))
 
     def _test_broken_context(self, runner):
         rally = utils.Rally()
         cfg = {
             "Dummy.dummy": [
                 {
                     "args": {},
@@ -1214,31 +1211,31 @@
                        "Passed",
              "pos": 0},
             {"benchmark": "Dummy.dummy",
              "criterion": "something_went_wrong",
              "detail": mock.ANY,
              "pos": 0, "status": "FAIL"}
         ]
-        e = self.assertRaises(utils.RallyCliError,
-                              rally, "task sla-check --json", getjson=True)
-        self.assertEqual(expected, json.loads(e.output))
+        with self.assertRaises(utils.RallyCliError) as e_ctx:
+            rally("task sla-check --json", getjson=True)
+        self.assertEqual(expected, json.loads(e_ctx.exception.output))
 
     def test_broken_context_with_constant_runner(self):
         self._test_broken_context({"type": "constant",
                                    "times": 5,
                                    "concurrency": 5})
 
     def test_broken_context_with_rps_runner(self):
         self._test_broken_context({"type": "rps",
                                    "times": 5,
                                    "rps": 3,
                                    "timeout": 6})
 
 
-class SLAPerfDegrTestCase(testtools.TestCase):
+class SLAPerfDegrTestCase(unittest.TestCase):
 
     def _get_sample_task_config(self, max_degradation=500):
         return {
             "Dummy.dummy_random_action": [
                 {
                     "args": {
                         "actions_num": 5,
@@ -1259,20 +1256,18 @@
             ]
         }
 
     def test_sla_fail(self):
         rally = utils.Rally()
         cfg = self._get_sample_task_config(max_degradation=1)
         config = utils.TaskConfig(cfg)
-        err = self.assertRaises(
-            utils.RallyCliError,
-            rally, "task start --task %s" % config.filename)
-        output = err.output
+        with self.assertRaises(utils.RallyCliError) as e_ctx:
+            rally(f"task start --task {config.filename}")
         self.assertIn("At least one workload did not pass SLA criteria.",
-                      output)
+                      e_ctx.exception.output)
         self.assertRaises(utils.RallyCliError, rally, "task sla-check")
 
     def test_sla_success(self):
         rally = utils.Rally()
         config = utils.TaskConfig(self._get_sample_task_config())
         rally("task start --task %s" % config.filename)
         rally("task sla-check")
@@ -1282,15 +1277,15 @@
              "detail": mock.ANY,
              "pos": 0, "status": "PASS"},
         ]
         data = rally("task sla-check --json", getjson=True)
         self.assertEqual(expected, data)
 
 
-class HookTestCase(testtools.TestCase):
+class HookTestCase(unittest.TestCase):
 
     def setUp(self):
         super(HookTestCase, self).setUp()
         self.started = time.time()
 
     def _assert_results_time(self, results):
         for trigger_results in results:
```

### Comparing `rally-4.0.0/tests/functional/test_cli_verify.py` & `rally-4.1.0/tests/functional/test_cli_verify.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import re
-
-import testtools
+import unittest
 
 from tests.functional import utils
 
 
-class VerifyTestCase(testtools.TestCase):
+class VerifyTestCase(unittest.TestCase):
 
     def test_list_plugins(self):
         rally = utils.Rally(plugin_path="tests/functional/extra")
         output = rally("verify list-plugins")
         self.assertIn("fakeverifier", output)
         self.assertIn("installation", output)
```

### Comparing `rally-4.0.0/tests/functional/test_lib_api.py` & `rally-4.1.0/tests/functional/test_lib_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,20 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import os
 import subprocess
-
-import testtools
+import unittest
 
 from tests.functional import utils
 
 
-class LibAPITestCase(testtools.TestCase):
+class LibAPITestCase(unittest.TestCase):
 
     def test_rally_lib(self):
         rally = utils.Rally(force_new_db=True)
         cdir = os.path.dirname(os.path.realpath(__file__))
         app = os.path.join(cdir, "../ci/rally_app.py")
         subprocess.check_output(
             ["python", app, "--config-file", rally.config_filename])
```

### Comparing `rally-4.0.0/tests/functional/utils.py` & `rally-4.1.0/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/hacking/checks.py` & `rally-4.1.0/tests/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/samples/test_task_samples.py` & `rally-4.1.0/tests/samples/test_task_samples.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/commands/test_db.py` & `rally-4.1.0/tests/unit/cli/commands/test_db.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/commands/test_deployment.py` & `rally-4.1.0/tests/unit/cli/commands/test_deployment.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/commands/test_docstrings.py` & `rally-4.1.0/tests/unit/cli/commands/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/commands/test_env.py` & `rally-4.1.0/tests/unit/cli/commands/test_env.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/commands/test_plugin.py` & `rally-4.1.0/tests/unit/cli/commands/test_plugin.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/commands/test_task.py` & `rally-4.1.0/tests/unit/cli/commands/test_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -698,15 +698,15 @@
             task_obj["subtasks"][0]["workloads"])
 
         self.fake_api.task.get.return_value = task_obj
 
         self.assertIsNone(self.task.results(self.fake_api, task_id))
         self.assertEqual(1, mock_json_dumps.call_count)
         self.assertEqual(1, len(mock_json_dumps.call_args[0]))
-        self.assertSequenceEqual(result, mock_json_dumps.call_args[0][0])
+        self.assertEqual(list(result), mock_json_dumps.call_args[0][0])
         self.assertEqual({"sort_keys": False, "indent": 4},
                          mock_json_dumps.call_args[1])
         self.fake_api.task.get.assert_called_once_with(
             task_id=task_id, detailed=True)
 
     @mock.patch("rally.cli.commands.task.sys.stdout")
     def test_results_no_data(self, mock_stdout):
```

### Comparing `rally-4.0.0/tests/unit/cli/commands/test_verify.py` & `rally-4.1.0/tests/unit/cli/commands/test_verify.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/test_cliutils.py` & `rally-4.1.0/tests/unit/cli/test_cliutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/test_envutils.py` & `rally-4.1.0/tests/unit/cli/test_envutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/test_task_results_loader.py` & `rally-4.1.0/tests/unit/cli/test_task_results_loader.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/cli/test_yamlutils.py` & `rally-4.1.0/tests/unit/cli/test_yamlutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/db/test_api.py` & `rally-4.1.0/tests/unit/common/db/test_api.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/db/test_migrations.py` & `rally-4.1.0/tests/unit/common/db/test_migrations.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import copy
 import datetime as dt
 import importlib
 import iso8601
 import json
 import pickle
 import pprint
+import typing as t
 from unittest import mock
 import uuid
 
 import alembic
 import jsonschema
 from oslo_db.sqlalchemy import test_migrations
 from oslo_db.sqlalchemy import utils as db_utils
@@ -273,15 +274,15 @@
                 break
 
         self.assertEqual(sorted(members), sorted(index_columns))
 
     def test_walk_versions(self):
         self.walk_versions(self.engine)
 
-    def _check_3177d36ea270(self, engine, data):
+    def _check_3177d36ea270(self, engine: sa.engine.Engine):
         self.assertEqual(
             "3177d36ea270", db.schema.schema_revision(engine=engine))
         self.assertColumnExists(engine, "deployments", "credentials")
         self.assertColumnNotExists(engine, "deployments", "admin")
         self.assertColumnNotExists(engine, "deployments", "users")
 
     def _pre_upgrade_54e844ebfbc3(self, engine):
@@ -344,15 +345,15 @@
                 "region_name": "RegionOne",
                 "type": "ExistingCloud",
                 "endpoint_type": "internal"},
         }
         deployment_table = db_utils.get_table(engine, "deployments")
 
         deployment_status = consts.DeployStatus.DEPLOY_FINISHED
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             for deployment in self._54e844ebfbc3_deployments:
                 conf = json.dumps(self._54e844ebfbc3_deployments[deployment])
                 conn.execute(
                     deployment_table.insert(),
                     [{"uuid": deployment, "name": deployment,
                       "config": conf,
                       "enum_deployments_status": deployment_status,
@@ -421,25 +422,27 @@
                     }
                 ],
             }
         }
 
     }
 
-    def _check_54e844ebfbc3(self, engine, data):
+    def _check_54e844ebfbc3(self, engine: sa.engine.Engine):
         self.assertEqual("54e844ebfbc3",
                          db.schema.schema_revision(engine=engine))
 
         original_deployments = self._54e844ebfbc3_deployments
 
         deployment_table = db_utils.get_table(engine, "deployments")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             deployments_found = conn.execute(
                 deployment_table.select()).fetchall()
+            self.assertEqual(len(self._54e844ebfbc3_deployments),
+                             len(deployments_found))
             for deployment in deployments_found:
                 # check deployment
                 self.assertIn(deployment.uuid, original_deployments)
                 self.assertIn(deployment.name, original_deployments)
 
                 config = json.loads(deployment.config)
                 if config != original_deployments[deployment.uuid]:
@@ -489,15 +492,15 @@
                                "File some2.py, line ...\nSomeCls: msg"}},
         ]
 
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
 
         self._08e1515a576c_deployment_uuid = "08e1515a576c-uuuu-uuuu-iiii-dddd"
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{"uuid": self._08e1515a576c_deployment_uuid,
                   "name": self._08e1515a576c_deployment_uuid,
                   "config": b("{}"),
                   "enum_deployments_status":
                   consts.DeployStatus.DEPLOY_FINISHED,
@@ -511,25 +514,27 @@
                     [{"uuid": i,
                       "verification_log": log,
                       "status": "failed",
                       "enum_tasks_status": "failed",
                       "deployment_uuid": self._08e1515a576c_deployment_uuid
                       }])
 
-    def _check_08e1515a576c(self, engine, data):
+    def _check_08e1515a576c(self, engine: sa.engine.Engine):
         self.assertEqual("08e1515a576c",
                          db.schema.schema_revision(engine=engine))
 
         tasks = self._08e1515a576c_logs
 
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             tasks_found = conn.execute(task_table.select()).fetchall()
+            self.assertEqual(len(self._08e1515a576c_logs),
+                             len(tasks_found))
             for task in tasks_found:
                 actual_log = json.loads(task.verification_log)
                 self.assertIsInstance(actual_log, dict)
                 expected = tasks[int(task.uuid)]["post"]
                 for key in expected:
                     self.assertEqual(expected[key], actual_log[key])
 
@@ -545,15 +550,15 @@
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
         taskresult_table = db_utils.get_table(engine, "task_results")
 
         self._e654a0648db0_task_uuid = str(uuid.uuid4())
         self._e654a0648db0_deployment_uuid = str(uuid.uuid4())
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{
                     "uuid": self._e654a0648db0_deployment_uuid,
                     "name": self._e654a0648db0_deployment_uuid,
                     "config": "{}",
                     "enum_deployments_status": consts.DeployStatus.DEPLOY_INIT,
@@ -601,26 +606,26 @@
                             "full_duration": 142,
                             "sla": [{"success": True}, {"success": False}]
                         })
                     }
                 ]
             )
 
-    def _check_e654a0648db0(self, engine, data):
+    def _check_e654a0648db0(self, engine: sa.engine.Engine):
         self.assertEqual(
             "e654a0648db0", db.schema.schema_revision(engine=engine))
 
         task_table = db_utils.get_table(engine, "tasks")
         subtask_table = db_utils.get_table(engine, "subtasks")
         workload_table = db_utils.get_table(engine, "workloads")
         workloaddata_table = db_utils.get_table(engine, "workloaddata")
         tag_table = db_utils.get_table(engine, "tags")
         deployment_table = db_utils.get_table(engine, "deployments")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
 
             # Check task
 
             tasks_found = conn.execute(
                 task_table.select().
                 where(task_table.c.uuid == self._e654a0648db0_task_uuid)
             ).fetchall()
@@ -785,15 +790,15 @@
                       == self._e654a0648db0_deployment_uuid)
             )
 
     def _pre_upgrade_6ad4f426f005(self, engine):
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
         task_result_table = db_utils.get_table(engine, "task_results")
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             # create deployment
             conf = {
                 "admin": {"username": "admin",
                           "password": "passwd",
                           "project_name": "admin"},
                 "auth_url": "http://example.com:5000/v3",
                 "region_name": "RegionOne",
@@ -826,22 +831,22 @@
                 [{
                     "task_uuid": "my_task",
                     "key": json.dumps({}),
                     "data": json.dumps({}),
                 }]
             )
 
-    def _check_6ad4f426f005(self, engine, data):
+    def _check_6ad4f426f005(self, engine: sa.engine.Engine):
         self.assertEqual("6ad4f426f005",
                          db.schema.schema_revision(engine=engine))
 
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
         task_result_table = db_utils.get_table(engine, "task_results")
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             task_results = conn.execute(task_result_table.select()).fetchall()
             self.assertEqual(1, len(task_results))
             task_result = task_results[0]
 
             # check that "hooks" field added
             self.assertEqual({"hooks": []}, json.loads(task_result.data))
 
@@ -895,38 +900,40 @@
                 "auth_url": "http://example.com:5000/v3",
                 "region_name": "RegionOne",
                 "type": "ExistingCloud"},
         }
         deployment_table = db_utils.get_table(engine, "deployments")
 
         deployment_status = consts.DeployStatus.DEPLOY_FINISHED
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             for deployment in self._32fada9b2fde_deployments:
                 conf = json.dumps(
                     self._32fada9b2fde_deployments[deployment])
                 conn.execute(
                     deployment_table.insert(),
                     [{"uuid": deployment, "name": deployment,
                       "config": conf,
                       "enum_deployments_status": deployment_status,
                       "credentials": b(json.dumps([])),
                       "users": b(json.dumps([]))
                       }])
 
-    def _check_32fada9b2fde(self, engine, data):
+    def _check_32fada9b2fde(self, engine: sa.engine.Engine):
         self.assertEqual("32fada9b2fde",
                          db.schema.schema_revision(engine=engine))
 
         original_deployments = self._32fada9b2fde_deployments
 
         deployment_table = db_utils.get_table(engine, "deployments")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             deployments_found = conn.execute(
                 deployment_table.select()).fetchall()
+            self.assertEqual(len(self._32fada9b2fde_deployments),
+                             len(deployments_found))
             for deployment in deployments_found:
                 # check deployment
                 self.assertIn(deployment.uuid, original_deployments)
                 self.assertIn(deployment.name, original_deployments)
 
                 config = json.loads(deployment.config)
                 if config != original_deployments[deployment.uuid]:
@@ -999,28 +1006,28 @@
         deployment_table = db_utils.get_table(engine, "deployments")
         verifications_table = db_utils.get_table(engine, "verifications")
         vresults_table = db_utils.get_table(engine,
                                             "verification_results")
 
         deployment_status = consts.DeployStatus.DEPLOY_FINISHED
         vstatus = consts.TaskStatus.FINISHED
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{"uuid": self._484cd9413e66_deployment_uuid,
                   "name": self._484cd9413e66_deployment_uuid,
                   "config": b(json.dumps([])),
                   "enum_deployments_status": deployment_status,
                   "credentials": b(json.dumps([])),
                   "users": b(json.dumps([]))
                   }])
 
             for i in range(len(self._484cd9413e66_verifications)):
                 verification = self._484cd9413e66_verifications[i]
-                vuuid = "uuid-%s" % i
+                vuuid = f"484cd9413e66-uuid-{i}"
                 conn.execute(
                     verifications_table.insert(),
                     [{"uuid": vuuid,
                       "deployment_uuid":
                       self._484cd9413e66_deployment_uuid,
                       "status": vstatus,
                       "set_name": verification["set_name"],
@@ -1035,23 +1042,26 @@
                 conn.execute(
                     vresults_table.insert(),
                     [{"uuid": vuuid,
                       "verification_uuid": vuuid,
                       "data": json.dumps(data)
                       }])
 
-    def _check_484cd9413e66(self, engine, data):
+    def _check_484cd9413e66(self, engine: sa.engine.Engine):
         self.assertEqual("484cd9413e66",
                          db.schema.schema_revision(engine=engine))
 
         verifications_table = db_utils.get_table(engine, "verifications")
+        deployment_table = db_utils.get_table(engine, "deployments")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             verifications = conn.execute(
                 verifications_table.select()).fetchall()
+            self.assertEqual(len(self._484cd9413e66_verifications),
+                             len(verifications))
             for i in range(len(verifications)):
                 verification_orig = self._484cd9413e66_verifications[i]
                 verification = verifications[i]
                 total = {"time": verification.tests_duration,
                          "failures": verification.failures,
                          "skipped": verification.skipped,
                          "success": verification.success,
@@ -1086,21 +1096,19 @@
 
                 self.assertEqual(
                     verification_orig["total"].get("unexpected_success", 0),
                     verification.unexpected_success)
                 self.assertEqual(
                     verification_orig["total"].get("expected_failures", 0),
                     verification.expected_failures)
-
                 conn.execute(
                     verifications_table.delete().where(
-                        verifications_table.c.uuid == verification.uuid)
+                        verifications_table.c.uuid == verification.uuid
+                    )
                 )
-
-            deployment_table = db_utils.get_table(engine, "deployments")
             conn.execute(
                 deployment_table.delete().where(
                     deployment_table.c.uuid
                     == self._484cd9413e66_deployment_uuid)
             )
 
     def _pre_upgrade_37fdbb373e8d(self, engine):
@@ -1138,15 +1146,16 @@
         ]
 
         deployment_table = db_utils.get_table(engine, "deployments")
         verifiers_table = db_utils.get_table(engine, "verifiers")
         verifications_table = db_utils.get_table(engine, "verifications")
 
         deployment_status = consts.DeployStatus.DEPLOY_FINISHED
-        with engine.connect() as conn:
+        with engine.begin() as conn:
+
             conn.execute(
                 deployment_table.insert(),
                 [{"uuid": self._37fdbb373e8d_deployment_uuid,
                   "name": self._37fdbb373e8d_deployment_uuid,
                   "config": b(json.dumps([])),
                   "enum_deployments_status": deployment_status,
                   "credentials": b(json.dumps([])),
@@ -1169,20 +1178,22 @@
                       "deployment_uuid":
                           self._37fdbb373e8d_deployment_uuid,
                       "verifier_uuid": self._37fdbb373e8d_verifier_uuid,
                       "status": consts.VerificationStatus.FINISHED,
                       "tests": json.dumps(tests)
                       }])
 
-    def _check_37fdbb373e8d(self, engine, data):
+    def _check_37fdbb373e8d(self, engine: sa.engine.Engine):
         self.assertEqual("37fdbb373e8d",
                          db.schema.schema_revision(engine=engine))
 
         verifications_table = db_utils.get_table(engine, "verifications")
-        with engine.connect() as conn:
+        deployment_table = db_utils.get_table(engine, "deployments")
+
+        with engine.begin() as conn:
             verifications = conn.execute(
                 verifications_table.select()).fetchall()
             self.assertEqual(len(verifications),
                              len(self._37fdbb373e8d_verifications_tests))
 
             for i in range(len(verifications)):
                 v = verifications[i]
@@ -1195,15 +1206,14 @@
                 self.assertEqual(expected_tests, updated_tests)
 
                 conn.execute(
                     verifications_table.delete().where(
                         verifications_table.c.uuid == v.uuid)
                 )
 
-            deployment_table = db_utils.get_table(engine, "deployments")
             conn.execute(
                 deployment_table.delete().where(
                     deployment_table.c.uuid
                     == self._37fdbb373e8d_deployment_uuid)
             )
 
     def _pre_upgrade_a6f364988fc2(self, engine):
@@ -1222,37 +1232,42 @@
                 "uuid": "uuid-3",
                 "type": "task",
                 "tag": "tag-3"
             }
         ]
 
         tags_table = db_utils.get_table(engine, "tags")
-        with engine.connect() as conn:
-            for t in self._a6f364988fc2_tags:
+        with engine.begin() as conn:
+            for tag in self._a6f364988fc2_tags:
                 conn.execute(
                     tags_table.insert(),
                     [{
-                        "uuid": t["uuid"],
-                        "enum_tag_types": t["type"],
-                        "type": t["type"],
-                        "tag": t["tag"]
+                        "uuid": tag["uuid"],
+                        "enum_tag_types": tag["type"],
+                        "type": tag["type"],
+                        "tag": tag["tag"]
                     }])
 
-    def _check_a6f364988fc2(self, engine, data):
+    def _check_a6f364988fc2(self, engine: sa.engine.Engine):
         self.assertEqual("a6f364988fc2",
                          db.schema.schema_revision(engine=engine))
 
         tags_table = db_utils.get_table(engine, "tags")
-        with engine.connect() as conn:
-            tags = conn.execute(tags_table.select()).fetchall()
+        with engine.begin() as conn:
+            tags: t.Sequence[sa.Row] = (
+                conn.execute(tags_table.select()).fetchall()
+            )
             self.assertEqual(len(tags), len(self._a6f364988fc2_tags))
 
             for i in range(len(tags)):
+                actual_tag = tags[i]._mapping
                 for k in ("uuid", "type", "tag"):
-                    self.assertEqual(self._a6f364988fc2_tags[i][k], tags[i][k])
+                    self.assertEqual(
+                        self._a6f364988fc2_tags[i][k], actual_tag[k]
+                    )
 
                 conn.execute(
                     tags_table.delete().where(
                         tags_table.c.uuid == tags[i].uuid))
 
     def _pre_upgrade_f33f4610dcda(self, engine):
         self._f33f4610dcda_deployment_uuid = "f33f4610dcda-deployment"
@@ -1272,15 +1287,15 @@
         ]
 
         deployment_table = db_utils.get_table(engine, "deployments")
         verifiers_table = db_utils.get_table(engine, "verifiers")
         verifications_table = db_utils.get_table(engine, "verifications")
 
         deployment_status = consts.DeployStatus.DEPLOY_FINISHED
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{"uuid": self._f33f4610dcda_deployment_uuid,
                   "name": self._f33f4610dcda_deployment_uuid,
                   "config": b(json.dumps([])),
                   "enum_deployments_status": deployment_status,
                   "credentials": b(json.dumps([])),
@@ -1303,20 +1318,20 @@
                       "deployment_uuid": self._f33f4610dcda_deployment_uuid,
                       "verifier_uuid": self._f33f4610dcda_verifier_uuid,
                       "status": v["status"],
                       "failures": v["failures"],
                       "unexpected_success": v["unexpected_success"]
                       }])
 
-    def _check_f33f4610dcda(self, engine, data):
+    def _check_f33f4610dcda(self, engine: sa.engine.Engine):
         self.assertEqual("f33f4610dcda",
                          db.schema.schema_revision(engine=engine))
 
         verifications_table = db_utils.get_table(engine, "verifications")
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             verifications = conn.execute(
                 verifications_table.select()).fetchall()
             self.assertEqual(len(verifications),
                              len(self._f33f4610dcda_verifications))
 
             for i in range(len(verifications)):
                 if "new_status" in self._f33f4610dcda_verifications[i]:
@@ -1357,78 +1372,78 @@
             "should-be-changed-2": {
                 "uuid": "should-be-changed-2",
                 "deployment_uuid": self._4ef544102ba7_deployment_uuid,
                 "validation_result": {},
                 "status": "verifying"},
         }
         deployment_table = db_utils.get_table(engine, "deployments")
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{"uuid": self._4ef544102ba7_deployment_uuid,
                   "name": self._4ef544102ba7_deployment_uuid,
                   "config": b(json.dumps([])),
                   "enum_deployments_status":
                   consts.DeployStatus.DEPLOY_FINISHED,
                   "credentials": b(json.dumps([])),
                   "users": b(json.dumps([]))
                   }])
 
         task_table = db_utils.get_table(engine, "tasks")
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             for task in self.tasks:
                 conn.execute(
                     task_table.insert(),
                     [{
                         "deployment_uuid": self.tasks[task][
                             "deployment_uuid"],
                         "status": self.tasks[task]["status"],
                         "validation_result": json.dumps(
                             self.tasks[task]["validation_result"]),
                         "uuid": self.tasks[task]["uuid"]
                     }])
 
         subtask_table = db_utils.get_table(engine, "subtasks")
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             for task in self.tasks:
                 conn.execute(
                     subtask_table.insert(),
                     [{
                         "task_uuid": self.tasks[task]["uuid"],
                         "status": consts.SubtaskStatus.RUNNING,
                         "context": json.dumps({}),
                         "sla": json.dumps({}),
                         "run_in_parallel": False,
                         "uuid": "subtask_" + self.tasks[task]["uuid"]
                     }])
 
-    def _check_4ef544102ba7(self, engine, data):
+    def _check_4ef544102ba7(self, engine: sa.engine.Engine):
         self.assertEqual("4ef544102ba7",
                          db.schema.schema_revision(engine=engine))
 
         org_tasks = self.tasks
 
         task_table = db_utils.get_table(engine, "tasks")
         subtask_table = db_utils.get_table(engine, "subtasks")
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             subtasks_found = conn.execute(
                 subtask_table.select()).fetchall()
             for subtask in subtasks_found:
                 conn.execute(
                     subtask_table.delete().where(
                         subtask_table.c.id == subtask.id)
                 )
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             tasks_found = conn.execute(
                 task_table.select()).fetchall()
             self.assertEqual(3, len(tasks_found))
             for task in tasks_found:
-                self.assertIn("uuid", task)
-                self.assertIn("status", task)
+                self.assertIn("uuid", task._mapping)
+                self.assertIn("status", task._mapping)
 
                 if task.status != org_tasks[task.uuid]["status"]:
                     if task.uuid.startswith("should-not-be-changed"):
                         self.fail("Config of deployment '%s' is changes, but "
                                   "should not." % task.uuid)
                     if task.status != "crashed" and task.uuid == (
                             "should-be-changed-1"):
@@ -1462,36 +1477,36 @@
             ("multi-cred", [["spam", {"foo": "bar1"}],
                             ["eggs", {"foo": "bar2"}]]),
         ]
 
         deployment_table = db_utils.get_table(engine, "deployments")
         deployment_status = consts.DeployStatus.DEPLOY_FINISHED
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             for deployment, creds in self._92aaaa2a6bb3_deployments:
                 conn.execute(
                     deployment_table.insert(),
                     [{"uuid": deployment, "name": deployment,
                       "config": json.dumps({}),
                       "enum_deployments_status": deployment_status,
                       "credentials": pickle.dumps(creds),
                       }])
 
-    def _check_92aaaa2a6bb3(self, engine, data):
+    def _check_92aaaa2a6bb3(self, engine: sa.engine.Engine):
         expected_credentials = [
             ("1-cred", {"openstack": [{"foo": "bar"}]}),
             ("2-cred", {"openstack": [{"foo": "bar1"},
                                       {"foo": "bar2"}]}),
             ("multi-cred", {"spam": [{"foo": "bar1"}],
                             "eggs": [{"foo": "bar2"}]}),
         ]
 
         deployment_table = db_utils.get_table(engine, "deployments")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             for deployment, expected_creds in expected_credentials:
 
                 dep_obj = conn.execute(
                     deployment_table.select().where(
                         deployment_table.c.uuid == deployment)).fetchone()
                 self.assertEqual(
                     expected_creds, json.loads(dep_obj.credentials))
@@ -1523,15 +1538,15 @@
                  "load_duration": 3},
                 {"uuid": str(uuid.uuid4()),
                  "pass_sla": False,
                  "load_duration": 7}
             ]
         }
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{
                     "uuid": deployment_uuid,
                     "name": str(uuid.uuid4()),
                     "config": "{}",
                     "enum_deployments_status": consts.DeployStatus.DEPLOY_INIT,
@@ -1586,21 +1601,21 @@
                             "sla_results": "",
                             "args": "",
                             "load_duration": workload["load_duration"],
                             "pass_sla": workload["pass_sla"]
                         }]
                     )
 
-    def _check_35fe16d4ab1c(self, engine, data):
+    def _check_35fe16d4ab1c(self, engine: sa.engine.Engine):
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
         subtask_table = db_utils.get_table(engine, "subtasks")
         workload_table = db_utils.get_table(engine, "workloads")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             task_id = self._35fe16d4ab1c_task_uuid
             task_obj = conn.execute(
                 task_table.select().where(
                     task_table.c.uuid == task_id)).fetchone()
             self.assertFalse(task_obj.pass_sla)
             subtask_duration = dict(
                 [(k, sum([w["load_duration"] for w in v]))
@@ -1644,15 +1659,15 @@
         self._7948b83229f6_workloads = {
             str(uuid.uuid4()): {"preprocessed": 1, "expected": 1},
             str(uuid.uuid4()): {"preprocessed": 0, "expected": None},
             str(uuid.uuid4()): {"preprocessed": 0, "expected": 0,
                                 "wdata": True},
             str(uuid.uuid4()): {"preprocessed": -1, "expected": None}}
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{
                     "uuid": self._7948b83229f6_deployment_uuid,
                     "name": str(uuid.uuid4()),
                     "config": "{}",
                     "enum_deployments_status": consts.DeployStatus.DEPLOY_INIT,
@@ -1728,27 +1743,32 @@
                             "failed_iteration_count": 0,
                             "chunk_size": 0,
                             "compressed_chunk_size": 0,
                             "chunk_data": b(json.dumps([]))
                         }]
                     )
 
-    def _check_7948b83229f6(self, engine, data):
+    def _check_7948b83229f6(self, engine: sa.engine.Engine):
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
         subtask_table = db_utils.get_table(engine, "subtasks")
         workload_table = db_utils.get_table(engine, "workloads")
         wdata_table = db_utils.get_table(engine, "workloaddata")
 
         subtask_uuid = None
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             task_uuid = self._7948b83229f6_task_uuid
-            for workload in conn.execute(workload_table.select().where(
-                    workload_table.c.task_uuid == task_uuid)).fetchall():
+
+            workloads_found = conn.execute(workload_table.select().where(
+                workload_table.c.task_uuid == task_uuid)).fetchall()
+            self.assertEqual(len(self._7948b83229f6_workloads),
+                             len(workloads_found))
+
+            for workload in workloads_found:
                 if subtask_uuid is None:
                     subtask_uuid = workload.subtask_uuid
                 if workload.uuid not in self._7948b83229f6_workloads:
                     self.fail("Unknown workload found for 7948b83229f6 "
                               "migration.")
                 original = self._7948b83229f6_workloads[workload.uuid]
                 self.assertEqual(original["expected"],
@@ -1798,15 +1818,15 @@
                                    "name": "foo",
                                    "trigger": {"name": "bar",
                                                "args": {"arg2": "v2"}}}}
                 ]
             }
         ]
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{
                     "uuid": self._046a38742e89_deployment_uuid,
                     "name": str(uuid.uuid4()),
                     "config": "{}",
                     "enum_deployments_status": consts.DeployStatus.DEPLOY_INIT,
@@ -1863,26 +1883,30 @@
                         "load_duration": 0,
                         "pass_sla": True,
                         "min_duration": 0,
                         "max_duration": 1
                     }]
                 )
 
-    def _check_046a38742e89(self, engine, data):
+    def _check_046a38742e89(self, engine: sa.engine.Engine):
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
         subtask_table = db_utils.get_table(engine, "subtasks")
         workload_table = db_utils.get_table(engine, "workloads")
 
         subtask_uuid = None
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             task_uuid = self._046a38742e89_task_uuid
-            for workload in conn.execute(workload_table.select().where(
-                    workload_table.c.task_uuid == task_uuid)).fetchall():
+
+            workloads_found = conn.execute(workload_table.select().where(
+                workload_table.c.task_uuid == task_uuid)).fetchall()
+            self.assertEqual(2, len(workloads_found))
+
+            for workload in workloads_found:
                 if subtask_uuid is None:
                     subtask_uuid = workload.subtask_uuid
 
                 runner = json.loads(workload.runner)
                 self.assertNotIn("type", runner)
 
                 hooks = json.loads(workload.hooks)
@@ -2053,15 +2077,15 @@
                                       "success": "100.0%"}
                          }
                      ]
                  }
              }}}
         ]
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{
                     "uuid": self._4394bdc32cfd_deployment_uuid,
                     "name": str(uuid.uuid4()),
                     "config": "{}",
                     "enum_deployments_status": consts.DeployStatus.DEPLOY_INIT,
@@ -2134,27 +2158,31 @@
                         "failed_iteration_count": 0,
                         "chunk_size": 0,
                         "compressed_chunk_size": 0,
                         "chunk_data": json.dumps({"raw": workload["data"]})
                     }]
                 )
 
-    def _check_4394bdc32cfd(self, engine, data):
+    def _check_4394bdc32cfd(self, engine: sa.engine.Engine):
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
         subtask_table = db_utils.get_table(engine, "subtasks")
         workload_table = db_utils.get_table(engine, "workloads")
         wdata_table = db_utils.get_table(engine, "workloaddata")
 
         task_uuid = None
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             subtask_id = self._4394bdc32cfd_subtask
-            for workload in conn.execute(workload_table.select().where(
-                    workload_table.c.subtask_uuid == subtask_id)).fetchall():
+
+            workloads_found = conn.execute(workload_table.select().where(
+                workload_table.c.subtask_uuid == subtask_id)).fetchall()
+            self.assertEqual(2, len(workloads_found))
+
+            for workload in workloads_found:
                 if task_uuid is None:
                     task_uuid = workload.task_uuid
                 original = [w for w in self._4394bdc32cfd_workloads
                             if w["uuid"] == workload.uuid][0]
                 if workload.start_time is None:
                     start_time = None
                 else:
@@ -2228,15 +2256,15 @@
                 "context": {"foobar": {"foo": "bar"}},
                 "with_fake_context": True,
                 "full_duration": 10,
                 "load_duration": 3
             }
         }
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{
                     "uuid": self._046a38742e89_deployment_uuid,
                     "name": str(uuid.uuid4()),
                     "config": "{}",
                     "enum_deployments_status": consts.DeployStatus.DEPLOY_INIT,
@@ -2293,46 +2321,46 @@
                     "start_time": w["start_time"],
                     "pass_sla": True,
                     "min_duration": 0,
                     "max_duration": 1
                 } for w_uuid, w in self._dc46687661df_workloads.items()]
             )
 
-    def _check_dc46687661df(self, engine, data):
+    def _check_dc46687661df(self, engine: sa.engine.Engine):
         deployment_table = db_utils.get_table(engine, "deployments")
         task_table = db_utils.get_table(engine, "tasks")
         subtask_table = db_utils.get_table(engine, "subtasks")
         workload_table = db_utils.get_table(engine, "workloads")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             task_uuid = self._dc46687661df_task_uuid
             for w_uuid, w in self._dc46687661df_workloads.items():
                 workload = conn.execute(workload_table.select().where(
                     workload_table.c.uuid == w_uuid)).first()
 
-                self.assertNotIn("context", workload)
-                self.assertNotIn("context_execution", workload)
+                self.assertNotIn("context", workload._mapping)
+                self.assertNotIn("context_execution", workload._mapping)
 
                 self.assertEqual(w["context"],
-                                 json.loads(workload["contexts"]))
+                                 json.loads(workload.contexts))
                 if w["start_time"] is None:
-                    self.assertEqual("[]", workload["contexts_results"])
+                    self.assertEqual("[]", workload.contexts_results)
                 elif w.get("with_fake_context", False):
                     self.assertEqual([{
                         "plugin_cfg": {"description": mock.ANY},
                         "plugin_name": "AllExecutedContexts",
                         "setup": {"started_at": 1483221600.0,
                                   "finished_at": 1483221601.99,
                                   "atomic_actions": [],
                                   "error": None},
                         "cleanup": {"started_at": 1483221605.01,
                                     "finished_at": 1483221609.9,
                                     "atomic_actions": [],
                                     "error": None}}],
-                        json.loads(workload["contexts_results"]))
+                        json.loads(workload.contexts_results))
                 else:
                     self.assertEqual([{
                         "plugin_name": "AllExecutedContexts",
                         "plugin_cfg": {
                             "description": mock.ANY,
                             "order_of_execution": {
                                 "note": mock.ANY,
@@ -2344,32 +2372,32 @@
                                   "finished_at": 1483221601.99,
                                   "atomic_actions": [],
                                   "error": None},
                         "cleanup": {"started_at": 1483221605.01,
                                     "finished_at": 1483221609.9,
                                     "atomic_actions": [],
                                     "error": None}}],
-                        json.loads(workload["contexts_results"]))
+                        json.loads(workload.contexts_results))
 
                 conn.execute(
                     workload_table.delete().where(
                         workload_table.c.uuid == workload.uuid))
 
             subtask = conn.execute(subtask_table.select().where(
                 subtask_table.c.task_uuid == task_uuid)).first()
 
-            self.assertNotIn("context", subtask)
-            self.assertNotIn("context_execution", subtask)
+            self.assertNotIn("context", subtask._mapping)
+            self.assertNotIn("context_execution", subtask._mapping)
 
-            self.assertEqual("{}", subtask["contexts"])
-            self.assertEqual("[]", subtask["contexts_results"])
+            self.assertEqual("{}", subtask.contexts)
+            self.assertEqual("[]", subtask.contexts_results)
 
             conn.execute(
                 subtask_table.delete().where(
-                    subtask_table.c.uuid == subtask["uuid"]))
+                    subtask_table.c.uuid == subtask.uuid))
 
             conn.execute(
                 task_table.delete().where(task_table.c.uuid == task_uuid))
 
             deployment_uuid = self._046a38742e89_deployment_uuid
             conn.execute(
                 deployment_table.delete().where(
@@ -2413,32 +2441,32 @@
                 "https_insecure": False,
                 "https_cacert": "",
                 "extra": {}
             }),
             # some custom unknown thing
             (str(uuid.uuid4()), {"some_special_deployment": "foo"})
         ]
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{
                     "uuid": d_uuid,
                     "name": str(uuid.uuid4()),
                     "config": (
                         json.dumps(d_cfg) if d_cfg
                         else b(json.dumps(d_cfg))),
                     "enum_deployments_status": consts.DeployStatus.DEPLOY_INIT,
                     "credentials": b(json.dumps([]))
                 } for d_uuid, d_cfg in self._dc0fe6de6786_deployments]
             )
 
-    def _check_dc0fe6de6786(self, engine, data):
+    def _check_dc0fe6de6786(self, engine: sa.engine.Engine):
         deployment_table = db_utils.get_table(engine, "deployments")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
 
             for d_uuid, d_cfg in self._dc0fe6de6786_deployments:
                 deployment = conn.execute(deployment_table.select().where(
                     deployment_table.c.uuid == d_uuid)).first()
                 config = json.loads(deployment.config)
                 if "type" in config:
                     self.assertEqual(config["type"],
@@ -2486,15 +2514,15 @@
             # some custom unknown thing
             (str(uuid.uuid4()), {"some_special_deployment": "foo"})
         ]
         self._bc908ac9a1fc_task_uuid = str(uuid.uuid4())
         self._bc908ac9a1fc_verifier_uuid = str(uuid.uuid4())
         self._bc908ac9a1fc_verification_uuid = str(uuid.uuid4())
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
             conn.execute(
                 deployment_table.insert(),
                 [{
                     "uuid": d_uuid,
                     "name": str(uuid.uuid4()),
                     "config": (
                         json.dumps(d_cfg) if d_cfg
@@ -2536,53 +2564,53 @@
                     "verifier_uuid": self._bc908ac9a1fc_verifier_uuid,
                     "status": consts.VerificationStatus.INIT,
                     "created_at": dt.datetime.utcnow(),
                     "updated_at": dt.datetime.utcnow(),
                 }]
             )
 
-    def _check_bc908ac9a1fc(self, engine, data):
+    def _check_bc908ac9a1fc(self, engine: sa.engine.Engine):
         env_table = db_utils.get_table(engine, "envs")
         platform_table = db_utils.get_table(engine, "platforms")
         task_table = db_utils.get_table(engine, "tasks")
         verifier_table = db_utils.get_table(engine, "verifiers")
         verification_table = db_utils.get_table(engine, "verifications")
 
-        with engine.connect() as conn:
+        with engine.begin() as conn:
 
             task = conn.execute(task_table.select().where(
                 task_table.c.uuid == self._bc908ac9a1fc_task_uuid)).first()
-            self.assertNotIn("deployment_uuid", task)
-            self.assertIn("env_uuid", task)
+            self.assertNotIn("deployment_uuid", task._mapping)
+            self.assertIn("env_uuid", task._mapping)
             self.assertEqual(self._bc908ac9a1fc_deployments[0][0],
-                             task["env_uuid"])
+                             task.env_uuid)
             conn.execute(
                 task_table.delete().where(
                     task_table.c.uuid == self._bc908ac9a1fc_task_uuid))
 
             v_id = self._bc908ac9a1fc_verification_uuid
             verification = conn.execute(verification_table.select().where(
                 verification_table.c.uuid == v_id)).first()
-            self.assertNotIn("deployment_uuid", verification)
-            self.assertIn("env_uuid", verification)
+            self.assertNotIn("deployment_uuid", verification._mapping)
+            self.assertIn("env_uuid", verification._mapping)
             self.assertEqual(self._bc908ac9a1fc_deployments[0][0],
-                             verification["env_uuid"])
+                             verification.env_uuid)
             conn.execute(
                 verification_table.delete().where(
                     verification_table.c.uuid == v_id))
             conn.execute(
                 verifier_table.delete().where(
                     verifier_table.c.uuid == self._bc908ac9a1fc_verifier_uuid))
 
             for d_uuid, d_cfg in self._bc908ac9a1fc_deployments:
                 env = conn.execute(env_table.select().where(
                     env_table.c.uuid == d_uuid)).first()
                 if d_cfg.get("creds", {}):
                     # openstack deployment
-                    env_spec = json.loads(env["spec"])
+                    env_spec = json.loads(env.spec)
                     self.assertEqual({"existing@openstack"},
                                      set(env_spec.keys()))
                     self.assertEqual(
                         d_cfg["creds"]["openstack"],
                         env_spec["existing@openstack"])
 
                     platforms = conn.execute(platform_table.select().where(
@@ -2610,18 +2638,18 @@
 
                     conn.execute(
                         platform_table.delete().where(
                             platform_table.c.env_uuid == d_uuid))
                 else:
                     if "creds" in d_cfg:
                         # empty deployment
-                        self.assertEqual({}, json.loads(env["spec"]))
+                        self.assertEqual({}, json.loads(env.spec))
                     else:
                         # something
-                        self.assertEqual(d_cfg, json.loads(env["spec"]))
+                        self.assertEqual(d_cfg, json.loads(env.spec))
 
                     platforms = conn.execute(platform_table.select().where(
                         platform_table.c.env_uuid == d_uuid)).fetchall()
                     self.assertEqual(0, len(platforms))
 
                 conn.execute(
                     env_table.delete().where(
```

### Comparing `rally-4.0.0/tests/unit/common/db/test_migrations_base.py` & `rally-4.1.0/tests/unit/common/db/test_migrations_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,16 +101,16 @@
 
         self._configure(engine)
         # NOTE(ikhudoshyn): Now DB contains certain schema
         # so we can not execute all migrations starting from
         # init. So we cleanup the DB.
         db.schema.schema_cleanup()
         up_and_down_versions = self._up_and_down_versions()
-        for ver_up, ver_down in up_and_down_versions:
-            self._migrate_up(engine, ver_up, with_data=True)
+        for ver_up, prev_version in up_and_down_versions:
+            self._migrate_up(engine, ver_up)
 
     def _get_version_from_db(self, engine):
         """Return latest version for each type of migrate repo from db."""
         conn = engine.connect()
         try:
             context = migration.MigrationContext.configure(conn)
             version = context.get_current_revision() or "-1"
@@ -122,34 +122,31 @@
         """Base method for manipulation with migrate repo.
 
         It will upgrade the actual database.
         """
 
         self._alembic_command(cmd, engine, self.ALEMBIC_CONFIG, version)
 
-    def _migrate_up(self, engine, version, with_data=False):
+    def _migrate_up(self, engine, version):
         """Migrate up to a new version of the db.
 
         We allow for data insertion and post checks at every
         migration version with special _pre_upgrade_### and
         _check_### functions in the main test.
         """
         # NOTE(sdague): try block is here because it's impossible to debug
         # where a failed data migration happens otherwise
         check_version = version
         try:
-            if with_data:
-                data = None
-                pre_upgrade = getattr(
-                    self, "_pre_upgrade_%s" % check_version, None)
-                if pre_upgrade:
-                    data = pre_upgrade(engine)
+            pre_upgrade = getattr(
+                self, "_pre_upgrade_%s" % check_version, None)
+            if pre_upgrade:
+                pre_upgrade(engine)
             self._migrate(engine, version, "upgrade")
             self.assertEqual(version, self._get_version_from_db(engine))
-            if with_data:
-                check = getattr(self, "_check_%s" % check_version, None)
-                if check:
-                    check(engine, data)
+            check = getattr(self, "_check_%s" % check_version, None)
+            if check:
+                check(engine)
         except Exception:
             LOG.error("Failed to migrate to version %(ver)s on engine %(eng)s"
                       % {"ver": version, "eng": engine})
             raise
```

### Comparing `rally-4.0.0/tests/unit/common/db/test_types.py` & `rally-4.1.0/tests/unit/common/db/test_types.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/io/subunit_v2.stream` & `rally-4.1.0/tests/unit/common/io/subunit_v2.stream`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/io/test_junit.py` & `rally-4.1.0/tests/unit/common/io/test_junit.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/io/test_subunit_v2.py` & `rally-4.1.0/tests/unit/common/io/test_subunit_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                           "unexpected_success": 1}, result.totals)
         self.assertEqual(len(result.tests), result.totals["tests_count"])
 
         skipped_tests = result.filter_tests("skip")
         skipped_test = "test_foo.SimpleTestCase.test_skip_something"
 
         self.assertEqual(result.totals["skipped"], len(skipped_tests))
-        self.assertSequenceEqual([skipped_test], skipped_tests.keys())
+        self.assertSequenceEqual([skipped_test], list(skipped_tests))
         self.assertEqual(
             {"status": "skip", "reason": "This should be skipped.",
              "duration": "0.000", "name": skipped_test, "tags": [],
              "timestamp": "2015-06-03T08:46:17+0000"},
             skipped_tests[skipped_test])
 
         failed_tests = result.filter_tests("fail")
```

### Comparing `rally-4.0.0/tests/unit/common/objects/test_deploy.py` & `rally-4.1.0/tests/unit/common/objects/test_deploy.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/objects/test_task.py` & `rally-4.1.0/tests/unit/common/objects/test_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,15 +378,15 @@
                                      data, expected=False,
                                      validate_output_return_value=None,
                                      validate_output_calls=None):
         task = objects.Task(task=self.task)
         mock_validate_output.return_value = validate_output_return_value
         self.assertEqual(expected,
                          task.result_has_valid_schema(data),
-                         message=repr(data))
+                         msg=repr(data))
         if validate_output_calls:
             mock_validate_output.assert_has_calls(
                 [mock.call(*args) for args in validate_output_calls],
                 any_order=True)
 
 
 class SubtaskTestCase(test.TestCase):
```

### Comparing `rally-4.0.0/tests/unit/common/objects/test_verification.py` & `rally-4.1.0/tests/unit/common/objects/test_verification.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/objects/test_verifier.py` & `rally-4.1.0/tests/unit/common/objects/test_verifier.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/plugin/test_discover.py` & `rally-4.1.0/tests/unit/common/plugin/test_discover.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/plugin/test_info.py` & `rally-4.1.0/tests/unit/common/plugin/test_info.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/plugin/test_meta.py` & `rally-4.1.0/tests/unit/common/plugin/test_meta.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/plugin/test_plugin.py` & `rally-4.1.0/tests/unit/common/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/test_broker.py` & `rally-4.1.0/tests/unit/common/test_broker.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/test_logging.py` & `rally-4.1.0/tests/unit/common/test_logging.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/test_opts.py` & `rally-4.1.0/tests/unit/common/test_opts.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 class RegisterOptsTestCase(test.TestCase):
     @mock.patch("rally.common.opts.register_opts")
     def test_register_options_from_path(self, mock_register_opts):
 
         opts.register_options_from_path("unexisting.path.without.method.name")
         self.assertFalse(mock_register_opts.called)
-        self.assertIsEmpty(opts._registered_paths)
+        self.assertEqual(0, len(opts._registered_paths))
 
         opts.register_options_from_path("unexisting.path:method_name")
         self.assertFalse(mock_register_opts.called)
-        self.assertIsEmpty(opts._registered_paths)
+        self.assertEqual(0, len(opts._registered_paths))
 
         opts.register_options_from_path(
             "tests.unit.common.test_opts:fake_list_opts")
         mock_register_opts.assert_called_once_with(fake_list_opts().items())
         self.assertIn("tests.unit.common.test_opts:fake_list_opts",
                       opts._registered_paths)
```

### Comparing `rally-4.0.0/tests/unit/common/test_streaming_algorithms.py` & `rally-4.1.0/tests/unit/common/test_streaming_algorithms.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/test_utils.py` & `rally-4.1.0/tests/unit/common/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 import collections
 import queue as Queue
 import string
 import sys
 import threading
 import time
+import unittest
 from unittest import mock
 
 import ddt
 import pytest
-import testtools
 
 from rally.common import utils
 from rally import exceptions
 from tests.unit import test
 
 
 class ImmutableMixinTestCase(test.TestCase):
@@ -121,16 +121,16 @@
 
 def module_level_method():
     pass
 
 
 class MethodClassTestCase(test.TestCase):
 
-    @testtools.skipIf(sys.version_info > (2, 9), "Problems with access to "
-                                                 "class from <locals>")
+    @unittest.skipIf(sys.version_info > (2, 9), "Problems with access to "
+                                                "class from <locals>")
     def test_method_class_for_class_level_method(self):
         class A(object):
             def m(self):
                 pass
         self.assertEqual(A, utils.get_method_class(A.m))
 
     def test_method_class_for_module_level_method(self):
```

### Comparing `rally-4.0.0/tests/unit/common/test_validation.py` & `rally-4.1.0/tests/unit/common/test_validation.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/common/test_version.py` & `rally-4.1.0/tests/unit/common/test_version.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/doc/test_docker_readme.py` & `rally-4.1.0/tests/unit/doc/test_docker_readme.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/doc/test_docstrings.py` & `rally-4.1.0/tests/unit/doc/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/doc/test_format.py` & `rally-4.1.0/tests/unit/doc/test_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import fnmatch
 import io
 import os
 import re
+import unittest
 
-import testtools
 
-
-class TestFormat(testtools.TestCase):
+class TestFormat(unittest.TestCase):
     def _check_lines_wrapping(self, doc_file, raw):
         code_block = False
         text_inside_simple_tables = False
         lines = raw.split("\n")
         for i, line in enumerate(lines):
             if code_block:
                 if not line or line.startswith(" "):
```

### Comparing `rally-4.0.0/tests/unit/doc/test_jsonschemas.py` & `rally-4.1.0/tests/unit/doc/test_jsonschemas.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/doc/test_specs.py` & `rally-4.1.0/tests/unit/doc/test_specs.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/doc/utils.py` & `rally-4.1.0/tests/unit/doc/utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/env/test_env_mgr.py` & `rally-4.1.0/tests/unit/env/test_env_mgr.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/env/test_platform.py` & `rally-4.1.0/tests/unit/env/test_platform.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/fakes.py` & `rally-4.1.0/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/common/test_validators.py` & `rally-4.1.0/tests/unit/plugins/common/test_validators.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/contexts/test_dummy.py` & `rally-4.1.0/tests/unit/plugins/task/contexts/test_dummy.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/dummy_data.py` & `rally-4.1.0/tests/unit/plugins/task/exporters/dummy_data.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/elastic/test_client.py` & `rally-4.1.0/tests/unit/plugins/task/exporters/elastic/test_client.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/elastic/test_exporter.py` & `rally-4.1.0/tests/unit/plugins/task/exporters/elastic/test_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/elastic/test_flatten.py` & `rally-4.1.0/tests/unit/plugins/task/exporters/elastic/test_flatten.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/junit_report.xml` & `rally-4.1.0/tests/unit/plugins/task/exporters/junit_report.xml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/test_html.py` & `rally-4.1.0/tests/unit/plugins/task/exporters/test_html.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/test_json_exporter.py` & `rally-4.1.0/tests/unit/plugins/task/exporters/test_json_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/test_junit.py` & `rally-4.1.0/tests/unit/plugins/task/exporters/test_junit.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/test_old_json_results.py` & `rally-4.1.0/tests/unit/plugins/task/exporters/test_old_json_results.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/exporters/test_trends.py` & `rally-4.1.0/tests/unit/plugins/task/exporters/test_trends.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/hook_triggers/test_event.py` & `rally-4.1.0/tests/unit/plugins/task/hook_triggers/test_event.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/hook_triggers/test_periodic.py` & `rally-4.1.0/tests/unit/plugins/task/hook_triggers/test_periodic.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/hooks/test_sys_call.py` & `rally-4.1.0/tests/unit/plugins/task/hooks/test_sys_call.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/runners/test_constant.py` & `rally-4.1.0/tests/unit/plugins/task/runners/test_constant.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/runners/test_rps.py` & `rally-4.1.0/tests/unit/plugins/task/runners/test_rps.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,29 +261,29 @@
     )
     @ddt.unpack
     @mock.patch(RUNNERS + "rps.time.sleep")
     def test__run_scenario(self, mock_sleep, config):
         runner_obj = rps.RPSScenarioRunner(self.task, config)
 
         runner_obj._run_scenario(fakes.FakeScenario, "do_it",
-                                 fakes.FakeContext({}).context, {})
+                                 {"task": {"uuid": 1}}, {})
 
         self.assertEqual(config["times"], len(runner_obj.result_queue))
 
         for result_batch in runner_obj.result_queue:
             for result in result_batch:
                 self.assertIsNotNone(result)
 
     @mock.patch(RUNNERS + "rps.time.sleep")
     def test__run_scenario_exception(self, mock_sleep):
         config = {"times": 4, "rps": 10}
         runner_obj = rps.RPSScenarioRunner(self.task, config)
 
         runner_obj._run_scenario(fakes.FakeScenario, "something_went_wrong",
-                                 fakes.FakeContext({}).context, {})
+                                 {"task": {"uuid": 1}}, {})
         self.assertEqual(config["times"], len(runner_obj.result_queue))
         for result_batch in runner_obj.result_queue:
             for result in result_batch:
                 self.assertIsNotNone(result)
 
     @mock.patch(RUNNERS + "rps.time.sleep")
     def test__run_scenario_aborted(self, mock_sleep):
```

### Comparing `rally-4.0.0/tests/unit/plugins/task/runners/test_serial.py` & `rally-4.1.0/tests/unit/plugins/task/runners/test_serial.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/scenarios/dummy/test_dummy.py` & `rally-4.1.0/tests/unit/plugins/task/scenarios/dummy/test_dummy.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/scenarios/requests/test_http_requests.py` & `rally-4.1.0/tests/unit/plugins/task/scenarios/requests/test_http_requests.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/scenarios/requests/test_utils.py` & `rally-4.1.0/tests/unit/plugins/task/scenarios/requests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/sla/test_failure_rate.py` & `rally-4.1.0/tests/unit/plugins/task/sla/test_failure_rate.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/sla/test_iteration_time.py` & `rally-4.1.0/tests/unit/plugins/task/sla/test_iteration_time.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/sla/test_max_average_duration.py` & `rally-4.1.0/tests/unit/plugins/task/sla/test_max_average_duration.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/sla/test_max_average_duration_per_atomic.py` & `rally-4.1.0/tests/unit/plugins/task/sla/test_max_average_duration_per_atomic.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/sla/test_outliers.py` & `rally-4.1.0/tests/unit/plugins/task/sla/test_outliers.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/sla/test_performance_degradation.py` & `rally-4.1.0/tests/unit/plugins/task/sla/test_performance_degradation.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/task/test_types.py` & `rally-4.1.0/tests/unit/plugins/task/test_types.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/verification/junit_report.xml` & `rally-4.1.0/tests/unit/plugins/verification/junit_report.xml`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/verification/test_reporters.py` & `rally-4.1.0/tests/unit/plugins/verification/test_reporters.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/plugins/verification/test_testr.py` & `rally-4.1.0/tests/unit/plugins/verification/test_testr.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.verifier = mock.Mock()
         self.prepare_run_args = self.verifier.manager.prepare_run_args
         self.prepare_run_args.side_effect = lambda x: x
 
     def assertEqualCmd(self, expected, actual, msg="", stestr=False):
         cmd = ["stestr" if stestr else "testr", "run", "--subunit"]
         cmd.extend(expected)
-        self.assertEqual(cmd, actual, message=msg)
+        self.assertEqual(cmd, actual, msg=msg)
 
     def test_setup_with_concurrency(self):
         # default behaviour
         cfg = {"verifier": self.verifier}
         ctx = testr.TestrContext(cfg)
         ctx.setup()
         self.assertEqualCmd(["--parallel"], cfg["testr_cmd"])
```

### Comparing `rally-4.0.0/tests/unit/task/processing/test_charts.py` & `rally-4.1.0/tests/unit/task/processing/test_charts.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/processing/test_plot.py` & `rally-4.1.0/tests/unit/task/processing/test_plot.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/processing/test_utils.py` & `rally-4.1.0/tests/unit/task/processing/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_atomic.py` & `rally-4.1.0/tests/unit/task/test_atomic.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_context.py` & `rally-4.1.0/tests/unit/task/test_context.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_engine.py` & `rally-4.1.0/tests/unit/task/test_engine.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_exporter.py` & `rally-4.1.0/tests/unit/task/test_exporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_functional.py` & `rally-4.1.0/tests/unit/task/test_functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-import sys
-
-import testtools
-
 from rally import exceptions
 from rally.task import functional
 from tests.unit import test
 
 
 class FunctionalMixinTestCase(test.TestCase):
 
@@ -109,16 +105,14 @@
         self.assertRaises(exceptions.RallyAssertionError,
                           a.assertGreater,
                           len(["1", "2", "3"]), len(["3", "4", "5"]))
         self.assertRaises(exceptions.RallyAssertionError,
                           a.assertGreater,
                           len(["1", "2"]), len(["3", "4", "5"]))
 
-    @testtools.skipIf(sys.version_info < (2, 7),
-                      "assertRaises as context not supported")
     def test_assert_with_custom_message(self):
         class A(functional.FunctionalMixin):
             def __init__(self):
                 super(A, self).__init__()
 
         a = A()
         custom_message = "A custom message"
```

### Comparing `rally-4.0.0/tests/unit/task/test_hook.py` & `rally-4.1.0/tests/unit/task/test_hook.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_runner.py` & `rally-4.1.0/tests/unit/task/test_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,18 @@
             "atomic_actions": []
         }
         self.assertEqual(expected_result, result)
         self.assertEqual(expected_error[:2],
                          ["Exception", "Something went wrong"])
 
 
+def noop_worker_process(i):
+    pass
+
+
 @ddt.ddt
 class ScenarioRunnerTestCase(test.TestCase):
 
     @mock.patch(BASE + "rutils.Timer.duration", return_value=10)
     def test_run(self, mock_timer_duration):
         scenario_class = fakes.FakeClassBasedScenario
         runner_obj = serial.SerialScenarioRunner(
@@ -166,21 +170,18 @@
     def test__create_process_pool(self):
         runner_obj = serial.SerialScenarioRunner(
             mock.MagicMock(),
             mock.MagicMock())
 
         processes_to_start = 10
 
-        def worker_process(i):
-            pass
-
         counter = ((i,) for i in range(100))
 
         process_pool = runner_obj._create_process_pool(
-            processes_to_start, worker_process, counter)
+            processes_to_start, noop_worker_process, counter)
         self.assertEqual(processes_to_start, len(process_pool))
         for process in process_pool:
             self.assertIsInstance(process, multiprocessing.Process)
 
     @mock.patch(BASE + "ScenarioRunner._send_result")
     def test__join_processes(self, mock_scenario_runner__send_result):
         process = mock.MagicMock(is_alive=mock.MagicMock(return_value=False))
```

### Comparing `rally-4.0.0/tests/unit/task/test_scenario.py` & `rally-4.1.0/tests/unit/task/test_scenario.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_services.py` & `rally-4.1.0/tests/unit/task/test_services.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_sla.py` & `rally-4.1.0/tests/unit/task/test_sla.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_task_cfg.py` & `rally-4.1.0/tests/unit/task/test_task_cfg.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_types.py` & `rally-4.1.0/tests/unit/task/test_types.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/task/test_utils.py` & `rally-4.1.0/tests/unit/task/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/test.py` & `rally-4.1.0/tests/unit/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import fixtures
 from fixtures._fixtures.tempdir import TempDir
 import os
+import unittest
 from unittest import mock
 import uuid
 
-import testtools
+from oslo_config import fixture as cfg_fixture  # noqa N311
 
-from rally.common import cfg
 from rally.common import db
 from rally import plugins
 
 
 class TempHomeDir(TempDir):
     """Create a temporary directory and set it as $HOME
 
@@ -33,26 +33,26 @@
     """
 
     def _setUp(self):
         super(TempHomeDir, self)._setUp()
         self.useFixture(fixtures.EnvironmentVariable("HOME", self.path))
 
 
-class DatabaseFixture(cfg.fixture.Config):
+class DatabaseFixture(cfg_fixture.Config):
     """Create clean DB before starting test."""
     def setUp(self):
         super(DatabaseFixture, self).setUp()
         db_url = os.environ.get("RALLY_UNITTEST_DB_URL", "sqlite://")
         db.engine_reset()
         self.conf.set_default("connection", db_url, group="database")
         db.schema.schema_cleanup()
         db.schema.schema_create()
 
 
-class TestCase(testtools.TestCase):
+class TestCase(fixtures.TestWithFixtures, unittest.TestCase):
     """Test case base class for all unit tests."""
 
     def __init__(self, *args, **kwargs):
         super(TestCase, self).__init__(*args, **kwargs)
 
         # This is the number of characters shown when two objects do not
         # match for assertDictEqual, assertMultiLineEqual, and
@@ -63,16 +63,15 @@
     def setUp(self):
         super(TestCase, self).setUp()
         self.addCleanup(mock.patch.stopall)
         plugins.load()
         self.useFixture(TempHomeDir())
 
     def _test_atomic_action_timer(self, atomic_actions, name, count=1,
-                                  parent=[]):
-
+                                  parent=None):
         if parent:
             is_found = False
             for action in atomic_actions:
                 if action["name"] == parent[0]:
                     is_found = True
                     self._test_atomic_action_timer(action["children"],
                                                    name, count=count,
@@ -90,26 +89,25 @@
             if count != actual_count:
                 self.fail("%(count)d count is expected for atomic action"
                           " %(name)s, the actual count"
                           " is %(actual_count)d."
                           % {"name": name, "count": count,
                              "actual_count": actual_count})
 
-    def assertSequenceEqual(self, iterable_1, iterable_2, msg=None):
-        self.assertEqual(tuple(iterable_1), tuple(iterable_2), msg)
-
-    _IS_EMPTY_MSG = "Iterable is not empty"
-
-    def assertIsEmpty(self, iterable, msg=None):
-        if len(iterable):
-            if msg:
-                msg = "%s : %s" % (self._IS_EMPTY_MSG, msg)
-            else:
-                msg = self._IS_EMPTY_MSG
-            raise self.failureException(msg)
+    # TODO(andreykurilin): port existing code to use 'standard' flow
+    def assertRaises(
+        self,
+        expected_exception,
+        callable,
+        *args,
+        **kwargs,
+    ):
+        with super().assertRaises(expected_exception) as ctx:
+            callable(*args, **kwargs)
+        return ctx.exception
 
 
 class DBTestCase(TestCase):
     """Base class for tests which use DB."""
 
     def setUp(self):
         super(DBTestCase, self).setUp()
```

### Comparing `rally-4.0.0/tests/unit/test_api.py` & `rally-4.1.0/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/test_ddt.py` & `rally-4.1.0/tests/unit/test_ddt.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/test_exceptions.py` & `rally-4.1.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/test_hacking.py` & `rally-4.1.0/tests/unit/test_hacking.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/test_mock.py` & `rally-4.1.0/tests/unit/test_mock.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/test_pytest_launcher.py` & `rally-4.1.0/tests/unit/test_pytest_launcher.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/test_resources.py` & `rally-4.1.0/tests/unit/test_resources.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/test_test_ddt.py` & `rally-4.1.0/tests/unit/test_test_ddt.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/test_test_mock.py` & `rally-4.1.0/tests/unit/test_test_mock.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import ast
-import sys
 from unittest import mock
 
 from tests.unit import test
 from tests.unit import test_mock
 
 
 class VariantsTestCase(test.TestCase):
@@ -323,23 +322,18 @@
             return_value=[variants]
         )
         self.visitor._get_mock_args = mock.Mock(
             return_value=["bar_foo_misnamed"]
         )
 
         self.assertIsNone(self.visitor.visit_FunctionDef(self.tree))
-        if sys.version_info < (3, 8):
-            # https://github.com/python/cpython/pull/9731
-            lineno = 2
-        else:
-            lineno = 7
         self.assertEqual(
             [
                 {
-                    "lineno": lineno,
+                    "lineno": 7,
                     "messages": [
                         "Argument 'mock_bar_foo_misnamed' misnamed; should be "
                         "either of %s that is derived from the mock decorator "
                         "args.\n" % variants
                     ],
                     "mismatch_pairs": [
                         ("bar_foo_misnamed", variants)
@@ -363,23 +357,18 @@
             return_value=[variants]
         )
         self.visitor._get_mock_args = mock.Mock(
             return_value=["bar_foo_misnamed", "mismatched"]
         )
 
         self.assertIsNone(self.visitor.visit_FunctionDef(self.tree))
-        if sys.version_info < (3, 8):
-            # https://github.com/python/cpython/pull/9731
-            lineno = 2
-        else:
-            lineno = 7
         self.assertEqual(
             [
                 {
-                    "lineno": lineno,
+                    "lineno": 7,
                     "messages": [
                         "Argument 'mock_bar_foo_misnamed' misnamed; should be "
                         "either of %s that is derived from the mock decorator "
                         "args.\n" % variants,
                         "Missing or malformed decorator for 'mock_mismatched' "
                         "argument."
                     ],
@@ -404,23 +393,18 @@
             return_value=[variants]
         )
         self.visitor._get_mock_args = mock.Mock(
             return_value=[]
         )
 
         self.assertIsNone(self.visitor.visit_FunctionDef(self.tree))
-        if sys.version_info < (3, 8):
-            # https://github.com/python/cpython/pull/9731
-            lineno = 2
-        else:
-            lineno = 7
         self.assertEqual(
             [
                 {
-                    "lineno": lineno,
+                    "lineno": 7,
                     "messages": [
                         "Missing or malformed argument for {'mock_foo', "
                         "'mock_foo_bar', 'mock_pkg_foo_bar', ...} decorator."
                     ],
                     "args": self.visitor._get_mock_args.return_value,
                     "decs": [variants]
                 }
@@ -444,20 +428,15 @@
         )
 
         self.assertEqual(
             self.code_mock_decorators,
             self.visitor.errors[0]["decs"]
         )
 
-        if sys.version_info < (3, 8):
-            # https://github.com/python/cpython/pull/9731
-            lineno = 2
-        else:
-            lineno = 7
-        self.assertEqual(lineno, self.visitor.errors[0]["lineno"])
+        self.assertEqual(7, self.visitor.errors[0]["lineno"])
 
     def test_visit_ok(self):
         self.visitor.classname_python = "my_class_object"
         self.visitor.visit(
             self._parse_expr(
                 """
 class MyClassObjectTestCase(object):
```

### Comparing `rally-4.0.0/tests/unit/ui/test_utils.py` & `rally-4.1.0/tests/unit/ui/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/utils/test_encodeutils.py` & `rally-4.1.0/tests/unit/utils/test_encodeutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/utils/test_sshutils.py` & `rally-4.1.0/tests/unit/utils/test_sshutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/utils/test_strutils.py` & `rally-4.1.0/tests/unit/utils/test_strutils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/verification/test_context.py` & `rally-4.1.0/tests/unit/verification/test_context.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/verification/test_manager.py` & `rally-4.1.0/tests/unit/verification/test_manager.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/verification/test_reporter.py` & `rally-4.1.0/tests/unit/verification/test_reporter.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tests/unit/verification/test_utils.py` & `rally-4.1.0/tests/unit/verification/test_utils.py`

 * *Files identical despite different names*

### Comparing `rally-4.0.0/tox.ini` & `rally-4.1.0/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 extras = {env:RALLY_EXTRAS:}
 setenv = VIRTUAL_ENV={envdir}
          LANG=en_US.UTF-8
          LANGUAGE=en_US:en
          LC_ALL=C
          PYTHONHASHSEED=0
          TOX_ENV_NAME={envname}
+         sa14: SQLALCHEMY_SILENCE_UBER_WARNING=1
 allowlist_externals = find
                       rm
                       make
                       mkdir
 deps = -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
        -c{toxinidir}/upper-constraints.txt
+       sa14: SQLAlchemy<1.5
+       sa2: SQLAlchemy>=2
 usedevelop = True
 commands =
   find . -type f -name "*.pyc" -delete
   python {toxinidir}/tests/ci/pytest_launcher.py tests/unit --posargs={posargs}
 distribute = false
 basepython = python3
 passenv =
@@ -34,20 +37,14 @@
           NO_PROXY
           HOME
 
 [testenv:pep8]
 commands = flake8
 distribute = false
 
-[testenv:py38]
-basepython = python3.8
-
-[testenv:py39]
-basepython = python3.9
-
 [testenv:samples]
 commands =
   find . -type f -name "*.pyc" -delete
   python {toxinidir}/tests/ci/pytest_launcher.py tests/samples --posargs={posargs}
 
 
 [testenv:venv]
@@ -139,31 +136,17 @@
   find . -type f -name "*.pyc" -delete
   mkdir -p {toxinidir}/.test_results
   python3 {toxinidir}/tests/ci/rally_self_job.py --task {toxinidir}/rally-jobs/self-rally.yaml --plugins-path {toxinidir}/rally-jobs/plugins
 
 [pytest]
 filterwarnings =
     error
-    ignore:.*EngineFacade is deprecated; please use oslo_db.sqlalchemy.enginefacade*:
-    # Introduced with oslo.db-12.1.0
-    ignore:.*Support for the MySQL NDB Cluster storage engine has been deprecated and will be removed in a future release.:DeprecationWarning:
-    # Introuduced with SQLAlchemy-1.4.46, can be removed when rally supports SQLAlchemy>=2.0.0
-    ignore:.*Set environment variable SQLALCHEMY_SILENCE_UBER_WARNING=1 to silence this message.*
-    # instead of ignoring all modules, let's list only libraries that are failing
-    ignore:invalid escape sequence:DeprecationWarning:.*netaddr.*
-    ignore:invalid escape sequence:DeprecationWarning:.*prettytable
-    ignore:invalid escape sequence:DeprecationWarning:.*subunit.*
-    ignore:invalid escape sequence:DeprecationWarning:.*docutils.*
     # we do not use anything inner from OptionParser, so we do not care about it's parent
     ignore:The frontend.OptionParser class will be replaced by a subclass of argparse.ArgumentParser in Docutils 0.21 or later.:DeprecationWarning:
     # we do not use Option directly, it is initialized by OptionParser by itself.
     # as soon as docutils team get rid of frontend.Option, they will also fix OptionParser
     ignore: The frontend.Option class will be removed in Docutils 0.21 or later.:DeprecationWarning:
-    # python 3.7
-    ignore:Using or importing the ABCs:DeprecationWarning:unittest2.*
-    # python 3.8
-    ignore:::.*netaddr.strategy.*
     # python 3.10
     ignore:The distutils package is deprecated and slated for removal in Python 3.12. Use setuptools or check PEP 632 for potential alternatives:DeprecationWarning:
     ignore:pkg_resources is deprecated as an API:DeprecationWarning:
-    # pytest-cov
+    # pytest-cov & pytest-xdist
     ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning:
```


# Comparing `tmp/tickforge_client-1.3.0.tar.gz` & `tmp/tickforge_client-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickforge_client-1.3.0.tar", max compression
+gzip compressed data, was "tickforge_client-1.4.0.tar", max compression
```

## Comparing `tickforge_client-1.3.0.tar` & `tickforge_client-1.4.0.tar`

### file list

```diff
@@ -1,55 +1,85 @@
--rw-r--r--   0        0        0     8817 2024-03-04 23:53:52.114683 tickforge_client-1.3.0/README.md
--rw-r--r--   0        0        0      726 2024-03-04 23:53:52.126329 tickforge_client-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4294 2024-03-04 23:53:52.131844 tickforge_client-1.3.0/tickforge_client/__init__.py
--rw-r--r--   0        0        0      636 2024-03-04 23:53:52.134427 tickforge_client-1.3.0/tickforge_client/api/__init__.py
--rw-r--r--   0        0        0    19040 2024-03-04 23:53:52.058858 tickforge_client-1.3.0/tickforge_client/api/auth_api.py
--rw-r--r--   0        0        0     7455 2024-03-04 23:53:52.064552 tickforge_client-1.3.0/tickforge_client/api/builds_api.py
--rw-r--r--   0        0        0     7164 2024-03-04 23:53:52.072553 tickforge_client-1.3.0/tickforge_client/api/db_api.py
--rw-r--r--   0        0        0    17110 2024-03-04 23:53:52.077029 tickforge_client-1.3.0/tickforge_client/api/default_api.py
--rw-r--r--   0        0        0    12503 2024-03-04 23:53:52.083398 tickforge_client-1.3.0/tickforge_client/api/git_api.py
--rw-r--r--   0        0        0     8664 2024-03-04 23:53:52.087496 tickforge_client-1.3.0/tickforge_client/api/github_api.py
--rw-r--r--   0        0        0     6735 2024-03-04 23:53:52.092228 tickforge_client-1.3.0/tickforge_client/api/jobs_api.py
--rw-r--r--   0        0        0    14885 2024-03-04 23:53:52.096362 tickforge_client-1.3.0/tickforge_client/api/metrics_api.py
--rw-r--r--   0        0        0    21793 2024-03-04 23:53:52.100225 tickforge_client-1.3.0/tickforge_client/api/redirects_api.py
--rw-r--r--   0        0        0    17297 2024-03-04 23:53:52.103599 tickforge_client-1.3.0/tickforge_client/api/slack_api.py
--rw-r--r--   0        0        0    59120 2024-03-04 23:53:52.109114 tickforge_client-1.3.0/tickforge_client/api/workspaces_api.py
--rw-r--r--   0        0        0    29482 2024-03-04 23:53:52.138999 tickforge_client-1.3.0/tickforge_client/api_client.py
--rw-r--r--   0        0        0      852 2024-03-04 23:53:52.140504 tickforge_client-1.3.0/tickforge_client/api_response.py
--rw-r--r--   0        0        0    14361 2024-03-04 23:53:52.128715 tickforge_client-1.3.0/tickforge_client/configuration.py
--rw-r--r--   0        0        0     5374 2024-03-04 23:53:52.135745 tickforge_client-1.3.0/tickforge_client/exceptions.py
--rw-r--r--   0        0        0     2435 2024-03-04 23:53:52.133357 tickforge_client-1.3.0/tickforge_client/models/__init__.py
--rw-r--r--   0        0        0     4612 2024-02-23 04:03:31.417408 tickforge_client-1.3.0/tickforge_client/models/author_name.py
--rw-r--r--   0        0        0     2483 2024-03-04 23:53:51.867213 tickforge_client-1.3.0/tickforge_client/models/backup.py
--rw-r--r--   0        0        0     2094 2024-03-04 23:53:51.875133 tickforge_client-1.3.0/tickforge_client/models/base_user.py
--rw-r--r--   0        0        0     4582 2024-03-04 23:53:51.886454 tickforge_client-1.3.0/tickforge_client/models/batch_id.py
--rw-r--r--   0        0        0     2348 2024-03-04 23:53:51.891643 tickforge_client-1.3.0/tickforge_client/models/body_bump_app_api_workspaces_app_name_bump_post.py
--rw-r--r--   0        0        0     2663 2024-03-04 23:53:51.896849 tickforge_client-1.3.0/tickforge_client/models/body_qadeploy_api_workspaces_qadeploy_post.py
--rw-r--r--   0        0        0     2257 2024-03-04 23:53:51.901325 tickforge_client-1.3.0/tickforge_client/models/body_qadestroy_api_workspaces_qadestroy_post.py
--rw-r--r--   0        0        0     4572 2024-03-04 23:53:51.907169 tickforge_client-1.3.0/tickforge_client/models/branch.py
--rw-r--r--   0        0        0     2819 2024-03-04 23:53:51.911467 tickforge_client-1.3.0/tickforge_client/models/build_schema.py
--rw-r--r--   0        0        0      767 2024-03-04 23:53:51.916847 tickforge_client-1.3.0/tickforge_client/models/cluster.py
--rw-r--r--   0        0        0     2131 2024-03-04 23:53:51.920347 tickforge_client-1.3.0/tickforge_client/models/copy_db_payload.py
--rw-r--r--   0        0        0     2222 2024-03-04 23:53:51.923773 tickforge_client-1.3.0/tickforge_client/models/create_backup_response.py
--rw-r--r--   0        0        0     2664 2024-03-04 23:53:51.927958 tickforge_client-1.3.0/tickforge_client/models/create_build_payload.py
--rw-r--r--   0        0        0     2342 2024-03-04 23:53:51.933493 tickforge_client-1.3.0/tickforge_client/models/create_metric_payload.py
--rw-r--r--   0        0        0     2558 2024-03-04 23:53:51.937394 tickforge_client-1.3.0/tickforge_client/models/create_workspace_payload.py
--rw-r--r--   0        0        0     2377 2024-03-04 23:53:51.941390 tickforge_client-1.3.0/tickforge_client/models/http_validation_error.py
--rw-r--r--   0        0        0     2704 2024-03-04 23:53:51.944945 tickforge_client-1.3.0/tickforge_client/models/job.py
--rw-r--r--   0        0        0      722 2024-03-04 23:53:51.947417 tickforge_client-1.3.0/tickforge_client/models/job_status.py
--rw-r--r--   0        0        0     4573 2024-03-04 23:53:51.951448 tickforge_client-1.3.0/tickforge_client/models/limit.py
--rw-r--r--   0        0        0     2249 2024-03-04 23:53:51.954779 tickforge_client-1.3.0/tickforge_client/models/metric.py
--rw-r--r--   0        0        0     4612 2024-03-04 23:53:51.958656 tickforge_client-1.3.0/tickforge_client/models/metric_name.py
--rw-r--r--   0        0        0     4602 2024-03-04 23:53:51.962242 tickforge_client-1.3.0/tickforge_client/models/namespace.py
--rw-r--r--   0        0        0      760 2024-03-04 23:53:51.964850 tickforge_client-1.3.0/tickforge_client/models/server_timezone.py
--rw-r--r--   0        0        0      735 2024-03-04 23:53:51.967709 tickforge_client-1.3.0/tickforge_client/models/server_type.py
--rw-r--r--   0        0        0     4545 2024-03-04 23:53:51.975489 tickforge_client-1.3.0/tickforge_client/models/size.py
--rw-r--r--   0        0        0     1970 2024-03-04 23:53:51.979622 tickforge_client-1.3.0/tickforge_client/models/token_response.py
--rw-r--r--   0        0        0     2508 2024-03-04 23:53:51.983110 tickforge_client-1.3.0/tickforge_client/models/validation_error.py
--rw-r--r--   0        0        0     4733 2024-03-04 23:53:51.986955 tickforge_client-1.3.0/tickforge_client/models/validation_error_loc_inner.py
--rw-r--r--   0        0        0     2442 2024-03-04 23:53:51.990436 tickforge_client-1.3.0/tickforge_client/models/versions_config.py
--rw-r--r--   0        0        0     2706 2024-03-04 23:53:51.993791 tickforge_client-1.3.0/tickforge_client/models/workspace.py
--rw-r--r--   0        0        0     4609 2024-03-04 23:53:51.996883 tickforge_client-1.3.0/tickforge_client/models/workspace_cluster.py
--rw-r--r--   0        0        0     4672 2024-03-04 23:53:52.000949 tickforge_client-1.3.0/tickforge_client/models/x_hub_signature256.py
--rw-r--r--   0        0        0        0 2024-03-04 23:53:52.126992 tickforge_client-1.3.0/tickforge_client/py.typed
--rw-r--r--   0        0        0    13827 2024-03-04 23:53:52.142063 tickforge_client-1.3.0/tickforge_client/rest.py
--rw-r--r--   0        0        0     9776 1970-01-01 00:00:00.000000 tickforge_client-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10418 2024-05-08 00:08:21.322987 tickforge_client-1.4.0/README.md
+-rw-r--r--   0        0        0      726 2024-05-08 00:08:21.335783 tickforge_client-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6022 2024-05-08 00:08:21.341874 tickforge_client-1.4.0/tickforge_client/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-08 00:08:21.344494 tickforge_client-1.4.0/tickforge_client/api/__init__.py
+-rw-r--r--   0        0        0    19040 2024-05-08 00:08:21.267912 tickforge_client-1.4.0/tickforge_client/api/auth_api.py
+-rw-r--r--   0        0        0     7455 2024-05-08 00:08:21.273214 tickforge_client-1.4.0/tickforge_client/api/builds_api.py
+-rw-r--r--   0        0        0     7164 2024-05-08 00:08:21.277152 tickforge_client-1.4.0/tickforge_client/api/db_api.py
+-rw-r--r--   0        0        0    17110 2024-05-08 00:08:21.281539 tickforge_client-1.4.0/tickforge_client/api/default_api.py
+-rw-r--r--   0        0        0    12503 2024-05-08 00:08:21.284726 tickforge_client-1.4.0/tickforge_client/api/git_api.py
+-rw-r--r--   0        0        0     8664 2024-05-08 00:08:21.288866 tickforge_client-1.4.0/tickforge_client/api/github_api.py
+-rw-r--r--   0        0        0     6735 2024-05-08 00:08:21.294076 tickforge_client-1.4.0/tickforge_client/api/jobs_api.py
+-rw-r--r--   0        0        0    27945 2024-05-08 00:08:21.299287 tickforge_client-1.4.0/tickforge_client/api/metrics_api.py
+-rw-r--r--   0        0        0    21793 2024-05-08 00:08:21.304618 tickforge_client-1.4.0/tickforge_client/api/redirects_api.py
+-rw-r--r--   0        0        0    23947 2024-05-08 00:08:21.308290 tickforge_client-1.4.0/tickforge_client/api/slack_api.py
+-rw-r--r--   0        0        0    59120 2024-05-08 00:08:21.315372 tickforge_client-1.4.0/tickforge_client/api/workspaces_api.py
+-rw-r--r--   0        0        0    29482 2024-05-08 00:08:21.349580 tickforge_client-1.4.0/tickforge_client/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-08 00:08:21.350843 tickforge_client-1.4.0/tickforge_client/api_response.py
+-rw-r--r--   0        0        0    14627 2024-05-08 00:08:21.340061 tickforge_client-1.4.0/tickforge_client/configuration.py
+-rw-r--r--   0        0        0     5374 2024-05-08 00:08:21.345944 tickforge_client-1.4.0/tickforge_client/exceptions.py
+-rw-r--r--   0        0        0     4163 2024-05-08 00:08:21.343303 tickforge_client-1.4.0/tickforge_client/models/__init__.py
+-rw-r--r--   0        0        0     4652 2024-05-08 00:08:20.948458 tickforge_client-1.4.0/tickforge_client/models/always_active.py
+-rw-r--r--   0        0        0     4612 2024-02-23 04:03:31.417408 tickforge_client-1.4.0/tickforge_client/models/author_name.py
+-rw-r--r--   0        0        0     2483 2024-05-08 00:08:20.957835 tickforge_client-1.4.0/tickforge_client/models/backup.py
+-rw-r--r--   0        0        0     2094 2024-05-08 00:08:20.964081 tickforge_client-1.4.0/tickforge_client/models/base_user.py
+-rw-r--r--   0        0        0     4582 2024-05-08 00:08:20.969309 tickforge_client-1.4.0/tickforge_client/models/batch_id.py
+-rw-r--r--   0        0        0     2348 2024-05-08 00:08:20.974367 tickforge_client-1.4.0/tickforge_client/models/body_bump_app_api_workspaces_app_name_bump_post.py
+-rw-r--r--   0        0        0     2663 2024-05-08 00:08:20.979336 tickforge_client-1.4.0/tickforge_client/models/body_qadeploy_api_workspaces_qadeploy_post.py
+-rw-r--r--   0        0        0     2257 2024-05-08 00:08:20.984080 tickforge_client-1.4.0/tickforge_client/models/body_qadestroy_api_workspaces_qadestroy_post.py
+-rw-r--r--   0        0        0     4572 2024-05-08 00:08:20.988849 tickforge_client-1.4.0/tickforge_client/models/branch.py
+-rw-r--r--   0        0        0     2819 2024-05-08 00:08:20.993101 tickforge_client-1.4.0/tickforge_client/models/build_schema.py
+-rw-r--r--   0        0        0      957 2024-05-08 00:08:20.996745 tickforge_client-1.4.0/tickforge_client/models/cluster.py
+-rw-r--r--   0        0        0     1992 2024-05-08 00:08:21.000060 tickforge_client-1.4.0/tickforge_client/models/code_metric_blob_payload.py
+-rw-r--r--   0        0        0     2081 2024-05-08 00:08:21.004606 tickforge_client-1.4.0/tickforge_client/models/code_metric_blob_response.py
+-rw-r--r--   0        0        0     2131 2024-05-08 00:08:21.009961 tickforge_client-1.4.0/tickforge_client/models/copy_db_payload.py
+-rw-r--r--   0        0        0     2222 2024-05-08 00:08:21.013738 tickforge_client-1.4.0/tickforge_client/models/create_backup_response.py
+-rw-r--r--   0        0        0     2664 2024-05-08 00:08:21.017507 tickforge_client-1.4.0/tickforge_client/models/create_build_payload.py
+-rw-r--r--   0        0        0     2342 2024-05-08 00:08:21.025496 tickforge_client-1.4.0/tickforge_client/models/create_metric_payload.py
+-rw-r--r--   0        0        0     2558 2024-05-08 00:08:21.029253 tickforge_client-1.4.0/tickforge_client/models/create_workspace_payload.py
+-rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.032872 tickforge_client-1.4.0/tickforge_client/models/deleted.py
+-rw-r--r--   0        0        0     4622 2024-05-08 00:08:21.037831 tickforge_client-1.4.0/tickforge_client/models/display_name.py
+-rw-r--r--   0        0        0     4562 2024-05-08 00:08:21.043069 tickforge_client-1.4.0/tickforge_client/models/email.py
+-rw-r--r--   0        0        0     4562 2024-05-08 00:08:21.047433 tickforge_client-1.4.0/tickforge_client/models/error.py
+-rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.052418 tickforge_client-1.4.0/tickforge_client/models/first_name.py
+-rw-r--r--   0        0        0     2377 2024-05-08 00:08:21.056540 tickforge_client-1.4.0/tickforge_client/models/http_validation_error.py
+-rw-r--r--   0        0        0     4582 2024-05-08 00:08:21.060466 tickforge_client-1.4.0/tickforge_client/models/image32.py
+-rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.065262 tickforge_client-1.4.0/tickforge_client/models/is_admin.py
+-rw-r--r--   0        0        0     4622 2024-05-08 00:08:21.070320 tickforge_client-1.4.0/tickforge_client/models/is_app_user.py
+-rw-r--r--   0        0        0     4582 2024-05-08 00:08:21.075276 tickforge_client-1.4.0/tickforge_client/models/is_bot.py
+-rw-r--r--   0        0        0     4692 2024-05-08 00:08:21.080324 tickforge_client-1.4.0/tickforge_client/models/is_email_confirmed.py
+-rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.085256 tickforge_client-1.4.0/tickforge_client/models/is_owner.py
+-rw-r--r--   0        0        0     4672 2024-05-08 00:08:21.089602 tickforge_client-1.4.0/tickforge_client/models/is_primary_owner.py
+-rw-r--r--   0        0        0     4652 2024-05-08 00:08:21.095776 tickforge_client-1.4.0/tickforge_client/models/is_restricted.py
+-rw-r--r--   0        0        0     2704 2024-05-08 00:08:21.099939 tickforge_client-1.4.0/tickforge_client/models/job.py
+-rw-r--r--   0        0        0      722 2024-05-08 00:08:21.102924 tickforge_client-1.4.0/tickforge_client/models/job_status.py
+-rw-r--r--   0        0        0     4592 2024-05-08 00:08:21.106067 tickforge_client-1.4.0/tickforge_client/models/last_name.py
+-rw-r--r--   0        0        0     4573 2024-05-08 00:08:21.110552 tickforge_client-1.4.0/tickforge_client/models/limit.py
+-rw-r--r--   0        0        0     3737 2024-05-08 00:08:21.113656 tickforge_client-1.4.0/tickforge_client/models/list_user_response.py
+-rw-r--r--   0        0        0     2249 2024-05-08 00:08:21.117276 tickforge_client-1.4.0/tickforge_client/models/metric.py
+-rw-r--r--   0        0        0     4612 2024-05-08 00:08:21.120704 tickforge_client-1.4.0/tickforge_client/models/metric_name.py
+-rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.123578 tickforge_client-1.4.0/tickforge_client/models/namespace.py
+-rw-r--r--   0        0        0     4572 2024-05-08 00:08:21.127167 tickforge_client-1.4.0/tickforge_client/models/offset.py
+-rw-r--r--   0        0        0     5185 2024-05-08 00:08:21.131033 tickforge_client-1.4.0/tickforge_client/models/profile.py
+-rw-r--r--   0        0        0     4592 2024-05-08 00:08:21.135535 tickforge_client-1.4.0/tickforge_client/models/real_name.py
+-rw-r--r--   0        0        0     1869 2024-05-08 00:08:21.138685 tickforge_client-1.4.0/tickforge_client/models/response_metadata.py
+-rw-r--r--   0        0        0      760 2024-05-08 00:08:21.142346 tickforge_client-1.4.0/tickforge_client/models/server_timezone.py
+-rw-r--r--   0        0        0      735 2024-05-08 00:08:21.144529 tickforge_client-1.4.0/tickforge_client/models/server_type.py
+-rw-r--r--   0        0        0     4545 2024-05-08 00:08:21.147922 tickforge_client-1.4.0/tickforge_client/models/size.py
+-rw-r--r--   0        0        0     7835 2024-05-08 00:08:21.150969 tickforge_client-1.4.0/tickforge_client/models/slack_member.py
+-rw-r--r--   0        0        0     4552 2024-05-08 00:08:21.155433 tickforge_client-1.4.0/tickforge_client/models/team.py
+-rw-r--r--   0        0        0     4572 2024-05-08 00:08:21.159306 tickforge_client-1.4.0/tickforge_client/models/team_id.py
+-rw-r--r--   0        0        0     4562 2024-05-08 00:08:21.164471 tickforge_client-1.4.0/tickforge_client/models/title.py
+-rw-r--r--   0        0        0     1970 2024-05-08 00:08:21.168609 tickforge_client-1.4.0/tickforge_client/models/token_response.py
+-rw-r--r--   0        0        0     4532 2024-05-08 00:08:21.172092 tickforge_client-1.4.0/tickforge_client/models/tz.py
+-rw-r--r--   0        0        0     4582 2024-05-08 00:08:21.176599 tickforge_client-1.4.0/tickforge_client/models/tz_label.py
+-rw-r--r--   0        0        0     4603 2024-05-08 00:08:21.180037 tickforge_client-1.4.0/tickforge_client/models/tz_offset.py
+-rw-r--r--   0        0        0     4593 2024-05-08 00:08:21.184197 tickforge_client-1.4.0/tickforge_client/models/updated.py
+-rw-r--r--   0        0        0     2508 2024-05-08 00:08:21.188000 tickforge_client-1.4.0/tickforge_client/models/validation_error.py
+-rw-r--r--   0        0        0     4733 2024-05-08 00:08:21.190608 tickforge_client-1.4.0/tickforge_client/models/validation_error_loc_inner.py
+-rw-r--r--   0        0        0     2442 2024-05-08 00:08:21.193748 tickforge_client-1.4.0/tickforge_client/models/versions_config.py
+-rw-r--r--   0        0        0     2706 2024-05-08 00:08:21.196798 tickforge_client-1.4.0/tickforge_client/models/workspace.py
+-rw-r--r--   0        0        0     4609 2024-05-08 00:08:21.200222 tickforge_client-1.4.0/tickforge_client/models/workspace_cluster.py
+-rw-r--r--   0        0        0     4672 2024-05-08 00:08:21.203641 tickforge_client-1.4.0/tickforge_client/models/x_hub_signature256.py
+-rw-r--r--   0        0        0        0 2024-05-08 00:08:21.337500 tickforge_client-1.4.0/tickforge_client/py.typed
+-rw-r--r--   0        0        0    13827 2024-05-08 00:08:21.352445 tickforge_client-1.4.0/tickforge_client/rest.py
+-rw-r--r--   0        0        0    11377 1970-01-01 00:00:00.000000 tickforge_client-1.4.0/PKG-INFO
```

### Comparing `tickforge_client-1.3.0/README.md` & `tickforge_client-1.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,40 @@
+Metadata-Version: 2.1
+Name: tickforge_client
+Version: 1.4.0
+Summary: Tickforge API
+Home-page: https://github.com/uptick/tickforge
+License: NoLicense
+Keywords: OpenAPI,OpenAPI-Generator,Tickforge API
+Author: William Chu
+Author-email: william.chu@uptickhq.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aenum (>=3.1.11)
+Requires-Dist: boto3
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: python-dateutil (>=2.8.2)
+Requires-Dist: urllib3 (>=1.25.3)
+Project-URL: Repository, https://github.com/uptick/tickforge
+Description-Content-Type: text/markdown
+
 # tickforge-client
 An API to interact with Uptick Internal Resources
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.3.0
+- Package version: 1.4.0
 - Build package: org.openapitools.codegen.languages.PythonPydanticV1ClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -95,72 +121,111 @@
 *DefaultApi* | [**health_check_livez_get**](docs/DefaultApi.md#health_check_livez_get) | **GET** /livez | Health Check
 *DefaultApi* | [**health_check_readyz_get**](docs/DefaultApi.md#health_check_readyz_get) | **GET** /readyz | Health Check
 *GitApi* | [**refresh_respository_api_git_refresh_repository_post**](docs/GitApi.md#refresh_respository_api_git_refresh_repository_post) | **POST** /api/git/refresh_repository | Refresh Respository
 *GitApi* | [**versions_config_api_git_versions_get**](docs/GitApi.md#versions_config_api_git_versions_get) | **GET** /api/git/versions | Versions Config
 *GithubApi* | [**workflow_job_webhook_api_github_webhooks_workflow_job_post**](docs/GithubApi.md#workflow_job_webhook_api_github_webhooks_workflow_job_post) | **POST** /api/github/webhooks/workflow_job | Workflow Job Webhook
 *JobsApi* | [**get_job_api_jobs_job_id_get**](docs/JobsApi.md#get_job_api_jobs_job_id_get) | **GET** /api/jobs/{job_id} | Get Job
 *MetricsApi* | [**create_metric_api_metrics_post**](docs/MetricsApi.md#create_metric_api_metrics_post) | **POST** /api/metrics/ | Create Metric
+*MetricsApi* | [**create_metric_blob_api_metrics_blob_post**](docs/MetricsApi.md#create_metric_blob_api_metrics_blob_post) | **POST** /api/metrics/blob | Create Metric Blob
 *MetricsApi* | [**get_metric_api_metrics_get**](docs/MetricsApi.md#get_metric_api_metrics_get) | **GET** /api/metrics/ | Get Metric
+*MetricsApi* | [**get_metric_blob_api_metrics_blob_get**](docs/MetricsApi.md#get_metric_blob_api_metrics_blob_get) | **GET** /api/metrics/blob | Get Metric Blob
 *RedirectsApi* | [**me_redirect_me_get**](docs/RedirectsApi.md#me_redirect_me_get) | **GET** /me | Me Redirect
 *RedirectsApi* | [**refresh_repository_redirect_api_refresh_repository_post**](docs/RedirectsApi.md#refresh_repository_redirect_api_refresh_repository_post) | **POST** /api/refresh_repository | Refresh Repository Redirect
 *RedirectsApi* | [**token_redirect_token_post**](docs/RedirectsApi.md#token_redirect_token_post) | **POST** /token | Token Redirect
 *RedirectsApi* | [**versions_redirect_api_versions_get**](docs/RedirectsApi.md#versions_redirect_api_versions_get) | **GET** /api/versions | Versions Redirect
 *SlackApi* | [**event_handler_slack_events_get**](docs/SlackApi.md#event_handler_slack_events_get) | **GET** /slack/events | Event Handler
 *SlackApi* | [**event_handler_slack_events_patch**](docs/SlackApi.md#event_handler_slack_events_patch) | **PATCH** /slack/events | Event Handler
 *SlackApi* | [**event_handler_slack_events_post**](docs/SlackApi.md#event_handler_slack_events_post) | **POST** /slack/events | Event Handler
+*SlackApi* | [**search_users_api_slack_search_get**](docs/SlackApi.md#search_users_api_slack_search_get) | **GET** /api/slack/search | Search Users
 *WorkspacesApi* | [**bump_app_api_workspaces_app_name_bump_post**](docs/WorkspacesApi.md#bump_app_api_workspaces_app_name_bump_post) | **POST** /api/workspaces/{app_name}/bump | Bump App
 *WorkspacesApi* | [**create_backup_api_workspaces_workspace_name_backups_post**](docs/WorkspacesApi.md#create_backup_api_workspaces_workspace_name_backups_post) | **POST** /api/workspaces/{workspace_name}/backups | Create Backup
 *WorkspacesApi* | [**create_workspace_api_workspaces_create_post**](docs/WorkspacesApi.md#create_workspace_api_workspaces_create_post) | **POST** /api/workspaces/create | Create Workspace
 *WorkspacesApi* | [**create_workspace_api_workspaces_post**](docs/WorkspacesApi.md#create_workspace_api_workspaces_post) | **POST** /api/workspaces/ | Create Workspace
 *WorkspacesApi* | [**list_backups_api_workspaces_workspace_name_backups_get**](docs/WorkspacesApi.md#list_backups_api_workspaces_workspace_name_backups_get) | **GET** /api/workspaces/{workspace_name}/backups | List Backups
 *WorkspacesApi* | [**list_workspaces_api_workspaces_get**](docs/WorkspacesApi.md#list_workspaces_api_workspaces_get) | **GET** /api/workspaces/ | List Workspaces
 *WorkspacesApi* | [**qadeploy_api_workspaces_qadeploy_post**](docs/WorkspacesApi.md#qadeploy_api_workspaces_qadeploy_post) | **POST** /api/workspaces/qadeploy | Qadeploy
 *WorkspacesApi* | [**qadestroy_api_workspaces_qadestroy_post**](docs/WorkspacesApi.md#qadestroy_api_workspaces_qadestroy_post) | **POST** /api/workspaces/qadestroy | Qadestroy
 *WorkspacesApi* | [**suspend_workspace_api_workspaces_workspace_name_suspend_post**](docs/WorkspacesApi.md#suspend_workspace_api_workspaces_workspace_name_suspend_post) | **POST** /api/workspaces/{workspace_name}/suspend | Suspend Workspace
 
 
 ## Documentation For Models
 
+ - [AlwaysActive](docs/AlwaysActive.md)
  - [Backup](docs/Backup.md)
  - [BaseUser](docs/BaseUser.md)
  - [BatchId](docs/BatchId.md)
  - [BodyBumpAppApiWorkspacesAppNameBumpPost](docs/BodyBumpAppApiWorkspacesAppNameBumpPost.md)
  - [BodyQadeployApiWorkspacesQadeployPost](docs/BodyQadeployApiWorkspacesQadeployPost.md)
  - [BodyQadestroyApiWorkspacesQadestroyPost](docs/BodyQadestroyApiWorkspacesQadestroyPost.md)
  - [Branch](docs/Branch.md)
  - [BuildSchema](docs/BuildSchema.md)
  - [Cluster](docs/Cluster.md)
+ - [CodeMetricBlobPayload](docs/CodeMetricBlobPayload.md)
+ - [CodeMetricBlobResponse](docs/CodeMetricBlobResponse.md)
  - [CopyDBPayload](docs/CopyDBPayload.md)
  - [CreateBackupResponse](docs/CreateBackupResponse.md)
  - [CreateBuildPayload](docs/CreateBuildPayload.md)
  - [CreateMetricPayload](docs/CreateMetricPayload.md)
  - [CreateWorkspacePayload](docs/CreateWorkspacePayload.md)
+ - [Deleted](docs/Deleted.md)
+ - [DisplayName](docs/DisplayName.md)
+ - [Email](docs/Email.md)
+ - [Error](docs/Error.md)
+ - [FirstName](docs/FirstName.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
+ - [Image32](docs/Image32.md)
+ - [IsAdmin](docs/IsAdmin.md)
+ - [IsAppUser](docs/IsAppUser.md)
+ - [IsBot](docs/IsBot.md)
+ - [IsEmailConfirmed](docs/IsEmailConfirmed.md)
+ - [IsOwner](docs/IsOwner.md)
+ - [IsPrimaryOwner](docs/IsPrimaryOwner.md)
+ - [IsRestricted](docs/IsRestricted.md)
  - [Job](docs/Job.md)
  - [JobStatus](docs/JobStatus.md)
+ - [LastName](docs/LastName.md)
  - [Limit](docs/Limit.md)
+ - [ListUserResponse](docs/ListUserResponse.md)
  - [Metric](docs/Metric.md)
  - [MetricName](docs/MetricName.md)
  - [Namespace](docs/Namespace.md)
+ - [Offset](docs/Offset.md)
+ - [Profile](docs/Profile.md)
+ - [RealName](docs/RealName.md)
+ - [ResponseMetadata](docs/ResponseMetadata.md)
  - [ServerTimezone](docs/ServerTimezone.md)
  - [ServerType](docs/ServerType.md)
  - [Size](docs/Size.md)
+ - [SlackMember](docs/SlackMember.md)
+ - [Team](docs/Team.md)
+ - [TeamId](docs/TeamId.md)
+ - [Title](docs/Title.md)
  - [TokenResponse](docs/TokenResponse.md)
+ - [Tz](docs/Tz.md)
+ - [TzLabel](docs/TzLabel.md)
+ - [TzOffset](docs/TzOffset.md)
+ - [Updated](docs/Updated.md)
  - [ValidationError](docs/ValidationError.md)
  - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
  - [VersionsConfig](docs/VersionsConfig.md)
  - [Workspace](docs/Workspace.md)
  - [WorkspaceCluster](docs/WorkspaceCluster.md)
  - [XHubSignature256](docs/XHubSignature256.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
-Endpoints do not require authorization.
+
+Authentication schemes defined for the API:
+<a id="HTTPBearer"></a>
+### HTTPBearer
+
+- **Type**: Bearer authentication
 
 
 ## Author
 
 
 
 
+
```

### Comparing `tickforge_client-1.3.0/pyproject.toml` & `tickforge_client-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tickforge_client"
-version = "1.3.0"
+version = "1.4.0"
 description = "Tickforge API"
 authors = ["William Chu <william.chu@uptickhq.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/uptick/tickforge"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Tickforge API"]
 include = ["tickforge_client/py.typed"]
```

### Comparing `tickforge_client-1.3.0/tickforge_client/__init__.py` & `tickforge_client-1.4.0/tickforge_client/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,77 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Tickforge API
 
     An API to interact with Uptick Internal Resources
 
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.0"
-
-# import apis into sdk package
-from tickforge_client.api.auth_api import AuthApi
-from tickforge_client.api.builds_api import BuildsApi
-from tickforge_client.api.db_api import DbApi
-from tickforge_client.api.default_api import DefaultApi
-from tickforge_client.api.git_api import GitApi
-from tickforge_client.api.github_api import GithubApi
-from tickforge_client.api.jobs_api import JobsApi
-from tickforge_client.api.metrics_api import MetricsApi
-from tickforge_client.api.redirects_api import RedirectsApi
-from tickforge_client.api.slack_api import SlackApi
-from tickforge_client.api.workspaces_api import WorkspacesApi
-
-# import ApiClient
-from tickforge_client.api_response import ApiResponse
-from tickforge_client.api_client import ApiClient
-from tickforge_client.configuration import Configuration
-from tickforge_client.exceptions import OpenApiException
-from tickforge_client.exceptions import ApiTypeError
-from tickforge_client.exceptions import ApiValueError
-from tickforge_client.exceptions import ApiKeyError
-from tickforge_client.exceptions import ApiAttributeError
-from tickforge_client.exceptions import ApiException
-
-# import models into sdk package
+# import models into model package
+from tickforge_client.models.always_active import AlwaysActive
 from tickforge_client.models.backup import Backup
 from tickforge_client.models.base_user import BaseUser
 from tickforge_client.models.batch_id import BatchId
 from tickforge_client.models.body_bump_app_api_workspaces_app_name_bump_post import BodyBumpAppApiWorkspacesAppNameBumpPost
 from tickforge_client.models.body_qadeploy_api_workspaces_qadeploy_post import BodyQadeployApiWorkspacesQadeployPost
 from tickforge_client.models.body_qadestroy_api_workspaces_qadestroy_post import BodyQadestroyApiWorkspacesQadestroyPost
 from tickforge_client.models.branch import Branch
 from tickforge_client.models.build_schema import BuildSchema
 from tickforge_client.models.cluster import Cluster
+from tickforge_client.models.code_metric_blob_payload import CodeMetricBlobPayload
+from tickforge_client.models.code_metric_blob_response import CodeMetricBlobResponse
 from tickforge_client.models.copy_db_payload import CopyDBPayload
 from tickforge_client.models.create_backup_response import CreateBackupResponse
 from tickforge_client.models.create_build_payload import CreateBuildPayload
 from tickforge_client.models.create_metric_payload import CreateMetricPayload
 from tickforge_client.models.create_workspace_payload import CreateWorkspacePayload
+from tickforge_client.models.deleted import Deleted
+from tickforge_client.models.display_name import DisplayName
+from tickforge_client.models.email import Email
+from tickforge_client.models.error import Error
+from tickforge_client.models.first_name import FirstName
 from tickforge_client.models.http_validation_error import HTTPValidationError
+from tickforge_client.models.image32 import Image32
+from tickforge_client.models.is_admin import IsAdmin
+from tickforge_client.models.is_app_user import IsAppUser
+from tickforge_client.models.is_bot import IsBot
+from tickforge_client.models.is_email_confirmed import IsEmailConfirmed
+from tickforge_client.models.is_owner import IsOwner
+from tickforge_client.models.is_primary_owner import IsPrimaryOwner
+from tickforge_client.models.is_restricted import IsRestricted
 from tickforge_client.models.job import Job
 from tickforge_client.models.job_status import JobStatus
+from tickforge_client.models.last_name import LastName
 from tickforge_client.models.limit import Limit
+from tickforge_client.models.list_user_response import ListUserResponse
 from tickforge_client.models.metric import Metric
 from tickforge_client.models.metric_name import MetricName
 from tickforge_client.models.namespace import Namespace
+from tickforge_client.models.offset import Offset
+from tickforge_client.models.profile import Profile
+from tickforge_client.models.real_name import RealName
+from tickforge_client.models.response_metadata import ResponseMetadata
 from tickforge_client.models.server_timezone import ServerTimezone
 from tickforge_client.models.server_type import ServerType
 from tickforge_client.models.size import Size
+from tickforge_client.models.slack_member import SlackMember
+from tickforge_client.models.team import Team
+from tickforge_client.models.team_id import TeamId
+from tickforge_client.models.title import Title
 from tickforge_client.models.token_response import TokenResponse
+from tickforge_client.models.tz import Tz
+from tickforge_client.models.tz_label import TzLabel
+from tickforge_client.models.tz_offset import TzOffset
+from tickforge_client.models.updated import Updated
 from tickforge_client.models.validation_error import ValidationError
 from tickforge_client.models.validation_error_loc_inner import ValidationErrorLocInner
 from tickforge_client.models.versions_config import VersionsConfig
 from tickforge_client.models.workspace import Workspace
 from tickforge_client.models.workspace_cluster import WorkspaceCluster
 from tickforge_client.models.x_hub_signature256 import XHubSignature256
-
-
-def get_sts_url() -> str:
-    import boto3
-    import botocore
-    sts_client = boto3.client("sts")
-    url = botocore.signers.generate_presigned_url(sts_client, "get_caller_identity", HttpMethod="GET")
-    assert isinstance(url, str)
-    return url
-
-
-def get_access_token(configuration=None) -> str:
-    with ApiClient(configuration) as api_client:
-        return AuthApi(api_client).login_for_access_token_api_auth_token_post(username=get_sts_url()).access_token
-
-
-def set_default_config() -> None:
-    access_token = get_access_token()
-    default_api_client = ApiClient()
-    default_api_client.set_default_header("Authorization", f"Bearer {access_token}")
-    ApiClient.set_default(default_api_client)
```

### Comparing `tickforge_client-1.3.0/tickforge_client/api/__init__.py` & `tickforge_client-1.4.0/tickforge_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api/auth_api.py` & `tickforge_client-1.4.0/tickforge_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api/builds_api.py` & `tickforge_client-1.4.0/tickforge_client/api/builds_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api/db_api.py` & `tickforge_client-1.4.0/tickforge_client/api/db_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api/default_api.py` & `tickforge_client-1.4.0/tickforge_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api/git_api.py` & `tickforge_client-1.4.0/tickforge_client/api/git_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api/github_api.py` & `tickforge_client-1.4.0/tickforge_client/api/github_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api/jobs_api.py` & `tickforge_client-1.4.0/tickforge_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api/redirects_api.py` & `tickforge_client-1.4.0/tickforge_client/api/redirects_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api/slack_api.py` & `tickforge_client-1.4.0/tickforge_client/api/slack_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 
 import re  # noqa: F401
 import io
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 
+from pydantic import StrictStr
+
 from typing import Any
 
+from tickforge_client.models.list_user_response import ListUserResponse
 
 from tickforge_client.api_client import ApiClient
 from tickforge_client.api_response import ApiResponse
 from tickforge_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -419,14 +422,163 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def search_users_api_slack_search_get(self, name : StrictStr, email : StrictStr, **kwargs) -> ListUserResponse:  # noqa: E501
+        """Search Users  # noqa: E501
+
+        Given a name and email, find the slack user that matches the search criteria  This is a proxied endpoint for downstream services that behaves like slacks api  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.search_users_api_slack_search_get(name, email, async_req=True)
+        >>> result = thread.get()
+
+        :param name: (required)
+        :type name: str
+        :param email: (required)
+        :type email: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ListUserResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the search_users_api_slack_search_get_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.search_users_api_slack_search_get_with_http_info(name, email, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def search_users_api_slack_search_get_with_http_info(self, name : StrictStr, email : StrictStr, **kwargs) -> ApiResponse:  # noqa: E501
+        """Search Users  # noqa: E501
+
+        Given a name and email, find the slack user that matches the search criteria  This is a proxied endpoint for downstream services that behaves like slacks api  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.search_users_api_slack_search_get_with_http_info(name, email, async_req=True)
+        >>> result = thread.get()
+
+        :param name: (required)
+        :type name: str
+        :param email: (required)
+        :type email: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(ListUserResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'name',
+            'email'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method search_users_api_slack_search_get" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('name') is not None:  # noqa: E501
+            _query_params.append(('name', _params['name']))
+
+        if _params.get('email') is not None:  # noqa: E501
+            _query_params.append(('email', _params['email']))
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['HTTPBearer']  # noqa: E501
+
+        _response_types_map = {
+            '200': "ListUserResponse",
+            '422': "HTTPValidationError",
+        }
+
+        return self.api_client.call_api(
+            '/api/slack/search', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `tickforge_client-1.3.0/tickforge_client/api/workspaces_api.py` & `tickforge_client-1.4.0/tickforge_client/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/api_client.py` & `tickforge_client-1.4.0/tickforge_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.4.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tickforge_client-1.3.0/tickforge_client/api_response.py` & `tickforge_client-1.4.0/tickforge_client/api_response.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/configuration.py` & `tickforge_client-1.4.0/tickforge_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum
       values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
       in PEM format.
 
+    :Example:
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
@@ -353,26 +354,33 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
+        if self.access_token is not None:
+            auth['HTTPBearer'] = {
+                'type': 'bearer',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': 'Bearer ' + self.access_token
+            }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.3.0".\
+               "SDK Package Version: 1.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `tickforge_client-1.3.0/tickforge_client/exceptions.py` & `tickforge_client-1.4.0/tickforge_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/author_name.py` & `tickforge_client-1.4.0/tickforge_client/models/author_name.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/backup.py` & `tickforge_client-1.4.0/tickforge_client/models/backup.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/base_user.py` & `tickforge_client-1.4.0/tickforge_client/models/base_user.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/batch_id.py` & `tickforge_client-1.4.0/tickforge_client/models/batch_id.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/body_bump_app_api_workspaces_app_name_bump_post.py` & `tickforge_client-1.4.0/tickforge_client/models/body_bump_app_api_workspaces_app_name_bump_post.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/body_qadeploy_api_workspaces_qadeploy_post.py` & `tickforge_client-1.4.0/tickforge_client/models/body_qadeploy_api_workspaces_qadeploy_post.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/body_qadestroy_api_workspaces_qadestroy_post.py` & `tickforge_client-1.4.0/tickforge_client/models/body_qadestroy_api_workspaces_qadestroy_post.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/branch.py` & `tickforge_client-1.4.0/tickforge_client/models/branch.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/build_schema.py` & `tickforge_client-1.4.0/tickforge_client/models/build_schema.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/cluster.py` & `tickforge_client-1.4.0/tickforge_client/models/job_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,28 +17,26 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class Cluster(str, Enum):
+class JobStatus(str, Enum):
     """
-    Name of our EKS Clusters
+    JobStatus
     """
 
     """
     allowed enum values
     """
-    LUNA = 'luna'
-    BLUE = 'blue'
-    SOOTY = 'sooty'
-    THEO = 'theo'
-    MESHMESH = 'meshmesh'
-    STAGING = 'staging'
+    QUEUED = 'QUEUED'
+    FAILED = 'FAILED'
+    RUNNING = 'RUNNING'
+    DONE = 'DONE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> Cluster:
-        """Create an instance of Cluster from a JSON string"""
-        return Cluster(json.loads(json_str))
+    def from_json(cls, json_str: str) -> JobStatus:
+        """Create an instance of JobStatus from a JSON string"""
+        return JobStatus(json.loads(json_str))
```

### Comparing `tickforge_client-1.3.0/tickforge_client/models/copy_db_payload.py` & `tickforge_client-1.4.0/tickforge_client/models/copy_db_payload.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/create_backup_response.py` & `tickforge_client-1.4.0/tickforge_client/models/create_backup_response.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/create_build_payload.py` & `tickforge_client-1.4.0/tickforge_client/models/create_build_payload.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/create_metric_payload.py` & `tickforge_client-1.4.0/tickforge_client/models/create_metric_payload.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/create_workspace_payload.py` & `tickforge_client-1.4.0/tickforge_client/models/create_workspace_payload.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/http_validation_error.py` & `tickforge_client-1.4.0/tickforge_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/job.py` & `tickforge_client-1.4.0/tickforge_client/models/job.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/job_status.py` & `tickforge_client-1.4.0/tickforge_client/models/server_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class JobStatus(str, Enum):
+class ServerType(str, Enum):
     """
-    JobStatus
+    ServerType
     """
 
     """
     allowed enum values
     """
-    QUEUED = 'QUEUED'
-    FAILED = 'FAILED'
-    RUNNING = 'RUNNING'
-    DONE = 'DONE'
+    PRODUCTION = 'production'
+    TEMPLATE = 'template'
+    SANDBOX = 'sandbox'
+    QA = 'qa'
 
     @classmethod
-    def from_json(cls, json_str: str) -> JobStatus:
-        """Create an instance of JobStatus from a JSON string"""
-        return JobStatus(json.loads(json_str))
+    def from_json(cls, json_str: str) -> ServerType:
+        """Create an instance of ServerType from a JSON string"""
+        return ServerType(json.loads(json_str))
```

### Comparing `tickforge_client-1.3.0/tickforge_client/models/limit.py` & `tickforge_client-1.4.0/tickforge_client/models/limit.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/metric.py` & `tickforge_client-1.4.0/tickforge_client/models/metric.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/metric_name.py` & `tickforge_client-1.4.0/tickforge_client/models/metric_name.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/namespace.py` & `tickforge_client-1.4.0/tickforge_client/models/namespace.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/server_timezone.py` & `tickforge_client-1.4.0/tickforge_client/models/server_timezone.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/server_type.py` & `tickforge_client-1.4.0/tickforge_client/models/cluster.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,26 +17,32 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ServerType(str, Enum):
+class Cluster(str, Enum):
     """
-    ServerType
+    Name of our EKS Clusters
     """
 
     """
     allowed enum values
     """
-    PRODUCTION = 'production'
-    TEMPLATE = 'template'
-    SANDBOX = 'sandbox'
-    QA = 'qa'
+    LUNA = 'luna'
+    BLUE = 'blue'
+    SOOTY = 'sooty'
+    THEO = 'theo'
+    DEV_MINUS_AU_MINUS_1 = 'dev-au-1'
+    STAGING_MINUS_AU_MINUS_1 = 'staging-au-1'
+    PROD_MINUS_AU_MINUS_1 = 'prod-au-1'
+    PROD_MINUS_AU_MINUS_2 = 'prod-au-2'
+    PROD_MINUS_GB_MINUS_1 = 'prod-gb-1'
+    OBSERVABILITY = 'observability'
 
     @classmethod
-    def from_json(cls, json_str: str) -> ServerType:
-        """Create an instance of ServerType from a JSON string"""
-        return ServerType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> Cluster:
+        """Create an instance of Cluster from a JSON string"""
+        return Cluster(json.loads(json_str))
```

### Comparing `tickforge_client-1.3.0/tickforge_client/models/size.py` & `tickforge_client-1.4.0/tickforge_client/models/size.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/token_response.py` & `tickforge_client-1.4.0/tickforge_client/models/token_response.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/validation_error.py` & `tickforge_client-1.4.0/tickforge_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/validation_error_loc_inner.py` & `tickforge_client-1.4.0/tickforge_client/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/versions_config.py` & `tickforge_client-1.4.0/tickforge_client/models/versions_config.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/workspace.py` & `tickforge_client-1.4.0/tickforge_client/models/workspace.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/workspace_cluster.py` & `tickforge_client-1.4.0/tickforge_client/models/workspace_cluster.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/models/x_hub_signature256.py` & `tickforge_client-1.4.0/tickforge_client/models/x_hub_signature256.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/tickforge_client/rest.py` & `tickforge_client-1.4.0/tickforge_client/rest.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.3.0/PKG-INFO` & `tickforge_client-1.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,14 @@
-Metadata-Version: 2.1
-Name: tickforge_client
-Version: 1.3.0
-Summary: Tickforge API
-Home-page: https://github.com/uptick/tickforge
-License: NoLicense
-Keywords: OpenAPI,OpenAPI-Generator,Tickforge API
-Author: William Chu
-Author-email: william.chu@uptickhq.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aenum (>=3.1.11)
-Requires-Dist: boto3
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: python-dateutil (>=2.8.2)
-Requires-Dist: urllib3 (>=1.25.3)
-Project-URL: Repository, https://github.com/uptick/tickforge
-Description-Content-Type: text/markdown
-
 # tickforge-client
 An API to interact with Uptick Internal Resources
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.3.0
+- Package version: 1.4.0
 - Build package: org.openapitools.codegen.languages.PythonPydanticV1ClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -121,73 +95,110 @@
 *DefaultApi* | [**health_check_livez_get**](docs/DefaultApi.md#health_check_livez_get) | **GET** /livez | Health Check
 *DefaultApi* | [**health_check_readyz_get**](docs/DefaultApi.md#health_check_readyz_get) | **GET** /readyz | Health Check
 *GitApi* | [**refresh_respository_api_git_refresh_repository_post**](docs/GitApi.md#refresh_respository_api_git_refresh_repository_post) | **POST** /api/git/refresh_repository | Refresh Respository
 *GitApi* | [**versions_config_api_git_versions_get**](docs/GitApi.md#versions_config_api_git_versions_get) | **GET** /api/git/versions | Versions Config
 *GithubApi* | [**workflow_job_webhook_api_github_webhooks_workflow_job_post**](docs/GithubApi.md#workflow_job_webhook_api_github_webhooks_workflow_job_post) | **POST** /api/github/webhooks/workflow_job | Workflow Job Webhook
 *JobsApi* | [**get_job_api_jobs_job_id_get**](docs/JobsApi.md#get_job_api_jobs_job_id_get) | **GET** /api/jobs/{job_id} | Get Job
 *MetricsApi* | [**create_metric_api_metrics_post**](docs/MetricsApi.md#create_metric_api_metrics_post) | **POST** /api/metrics/ | Create Metric
+*MetricsApi* | [**create_metric_blob_api_metrics_blob_post**](docs/MetricsApi.md#create_metric_blob_api_metrics_blob_post) | **POST** /api/metrics/blob | Create Metric Blob
 *MetricsApi* | [**get_metric_api_metrics_get**](docs/MetricsApi.md#get_metric_api_metrics_get) | **GET** /api/metrics/ | Get Metric
+*MetricsApi* | [**get_metric_blob_api_metrics_blob_get**](docs/MetricsApi.md#get_metric_blob_api_metrics_blob_get) | **GET** /api/metrics/blob | Get Metric Blob
 *RedirectsApi* | [**me_redirect_me_get**](docs/RedirectsApi.md#me_redirect_me_get) | **GET** /me | Me Redirect
 *RedirectsApi* | [**refresh_repository_redirect_api_refresh_repository_post**](docs/RedirectsApi.md#refresh_repository_redirect_api_refresh_repository_post) | **POST** /api/refresh_repository | Refresh Repository Redirect
 *RedirectsApi* | [**token_redirect_token_post**](docs/RedirectsApi.md#token_redirect_token_post) | **POST** /token | Token Redirect
 *RedirectsApi* | [**versions_redirect_api_versions_get**](docs/RedirectsApi.md#versions_redirect_api_versions_get) | **GET** /api/versions | Versions Redirect
 *SlackApi* | [**event_handler_slack_events_get**](docs/SlackApi.md#event_handler_slack_events_get) | **GET** /slack/events | Event Handler
 *SlackApi* | [**event_handler_slack_events_patch**](docs/SlackApi.md#event_handler_slack_events_patch) | **PATCH** /slack/events | Event Handler
 *SlackApi* | [**event_handler_slack_events_post**](docs/SlackApi.md#event_handler_slack_events_post) | **POST** /slack/events | Event Handler
+*SlackApi* | [**search_users_api_slack_search_get**](docs/SlackApi.md#search_users_api_slack_search_get) | **GET** /api/slack/search | Search Users
 *WorkspacesApi* | [**bump_app_api_workspaces_app_name_bump_post**](docs/WorkspacesApi.md#bump_app_api_workspaces_app_name_bump_post) | **POST** /api/workspaces/{app_name}/bump | Bump App
 *WorkspacesApi* | [**create_backup_api_workspaces_workspace_name_backups_post**](docs/WorkspacesApi.md#create_backup_api_workspaces_workspace_name_backups_post) | **POST** /api/workspaces/{workspace_name}/backups | Create Backup
 *WorkspacesApi* | [**create_workspace_api_workspaces_create_post**](docs/WorkspacesApi.md#create_workspace_api_workspaces_create_post) | **POST** /api/workspaces/create | Create Workspace
 *WorkspacesApi* | [**create_workspace_api_workspaces_post**](docs/WorkspacesApi.md#create_workspace_api_workspaces_post) | **POST** /api/workspaces/ | Create Workspace
 *WorkspacesApi* | [**list_backups_api_workspaces_workspace_name_backups_get**](docs/WorkspacesApi.md#list_backups_api_workspaces_workspace_name_backups_get) | **GET** /api/workspaces/{workspace_name}/backups | List Backups
 *WorkspacesApi* | [**list_workspaces_api_workspaces_get**](docs/WorkspacesApi.md#list_workspaces_api_workspaces_get) | **GET** /api/workspaces/ | List Workspaces
 *WorkspacesApi* | [**qadeploy_api_workspaces_qadeploy_post**](docs/WorkspacesApi.md#qadeploy_api_workspaces_qadeploy_post) | **POST** /api/workspaces/qadeploy | Qadeploy
 *WorkspacesApi* | [**qadestroy_api_workspaces_qadestroy_post**](docs/WorkspacesApi.md#qadestroy_api_workspaces_qadestroy_post) | **POST** /api/workspaces/qadestroy | Qadestroy
 *WorkspacesApi* | [**suspend_workspace_api_workspaces_workspace_name_suspend_post**](docs/WorkspacesApi.md#suspend_workspace_api_workspaces_workspace_name_suspend_post) | **POST** /api/workspaces/{workspace_name}/suspend | Suspend Workspace
 
 
 ## Documentation For Models
 
+ - [AlwaysActive](docs/AlwaysActive.md)
  - [Backup](docs/Backup.md)
  - [BaseUser](docs/BaseUser.md)
  - [BatchId](docs/BatchId.md)
  - [BodyBumpAppApiWorkspacesAppNameBumpPost](docs/BodyBumpAppApiWorkspacesAppNameBumpPost.md)
  - [BodyQadeployApiWorkspacesQadeployPost](docs/BodyQadeployApiWorkspacesQadeployPost.md)
  - [BodyQadestroyApiWorkspacesQadestroyPost](docs/BodyQadestroyApiWorkspacesQadestroyPost.md)
  - [Branch](docs/Branch.md)
  - [BuildSchema](docs/BuildSchema.md)
  - [Cluster](docs/Cluster.md)
+ - [CodeMetricBlobPayload](docs/CodeMetricBlobPayload.md)
+ - [CodeMetricBlobResponse](docs/CodeMetricBlobResponse.md)
  - [CopyDBPayload](docs/CopyDBPayload.md)
  - [CreateBackupResponse](docs/CreateBackupResponse.md)
  - [CreateBuildPayload](docs/CreateBuildPayload.md)
  - [CreateMetricPayload](docs/CreateMetricPayload.md)
  - [CreateWorkspacePayload](docs/CreateWorkspacePayload.md)
+ - [Deleted](docs/Deleted.md)
+ - [DisplayName](docs/DisplayName.md)
+ - [Email](docs/Email.md)
+ - [Error](docs/Error.md)
+ - [FirstName](docs/FirstName.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
+ - [Image32](docs/Image32.md)
+ - [IsAdmin](docs/IsAdmin.md)
+ - [IsAppUser](docs/IsAppUser.md)
+ - [IsBot](docs/IsBot.md)
+ - [IsEmailConfirmed](docs/IsEmailConfirmed.md)
+ - [IsOwner](docs/IsOwner.md)
+ - [IsPrimaryOwner](docs/IsPrimaryOwner.md)
+ - [IsRestricted](docs/IsRestricted.md)
  - [Job](docs/Job.md)
  - [JobStatus](docs/JobStatus.md)
+ - [LastName](docs/LastName.md)
  - [Limit](docs/Limit.md)
+ - [ListUserResponse](docs/ListUserResponse.md)
  - [Metric](docs/Metric.md)
  - [MetricName](docs/MetricName.md)
  - [Namespace](docs/Namespace.md)
+ - [Offset](docs/Offset.md)
+ - [Profile](docs/Profile.md)
+ - [RealName](docs/RealName.md)
+ - [ResponseMetadata](docs/ResponseMetadata.md)
  - [ServerTimezone](docs/ServerTimezone.md)
  - [ServerType](docs/ServerType.md)
  - [Size](docs/Size.md)
+ - [SlackMember](docs/SlackMember.md)
+ - [Team](docs/Team.md)
+ - [TeamId](docs/TeamId.md)
+ - [Title](docs/Title.md)
  - [TokenResponse](docs/TokenResponse.md)
+ - [Tz](docs/Tz.md)
+ - [TzLabel](docs/TzLabel.md)
+ - [TzOffset](docs/TzOffset.md)
+ - [Updated](docs/Updated.md)
  - [ValidationError](docs/ValidationError.md)
  - [ValidationErrorLocInner](docs/ValidationErrorLocInner.md)
  - [VersionsConfig](docs/VersionsConfig.md)
  - [Workspace](docs/Workspace.md)
  - [WorkspaceCluster](docs/WorkspaceCluster.md)
  - [XHubSignature256](docs/XHubSignature256.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
-Endpoints do not require authorization.
 
+Authentication schemes defined for the API:
+<a id="HTTPBearer"></a>
+### HTTPBearer
 
-## Author
+- **Type**: Bearer authentication
 
 
+## Author
+
```


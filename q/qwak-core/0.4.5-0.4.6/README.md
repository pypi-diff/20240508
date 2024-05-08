# Comparing `tmp/qwak_core-0.4.5.tar.gz` & `tmp/qwak_core-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.4.5.tar", max compression
+gzip compressed data, was "qwak_core-0.4.6.tar", max compression
```

## Comparing `qwak_core-0.4.5.tar` & `qwak_core-0.4.6.tar`

### file list

```diff
@@ -1,818 +1,818 @@
--rw-r--r--   0        0        0      264 2024-05-08 07:57:46.499539 qwak_core-0.4.5/README.md
--rw-r--r--   0        0        0        0 2024-05-08 08:02:06.905411 qwak_core-0.4.5/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5877 2024-05-08 08:02:06.993412 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     7824 2024-05-08 08:01:19.557052 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:06.997412 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0    12703 2024-05-08 08:02:06.997412 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py
--rw-r--r--   0        0        0    10914 2024-05-08 08:01:19.897055 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi
--rw-r--r--   0        0        0    14681 2024-05-08 08:02:07.001412 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2024-05-08 08:02:06.985412 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2024-05-08 08:01:18.881048 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:06.985412 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2024-05-08 08:02:06.989412 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2024-05-08 08:01:19.233050 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:06.989412 qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2024-05-08 08:02:06.969412 qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2024-05-08 08:01:17.877040 qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2024-05-08 08:02:06.973412 qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2024-05-08 08:02:06.973412 qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2024-05-08 08:01:18.209043 qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:06.977412 qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2024-05-08 08:02:06.977412 qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2024-05-08 08:01:18.545045 qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:06.981412 qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2024-05-08 08:02:06.905411 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2024-05-08 08:01:17.513038 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2024-05-08 08:02:06.941412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     7360 2024-05-08 08:02:06.945412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0    11651 2024-05-08 08:01:20.249057 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:06.949412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     5029 2024-05-08 08:02:06.953412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     6943 2024-05-08 08:01:20.949062 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:06.957412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2024-05-08 08:02:06.961412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2024-05-08 08:01:21.293065 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2024-05-08 08:02:06.961412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2024-05-08 08:02:06.949412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2024-05-08 08:01:20.585060 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:06.953412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6541 2024-05-08 08:02:06.965412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10595 2024-05-08 08:01:21.613067 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:06.965412 qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0    15382 2024-05-08 08:02:07.065413 qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    20668 2024-05-08 08:01:26.161099 qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.069413 qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2024-05-08 08:02:07.069413 qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2024-05-08 08:01:26.485101 qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2024-05-08 08:02:07.073413 qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7616 2024-05-08 08:02:07.293415 qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11995 2024-05-08 08:01:41.729210 qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.293415 qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0    14893 2024-05-08 08:02:07.297415 qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0    11812 2024-05-08 08:01:42.025211 qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    19155 2024-05-08 08:02:07.301415 qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2024-05-08 08:02:07.305415 qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2024-05-08 08:01:43.973226 qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2024-05-08 08:02:07.309415 qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8864 2024-05-08 08:02:07.301415 qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13789 2024-05-08 08:01:43.597223 qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.305415 qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2024-05-08 08:02:07.309415 qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2024-05-08 08:01:44.353229 qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.313415 qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2024-05-08 08:02:07.313415 qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2024-05-08 08:01:44.693232 qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2024-05-08 08:02:07.317415 qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    14053 2024-05-08 08:02:07.549417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    20860 2024-05-08 08:02:01.273363 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.549417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2024-05-08 08:02:07.541417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2024-05-08 08:02:00.605357 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.541417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3954 2024-05-08 08:02:07.545417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     5309 2024-05-08 08:02:00.913360 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.545417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    21176 2024-05-08 08:02:07.533417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    15049 2024-05-08 08:01:59.933352 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    25475 2024-05-08 08:02:07.533417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2024-05-08 08:02:07.537417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2024-05-08 08:02:00.289355 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.537417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2024-05-08 08:02:07.561417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2024-05-08 08:02:02.217371 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.561417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2024-05-08 08:02:07.557417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2024-05-08 08:02:01.905368 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.557417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2024-05-08 08:02:07.553417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2024-05-08 08:02:01.581366 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.553417 qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    11218 2024-05-08 08:02:07.529417 qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    15584 2024-05-08 08:01:59.581349 qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.529417 qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2083 2024-05-08 08:02:07.521417 qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1977 2024-05-08 08:01:58.861342 qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.521417 qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    46028 2024-05-08 08:02:07.525417 qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    60013 2024-05-08 08:01:59.245346 qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    32008 2024-05-08 08:02:07.525417 qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    29124 2024-05-08 08:02:07.421416 qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    24434 2024-05-08 08:01:48.545262 qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    27837 2024-05-08 08:02:07.425416 qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    33279 2024-05-08 08:02:07.417416 qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    52325 2024-05-08 08:01:47.773256 qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.421416 qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0     5757 2024-05-08 08:02:07.429416 qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py
--rw-r--r--   0        0        0     4013 2024-05-08 08:01:49.653271 qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi
--rw-r--r--   0        0        0     6783 2024-05-08 08:02:07.433416 qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py
--rw-r--r--   0        0        0     6016 2024-05-08 08:02:07.425416 qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_pb2.py
--rw-r--r--   0        0        0     7049 2024-05-08 08:01:49.285268 qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.429416 qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_pb2_grpc.py
--rw-r--r--   0        0        0    14932 2024-05-08 08:02:07.393416 qwak_core-0.4.5/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    24192 2024-05-08 08:01:47.373253 qwak_core-0.4.5/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.397415 qwak_core-0.4.5/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     5552 2024-05-08 08:02:07.397415 qwak_core-0.4.5/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     7299 2024-05-08 08:01:48.149259 qwak_core-0.4.5/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.401416 qwak_core-0.4.5/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    15672 2024-05-08 08:02:07.401416 qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0    12741 2024-05-08 08:01:48.929266 qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    16925 2024-05-08 08:02:07.405416 qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38491 2024-05-08 08:02:07.413416 qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    53557 2024-05-08 08:01:50.865281 qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2024-05-08 08:02:07.413416 qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     3508 2024-05-08 08:02:07.405416 qwak_core-0.4.5/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     2300 2024-05-08 08:01:49.989274 qwak_core-0.4.5/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0     3101 2024-05-08 08:02:07.409416 qwak_core-0.4.5/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0     2270 2024-05-08 08:02:07.445416 qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     2697 2024-05-08 08:01:51.685287 qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.445416 qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4458 2024-05-08 08:02:07.445416 qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     3113 2024-05-08 08:01:52.061290 qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2024-05-08 08:02:07.449416 qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2024-05-08 08:02:07.381415 qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2024-05-08 08:01:46.269245 qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.385415 qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11871 2024-05-08 08:02:07.385415 qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     8790 2024-05-08 08:01:46.625247 qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2024-05-08 08:02:07.389416 qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2024-05-08 08:02:07.373415 qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2024-05-08 08:01:45.485238 qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.377415 qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    50041 2024-05-08 08:02:07.317415 qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    74372 2024-05-08 08:01:45.089235 qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.321415 qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    46309 2024-05-08 08:02:07.377415 qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    40356 2024-05-08 08:01:45.901242 qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    27756 2024-05-08 08:02:07.381415 qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     3345 2024-05-08 08:02:07.041412 qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     4098 2024-05-08 08:01:24.509087 qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.045413 qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12707 2024-05-08 08:02:07.045413 qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    13800 2024-05-08 08:01:24.825090 qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.049413 qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    17949 2024-05-08 08:02:07.049413 qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    18562 2024-05-08 08:01:25.185092 qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    12833 2024-05-08 08:02:07.053413 qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     6463 2024-05-08 08:02:07.213414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/backfill_pb2.py
--rw-r--r--   0        0        0     7945 2024-05-08 08:01:34.609159 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.217414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/backfill_pb2_grpc.py
--rw-r--r--   0        0        0     2971 2024-05-08 08:02:07.217414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/batch_pb2.py
--rw-r--r--   0        0        0     3266 2024-05-08 08:01:34.901161 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.221414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/batch_pb2_grpc.py
--rw-r--r--   0        0        0     2210 2024-05-08 08:02:07.221414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/deletion_pb2.py
--rw-r--r--   0        0        0     1540 2024-05-08 08:01:35.221163 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.225414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/deletion_pb2_grpc.py
--rw-r--r--   0        0        0     5793 2024-05-08 08:02:07.229414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_pb2.py
--rw-r--r--   0        0        0     7373 2024-05-08 08:01:35.525165 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.229414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_pb2_grpc.py
--rw-r--r--   0        0        0    14900 2024-05-08 08:02:07.233414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_service_pb2.py
--rw-r--r--   0        0        0    11103 2024-05-08 08:01:35.881168 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi
--rw-r--r--   0        0        0    17220 2024-05-08 08:02:07.233414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py
--rw-r--r--   0        0        0     7695 2024-05-08 08:02:07.241414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py
--rw-r--r--   0        0        0    14959 2024-05-08 08:01:36.593173 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.241414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0    19304 2024-05-08 08:02:07.245414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py
--rw-r--r--   0        0        0    16916 2024-05-08 08:01:36.897175 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    21145 2024-05-08 08:02:07.245414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     8440 2024-05-08 08:02:07.237414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py
--rw-r--r--   0        0        0    13312 2024-05-08 08:01:36.281171 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.237414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     2051 2024-05-08 08:02:07.249414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py
--rw-r--r--   0        0        0     1952 2024-05-08 08:01:37.201177 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.249414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_pb2_grpc.py
--rw-r--r--   0        0        0    12222 2024-05-08 08:02:07.253414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py
--rw-r--r--   0        0        0     7930 2024-05-08 08:01:37.525179 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi
--rw-r--r--   0        0        0    14212 2024-05-08 08:02:07.257414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py
--rw-r--r--   0        0        0     1685 2024-05-08 08:02:07.257414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py
--rw-r--r--   0        0        0     1272 2024-05-08 08:01:37.829182 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.261414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2_grpc.py
--rw-r--r--   0        0        0     6198 2024-05-08 08:02:07.261414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py
--rw-r--r--   0        0        0     7677 2024-05-08 08:01:38.121184 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.265414 qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2024-05-08 08:02:07.169414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2024-05-08 08:01:34.305157 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.173414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2024-05-08 08:02:07.165413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2024-05-08 08:01:33.989154 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2024-05-08 08:02:07.165413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2024-05-08 08:02:07.113413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2024-05-08 08:01:30.445129 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.117413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0    13825 2024-05-08 08:02:07.137413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_pb2.py
--rw-r--r--   0        0        0    19227 2024-05-08 08:01:32.037141 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.137413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3307 2024-05-08 08:02:07.141413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py
--rw-r--r--   0        0        0     1637 2024-05-08 08:01:32.353143 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3293 2024-05-08 08:02:07.145413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2024-05-08 08:02:07.109413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2024-05-08 08:01:30.141127 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.113413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2024-05-08 08:02:07.093413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2024-05-08 08:01:29.201120 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.097413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2024-05-08 08:02:07.105413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2024-05-08 08:01:29.837125 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2024-05-08 08:02:07.105413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2024-05-08 08:02:07.117413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2024-05-08 08:01:30.761132 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.121413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2024-05-08 08:02:07.125413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2024-05-08 08:01:31.093134 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2024-05-08 08:02:07.125413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    26853 2024-05-08 08:02:07.097413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    39247 2024-05-08 08:01:29.513123 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.101413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2024-05-08 08:02:07.129413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2024-05-08 08:01:31.397136 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.129413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    13240 2024-05-08 08:02:07.133413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    18420 2024-05-08 08:01:31.705138 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.133413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2024-05-08 08:02:07.173414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2024-05-08 08:02:05.337398 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.177414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2024-05-08 08:02:07.177414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2024-05-08 08:02:05.677401 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2024-05-08 08:02:07.181414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     4308 2024-05-08 08:02:07.185414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     7410 2024-05-08 08:01:40.817203 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.185414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    15316 2024-05-08 08:02:07.189414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    14087 2024-05-08 08:01:41.129205 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    18465 2024-05-08 08:02:07.189414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2024-05-08 08:02:07.193414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2024-05-08 08:01:41.433207 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.193414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     5111 2024-05-08 08:02:07.209414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/management_pb2.py
--rw-r--r--   0        0        0     2739 2024-05-08 08:01:43.249221 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi
--rw-r--r--   0        0        0     5436 2024-05-08 08:02:07.213414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py
--rw-r--r--   0        0        0     5385 2024-05-08 08:02:07.201414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     7551 2024-05-08 08:01:42.629216 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.205414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    17474 2024-05-08 08:02:07.197414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2024-05-08 08:01:42.325214 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2024-05-08 08:02:07.197414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2024-05-08 08:02:07.205414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2024-05-08 08:01:42.917218 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.209414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    27355 2024-05-08 08:02:07.145413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    43393 2024-05-08 08:01:32.681145 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.149413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5147 2024-05-08 08:02:07.149413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6208 2024-05-08 08:01:33.009148 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.153413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2024-05-08 08:02:07.153413 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2024-05-08 08:01:33.353150 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2024-05-08 08:02:07.157414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11049 2024-05-08 08:02:07.161414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15942 2024-05-08 08:01:33.677152 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.161414 qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2024-05-08 08:02:07.573417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2024-05-08 08:02:03.441382 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.577417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2024-05-08 08:02:07.577417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2024-05-08 08:02:03.753384 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2024-05-08 08:02:07.581417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2024-05-08 08:02:07.581417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2024-05-08 08:02:04.073387 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.585417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2024-05-08 08:02:07.585417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2024-05-08 08:02:04.397390 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2024-05-08 08:02:07.585417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0    10469 2024-05-08 08:02:07.593417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0    11719 2024-05-08 08:02:04.741393 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     9458 2024-05-08 08:02:07.593417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     5302 2024-05-08 08:02:07.597417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     5484 2024-05-08 08:02:05.037395 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.597417 qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2975 2024-05-08 08:02:07.449416 qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     4026 2024-05-08 08:01:52.409293 qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.453416 qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4455 2024-05-08 08:02:07.453416 qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     3113 2024-05-08 08:01:52.769296 qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2024-05-08 08:02:07.457416 qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6950 2024-05-08 08:02:07.073413 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    11560 2024-05-08 08:01:27.825111 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.077413 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     3442 2024-05-08 08:02:07.081413 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     5719 2024-05-08 08:01:28.141113 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.081413 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2024-05-08 08:02:07.085413 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2024-05-08 08:01:28.473115 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2024-05-08 08:02:07.089413 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8504 2024-05-08 08:02:07.089413 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12440 2024-05-08 08:01:28.769117 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.093413 qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2024-05-08 08:02:07.389416 qwak_core-0.4.5/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2024-05-08 08:01:46.993250 qwak_core-0.4.5/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2024-05-08 08:02:07.393416 qwak_core-0.4.5/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3876 2024-05-08 08:02:07.457416 qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4658 2024-05-08 08:01:53.133299 qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.461416 qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2024-05-08 08:02:07.461416 qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2024-05-08 08:01:53.481301 qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2024-05-08 08:02:07.465416 qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2024-05-08 08:02:07.485416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2024-05-08 08:01:55.649319 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.489416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2024-05-08 08:02:07.489416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2024-05-08 08:01:55.993321 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.493416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    25218 2024-05-08 08:02:07.493416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    31280 2024-05-08 08:01:56.349324 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.493416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13432 2024-05-08 08:02:07.497416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    22974 2024-05-08 08:01:56.697327 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.501417 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12784 2024-05-08 08:02:07.501417 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16585 2024-05-08 08:01:57.081329 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.505416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    51171 2024-05-08 08:02:07.505416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    40800 2024-05-08 08:01:57.469332 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    73869 2024-05-08 08:02:07.509416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-05-08 08:02:07.509416 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2024-05-08 08:01:57.813335 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.513417 qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2024-05-08 08:02:07.469416 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2024-05-08 08:01:54.201307 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.473416 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2024-05-08 08:02:07.481416 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2024-05-08 08:01:55.297316 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.485416 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2024-05-08 08:02:07.473416 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2024-05-08 08:01:54.601310 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2024-05-08 08:02:07.477416 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2024-05-08 08:02:07.477416 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2024-05-08 08:01:54.969313 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.481416 qwak_core-0.4.5/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    27866 2024-05-08 08:02:07.441416 qwak_core-0.4.5/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    32184 2024-05-08 08:01:51.305284 qwak_core-0.4.5/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    19830 2024-05-08 08:02:07.441416 qwak_core-0.4.5/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2024-05-08 08:02:07.033412 qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2024-05-08 08:01:27.133106 qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2024-05-08 08:02:07.033412 qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2024-05-08 08:02:07.025412 qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2024-05-08 08:01:26.821104 qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.029412 qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2024-05-08 08:02:07.037413 qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2024-05-08 08:01:27.493108 qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2024-05-08 08:02:07.037413 qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     1598 2024-05-08 08:02:07.565417 qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py
--rw-r--r--   0        0        0     1221 2024-05-08 08:02:02.517374 qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.565417 qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2_grpc.py
--rw-r--r--   0        0        0    11437 2024-05-08 08:02:07.569417 qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py
--rw-r--r--   0        0        0    12170 2024-05-08 08:02:03.145379 qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi
--rw-r--r--   0        0        0     9793 2024-05-08 08:02:07.573417 qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4060 2024-05-08 08:02:07.569417 qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/population_pb2.py
--rw-r--r--   0        0        0     3906 2024-05-08 08:02:02.837376 qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.569417 qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/population_pb2_grpc.py
--rw-r--r--   0        0        0    10804 2024-05-08 08:02:07.433416 qwak_core-0.4.5/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0    12120 2024-05-08 08:01:50.441278 qwak_core-0.4.5/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     9642 2024-05-08 08:02:07.437416 qwak_core-0.4.5/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2024-05-08 08:02:07.465416 qwak_core-0.4.5/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2024-05-08 08:01:53.849304 qwak_core-0.4.5/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2024-05-08 08:02:07.469416 qwak_core-0.4.5/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0    10718 2024-05-08 08:02:07.021412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0    12627 2024-05-08 08:01:23.213078 qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.021412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    19751 2024-05-08 08:02:07.017412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    13467 2024-05-08 08:01:22.909076 qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    24352 2024-05-08 08:02:07.017412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2024-05-08 08:02:07.001412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2024-05-08 08:01:21.941069 qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.005412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2477 2024-05-08 08:02:07.005412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2679 2024-05-08 08:01:22.261072 qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.009412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2024-05-08 08:02:07.013412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2024-05-08 08:01:22.573074 qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2024-05-08 08:02:07.013412 qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6909 2024-05-08 08:02:07.517417 qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     5186 2024-05-08 08:01:58.513340 qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2024-05-08 08:02:07.521417 qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7868 2024-05-08 08:02:07.513417 qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    12177 2024-05-08 08:01:58.161337 qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.517417 qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11396 2024-05-08 08:02:07.053413 qwak_core-0.4.5/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15139 2024-05-08 08:01:25.501094 qwak_core-0.4.5/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.057413 qwak_core-0.4.5/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3645 2024-05-08 08:02:07.061413 qwak_core-0.4.5/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2983 2024-05-08 08:01:25.837097 qwak_core-0.4.5/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.061413 qwak_core-0.4.5/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     8648 2024-05-08 08:02:07.269415 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py
--rw-r--r--   0        0        0    12852 2024-05-08 08:01:38.709188 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.273414 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_pb2_grpc.py
--rw-r--r--   0        0        0    13830 2024-05-08 08:02:07.273414 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py
--rw-r--r--   0        0        0    10297 2024-05-08 08:01:39.009190 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi
--rw-r--r--   0        0        0    17183 2024-05-08 08:02:07.277414 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py
--rw-r--r--   0        0        0     1873 2024-05-08 08:02:07.265414 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py
--rw-r--r--   0        0        0     1550 2024-05-08 08:01:38.409186 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.269415 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2_grpc.py
--rw-r--r--   0        0        0     8996 2024-05-08 08:02:07.277414 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/filters_pb2.py
--rw-r--r--   0        0        0    11380 2024-05-08 08:01:39.305192 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.281415 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/filters_pb2_grpc.py
--rw-r--r--   0        0        0     4533 2024-05-08 08:02:07.285415 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_pb2.py
--rw-r--r--   0        0        0     6103 2024-05-08 08:01:39.597194 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.285415 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_pb2_grpc.py
--rw-r--r--   0        0        0     9738 2024-05-08 08:02:07.289415 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py
--rw-r--r--   0        0        0    10977 2024-05-08 08:01:39.897196 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi
--rw-r--r--   0        0        0    10157 2024-05-08 08:02:07.289415 qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py
--rw-r--r--   0        0        0    10852 2024-05-08 08:02:07.601417 qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_pb2.py
--rw-r--r--   0        0        0    17043 2024-05-08 08:02:06.005404 qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 08:02:07.601417 qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_pb2_grpc.py
--rw-r--r--   0        0        0    21429 2024-05-08 08:02:07.605417 qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_service_pb2.py
--rw-r--r--   0        0        0    13726 2024-05-08 08:02:06.305406 qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi
--rw-r--r--   0        0        0    27193 2024-05-08 08:02:07.605417 qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py
--rw-r--r--   0        0        0     3696 2024-05-08 08:02:14.745471 qwak_core-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      585 2024-05-08 08:02:14.749472 qwak_core-0.4.5/qwak/__init__.py
--rw-r--r--   0        0        0     1522 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3228 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12456 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/automations/automations.py
--rw-r--r--   0        0        0    12907 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    26800 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     2404 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/_inner/__init__.py
--rw-r--r--   0        0        0      849 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/_inner/edge_communications.py
--rw-r--r--   0        0        0      224 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5340 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       43 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/alerts_registry/__init__.py
--rw-r--r--   0        0        0     4040 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/alerts_registry/channel.py
--rw-r--r--   0        0        0     5355 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/alerts_registry/client.py
--rw-r--r--   0        0        0       42 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     9034 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    21054 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6882 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4209 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0      105 2024-05-08 07:57:46.503539 qwak_core-0.4.5/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0     5045 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/build_orchestrator/build_model_request_getter.py
--rw-r--r--   0        0        0    16148 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0     3981 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/build_orchestrator/internal_client.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     2401 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0      885 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/data_versioning/data_tag_filter.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6806 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     4051 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/feature_store/execution_management_client.py
--rw-r--r--   0        0        0     2635 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    16056 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     8022 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/feature_store/offline_serving_client.py
--rw-r--r--   0        0        0     5811 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     2505 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0      885 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/file_versioning/file_tag_filter.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2509 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9308 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     4431 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3581 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      102 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/vector_store/__init__.py
--rw-r--r--   0        0        0     4247 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/vector_store/management_client.py
--rw-r--r--   0        0        0     5293 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/vector_store/serving_client.py
--rw-r--r--   0        0        0       43 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/workspace_manager/__init__.py
--rw-r--r--   0        0        0     8136 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/clients/workspace_manager/client.py
--rw-r--r--   0        0        0      790 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      192 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      424 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_general_build_exception.py
--rw-r--r--   0        0        0      579 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0       54 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_load_configuration_exception.py
--rw-r--r--   0        0        0      274 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      137 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_remote_build_failed.py
--rw-r--r--   0        0        0      746 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/exceptions/qwak_suggestion_exception.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     1977 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/_common/artifact_utils.py
--rw-r--r--   0        0        0     7046 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/_common/feature_set_utils.py
--rw-r--r--   0        0        0     4707 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     6680 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/_common/packaging.py
--rw-r--r--   0        0        0     2316 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0     2694 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/base.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/__init__.py
--rw-r--r--   0        0        0      197 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/_batch.py
--rw-r--r--   0        0        0      658 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/_jdbc.py
--rw-r--r--   0        0        0    10805 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/athena.py
--rw-r--r--   0        0        0     3022 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/big_query.py
--rw-r--r--   0        0        0     2063 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/clickhouse.py
--rw-r--r--   0        0        0     1981 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/csv.py
--rw-r--r--   0        0        0     2130 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/elastic_search.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/filesystem/__init__.py
--rw-r--r--   0        0        0     2828 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/filesystem/aws.py
--rw-r--r--   0        0        0      245 2024-05-08 07:57:46.507539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/filesystem/base_config.py
--rw-r--r--   0        0        0     1572 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/filesystem/gcp.py
--rw-r--r--   0        0        0     1874 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/filesystem/utils.py
--rw-r--r--   0        0        0     1921 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/mongodb.py
--rw-r--r--   0        0        0     1595 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/mysql.py
--rw-r--r--   0        0        0     1867 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/parquet.py
--rw-r--r--   0        0        0     1648 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/postgres.py
--rw-r--r--   0        0        0     3114 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/redshift.py
--rw-r--r--   0        0        0     2579 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/snowflake.py
--rw-r--r--   0        0        0     1830 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/batch/vertica.py
--rw-r--r--   0        0        0      895 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/source_authentication.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/__init__.py
--rw-r--r--   0        0        0      181 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/_streaming.py
--rw-r--r--   0        0        0      649 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/kafka/__init__.py
--rw-r--r--   0        0        0     3959 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/kafka/authentication.py
--rw-r--r--   0        0        0     3510 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/kafka/deserialization.py
--rw-r--r--   0        0        0     4398 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/kafka/kafka.py
--rw-r--r--   0        0        0     5984 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/data_sources/time_partition_columns.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     2313 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/execution/__init__.py
--rw-r--r--   0        0        0     6470 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/execution/backfill.py
--rw-r--r--   0        0        0    21243 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/execution/execution.py
--rw-r--r--   0        0        0     3564 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/execution/execution_query.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1636 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/_utils/_featureset_utils.py
--rw-r--r--   0        0        0     1979 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0     5285 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/base_feature_set.py
--rw-r--r--   0        0        0    16910 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1670 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0     1155 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0    23233 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/streaming.py
--rw-r--r--   0        0        0     9584 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/streaming_backfill.py
--rw-r--r--   0        0        0      733 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/aggregations/__init__.py
--rw-r--r--   0        0        0    14117 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py
--rw-r--r--   0        0        0     2253 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/aggregations/windows.py
--rw-r--r--   0        0        0      281 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/functions/__init__.py
--rw-r--r--   0        0        0     2425 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py
--rw-r--r--   0        0        0     1156 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/functions/schema.py
--rw-r--r--   0        0        0     9659 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/transformations.py
--rw-r--r--   0        0        0      173 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0     1216 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/offline/_offline_serving_validations.py
--rw-r--r--   0        0        0      738 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28651 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0    12597 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/offline/client_v2.py
--rw-r--r--   0        0        0      739 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/offline/feature_set_features.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0    11144 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0     2210 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/online/endpoint_utils.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/validations/__init__.py
--rw-r--r--   0        0        0     2656 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/validations/validation_options.py
--rw-r--r--   0        0        0     3783 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/validations/validation_response.py
--rw-r--r--   0        0        0     3864 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/feature_store/validations/validator.py
--rw-r--r--   0        0        0      226 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/inner/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/inner/build_config/__init__.py
--rw-r--r--   0        0        0    10978 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/inner/build_config/build_config_v1.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/inner/build_logic/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/inner/build_logic/build_loggers/__init__.py
--rw-r--r--   0        0        0     1426 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/inner/build_logic/build_loggers/trigger_build_logger.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/inner/build_logic/constants/__init__.py
--rw-r--r--   0        0        0      209 2024-05-08 07:57:46.511539 qwak_core-0.4.5/qwak/inner/build_logic/constants/dependencies.py
--rw-r--r--   0        0        0      131 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/constants/host_resource.py
--rw-r--r--   0        0        0       94 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/constants/messages.py
--rw-r--r--   0        0        0       36 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/constants/temp_dir.py
--rw-r--r--   0        0        0      279 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/constants/upload_tag.py
--rw-r--r--   0        0        0      116 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/dependency_manager_type.py
--rw-r--r--   0        0        0     2299 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/execute_build_pipeline.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/interface/__init__.py
--rw-r--r--   0        0        0      528 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/interface/build_logger_interface.py
--rw-r--r--   0        0        0      675 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/interface/build_phase.py
--rw-r--r--   0        0        0     2247 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/interface/context_interface.py
--rw-r--r--   0        0        0     1723 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/interface/phase_run_handler.py
--rw-r--r--   0        0        0      718 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/interface/step_inteface.py
--rw-r--r--   0        0        0      585 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/interface/time_source.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/__init__.py
--rw-r--r--   0        0        0     1895 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/__init__.py
--rw-r--r--   0        0        0      953 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py
--rw-r--r--   0        0        0     2067 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/__init__.py
--rw-r--r--   0        0        0     5057 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/__init__.py
--rw-r--r--   0        0        0     5944 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py
--rw-r--r--   0        0        0     1424 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/__init__.py
--rw-r--r--   0        0        0     2258 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py
--rw-r--r--   0        0        0     5399 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py
--rw-r--r--   0        0        0    10894 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py
--rw-r--r--   0        0        0     1186 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/__init__.py
--rw-r--r--   0        0        0      618 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py
--rw-r--r--   0        0        0     1599 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py
--rw-r--r--   0        0        0     9553 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py
--rw-r--r--   0        0        0     1244 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/phases/phases_pipeline.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/run_handlers/__init__.py
--rw-r--r--   0        0        0     3484 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/tools/__init__.py
--rw-r--r--   0        0        0     2498 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/tools/dependencies_tools.py
--rw-r--r--   0        0        0     8228 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/tools/files.py
--rw-r--r--   0        0        0      750 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/tools/ignore_files.py
--rw-r--r--   0        0        0      188 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/tools/text.py
--rw-r--r--   0        0        0      200 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/build_logic/trigger_build_context.py
--rw-r--r--   0        0        0     1084 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/const.py
--rw-r--r--   0        0        0     1595 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0      242 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0     1136 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      414 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/instance_template/__init__.py
--rw-r--r--   0        0        0     1916 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/instance_template/verify_template_id.py
--rw-r--r--   0        0        0     2933 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0       70 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/provider.py
--rw-r--r--   0        0        0      281 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      545 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3830 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      361 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     6897 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      422 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0     1686 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/protobuf_factory.py
--rw-r--r--   0        0        0      435 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     4200 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6976 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/__init__.py
--rw-r--r--   0        0        0     4762 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/_entity_extraction.py
--rw-r--r--   0        0        0     1739 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      322 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      321 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2024-05-08 07:57:46.515539 qwak_core-0.4.5/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/base.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1938 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/decorators/api.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/decorators/impl/__init__.py
--rw-r--r--   0        0        0      993 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/decorators/impl/api_implementation.py
--rw-r--r--   0        0        0      215 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/decorators/impl/timer_implementation.py
--rw-r--r--   0        0        0      739 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/decorators/timer.py
--rw-r--r--   0        0        0     1503 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0     1981 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/schema.py
--rw-r--r--   0        0        0     2411 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      786 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     2176 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0     1560 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2712 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      798 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0     2289 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2938 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5472 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0     1757 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/batch_jobs/execution.py
--rw-r--r--   0        0        0     1531 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/batch_jobs/task.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/build_api_helpers/__init__.py
--rw-r--r--   0        0        0     1886 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/build_api_helpers/build_api_steps.py
--rw-r--r--   0        0        0      184 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/build_api_helpers/messages.py
--rw-r--r--   0        0        0     2355 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/build_api_helpers/trigger_build_api.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    26693 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/data_versioning/__init__.py
--rw-r--r--   0        0        0      806 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/data_versioning/data_tag.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13288 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/file_versioning/__init__.py
--rw-r--r--   0        0        0      806 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/file_versioning/file_tag.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0     1191 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/utils/__init__.py
--rw-r--r--   0        0        0      581 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/utils/datetime_utils.py
--rw-r--r--   0        0        0      120 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/vector_store/__init__.py
--rw-r--r--   0        0        0     6040 2024-05-08 07:57:46.519539 qwak_core-0.4.5/qwak/vector_store/client.py
--rw-r--r--   0        0        0    16916 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak/vector_store/collection.py
--rw-r--r--   0        0        0     8209 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak/vector_store/filters.py
--rw-r--r--   0        0        0     3711 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak/vector_store/inference_client.py
--rw-r--r--   0        0        0     2658 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak/vector_store/rest_helpers.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak/vector_store/utils/__init__.py
--rw-r--r--   0        0        0      837 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak/vector_store/utils/filter_utils.py
--rw-r--r--   0        0        0     7459 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak/vector_store/utils/upsert_utils.py
--rw-r--r--   0        0        0       46 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2263 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/alert_registry_service_api.py
--rw-r--r--   0        0        0     2129 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1189 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    13129 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3686 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     4984 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     1264 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py
--rw-r--r--   0        0        0     5226 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     2453 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    20753 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1608 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0      886 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/execution_management_service.py
--rw-r--r--   0        0        0     3207 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     3400 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3712 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     6800 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     2592 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     1635 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/fs_offline_serving_service.py
--rw-r--r--   0        0        0     4567 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     1046 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/internal_build_orchestrator_service.py
--rw-r--r--   0        0        0     2696 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     4153 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     5500 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0     5722 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/vector_serving_api.py
--rw-r--r--   0        0        0     3594 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/vectors_management_api.py
--rw-r--r--   0        0        0     7591 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/mocks/workspace_manager_service_mock.py
--rw-r--r--   0        0        0    17551 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2024-05-08 07:57:46.523539 qwak_core-0.4.5/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 qwak_core-0.4.5/setup.py
--rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 qwak_core-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      264 2024-05-08 08:49:55.343554 qwak_core-0.4.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 08:52:35.502785 qwak_core-0.4.6/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5877 2024-05-08 08:52:35.534784 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     7824 2024-05-08 08:52:05.615685 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.534784 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0    12703 2024-05-08 08:52:35.534784 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py
+-rw-r--r--   0        0        0    10914 2024-05-08 08:52:05.827679 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi
+-rw-r--r--   0        0        0    14681 2024-05-08 08:52:35.534784 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2024-05-08 08:52:35.526784 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2024-05-08 08:52:05.199697 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.530784 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2024-05-08 08:52:35.530784 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2024-05-08 08:52:05.407691 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.530784 qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2024-05-08 08:52:35.518784 qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2024-05-08 08:52:04.563717 qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2024-05-08 08:52:35.522784 qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2024-05-08 08:52:35.522784 qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2024-05-08 08:52:04.767710 qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.522784 qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2024-05-08 08:52:35.526784 qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2024-05-08 08:52:04.967704 qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.526784 qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2024-05-08 08:52:35.506785 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2024-05-08 08:52:04.355723 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2024-05-08 08:52:35.506785 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7360 2024-05-08 08:52:35.506785 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0    11651 2024-05-08 08:52:06.043672 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.510784 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     5029 2024-05-08 08:52:35.510784 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     6943 2024-05-08 08:52:06.487659 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.514784 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2024-05-08 08:52:35.514784 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2024-05-08 08:52:06.711652 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2024-05-08 08:52:35.514784 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2024-05-08 08:52:35.510784 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2024-05-08 08:52:06.259665 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.510784 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6541 2024-05-08 08:52:35.518784 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10595 2024-05-08 08:52:06.943645 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.518784 qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0    15382 2024-05-08 08:52:35.570783 qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    20668 2024-05-08 08:52:09.999553 qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.570783 qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2024-05-08 08:52:35.570783 qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2024-05-08 08:52:10.211547 qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2024-05-08 08:52:35.574782 qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7616 2024-05-08 08:52:35.694779 qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11995 2024-05-08 08:52:20.323240 qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.694779 qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0    14893 2024-05-08 08:52:35.694779 qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0    11812 2024-05-08 08:52:20.535234 qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    19155 2024-05-08 08:52:35.698779 qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2024-05-08 08:52:35.698779 qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2024-05-08 08:52:21.775196 qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2024-05-08 08:52:35.702779 qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8864 2024-05-08 08:52:35.698779 qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13789 2024-05-08 08:52:21.571202 qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.698779 qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2024-05-08 08:52:35.702779 qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2024-05-08 08:52:21.983189 qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.702779 qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2024-05-08 08:52:35.706779 qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2024-05-08 08:52:22.183183 qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2024-05-08 08:52:35.706779 qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    14053 2024-05-08 08:52:35.814775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    20860 2024-05-08 08:52:31.806894 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.818775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2024-05-08 08:52:35.810776 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2024-05-08 08:52:31.390907 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.810776 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3954 2024-05-08 08:52:35.814775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     5309 2024-05-08 08:52:31.594901 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.814775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    21176 2024-05-08 08:52:35.806776 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    15049 2024-05-08 08:52:30.978919 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    25475 2024-05-08 08:52:35.806776 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2024-05-08 08:52:35.806776 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2024-05-08 08:52:31.186913 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.810776 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2024-05-08 08:52:35.822775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2024-05-08 08:52:32.414876 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.822775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2024-05-08 08:52:35.818775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2024-05-08 08:52:32.210883 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.822775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2024-05-08 08:52:35.818775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2024-05-08 08:52:32.010888 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.818775 qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    11218 2024-05-08 08:52:35.802776 qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    15584 2024-05-08 08:52:30.754926 qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.806776 qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2083 2024-05-08 08:52:35.798776 qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1977 2024-05-08 08:52:30.330938 qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.798776 qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    46028 2024-05-08 08:52:35.802776 qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    60013 2024-05-08 08:52:30.550932 qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    32008 2024-05-08 08:52:35.802776 qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    29124 2024-05-08 08:52:35.738778 qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    24434 2024-05-08 08:52:24.327118 qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    27837 2024-05-08 08:52:35.738778 qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    33279 2024-05-08 08:52:35.734778 qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    52325 2024-05-08 08:52:23.907131 qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.734778 qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0     5757 2024-05-08 08:52:35.742777 qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py
+-rw-r--r--   0        0        0     4013 2024-05-08 08:52:25.007097 qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi
+-rw-r--r--   0        0        0     6783 2024-05-08 08:52:35.742777 qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py
+-rw-r--r--   0        0        0     6016 2024-05-08 08:52:35.738778 qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_pb2.py
+-rw-r--r--   0        0        0     7049 2024-05-08 08:52:24.795103 qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.742777 qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_pb2_grpc.py
+-rw-r--r--   0        0        0    14991 2024-05-08 08:52:35.722778 qwak_core-0.4.6/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    24472 2024-05-08 08:52:23.683137 qwak_core-0.4.6/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.722778 qwak_core-0.4.6/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     5552 2024-05-08 08:52:35.726778 qwak_core-0.4.6/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     7299 2024-05-08 08:52:24.111124 qwak_core-0.4.6/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.726778 qwak_core-0.4.6/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    15672 2024-05-08 08:52:35.726778 qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0    12741 2024-05-08 08:52:24.567110 qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    16925 2024-05-08 08:52:35.726778 qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38491 2024-05-08 08:52:35.730778 qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    53557 2024-05-08 08:52:25.719075 qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2024-05-08 08:52:35.734778 qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     3508 2024-05-08 08:52:35.730778 qwak_core-0.4.6/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     2300 2024-05-08 08:52:25.223090 qwak_core-0.4.6/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0     3101 2024-05-08 08:52:35.730778 qwak_core-0.4.6/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2270 2024-05-08 08:52:35.750777 qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     2697 2024-05-08 08:52:26.191061 qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.750777 qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4458 2024-05-08 08:52:35.750777 qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     3113 2024-05-08 08:52:26.399055 qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2024-05-08 08:52:35.754777 qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2024-05-08 08:52:35.714778 qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2024-05-08 08:52:23.063156 qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.714778 qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11871 2024-05-08 08:52:35.718778 qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     8790 2024-05-08 08:52:23.271150 qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2024-05-08 08:52:35.718778 qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2024-05-08 08:52:35.710779 qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2024-05-08 08:52:22.623170 qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.710779 qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    50041 2024-05-08 08:52:35.706779 qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    74372 2024-05-08 08:52:22.407176 qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.710779 qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    46309 2024-05-08 08:52:35.714778 qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    40356 2024-05-08 08:52:22.851163 qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    27756 2024-05-08 08:52:35.714778 qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3345 2024-05-08 08:52:35.558783 qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     4098 2024-05-08 08:52:08.915586 qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.558783 qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12707 2024-05-08 08:52:35.558783 qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    13800 2024-05-08 08:52:09.135579 qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.562783 qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    17949 2024-05-08 08:52:35.562783 qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    18562 2024-05-08 08:52:09.355573 qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    12833 2024-05-08 08:52:35.562783 qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6463 2024-05-08 08:52:35.650780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/backfill_pb2.py
+-rw-r--r--   0        0        0     7945 2024-05-08 08:52:15.559385 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.650780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/backfill_pb2_grpc.py
+-rw-r--r--   0        0        0     2971 2024-05-08 08:52:35.650780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/batch_pb2.py
+-rw-r--r--   0        0        0     3266 2024-05-08 08:52:15.763379 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.654780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     2210 2024-05-08 08:52:35.654780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/deletion_pb2.py
+-rw-r--r--   0        0        0     1540 2024-05-08 08:52:15.967373 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.654780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/deletion_pb2_grpc.py
+-rw-r--r--   0        0        0     5793 2024-05-08 08:52:35.658780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_pb2.py
+-rw-r--r--   0        0        0     7373 2024-05-08 08:52:16.175367 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.658780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    14900 2024-05-08 08:52:35.658780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_service_pb2.py
+-rw-r--r--   0        0        0    11103 2024-05-08 08:52:16.387360 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi
+-rw-r--r--   0        0        0    17220 2024-05-08 08:52:35.662780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7695 2024-05-08 08:52:35.662780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py
+-rw-r--r--   0        0        0    14959 2024-05-08 08:52:16.811347 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.666780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0    19304 2024-05-08 08:52:35.666780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0    16916 2024-05-08 08:52:17.031340 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    21145 2024-05-08 08:52:35.666780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8440 2024-05-08 08:52:35.662780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py
+-rw-r--r--   0        0        0    13312 2024-05-08 08:52:16.599354 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.662780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     2051 2024-05-08 08:52:35.670780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py
+-rw-r--r--   0        0        0     1952 2024-05-08 08:52:17.235334 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.670780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_pb2_grpc.py
+-rw-r--r--   0        0        0    12222 2024-05-08 08:52:35.670780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py
+-rw-r--r--   0        0        0     7930 2024-05-08 08:52:17.443328 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi
+-rw-r--r--   0        0        0    14212 2024-05-08 08:52:35.674780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1685 2024-05-08 08:52:35.674780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py
+-rw-r--r--   0        0        0     1272 2024-05-08 08:52:17.643322 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.674780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2_grpc.py
+-rw-r--r--   0        0        0     6198 2024-05-08 08:52:35.674780 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py
+-rw-r--r--   0        0        0     7677 2024-05-08 08:52:17.847316 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.678779 qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2024-05-08 08:52:35.626781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2024-05-08 08:52:15.351392 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.626781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2024-05-08 08:52:35.622781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2024-05-08 08:52:15.151398 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2024-05-08 08:52:35.622781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2024-05-08 08:52:35.594782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2024-05-08 08:52:12.843468 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.598782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0    13825 2024-05-08 08:52:35.606782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_pb2.py
+-rw-r--r--   0        0        0    19227 2024-05-08 08:52:13.903436 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.610782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3307 2024-05-08 08:52:35.610782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py
+-rw-r--r--   0        0        0     1637 2024-05-08 08:52:14.111430 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3293 2024-05-08 08:52:35.610782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2024-05-08 08:52:35.594782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2024-05-08 08:52:12.635474 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.594782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2024-05-08 08:52:35.586782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2024-05-08 08:52:11.987493 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.586782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2024-05-08 08:52:35.590782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2024-05-08 08:52:12.427480 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2024-05-08 08:52:35.590782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2024-05-08 08:52:35.598782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2024-05-08 08:52:13.051462 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.598782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2024-05-08 08:52:35.602782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2024-05-08 08:52:13.275455 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2024-05-08 08:52:35.602782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    26853 2024-05-08 08:52:35.586782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    39247 2024-05-08 08:52:12.207487 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.590782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2024-05-08 08:52:35.602782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2024-05-08 08:52:13.479449 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.606782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    13240 2024-05-08 08:52:35.606782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    18420 2024-05-08 08:52:13.695443 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.606782 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2024-05-08 08:52:35.626781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2024-05-08 08:52:34.498814 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.630781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2024-05-08 08:52:35.630781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2024-05-08 08:52:34.702808 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2024-05-08 08:52:35.630781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4308 2024-05-08 08:52:35.634781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     7410 2024-05-08 08:52:19.703259 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.634781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    15316 2024-05-08 08:52:35.634781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    14087 2024-05-08 08:52:19.911253 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    18465 2024-05-08 08:52:35.634781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2024-05-08 08:52:35.638781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2024-05-08 08:52:20.115246 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.638781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     5111 2024-05-08 08:52:35.646780 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/management_pb2.py
+-rw-r--r--   0        0        0     2739 2024-05-08 08:52:21.363208 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi
+-rw-r--r--   0        0        0     5436 2024-05-08 08:52:35.650780 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py
+-rw-r--r--   0        0        0     5385 2024-05-08 08:52:35.642781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     7551 2024-05-08 08:52:20.951221 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.642781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    17474 2024-05-08 08:52:35.638781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2024-05-08 08:52:20.739227 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2024-05-08 08:52:35.642781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2024-05-08 08:52:35.646780 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2024-05-08 08:52:21.155215 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.646780 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    27355 2024-05-08 08:52:35.614781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    43393 2024-05-08 08:52:14.319423 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.614781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5147 2024-05-08 08:52:35.614781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6208 2024-05-08 08:52:14.527417 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.618781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2024-05-08 08:52:35.618781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2024-05-08 08:52:14.739410 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2024-05-08 08:52:35.618781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11049 2024-05-08 08:52:35.622781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15942 2024-05-08 08:52:14.943404 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.622781 qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2024-05-08 08:52:35.834775 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2024-05-08 08:52:33.230852 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.834775 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2024-05-08 08:52:35.834775 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2024-05-08 08:52:33.442846 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2024-05-08 08:52:35.834775 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2024-05-08 08:52:35.838775 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2024-05-08 08:52:33.650840 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.838775 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2024-05-08 08:52:35.838775 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2024-05-08 08:52:33.866833 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2024-05-08 08:52:35.842774 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10469 2024-05-08 08:52:35.842774 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0    11719 2024-05-08 08:52:34.086827 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     9458 2024-05-08 08:52:35.842774 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5302 2024-05-08 08:52:35.846774 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     5484 2024-05-08 08:52:34.294821 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.846774 qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2975 2024-05-08 08:52:35.754777 qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     4026 2024-05-08 08:52:26.611049 qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.754777 qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4455 2024-05-08 08:52:35.758777 qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     3113 2024-05-08 08:52:26.815043 qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2024-05-08 08:52:35.758777 qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6950 2024-05-08 08:52:35.574782 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    11560 2024-05-08 08:52:11.139519 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.574782 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     3442 2024-05-08 08:52:35.578782 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     5719 2024-05-08 08:52:11.347513 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.578782 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2024-05-08 08:52:35.578782 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2024-05-08 08:52:11.551507 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2024-05-08 08:52:35.582782 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8504 2024-05-08 08:52:35.582782 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12440 2024-05-08 08:52:11.759500 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.582782 qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2024-05-08 08:52:35.718778 qwak_core-0.4.6/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2024-05-08 08:52:23.475144 qwak_core-0.4.6/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2024-05-08 08:52:35.722778 qwak_core-0.4.6/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3876 2024-05-08 08:52:35.758777 qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4658 2024-05-08 08:52:27.023036 qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.758777 qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2024-05-08 08:52:35.762777 qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2024-05-08 08:52:27.223030 qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2024-05-08 08:52:35.762777 qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2024-05-08 08:52:35.774777 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2024-05-08 08:52:28.446994 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.778777 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2024-05-08 08:52:35.778777 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2024-05-08 08:52:28.650988 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.778777 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    25218 2024-05-08 08:52:35.782776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    31280 2024-05-08 08:52:28.858982 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.782776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13432 2024-05-08 08:52:35.782776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    22974 2024-05-08 08:52:29.066976 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.786776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12784 2024-05-08 08:52:35.786776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16585 2024-05-08 08:52:29.278969 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.786776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    51171 2024-05-08 08:52:35.790776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    40800 2024-05-08 08:52:29.506963 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    73869 2024-05-08 08:52:35.790776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-05-08 08:52:35.790776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2024-05-08 08:52:29.710957 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.790776 qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2024-05-08 08:52:35.766777 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2024-05-08 08:52:27.631018 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.766777 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2024-05-08 08:52:35.774777 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2024-05-08 08:52:28.243000 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.774777 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2024-05-08 08:52:35.770777 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2024-05-08 08:52:27.835012 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2024-05-08 08:52:35.770777 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2024-05-08 08:52:35.770777 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2024-05-08 08:52:28.043006 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.770777 qwak_core-0.4.6/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    27866 2024-05-08 08:52:35.746777 qwak_core-0.4.6/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    32184 2024-05-08 08:52:25.943069 qwak_core-0.4.6/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    19830 2024-05-08 08:52:35.746777 qwak_core-0.4.6/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2024-05-08 08:52:35.550783 qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2024-05-08 08:52:10.679533 qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2024-05-08 08:52:35.554783 qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2024-05-08 08:52:35.550783 qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2024-05-08 08:52:10.431540 qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.550783 qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2024-05-08 08:52:35.554783 qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2024-05-08 08:52:10.907526 qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2024-05-08 08:52:35.554783 qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1598 2024-05-08 08:52:35.826775 qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py
+-rw-r--r--   0        0        0     1221 2024-05-08 08:52:32.618870 qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.826775 qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2_grpc.py
+-rw-r--r--   0        0        0    11437 2024-05-08 08:52:35.830775 qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py
+-rw-r--r--   0        0        0    12170 2024-05-08 08:52:33.030858 qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi
+-rw-r--r--   0        0        0     9793 2024-05-08 08:52:35.830775 qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4060 2024-05-08 08:52:35.826775 qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/population_pb2.py
+-rw-r--r--   0        0        0     3906 2024-05-08 08:52:32.822864 qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.830775 qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/population_pb2_grpc.py
+-rw-r--r--   0        0        0    10804 2024-05-08 08:52:35.746777 qwak_core-0.4.6/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0    12120 2024-05-08 08:52:25.491082 qwak_core-0.4.6/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     9642 2024-05-08 08:52:35.746777 qwak_core-0.4.6/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2024-05-08 08:52:35.762777 qwak_core-0.4.6/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2024-05-08 08:52:27.427024 qwak_core-0.4.6/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2024-05-08 08:52:35.766777 qwak_core-0.4.6/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10718 2024-05-08 08:52:35.546783 qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0    12627 2024-05-08 08:52:08.011613 qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.550783 qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    19751 2024-05-08 08:52:35.546783 qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    13467 2024-05-08 08:52:07.807619 qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    24352 2024-05-08 08:52:35.546783 qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2024-05-08 08:52:35.538784 qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2024-05-08 08:52:07.155639 qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.538784 qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2477 2024-05-08 08:52:35.538784 qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2679 2024-05-08 08:52:07.375632 qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.542784 qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2024-05-08 08:52:35.542784 qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2024-05-08 08:52:07.583626 qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2024-05-08 08:52:35.542784 qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6909 2024-05-08 08:52:35.794776 qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     5186 2024-05-08 08:52:30.126944 qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2024-05-08 08:52:35.798776 qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7868 2024-05-08 08:52:35.794776 qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    12177 2024-05-08 08:52:29.922950 qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.794776 qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11396 2024-05-08 08:52:35.566783 qwak_core-0.4.6/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15139 2024-05-08 08:52:09.575566 qwak_core-0.4.6/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.566783 qwak_core-0.4.6/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3645 2024-05-08 08:52:35.566783 qwak_core-0.4.6/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2983 2024-05-08 08:52:09.783560 qwak_core-0.4.6/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.570783 qwak_core-0.4.6/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     8648 2024-05-08 08:52:35.682779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py
+-rw-r--r--   0        0        0    12852 2024-05-08 08:52:18.263303 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.682779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_pb2_grpc.py
+-rw-r--r--   0        0        0    13830 2024-05-08 08:52:35.682779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py
+-rw-r--r--   0        0        0    10297 2024-05-08 08:52:18.471296 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi
+-rw-r--r--   0        0        0    17183 2024-05-08 08:52:35.686779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1873 2024-05-08 08:52:35.678779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py
+-rw-r--r--   0        0        0     1550 2024-05-08 08:52:18.059309 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.678779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2_grpc.py
+-rw-r--r--   0        0        0     8996 2024-05-08 08:52:35.686779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/filters_pb2.py
+-rw-r--r--   0        0        0    11380 2024-05-08 08:52:18.675290 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.686779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/filters_pb2_grpc.py
+-rw-r--r--   0        0        0     4533 2024-05-08 08:52:35.686779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_pb2.py
+-rw-r--r--   0        0        0     6103 2024-05-08 08:52:18.879284 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.690779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_pb2_grpc.py
+-rw-r--r--   0        0        0     9738 2024-05-08 08:52:35.690779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py
+-rw-r--r--   0        0        0    10977 2024-05-08 08:52:19.091278 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi
+-rw-r--r--   0        0        0    10157 2024-05-08 08:52:35.690779 qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10852 2024-05-08 08:52:35.846774 qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_pb2.py
+-rw-r--r--   0        0        0    17043 2024-05-08 08:52:34.910802 qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 08:52:35.846774 qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0    21429 2024-05-08 08:52:35.850774 qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_service_pb2.py
+-rw-r--r--   0        0        0    13726 2024-05-08 08:52:35.122796 qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi
+-rw-r--r--   0        0        0    27193 2024-05-08 08:52:35.850774 qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3696 2024-05-08 08:52:39.050679 qwak_core-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      585 2024-05-08 08:52:39.050679 qwak_core-0.4.6/qwak/__init__.py
+-rw-r--r--   0        0        0     1522 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12456 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/automations/automations.py
+-rw-r--r--   0        0        0    12907 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    26800 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     2404 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/_inner/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/_inner/edge_communications.py
+-rw-r--r--   0        0        0      224 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5340 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       43 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/alerts_registry/__init__.py
+-rw-r--r--   0        0        0     4040 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/alerts_registry/channel.py
+-rw-r--r--   0        0        0     5355 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/alerts_registry/client.py
+-rw-r--r--   0        0        0       42 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     9034 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    21054 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6882 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4209 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0      105 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0     5045 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/build_orchestrator/build_model_request_getter.py
+-rw-r--r--   0        0        0    16148 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0     3981 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/build_orchestrator/internal_client.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     2401 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0      885 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/data_versioning/data_tag_filter.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6806 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     4051 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/feature_store/execution_management_client.py
+-rw-r--r--   0        0        0     2635 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    16056 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     8022 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/feature_store/offline_serving_client.py
+-rw-r--r--   0        0        0     5811 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     2505 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0      885 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/file_versioning/file_tag_filter.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2509 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9308 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2024-05-08 08:49:55.347554 qwak_core-0.4.6/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     4431 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3581 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      102 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/vector_store/__init__.py
+-rw-r--r--   0        0        0     4247 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/vector_store/management_client.py
+-rw-r--r--   0        0        0     5293 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/vector_store/serving_client.py
+-rw-r--r--   0        0        0       43 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/workspace_manager/__init__.py
+-rw-r--r--   0        0        0     8136 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/clients/workspace_manager/client.py
+-rw-r--r--   0        0        0      790 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      192 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      424 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_general_build_exception.py
+-rw-r--r--   0        0        0      579 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0       54 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_load_configuration_exception.py
+-rw-r--r--   0        0        0      274 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      137 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_remote_build_failed.py
+-rw-r--r--   0        0        0      746 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/exceptions/qwak_suggestion_exception.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     1977 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/_common/artifact_utils.py
+-rw-r--r--   0        0        0     7046 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/_common/feature_set_utils.py
+-rw-r--r--   0        0        0     4707 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     6680 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/_common/packaging.py
+-rw-r--r--   0        0        0     2316 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0     2694 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/base.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/_batch.py
+-rw-r--r--   0        0        0      658 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/_jdbc.py
+-rw-r--r--   0        0        0    10805 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/athena.py
+-rw-r--r--   0        0        0     3022 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/big_query.py
+-rw-r--r--   0        0        0     2063 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/clickhouse.py
+-rw-r--r--   0        0        0     1981 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/csv.py
+-rw-r--r--   0        0        0     2130 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/elastic_search.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/filesystem/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/filesystem/aws.py
+-rw-r--r--   0        0        0      245 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/filesystem/base_config.py
+-rw-r--r--   0        0        0     1572 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/filesystem/gcp.py
+-rw-r--r--   0        0        0     1874 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/filesystem/utils.py
+-rw-r--r--   0        0        0     1921 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/mongodb.py
+-rw-r--r--   0        0        0     1595 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/mysql.py
+-rw-r--r--   0        0        0     1867 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/parquet.py
+-rw-r--r--   0        0        0     1648 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/postgres.py
+-rw-r--r--   0        0        0     3114 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/redshift.py
+-rw-r--r--   0        0        0     2579 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/snowflake.py
+-rw-r--r--   0        0        0     1830 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/batch/vertica.py
+-rw-r--r--   0        0        0      895 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/source_authentication.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/__init__.py
+-rw-r--r--   0        0        0      181 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/_streaming.py
+-rw-r--r--   0        0        0      649 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/kafka/__init__.py
+-rw-r--r--   0        0        0     3959 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/kafka/authentication.py
+-rw-r--r--   0        0        0     3510 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/kafka/deserialization.py
+-rw-r--r--   0        0        0     4398 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/kafka/kafka.py
+-rw-r--r--   0        0        0     5984 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/data_sources/time_partition_columns.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     2313 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/execution/__init__.py
+-rw-r--r--   0        0        0     6470 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/execution/backfill.py
+-rw-r--r--   0        0        0    21243 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/execution/execution.py
+-rw-r--r--   0        0        0     3564 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/execution/execution_query.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1636 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/_utils/_featureset_utils.py
+-rw-r--r--   0        0        0     1979 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0     5285 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/base_feature_set.py
+-rw-r--r--   0        0        0    16910 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1670 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0     1155 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0    23233 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/streaming.py
+-rw-r--r--   0        0        0     9584 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/streaming_backfill.py
+-rw-r--r--   0        0        0      733 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/aggregations/__init__.py
+-rw-r--r--   0        0        0    14117 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py
+-rw-r--r--   0        0        0     2253 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/aggregations/windows.py
+-rw-r--r--   0        0        0      281 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/functions/__init__.py
+-rw-r--r--   0        0        0     2425 2024-05-08 08:49:55.351554 qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py
+-rw-r--r--   0        0        0     1156 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/functions/schema.py
+-rw-r--r--   0        0        0     9659 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/transformations.py
+-rw-r--r--   0        0        0      173 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0     1216 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/offline/_offline_serving_validations.py
+-rw-r--r--   0        0        0      738 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28651 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0    12597 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/offline/client_v2.py
+-rw-r--r--   0        0        0      739 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/offline/feature_set_features.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0    11144 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0     2210 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/online/endpoint_utils.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/validations/__init__.py
+-rw-r--r--   0        0        0     2656 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/validations/validation_options.py
+-rw-r--r--   0        0        0     3783 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/validations/validation_response.py
+-rw-r--r--   0        0        0     3864 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/feature_store/validations/validator.py
+-rw-r--r--   0        0        0      226 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_config/__init__.py
+-rw-r--r--   0        0        0    10978 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_config/build_config_v1.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/build_loggers/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/build_loggers/trigger_build_logger.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/constants/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/constants/dependencies.py
+-rw-r--r--   0        0        0      131 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/constants/host_resource.py
+-rw-r--r--   0        0        0       94 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/constants/messages.py
+-rw-r--r--   0        0        0       36 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/constants/temp_dir.py
+-rw-r--r--   0        0        0      279 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/constants/upload_tag.py
+-rw-r--r--   0        0        0      116 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/dependency_manager_type.py
+-rw-r--r--   0        0        0     2299 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/execute_build_pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/interface/__init__.py
+-rw-r--r--   0        0        0      528 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/interface/build_logger_interface.py
+-rw-r--r--   0        0        0      675 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/interface/build_phase.py
+-rw-r--r--   0        0        0     2247 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/interface/context_interface.py
+-rw-r--r--   0        0        0     1723 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/interface/phase_run_handler.py
+-rw-r--r--   0        0        0      718 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/interface/step_inteface.py
+-rw-r--r--   0        0        0      585 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/interface/time_source.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/__init__.py
+-rw-r--r--   0        0        0     1895 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py
+-rw-r--r--   0        0        0     2067 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/__init__.py
+-rw-r--r--   0        0        0     5057 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/__init__.py
+-rw-r--r--   0        0        0     5944 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py
+-rw-r--r--   0        0        0     1424 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/__init__.py
+-rw-r--r--   0        0        0     2258 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py
+-rw-r--r--   0        0        0     5399 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py
+-rw-r--r--   0        0        0    10894 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py
+-rw-r--r--   0        0        0     1186 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/__init__.py
+-rw-r--r--   0        0        0      618 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py
+-rw-r--r--   0        0        0     1599 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py
+-rw-r--r--   0        0        0     9553 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py
+-rw-r--r--   0        0        0     1244 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/phases/phases_pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/run_handlers/__init__.py
+-rw-r--r--   0        0        0     3484 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/tools/__init__.py
+-rw-r--r--   0        0        0     2498 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/tools/dependencies_tools.py
+-rw-r--r--   0        0        0     8228 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/tools/files.py
+-rw-r--r--   0        0        0      750 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/tools/ignore_files.py
+-rw-r--r--   0        0        0      188 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/tools/text.py
+-rw-r--r--   0        0        0      200 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/build_logic/trigger_build_context.py
+-rw-r--r--   0        0        0     1084 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/const.py
+-rw-r--r--   0        0        0     1595 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0      242 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0     1136 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      414 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/instance_template/__init__.py
+-rw-r--r--   0        0        0     1916 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/instance_template/verify_template_id.py
+-rw-r--r--   0        0        0     2933 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0       70 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/provider.py
+-rw-r--r--   0        0        0      281 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      545 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3830 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     6897 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      422 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0     1686 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/protobuf_factory.py
+-rw-r--r--   0        0        0      435 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     4200 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6976 2024-05-08 08:49:55.355553 qwak_core-0.4.6/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/__init__.py
+-rw-r--r--   0        0        0     4762 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/_entity_extraction.py
+-rw-r--r--   0        0        0     1739 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      322 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      321 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1938 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/decorators/impl/__init__.py
+-rw-r--r--   0        0        0      993 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/decorators/impl/api_implementation.py
+-rw-r--r--   0        0        0      215 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/decorators/impl/timer_implementation.py
+-rw-r--r--   0        0        0      739 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/decorators/timer.py
+-rw-r--r--   0        0        0     1503 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0     1981 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/schema.py
+-rw-r--r--   0        0        0     2411 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      786 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     2176 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0     1560 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2712 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      798 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0     2289 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2938 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5472 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0     1757 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/batch_jobs/execution.py
+-rw-r--r--   0        0        0     1531 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/batch_jobs/task.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/build_api_helpers/__init__.py
+-rw-r--r--   0        0        0     1886 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/build_api_helpers/build_api_steps.py
+-rw-r--r--   0        0        0      184 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/build_api_helpers/messages.py
+-rw-r--r--   0        0        0     2355 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/build_api_helpers/trigger_build_api.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    26693 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/data_versioning/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/data_versioning/data_tag.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13288 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/file_versioning/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/file_versioning/file_tag.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0     1191 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/utils/__init__.py
+-rw-r--r--   0        0        0      581 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/utils/datetime_utils.py
+-rw-r--r--   0        0        0      120 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/vector_store/__init__.py
+-rw-r--r--   0        0        0     6040 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/vector_store/client.py
+-rw-r--r--   0        0        0    16916 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/vector_store/collection.py
+-rw-r--r--   0        0        0     8209 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/vector_store/filters.py
+-rw-r--r--   0        0        0     3711 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/vector_store/inference_client.py
+-rw-r--r--   0        0        0     2658 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/vector_store/rest_helpers.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.359553 qwak_core-0.4.6/qwak/vector_store/utils/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak/vector_store/utils/filter_utils.py
+-rw-r--r--   0        0        0     7459 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak/vector_store/utils/upsert_utils.py
+-rw-r--r--   0        0        0       46 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2263 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/alert_registry_service_api.py
+-rw-r--r--   0        0        0     2129 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1189 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    13129 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3686 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     4984 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     1264 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py
+-rw-r--r--   0        0        0     5226 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     2453 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    20753 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1608 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0      886 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/execution_management_service.py
+-rw-r--r--   0        0        0     3207 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     3400 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3712 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     6800 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     2592 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     1635 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/fs_offline_serving_service.py
+-rw-r--r--   0        0        0     4567 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     1046 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/internal_build_orchestrator_service.py
+-rw-r--r--   0        0        0     2696 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     4153 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     5500 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0     5722 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/vector_serving_api.py
+-rw-r--r--   0        0        0     3594 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/vectors_management_api.py
+-rw-r--r--   0        0        0     7591 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/mocks/workspace_manager_service_mock.py
+-rw-r--r--   0        0        0    17551 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2024-05-08 08:49:55.363553 qwak_core-0.4.6/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 qwak_core-0.4.6/setup.py
+-rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 qwak_core-0.4.6/PKG-INFO
```

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 from _qwak_proto.qwak.fitness_service import fitness_pb2 as qwak_dot_fitness__service_dot_fitness__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17qwak/builds/build.proto\x12\x18qwak.builds.orchestrator\x1a/qwak/user_application/common/v0/resources.proto\x1a\"qwak/fitness_service/fitness.proto\"\xc8\x05\n\x0fRemoteBuildSpec\x12\x43\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32).qwak.builds.orchestrator.BuildProperties\x12\x35\n\tbuild_env\x18\x02 \x01(\x0b\x32\".qwak.builds.orchestrator.BuildEnv\x12\x43\n\rcpu_resources\x18\x03 \x01(\x0b\x32&.qwak.builds.orchestrator.CpuResourcesB\x02\x18\x01H\x00\x12\x43\n\rgpu_resources\x18\x07 \x01(\x0b\x32&.qwak.builds.orchestrator.GpuResourcesB\x02\x18\x01H\x00\x12\x62\n\x1c\x63lient_pod_compute_resources\x18\r \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResourcesH\x00\x12\x0f\n\x07verbose\x18\x04 \x01(\x05\x12\x17\n\x0f\x62uild_code_path\x18\x05 \x01(\t\x12\x14\n\x0c\x62uild_config\x18\x06 \x01(\t\x12\x15\n\rbuild_v1_flag\x18\x08 \x01(\x08\x12H\n\x13\x62uild_properties_v1\x18\t \x01(\x0b\x32+.qwak.builds.orchestrator.BuildPropertiesV1\x12\x13\n\x0b\x62uild_steps\x18\n \x03(\t\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x13\n\x0bsdk_version\x18\x0c \x01(\t\x12=\n\x0fpurchase_option\x18\x0e \x01(\x0e\x32$.qwak.fitness.service.PurchaseOption\x12\x1c\n\x14\x62uild_destined_image\x18\x0f \x01(\tB\x0b\n\tResources\"g\n\x11\x42uildPropertiesV1\x12\x18\n\x10\x62uild_config_url\x18\x01 \x01(\t\x12\x1a\n\x12qwak_sdk_wheel_url\x18\x02 \x01(\t\x12\x1c\n\x14qwak_sdk_version_url\x18\x03 \x01(\t\"\xa6\x01\n\x0f\x42uildProperties\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x39\n\tmodel_uri\x18\x05 \x01(\x0b\x32&.qwak.builds.orchestrator.ModelUriSpec\x12\x16\n\x0egpu_compatible\x18\x06 \x01(\x08\"\xb2\x01\n\x0cModelUriSpec\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x17\n\x0fgit_credentials\x18\x03 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x04 \x01(\t\x12\x11\n\tcommit_id\x18\x05 \x01(\t\x12\x10\n\x08main_dir\x18\x06 \x01(\t\x12#\n\x1b\x64\x65pendency_required_folders\x18\x07 \x03(\t\"|\n\x08\x42uildEnv\x12\x37\n\ndocker_env\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.DockerEnv\x12\x37\n\npython_env\x18\x02 \x01(\x0b\x32#.qwak.builds.orchestrator.PythonEnv\"\x8a\x01\n\tDockerEnv\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x10\n\x08\x65nv_vars\x18\x02 \x03(\t\x12\x10\n\x08no_cache\x18\x03 \x01(\x08\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x04 \x01(\t\x12\'\n\x1fservice_account_key_secret_name\x18\x05 \x01(\t\"|\n\tPythonEnv\x12\x17\n\x0fgit_credentials\x18\x01 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x02 \x01(\t\x12\x18\n\x10qwak_sdk_version\x18\x03 \x01(\t\x12\x1c\n\x14qwak_sdk_extra_index\x18\x04 \x01(\t\"n\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12:\n\x0cmemory_units\x18\x03 \x01(\x0e\x32$.qwak.builds.orchestrator.MemoryUnit\"W\n\x0cGpuResources\x12\x33\n\x08gpu_type\x18\x01 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x91\x01\n\x13\x44\x61taTableDefinition\x12?\n\x07\x63olumns\x18\x01 \x03(\x0b\x32..qwak.builds.orchestrator.DataColumnDefinition\x12\x39\n\x0b\x64\x61ta_format\x18\x02 \x01(\x0b\x32$.qwak.builds.orchestrator.DataFormat\"\\\n\x14\x44\x61taColumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x04type\x18\x02 \x01(\x0e\x32(.qwak.builds.orchestrator.DataColumnType\"J\n\nDataFormat\x12\x32\n\x03\x63sv\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.CsvFormatH\x00\x42\x08\n\x06\x66ormat\"G\n\tCsvFormat\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\x12\n\nquote_char\x18\x02 \x01(\t\x12\x13\n\x0b\x65scape_char\x18\x03 \x01(\t\"\xa5\x01\n\x0e\x42uildInitiator\x12<\n\x04user\x18\x01 \x01(\x0b\x32,.qwak.builds.orchestrator.UserBuildInitiatorH\x00\x12H\n\nautomation\x18\x02 \x01(\x0b\x32\x32.qwak.builds.orchestrator.AutomationBuildInitiatorH\x00\x42\x0b\n\tInitiator\"\x14\n\x12UserBuildInitiator\"`\n\x18\x41utomationBuildInitiator\x12\x15\n\rautomation_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x17\n\x0f\x61utomation_name\x18\x03 \x01(\t*7\n\nMemoryUnit\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x8c\x02\n\x07GpuType\x12\x0b\n\x07INVALID\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06\x12\x14\n\x10NVIDIA_T4_1_4_15\x10\x07\x12\x14\n\x10NVIDIA_T4_1_8_30\x10\x08\x12\x15\n\x11NVIDIA_T4_1_16_60\x10\t\x12\x1e\n\x1aNVIDIA_A100_80GB_8_96_1360\x10\n\x12\x16\n\x12NVIDIA_V100_1_8_52\x10\x0b\x12\x18\n\x14NVIDIA_V100_4_32_208\x10\x0c*d\n\x0e\x44\x61taColumnType\x12\x17\n\x13INVALID_COLUMN_TYPE\x10\x00\x12\n\n\x06OBJECT\x10\x01\x12\x07\n\x03INT\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07\x42OOLEAN\x10\x04\x12\x0c\n\x08\x44\x41TETIME\x10\x05*K\n\x13\x42\x61seDockerImageType\x12\"\n\x1eUNKNOWN_BASE_DOCKER_IMAGE_TYPE\x10\x00\x12\x07\n\x03\x43PU\x10\x01\x12\x07\n\x03GPU\x10\x02\x42\'\n#com.qwak.ai.builds.orchestrator.apiP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17qwak/builds/build.proto\x12\x18qwak.builds.orchestrator\x1a/qwak/user_application/common/v0/resources.proto\x1a\"qwak/fitness_service/fitness.proto\"\xec\x05\n\x0fRemoteBuildSpec\x12\x43\n\x10\x62uild_properties\x18\x01 \x01(\x0b\x32).qwak.builds.orchestrator.BuildProperties\x12\x35\n\tbuild_env\x18\x02 \x01(\x0b\x32\".qwak.builds.orchestrator.BuildEnv\x12\x43\n\rcpu_resources\x18\x03 \x01(\x0b\x32&.qwak.builds.orchestrator.CpuResourcesB\x02\x18\x01H\x00\x12\x43\n\rgpu_resources\x18\x07 \x01(\x0b\x32&.qwak.builds.orchestrator.GpuResourcesB\x02\x18\x01H\x00\x12\x62\n\x1c\x63lient_pod_compute_resources\x18\r \x01(\x0b\x32:.qwak.user_application.common.v0.ClientPodComputeResourcesH\x00\x12\x0f\n\x07verbose\x18\x04 \x01(\x05\x12\x17\n\x0f\x62uild_code_path\x18\x05 \x01(\t\x12\x14\n\x0c\x62uild_config\x18\x06 \x01(\t\x12\x15\n\rbuild_v1_flag\x18\x08 \x01(\x08\x12H\n\x13\x62uild_properties_v1\x18\t \x01(\x0b\x32+.qwak.builds.orchestrator.BuildPropertiesV1\x12\x13\n\x0b\x62uild_steps\x18\n \x03(\t\x12\x16\n\x0e\x65nvironment_id\x18\x0b \x01(\t\x12\x13\n\x0bsdk_version\x18\x0c \x01(\t\x12=\n\x0fpurchase_option\x18\x0e \x01(\x0e\x32$.qwak.fitness.service.PurchaseOption\x12\x1c\n\x14\x62uild_destined_image\x18\x0f \x01(\t\x12\"\n\x1aprovision_instance_timeout\x18\x10 \x01(\x05\x42\x0b\n\tResources\"g\n\x11\x42uildPropertiesV1\x12\x18\n\x10\x62uild_config_url\x18\x01 \x01(\t\x12\x1a\n\x12qwak_sdk_wheel_url\x18\x02 \x01(\t\x12\x1c\n\x14qwak_sdk_version_url\x18\x03 \x01(\t\"\xa6\x01\n\x0f\x42uildProperties\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x10\n\x08model_id\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x39\n\tmodel_uri\x18\x05 \x01(\x0b\x32&.qwak.builds.orchestrator.ModelUriSpec\x12\x16\n\x0egpu_compatible\x18\x06 \x01(\x08\"\xb2\x01\n\x0cModelUriSpec\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\ngit_branch\x18\x02 \x01(\t\x12\x17\n\x0fgit_credentials\x18\x03 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x04 \x01(\t\x12\x11\n\tcommit_id\x18\x05 \x01(\t\x12\x10\n\x08main_dir\x18\x06 \x01(\t\x12#\n\x1b\x64\x65pendency_required_folders\x18\x07 \x03(\t\"|\n\x08\x42uildEnv\x12\x37\n\ndocker_env\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.DockerEnv\x12\x37\n\npython_env\x18\x02 \x01(\x0b\x32#.qwak.builds.orchestrator.PythonEnv\"\x8a\x01\n\tDockerEnv\x12\x12\n\nbase_image\x18\x01 \x01(\t\x12\x10\n\x08\x65nv_vars\x18\x02 \x03(\t\x12\x10\n\x08no_cache\x18\x03 \x01(\x08\x12\x1c\n\x14\x61ssumed_iam_role_arn\x18\x04 \x01(\t\x12\'\n\x1fservice_account_key_secret_name\x18\x05 \x01(\t\"|\n\tPythonEnv\x12\x17\n\x0fgit_credentials\x18\x01 \x01(\t\x12\x1e\n\x16git_credentials_secret\x18\x02 \x01(\t\x12\x18\n\x10qwak_sdk_version\x18\x03 \x01(\t\x12\x1c\n\x14qwak_sdk_extra_index\x18\x04 \x01(\t\"n\n\x0c\x43puResources\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x15\n\rmemory_amount\x18\x02 \x01(\x05\x12:\n\x0cmemory_units\x18\x03 \x01(\x0e\x32$.qwak.builds.orchestrator.MemoryUnit\"W\n\x0cGpuResources\x12\x33\n\x08gpu_type\x18\x01 \x01(\x0e\x32!.qwak.builds.orchestrator.GpuType\x12\x12\n\ngpu_amount\x18\x02 \x01(\x05\"\x91\x01\n\x13\x44\x61taTableDefinition\x12?\n\x07\x63olumns\x18\x01 \x03(\x0b\x32..qwak.builds.orchestrator.DataColumnDefinition\x12\x39\n\x0b\x64\x61ta_format\x18\x02 \x01(\x0b\x32$.qwak.builds.orchestrator.DataFormat\"\\\n\x14\x44\x61taColumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x36\n\x04type\x18\x02 \x01(\x0e\x32(.qwak.builds.orchestrator.DataColumnType\"J\n\nDataFormat\x12\x32\n\x03\x63sv\x18\x01 \x01(\x0b\x32#.qwak.builds.orchestrator.CsvFormatH\x00\x42\x08\n\x06\x66ormat\"G\n\tCsvFormat\x12\x11\n\tdelimiter\x18\x01 \x01(\t\x12\x12\n\nquote_char\x18\x02 \x01(\t\x12\x13\n\x0b\x65scape_char\x18\x03 \x01(\t\"\xa5\x01\n\x0e\x42uildInitiator\x12<\n\x04user\x18\x01 \x01(\x0b\x32,.qwak.builds.orchestrator.UserBuildInitiatorH\x00\x12H\n\nautomation\x18\x02 \x01(\x0b\x32\x32.qwak.builds.orchestrator.AutomationBuildInitiatorH\x00\x42\x0b\n\tInitiator\"\x14\n\x12UserBuildInitiator\"`\n\x18\x41utomationBuildInitiator\x12\x15\n\rautomation_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x17\n\x0f\x61utomation_name\x18\x03 \x01(\t*7\n\nMemoryUnit\x12\x17\n\x13UNKNOWN_MEMORY_UNIT\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02*\x8c\x02\n\x07GpuType\x12\x0b\n\x07INVALID\x10\x00\x12\x0e\n\nNVIDIA_K80\x10\x01\x12\x0f\n\x0bNVIDIA_V100\x10\x02\x12\x0f\n\x0bNVIDIA_A100\x10\x03\x12\r\n\tNVIDIA_T4\x10\x04\x12\x0f\n\x0bNVIDIA_A10G\x10\x05\x12\r\n\tNVIDIA_L4\x10\x06\x12\x14\n\x10NVIDIA_T4_1_4_15\x10\x07\x12\x14\n\x10NVIDIA_T4_1_8_30\x10\x08\x12\x15\n\x11NVIDIA_T4_1_16_60\x10\t\x12\x1e\n\x1aNVIDIA_A100_80GB_8_96_1360\x10\n\x12\x16\n\x12NVIDIA_V100_1_8_52\x10\x0b\x12\x18\n\x14NVIDIA_V100_4_32_208\x10\x0c*d\n\x0e\x44\x61taColumnType\x12\x17\n\x13INVALID_COLUMN_TYPE\x10\x00\x12\n\n\x06OBJECT\x10\x01\x12\x07\n\x03INT\x10\x02\x12\t\n\x05\x46LOAT\x10\x03\x12\x0b\n\x07\x42OOLEAN\x10\x04\x12\x0c\n\x08\x44\x41TETIME\x10\x05*K\n\x13\x42\x61seDockerImageType\x12\"\n\x1eUNKNOWN_BASE_DOCKER_IMAGE_TYPE\x10\x00\x12\x07\n\x03\x43PU\x10\x01\x12\x07\n\x03GPU\x10\x02\x42\'\n#com.qwak.ai.builds.orchestrator.apiP\x01\x62\x06proto3')
 
 _MEMORYUNIT = DESCRIPTOR.enum_types_by_name['MemoryUnit']
 MemoryUnit = enum_type_wrapper.EnumTypeWrapper(_MEMORYUNIT)
 _GPUTYPE = DESCRIPTOR.enum_types_by_name['GpuType']
 GpuType = enum_type_wrapper.EnumTypeWrapper(_GPUTYPE)
 _DATACOLUMNTYPE = DESCRIPTOR.enum_types_by_name['DataColumnType']
 DataColumnType = enum_type_wrapper.EnumTypeWrapper(_DATACOLUMNTYPE)
@@ -186,48 +186,48 @@
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n#com.qwak.ai.builds.orchestrator.apiP\001'
   _REMOTEBUILDSPEC.fields_by_name['cpu_resources']._options = None
   _REMOTEBUILDSPEC.fields_by_name['cpu_resources']._serialized_options = b'\030\001'
   _REMOTEBUILDSPEC.fields_by_name['gpu_resources']._options = None
   _REMOTEBUILDSPEC.fields_by_name['gpu_resources']._serialized_options = b'\030\001'
-  _MEMORYUNIT._serialized_start=2581
-  _MEMORYUNIT._serialized_end=2636
-  _GPUTYPE._serialized_start=2639
-  _GPUTYPE._serialized_end=2907
-  _DATACOLUMNTYPE._serialized_start=2909
-  _DATACOLUMNTYPE._serialized_end=3009
-  _BASEDOCKERIMAGETYPE._serialized_start=3011
-  _BASEDOCKERIMAGETYPE._serialized_end=3086
+  _MEMORYUNIT._serialized_start=2617
+  _MEMORYUNIT._serialized_end=2672
+  _GPUTYPE._serialized_start=2675
+  _GPUTYPE._serialized_end=2943
+  _DATACOLUMNTYPE._serialized_start=2945
+  _DATACOLUMNTYPE._serialized_end=3045
+  _BASEDOCKERIMAGETYPE._serialized_start=3047
+  _BASEDOCKERIMAGETYPE._serialized_end=3122
   _REMOTEBUILDSPEC._serialized_start=139
-  _REMOTEBUILDSPEC._serialized_end=851
-  _BUILDPROPERTIESV1._serialized_start=853
-  _BUILDPROPERTIESV1._serialized_end=956
-  _BUILDPROPERTIES._serialized_start=959
-  _BUILDPROPERTIES._serialized_end=1125
-  _MODELURISPEC._serialized_start=1128
-  _MODELURISPEC._serialized_end=1306
-  _BUILDENV._serialized_start=1308
-  _BUILDENV._serialized_end=1432
-  _DOCKERENV._serialized_start=1435
-  _DOCKERENV._serialized_end=1573
-  _PYTHONENV._serialized_start=1575
-  _PYTHONENV._serialized_end=1699
-  _CPURESOURCES._serialized_start=1701
-  _CPURESOURCES._serialized_end=1811
-  _GPURESOURCES._serialized_start=1813
-  _GPURESOURCES._serialized_end=1900
-  _DATATABLEDEFINITION._serialized_start=1903
-  _DATATABLEDEFINITION._serialized_end=2048
-  _DATACOLUMNDEFINITION._serialized_start=2050
-  _DATACOLUMNDEFINITION._serialized_end=2142
-  _DATAFORMAT._serialized_start=2144
-  _DATAFORMAT._serialized_end=2218
-  _CSVFORMAT._serialized_start=2220
-  _CSVFORMAT._serialized_end=2291
-  _BUILDINITIATOR._serialized_start=2294
-  _BUILDINITIATOR._serialized_end=2459
-  _USERBUILDINITIATOR._serialized_start=2461
-  _USERBUILDINITIATOR._serialized_end=2481
-  _AUTOMATIONBUILDINITIATOR._serialized_start=2483
-  _AUTOMATIONBUILDINITIATOR._serialized_end=2579
+  _REMOTEBUILDSPEC._serialized_end=887
+  _BUILDPROPERTIESV1._serialized_start=889
+  _BUILDPROPERTIESV1._serialized_end=992
+  _BUILDPROPERTIES._serialized_start=995
+  _BUILDPROPERTIES._serialized_end=1161
+  _MODELURISPEC._serialized_start=1164
+  _MODELURISPEC._serialized_end=1342
+  _BUILDENV._serialized_start=1344
+  _BUILDENV._serialized_end=1468
+  _DOCKERENV._serialized_start=1471
+  _DOCKERENV._serialized_end=1609
+  _PYTHONENV._serialized_start=1611
+  _PYTHONENV._serialized_end=1735
+  _CPURESOURCES._serialized_start=1737
+  _CPURESOURCES._serialized_end=1847
+  _GPURESOURCES._serialized_start=1849
+  _GPURESOURCES._serialized_end=1936
+  _DATATABLEDEFINITION._serialized_start=1939
+  _DATATABLEDEFINITION._serialized_end=2084
+  _DATACOLUMNDEFINITION._serialized_start=2086
+  _DATACOLUMNDEFINITION._serialized_end=2178
+  _DATAFORMAT._serialized_start=2180
+  _DATAFORMAT._serialized_end=2254
+  _CSVFORMAT._serialized_start=2256
+  _CSVFORMAT._serialized_end=2327
+  _BUILDINITIATOR._serialized_start=2330
+  _BUILDINITIATOR._serialized_end=2495
+  _USERBUILDINITIATOR._serialized_start=2497
+  _USERBUILDINITIATOR._serialized_end=2517
+  _AUTOMATIONBUILDINITIATOR._serialized_start=2519
+  _AUTOMATIONBUILDINITIATOR._serialized_end=2615
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     BUILD_V1_FLAG_FIELD_NUMBER: builtins.int
     BUILD_PROPERTIES_V1_FIELD_NUMBER: builtins.int
     BUILD_STEPS_FIELD_NUMBER: builtins.int
     ENVIRONMENT_ID_FIELD_NUMBER: builtins.int
     SDK_VERSION_FIELD_NUMBER: builtins.int
     PURCHASE_OPTION_FIELD_NUMBER: builtins.int
     BUILD_DESTINED_IMAGE_FIELD_NUMBER: builtins.int
+    PROVISION_INSTANCE_TIMEOUT_FIELD_NUMBER: builtins.int
     @property
     def build_properties(self) -> global___BuildProperties: ...
     @property
     def build_env(self) -> global___BuildEnv: ...
     @property
     def cpu_resources(self) -> global___CpuResources:
         """CPU Properties"""
@@ -179,14 +180,16 @@
     environment_id: builtins.str
     """The environment to build on"""
     sdk_version: builtins.str
     """The build SDK version"""
     purchase_option: qwak.fitness_service.fitness_pb2.PurchaseOption.ValueType
     """Purchase option for the build"""
     build_destined_image: builtins.str
+    provision_instance_timeout: builtins.int
+    """Timeout in minutes of the provisioning build step"""
     def __init__(
         self,
         *,
         build_properties: global___BuildProperties | None = ...,
         build_env: global___BuildEnv | None = ...,
         cpu_resources: global___CpuResources | None = ...,
         gpu_resources: global___GpuResources | None = ...,
@@ -197,17 +200,18 @@
         build_v1_flag: builtins.bool = ...,
         build_properties_v1: global___BuildPropertiesV1 | None = ...,
         build_steps: collections.abc.Iterable[builtins.str] | None = ...,
         environment_id: builtins.str = ...,
         sdk_version: builtins.str = ...,
         purchase_option: qwak.fitness_service.fitness_pb2.PurchaseOption.ValueType = ...,
         build_destined_image: builtins.str = ...,
+        provision_instance_timeout: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["Resources", b"Resources", "build_env", b"build_env", "build_properties", b"build_properties", "build_properties_v1", b"build_properties_v1", "client_pod_compute_resources", b"client_pod_compute_resources", "cpu_resources", b"cpu_resources", "gpu_resources", b"gpu_resources"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["Resources", b"Resources", "build_code_path", b"build_code_path", "build_config", b"build_config", "build_destined_image", b"build_destined_image", "build_env", b"build_env", "build_properties", b"build_properties", "build_properties_v1", b"build_properties_v1", "build_steps", b"build_steps", "build_v1_flag", b"build_v1_flag", "client_pod_compute_resources", b"client_pod_compute_resources", "cpu_resources", b"cpu_resources", "environment_id", b"environment_id", "gpu_resources", b"gpu_resources", "purchase_option", b"purchase_option", "sdk_version", b"sdk_version", "verbose", b"verbose"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["Resources", b"Resources", "build_code_path", b"build_code_path", "build_config", b"build_config", "build_destined_image", b"build_destined_image", "build_env", b"build_env", "build_properties", b"build_properties", "build_properties_v1", b"build_properties_v1", "build_steps", b"build_steps", "build_v1_flag", b"build_v1_flag", "client_pod_compute_resources", b"client_pod_compute_resources", "cpu_resources", b"cpu_resources", "environment_id", b"environment_id", "gpu_resources", b"gpu_resources", "provision_instance_timeout", b"provision_instance_timeout", "purchase_option", b"purchase_option", "sdk_version", b"sdk_version", "verbose", b"verbose"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["Resources", b"Resources"]) -> typing_extensions.Literal["cpu_resources", "gpu_resources", "client_pod_compute_resources"] | None: ...
 
 global___RemoteBuildSpec = RemoteBuildSpec
 
 class BuildPropertiesV1(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/backfill_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/backfill_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/batch_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/batch_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/deletion_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/deletion_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/management_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/management_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/population_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/population_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/filters_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/filters_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_service_pb2.py` & `qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi` & `qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py` & `qwak_core-0.4.6/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/pyproject.toml` & `qwak_core-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.4.5"
+version = "0.4.6"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.4.5/qwak/__init__.py` & `qwak_core-0.4.6/qwak/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for qwak-core."""
 
 __author__ = "Qwak.ai"
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 
 from qwak.inner.di_configuration import wire_dependencies
 from qwak.model.experiment_tracking import log_metric, log_param
 from qwak.model_loggers.artifact_logger import load_file, log_file
 from qwak.model_loggers.data_logger import load_data, log_data
 from qwak.model_loggers.model_logger import load_model, log_model
```

### Comparing `qwak_core-0.4.5/qwak/automations/__init__.py` & `qwak_core-0.4.6/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/automations/automation_executions.py` & `qwak_core-0.4.6/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/automations/automations.py` & `qwak_core-0.4.6/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/automations/batch_execution_action.py` & `qwak_core-0.4.6/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.4.6/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/automations/common.py` & `qwak_core-0.4.6/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/_inner/edge_communications.py` & `qwak_core-0.4.6/qwak/clients/_inner/edge_communications.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.4.6/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/administration/authentication/client.py` & `qwak_core-0.4.6/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.4.6/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/administration/environment/client.py` & `qwak_core-0.4.6/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/administration/self_service/client.py` & `qwak_core-0.4.6/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/alert_management/client.py` & `qwak_core-0.4.6/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/alerts_registry/channel.py` & `qwak_core-0.4.6/qwak/clients/alerts_registry/channel.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/alerts_registry/client.py` & `qwak_core-0.4.6/qwak/clients/alerts_registry/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/analytics/client.py` & `qwak_core-0.4.6/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/audience/client.py` & `qwak_core-0.4.6/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/automation_management/client.py` & `qwak_core-0.4.6/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/autoscaling/client.py` & `qwak_core-0.4.6/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/batch_job_management/client.py` & `qwak_core-0.4.6/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.4.6/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/batch_job_management/results.py` & `qwak_core-0.4.6/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/build_management/client.py` & `qwak_core-0.4.6/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/build_orchestrator/build_model_request_getter.py` & `qwak_core-0.4.6/qwak/clients/build_orchestrator/build_model_request_getter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.4.6/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/build_orchestrator/internal_client.py` & `qwak_core-0.4.6/qwak/clients/build_orchestrator/internal_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/data_versioning/client.py` & `qwak_core-0.4.6/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/data_versioning/data_tag_filter.py` & `qwak_core-0.4.6/qwak/clients/data_versioning/data_tag_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/deployment/client.py` & `qwak_core-0.4.6/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/feature_store/execution_management_client.py` & `qwak_core-0.4.6/qwak/clients/feature_store/execution_management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.4.6/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/feature_store/management_client.py` & `qwak_core-0.4.6/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/feature_store/offline_serving_client.py` & `qwak_core-0.4.6/qwak/clients/feature_store/offline_serving_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.4.6/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/file_versioning/client.py` & `qwak_core-0.4.6/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/file_versioning/file_tag_filter.py` & `qwak_core-0.4.6/qwak/clients/file_versioning/file_tag_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/instance_template/client.py` & `qwak_core-0.4.6/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.4.6/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/logging_client/client.py` & `qwak_core-0.4.6/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/model_management/client.py` & `qwak_core-0.4.6/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/project/client.py` & `qwak_core-0.4.6/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/secret_service/client.py` & `qwak_core-0.4.6/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/user_application_instance/client.py` & `qwak_core-0.4.6/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/vector_store/management_client.py` & `qwak_core-0.4.6/qwak/clients/vector_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/vector_store/serving_client.py` & `qwak_core-0.4.6/qwak/clients/vector_store/serving_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/clients/workspace_manager/client.py` & `qwak_core-0.4.6/qwak/clients/workspace_manager/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/exceptions/__init__.py` & `qwak_core-0.4.6/qwak/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/exceptions/quiet_error.py` & `qwak_core-0.4.6/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.4.6/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/exceptions/qwak_suggestion_exception.py` & `qwak_core-0.4.6/qwak/exceptions/qwak_suggestion_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/_common/artifact_utils.py` & `qwak_core-0.4.6/qwak/feature_store/_common/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/_common/feature_set_utils.py` & `qwak_core-0.4.6/qwak/feature_store/_common/feature_set_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.4.6/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/_common/functions.py` & `qwak_core-0.4.6/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/_common/packaging.py` & `qwak_core-0.4.6/qwak/feature_store/_common/packaging.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/base.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/_jdbc.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/athena.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/athena.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/big_query.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/clickhouse.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/clickhouse.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/csv.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/elastic_search.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/filesystem/aws.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/filesystem/aws.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/filesystem/gcp.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/filesystem/gcp.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/filesystem/utils.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/filesystem/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/mongodb.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/mysql.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/parquet.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/postgres.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/redshift.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/snowflake.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/batch/vertica.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/batch/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/source_authentication.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/source_authentication.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/kafka/__init__.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/kafka/authentication.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/kafka/deserialization.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/kafka/deserialization.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/streaming/kafka/kafka.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/streaming/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/data_sources/time_partition_columns.py` & `qwak_core-0.4.6/qwak/feature_store/data_sources/time_partition_columns.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/entities/entity.py` & `qwak_core-0.4.6/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/execution/backfill.py` & `qwak_core-0.4.6/qwak/feature_store/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/execution/execution.py` & `qwak_core-0.4.6/qwak/feature_store/execution/execution.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/execution/execution_query.py` & `qwak_core-0.4.6/qwak/feature_store/execution/execution_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/_utils/_featureset_utils.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/_utils/_featureset_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/base_feature_set.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/base_feature_set.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/streaming.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/streaming.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/streaming_backfill.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/streaming_backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/__init__.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/aggregations/windows.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/aggregations/windows.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/functions/schema.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/functions/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/feature_sets/transformations/transformations.py` & `qwak_core-0.4.6/qwak/feature_store/feature_sets/transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/offline/_offline_serving_validations.py` & `qwak_core-0.4.6/qwak/feature_store/offline/_offline_serving_validations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.4.6/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.4.6/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/offline/client.py` & `qwak_core-0.4.6/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/offline/client_v2.py` & `qwak_core-0.4.6/qwak/feature_store/offline/client_v2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/offline/feature_set_features.py` & `qwak_core-0.4.6/qwak/feature_store/offline/feature_set_features.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/online/client.py` & `qwak_core-0.4.6/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/online/endpoint_utils.py` & `qwak_core-0.4.6/qwak/feature_store/online/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/validations/validation_options.py` & `qwak_core-0.4.6/qwak/feature_store/validations/validation_options.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/validations/validation_response.py` & `qwak_core-0.4.6/qwak/feature_store/validations/validation_response.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/feature_store/validations/validator.py` & `qwak_core-0.4.6/qwak/feature_store/validations/validator.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_config/build_config_v1.py` & `qwak_core-0.4.6/qwak/inner/build_config/build_config_v1.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/build_loggers/trigger_build_logger.py` & `qwak_core-0.4.6/qwak/inner/build_logic/build_loggers/trigger_build_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/execute_build_pipeline.py` & `qwak_core-0.4.6/qwak/inner/build_logic/execute_build_pipeline.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/interface/build_logger_interface.py` & `qwak_core-0.4.6/qwak/inner/build_logic/interface/build_logger_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/interface/build_phase.py` & `qwak_core-0.4.6/qwak/inner/build_logic/interface/build_phase.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/interface/context_interface.py` & `qwak_core-0.4.6/qwak/inner/build_logic/interface/context_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/interface/phase_run_handler.py` & `qwak_core-0.4.6/qwak/inner/build_logic/interface/phase_run_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/interface/step_inteface.py` & `qwak_core-0.4.6/qwak/inner/build_logic/interface/step_inteface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/interface/time_source.py` & `qwak_core-0.4.6/qwak/inner/build_logic/interface/time_source.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/phases/phases_pipeline.py` & `qwak_core-0.4.6/qwak/inner/build_logic/phases/phases_pipeline.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py` & `qwak_core-0.4.6/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/tools/dependencies_tools.py` & `qwak_core-0.4.6/qwak/inner/build_logic/tools/dependencies_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/tools/files.py` & `qwak_core-0.4.6/qwak/inner/build_logic/tools/files.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/build_logic/tools/ignore_files.py` & `qwak_core-0.4.6/qwak/inner/build_logic/tools/ignore_files.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/const.py` & `qwak_core-0.4.6/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.4.6/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/di_configuration/account.py` & `qwak_core-0.4.6/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/di_configuration/containers.py` & `qwak_core-0.4.6/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/instance_template/verify_template_id.py` & `qwak_core-0.4.6/qwak/inner/instance_template/verify_template_id.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/model_loggers_utils.py` & `qwak_core-0.4.6/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/runtime_di/containers.py` & `qwak_core-0.4.6/qwak/inner/runtime_di/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/singleton_meta.py` & `qwak_core-0.4.6/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/tool/auth.py` & `qwak_core-0.4.6/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.4.6/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/tool/protobuf_factory.py` & `qwak_core-0.4.6/qwak/inner/tool/protobuf_factory.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/tool/run_config/base.py` & `qwak_core-0.4.6/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.4.6/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/_entity_extraction.py` & `qwak_core-0.4.6/qwak/model/_entity_extraction.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/adapters/__init__.py` & `qwak_core-0.4.6/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.4.6/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.4.6/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.4.6/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.4.6/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.4.6/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/base.py` & `qwak_core-0.4.6/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/decorators/api.py` & `qwak_core-0.4.6/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/decorators/impl/api_implementation.py` & `qwak_core-0.4.6/qwak/model/decorators/impl/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/decorators/timer.py` & `qwak_core-0.4.6/qwak/model/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/experiment_tracking.py` & `qwak_core-0.4.6/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/schema.py` & `qwak_core-0.4.6/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/schema_entities.py` & `qwak_core-0.4.6/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/__init__.py` & `qwak_core-0.4.6/qwak/model/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/input.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/output.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.4.6/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model/tools/run_model_locally.py` & `qwak_core-0.4.6/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.4.6/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model_loggers/data_logger.py` & `qwak_core-0.4.6/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/model_loggers/model_logger.py` & `qwak_core-0.4.6/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/batch_jobs/execution.py` & `qwak_core-0.4.6/qwak/qwak_client/batch_jobs/execution.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/batch_jobs/task.py` & `qwak_core-0.4.6/qwak/qwak_client/batch_jobs/task.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/build_api_helpers/build_api_steps.py` & `qwak_core-0.4.6/qwak/qwak_client/build_api_helpers/build_api_steps.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/build_api_helpers/trigger_build_api.py` & `qwak_core-0.4.6/qwak/qwak_client/build_api_helpers/trigger_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/builds/build.py` & `qwak_core-0.4.6/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.4.6/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.4.6/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/client.py` & `qwak_core-0.4.6/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/data_versioning/data_tag.py` & `qwak_core-0.4.6/qwak/qwak_client/data_versioning/data_tag.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.4.6/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/file_versioning/file_tag.py` & `qwak_core-0.4.6/qwak/qwak_client/file_versioning/file_tag.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/models/model.py` & `qwak_core-0.4.6/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.4.6/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/qwak_client/projects/project.py` & `qwak_core-0.4.6/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/tools/logger/logger.py` & `qwak_core-0.4.6/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/tools/logger/logging.yml` & `qwak_core-0.4.6/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/utils/datetime_utils.py` & `qwak_core-0.4.6/qwak/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/vector_store/client.py` & `qwak_core-0.4.6/qwak/vector_store/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/vector_store/collection.py` & `qwak_core-0.4.6/qwak/vector_store/collection.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/vector_store/filters.py` & `qwak_core-0.4.6/qwak/vector_store/filters.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/vector_store/inference_client.py` & `qwak_core-0.4.6/qwak/vector_store/inference_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/vector_store/rest_helpers.py` & `qwak_core-0.4.6/qwak/vector_store/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/vector_store/utils/filter_utils.py` & `qwak_core-0.4.6/qwak/vector_store/utils/filter_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak/vector_store/utils/upsert_utils.py` & `qwak_core-0.4.6/qwak/vector_store/utils/upsert_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/alert_registry_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/alert_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/execution_management_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/execution_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/fs_offline_serving_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/fs_offline_serving_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/internal_build_orchestrator_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/internal_build_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/vector_serving_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/vector_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/vectors_management_api.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/vectors_management_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/mocks/workspace_manager_service_mock.py` & `qwak_core-0.4.6/qwak_services_mock/mocks/workspace_manager_service_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/qwak_services_mock/services_mock.py` & `qwak_core-0.4.6/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.5/setup.py` & `qwak_core-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 {':extra == "feature-store"': ['cloudpickle==2.2.1'],
  ':python_full_version >= "3.7.1" and python_version < "3.10"': ['protobuf>=3.10,<4'],
  ':python_version >= "3.10"': ['protobuf>=4.21.6'],
  'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.4.5',
+    'version': '0.4.6',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.4.5/PKG-INFO` & `qwak_core-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.4.5
+Version: 0.4.6
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```


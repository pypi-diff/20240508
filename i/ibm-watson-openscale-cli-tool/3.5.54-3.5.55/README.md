# Comparing `tmp/ibm-watson-openscale-cli-tool-3.5.54.tar.gz` & `tmp/ibm-watson-openscale-cli-tool-3.5.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-watson-openscale-cli-tool-3.5.54.tar", last modified: Thu Aug  3 03:03:14 2023, max compression
+gzip compressed data, was "ibm-watson-openscale-cli-tool-3.5.55.tar", last modified: Wed May  8 04:31:35 2024, max compression
```

## Comparing `ibm-watson-openscale-cli-tool-3.5.54.tar` & `ibm-watson-openscale-cli-tool-3.5.55.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.585342 ibm-watson-openscale-cli-tool-3.5.54/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    10173 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/LICENSE
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)      215 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/MANIFEST.in
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    21142 2023-08-03 03:03:14.585023 ibm-watson-openscale-cli-tool-3.5.54/PKG-INFO
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    20369 2023-02-10 07:19:55.000000 ibm-watson-openscale-cli-tool-3.5.54/README.md
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.318239 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)        6 2023-07-20 16:12:01.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/VERSION
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1557 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/__init__.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4804 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/api_environment.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4705 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/credentials.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.322748 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4514 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/cos.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    13546 2022-09-26 12:11:09.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/db2.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     7086 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/postgres.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1078 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/postgres_compose.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1055 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/postgres_icd.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     1288 2023-03-27 07:39:06.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/enums.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     5562 2023-07-27 12:04:31.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/environments.py
--rwxr-xr-x   0 prateekgoyal   (501) staff       (20)    21875 2023-08-03 03:02:45.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/main.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.326553 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2900 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/azure_machine_learning.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1875 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/custom_machine_learning.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2084 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/sagemaker_machine_learning.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1584 2022-08-01 08:54:52.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/spss_machine_learning.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    25312 2023-05-08 06:59:25.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/watson_machine_learning.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.327964 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.341607 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.342808 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     2512 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/configuration.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.344496 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     2512 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/configuration.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   200347 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/history_payloads.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.347137 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     2500 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/configuration.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   116539 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/history_payloads.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     7171 2023-03-03 05:56:45.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/feedback_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)  1152715 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_fairness.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    90011 2023-03-03 05:56:45.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_quality_monitor.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.358225 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     5766 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/configuration.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     7631 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/feedback_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   561618 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_fairness.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   107766 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_payloads.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   634377 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    24287 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data_statistics.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.359662 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     2503 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/configuration.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   337912 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/history_payloads.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   688531 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    31533 2023-03-03 06:16:49.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data_statistics.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.522759 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     6043 2023-03-27 07:39:06.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/configuration.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.305469 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.524305 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/4.7/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   161371 2023-04-24 12:00:29.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/4.7/baseline.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.526699 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/public_cloud/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   161371 2023-04-24 12:00:29.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/public_cloud/baseline.tar.gz
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   320533 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_history_measurements_payload_per_run.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   377407 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_insights_record_payloads.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   221506 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_intervals_record_payloads.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   196012 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_baseline_record_payloads.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)  1200592 2023-04-28 09:23:48.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_production_record_payloads.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.306154 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.528522 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/4.7/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   126846 2023-07-12 09:54:00.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/4.7/explainability.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.530105 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/public_cloud/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   126846 2023-07-12 09:54:00.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/public_cloud/explainability.tar.gz
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14206 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/feedback_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   710154 2022-08-26 05:34:41.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debias.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537110 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_0.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   536973 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_1.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537385 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_2.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537039 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_3.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537121 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_4.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537075 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_5.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   537028 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_6.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     5327 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_explanations.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)  1152715 2022-08-26 05:34:41.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_fairness.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  1432534 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_manual_labeling.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   242701 2023-07-20 16:12:01.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_mhm.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5209548 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_0.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5207503 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_1.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5210337 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_2.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5210470 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_3.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5209458 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_4.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5210872 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_5.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)  5209866 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_6.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    15288 2022-08-01 08:55:15.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_performance.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.535830 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.538004 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    60889 2023-04-24 13:19:16.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_content.gzip
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    13447 2023-04-24 13:19:16.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_meta.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     2751 2023-03-27 07:39:06.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/configuration.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.307294 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.538735 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/4.7/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   158866 2023-04-24 12:00:29.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/4.7/baseline.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.540529 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/public_cloud/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   158866 2023-04-24 12:00:29.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/public_cloud/baseline.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.307957 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.542179 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/4.7/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   130504 2023-07-12 09:54:00.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/4.7/explainability.tar.gz
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.543593 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/public_cloud/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   130504 2023-07-12 09:54:00.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/public_cloud/explainability.tar.gz
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14275 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/mrm_evaluation_data.csv
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.546277 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    60883 2023-04-20 13:09:42.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_content.gzip
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    13447 2023-04-20 13:09:42.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.548115 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    61574 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    13626 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.550002 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    60715 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    13666 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.551367 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    60839 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_content.gzip
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    13629 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_meta.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   689622 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    31531 2022-12-08 09:39:57.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data_statistics.json
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14206 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm_evaluation_data.csv
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    13227 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/scoring_data.csv
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)   688531 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data.csv
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    28527 2022-12-08 09:39:57.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data_statistics.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.553588 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    37201 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    15506 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.310390 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.555222 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    68724 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14847 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.556804 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    49882 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_content.gzip
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    14851 2022-08-01 08:55:35.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.558389 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    34280 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_content.gzip
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    14851 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_meta.json
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.560248 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    34778 2023-04-24 13:19:16.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_content.gzip
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    14703 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_meta.json
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    33548 2023-08-03 03:02:45.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/model.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.562424 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/openscale/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     6445 2023-02-07 10:22:14.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/openscale/openscale.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)   109898 2023-08-03 03:02:45.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/openscale/openscale_client.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     8653 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/openscale/openscale_reset.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    13187 2023-08-03 03:02:45.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/openscale_ops.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     7791 2023-03-27 07:39:06.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ops.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2733 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/reset_ops.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.568567 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    10509 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/cloud_foundry.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     6938 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/cloud_foundry_cli.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     8801 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/resource_controller.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5908 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/resource_controller_cli.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1331 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     3647 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_cli.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     8861 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_rest.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     3750 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_ibmcloudprivate_services.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2880 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_services.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     6829 2023-02-14 09:40:21.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/token_manager.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.572443 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     3911 2023-08-03 03:02:45.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/constants.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5917 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/fastpath_logger.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     1517 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/keras_unstructured_binary_text.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2794 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/statistics_generator.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)      825 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/timer.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     5494 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/utils.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.576020 ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    21142 2023-08-03 03:03:14.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/PKG-INFO
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     9508 2023-08-03 03:03:14.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/SOURCES.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)        1 2023-08-03 03:03:14.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/dependency_links.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)       76 2023-08-03 03:03:14.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/entry_points.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)      229 2023-08-03 03:03:14.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/requires.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)       21 2023-08-03 03:03:14.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/top_level.txt
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)        1 2021-02-19 08:47:18.000000 ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/zip-safe
--rw-r--r--   0 prateekgoyal   (501) staff       (20)       38 2023-08-03 03:03:14.585431 ibm-watson-openscale-cli-tool-3.5.54/setup.cfg
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     3350 2023-07-20 16:12:01.000000 ibm-watson-openscale-cli-tool-3.5.54/setup.py
-drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2023-08-03 03:03:14.584241 ibm-watson-openscale-cli-tool-3.5.54/tests/
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)    12683 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_cloud_foundry.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     2984 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_db2.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     1792 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_openscale.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)     4229 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_postgres.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)    10808 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_resource_controller.py
--rwxrwxrwx   0 prateekgoyal   (501) staff       (20)        0 2022-08-01 08:55:50.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_set_up.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     1434 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_setup_ibmcloud_services.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     9611 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_setup_ibmcloud_services_rest.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     1653 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_setup_ibmcloudprivate_services.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     5170 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_token_manager.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     1744 2023-02-17 11:22:39.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_utils.py
--rw-r--r--   0 prateekgoyal   (501) staff       (20)     8285 2023-02-10 07:19:56.000000 ibm-watson-openscale-cli-tool-3.5.54/tests/test_watson_machine_learning.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.132914 ibm-watson-openscale-cli-tool-3.5.55/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    10173 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/LICENSE
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)      215 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/MANIFEST.in
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    21551 2024-05-08 04:31:35.132133 ibm-watson-openscale-cli-tool-3.5.55/PKG-INFO
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    20369 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/README.md
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.849265 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)        6 2024-05-08 04:30:46.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/VERSION
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1557 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/__init__.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     4784 2024-01-29 04:30:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/api_environment.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     4705 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/credentials.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.852621 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     4514 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/cos.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13546 2023-09-27 03:47:07.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/db2.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     7086 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/postgres.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1078 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/postgres_compose.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1055 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/postgres_icd.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1322 2024-02-22 05:22:40.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/enums.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5562 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/environments.py
+-rwxr-xr-x   0 prateekgoyal   (501) staff       (20)    21875 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/main.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.855685 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2900 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/azure_machine_learning.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1875 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/custom_machine_learning.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2084 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/sagemaker_machine_learning.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1584 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/spss_machine_learning.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    27122 2024-02-22 05:22:19.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/watson_machine_learning.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.856751 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.868529 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.869703 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2512 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/configuration.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.871470 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2512 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/configuration.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   200347 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/history_payloads.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.874491 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2500 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/configuration.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   116539 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/history_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     7171 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/feedback_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  1152715 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_fairness.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    90011 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_quality_monitor.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.886199 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5766 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/configuration.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     7631 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/feedback_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   561618 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_fairness.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   107766 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   634377 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    24287 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data_statistics.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.888062 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2503 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/configuration.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   337912 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/history_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   688531 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    31533 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data_statistics.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.064568 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    11037 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/configuration.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.833542 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.065885 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/4.7/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   161371 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/4.7/baseline.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.067732 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/public_cloud/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   272085 2024-05-07 11:55:23.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/public_cloud/baseline.tar.gz
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   320533 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_history_measurements_payload_per_run.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   377407 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_insights_record_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   221506 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_intervals_record_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   196012 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_baseline_record_payloads.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  1200592 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_production_record_payloads.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.834284 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.068643 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/4.7/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   126846 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/4.7/explainability.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.070552 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/public_cloud/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   126846 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/public_cloud/explainability.tar.gz
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    14206 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/feedback_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   710154 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debias.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   537110 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_0.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   536973 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_1.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   537385 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_2.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   537039 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_3.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   537121 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_4.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   537075 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_5.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   537028 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_6.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5327 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_explanations.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  1152715 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_fairness.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  1432534 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_manual_labeling.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   242701 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_mhm.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  5209548 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_0.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  5207503 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_1.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  5210337 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_2.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  5210470 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_3.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  5209458 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_4.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  5210872 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_5.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)  5209866 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_6.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    15288 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_performance.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.079463 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.082889 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    60889 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13447 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_meta.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     7745 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/configuration.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.835353 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.083732 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/4.7/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   158866 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/4.7/baseline.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.085520 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/public_cloud/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   235468 2024-05-07 11:55:23.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/public_cloud/baseline.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.836443 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.086207 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/4.7/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   130504 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/4.7/explainability.tar.gz
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.088366 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/public_cloud/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   130504 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/public_cloud/explainability.tar.gz
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    14275 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/mrm_evaluation_data.csv
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.090805 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    60883 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13447 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.092349 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    61574 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13626 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.094105 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    60715 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13666 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.095561 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    60839 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13629 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_meta.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   689622 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    31531 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data_statistics.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    14206 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm_evaluation_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13227 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/scoring_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   688531 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data.csv
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    28527 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data_statistics.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.096806 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    37201 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    15506 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:34.838701 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.098617 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    68724 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    14847 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.100132 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    49882 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    14851 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.101927 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    34280 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    14851 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_meta.json
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.103106 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    34778 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_content.gzip
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    14703 2023-08-22 05:01:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_meta.json
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    33548 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/model.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.106409 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/openscale/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     6701 2023-11-13 09:25:20.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/openscale/openscale.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)   108699 2024-02-29 05:21:44.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/openscale/openscale_client.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     9353 2024-02-22 05:22:19.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/openscale/openscale_reset.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    13877 2024-02-22 05:22:19.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/openscale_ops.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     7948 2024-02-22 05:22:40.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ops.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2987 2024-02-22 05:22:19.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/reset_ops.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.113203 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    10509 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/cloud_foundry.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     6938 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/cloud_foundry_cli.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     8801 2024-04-03 06:46:51.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/resource_controller.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5908 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/resource_controller_cli.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1331 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     3647 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_cli.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     8861 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_rest.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     3750 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_ibmcloudprivate_services.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2880 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_services.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     6829 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/token_manager.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.116670 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     4268 2024-02-22 05:22:40.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/constants.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5917 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/fastpath_logger.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1517 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/keras_unstructured_binary_text.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2794 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/statistics_generator.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)      825 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/timer.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     6015 2024-01-02 09:04:17.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/utils.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.131091 ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    21551 2024-05-08 04:31:34.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/PKG-INFO
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     9508 2024-05-08 04:31:34.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)        1 2024-05-08 04:31:34.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)       76 2024-05-08 04:31:34.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/entry_points.txt
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)      229 2024-05-08 04:31:34.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/requires.txt
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)       21 2024-05-08 04:31:34.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/top_level.txt
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)        1 2023-08-23 05:56:44.000000 ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/zip-safe
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)       38 2024-05-08 04:31:35.133076 ibm-watson-openscale-cli-tool-3.5.55/setup.cfg
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     3350 2023-10-25 13:22:42.000000 ibm-watson-openscale-cli-tool-3.5.55/setup.py
+drwxr-xr-x   0 prateekgoyal   (501) staff       (20)        0 2024-05-08 04:31:35.130057 ibm-watson-openscale-cli-tool-3.5.55/tests/
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    12683 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_cloud_foundry.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     2984 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_db2.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1792 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_openscale.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     4229 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_postgres.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)    10808 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_resource_controller.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)        0 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_set_up.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1434 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_setup_ibmcloud_services.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     9611 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_setup_ibmcloud_services_rest.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1653 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_setup_ibmcloudprivate_services.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     5170 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_token_manager.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     1744 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_utils.py
+-rw-r--r--   0 prateekgoyal   (501) staff       (20)     8285 2023-08-22 05:01:21.000000 ibm-watson-openscale-cli-tool-3.5.55/tests/test_watson_machine_learning.py
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/LICENSE` & `ibm-watson-openscale-cli-tool-3.5.55/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/PKG-INFO` & `ibm-watson-openscale-cli-tool-3.5.55/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: ibm-watson-openscale-cli-tool
-Version: 3.5.54
-Summary: CLI library to automate the onboarding process to IBM Watson OpenScale
-Home-page: https://www.ibm.com/cloud/watson-openscale
-Author: IBM Corp
-Author-email: wps@us.ibm.com
-License: Apache-2.0
-Keywords: ai-openscale,ibm-watson
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ibm-watson-openscale-cli
 ![Status](https://img.shields.io/badge/status-beta-yellow.svg)
 [![Latest Stable Version](https://img.shields.io/pypi/v/ibm-watson-openscale-cli.svg)](https://pypi.python.org/pypi/ibm-watson-openscale-cli-tool)
 
 IBM Watson Openscale "express path" configuration tool. This tool allows the user to get started quickly with Watson OpenScale.
 * If needed, automatically provision a Lite plan instance for IBM Watson OpenScale.
 * If needed, automatically provision a Lite plan instance for IBM Watson Machine Learning.
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/README.md` & `ibm-watson-openscale-cli-tool-3.5.55/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: ibm-watson-openscale-cli-tool
+Version: 3.5.55
+Summary: CLI library to automate the onboarding process to IBM Watson OpenScale
+Home-page: https://www.ibm.com/cloud/watson-openscale
+Author: IBM Corp
+Author-email: wps@us.ibm.com
+License: Apache-2.0
+Keywords: ai-openscale,ibm-watson
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: h5py>=2.9.0
+Requires-Dist: requests<3.0,>=2.0
+Requires-Dist: urllib3==1.26.18
+Requires-Dist: retrying==1.3.3
+Requires-Dist: boto3==1.17.22
+Requires-Dist: psycopg2==2.8.6
+Requires-Dist: ibm-db>=3.0.3
+Requires-Dist: ibm-cloud-sdk-core==3.16.5
+Requires-Dist: ibm-watson-openscale>=3.0.32
+Requires-Dist: ibm-watson-machine-learning>=1.0.264
+Requires-Dist: pandas==1.3.5
+Requires-Dist: pyJWT==2.4.0
+
 # ibm-watson-openscale-cli
 ![Status](https://img.shields.io/badge/status-beta-yellow.svg)
 [![Latest Stable Version](https://img.shields.io/pypi/v/ibm-watson-openscale-cli.svg)](https://pypi.python.org/pypi/ibm-watson-openscale-cli-tool)
 
 IBM Watson Openscale "express path" configuration tool. This tool allows the user to get started quickly with Watson OpenScale.
 * If needed, automatically provision a Lite plan instance for IBM Watson OpenScale.
 * If needed, automatically provision a Lite plan instance for IBM Watson Machine Learning.
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/__init__.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/api_environment.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/api_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 5900-A3Q, 5737-H76
 # Copyright IBM Corp. 2021
 # The source code for this program is not published or other-wise divested of its trade 
 # secrets, irrespective of what has been deposited with the U.S.Copyright Office.
 # ----------------------------------------------------------------------------------------------------
 
 # coding=utf-8
-from distutils.util import strtobool
+from ibm_ai_openscale_cli.utility_classes.utils import strtobool
 from ibm_ai_openscale_cli.utility_classes.utils import get_path
 from pathlib import Path
 import logging
 import configparser
 import os
 
 logger = logging.getLogger(__name__)
@@ -53,15 +53,15 @@
                     config = configparser.ConfigParser()
                     config.read(properties_file)
                     if config.has_section("properties"):
                         ApiEnvironment.properties = config["properties"]
                 # set all the properties
                 ApiEnvironment.json_enabled = self.get_property_boolean_value('FASTPATH_CLI_JSON_LOGGING_ENABLED', False)
                 ApiEnvironment.logging_from_api = self.get_property_boolean_value('FASTPATH_CLI_LOGGING_FROM_API', False)
-                ApiEnvironment.icp_gateway_url = self.get_property_value('GATEWAY_URL', 'http://ai-open-scale-ibm-aios-nginx-internal')
+                ApiEnvironment.icp_gateway_url = self.get_property_value('GATEWAY_URL')
                 ApiEnvironment.icp4d_namespace = self.get_property_value('ICP4D_NAMESPACE', 'zen')
                 ApiEnvironment.aios_namespace = self.get_property_value('AIOS_NAMESPACE', 'aiopenscale')
                 ApiEnvironment.is_running_on_icp = self.get_property_boolean_value('ENABLE_ICP', False)
                 ApiEnvironment.log_source_crn = self.get_property_value('LOG_SOURCE_CRN', None)
                 ApiEnvironment.save_service_copy = self.get_property_boolean_value('SAVE_SERVICE_COPY', False)
                 # mark intialization done
                 ApiEnvironment.initialized = True
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/credentials.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/cos.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/cos.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/db2.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/db2.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/postgres.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/postgres.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/postgres_compose.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/postgres_compose.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/database_classes/postgres_icd.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/database_classes/postgres_icd.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/enums.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,8 +33,9 @@
     CPD_4_0_0 = "cpd_4.0.0"
     CPD_4_0_1 = "cpd_4.0.1"
     CPD_4_0_2_PLUS = "cpd_4.0.2+"
     CPD_4_0_8_PLUS = "cpd_4.0.8+"
     CPD_4_5 = "cpd_4.5"
     CPD_4_5_1_PLUS = "cpd_4.5.1+"
     CPD_4_5_3_PLUS = "cpd_4.5.3+"
-    CPD_4_7_PLUS = "cpd_4.7+"
+    CPD_4_7_PLUS = "cpd_4.7+"
+    CPD_4_8_4_PLUS = "cpd_4.8.4+"
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/environments.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/environments.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/main.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/main.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/azure_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/azure_machine_learning.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/custom_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/custom_machine_learning.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/sagemaker_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/sagemaker_machine_learning.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/spss_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/spss_machine_learning.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ml_engines/watson_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ml_engines/watson_machine_learning.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from ibm_ai_openscale_cli.utility_classes.utils import jsonFileToDict
 from ibm_watson_machine_learning import APIClient
 from ibm_watson_machine_learning.wml_client_error import ApiRequestFailure
 from ibm_ai_openscale_cli.utility_classes.constants import WML_CHALLENGER_SOFTWARE_SPEC_MAPPING, WML_CHALLENGER_SOFTWARE_SPEC_MAPPING_ZLINUX
 
 logger = FastpathLogger(__name__)
 
-
 class WatsonMachineLearningEngine:
 
     def __init__(self, credentials, openscale_client, cos_credentials=None, is_v4=False, is_mrm=False, is_icp=False, is_zlinux=False):
         start = time.time()
         self._credentials = credentials
         self._client = APIClient(dict(credentials))
         self._openscale_client = openscale_client
@@ -41,15 +40,15 @@
 
     def get_native_client(self):
         return self._client
 
     def set_model(self, model):
         self._model_metadata = model.metadata
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_create_space(self, space_name):
         logger.log_debug('Creating space {} ...'.format(space_name))
         start = time.time()
         space_props = None
         if not self._is_icp:
             space_props = {
                     self._client.spaces.ConfigurationMetaNames.NAME: space_name,
@@ -78,15 +77,15 @@
                 if state == "error":
                     raise Exception("Space creation failed with error. Status: {}".format(details["entity"]["status"]))
         elapsed = time.time() - start
         self._openscale_client.timer('WML create space completed', elapsed)
         logger.log_debug('Succesfully created space {} (id: {})'.format(space_name, space_id))
         return space_id
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_set_space(self, space_id, space_name):
         start = time.time()
         rc = self._client.set.default_space(space_id)
         elapsed = time.time() - start
         if not rc == 'SUCCESS':
             error_msg = 'ERROR: WML set.default_space failed for space {} (id: {}) {}'.format(space_name, space_id, rc)
             logger.log_error(error_msg)
@@ -115,14 +114,59 @@
             if space_name == space['entity']['name']:
                 space_id = space['metadata']['id']
                 break
         if not space_id:
             space_id = self._reliable_create_space(space_name=space_name)
         self._reliable_set_space(space_id, space_name)
 
+    def check_space_for_delete(self, space_name:str) -> bool:
+        """
+        Checks whether a space is supposed to be deleted or not.
+
+        :space_name: The name of the space to be checked
+
+        :returns: Boolean flag indicating whether the space should be deleted or not.
+        """
+        delete_space = False
+        if(space_name.startswith('openscale-express-path') and self._openscale_client.get_datamart_id() in space_name):
+            delete_space = True
+        return delete_space
+
+    def list_and_delete_spaces(self) -> None:
+        """
+        Lists out all the present spaces and deletes the space created by FastPath.
+
+        :returns: None.
+        """
+        attempt = 0
+        start = time.time()
+        try:
+            logger.log_info("Listing out present spaces ...")
+            spaces = self._client.spaces.get_details()
+            for space in spaces['resources']:
+                space_name = space['entity']['name']
+                space_id = space['metadata']['id']
+                if self.check_space_for_delete(space_name):
+                    attempt+=1
+                    logger.log_info("Deleting space with id: {} ...".format(space_id))
+                    self._client.spaces.delete(space_id)
+                    logger.log_info("Waiting 10 seconds for space cleanup")
+                    time.sleep(10)
+            if attempt==0:
+                logger.log_info("No spaces to be deleted found ...")
+            else:
+                logger.log_info("Deleted spaces ...")
+        except Exception as e:
+            logger.log_exception(e)
+            raise e
+        elapsed = time.time() - start
+        logger.log_timer('space.delete in {:.3f} seconds'.format(elapsed))
+        logger.log_info('Spaces deleted successfully')
+        return 
+
     def _create_pipeline(self, model_name, pipeline_metadata_file):
         logger.log_info('Creating pipeline for model {} ...'.format(self._model_metadata['model_name']))
         pipeline_metadata = jsonFileToDict(pipeline_metadata_file)
         pipeline_props = {
             self._client.repository.DefinitionMetaNames.AUTHOR_NAME: pipeline_metadata['author']['name'],
             self._client.repository.DefinitionMetaNames.NAME: pipeline_metadata['name'],
             self._client.repository.DefinitionMetaNames.FRAMEWORK_NAME: pipeline_metadata['framework']['name'],
@@ -176,15 +220,15 @@
                     self._reliable_delete_model(model_guid)
                     logger.log_info('Model deleted successfully')
                 except Exception as e:
                     logger.log_warning('Error deleting WML deployment "{}": {}'.format(model_guid, str(e)))
         if not found_model:
             logger.log_info('No existing model found with name: {}'.format(model_name))
 
-    @retry(stop_max_attempt_number=2, wait_exponential_multiplier=2000)
+    # @retry(stop_max_attempt_number=2, wait_exponential_multiplier=2000)
     def _reliable_delete_model(self, model_guid):
         all_models = self._client.repository.get_model_details()
         all_functions = self._client.repository.get_function_details()
         for model in (all_models['resources'] + all_functions['resources']):
             if self._is_v4:
                 artifact_model_id = model['metadata']['id']
             else:
@@ -274,15 +318,15 @@
             model_guid = self._client.repository.get_model_id(model_details)
         logger.log_info('Created new model {} successfully (guid: {})'.format(model_name, model_guid))
         model_url = '{}{}?space_id={}&version=2020-06-22'.format(self._credentials['url'],
                                                                  self._client._models.get_href(model_details),
                                                                  self.space_id)
         return metadata, model_guid, model_url
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_create_model(self, model_file, model_props):
         start = time.time()
         try:
             if "type" in model_props and model_props["type"] == "python":
                 model_details = self._client.repository.store_function(model_file, model_props)
             else:
                 model_details = self._client.repository.store_model(model_file, model_props)
@@ -314,15 +358,15 @@
         elapsed_time, deployment_details = self._reliable_deploy_model(model_guid, deployment_name, deployment_description)
         if self._is_v4:
             deployment_guid = deployment_details['metadata']['id']
         deployment_url = deployment_details["entity"]["status"]["serving_urls"][0] if "serving_urls" in deployment_details["entity"]["status"] else deployment_details["entity"]["status"]["online_url"]["url"]
         logger.log_info('Created new deployment {} (guid: {}) successfully in {} seconds'.format(deployment_name, deployment_guid, round(elapsed_time, 2)))
         return deployment_guid, deployment_url
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_deploy_model(self, model_guid, deployment_name, deployment_description):
         start = time.time()
         deployment_details = None
         if self._is_v4:
             meta_props = {
                 self._client.deployments.ConfigurationMetaNames.NAME: deployment_name,
                 self._client.deployments.ConfigurationMetaNames.DESCRIPTION: deployment_description,
@@ -331,15 +375,15 @@
             deployment_details = self._client.deployments.create(artifact_uid=model_guid, meta_props=meta_props)
         else:
             deployment_details = self._client.deployments.create(artifact_uid=model_guid, name=deployment_name, description=deployment_description)
         elapsed = time.time() - start
         self._openscale_client.timer('WML deployments.create', elapsed)
         return elapsed, deployment_details
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_delete_deployment(self, deployment_guid):
         all_deployments = self._client.deployments.get_details()
         for deployment in all_deployments['resources']:
             if self._is_v4:
                 artifact_deployment_id = deployment['metadata']['id']
             else:
                 artifact_deployment_id = deployment['metadata']['guid']
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlservice/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/history_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/azuremlstudio/history_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/history_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/custom/history_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/feedback_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/feedback_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_fairness.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_fairness.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_quality_monitor.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/history_quality_monitor.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/feedback_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/feedback_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_fairness.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_fairness.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/history_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data_statistics.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/sagemaker/training_data_statistics.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/configuration.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/configuration.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/history_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/spss/history_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data_statistics.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/training_data_statistics.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/4.7/baseline.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_archives/4.7/baseline.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_history_measurements_payload_per_run.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_history_measurements_payload_per_run.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_insights_record_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_insights_record_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_intervals_record_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_intervals_record_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_baseline_record_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_baseline_record_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_production_record_payloads.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/drift_v2_stats_production_record_payloads.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/4.7/explainability.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/4.7/explainability.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/public_cloud/explainability.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/explain_archives/public_cloud/explainability.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/feedback_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/feedback_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debias.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debias.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_0.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_0.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_1.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_1.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_2.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_2.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_3.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_3.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_4.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_4.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_5.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_5.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_6.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_debiased_payloads_6.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_explanations.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_explanations.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_fairness.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_fairness.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_manual_labeling.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_manual_labeling.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_mhm.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_mhm.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_0.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_0.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_1.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_1.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_2.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_2.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_3.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_3.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_4.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_4.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_5.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_5.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_6.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_payloads_6.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_performance.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/history_performance.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/4.7/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/4.7/baseline.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/drift_v2_archives/4.7/baseline.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/4.7/explainability.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/4.7/explainability.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/public_cloud/explainability.tar.gz` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/explain_archives/public_cloud/explainability.tar.gz`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/mrm_evaluation_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/mrm_evaluation_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.10/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.7/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.8/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/py_3.9/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data_statistics.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm/training_data_statistics.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm_evaluation_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/mrm_evaluation_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/scoring_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/scoring_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data.csv` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data.csv`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data_statistics.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/training_data_statistics.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v3/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_2.4/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.0/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.2/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_content.gzip` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_content.gzip`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_meta.json` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/GermanCreditRiskModel/wml/v4/spark_3.3/model_meta.json`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/models/model.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/models/model.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/openscale/openscale.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/openscale/openscale.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,68 +19,74 @@
 
 class OpenScale:
 
     DEFAULT_DATAMART_SCHEMA_NAME = 'wosfastpath'
 
     def __init__(self, args, credentials, database_credentials, ml_engine_credentials):
         self._args = args
+        self._header = {"origin":"cli://fastpath"}
         self._credentials = credentials
         self._keep_schema = self._args.keep_schema
         self._verify = False if self._args.is_icp else True
         self.timers = dict()
         self._database_credentials = database_credentials
         self._ml_engine_credentials = ml_engine_credentials
         self._database = self._get_database()
         start = time.time()
         wos_instance_id = args.datamart_id if args.datamart_id else None
         if not self._args.is_icp:
             if self._args.apikey:
                 self._client = APIClient(
                     authenticator=IAMAuthenticator(apikey=credentials['apikey'], url=self._args.env_dict['iam_url']),
                     service_url=credentials['url'],
-                    service_instance_id=wos_instance_id
+                    service_instance_id=wos_instance_id,
+                    header=self._header
                 )
             elif self._args.iam_token:
                 self._client = APIClient(
                     authenticator=BearerTokenAuthenticator(bearer_token=self._args.iam_token),
                     service_url=credentials['url'],
-                    service_instance_id=wos_instance_id
+                    service_instance_id=wos_instance_id,
+                    header=self._header
                 )
         else:
             if self._args.password:
                 self._client = APIClient(
                     authenticator=CloudPakForDataAuthenticator(
                         username=self._args.username,
                         password=self._args.password,
                         url=self._args.url,
                         disable_ssl_verification=True,
                     ),
                     service_url=credentials['url'],
                     service_instance_id=wos_instance_id,
-                    bedrock_url=self._args.bedrock_url
+                    bedrock_url=self._args.bedrock_url,
+                    header=self._header
                 )
             elif self._args.iam_token:
                 self._client = APIClient(
                     authenticator=BearerTokenAuthenticator(
                         bearer_token=self._args.iam_token
                     ),
                     service_url=credentials['url'],
-                    service_instance_id=wos_instance_id
+                    service_instance_id=wos_instance_id,
+                    header=self._header
                 )
             elif self._args.apikey:
                 self._client = APIClient(
                     authenticator=CloudPakForDataAuthenticator(
                         username=self._args.username,
                         apikey=self._args.apikey,
                         url=self._args.url,
                         disable_ssl_verification=True,
                     ),
                     service_url=credentials["url"],
                     service_instance_id=wos_instance_id,
-                    bedrock_url=self._args.bedrock_url
+                    bedrock_url=self._args.bedrock_url,
+                    header=self._header
                 )
         elapsed = time.time() - start
         self._datamart_name = self._get_datamart_name()
         logger.log_info('Using {} Python Client version: {}'.format(self._args.service_name, self._client.version))
         self.timer('connect to APIClient', elapsed)
 
     def get_datamart_id(self):
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/openscale/openscale_client.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/openscale/openscale_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         self._explainability_run_once = True
         self._use_bkpi = False
         self._configure_explain = True
 
     def set_cos_credentials(self, _cos_credentials):
         self._cos_credentials = _cos_credentials
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_get_or_create_bucket(self, _cos_instance):
         bucket = _cos_instance.get_wos_bucket()
         if not bucket:
             bucket = _cos_instance.create_wos_bucket()
         return bucket.name
 
     def perform_cos_operations(self, _cos_instance):
@@ -145,19 +145,19 @@
         if self._database is None:
             logger.log_info('PostgreSQL instance: internal')
         else:
             self._reliable_create_schema()
         self._reliable_create_datamart()
         logger.log_info('Datamart {} created successfully'.format(self._datamart_name))
 
-    @retry(stop_max_attempt_number=3, wait_exponential_multiplier=5000)
+    # @retry(stop_max_attempt_number=3, wait_exponential_multiplier=5000)
     def _reliable_create_schema(self):
         self._database.create_new_schema(self._datamart_name, self._keep_schema)
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_create_datamart(self):
         start = time.time()
         if self._database is None:
             self._client.data_marts.add(name=self._datamart_name, internal_database=True, background_mode=False)
         else:
             db_config_request = None
             if self._database_credentials['db_type'] == 'postgresql':
@@ -226,15 +226,15 @@
                     )
             except Exception as e:
                 raise Exception("Failed while creating datamart with the specified database instance: {}".format(str(e)))
 
         elapsed = time.time() - start
         self.timer('data_mart.setup', elapsed)
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_bind_mlinstance(self, credentials, ml_engine=None, is_mrm_preprod=False):
         # if self._args.ml_engine_type is MLEngineType.WML:
         #     if self._args.is_icp:
         #         if 'apikey' in credentials:
         #             ml_instance = WMLCredentialsCloud(credentials)
         #             binding_name = 'IBM Cloud {}'.format(binding_name)
         #         else:
@@ -256,93 +256,98 @@
         # elif self._args.ml_engine_type is MLEngineType.CUSTOM:
         #     ml_instance = CustomCredentials(credentials)
         # elif self._args.ml_engine_type is MLEngineType.SAGEMAKER:
         #     ml_instance = SageMakerCredentials(credentials)
 
 
         start = time.time()
-        if not self._args.is_icp:
-            bindings_url = "{}/openscale/{}/v2/service_providers".format(self._credentials['url'], self._credentials['data_mart_id'])
-
-            logger.log_info("Not using ML Instance information in the add service provider call ...")
-            if is_mrm_preprod:
-                operational_space_id = OPERATIONAL_PRE_PRODUCTION_SPACE_ID
-            else:
-                operational_space_id = OPERATIONAL_PRODUCTION_SPACE_ID
-            payload = {
-                "name": SERVICE_PROVIDER_NAME.format(operational_space_id),
-                "description": "WML Instance designated as {}".format(operational_space_id),
-                "service_type": "watson_machine_learning",
-                "credentials": {},
-                "operational_space_id": operational_space_id,
-                "deployment_space_id": ml_engine.space_id
-            }
-
-            binding_details = requests.post(bindings_url, json=payload, headers=self.iam_headers, verify=self._verify).json()
-            if is_mrm_preprod:
-                self._binding_id_mrm_preprod = binding_details["metadata"]["id"]
-            else:
-                self._binding_id = binding_details["metadata"]["id"]
-
-            binding_details = requests.get(bindings_url, headers=self.iam_headers, verify=self._verify).json()
+        try:
+            if not self._args.is_icp:
+                logger.log_info("Not using ML Instance information in the add service provider call ...")
+                if is_mrm_preprod:
+                    operational_space_id = OPERATIONAL_PRE_PRODUCTION_SPACE_ID
+                else:
+                    operational_space_id = OPERATIONAL_PRODUCTION_SPACE_ID
 
-            if 'entity' in binding_details:
-                if 'status' in binding_details['entity']:
-                    if 'state' in binding_details['entity']['status']:
-                        for i in range(12):
-                            # binding_details = self._client.service_providers.get(self._binding_id).get_result()
-                            binding_details = requests.get(bindings_url, headers=self.iam_headers, verify=self._verify).json()
-                            service_providers = binding_details['service_providers']
-                            for sp in service_providers:
-                                if sp['metadata']['id'] == self._binding_id:
-                                    state = sp["entity"]["status"]["state"]
-                                    _msg = "Service provider status = {}".format(state)
-                                    if state == "active":
-                                        logger.log_info(_msg)
-                                        break
-                                    if state == "error":
-                                        logger.log_info(_msg)
-                                        raise Exception("Service provider add failed.")
-                                    else:
-                                        _msg = _msg + ', rechecking in 5 seconds ...'
-                                        logger.log_info(_msg)
-                                        time.sleep(5)
-                            if state == "active":
-                                _msg = "Service provider status = {}".format(state)
-                                break
+                binding_details = self._client.service_providers.add(
+                    name=SERVICE_PROVIDER_NAME.format(operational_space_id),
+                    description="WML Instance designated as {}".format(operational_space_id),
+                    service_type="watson_machine_learning",
+                    credentials={},
+                    operational_space_id=operational_space_id,
+                    deployment_space_id=ml_engine.space_id,
+                    request_headers=self.iam_headers,
+                    background_mode=True
+                ).result
+
+                binding_id = binding_details.metadata.id
+                if is_mrm_preprod:
+                    self._binding_id_mrm_preprod = binding_id
+                else:
+                    self._binding_id = binding_id
+                
+                binding_details = self._client.service_providers.get(binding_id, headers=self.iam_headers, verify=self._verify).get_result()
+                state = binding_details.entity.status.state
+                _msg = "Service provider status = {} for service provider with id = {}...".format(state, binding_id)
+                logger.log_info(_msg)
+                
+                total_sleep_time = 120
+                sleep_interval = 5
+                sleep_time = 0
+                while state not in ["active", "error"]:
+                    if(sleep_time>=total_sleep_time):
+                        error_msg="Service provider with id: {} did not turn active within {} seconds...".format(binding_id, total_sleep_time)
+                        logger.log_error(error_msg)
+                        raise Exception(error_msg)
+                    _msg = "Service provider status = {} for service provider with id = {}, rechecking in {} seconds ...".format(state, binding_id, sleep_interval)
+                    logger.log_info(_msg)
+                    time.sleep(sleep_interval)
+                    sleep_time += sleep_interval
+                    binding_details = self._client.service_providers.get(binding_id, headers=self.iam_headers, verify=self._verify).get_result()
+                    state = binding_details.entity.status.state
+                    
+                if state == "error":
+                    error_msg = "Failed to add service provider with id: {}...\n{}".format(binding_id, str(binding_details.entity.status.failure.errors))
+                    logger.log_error(error_msg)
+                    raise Exception(error_msg)
 
-            logger.log_info('Waiting 15 seconds for the binding to be complete ...')
-            time.sleep(15)
+                logger.log_info('Waiting 15 seconds for the binding to be complete ...')
+                time.sleep(15)
 
-            elapsed = time.time() - start
-            logger.log_info('Binding {} created successfully'.format(self.get_binding_id()))
-        else:
-            wml_service_provider_creds = WMLCredentialsCP4D.from_dict({})
-            if is_mrm_preprod:
-                operational_space_id = OPERATIONAL_PRE_PRODUCTION_SPACE_ID
-            else:
-                operational_space_id = OPERATIONAL_PRODUCTION_SPACE_ID
-            service_provider_result = self._client.service_providers.add(
-                name=SERVICE_PROVIDER_NAME.format(operational_space_id),
-                description="Service Provider added by OpenScale Express Path",
-                service_type=ServiceTypes.WATSON_MACHINE_LEARNING,
-                credentials=wml_service_provider_creds,
-                operational_space_id=operational_space_id,
-                deployment_space_id=ml_engine.space_id,
-                background_mode=False
-            ).result
-            this_binding_id = service_provider_result.metadata.id
-            if is_mrm_preprod:
-                self._binding_id_mrm_preprod = this_binding_id
+                elapsed = time.time() - start
+                logger.log_info('Binding {} created successfully'.format(binding_id))
             else:
-                self._binding_id = this_binding_id
-            elapsed = time.time() - start
-            logger.log_info('Binding {} {} created successfully'.format(operational_space_id, this_binding_id))
+                wml_service_provider_creds = WMLCredentialsCP4D.from_dict({})
+                if is_mrm_preprod:
+                    operational_space_id = OPERATIONAL_PRE_PRODUCTION_SPACE_ID
+                else:
+                    operational_space_id = OPERATIONAL_PRODUCTION_SPACE_ID
+                service_provider_result = self._client.service_providers.add(
+                    name=SERVICE_PROVIDER_NAME.format(operational_space_id),
+                    description="Service Provider added by OpenScale Express Path",
+                    service_type=ServiceTypes.WATSON_MACHINE_LEARNING,
+                    credentials=wml_service_provider_creds,
+                    operational_space_id=operational_space_id,
+                    deployment_space_id=ml_engine.space_id,
+                    background_mode=False
+                ).result
+                this_binding_id = service_provider_result.metadata.id
+                if is_mrm_preprod:
+                    self._binding_id_mrm_preprod = this_binding_id
+                else:
+                    self._binding_id = this_binding_id
+                elapsed = time.time() - start
+                logger.log_info('Binding {} {} created successfully'.format(operational_space_id, this_binding_id))
+
+            self.timer('data_mart.bindings.add', elapsed)
 
-        self.timer('data_mart.bindings.add', elapsed)
+        except Exception as e:
+            error_msg = 'ERROR: Failed to bind {} ml instance : {}'.format("pre prod" if is_mrm_preprod else "prod", e)
+            logger.log_error(err_msg=error_msg)
+            raise Exception(error_msg)
 
     def bind_mlinstance(self, credentials, ml_engine_prod=None, ml_engine_preprod=None):
         logger.log_info('Binding {} instance to {} ...'.format(self._args.ml_engine_type.name.lower(), self._args.service_name))
         self._reliable_bind_mlinstance(credentials, ml_engine_prod, is_mrm_preprod=False)
         if self._args.mrm:
             self._reliable_bind_mlinstance(credentials, ml_engine_preprod, is_mrm_preprod=True)
 
@@ -356,15 +361,15 @@
                     self._binding_id = provider_id
                 elif provider_name == SERVICE_PROVIDER_NAME.format(OPERATIONAL_PRE_PRODUCTION_SPACE_ID):
                     self._binding_id_mrm_preprod = provider_id
         else:
             self._binding_id = asset_details_dict["binding_uid"]
         logger.log_info("Use existing binding {}".format(self.get_binding_id()))
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def use_existing_subscription(self, asset_details_dict):
         self._asset_details_dict = asset_details_dict
         asset_uid = asset_details_dict['source_uid']
         deployment_uid = asset_details_dict['source_entry_metadata_guid']
         logger.log_info('Get existing subscription for model {} deployment {}...'.format(asset_uid, deployment_uid))
         start = time.time()
         all_subscriptions = self._client.subscriptions.list().result.subscriptions
@@ -388,15 +393,15 @@
                                         target_target_type=TargetTypes.SUBSCRIPTION
                                     ).result.data_sets[0].metadata.id
         elapsed = time.time() - start
         self._model.expected_payload_row_count = self._reliable_count_payload_rows('use existing subscription')
         logger.log_info('Subscription {} found successfully'.format(self.get_subscription_id()))
         self._reliable_count_datamart_rows('use existing subscription')
 
-    @retry(stop_max_attempt_number=1, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=1, wait_exponential_multiplier=4000)
     def subscribe_to_model_deployment(self, asset_details_dict):
         '''
         Create subscription for the given model
         '''
         logger.log_info('Subscribing ML deployment to {} ...'.format(self._args.service_name))
         self._reliable_count_datamart_rows('create subscription start')
         asset_metadata = self._model.configuration_data['asset_metadata']
@@ -552,15 +557,15 @@
         elif data == 'MULTICLASS_CLASSIFICATION':
             return ProblemType.MULTICLASS_CLASSIFICATION
         elif data == 'REGRESSION':
             return ProblemType.REGRESSION
         return None
 
     # not actually called, because payload logging and performance monitoring are both already enabled by default
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
     def configure_subscription(self):
         '''
         Configure payload logging and performance monitoring
         '''
         logger.log_info('Enabling payload logging ...')
         start = time.time()
         self._subscription.payload_logging.enable()
@@ -640,35 +645,15 @@
                 "min_records": params["min_records"],
                 "training_data_distributions": self._model.training_data_statistics["fairness_configuration"]["parameters"]["training_data_distributions"]
             }
             target = Target(
                 target_type=TargetTypes.SUBSCRIPTION,
                 target_id=self._subscription_id
             )
-            thresholds = []
-            for feature in params["features"]:
-                thresholds.append(
-                    {
-                        "metric_id": "fairness_value",
-                        "specific_values": [
-                            {
-                                "applies_to": [
-                                    {
-                                        "type": "tag",
-                                        "value": feature["feature"],
-                                        "key": "feature"
-                                    }
-                                ],
-                                "value": int(feature["threshold"] * 100)
-                            }
-                        ],
-                        "type": "lower_limit",
-                        "value": int(feature["threshold"] * 100)
-                    }
-                )
+            thresholds = params["thresholds"]
             fairness_monitor_details = self._client.monitor_instances.create(
                 data_mart_id=self._credentials['data_mart_id'],
                 background_mode=True,
                 monitor_definition_id=self._client.monitor_definitions.MONITORS.FAIRNESS.ID,
                 target=target,
                 parameters=parameters,
                 thresholds=thresholds
@@ -685,21 +670,15 @@
         if params:
             start = time.time()
             target = Target(
                 target_type=TargetTypes.SUBSCRIPTION,
                 target_id=self._subscription_id
             )
             parameters = {"min_feedback_data_size": params["min_records"]}
-            thresholds = [
-                {
-                    "metric_id": "area_under_roc",
-                    "type": "lower_limit",
-                    "value": params["threshold"]
-                }
-            ]
+            thresholds = params["thresholds"]
             quality_monitor_details = self._client.monitor_instances.create(
                 data_mart_id=self._credentials["data_mart_id"],
                 background_mode=True,
                 monitor_definition_id=self._client.monitor_definitions.MONITORS.QUALITY.ID,
                 target=target,
                 parameters=parameters,
                 thresholds=thresholds
@@ -791,15 +770,15 @@
         url = "{}/v1/fairness_monitoring/heartbeat".format(service_url)
 
         payload = {}
         headers = {
             "Accept": "application/json"
         }
 
-        response = requests.get(url, headers=headers, data=payload, verify=False)
+        response = requests.get(url, headers=headers, data=payload, verify=True)
 
         if response.ok is False:
             error_msg = "ERROR: Failed to get the fairness heartbeat, url: {}, rc: {}, response: {}".format(url, response.status_code, response.text)
             logger.log_error(error_msg)
             raise Exception(error_msg)
 
         return response.json()
@@ -821,60 +800,57 @@
         else:
             self.mrm_prod_instance_id = response.result.metadata.id
         self.timer('subscription.mrm.enable', elapsed)
 
         # for the preprod model, mark it as approved for production
         if self.is_mrm_preprod and self.mrm_preprod_instance_id:
             payload = {'state': 'approved'}
-            mrm_url = '{}/openscale/{}/v2/subscriptions/{}/risk_evaluation_status'.format(self._credentials['url'], self._credentials['data_mart_id'], self.get_subscription_id())
             start = time.time()
-            response = requests.put(mrm_url, json=payload, headers=self.iam_headers, verify=self._verify)
+            response = self._client.monitor_instances.mrm.mrm_update_risk_evaluation_status(subscription_id=self.get_subscription_id(), state="approved", headers=self.iam_headers)
             elapsed = time.time() - start
             if response.status_code != 200:
-                error_msg = 'ERROR: Failed to approve pre-prod model, rc: {} url: {} payload: {} response: {}'.format(response.status_code, mrm_url, payload, response.text)
+                error_msg = 'ERROR: Failed to approve pre-prod model, rc: {} method: {} payload: {} response: {}'.format(response.status_code, "monitor_instances.mrm.mrm_update_risk_evaluation_status()", payload, response.get_result())
                 logger.log_error(error_msg)
                 raise Exception(error_msg)
             self.timer('subscription.mrm approve preprod', elapsed)
 
         # for the prod model, link it back to the preprod model
         if self.is_mrm_prod and self.mrm_preprod_subscription_id:
             payload = [{ "op": "add", "path": "/pre_production_reference_id", "value": self.mrm_preprod_subscription_id }]
-            mrm_url = '{}/openscale/{}/v2/subscriptions/{}'.format(self._credentials['url'], self._credentials['data_mart_id'], self.get_subscription_id())
             start = time.time()
-            response = requests.patch(mrm_url, json=payload, headers=self.iam_headers, verify=self._verify)
+            response = self._client.subscriptions.update(self.get_subscription_id(), patch_document=payload, headers=self.iam_headers)
             elapsed = time.time() - start
             if response.status_code != 200:
-                error_msg = 'ERROR: Failed to patch subscription with pre-prod reference, rc: {} url: {} payload: {} response: {}'.format(response.status_code, mrm_url, payload, response.text)
+                error_msg = 'ERROR: Failed to patch subscription with pre-prod reference, rc: {} method: {} payload: {} response: {}'.format(response.status_code, "subscriptions.update()", payload, response.get_result())
                 logger.log_error(error_msg)
                 raise Exception(error_msg)
             self.timer('subscription.mrm patch prod', elapsed)
 
         logger.log_info('MRM configured successfully')
     
     def upload_drift_v2_archive(self, file_path: str) -> None:
         """
         Uploads the Drift_V2 baseline archive for the given subscription.
         :file_path: The file_path of the baseline archive.
 
         :returns: None.
         """
 
-        url = "{}/openscale/{}/v2/monitoring_services/drift_v2/archives?archive_name={}&subscription_id={}".format(self._client.service_url.split("/openscale")[0], self.get_datamart_id(), Model.DRIFT_V2_ARCHIVE_FILENAME, self.get_subscription_id())
 
         payload = open(file_path, "rb")
         token = self._args.iam_token if self._args.iam_token else self._client.authenticator.token_manager.get_token()
         headers = {
             "Authorization": "bearer {}".format(token),
             "Content-Type": "application/octet-stream"
         }
 
-        response = requests.request("PUT", url, headers=headers, data=payload, verify=False)
+        response = self._client.monitor_instances.drift_v2.upload_drift_v2_archive(subscription_id=self.get_subscription_id(), body=payload, archive_name= Model.DRIFT_V2_ARCHIVE_FILENAME, headers=headers)
 
-        if not response.ok:
-            error_msg = "ERROR: Failed to upload drift_v2 baseline archive, url: {}, rc: {}, response: {}".format(url, response.status_code, response.text)
+        if response.status_code != 200:
+            error_msg = "ERROR: Failed to upload drift_v2 baseline archive, method: {}, rc: {}, response: {}".format("monitor_instances.drift_v2.upload_drift_v2_archive()", response.status_code, response.get_result())
             logger.log_error(error_msg)
             raise Exception(error_msg)
 
         return
     
     def configure_drift_v2(self, params: dict) -> None:
         """
@@ -1132,15 +1108,15 @@
                 )
                 patch_documents.append(patch_document)
             if len(patch_documents) > 0:
                 response = records_client.patch(data_set_id=self._payload_dataset_id, patch_document=patch_documents)
             if (day + 1) == self._args.history:
                 logger.log_info('Historical manual labeling data loaded successfully')
     
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_store_fairness_monitor_metrics(self, records):
         '''
         Retry the loading metrics so that if a specific day fails, just retry that day, rather than retry the whole sequence
         '''
         if not records:
             logger.log_debug('No fairness_monitor history provided to load - skipping')
             return
@@ -1331,15 +1307,15 @@
                             request_body=production_records,
                             background_mode=False
                         )
                 logger.log_info('Historical drift_v2 metrics generated successfully.')
         
         return
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=8000)
     def _reliable_upload_feedback(self, feedback_data):
         start = time.time()
         if self._model.is_unstructured_text:
             self._subscription.feedback_logging.store(feedback_data)
         else:
             self._feedback_dataset_id = self._client.data_sets.list(
                 type=DataSetTypes.FEEDBACK,
@@ -1352,15 +1328,15 @@
                 self._feedback_dataset_id,
                 request_body=feedback_data,
                 background_mode=False
             ).result.to_dict()
         elapsed = time.time() - start
         self.timer('subscription.feedback_logging.store', elapsed)
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_single_score(self, engine_client, deployment_url, score_input, score_num, values_per_score, totalelapsed, firststart, lastend, tokenizer=None):
         record = None
         start = time.time()
         if self._args.v4:
             deployment_id = self._asset_details_dict['source_entry_metadata_guid']
             if 'fields' in score_input:
                 record = engine_client.score(deployment_id, values=score_input['values'], fields=score_input['fields'])
@@ -1550,27 +1526,27 @@
         if to_init_payload_logging:
             context = 'init payload logging'
         else:
             context = 'live scoring'
         self.wait_for_payload_logging(context=context, to_init_payload_logging=to_init_payload_logging)
         self._reliable_count_datamart_rows('generated sample scores and confirmed payload logging')
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_count_payload_rows(self, context=None):
         start = time.time()
         actual_payload_rows = self._client.data_sets.get_records_count(data_set_id = self._payload_dataset_id)
         elapsed = time.time() - start
         if context:
             context = ', {}'.format(context)
         else:
             context = ''
         logger.log_timer('subscription count payload rows in {:.3f} seconds, rows={}, expected={}{}'.format(elapsed, actual_payload_rows, self._model.expected_payload_row_count, context))
         return actual_payload_rows
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_count_datamart_rows(self, context=None):
         if self._database is None: # internal db
             logger.log_debug('DEBUG: cannot count datamart rows for internal db')
             if self._args.database_counts:
                 logger.log_info('Cannot count datamart rows for internal db - skipping')
             return
         start = time.time()
@@ -1648,15 +1624,15 @@
             monitor_instance_id=self._drift_v2_monitor_instance_id,
             triggered_by="user",
             background_mode=True
         )
 
         return
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_fairness_check(self, background_mode):
         if 'fairness_configuration' not in self._model.configuration_data:
             logger.log_info('Skip fairness check since fairness not configured for model')
         else:
             try:
                 deployment_uid = self._asset_details_dict['source_entry_metadata_guid']
                 logger.log_info('Triggering immediate fairness check ...')
@@ -1669,15 +1645,15 @@
                     if not result or (isinstance(result, str) and 'error' in result.lower()) or result.entity.status.state.lower() != 'finished':
                         self.metric_check_errors.append([self._model.name, 'fairness-check', 'failed'])
             except Exception as e:
                 message = 'WARNING: Problems occurred while running fairness check: {}'.format(str(e))
                 logger.log_warning(message)
                 self.metric_check_errors.append([self._model.name, 'fairness-check', 'failed'])
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_quality_check(self, background_mode):
         if 'quality_configuration' not in self._model.configuration_data:
             logger.log_info('Skip quality check since quality monitoring not configured for model')
         elif (not self._model.feedback_data or self._args.no_new_feedback) and (not self._model.feedback_history or self._args.history < 1):
             logger.log_info('Skip quality check for model since there is no feedback data yet')
         else:
             try:
@@ -1691,15 +1667,15 @@
                     if not result or (isinstance(result, str) and 'error' in result.lower()) or result.entity.status.state.lower() != 'finished':
                         self.metric_check_errors.append([self._model.name, 'quality-check', 'failed'])
             except Exception as e:
                 message = 'WARNING: Problems occurred while running quality check: {}'.format(str(e))
                 logger.log_warning(message)
                 self.metric_check_errors.append([self._model.name, 'quality-check', 'failed'])
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_drift_check(self, background_mode):
         if 'drift_configuration' not in self._model.configuration_data:
             logger.log_info('Skip drift check since drift monitoring not configured for model')
         else:
             try:
                 logger.log_info('Triggering immediate drift check ...')
                 start = time.time()
@@ -1710,47 +1686,45 @@
                 if not result or (isinstance(result, str) and 'error' in result.lower()):
                     self.metric_check_errors.append([self._model.name, 'drift-check', 'failed'])
             except Exception as e:
                 message = 'WARNING: Problems occurred while running drift check: {}'.format(str(e))
                 logger.log_warning(message)
                 self.metric_check_errors.append([self._model.name, 'drift-check', 'failed'])
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_mrm_prod_check(self, mrm_instance_id, background_mode):
-        mrm_url = '{}/openscale/{}/v2/monitor_instances/{}/runs'.format(self._credentials['url'], self._credentials['data_mart_id'], mrm_instance_id)
-        payload = {
+        params = {
             "parameters": {
                 "publish_fact": "true",
                 "on_demand_trigger": True
-            },
-            "triggered_by": "user"
+            }
         }
 
         # trigger the MRM check
         start = time.time()
-        response = requests.post(url=mrm_url, json=payload, headers=self.iam_headers, verify=self._verify)
+        response = self._client.monitor_instances.runs.add(monitor_instance_id=mrm_instance_id, triggered_by="user", parameters=params, headers=self.iam_headers)
         elapsed = time.time() - start
         self.timer('trigger mrm prod check', elapsed)
 
         # check to see if the call was successful
         if response.status_code != 201 and response.status_code != 202:
-            error_msg = 'ERROR: Failed to trigger MRM check, url: {}, rc: {}, response: {}'.format(mrm_url, response.status_code, response.text)
+            error_msg = 'ERROR: Failed to trigger MRM check, method: {}, rc: {}, response: {}'.format("monitor_instances.runs.add()", response.status_code, response.get_result())
             logger.log_error(error_msg)
             raise Exception(error_msg)
         mrm_run_id = None
-        json_data = response.json()
-        if "metadata" in json_data and "id" in json_data["metadata"]:
-            mrm_run_id = json_data["metadata"]["id"]
+        json_data = response.result
+        if json_data.metadata and json_data.metadata.id:
+            mrm_run_id = json_data.metadata.id
         else:
-            error_msg = 'ERROR: Failed to trigger MRM check, url: {}, rc: {}, response: {}'.format(mrm_url, response.status_code, response.text)
+            error_msg = 'ERROR: Failed to trigger MRM check, method: {}, rc: {}, response: {}'.format("monitor_instances.runs.add()", response.status_code, response.get_result())
             logger.log_error(error_msg)
             raise Exception(error_msg)
         return mrm_run_id
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_trigger_mrm_preprod_check(self, mrm_instance_id, background_mode):
         if self.is_mrm_challenger:
             filename = 'test_data_challenger.csv'
         else:
             filename = 'test_data_preprod.csv'
         mrm_url = '{}/openscale/{}/v2/monitoring_services/mrm/monitor_instances/{}/risk_evaluations?test_data_set_name={}'.format(self._credentials['url'], self._credentials['data_mart_id'], mrm_instance_id, filename)
         payload = self._model.mrm_evaluation_data
@@ -1764,31 +1738,30 @@
 
         # check to see if the call was successful
         if response.status_code != 201 and response.status_code != 202:
             error_msg = 'ERROR: Failed to trigger MRM check, url: {}, rc: {}, response: {}'.format(mrm_url, response.status_code, response.text)
             logger.log_error(error_msg)
             raise Exception(error_msg)
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_get_mrm_check_status(self, mrm_instance_id, mrm_run_id=None):
         # different URLs to check MRM run status between prod and pre-prod (PreProd or Challenger)
+        start = time.time()
         if self.is_mrm_prod:
-            results_url = '{}/openscale/{}/v2/monitor_instances/{}/runs/{}'.format(self._credentials['url'], self._credentials['data_mart_id'], mrm_instance_id, mrm_run_id)
+            response = self._client.monitor_instances.runs.get(monitor_instance_id=mrm_instance_id, monitoring_run_id=mrm_run_id, headers=self.iam_headers)
         else:
-            results_url = '{}/openscale/{}/v2/monitoring_services/mrm/monitor_instances/{}/risk_evaluations'.format(self._credentials['url'], self._credentials['data_mart_id'], mrm_instance_id)
-        start = time.time()
-        response = requests.get(url=results_url, headers=self.iam_headers, verify=self._verify)
+            response = self._client.monitor_instances.mrm.get_risk_evaluation(monitor_instance_id=mrm_instance_id, headers=self.iam_headers)
         elapsed = time.time() - start
         if response.status_code != 200:
-            error_msg = 'ERROR: Failed to get MRM check status, rc: {} {}'.format(response.status_code, response.text)
+            error_msg = 'ERROR: Failed to get MRM check status, rc: {} {}'.format(response.status_code, response.get_result())
             raise Exception(error_msg)
-        state = response.json()['entity']['status']['state']
+        state = response.result.entity.status.state
         logger.log_debug('MRM check status: {}'.format(state))
         if state == 'error':
-            error_msg = 'ERROR: MRM check failed: {}'.format(response.text)
+            error_msg = 'ERROR: MRM check failed: {}'.format(response.get_result())
             raise Exception(error_msg)
         self.timer('get mrm monitoring.run', elapsed)
         return response
 
     def trigger_mrm_check(self, background_mode):
         if 'mrm_configuration' not in self._model.configuration_data:
             logger.log_info('Skip mrm check since MRM not configured for model')
@@ -1811,43 +1784,43 @@
             return
         logger.log_info('MRM check running ...')
 
         try:
             check_completed = False
             for i in range(18):
                 response = self._reliable_get_mrm_check_status(mrm_instance_id, mrm_run_id)
-                state = response.json()['entity']['status']['state'].lower()
+                state = response.result.entity.status.state.lower()
                 if state != 'running' and state != 'upload_in_progress':
                     check_completed = True
                     break
                 logger.log_info('MRM check still running; wait 10 seconds and check again')
                 time.sleep(10)
             if check_completed:
                 logger.log_info('MRM check completed')
             else:
                 logger.log_info('MRM check did not complete in 3 minutes, continuing')
         except Exception as e:
             message = 'WARNING: Problems occurred while running MRM check: {}'.format(str(e))
             logger.log_warning(message)
             self.metric_check_errors.append([self._model.name, 'mrm-check', 'failed'])
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_post_payloads(self, records):
         '''
         Retry the loading payloads so that if a specific day fails, just retry that day, rather than retry the whole sequence
         '''
         if not records:
             logger.log_debug('No payload history provided to load - skipping')
             return
         start = time.time()
         self._client.data_sets.store_records(data_set_id=self._payload_dataset_id, request_body=records)
         elapsed = time.time() - start
         self.timer('subscription.payload_logging.store', elapsed)
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_post_debiased_payloads(self, records):
         """
         Retry the loading so that if a specific day fails, just retry that day, rather than retry the whole sequence
         """
         if not records:
             logger.log_debug('No debiased payloads history provided to load - skipping')
             return
@@ -1884,15 +1857,15 @@
 
         elapsed = time.time() - start
         self.timer('post data_mart debiased payloads history', elapsed)
 
         if response.status_code < 200 or response.status_code > 299:
             logger.log_warning('WARNING: while posting debiased payloads history: {}'.format(str(response.result.to_dict())))
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def _reliable_store_quality_monitor_metrics(self, records):
         '''
         Retry the loading metrics so that if a specific day fails, just retry that day, rather than retry the whole sequence
         '''
         if not records:
             logger.log_debug('No quality_monitor history provided to load - skipping')
             return
@@ -1920,15 +1893,15 @@
                 break
         if not 'source_uid' in asset_details_dict:
             error_msg = 'ERROR: Could not find a deployment with the name: {}'.format(name)
             logger.log_error(error_msg)
             raise Exception(error_msg)
         return asset_details_dict
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=1000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=1000)
     def _get_explanation_status(self, scoring_id, background_mode):
         cem = not self._args.explain_no_cem
         logger.log_info("Starting explain request for scoring id: {}".format(scoring_id))
         start = time.time()
         subscription_id = self.get_subscription_id()
         explain = self._client.monitor_instances.get_explanation_tasks(explanation_task_id=scoring_id, subscription_id=subscription_id).result.to_dict()
         status = explain['entity']['status']['state']
@@ -1963,15 +1936,15 @@
             scoring_ids = [payload_table["records"][i]["entity"]["values"]["scoring_id"] for i in range(min(max_explain_candidates, num_records))]
             random.shuffle(scoring_ids)
             return start, end, scoring_ids
         except Exception as e:
             logger.log_warning('WARNING: Problems occurred while getting scoring ids for explanation: {}'.format(str(e)))
         return None, None, None
     
-    @retry(stop_max_attempt_number=3, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=3, wait_exponential_multiplier=4000)
     def generate_explain_requests(self):
         # no explains for an MRM pre-production model
         if self._args.mrm and not self.is_mrm_prod:
             return
         num_explains = self._args.num_explains
         if num_explains < 1:
             return
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/openscale/openscale_reset.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/openscale/openscale_reset.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 import os
 import time
 from retrying import retry
 
 from ibm_ai_openscale_cli.enums import ResetType
 from ibm_ai_openscale_cli.openscale.openscale import OpenScale
 from ibm_ai_openscale_cli.utility_classes.fastpath_logger import FastpathLogger
+from ibm_ai_openscale_cli.credentials import Credentials
+
+from ibm_ai_openscale_cli.ml_engines.watson_machine_learning import WatsonMachineLearningEngine
 
 logger = FastpathLogger(__name__)
 parent_dir = os.path.dirname(__file__)
 
 DATAMART_MAX_DELETION_ATTEMPTS = 10
 
 
@@ -27,42 +30,48 @@
     def filter(self, record):
         return not record.getMessage().startswith('Failure during delete of data mart')
 
 
 class OpenScaleReset(OpenScale):
 
     def __init__(self, args, credentials, database_credentials, ml_engine_credentials):
+        self._args = args
+        self._credentials_obj = Credentials(args)
         super().__init__(args, credentials, database_credentials, ml_engine_credentials)
 
     def reset(self, reset_type):
         if reset_type is ResetType.METRICS:
             self.reset_metrics()
         elif reset_type is ResetType.MONITORS:
             self.reset_metrics()
             self.reset_monitors()
         # "factory reset" the system
         elif reset_type is ResetType.DATAMART:
             self.delete_datamart()
             self.clean_database()
+        elif reset_type is ResetType.ALL:
+            self.delete_datamart()
+            self.clean_database()
+            self.delete_spaces()
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def reset_metrics(self):
         '''
         Clean up the payload logging table, monitoring history tables etc, so that it restores the system
         to a fresh state with datamart configured, model deployments added, all monitors configured,
         but no actual metrics in the system yet. The system is ready to go.
         '''
         if self._database is None:
             logger.log_info('Internal database metrics cannot be reset - skipping')
         else:
             logger.log_info('Deleting datamart metrics ...')
             self._database.reset_metrics_tables(self._datamart_name)
             logger.log_info('Datamart metrics deleted successfully')
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def reset_monitors(self):
         '''
         Remove all configured monitors and corresponding metrics and history, but leave the actual model deployments
         (if any) in the datamart. User can proceed to configure the monitors via user interface, API, or fastpath.
         '''
         logger.log_info('Deleting datamart monitors ...')
         subscription_uids = self._client.data_mart.subscriptions.get_uids()
@@ -101,15 +110,15 @@
         if self._database is None:
             logger.log_info('Internal database monitor-related tables cannot be deleted - skipping')
         else:
             logger.log_info('Deleting datamart monitor-related tables ...')
             self._database.drop_metrics_tables(self._datamart_name)
             logger.log_info('Datamart monitor-related tables deleted successfully')
 
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def delete_datamart(self):
         attempt = 0
         added_filter = False
         try:
             start = time.time()
             while attempt < DATAMART_MAX_DELETION_ATTEMPTS:  # Wait until exception is thrown to confirm datamart is completely deleted
                 if attempt == 1:
@@ -155,15 +164,25 @@
                 else:
                     logger.log_info('Confirmed datamart deletion')
             else:
                 raise e
         if added_filter:
             logger.logger.removeFilter(NonExistingDatamartDeleteErrorFilter())
     
-    @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
+    # @retry(stop_max_attempt_number=5, wait_exponential_multiplier=4000)
     def clean_database(self):
         if self._database is None:
             logger.log_info('Internal database instance cannot be deleted - skipping')
         else:
             logger.log_info('Cleaning database ...')
             self._database.drop_existing_schema(self._datamart_name, self._keep_schema)
             logger.log_info('Database cleaned successfully')
+
+    def delete_spaces(self) -> None:
+        """
+        Deletes spaces created for fast-path.
+
+        :returns: None.
+        """
+        wml_client = WatsonMachineLearningEngine(self._ml_engine_credentials, super(), self._credentials_obj._cos_credentials)
+        wml_client.list_and_delete_spaces()
+        return
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/openscale_ops.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/openscale_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,166 +93,170 @@
 
     def use_existing_binding_if_extending_datamart(self, openscale_client, asset_details_dict):
         if self._args.extend and self.run_once:
             self.run_once = False
             openscale_client.use_existing_binding(asset_details_dict)
 
     def execute(self):
+        try:
 
-        # validations
-        self._model_validations()
+            # validations
+            self._model_validations()
 
-        # credentials
-        openscale_client = self._instantiate_openscale_client()
+            # credentials
+            openscale_client = self._instantiate_openscale_client()
 
-        self._validate_datamart_reset(openscale_client)
+            self._validate_datamart_reset(openscale_client)
 
-        # Instantiate ml engine
-        """
-        if not self._args.is_icp:
-            if not self._args.is_icp and self._args.v4:
-                if self._args.ml_engine_type is MLEngineType.WML:
-                    self._cos_credentials, self._cos_instance = self.get_cos_instance()
-                    openscale_client.set_cos_credentials(self._cos_credentials)
-        """
-        ml_engine_prod = self.get_ml_engine_instance(openscale_client)
-
-        ml_engine_preprod = None
-        if self._args.mrm:
-            ml_engine_preprod = self.get_ml_engine_instance(openscale_client, self._args.mrm)
-
-        # reset datamart
-        self._reset_datamart(openscale_client)
-        if self._args.mrm:
-            self._bind_ml_instance(openscale_client, ml_engine_prod, ml_engine_preprod)
-        else:
-            self._bind_ml_instance(openscale_client, ml_engine_prod)
-
-        modeldata = None
-        first = True
-        for modelname in self._model_names:
-            openscale_client.is_mrm_challenger = False
-            openscale_client.is_mrm_preprod = False
-            openscale_client.is_mrm_prod = False
-            if self._args.mrm:
-                if 'challenger' in modelname.lower():
-                    ml_engine = ml_engine_preprod
-                    openscale_client.is_mrm_challenger = True
-                elif 'preprod' in modelname.lower():
-                    ml_engine = ml_engine_preprod
-                    openscale_client.is_mrm_preprod = True
-                else:
-                    ml_engine = ml_engine_prod
-                    openscale_client.is_mrm_prod = True
-            else:
-                ml_engine = ml_engine_prod
-            logger.log_info_h1('Model: {}, Engine: {}'.format(modelname, self._args.ml_engine_type.value))
-            for model_instance_num in range(self._args.model_first_instance, self._args.model_first_instance + self._args.model_instances):
-                if self._args.model_instances > 1:
-                    logger.log_info('Model instance {}'.format(model_instance_num))
-                if not first and self._args.pause_between_models > 0:
-                    logger.log_info('Pause for {:.3f} seconds before starting this model'.format(self._args.pause_between_models))
-                    time.sleep(self._args.pause_between_models)
-                first = False
-
-                # get the iam headers that will be used for all REST API calls for this model
-                openscale_client.set_iam_headers()
-
-                # model instance
-                modeldata = self.get_modeldata_instance(modelname, model_instance_num)
-                openscale_client.set_model(modeldata)
-                """
-                if not self._args.is_icp and self._args.v4:  # Cloud WML V4, COS is needed
+            # Instantiate ml engine
+            """
+            if not self._args.is_icp:
+                if not self._args.is_icp and self._args.v4:
                     if self._args.ml_engine_type is MLEngineType.WML:
-                        openscale_client.perform_cos_operations(self._cos_instance)
-                """
+                        self._cos_credentials, self._cos_instance = self.get_cos_instance()
+                        openscale_client.set_cos_credentials(self._cos_credentials)
+            """
+            ml_engine_prod = self.get_ml_engine_instance(openscale_client)
 
-                if self._args.values_per_score > 1 and (openscale_client.is_unstructured_text() or openscale_client.is_unstructured_image()):
-                    self._args.num_scores = self._args.values_per_score * self._args.num_scores
-                    self._args.values_per_score = 1
-                    logger.log_info('FYI: This model only supports 1 value per score request. Continuing with each value in its own score request')
+            ml_engine_preprod = None
+            if self._args.mrm:
+                ml_engine_preprod = self.get_ml_engine_instance(openscale_client, self._args.mrm)
 
+            # reset datamart
+            self._reset_datamart(openscale_client)
+            if self._args.mrm:
+                self._bind_ml_instance(openscale_client, ml_engine_prod, ml_engine_preprod)
+            else:
+                self._bind_ml_instance(openscale_client, ml_engine_prod)
 
-                asset_details_dict = None
-                # ml engine instance
-                if self._args.ml_engine_type is MLEngineType.WML:
-                    ml_engine.set_model(modeldata)
-                    if not self._args.deployment_name:
-                        asset_details_dict = ml_engine.create_model_and_deploy()
+            modeldata = None
+            first = True
+            for modelname in self._model_names:
+                openscale_client.is_mrm_challenger = False
+                openscale_client.is_mrm_preprod = False
+                openscale_client.is_mrm_prod = False
+                if self._args.mrm:
+                    if 'challenger' in modelname.lower():
+                        ml_engine = ml_engine_preprod
+                        openscale_client.is_mrm_challenger = True
+                    elif 'preprod' in modelname.lower():
+                        ml_engine = ml_engine_preprod
+                        openscale_client.is_mrm_preprod = True
                     else:
-                        asset_details_dict = ml_engine.get_existing_deployment(self._args.deployment_name)
+                        ml_engine = ml_engine_prod
+                        openscale_client.is_mrm_prod = True
                 else:
-                    asset_details_dict = openscale_client.get_asset_details(self._args.deployment_name)
+                    ml_engine = ml_engine_prod
+                logger.log_info_h1('Model: {}, Engine: {}'.format(modelname, self._args.ml_engine_type.value))
+                for model_instance_num in range(self._args.model_first_instance, self._args.model_first_instance + self._args.model_instances):
+                    if self._args.model_instances > 1:
+                        logger.log_info('Model instance {}'.format(model_instance_num))
+                    if not first and self._args.pause_between_models > 0:
+                        logger.log_info('Pause for {:.3f} seconds before starting this model'.format(self._args.pause_between_models))
+                        time.sleep(self._args.pause_between_models)
+                    first = False
+
+                    # get the iam headers that will be used for all REST API calls for this model
+                    openscale_client.set_iam_headers()
+
+                    # model instance
+                    modeldata = self.get_modeldata_instance(modelname, model_instance_num)
+                    openscale_client.set_model(modeldata)
+                    """
+                    if not self._args.is_icp and self._args.v4:  # Cloud WML V4, COS is needed
+                        if self._args.ml_engine_type is MLEngineType.WML:
+                            openscale_client.perform_cos_operations(self._cos_instance)
+                    """
+
+                    if self._args.values_per_score > 1 and (openscale_client.is_unstructured_text() or openscale_client.is_unstructured_image()):
+                        self._args.num_scores = self._args.values_per_score * self._args.num_scores
+                        self._args.values_per_score = 1
+                        logger.log_info('FYI: This model only supports 1 value per score request. Continuing with each value in its own score request')
 
-                self.use_existing_binding_if_extending_datamart(openscale_client, asset_details_dict)
 
-                # ai openscale operations
-                if self._args.history_only:
-                    openscale_client.use_existing_subscription(asset_details_dict)
-                else:
-                    openscale_client.subscribe_to_model_deployment(asset_details_dict)
-                    openscale_client.generate_sample_scoring(ml_engine, numscores=1, values_per_score=1, to_init_payload_logging=True)
-                    openscale_client.configure_subscription_monitors()
-
-                if self._args.subscription_details != 'none':
-                    openscale_client.save_subscription_details()
-                if openscale_client.generate_sample_metrics():
-                    openscale_client.load_historical_payloads()
-                    openscale_client.load_historical_fairness()
-                    openscale_client.load_historical_quality()
-                    openscale_client.confirm_payload_logging()
-                    openscale_client.load_historical_debiased_payloads()
-                    openscale_client.load_historical_drift_v2()
-                    openscale_client.load_historical_performance()
-                    openscale_client.load_historical_mhm()
-                    # Skip loading historic explanations in the case of CLI run
-                    # Tracker: 24375
-                    #openscale_client.load_historical_explanations()
-                
-                openscale_client.generate_sample_scoring(ml_engine, numscores=self._args.num_scores, values_per_score=self._args.values_per_score)
-                openscale_client.trigger_monitors()
-                openscale_client.generate_explain_requests()
-
-        if self._args.summary:
-            try:
-                from tabulate import tabulate
-            except ModuleNotFoundError as e:
-                logger.log_info('Module "tabulate" not found, attempting to install ...')
-                from ibm_ai_openscale_cli.utility_classes.utils import pip_install
-                pip_install('tabulate')
-            length_errors = len(openscale_client.metric_check_errors)
-            if length_errors > 1:
-                summary_title = tabulate([tabulate([['Summary:']])])
-                table_headers = openscale_client.metric_check_errors[0]
-                table_rows = openscale_client.metric_check_errors[1:length_errors]
-                summary_table = tabulate(table_rows, headers=table_headers)
-                logger.log_info('\n' * 3)
-                logger.log_info(summary_title)
-                logger.log_info('')
-                logger.log_info(summary_table)
-                logger.log_info('')
-
-            if len(list(openscale_client.timers)) > 0 or len(list(self.timers)) > 0:
-                summary_title = tabulate([tabulate([['Timers:']])])
-                table_headers = ['tag', 'count', 'seconds', 'average']
-                table_rows = []
-                total_count = 0
-                total_seconds = 0
-                for tag in list(openscale_client.timers):
-                    total_count += openscale_client.timers[tag]['count']
-                    total_seconds += openscale_client.timers[tag]['seconds']
-                    average = openscale_client.timers[tag]['seconds'] / openscale_client.timers[tag]['count']
-                    table_rows.append([tag, openscale_client.timers[tag]['count'], openscale_client.timers[tag]['seconds'], average])
-                for tag in list(self.timers):
-                    total_count += self.timers[tag]['count']
-                    total_seconds += self.timers[tag]['seconds']
-                    average = self.timers[tag]['seconds'] / self.timers[tag]['count']
-                    table_rows.append([tag, self.timers[tag]['count'], self.timers[tag]['seconds'], average])
-                table_rows.sort(key=lambda item: item[0])
-                table_rows.append(['TOTAL', total_count, total_seconds])
-                summary_table = tabulate(table_rows, headers=table_headers)
-                logger.log_info('\n' * 3)
-                logger.log_info(summary_title)
-                logger.log_info('')
-                logger.log_info(summary_table)
-                logger.log_info('')
+                    asset_details_dict = None
+                    # ml engine instance
+                    if self._args.ml_engine_type is MLEngineType.WML:
+                        ml_engine.set_model(modeldata)
+                        if not self._args.deployment_name:
+                            asset_details_dict = ml_engine.create_model_and_deploy()
+                        else:
+                            asset_details_dict = ml_engine.get_existing_deployment(self._args.deployment_name)
+                    else:
+                        asset_details_dict = openscale_client.get_asset_details(self._args.deployment_name)
+
+                    self.use_existing_binding_if_extending_datamart(openscale_client, asset_details_dict)
 
+                    # ai openscale operations
+                    if self._args.history_only:
+                        openscale_client.use_existing_subscription(asset_details_dict)
+                    else:
+                        openscale_client.subscribe_to_model_deployment(asset_details_dict)
+                        openscale_client.generate_sample_scoring(ml_engine, numscores=1, values_per_score=1, to_init_payload_logging=True)
+                        openscale_client.configure_subscription_monitors()
+
+                    if self._args.subscription_details != 'none':
+                        openscale_client.save_subscription_details()
+                    if openscale_client.generate_sample_metrics():
+                        openscale_client.load_historical_payloads()
+                        openscale_client.load_historical_fairness()
+                        openscale_client.load_historical_quality()
+                        openscale_client.confirm_payload_logging()
+                        openscale_client.load_historical_debiased_payloads()
+                        openscale_client.load_historical_drift_v2()
+                        openscale_client.load_historical_performance()
+                        openscale_client.load_historical_mhm()
+                        # Skip loading historic explanations in the case of CLI run
+                        # Tracker: 24375
+                        #openscale_client.load_historical_explanations()
+                    
+                    openscale_client.generate_sample_scoring(ml_engine, numscores=self._args.num_scores, values_per_score=self._args.values_per_score)
+                    openscale_client.trigger_monitors()
+                    openscale_client.generate_explain_requests()
+
+            if self._args.summary:
+                try:
+                    from tabulate import tabulate
+                except ModuleNotFoundError as e:
+                    logger.log_info('Module "tabulate" not found, attempting to install ...')
+                    from ibm_ai_openscale_cli.utility_classes.utils import pip_install
+                    pip_install('tabulate')
+                length_errors = len(openscale_client.metric_check_errors)
+                if length_errors > 1:
+                    summary_title = tabulate([tabulate([['Summary:']])])
+                    table_headers = openscale_client.metric_check_errors[0]
+                    table_rows = openscale_client.metric_check_errors[1:length_errors]
+                    summary_table = tabulate(table_rows, headers=table_headers)
+                    logger.log_info('\n' * 3)
+                    logger.log_info(summary_title)
+                    logger.log_info('')
+                    logger.log_info(summary_table)
+                    logger.log_info('')
+
+                if len(list(openscale_client.timers)) > 0 or len(list(self.timers)) > 0:
+                    summary_title = tabulate([tabulate([['Timers:']])])
+                    table_headers = ['tag', 'count', 'seconds', 'average']
+                    table_rows = []
+                    total_count = 0
+                    total_seconds = 0
+                    for tag in list(openscale_client.timers):
+                        total_count += openscale_client.timers[tag]['count']
+                        total_seconds += openscale_client.timers[tag]['seconds']
+                        average = openscale_client.timers[tag]['seconds'] / openscale_client.timers[tag]['count']
+                        table_rows.append([tag, openscale_client.timers[tag]['count'], openscale_client.timers[tag]['seconds'], average])
+                    for tag in list(self.timers):
+                        total_count += self.timers[tag]['count']
+                        total_seconds += self.timers[tag]['seconds']
+                        average = self.timers[tag]['seconds'] / self.timers[tag]['count']
+                        table_rows.append([tag, self.timers[tag]['count'], self.timers[tag]['seconds'], average])
+                    table_rows.sort(key=lambda item: item[0])
+                    table_rows.append(['TOTAL', total_count, total_seconds])
+                    summary_table = tabulate(table_rows, headers=table_headers)
+                    logger.log_info('\n' * 3)
+                    logger.log_info(summary_title)
+                    logger.log_info('')
+                    logger.log_info(summary_table)
+                    logger.log_info('')
+                    
+        except Exception as e:
+            logger.log_error(e)
+            raise Exception(e)
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/ops.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,11 +135,13 @@
             self._args.environment = Environment.CPD_4_0_8_PLUS.value
         elif fairness_version.startswith("4.5.0"):
             self._args.environment = Environment.CPD_4_5.value
         elif fairness_version.startswith(("4.5.1", "4.5.2")):
             self._args.environment = Environment.CPD_4_5_1_PLUS.value
         elif fairness_version.startswith(("4.5", "4.6")):
             self._args.environment = Environment.CPD_4_5_3_PLUS.value
-        else:
+        elif fairness_version.startswith(("4.7", "4.8.0", "4.8.1", "4.8.2", "4.8.3")):
             self._args.environment = Environment.CPD_4_7_PLUS.value
+        else:
+            self._args.environment = Environment.CPD_4_8_4_PLUS.value
 
         return
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/reset_ops.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/reset_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,18 +38,22 @@
             self._reset_one_model(modelname, ml_engine)
         if self._args.mrm:
             ml_engine = self.get_ml_engine_instance(self._openscale_client, self._args.mrm)
             for modelname in ['GermanCreditRiskModelPreProd', 'GermanCreditRiskModelChallenger']:
                 self._reset_one_model(modelname, ml_engine)
 
     def _reset_openscale(self, reset_type):
-        if reset_type == ResetType.ALL:
-            self._openscale_client.reset(ResetType.DATAMART)
-        else:
-            self._openscale_client.reset(reset_type)
+        # if reset_type == ResetType.ALL:
+        #     self._openscale_client.reset(ResetType.DATAMART)
+        # else:
+        self._openscale_client.reset(reset_type)
 
     def execute(self):
-        if self._args.reset_type is not ResetType.MODEL:
+        if self._args.reset_type is ResetType.ALL and self._args.ml_engine_type is MLEngineType.WML:
             self._reset_openscale(self._args.reset_type)
-
-        if (self._args.reset_type is ResetType.MODEL or self._args.reset_type is ResetType.ALL) and self._args.ml_engine_type is MLEngineType.WML:
+        elif self._args.reset_type is not ResetType.MODEL:
+            if self._args.reset_type is ResetType.ALL:
+                self._reset_openscale(ResetType.DATAMART)
+            else:
+                self._reset_openscale(self._args.reset_type)
+        elif self._args.reset_type is ResetType.MODEL and self._args.ml_engine_type is MLEngineType.WML:
             self._reset_model()
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/cloud_foundry.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/cloud_foundry.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/cloud_foundry_cli.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/cloud_foundry_cli.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/resource_controller.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/resource_controller.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/resource_controller_cli.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/resource_controller_cli.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_cli.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_cli.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_rest.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_ibmcloud_services_rest.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_ibmcloudprivate_services.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_ibmcloudprivate_services.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/setup_services.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/setup_services.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/setup_classes/token_manager.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/setup_classes/token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/constants.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,74 +20,81 @@
     Environment.CPD_4_0_0.value: "spark_2.4",
     Environment.CPD_4_0_1.value: "spark_2.4",
     Environment.CPD_4_0_2_PLUS.value: "spark_3.0",
     Environment.CPD_4_0_8_PLUS.value: "spark_3.0",
     Environment.CPD_4_5.value: "spark_3.0",
     Environment.CPD_4_5_1_PLUS.value: "spark_3.2",
     Environment.CPD_4_5_3_PLUS.value: "spark_3.3",
-    Environment.CPD_4_7_PLUS.value: "spark_3.3"
+    Environment.CPD_4_7_PLUS.value: "spark_3.3",
+    Environment.CPD_4_8_4_PLUS.value: "spark_3.3"
 }
 
 # Stored the environment to use for the Challenger model
 WML_CHALLENGER_ENVIRONMENT_MAPPING = {
     Environment.PUBLIC_CLOUD.value: "py_3.10",
     Environment.CPD_3_X.value: "py_3.7",
     Environment.CPD_4_0_0.value: "py_3.7",
     Environment.CPD_4_0_1.value: "py_3.7",
     Environment.CPD_4_0_2_PLUS.value: "py_3.7",
     Environment.CPD_4_0_8_PLUS.value: "py_3.9",
     Environment.CPD_4_5.value: "py_3.9",
     Environment.CPD_4_5_1_PLUS.value: "py_3.9",
     Environment.CPD_4_5_3_PLUS.value: "py_3.10",
-    Environment.CPD_4_7_PLUS.value: "4.7"
+    Environment.CPD_4_7_PLUS.value: "4.7",
+    Environment.CPD_4_8_4_PLUS.value: "4.7"
 }
 WML_CHALLENGER_ENVIRONMENT_MAPPING_ZLINUX = {
     Environment.PUBLIC_CLOUD.value: "py_3.10",
     Environment.CPD_3_X.value: "py_3.7",
     Environment.CPD_4_0_0.value: "py_3.7",
     Environment.CPD_4_0_1.value: "py_3.7",
     Environment.CPD_4_0_2_PLUS.value: "py_3.7",
     Environment.CPD_4_0_8_PLUS.value: "py_3.9",
     Environment.CPD_4_5.value: "py_3.9",
     Environment.CPD_4_5_1_PLUS.value: "py_3.9",
     Environment.CPD_4_5_3_PLUS.value: "py_3.10",
-    Environment.CPD_4_7_PLUS.value: "py_3.10"
+    Environment.CPD_4_7_PLUS.value: "py_3.10",
+    Environment.CPD_4_8_4_PLUS.value: "py_3.10"
 }
 
 # Software spec mapping for the challenger model
 WML_CHALLENGER_SOFTWARE_SPEC_MAPPING = {
-    Environment.PUBLIC_CLOUD.value: "runtime-22.2-py3.10",
+    Environment.PUBLIC_CLOUD.value: "runtime-23.1-py3.10",
     Environment.CPD_3_X.value: "default_py3.7",
     Environment.CPD_4_0_0.value: "default_py3.7",
     Environment.CPD_4_0_1.value: "default_py3.7",
     Environment.CPD_4_0_2_PLUS.value: "default_py3.7_opence",
     Environment.CPD_4_0_8_PLUS.value: "runtime-22.1-py3.9",
     Environment.CPD_4_5.value: "runtime-22.1-py3.9",
     Environment.CPD_4_5_1_PLUS.value: "runtime-22.1-py3.9",
     Environment.CPD_4_5_3_PLUS.value: "runtime-22.2-py3.10",
-    Environment.CPD_4_7_PLUS.value: "runtime-23.1-py3.10"
+    Environment.CPD_4_7_PLUS.value: "runtime-23.1-py3.10",
+    Environment.CPD_4_8_4_PLUS.value: "runtime-23.1-py3.10"
 }
 
 WML_CHALLENGER_SOFTWARE_SPEC_MAPPING_ZLINUX = {
-    Environment.PUBLIC_CLOUD.value: "runtime-22.2-py3.10",
+    Environment.PUBLIC_CLOUD.value: "runtime-23.1-py3.10",
     Environment.CPD_3_X.value: "default_py3.7",
     Environment.CPD_4_0_0.value: "default_py3.7",
     Environment.CPD_4_0_1.value: "default_py3.7",
     Environment.CPD_4_0_2_PLUS.value: "default_py3.7_opence",
     Environment.CPD_4_0_8_PLUS.value: "runtime-22.1-py3.9",
     Environment.CPD_4_5.value: "runtime-22.1-py3.9",
     Environment.CPD_4_5_1_PLUS.value: "runtime-22.1-py3.9",
     Environment.CPD_4_5_3_PLUS.value: "runtime-22.2-py3.10",
-    Environment.CPD_4_7_PLUS.value: "runtime-22.2-py3.10"
+    Environment.CPD_4_7_PLUS.value: "runtime-22.2-py3.10",
+    Environment.CPD_4_8_4_PLUS.value: "runtime-23.1-py3.10"
 }
 
 # Stores the environment mapping to the Drift_V2 baseline archive folder
 DRIFT_V2_ARCHIVE_ENV_MAPPING = {
     Environment.PUBLIC_CLOUD.value: "public_cloud",
-    Environment.CPD_4_7_PLUS.value: "4.7"
+    Environment.CPD_4_7_PLUS.value: "4.7",
+    Environment.CPD_4_8_4_PLUS.value: "4.7"
 }
 
 # Stores the environment mapping to the explain configuration archive folder
 EXPLAIN_ARCHIVE_ENV_MAPPING = {
     Environment.PUBLIC_CLOUD.value: "public_cloud",
-    Environment.CPD_4_7_PLUS.value: "4.7"
+    Environment.CPD_4_7_PLUS.value: "4.7",
+    Environment.CPD_4_8_4_PLUS.value: "4.7"
 }
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/fastpath_logger.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/fastpath_logger.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/keras_unstructured_binary_text.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/keras_unstructured_binary_text.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/statistics_generator.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/statistics_generator.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/timer.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/timer.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_ai_openscale_cli/utility_classes/utils.py` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_ai_openscale_cli/utility_classes/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -162,7 +162,21 @@
 
 def load_pickle_file(pickle_file_path):
     # import pickle
     # with open(pickle_file_path, 'rb') as handle:
     #     return pickle.load(handle)
     pass
 
+def strtobool(val: str):
+    """
+    Convert a string representation of truth to true (1) or false (0).
+    True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
+    are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
+    'val' is anything else.
+    """
+    val = str(val).lower()
+    if val in ('y', 'yes', 't', 'true', 'on', '1'):
+        return 1
+    elif val in ('n', 'no', 'f', 'false', 'off', '0'):
+        return 0
+    else:
+        raise ValueError("invalid truth value %r" % (val,))
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/PKG-INFO` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-watson-openscale-cli-tool
-Version: 3.5.54
+Version: 3.5.55
 Summary: CLI library to automate the onboarding process to IBM Watson OpenScale
 Home-page: https://www.ibm.com/cloud/watson-openscale
 Author: IBM Corp
 Author-email: wps@us.ibm.com
 License: Apache-2.0
 Keywords: ai-openscale,ibm-watson
 Classifier: Programming Language :: Python
@@ -13,14 +13,26 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: h5py>=2.9.0
+Requires-Dist: requests<3.0,>=2.0
+Requires-Dist: urllib3==1.26.18
+Requires-Dist: retrying==1.3.3
+Requires-Dist: boto3==1.17.22
+Requires-Dist: psycopg2==2.8.6
+Requires-Dist: ibm-db>=3.0.3
+Requires-Dist: ibm-cloud-sdk-core==3.16.5
+Requires-Dist: ibm-watson-openscale>=3.0.32
+Requires-Dist: ibm-watson-machine-learning>=1.0.264
+Requires-Dist: pandas==1.3.5
+Requires-Dist: pyJWT==2.4.0
 
 # ibm-watson-openscale-cli
 ![Status](https://img.shields.io/badge/status-beta-yellow.svg)
 [![Latest Stable Version](https://img.shields.io/pypi/v/ibm-watson-openscale-cli.svg)](https://pypi.python.org/pypi/ibm-watson-openscale-cli-tool)
 
 IBM Watson Openscale "express path" configuration tool. This tool allows the user to get started quickly with Watson OpenScale.
 * If needed, automatically provision a Lite plan instance for IBM Watson OpenScale.
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/ibm_watson_openscale_cli_tool.egg-info/SOURCES.txt` & `ibm-watson-openscale-cli-tool-3.5.55/ibm_watson_openscale_cli_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/setup.py` & `ibm-watson-openscale-cli-tool-3.5.55/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,19 +61,19 @@
     description='CLI library to automate the onboarding process to IBM Watson OpenScale',
     license='Apache-2.0',
     python_requires='>=3.5',
     long_description_content_type='text/markdown',
     install_requires=[
         'h5py>=2.9.0',
         'requests>=2.0, <3.0',
-        'urllib3==1.26.12',
+        'urllib3==1.26.18',
         'retrying==1.3.3',
         'boto3==1.17.22',
         'psycopg2==2.8.6',
-        'ibm-db==3.0.3',
+        'ibm-db>=3.0.3',
         'ibm-cloud-sdk-core==3.16.5',
         'ibm-watson-openscale>=3.0.32',
         'ibm-watson-machine-learning>=1.0.264',
         'pandas==1.3.5',
         "pyJWT==2.4.0"
     ],
     dependency_links=[],
```

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_cloud_foundry.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_cloud_foundry.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_db2.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_db2.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_openscale.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_openscale.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_postgres.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_resource_controller.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_resource_controller.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_setup_ibmcloud_services.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_setup_ibmcloud_services.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_setup_ibmcloud_services_rest.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_setup_ibmcloud_services_rest.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_setup_ibmcloudprivate_services.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_setup_ibmcloudprivate_services.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_token_manager.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_utils.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-openscale-cli-tool-3.5.54/tests/test_watson_machine_learning.py` & `ibm-watson-openscale-cli-tool-3.5.55/tests/test_watson_machine_learning.py`

 * *Files identical despite different names*


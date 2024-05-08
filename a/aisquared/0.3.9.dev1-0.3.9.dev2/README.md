# Comparing `tmp/aisquared-0.3.9.dev1.tar.gz` & `tmp/aisquared-0.3.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisquared-0.3.9.dev1.tar", last modified: Fri Sep  8 16:23:31 2023, max compression
+gzip compressed data, was "aisquared-0.3.9.dev2.tar", last modified: Mon Sep 18 18:00:21 2023, max compression
```

## Comparing `aisquared-0.3.9.dev1.tar` & `aisquared-0.3.9.dev2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.921283 aisquared-0.3.9.dev1/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    20075 2023-09-08 16:23:31.920797 aisquared-0.3.9.dev1/PKG-INFO
--rw-r--r--   0 jwrenn4    (501) staff       (20)    19751 2023-09-08 16:22:26.000000 aisquared-0.3.9.dev1/README.md
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.889566 aisquared-0.3.9.dev1/aisquared/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      483 2023-09-08 16:22:26.000000 aisquared-0.3.9.dev1/aisquared/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.894134 aisquared-0.3.9.dev1/aisquared/base/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/base/BaseObject.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3132 2023-09-08 16:22:26.000000 aisquared-0.3.9.dev1/aisquared/base/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3474 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/base/css.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      581 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/base/endpoints.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      220 2023-02-24 19:53:35.000000 aisquared-0.3.9.dev1/aisquared/base/harvesting.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      119 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/base/platform.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      136 2023-02-24 19:53:35.000000 aisquared-0.3.9.dev1/aisquared/base/preprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      683 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev1/aisquared/base/rendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      169 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/base/stages.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.895688 aisquared-0.3.9.dev1/aisquared/config/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1406 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/config/CustomObject.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8948 2023-08-04 14:53:56.000000 aisquared-0.3.9.dev1/aisquared/config/GraphConfiguration.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    19309 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev1/aisquared/config/ModelConfiguration.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      451 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/config/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.897572 aisquared-0.3.9.dev1/aisquared/config/analytic/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3349 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev1/aisquared/config/analytic/DeployedAnalytic.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2226 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/analytic/DeployedModel.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1911 2023-02-20 18:21:49.000000 aisquared-0.3.9.dev1/aisquared/config/analytic/LocalAnalytic.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1446 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/analytic/LocalModel.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5569 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/analytic/ReverseMLWorkflow.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      316 2023-02-20 18:02:37.000000 aisquared-0.3.9.dev1/aisquared/config/analytic/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.899856 aisquared-0.3.9.dev1/aisquared/config/feedback/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1138 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/feedback/BinaryFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2771 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/feedback/ModelFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1131 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/feedback/MulticlassFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1921 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/feedback/QualitativeFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/feedback/RegressionFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      578 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/feedback/SimpleFeedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      395 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/feedback/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.901801 aisquared-0.3.9.dev1/aisquared/config/harvesting/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1287 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev1/aisquared/config/harvesting/ChatbotHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1100 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/harvesting/ImageHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3285 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev1/aisquared/config/harvesting/InputHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2620 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/harvesting/QueryParameterHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3510 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev1/aisquared/config/harvesting/TextHarvester.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      340 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev1/aisquared/config/harvesting/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.903485 aisquared-0.3.9.dev1/aisquared/config/postprocessing/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1995 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/postprocessing/BinaryClassification.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1499 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/postprocessing/MulticlassClassification.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1816 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/postprocessing/ObjectDetection.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2094 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/postprocessing/Regression.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      322 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/postprocessing/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.903764 aisquared-0.3.9.dev1/aisquared/config/preprocessing/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      357 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.904929 aisquared-0.3.9.dev1/aisquared/config/preprocessing/image/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1701 2023-08-04 14:53:56.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/image/ImagePreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8268 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/image/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      186 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/image/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.905979 aisquared-0.3.9.dev1/aisquared/config/preprocessing/tabular/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     8761 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/tabular/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1563 2023-08-04 14:53:56.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/tabular/TabularPreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      187 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/tabular/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.907060 aisquared-0.3.9.dev1/aisquared/config/preprocessing/text/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    11803 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/text/Steps.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1740 2023-08-04 14:53:56.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/text/TextPreprocessing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      175 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/preprocessing/text/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.912541 aisquared-0.3.9.dev1/aisquared/config/rendering/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5083 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/BarChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     6083 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/ContainerRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2212 2023-09-08 16:22:26.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/CustomRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     9187 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/DashboardRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1889 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/DashboardReplacementRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4829 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/DocumentRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5053 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/DoughnutChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2666 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/FilterRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3683 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/HTMLTagRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4940 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/ImageRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5036 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/LineChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3884 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/ObjectRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5068 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/PieChartRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1547 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/SOSRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2841 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/TableRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1320 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/TextRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     5031 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/WordRendering.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      987 2023-09-08 16:22:26.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      754 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/aisquared/config/rendering/utils.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.912794 aisquared-0.3.9.dev1/aisquared/logging/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      271 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/logging/__init__.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.915466 aisquared-0.3.9.dev1/aisquared/platform/
--rw-r--r--   0 jwrenn4    (501) staff       (20)       49 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/platform/AISquaredAPIException.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    46109 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/platform/AISquaredPlatformClient.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)       47 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/platform/NoResultsFoundError.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      375 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/platform/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      666 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/platform/additional_utils.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3539 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/platform/crudl.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3335 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/platform/feedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     2287 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/platform/metrics.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3224 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/platform/sharing.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    13405 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/platform/user_group.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.916162 aisquared-0.3.9.dev1/aisquared/serving/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1323 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/serving/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4929 2023-03-31 18:41:55.000000 aisquared-0.3.9.dev1/aisquared/serving/deploy_model.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1587 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/serving/get_remote_prediction.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.916717 aisquared-0.3.9.dev1/aisquared/utils/
--rw-r--r--   0 jwrenn4    (501) staff       (20)      459 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/aisquared/utils/__init__.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    10636 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/aisquared/utils/utils.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.890886 aisquared-0.3.9.dev1/aisquared.egg-info/
--rw-r--r--   0 jwrenn4    (501) staff       (20)    20075 2023-09-08 16:23:31.000000 aisquared-0.3.9.dev1/aisquared.egg-info/PKG-INFO
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3869 2023-09-08 16:23:31.000000 aisquared-0.3.9.dev1/aisquared.egg-info/SOURCES.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)        1 2023-09-08 16:23:31.000000 aisquared-0.3.9.dev1/aisquared.egg-info/dependency_links.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)      101 2023-09-08 16:23:31.000000 aisquared-0.3.9.dev1/aisquared.egg-info/requires.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)       10 2023-09-08 16:23:31.000000 aisquared-0.3.9.dev1/aisquared.egg-info/top_level.txt
--rw-r--r--   0 jwrenn4    (501) staff       (20)       38 2023-09-08 16:23:31.921357 aisquared-0.3.9.dev1/setup.cfg
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1422 2023-02-24 19:53:35.000000 aisquared-0.3.9.dev1/setup.py
-drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-08 16:23:31.920307 aisquared-0.3.9.dev1/tests/
--rw-r--r--   0 jwrenn4    (501) staff       (20)     4332 2023-08-04 14:53:57.000000 aisquared-0.3.9.dev1/tests/test_air.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1070 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/tests/test_analytics.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      958 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/tests/test_base.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      341 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev1/tests/test_custom.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3578 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/tests/test_feedback.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     3790 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev1/tests/test_harvesters.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1345 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev1/tests/test_postprocessors.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)     1980 2023-07-24 12:12:58.000000 aisquared-0.3.9.dev1/tests/test_preprocessors.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)    22740 2023-09-08 16:22:26.000000 aisquared-0.3.9.dev1/tests/test_renderers.py
--rw-r--r--   0 jwrenn4    (501) staff       (20)      107 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev1/tests/test_simple.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.966535 aisquared-0.3.9.dev2/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    20526 2023-09-18 18:00:21.966170 aisquared-0.3.9.dev2/PKG-INFO
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19824 2023-09-18 17:59:21.000000 aisquared-0.3.9.dev2/README.md
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.942793 aisquared-0.3.9.dev2/aisquared/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      483 2023-09-18 17:58:35.000000 aisquared-0.3.9.dev2/aisquared/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.946298 aisquared-0.3.9.dev2/aisquared/base/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/base/BaseObject.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3163 2023-09-18 17:56:53.000000 aisquared-0.3.9.dev2/aisquared/base/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3474 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/base/css.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      581 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/base/endpoints.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      220 2023-02-24 19:53:35.000000 aisquared-0.3.9.dev2/aisquared/base/harvesting.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      119 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/base/platform.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      136 2023-02-24 19:53:35.000000 aisquared-0.3.9.dev2/aisquared/base/preprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      683 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev2/aisquared/base/rendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      169 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/base/stages.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.947704 aisquared-0.3.9.dev2/aisquared/config/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1406 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/config/CustomObject.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8948 2023-08-04 14:53:56.000000 aisquared-0.3.9.dev2/aisquared/config/GraphConfiguration.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    19309 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev2/aisquared/config/ModelConfiguration.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      451 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/config/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.949302 aisquared-0.3.9.dev2/aisquared/config/analytic/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3349 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev2/aisquared/config/analytic/DeployedAnalytic.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2226 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/analytic/DeployedModel.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1911 2023-02-20 18:21:49.000000 aisquared-0.3.9.dev2/aisquared/config/analytic/LocalAnalytic.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1446 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/analytic/LocalModel.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5569 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/analytic/ReverseMLWorkflow.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      316 2023-02-20 18:02:37.000000 aisquared-0.3.9.dev2/aisquared/config/analytic/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.950789 aisquared-0.3.9.dev2/aisquared/config/feedback/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1138 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/feedback/BinaryFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2771 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/feedback/ModelFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1131 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/feedback/MulticlassFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1921 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/feedback/QualitativeFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      565 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/feedback/RegressionFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      578 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/feedback/SimpleFeedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      395 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/feedback/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.952099 aisquared-0.3.9.dev2/aisquared/config/harvesting/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1287 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev2/aisquared/config/harvesting/ChatbotHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1100 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/harvesting/ImageHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3285 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev2/aisquared/config/harvesting/InputHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2620 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/harvesting/QueryParameterHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3510 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev2/aisquared/config/harvesting/TextHarvester.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      340 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev2/aisquared/config/harvesting/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.953122 aisquared-0.3.9.dev2/aisquared/config/postprocessing/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1995 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/postprocessing/BinaryClassification.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1499 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/postprocessing/MulticlassClassification.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1816 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/postprocessing/ObjectDetection.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2094 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/postprocessing/Regression.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      322 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/postprocessing/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.953321 aisquared-0.3.9.dev2/aisquared/config/preprocessing/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      357 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.953929 aisquared-0.3.9.dev2/aisquared/config/preprocessing/image/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1701 2023-08-04 14:53:56.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/image/ImagePreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8268 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/image/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      186 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/image/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.954556 aisquared-0.3.9.dev2/aisquared/config/preprocessing/tabular/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     8761 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/tabular/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1563 2023-08-04 14:53:56.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/tabular/TabularPreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      187 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/tabular/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.955190 aisquared-0.3.9.dev2/aisquared/config/preprocessing/text/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    11803 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/text/Steps.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1740 2023-08-04 14:53:56.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/text/TextPreprocessing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      175 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/preprocessing/text/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.959243 aisquared-0.3.9.dev2/aisquared/config/rendering/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5083 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/BarChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     6083 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/ContainerRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2212 2023-09-08 16:22:26.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/CustomRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     9187 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/DashboardRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1889 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/DashboardReplacementRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4829 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/DocumentRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5053 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/DoughnutChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2666 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/FilterRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3683 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/HTMLTagRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4940 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/ImageRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5036 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/LineChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3884 2023-02-10 15:11:26.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/ObjectRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5068 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/PieChartRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1547 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/SOSRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2841 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/TableRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1320 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/TextRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     5031 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/WordRendering.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      987 2023-09-08 16:22:26.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      754 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/aisquared/config/rendering/utils.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.959495 aisquared-0.3.9.dev2/aisquared/logging/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      271 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/logging/__init__.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.961785 aisquared-0.3.9.dev2/aisquared/platform/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       49 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/platform/AISquaredAPIException.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    46109 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/platform/AISquaredPlatformClient.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       47 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/platform/NoResultsFoundError.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      375 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/platform/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      666 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/platform/additional_utils.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3539 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/platform/crudl.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3335 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/platform/feedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     2287 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/platform/metrics.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3224 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/platform/sharing.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    13405 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/platform/user_group.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.962431 aisquared-0.3.9.dev2/aisquared/serving/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1323 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/serving/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4929 2023-03-31 18:41:55.000000 aisquared-0.3.9.dev2/aisquared/serving/deploy_model.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1587 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/serving/get_remote_prediction.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.962847 aisquared-0.3.9.dev2/aisquared/utils/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      459 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/aisquared/utils/__init__.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    10636 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/aisquared/utils/utils.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.943910 aisquared-0.3.9.dev2/aisquared.egg-info/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    20526 2023-09-18 18:00:21.000000 aisquared-0.3.9.dev2/aisquared.egg-info/PKG-INFO
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3869 2023-09-18 18:00:21.000000 aisquared-0.3.9.dev2/aisquared.egg-info/SOURCES.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)        1 2023-09-18 18:00:21.000000 aisquared-0.3.9.dev2/aisquared.egg-info/dependency_links.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      101 2023-09-18 18:00:21.000000 aisquared-0.3.9.dev2/aisquared.egg-info/requires.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       10 2023-09-18 18:00:21.000000 aisquared-0.3.9.dev2/aisquared.egg-info/top_level.txt
+-rw-r--r--   0 jwrenn4    (501) staff       (20)       38 2023-09-18 18:00:21.966601 aisquared-0.3.9.dev2/setup.cfg
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1422 2023-02-24 19:53:35.000000 aisquared-0.3.9.dev2/setup.py
+drwxr-xr-x   0 jwrenn4    (501) staff       (20)        0 2023-09-18 18:00:21.965066 aisquared-0.3.9.dev2/tests/
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     4332 2023-08-04 14:53:57.000000 aisquared-0.3.9.dev2/tests/test_air.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1070 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/tests/test_analytics.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      958 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/tests/test_base.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      341 2023-03-09 19:06:33.000000 aisquared-0.3.9.dev2/tests/test_custom.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3578 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/tests/test_feedback.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     3790 2023-09-06 13:34:44.000000 aisquared-0.3.9.dev2/tests/test_harvesters.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1345 2023-05-30 14:21:20.000000 aisquared-0.3.9.dev2/tests/test_postprocessors.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)     1980 2023-07-24 12:12:58.000000 aisquared-0.3.9.dev2/tests/test_preprocessors.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)    22740 2023-09-08 16:22:26.000000 aisquared-0.3.9.dev2/tests/test_renderers.py
+-rw-r--r--   0 jwrenn4    (501) staff       (20)      107 2023-01-11 13:58:17.000000 aisquared-0.3.9.dev2/tests/test_simple.py
```

### Comparing `aisquared-0.3.9.dev1/PKG-INFO` & `aisquared-0.3.9.dev2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: aisquared
-Version: 0.3.9.dev1
-Summary: Utilities for interacting with the AI Squared Technology Stack
-Home-page: https://github.com/AISquaredInc/aisquared
-Author: The AI Squared Team
-Author-email: staff@squared.ai
-License: Apache 2.0
-Description-Content-Type: text/markdown
-Provides-Extra: full
-
 # AISquared
 
 [![Documentation](https://badgen.net/badge/icon/Documentation?icon=chrome&label)](https://aisquaredinc.github.io/aisquared/index.html)
 [![PyPI version](https://badge.fury.io/py/aisquared.svg)](https://badge.fury.io/py/aisquared)
 ![Tests](https://github.com/aisquaredinc/aisquared/actions/workflows/python-package.yml/badge.svg)
 [![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
 
@@ -347,7 +336,8 @@
 - Created `TextRendering` class
 - Changed location of reference lists of classes to clean up code
 - Updated class schemas to ensure compliance with expectations
 - Updated test cases
 
 ## Version 0.3.9
 - Added `CustomRendering` class
+- Changed to full import of `CustomObject` in `aisquared.base` subpackage
```

### Comparing `aisquared-0.3.9.dev1/README.md` & `aisquared-0.3.9.dev2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: aisquared
+Version: 0.3.9.dev2
+Summary: Utilities for interacting with the AI Squared Technology Stack
+Home-page: https://github.com/AISquaredInc/aisquared
+Author: The AI Squared Team
+Author-email: staff@squared.ai
+License: Apache 2.0
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: tensorflowjs
+Requires-Dist: tensorflow
+Requires-Dist: pandas
+Provides-Extra: full
+Requires-Dist: mlflow; extra == "full"
+Requires-Dist: flask; extra == "full"
+Requires-Dist: waitress; extra == "full"
+Requires-Dist: click; extra == "full"
+Requires-Dist: beyondml; extra == "full"
+Requires-Dist: scikit-learn; extra == "full"
+Requires-Dist: torch; extra == "full"
+
 # AISquared
 
 [![Documentation](https://badgen.net/badge/icon/Documentation?icon=chrome&label)](https://aisquaredinc.github.io/aisquared/index.html)
 [![PyPI version](https://badge.fury.io/py/aisquared.svg)](https://badge.fury.io/py/aisquared)
 ![Tests](https://github.com/aisquaredinc/aisquared/actions/workflows/python-package.yml/badge.svg)
 [![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
 
@@ -336,7 +358,8 @@
 - Created `TextRendering` class
 - Changed location of reference lists of classes to clean up code
 - Updated class schemas to ensure compliance with expectations
 - Updated test cases
 
 ## Version 0.3.9
 - Added `CustomRendering` class
+- Changed to full import of `CustomObject` in `aisquared.base` subpackage
```

### Comparing `aisquared-0.3.9.dev1/aisquared/base/BaseObject.py` & `aisquared-0.3.9.dev2/aisquared/base/BaseObject.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/base/__init__.py` & `aisquared-0.3.9.dev2/aisquared/base/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from aisquared.config.preprocessing.tabular import TabularPreprocesser
 from aisquared.config.preprocessing.image import ImagePreprocesser
 from aisquared.config.preprocessing.text import TextPreprocesser
 from aisquared.config.analytic import DeployedAnalytic, DeployedModel, LocalModel, LocalAnalytic, ReverseMLWorkflow
 from aisquared.config.postprocessing import BinaryClassification, MulticlassClassification, ObjectDetection, Regression
 from aisquared.config.rendering import ImageRendering, ObjectRendering, DocumentRendering, WordRendering, FilterRendering, ContainerRendering, HTMLTagRendering, DoughnutChartRendering, TableRendering, BarChartRendering, LineChartRendering, DashboardReplacementRendering, PieChartRendering, SOSRendering, TextRendering, CustomRendering  # , DashboardRendering
 from aisquared.config.feedback import SimpleFeedback, BinaryFeedback, MulticlassFeedback, RegressionFeedback, ModelFeedback, QualitativeFeedback
-from aisquared.config import CustomObject
+from aisquared.config.CustomObject import CustomObject
 
 HARVESTING_CLASSES = (
     ImageHarvester,
     TextHarvester,
     InputHarvester,
     QueryParameterHarvester,
     ChatbotHarvester,
@@ -77,15 +77,16 @@
 
 FEEDBACK_CLASSES = (
     ModelFeedback,
     SimpleFeedback,
     BinaryFeedback,
     MulticlassFeedback,
     RegressionFeedback,
-    QualitativeFeedback
+    QualitativeFeedback,
+    CustomObject
 )
 
 LOCAL_CLASSES = (
     LocalModel,
     LocalAnalytic,
     CustomObject
 )
```

### Comparing `aisquared-0.3.9.dev1/aisquared/base/css.py` & `aisquared-0.3.9.dev2/aisquared/base/css.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/base/endpoints.py` & `aisquared-0.3.9.dev2/aisquared/base/endpoints.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/base/rendering.py` & `aisquared-0.3.9.dev2/aisquared/base/rendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/CustomObject.py` & `aisquared-0.3.9.dev2/aisquared/config/CustomObject.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/GraphConfiguration.py` & `aisquared-0.3.9.dev2/aisquared/config/GraphConfiguration.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/ModelConfiguration.py` & `aisquared-0.3.9.dev2/aisquared/config/ModelConfiguration.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/analytic/DeployedAnalytic.py` & `aisquared-0.3.9.dev2/aisquared/config/analytic/DeployedAnalytic.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/analytic/DeployedModel.py` & `aisquared-0.3.9.dev2/aisquared/config/analytic/DeployedModel.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/analytic/LocalAnalytic.py` & `aisquared-0.3.9.dev2/aisquared/config/analytic/LocalAnalytic.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/analytic/LocalModel.py` & `aisquared-0.3.9.dev2/aisquared/config/analytic/LocalModel.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/analytic/ReverseMLWorkflow.py` & `aisquared-0.3.9.dev2/aisquared/config/analytic/ReverseMLWorkflow.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/feedback/BinaryFeedback.py` & `aisquared-0.3.9.dev2/aisquared/config/feedback/BinaryFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/feedback/ModelFeedback.py` & `aisquared-0.3.9.dev2/aisquared/config/feedback/ModelFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/feedback/MulticlassFeedback.py` & `aisquared-0.3.9.dev2/aisquared/config/feedback/MulticlassFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/feedback/QualitativeFeedback.py` & `aisquared-0.3.9.dev2/aisquared/config/feedback/QualitativeFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/feedback/RegressionFeedback.py` & `aisquared-0.3.9.dev2/aisquared/config/feedback/RegressionFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/feedback/SimpleFeedback.py` & `aisquared-0.3.9.dev2/aisquared/config/feedback/SimpleFeedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/harvesting/ChatbotHarvester.py` & `aisquared-0.3.9.dev2/aisquared/config/harvesting/ChatbotHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/harvesting/ImageHarvester.py` & `aisquared-0.3.9.dev2/aisquared/config/harvesting/ImageHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/harvesting/InputHarvester.py` & `aisquared-0.3.9.dev2/aisquared/config/harvesting/InputHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/harvesting/QueryParameterHarvester.py` & `aisquared-0.3.9.dev2/aisquared/config/harvesting/QueryParameterHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/harvesting/TextHarvester.py` & `aisquared-0.3.9.dev2/aisquared/config/harvesting/TextHarvester.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/postprocessing/BinaryClassification.py` & `aisquared-0.3.9.dev2/aisquared/config/postprocessing/BinaryClassification.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/postprocessing/MulticlassClassification.py` & `aisquared-0.3.9.dev2/aisquared/config/postprocessing/MulticlassClassification.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/postprocessing/ObjectDetection.py` & `aisquared-0.3.9.dev2/aisquared/config/postprocessing/ObjectDetection.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/postprocessing/Regression.py` & `aisquared-0.3.9.dev2/aisquared/config/postprocessing/Regression.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/preprocessing/image/ImagePreprocessing.py` & `aisquared-0.3.9.dev2/aisquared/config/preprocessing/image/ImagePreprocessing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/preprocessing/image/Steps.py` & `aisquared-0.3.9.dev2/aisquared/config/preprocessing/image/Steps.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/preprocessing/tabular/Steps.py` & `aisquared-0.3.9.dev2/aisquared/config/preprocessing/tabular/Steps.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/preprocessing/tabular/TabularPreprocessing.py` & `aisquared-0.3.9.dev2/aisquared/config/preprocessing/tabular/TabularPreprocessing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/preprocessing/text/Steps.py` & `aisquared-0.3.9.dev2/aisquared/config/preprocessing/text/Steps.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/preprocessing/text/TextPreprocessing.py` & `aisquared-0.3.9.dev2/aisquared/config/preprocessing/text/TextPreprocessing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/BarChartRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/BarChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/ContainerRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/ContainerRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/CustomRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/CustomRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/DashboardRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/DashboardRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/DashboardReplacementRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/DashboardReplacementRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/DocumentRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/DocumentRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/DoughnutChartRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/DoughnutChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/FilterRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/FilterRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/HTMLTagRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/HTMLTagRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/ImageRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/ImageRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/LineChartRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/LineChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/ObjectRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/ObjectRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/PieChartRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/PieChartRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/SOSRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/SOSRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/TableRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/TableRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/TextRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/TextRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/WordRendering.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/WordRendering.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/__init__.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/config/rendering/utils.py` & `aisquared-0.3.9.dev2/aisquared/config/rendering/utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/platform/AISquaredPlatformClient.py` & `aisquared-0.3.9.dev2/aisquared/platform/AISquaredPlatformClient.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/platform/additional_utils.py` & `aisquared-0.3.9.dev2/aisquared/platform/additional_utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/platform/crudl.py` & `aisquared-0.3.9.dev2/aisquared/platform/crudl.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/platform/feedback.py` & `aisquared-0.3.9.dev2/aisquared/platform/feedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/platform/metrics.py` & `aisquared-0.3.9.dev2/aisquared/platform/metrics.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/platform/sharing.py` & `aisquared-0.3.9.dev2/aisquared/platform/sharing.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/platform/user_group.py` & `aisquared-0.3.9.dev2/aisquared/platform/user_group.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/serving/__init__.py` & `aisquared-0.3.9.dev2/aisquared/serving/__init__.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/serving/deploy_model.py` & `aisquared-0.3.9.dev2/aisquared/serving/deploy_model.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/serving/get_remote_prediction.py` & `aisquared-0.3.9.dev2/aisquared/serving/get_remote_prediction.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared/utils/utils.py` & `aisquared-0.3.9.dev2/aisquared/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/aisquared.egg-info/PKG-INFO` & `aisquared-0.3.9.dev2/aisquared.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 Metadata-Version: 2.1
 Name: aisquared
-Version: 0.3.9.dev1
+Version: 0.3.9.dev2
 Summary: Utilities for interacting with the AI Squared Technology Stack
 Home-page: https://github.com/AISquaredInc/aisquared
 Author: The AI Squared Team
 Author-email: staff@squared.ai
 License: Apache 2.0
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: tensorflowjs
+Requires-Dist: tensorflow
+Requires-Dist: pandas
 Provides-Extra: full
+Requires-Dist: mlflow; extra == "full"
+Requires-Dist: flask; extra == "full"
+Requires-Dist: waitress; extra == "full"
+Requires-Dist: click; extra == "full"
+Requires-Dist: beyondml; extra == "full"
+Requires-Dist: scikit-learn; extra == "full"
+Requires-Dist: torch; extra == "full"
 
 # AISquared
 
 [![Documentation](https://badgen.net/badge/icon/Documentation?icon=chrome&label)](https://aisquaredinc.github.io/aisquared/index.html)
 [![PyPI version](https://badge.fury.io/py/aisquared.svg)](https://badge.fury.io/py/aisquared)
 ![Tests](https://github.com/aisquaredinc/aisquared/actions/workflows/python-package.yml/badge.svg)
 [![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
@@ -347,7 +358,8 @@
 - Created `TextRendering` class
 - Changed location of reference lists of classes to clean up code
 - Updated class schemas to ensure compliance with expectations
 - Updated test cases
 
 ## Version 0.3.9
 - Added `CustomRendering` class
+- Changed to full import of `CustomObject` in `aisquared.base` subpackage
```

### Comparing `aisquared-0.3.9.dev1/aisquared.egg-info/SOURCES.txt` & `aisquared-0.3.9.dev2/aisquared.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/setup.py` & `aisquared-0.3.9.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/tests/test_air.py` & `aisquared-0.3.9.dev2/tests/test_air.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/tests/test_analytics.py` & `aisquared-0.3.9.dev2/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/tests/test_base.py` & `aisquared-0.3.9.dev2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/tests/test_feedback.py` & `aisquared-0.3.9.dev2/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/tests/test_harvesters.py` & `aisquared-0.3.9.dev2/tests/test_harvesters.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/tests/test_postprocessors.py` & `aisquared-0.3.9.dev2/tests/test_postprocessors.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/tests/test_preprocessors.py` & `aisquared-0.3.9.dev2/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `aisquared-0.3.9.dev1/tests/test_renderers.py` & `aisquared-0.3.9.dev2/tests/test_renderers.py`

 * *Files identical despite different names*


# Comparing `tmp/msa_toolbox-0.0.2.tar.gz` & `tmp/msa_toolbox-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msa_toolbox-0.0.2.tar", last modified: Tue Jan 31 09:32:00 2023, max compression
+gzip compressed data, was "msa_toolbox-1.0.2.tar", last modified: Wed May  8 09:18:04 2024, max compression
```

## Comparing `msa_toolbox-0.0.2.tar` & `msa_toolbox-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 09:32:00.614011 msa_toolbox-0.0.2/
--rw-rw-rw-   0        0        0      568 2023-01-31 09:32:00.612926 msa_toolbox-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-01-31 07:50:42.000000 msa_toolbox-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-31 09:32:00.594207 msa_toolbox-0.0.2/msa_toolbox/
--rw-rw-rw-   0        0        0       23 2023-01-31 09:23:18.000000 msa_toolbox-0.0.2/msa_toolbox/__init__.py
--rw-rw-rw-   0        0        0       56 2023-01-31 09:20:13.000000 msa_toolbox-0.0.2/msa_toolbox/hello.py
-drwxrwxrwx   0        0        0        0 2023-01-31 09:32:00.610241 msa_toolbox-0.0.2/msa_toolbox.egg-info/
--rw-rw-rw-   0        0        0      568 2023-01-31 09:32:00.000000 msa_toolbox-0.0.2/msa_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-01-31 09:32:00.000000 msa_toolbox-0.0.2/msa_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 09:32:00.000000 msa_toolbox-0.0.2/msa_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-01-31 09:32:00.000000 msa_toolbox-0.0.2/msa_toolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-31 09:32:00.615600 msa_toolbox-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1000 2023-01-31 09:31:47.000000 msa_toolbox-0.0.2/setup.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.666166 msa_toolbox-1.0.2/
+-rw-r--r--   0 sumdev    (1004) sumdev    (1004)     3499 2024-05-08 09:18:04.666166 msa_toolbox-1.0.2/PKG-INFO
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)      404 2024-05-08 08:35:48.000000 msa_toolbox-1.0.2/README.md
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)       39 2023-09-09 15:59:47.000000 msa_toolbox-1.0.2/msa_toolbox/__init__.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/active_learning/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)       13 2023-09-09 19:38:47.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     9935 2024-04-15 17:41:26.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/active_learning_main.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     8430 2024-03-14 08:10:01.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/active_learning_main_api.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     4035 2024-04-15 17:42:27.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/active_learning_methods.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/active_learning/dfal/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-10-31 08:37:55.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/dfal/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     6796 2024-04-15 18:02:26.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/dfal/dfal_method.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/active_learning/entropy/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-06 05:24:57.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/entropy/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     6365 2024-03-21 06:24:53.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/entropy/entropy_method.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/active_learning/kcenter/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-10-23 13:16:21.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/kcenter/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     7258 2023-11-25 10:05:47.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/kcenter/kcenter_greedy.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     5287 2024-04-15 17:21:42.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/kcenter/kcenter_method.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     1332 2023-10-30 13:15:30.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/kcenter/utils.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/active_learning/montecarlo/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-09 19:38:33.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/montecarlo/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     7573 2024-03-21 06:26:08.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/montecarlo/montecarlo_method.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/active_learning/random/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-10 09:07:29.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/random/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     4989 2024-03-21 06:29:54.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/random/random_method.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/active_learning/vaal/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-06 05:24:57.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/vaal/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)    10382 2024-04-15 17:46:05.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/vaal/vaal_method.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     4530 2023-11-25 19:16:39.000000 msa_toolbox-1.0.2/msa_toolbox/active_learning/vaal/vaal_models.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)      862 2023-11-25 10:12:14.000000 msa_toolbox-1.0.2/msa_toolbox/config.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/datasets/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-09 15:42:30.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/__init__.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/datasets/image/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     5816 2023-09-06 05:15:44.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     5931 2023-11-25 10:06:54.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/caltech256.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     7277 2024-02-12 07:28:16.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/cifar.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     5212 2023-11-25 10:07:05.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/cubs200.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     1757 2023-11-25 10:07:07.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/custom_dataset.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     4199 2023-11-25 10:07:09.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/diabetic5.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     3779 2023-11-25 10:07:11.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/imagenet.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     3095 2023-11-25 10:07:13.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/indoor67.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     7898 2024-02-12 07:28:41.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/mnist.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     2692 2023-11-25 10:07:18.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/svhn.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     2493 2023-11-25 10:07:20.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/image/tinyimagenet200.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.658166 msa_toolbox-1.0.2/msa_toolbox/datasets/text/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-06 05:15:44.000000 msa_toolbox-1.0.2/msa_toolbox/datasets/text/__init__.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/defence/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-11-15 06:50:37.000000 msa_toolbox-1.0.2/msa_toolbox/defence/__init__.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/defence/adaptive_misinformation/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2024-04-13 16:47:21.000000 msa_toolbox-1.0.2/msa_toolbox/defence/adaptive_misinformation/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     1730 2024-04-15 17:38:35.000000 msa_toolbox-1.0.2/msa_toolbox/defence/adaptive_misinformation/adaptive_misinformation.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     1173 2024-04-13 16:52:08.000000 msa_toolbox-1.0.2/msa_toolbox/defence/defence_main.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     1391 2024-03-14 06:01:49.000000 msa_toolbox-1.0.2/msa_toolbox/defence/defence_main_api.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/defence/no_defence/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-11-15 13:48:32.000000 msa_toolbox-1.0.2/msa_toolbox/defence/no_defence/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     1481 2023-11-25 10:10:11.000000 msa_toolbox-1.0.2/msa_toolbox/defence/no_defence/no_defence.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     4821 2024-03-29 08:50:43.000000 msa_toolbox-1.0.2/msa_toolbox/defence/no_defence/no_defence_clarifai_api.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     2788 2024-03-29 08:54:17.000000 msa_toolbox-1.0.2/msa_toolbox/defence/no_defence/no_defence_huggingface_api.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/defence/prada/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-11-15 13:48:38.000000 msa_toolbox-1.0.2/msa_toolbox/defence/prada/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     3626 2024-04-15 17:48:42.000000 msa_toolbox-1.0.2/msa_toolbox/defence/prada/growing_distance_agent.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     3037 2023-11-25 10:10:03.000000 msa_toolbox-1.0.2/msa_toolbox/defence/prada/prada.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     2046 2024-03-14 05:54:55.000000 msa_toolbox-1.0.2/msa_toolbox/main.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/models/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-09 15:57:56.000000 msa_toolbox-1.0.2/msa_toolbox/models/__init__.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/models/image/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)      213 2023-09-06 05:15:44.000000 msa_toolbox-1.0.2/msa_toolbox/models/image/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     1609 2023-09-06 05:15:44.000000 msa_toolbox-1.0.2/msa_toolbox/models/image/alexnet.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     4421 2023-09-06 05:15:44.000000 msa_toolbox-1.0.2/msa_toolbox/models/image/densenet.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)    11929 2023-11-25 10:10:33.000000 msa_toolbox-1.0.2/msa_toolbox/models/image/efficientnet.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     4669 2023-09-06 05:15:44.000000 msa_toolbox-1.0.2/msa_toolbox/models/image/efficientnet_v2.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     1697 2023-11-25 10:10:35.000000 msa_toolbox-1.0.2/msa_toolbox/models/image/mobilenet_v2.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     3267 2023-11-25 10:10:37.000000 msa_toolbox-1.0.2/msa_toolbox/models/image/mobilenet_v3.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     7738 2023-11-25 10:10:39.000000 msa_toolbox-1.0.2/msa_toolbox/models/image/resnet.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)    11143 2023-11-25 10:10:41.000000 msa_toolbox-1.0.2/msa_toolbox/models/image/vgg.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/models/text/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-06 05:15:44.000000 msa_toolbox-1.0.2/msa_toolbox/models/text/__init__.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/utils/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-09 15:41:45.000000 msa_toolbox-1.0.2/msa_toolbox/utils/__init__.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/utils/image/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)      581 2023-09-06 05:15:44.000000 msa_toolbox-1.0.2/msa_toolbox/utils/image/__init__.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)    12840 2024-03-18 06:53:46.000000 msa_toolbox-1.0.2/msa_toolbox/utils/image/all_logs.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     1661 2023-11-25 10:11:44.000000 msa_toolbox-1.0.2/msa_toolbox/utils/image/cfg_reader.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)    16874 2023-11-25 10:11:48.000000 msa_toolbox-1.0.2/msa_toolbox/utils/image/load_data_and_models.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     4483 2024-04-15 06:56:01.000000 msa_toolbox-1.0.2/msa_toolbox/utils/image/load_victim_thief_data_and_model.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     4179 2023-11-25 10:11:55.000000 msa_toolbox-1.0.2/msa_toolbox/utils/image/loss_criterion.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     3169 2023-11-25 10:12:04.000000 msa_toolbox-1.0.2/msa_toolbox/utils/image/optimizer.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     9091 2023-11-25 10:12:02.000000 msa_toolbox-1.0.2/msa_toolbox/utils/image/train_model.py
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     3904 2024-04-15 17:12:20.000000 msa_toolbox-1.0.2/msa_toolbox/utils/image/train_utils.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox/utils/text/
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        0 2023-09-06 05:15:44.000000 msa_toolbox-1.0.2/msa_toolbox/utils/text/__init__.py
+drwxrwxr-x   0 sumdev    (1004) sumdev    (1004)        0 2024-05-08 09:18:04.662166 msa_toolbox-1.0.2/msa_toolbox.egg-info/
+-rw-r--r--   0 sumdev    (1004) sumdev    (1004)     3499 2024-05-08 09:18:04.000000 msa_toolbox-1.0.2/msa_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     3169 2024-05-08 09:18:04.000000 msa_toolbox-1.0.2/msa_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)        1 2024-05-08 09:18:04.000000 msa_toolbox-1.0.2/msa_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)       60 2024-05-08 09:18:04.000000 msa_toolbox-1.0.2/msa_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)      620 2024-05-08 09:18:04.000000 msa_toolbox-1.0.2/msa_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)       12 2024-05-08 09:18:04.000000 msa_toolbox-1.0.2/msa_toolbox.egg-info/top_level.txt
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)       38 2024-05-08 09:18:04.666166 msa_toolbox-1.0.2/setup.cfg
+-rw-rw-r--   0 sumdev    (1004) sumdev    (1004)     2482 2024-05-08 09:13:50.000000 msa_toolbox-1.0.2/setup.py
```

